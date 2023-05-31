# Comparing `tmp/pyjls-0.6.3.tar.gz` & `tmp/pyjls-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.6.3.tar", last modified: Tue May 16 19:15:22 2023, max compression
+gzip compressed data, was "pyjls-0.7.0.tar", last modified: Wed May 31 12:16:00 2023, max compression
```

## Comparing `pyjls-0.6.3.tar` & `pyjls-0.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.164675 pyjls-0.6.3/
--rw-rw-rw-   0        0        0     4555 2023-05-16 18:49:16.000000 pyjls-0.6.3/CHANGELOG.md
--rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.6.3/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.6.3/LICENSE
--rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0    14665 2023-05-16 19:15:22.164166 pyjls-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.102898 pyjls-0.6.3/include/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.108406 pyjls-0.6.3/include/jls/
--rw-rw-rw-   0        0        0     2745 2023-05-16 17:33:09.000000 pyjls-0.6.3/include/jls/backend.h
--rw-rw-rw-   0        0        0     2103 2023-05-16 17:35:22.000000 pyjls-0.6.3/include/jls/cmacro.h
--rw-rw-rw-   0        0        0     1593 2023-05-16 18:43:43.000000 pyjls-0.6.3/include/jls/crc32c.h
--rw-rw-rw-   0        0        0     4080 2023-05-16 18:43:53.000000 pyjls-0.6.3/include/jls/ec.h
--rw-rw-rw-   0        0        0    24468 2023-04-26 11:42:25.000000 pyjls-0.6.3/include/jls/format.h
--rw-rw-rw-   0        0        0    11561 2023-04-26 14:23:01.000000 pyjls-0.6.3/include/jls/log.h
--rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.6.3/include/jls/raw.h
--rw-rw-rw-   0        0        0    10319 2023-04-26 17:43:17.000000 pyjls-0.6.3/include/jls/reader.h
--rw-rw-rw-   0        0        0     4213 2023-05-16 18:44:44.000000 pyjls-0.6.3/include/jls/statistics.h
--rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.6.3/include/jls/threaded_writer.h
--rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.6.3/include/jls/time.h
--rw-rw-rw-   0        0        0     2760 2023-05-16 18:46:48.000000 pyjls-0.6.3/include/jls/version.h
--rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.6.3/include/jls/writer.h
--rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.6.3/include/jls.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.094388 pyjls-0.6.3/include_prv/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.111919 pyjls-0.6.3/include_prv/jls/
--rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.6.3/include_prv/jls/bit_shift.h
--rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.6.3/include_prv/jls/cdef.h
--rw-rw-rw-   0        0        0     1524 2022-03-07 15:46:24.000000 pyjls-0.6.3/include_prv/jls/datatype.h
--rw-rw-rw-   0        0        0     2676 2022-03-05 19:14:45.000000 pyjls-0.6.3/include_prv/jls/msg_ring_buffer.h
--rw-rw-rw-   0        0        0     1784 2023-04-26 18:12:34.000000 pyjls-0.6.3/include_prv/jls/rd_fsr.h
--rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.6.3/include_prv/jls/util.h
--rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.6.3/include_prv/jls/wr_fsr.h
--rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.6.3/include_prv/jls/wr_prv.h
--rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.6.3/include_prv/jls/wr_ts.h
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.120945 pyjls-0.6.3/pyjls/
--rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.6.3/pyjls/__init__.py
--rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.6.3/pyjls/__main__.py
--rw-rw-rw-   0        0        0  1587118 2023-04-26 19:59:45.000000 pyjls-0.6.3/pyjls/binding.c
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.132509 pyjls-0.6.3/pyjls/entry_points/
--rw-rw-rw-   0        0        0      869 2023-04-28 18:19:13.000000 pyjls-0.6.3/pyjls/entry_points/__init__.py
--rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.6.3/pyjls/entry_points/annotate.py
--rw-rw-rw-   0        0        0     2561 2023-04-28 18:26:31.000000 pyjls-0.6.3/pyjls/entry_points/export.py
--rw-rw-rw-   0        0        0     2019 2023-04-28 12:29:04.000000 pyjls-0.6.3/pyjls/entry_points/info.py
--rw-rw-rw-   0        0        0     2333 2023-04-28 12:48:59.000000 pyjls-0.6.3/pyjls/structs.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.133508 pyjls-0.6.3/pyjls/test/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.3/pyjls/test/__init__.py
--rw-rw-rw-   0        0        0    10313 2023-04-26 19:18:13.000000 pyjls-0.6.3/pyjls/test/test_binding.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.134012 pyjls-0.6.3/pyjls/v1/
--rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.6.3/pyjls/v1/__init__.py
--rw-rw-rw-   0        0        0     1059 2023-05-16 18:46:48.000000 pyjls-0.6.3/pyjls/version.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.130464 pyjls-0.6.3/pyjls.egg-info/
--rw-rw-rw-   0        0        0    14665 2023-05-16 19:15:22.000000 pyjls-0.6.3/pyjls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1339 2023-05-16 19:15:22.000000 pyjls-0.6.3/pyjls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:15:22.000000 pyjls-0.6.3/pyjls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-16 19:15:22.000000 pyjls-0.6.3/pyjls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2023-05-16 19:15:22.000000 pyjls-0.6.3/pyjls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 19:15:22.000000 pyjls-0.6.3/pyjls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 19:15:22.164675 pyjls-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     6742 2023-04-27 15:16:07.000000 pyjls-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:15:22.162663 pyjls-0.6.3/src/
--rw-rw-rw-   0        0        0     8684 2023-04-19 20:32:02.000000 pyjls-0.6.3/src/backend_posix.c
--rw-rw-rw-   0        0        0     9046 2023-05-16 17:32:59.000000 pyjls-0.6.3/src/backend_win.c
--rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.6.3/src/bit_shift.c
--rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.6.3/src/crc32c_arm_neon.c
--rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.6.3/src/crc32c_intel_sse4.c
--rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.6.3/src/crc32c_sw.c
--rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.6.3/src/datatype.c
--rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.6.3/src/ec.c
--rw-rw-rw-   0        0        0     1631 2023-04-19 17:02:27.000000 pyjls-0.6.3/src/log.c
--rw-rw-rw-   0        0        0     3970 2022-03-07 15:46:24.000000 pyjls-0.6.3/src/msg_ring_buffer.c
--rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.6.3/src/raw.c
--rw-rw-rw-   0        0        0     5903 2023-04-26 19:35:45.000000 pyjls-0.6.3/src/rd_fsr.c
--rw-rw-rw-   0        0        0    54650 2023-04-28 12:42:07.000000 pyjls-0.6.3/src/reader.c
--rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.6.3/src/statistics.c
--rw-rw-rw-   0        0        0    11622 2023-04-27 15:21:50.000000 pyjls-0.6.3/src/threaded_writer.c
--rw-rw-rw-   0        0        0    27815 2023-04-28 18:27:16.000000 pyjls-0.6.3/src/wr_fsr.c
--rw-rw-rw-   0        0        0     9691 2023-04-26 14:57:54.000000 pyjls-0.6.3/src/wr_ts.c
--rw-rw-rw-   0        0        0    30342 2023-04-26 12:23:06.000000 pyjls-0.6.3/src/writer.c
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.371623 pyjls-0.7.0/
+-rw-rw-rw-   0        0        0     5165 2023-05-31 11:39:34.000000 pyjls-0.7.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     3039 2021-03-18 16:48:36.000000 pyjls-0.7.0/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2018-07-03 17:53:12.000000 pyjls-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0      177 2021-03-10 13:52:18.000000 pyjls-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    14665 2023-05-31 12:16:00.371120 pyjls-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13054 2022-03-07 15:46:24.000000 pyjls-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.232833 pyjls-0.7.0/include/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.276142 pyjls-0.7.0/include/jls/
+-rw-rw-rw-   0        0        0     2745 2023-05-16 17:33:09.000000 pyjls-0.7.0/include/jls/backend.h
+-rw-rw-rw-   0        0        0     2103 2023-05-16 17:35:22.000000 pyjls-0.7.0/include/jls/cmacro.h
+-rw-rw-rw-   0        0        0     1593 2023-05-16 18:43:43.000000 pyjls-0.7.0/include/jls/crc32c.h
+-rw-rw-rw-   0        0        0     4080 2023-05-16 18:43:53.000000 pyjls-0.7.0/include/jls/ec.h
+-rw-rw-rw-   0        0        0    24468 2023-04-26 11:42:25.000000 pyjls-0.7.0/include/jls/format.h
+-rw-rw-rw-   0        0        0    12016 2023-05-30 20:46:47.000000 pyjls-0.7.0/include/jls/log.h
+-rw-rw-rw-   0        0        0     6351 2022-03-05 19:14:45.000000 pyjls-0.7.0/include/jls/raw.h
+-rw-rw-rw-   0        0        0    10319 2023-04-26 17:43:17.000000 pyjls-0.7.0/include/jls/reader.h
+-rw-rw-rw-   0        0        0     4213 2023-05-16 18:44:44.000000 pyjls-0.7.0/include/jls/statistics.h
+-rw-rw-rw-   0        0        0     2561 2022-03-05 19:14:45.000000 pyjls-0.7.0/include/jls/threaded_writer.h
+-rw-rw-rw-   0        0        0    12420 2023-04-19 20:31:02.000000 pyjls-0.7.0/include/jls/time.h
+-rw-rw-rw-   0        0        0     2760 2023-05-31 11:39:40.000000 pyjls-0.7.0/include/jls/version.h
+-rw-rw-rw-   0        0        0     5775 2022-03-05 19:14:45.000000 pyjls-0.7.0/include/jls/writer.h
+-rw-rw-rw-   0        0        0      895 2022-03-05 19:14:45.000000 pyjls-0.7.0/include/jls.h
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.217743 pyjls-0.7.0/include_prv/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.302849 pyjls-0.7.0/include_prv/jls/
+-rw-rw-rw-   0        0        0     1385 2022-03-07 15:46:24.000000 pyjls-0.7.0/include_prv/jls/bit_shift.h
+-rw-rw-rw-   0        0        0     2099 2022-03-05 19:14:45.000000 pyjls-0.7.0/include_prv/jls/cdef.h
+-rw-rw-rw-   0        0        0     1524 2023-05-27 15:49:14.000000 pyjls-0.7.0/include_prv/jls/datatype.h
+-rw-rw-rw-   0        0        0     2951 2023-05-25 18:56:38.000000 pyjls-0.7.0/include_prv/jls/msg_ring_buffer.h
+-rw-rw-rw-   0        0        0     1784 2023-04-26 18:12:34.000000 pyjls-0.7.0/include_prv/jls/rd_fsr.h
+-rw-rw-rw-   0        0        0     1276 2022-03-05 19:14:45.000000 pyjls-0.7.0/include_prv/jls/util.h
+-rw-rw-rw-   0        0        0     1945 2022-03-05 19:14:45.000000 pyjls-0.7.0/include_prv/jls/wr_fsr.h
+-rw-rw-rw-   0        0        0     1744 2022-03-05 19:14:45.000000 pyjls-0.7.0/include_prv/jls/wr_prv.h
+-rw-rw-rw-   0        0        0     3042 2022-03-05 19:14:45.000000 pyjls-0.7.0/include_prv/jls/wr_ts.h
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.308853 pyjls-0.7.0/pyjls/
+-rw-rw-rw-   0        0        0     1208 2023-03-04 20:14:09.000000 pyjls-0.7.0/pyjls/__init__.py
+-rw-rw-rw-   0        0        0     2557 2022-03-05 19:14:45.000000 pyjls-0.7.0/pyjls/__main__.py
+-rw-rw-rw-   0        0        0  1610185 2023-05-31 12:03:55.000000 pyjls-0.7.0/pyjls/binding.c
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.318165 pyjls-0.7.0/pyjls/entry_points/
+-rw-rw-rw-   0        0        0      869 2023-04-28 18:19:13.000000 pyjls-0.7.0/pyjls/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     2738 2022-03-05 19:14:45.000000 pyjls-0.7.0/pyjls/entry_points/annotate.py
+-rw-rw-rw-   0        0        0     2561 2023-04-28 18:26:31.000000 pyjls-0.7.0/pyjls/entry_points/export.py
+-rw-rw-rw-   0        0        0     2019 2023-04-28 12:29:04.000000 pyjls-0.7.0/pyjls/entry_points/info.py
+-rw-rw-rw-   0        0        0     2333 2023-04-28 12:48:59.000000 pyjls-0.7.0/pyjls/structs.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.319165 pyjls-0.7.0/pyjls/test/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.7.0/pyjls/test/__init__.py
+-rw-rw-rw-   0        0        0    10313 2023-04-26 19:18:13.000000 pyjls-0.7.0/pyjls/test/test_binding.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.319165 pyjls-0.7.0/pyjls/v1/
+-rw-rw-rw-   0        0        0      594 2022-03-05 19:14:45.000000 pyjls-0.7.0/pyjls/v1/__init__.py
+-rw-rw-rw-   0        0        0     1059 2023-05-31 11:39:40.000000 pyjls-0.7.0/pyjls/version.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.317166 pyjls-0.7.0/pyjls.egg-info/
+-rw-rw-rw-   0        0        0    14665 2023-05-31 12:16:00.000000 pyjls-0.7.0/pyjls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1339 2023-05-31 12:16:00.000000 pyjls-0.7.0/pyjls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:16:00.000000 pyjls-0.7.0/pyjls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-31 12:16:00.000000 pyjls-0.7.0/pyjls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2023-05-31 12:16:00.000000 pyjls-0.7.0/pyjls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 12:16:00.000000 pyjls-0.7.0/pyjls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2022-11-30 13:53:49.000000 pyjls-0.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 12:16:00.371623 pyjls-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     6742 2023-04-27 15:16:07.000000 pyjls-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:16:00.370120 pyjls-0.7.0/src/
+-rw-rw-rw-   0        0        0     8684 2023-05-25 21:22:49.000000 pyjls-0.7.0/src/backend_posix.c
+-rw-rw-rw-   0        0        0     9046 2023-05-25 21:36:14.000000 pyjls-0.7.0/src/backend_win.c
+-rw-rw-rw-   0        0        0     1179 2022-03-07 15:46:24.000000 pyjls-0.7.0/src/bit_shift.c
+-rw-rw-rw-   0        0        0     1855 2022-03-05 19:14:45.000000 pyjls-0.7.0/src/crc32c_arm_neon.c
+-rw-rw-rw-   0        0        0     2433 2022-03-05 19:14:45.000000 pyjls-0.7.0/src/crc32c_intel_sse4.c
+-rw-rw-rw-   0        0        0    33673 2022-03-05 19:14:45.000000 pyjls-0.7.0/src/crc32c_sw.c
+-rw-rw-rw-   0        0        0     3589 2022-03-07 15:46:24.000000 pyjls-0.7.0/src/datatype.c
+-rw-rw-rw-   0        0        0     1113 2022-03-05 19:14:45.000000 pyjls-0.7.0/src/ec.c
+-rw-rw-rw-   0        0        0     2132 2023-05-26 20:12:15.000000 pyjls-0.7.0/src/log.c
+-rw-rw-rw-   0        0        0     4190 2023-05-25 18:57:18.000000 pyjls-0.7.0/src/msg_ring_buffer.c
+-rw-rw-rw-   0        0        0    17311 2023-04-19 20:32:58.000000 pyjls-0.7.0/src/raw.c
+-rw-rw-rw-   0        0        0     5903 2023-04-26 19:35:45.000000 pyjls-0.7.0/src/rd_fsr.c
+-rw-rw-rw-   0        0        0    55073 2023-05-30 20:41:26.000000 pyjls-0.7.0/src/reader.c
+-rw-rw-rw-   0        0        0     4302 2022-03-05 19:14:45.000000 pyjls-0.7.0/src/statistics.c
+-rw-rw-rw-   0        0        0    12778 2023-05-26 17:57:32.000000 pyjls-0.7.0/src/threaded_writer.c
+-rw-rw-rw-   0        0        0    28085 2023-05-30 20:38:15.000000 pyjls-0.7.0/src/wr_fsr.c
+-rw-rw-rw-   0        0        0     9691 2023-04-26 14:57:54.000000 pyjls-0.7.0/src/wr_ts.c
+-rw-rw-rw-   0        0        0    30342 2023-04-26 12:23:06.000000 pyjls-0.7.0/src/writer.c
```

### Comparing `pyjls-0.6.3/CHANGELOG.md` & `pyjls-0.7.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the JLS project.
 
 
+## 0.7.0
+
+2023 May 31
+
+* Fixed incorrect write timestamp stride in FSR index/summary entries.
+  Any recording over 5.77 hours was incorrect. 
+* Improved threaded writer.
+  * Removed jls_wr_flush during close due to UI performance problems.
+  * Release the GIL on some python Writer operations.
+  * Reduced buffer size from 100,000,000 B to 64 MB. 
+  * Save string null termination byte for annotations and user_data.
+  * Increased thread priority on Windows.
+  * Do not quit until all messages are processed.
+* Added jls executable to examples.
+* Improved reader logging and error handling.
+
+
 ## 0.6.3
 
 2023 May 16
 
 * Added support for building a shared library.
   Initialize build subdir with "cmake -DBUILD_SHARED_LIBS=ON .."
```

### Comparing `pyjls-0.6.3/CREDITS.html` & `pyjls-0.7.0/CREDITS.html`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/LICENSE` & `pyjls-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/PKG-INFO` & `pyjls-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.6.3
+Version: 0.7.0
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.6.3/README.md` & `pyjls-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/backend.h` & `pyjls-0.7.0/include/jls/backend.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/cmacro.h` & `pyjls-0.7.0/include/jls/cmacro.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/crc32c.h` & `pyjls-0.7.0/include/jls/crc32c.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/ec.h` & `pyjls-0.7.0/include/jls/ec.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/format.h` & `pyjls-0.7.0/include/jls/format.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/log.h` & `pyjls-0.7.0/include/jls/log.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
  * \brief Trivial logging support.
  */
 
 #ifndef JLS_LOG_H_
 #define JLS_LOG_H_
 
 #include "jls/cmacro.h"
+#include <stdint.h>
 
 /**
  * @ingroup jls
  * @defgroup jls_log Console logging
  *
  * @brief Generic console logging with compile-time levels.
  *
@@ -197,14 +198,30 @@
 
 /**
  * @brief Map log level to a single character.
  */
 extern char const jls_log_level_char[JLS_LOG_LEVEL_ALL + 1];
 
 /**
+ * @brief Convert a log level to a user-meaningful string description.
+ *
+ * @param level The log level.
+ * @return The string description.
+ */
+JLS_API const char * jsdrv_log_level_to_str(int8_t level);
+
+/**
+ * @brief Convert a log level to a user-meaningful character.
+ *
+ * @param level The log level.
+ * @return The character representing the log level.
+ */
+JLS_API char jsdrv_log_level_to_char(int8_t level);
+
+/**
  * @brief Check the current level against the static logging configuration.
  *
  * @param level The level to query.
  * @return True if logging at level is permitted.
  */
 #define JLS_LOG_CHECK_STATIC(level) ((level <= JLS_LOG_GLOBAL_LEVEL) && (level <= JLS_LOG_LEVEL) && (level >= 0))
```

### Comparing `pyjls-0.6.3/include/jls/raw.h` & `pyjls-0.7.0/include/jls/raw.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/reader.h` & `pyjls-0.7.0/include/jls/reader.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/statistics.h` & `pyjls-0.7.0/include/jls/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/threaded_writer.h` & `pyjls-0.7.0/include/jls/threaded_writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/time.h` & `pyjls-0.7.0/include/jls/time.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls/version.h` & `pyjls-0.7.0/include/jls/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
  * @{
  */
 
 JLS_CPP_GUARD_START
 
 // Use version_update.py to update.
 #define JLS_VERSION_MAJOR 0
-#define JLS_VERSION_MINOR 6
-#define JLS_VERSION_PATCH 3
+#define JLS_VERSION_MINOR 7
+#define JLS_VERSION_PATCH 0
 
 /**
  * \brief Macro to encode version to uint32_t.
  *
  * \param major The major release number (0 to 255)
  * \param minor The minor release number (0 to 255)
  * \param patch The patch release number (0 to 65535)
```

### Comparing `pyjls-0.6.3/include/jls/writer.h` & `pyjls-0.7.0/include/jls/writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include/jls.h` & `pyjls-0.7.0/include/jls.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include_prv/jls/bit_shift.h` & `pyjls-0.7.0/include_prv/jls/bit_shift.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include_prv/jls/cdef.h` & `pyjls-0.7.0/include_prv/jls/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include_prv/jls/datatype.h` & `pyjls-0.7.0/include_prv/jls/datatype.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include_prv/jls/msg_ring_buffer.h` & `pyjls-0.7.0/include_prv/jls/msg_ring_buffer.h`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 extern "C" {
 #endif
 
 /// The message ring buffer instance.
 struct jls_mrb_s {
     volatile uint32_t head;
     volatile uint32_t tail;
-    volatile uint32_t count;
+    volatile uint32_t count;    ///< number of messages
     uint8_t * buf;
     uint32_t buf_size;  // Size of buf in bytes
 };
 
 /**
  * @brief Initialize the message ring buffer.
  *
@@ -61,14 +61,22 @@
  * @brief Clear all data from the memory buffer.
  *
  * @param self The ring buffer instance.
  */
 void jls_mrb_clear(struct jls_mrb_s * self);
 
 /**
+ * @brief Get the amount of buffer used, in bytes.
+ * @param self The ring buffer instance.
+ * @return The number of bytes used.
+ * @see self->count for the number of messages.
+ */
+uint32_t jls_mrb_used_bytes(struct jls_mrb_s * self);
+
+/**
  * @brief Allocate a message on the ring buffer.
  *
  * @param self The ring buffer instance.
  * @param size The desired size of the buffer.
  * @return The buffer or NULL on out of space.
  */
 uint8_t * jls_mrb_alloc(struct jls_mrb_s * self, uint32_t size);
```

### Comparing `pyjls-0.6.3/include_prv/jls/rd_fsr.h` & `pyjls-0.7.0/include_prv/jls/rd_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include_prv/jls/util.h` & `pyjls-0.7.0/include_prv/jls/util.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include_prv/jls/wr_fsr.h` & `pyjls-0.7.0/include_prv/jls/wr_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include_prv/jls/wr_prv.h` & `pyjls-0.7.0/include_prv/jls/wr_prv.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/include_prv/jls/wr_ts.h` & `pyjls-0.7.0/include_prv/jls/wr_ts.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/__init__.py` & `pyjls-0.7.0/pyjls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/__main__.py` & `pyjls-0.7.0/pyjls/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/binding.c` & `pyjls-0.7.0/pyjls/binding.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\bin\\Python3_8_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
             "C:\\bin\\Python3_8_10\\lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
@@ -44,16 +44,16 @@
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
@@ -113,16 +113,20 @@
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
@@ -1397,43 +1401,43 @@
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "pyjls/binding.pyx":252
+/* "pyjls/binding.pyx":254
  * 
  * 
  * cdef class Writer:             # <<<<<<<<<<<<<<
  *     cdef c_jls.jls_twr_s * _wr
  *     cdef c_jls.jls_signal_def_s _signals[_JLS_SIGNAL_COUNT]
  */
 struct __pyx_obj_5pyjls_7binding_Writer {
   PyObject_HEAD
   struct jls_twr_s *_wr;
   struct jls_signal_def_s _signals[0x100];
 };
 
 
-/* "pyjls/binding.pyx":391
+/* "pyjls/binding.pyx":440
  * 
  * 
  * cdef class AnnotationCallback:             # <<<<<<<<<<<<<<
  *     cdef uint8_t is_fsr
  *     cdef object cbk_fn
  */
 struct __pyx_obj_5pyjls_7binding_AnnotationCallback {
   PyObject_HEAD
   uint8_t is_fsr;
   PyObject *cbk_fn;
 };
 
 
-/* "pyjls/binding.pyx":400
+/* "pyjls/binding.pyx":449
  * 
  * 
  * cdef class Reader:             # <<<<<<<<<<<<<<
  *     cdef c_jls.jls_rd_s * _rd
  *     cdef object _sources
  */
 struct __pyx_obj_5pyjls_7binding_Reader {
@@ -1923,14 +1927,17 @@
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* BufferIndexError.proto */
 static void __Pyx_RaiseBufferIndexError(int axis);
 
+/* BufferIndexErrorNogil.proto */
+static void __Pyx_RaiseBufferIndexErrorNogil(int axis);
+
 /* MemviewSliceInit.proto */
 #define __Pyx_BUF_MAX_NDIMS %(BUF_MAX_NDIMS)d
 #define __Pyx_MEMVIEW_DIRECT   1
 #define __Pyx_MEMVIEW_PTR      2
 #define __Pyx_MEMVIEW_FULL     4
 #define __Pyx_MEMVIEW_CONTIG   8
 #define __Pyx_MEMVIEW_STRIDED  16
@@ -2001,17 +2008,14 @@
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
-/* BufferIndexErrorNogil.proto */
-static void __Pyx_RaiseBufferIndexErrorNogil(int axis);
-
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
@@ -2167,30 +2171,30 @@
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
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? _PyDict_SetItem_KnownHash(ns, name, value, ((PyASCIIObject *) name)->hash) : PyObject_SetItem(ns, name, value))
 #elif CYTHON_COMPILING_IN_CPYTHON
@@ -2294,14 +2298,17 @@
                 int ndim,
                 __Pyx_TypeInfo *dtype,
                 __Pyx_BufFmt_StackElem stack[],
                 __Pyx_memviewslice *memviewslice,
                 PyObject *original_obj);
 
 /* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(PyObject *, int writable_flag);
+
+/* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5numpy_float64_t(PyObject *, int writable_flag);
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
@@ -2440,20 +2447,20 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE uint32_t __Pyx_PyInt_As_uint32_t(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE enum jls_storage_type_e __Pyx_PyInt_As_enum__jls_storage_type_e(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE enum jls_annotation_type_e __Pyx_PyInt_As_enum__jls_annotation_type_e(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_uint16_t(uint16_t value);
 
 /* CIntToPy.proto */
@@ -2583,14 +2590,15 @@
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *, int, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
+static __Pyx_TypeInfo __Pyx_TypeInfo_nn_uint8_t__const__ = { "const uint8_t", NULL, sizeof(uint8_t const ), { 0 }, 0, IS_UNSIGNED(uint8_t const ) ? 'U' : 'I', IS_UNSIGNED(uint8_t const ), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_uint8_t = { "uint8_t", NULL, sizeof(__pyx_t_5numpy_uint8_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_uint8_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_uint8_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t = { "float64_t", NULL, sizeof(__pyx_t_5numpy_float64_t), { 0 }, 0, 'R', 0, 0 };
 #define __Pyx_MODULE_NAME "pyjls.binding"
 extern int __pyx_module_is_main_pyjls__binding;
 int __pyx_module_is_main_pyjls__binding = 0;
 
 /* Implementation of 'pyjls.binding' */
@@ -2620,17 +2628,18 @@
 static const char __pyx_k_I4[] = "I4";
 static const char __pyx_k_I8[] = "I8";
 static const char __pyx_k_U1[] = "U1";
 static const char __pyx_k_U4[] = "U4";
 static const char __pyx_k_U8[] = "U8";
 static const char __pyx_k__3[] = ":";
 static const char __pyx_k__4[] = "";
-static const char __pyx_k__5[] = "[";
-static const char __pyx_k__6[] = "]: ";
-static const char __pyx_k__7[] = " != ";
+static const char __pyx_k__5[] = "\000";
+static const char __pyx_k__6[] = "[";
+static const char __pyx_k__7[] = "]: ";
+static const char __pyx_k__8[] = " != ";
 static const char __pyx_k_i4[] = "i4";
 static const char __pyx_k_i8[] = "i8";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_rc[] = "rc";
 static const char __pyx_k_u1[] = "u1";
 static const char __pyx_k_u4[] = "u4";
@@ -2645,15 +2654,15 @@
 static const char __pyx_k_MAX[] = "MAX";
 static const char __pyx_k_MIN[] = "MIN";
 static const char __pyx_k_STD[] = "STD";
 static const char __pyx_k_U16[] = "U16";
 static const char __pyx_k_U32[] = "U32";
 static const char __pyx_k_U64[] = "U64";
 static const char __pyx_k_VSR[] = "VSR";
-static const char __pyx_k__42[] = "!";
+static const char __pyx_k__43[] = "!";
 static const char __pyx_k_all[] = "__all__";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_f32[] = "f32";
 static const char __pyx_k_f64[] = "f64";
 static const char __pyx_k_fsr[] = "fsr";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_i16[] = "i16";
@@ -2996,19 +3005,21 @@
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_u_W;
 static PyObject *__pyx_n_s_WARNING;
 static PyObject *__pyx_n_s_Writer;
 static PyObject *__pyx_n_u_Writer;
 static PyObject *__pyx_kp_u__3;
+static PyObject *__pyx_kp_b__4;
 static PyObject *__pyx_kp_u__4;
-static PyObject *__pyx_kp_u__42;
-static PyObject *__pyx_kp_u__5;
+static PyObject *__pyx_kp_u__43;
+static PyObject *__pyx_kp_b__5;
 static PyObject *__pyx_kp_u__6;
 static PyObject *__pyx_kp_u__7;
+static PyObject *__pyx_kp_u__8;
 static PyObject *__pyx_n_s_all;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_u_annotation;
 static PyObject *__pyx_n_s_annotation_decimate_factor;
 static PyObject *__pyx_n_s_annotation_map;
 static PyObject *__pyx_n_s_annotation_type;
 static PyObject *__pyx_n_s_base;
@@ -3342,17 +3353,16 @@
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_200305830;
 static PyObject *__pyx_int_1073741824;
 static PyObject *__pyx_int_1514764800;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__29;
+static PyObject *__pyx_slice__30;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
@@ -3364,47 +3374,48 @@
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
-static PyObject *__pyx_tuple__36;
-static PyObject *__pyx_tuple__38;
-static PyObject *__pyx_tuple__40;
-static PyObject *__pyx_tuple__43;
-static PyObject *__pyx_tuple__45;
-static PyObject *__pyx_tuple__47;
-static PyObject *__pyx_tuple__49;
-static PyObject *__pyx_tuple__51;
-static PyObject *__pyx_tuple__53;
-static PyObject *__pyx_tuple__55;
-static PyObject *__pyx_tuple__57;
+static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__39;
+static PyObject *__pyx_tuple__41;
+static PyObject *__pyx_tuple__44;
+static PyObject *__pyx_tuple__46;
+static PyObject *__pyx_tuple__48;
+static PyObject *__pyx_tuple__50;
+static PyObject *__pyx_tuple__52;
+static PyObject *__pyx_tuple__54;
+static PyObject *__pyx_tuple__56;
 static PyObject *__pyx_tuple__58;
 static PyObject *__pyx_tuple__59;
 static PyObject *__pyx_tuple__60;
 static PyObject *__pyx_tuple__61;
 static PyObject *__pyx_tuple__62;
-static PyObject *__pyx_codeobj__35;
-static PyObject *__pyx_codeobj__37;
-static PyObject *__pyx_codeobj__39;
-static PyObject *__pyx_codeobj__41;
-static PyObject *__pyx_codeobj__44;
-static PyObject *__pyx_codeobj__46;
-static PyObject *__pyx_codeobj__48;
-static PyObject *__pyx_codeobj__50;
-static PyObject *__pyx_codeobj__52;
-static PyObject *__pyx_codeobj__54;
-static PyObject *__pyx_codeobj__56;
-static PyObject *__pyx_codeobj__63;
+static PyObject *__pyx_tuple__63;
+static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__40;
+static PyObject *__pyx_codeobj__42;
+static PyObject *__pyx_codeobj__45;
+static PyObject *__pyx_codeobj__47;
+static PyObject *__pyx_codeobj__49;
+static PyObject *__pyx_codeobj__51;
+static PyObject *__pyx_codeobj__53;
+static PyObject *__pyx_codeobj__55;
+static PyObject *__pyx_codeobj__57;
+static PyObject *__pyx_codeobj__64;
 /* Late includes */
 
 /* "pyjls/binding.pyx":50
  * 
  * 
  * def _data_type_def(basetype, size, q):             # <<<<<<<<<<<<<<
  *     return (basetype & 0x0f) | ((size & 0xff) << 8) | ((q & 0xff) << 16)
@@ -4624,43 +4635,43 @@
   __Pyx_INCREF(__pyx_v_s);
 
   /* "pyjls/binding.pyx":208
  * 
  * def _encode_str(s):
  *     if s is None:             # <<<<<<<<<<<<<<
  *         s = ''
- *     return s.encode('utf-8')
+ *     return s.encode('utf-8') + b'\x00'
  */
   __pyx_t_1 = (__pyx_v_s == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
     /* "pyjls/binding.pyx":209
  * def _encode_str(s):
  *     if s is None:
  *         s = ''             # <<<<<<<<<<<<<<
- *     return s.encode('utf-8')
+ *     return s.encode('utf-8') + b'\x00'
  * 
  */
     __Pyx_INCREF(__pyx_kp_u__4);
     __Pyx_DECREF_SET(__pyx_v_s, __pyx_kp_u__4);
 
     /* "pyjls/binding.pyx":208
  * 
  * def _encode_str(s):
  *     if s is None:             # <<<<<<<<<<<<<<
  *         s = ''
- *     return s.encode('utf-8')
+ *     return s.encode('utf-8') + b'\x00'
  */
   }
 
   /* "pyjls/binding.pyx":210
  *     if s is None:
  *         s = ''
- *     return s.encode('utf-8')             # <<<<<<<<<<<<<<
+ *     return s.encode('utf-8') + b'\x00'             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
@@ -4674,16 +4685,19 @@
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_kp_b__5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_r = __pyx_t_4;
+  __pyx_t_4 = 0;
   goto __pyx_L0;
 
   /* "pyjls/binding.pyx":207
  * 
  * 
  * def _encode_str(s):             # <<<<<<<<<<<<<<
  *     if s is None:
@@ -4704,16 +4718,16 @@
   return __pyx_r;
 }
 
 /* "pyjls/binding.pyx":213
  * 
  * 
  * def _storage_pack(data):             # <<<<<<<<<<<<<<
- *     if isinstance(data, str):
- *         s = _encode_str(data)
+ *     if data is None:
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_13_storage_pack(PyObject *__pyx_self, PyObject *__pyx_v_data); /*proto*/
 static PyMethodDef __pyx_mdef_5pyjls_7binding_13_storage_pack = {"_storage_pack", (PyCFunction)__pyx_pw_5pyjls_7binding_13_storage_pack, METH_O, 0};
 static PyObject *__pyx_pw_5pyjls_7binding_13_storage_pack(PyObject *__pyx_self, PyObject *__pyx_v_data) {
   PyObject *__pyx_r = 0;
@@ -4742,218 +4756,263 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_storage_pack", 0);
 
   /* "pyjls/binding.pyx":214
  * 
  * def _storage_pack(data):
- *     if isinstance(data, str):             # <<<<<<<<<<<<<<
- *         s = _encode_str(data)
- *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
+ *     if data is None:             # <<<<<<<<<<<<<<
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
+ *     elif isinstance(data, str):
  */
-  __pyx_t_1 = PyUnicode_Check(__pyx_v_data); 
+  __pyx_t_1 = (__pyx_v_data == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
     /* "pyjls/binding.pyx":215
  * def _storage_pack(data):
- *     if isinstance(data, str):
+ *     if data is None:
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0             # <<<<<<<<<<<<<<
+ *     elif isinstance(data, str):
+ *         s = _encode_str(data)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_BINARY); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
+    __Pyx_INCREF(__pyx_kp_b__4);
+    __Pyx_GIVEREF(__pyx_kp_b__4);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_kp_b__4);
+    __Pyx_INCREF(__pyx_int_0);
+    __Pyx_GIVEREF(__pyx_int_0);
+    PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_int_0);
+    __pyx_t_3 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
+    goto __pyx_L0;
+
+    /* "pyjls/binding.pyx":214
+ * 
+ * def _storage_pack(data):
+ *     if data is None:             # <<<<<<<<<<<<<<
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
+ *     elif isinstance(data, str):
+ */
+  }
+
+  /* "pyjls/binding.pyx":216
+ *     if data is None:
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
+ *     elif isinstance(data, str):             # <<<<<<<<<<<<<<
+ *         s = _encode_str(data)
+ *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s)
+ */
+  __pyx_t_2 = PyUnicode_Check(__pyx_v_data); 
+  __pyx_t_1 = (__pyx_t_2 != 0);
+  if (__pyx_t_1) {
+
+    /* "pyjls/binding.pyx":217
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
+ *     elif isinstance(data, str):
  *         s = _encode_str(data)             # <<<<<<<<<<<<<<
- *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
+ *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s)
  *     elif isinstance(data, bytes):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
+    __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_data);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_v_s = __pyx_t_3;
-    __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_v_s = __pyx_t_4;
+    __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":216
- *     if isinstance(data, str):
+    /* "pyjls/binding.pyx":218
+ *     elif isinstance(data, str):
  *         s = _encode_str(data)
- *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1             # <<<<<<<<<<<<<<
+ *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s)             # <<<<<<<<<<<<<<
  *     elif isinstance(data, bytes):
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_STRING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 216, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_STRING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __Pyx_INCREF(__pyx_v_s);
     __Pyx_GIVEREF(__pyx_v_s);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_s);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
-    __pyx_t_3 = 0;
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_3);
     __pyx_t_4 = 0;
+    __pyx_t_3 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":214
- * 
- * def _storage_pack(data):
- *     if isinstance(data, str):             # <<<<<<<<<<<<<<
+    /* "pyjls/binding.pyx":216
+ *     if data is None:
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
+ *     elif isinstance(data, str):             # <<<<<<<<<<<<<<
  *         s = _encode_str(data)
- *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
+ *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s)
  */
   }
 
-  /* "pyjls/binding.pyx":217
+  /* "pyjls/binding.pyx":219
  *         s = _encode_str(data)
- *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
+ *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s)
  *     elif isinstance(data, bytes):             # <<<<<<<<<<<<<<
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)
  *     else:
  */
-  __pyx_t_2 = PyBytes_Check(__pyx_v_data); 
-  __pyx_t_1 = (__pyx_t_2 != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = PyBytes_Check(__pyx_v_data); 
+  __pyx_t_2 = (__pyx_t_1 != 0);
+  if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":218
- *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
+    /* "pyjls/binding.pyx":220
+ *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s)
  *     elif isinstance(data, bytes):
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)             # <<<<<<<<<<<<<<
  *     else:
  *         s = _encode_str(json.dumps(data))
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_BINARY); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_BINARY); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 218, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_6 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
-    PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_data);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_data);
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
     __pyx_t_5 = 0;
-    __pyx_t_4 = 0;
-    __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":217
+    /* "pyjls/binding.pyx":219
  *         s = _encode_str(data)
- *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s) + 1
+ *         return c_jls.JLS_STORAGE_TYPE_STRING, s, len(s)
  *     elif isinstance(data, bytes):             # <<<<<<<<<<<<<<
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)
  *     else:
  */
   }
 
-  /* "pyjls/binding.pyx":220
+  /* "pyjls/binding.pyx":222
  *         return c_jls.JLS_STORAGE_TYPE_BINARY, data, len(data)
  *     else:
  *         s = _encode_str(json.dumps(data))             # <<<<<<<<<<<<<<
- *         return c_jls.JLS_STORAGE_TYPE_JSON, s, len(s) + 1
+ *         return c_jls.JLS_STORAGE_TYPE_JSON, s, len(s)
  * 
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_json); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_json); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_dumps); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_dumps); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
       }
     }
     __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_data);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 220, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_8, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
+    __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_v_s = __pyx_t_3;
-    __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_v_s = __pyx_t_4;
+    __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":221
+    /* "pyjls/binding.pyx":223
  *     else:
  *         s = _encode_str(json.dumps(data))
- *         return c_jls.JLS_STORAGE_TYPE_JSON, s, len(s) + 1             # <<<<<<<<<<<<<<
+ *         return c_jls.JLS_STORAGE_TYPE_JSON, s, len(s)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_JSON); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 221, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 221, __pyx_L1_error)
-    __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_enum__jls_storage_type_e(JLS_STORAGE_TYPE_JSON); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __pyx_t_6 = PyObject_Length(__pyx_v_s); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 223, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __Pyx_INCREF(__pyx_v_s);
     __Pyx_GIVEREF(__pyx_v_s);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_s);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_4);
-    __pyx_t_3 = 0;
+    __Pyx_GIVEREF(__pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_3);
     __pyx_t_4 = 0;
+    __pyx_t_3 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
   }
 
   /* "pyjls/binding.pyx":213
  * 
  * 
  * def _storage_pack(data):             # <<<<<<<<<<<<<<
- *     if isinstance(data, str):
- *         s = _encode_str(data)
+ *     if data is None:
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
@@ -4964,15 +5023,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":224
+/* "pyjls/binding.pyx":226
  * 
  * 
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):             # <<<<<<<<<<<<<<
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  */
 
@@ -4985,119 +5044,119 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_storage_unpack", 0);
 
-  /* "pyjls/binding.pyx":225
+  /* "pyjls/binding.pyx":227
  * 
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):
  *     cdef const char * str = <const char *> data             # <<<<<<<<<<<<<<
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  *         return str[:data_size - 1].decode('utf-8')
  */
   __pyx_v_str = ((char const *)__pyx_v_data);
 
-  /* "pyjls/binding.pyx":226
+  /* "pyjls/binding.pyx":228
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:             # <<<<<<<<<<<<<<
  *         return str[:data_size - 1].decode('utf-8')
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:
  */
   switch (__pyx_v_storage_type) {
     case JLS_STORAGE_TYPE_STRING:
 
-    /* "pyjls/binding.pyx":227
+    /* "pyjls/binding.pyx":229
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  *         return str[:data_size - 1].decode('utf-8')             # <<<<<<<<<<<<<<
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:
  *         return data[:data_size]
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_str, 0, (__pyx_v_data_size - 1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_decode_c_string(__pyx_v_str, 0, (__pyx_v_data_size - 1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":226
+    /* "pyjls/binding.pyx":228
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:             # <<<<<<<<<<<<<<
  *         return str[:data_size - 1].decode('utf-8')
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:
  */
     break;
     case JLS_STORAGE_TYPE_BINARY:
 
-    /* "pyjls/binding.pyx":229
+    /* "pyjls/binding.pyx":231
  *         return str[:data_size - 1].decode('utf-8')
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:
  *         return data[:data_size]             # <<<<<<<<<<<<<<
  *     else:
  *         return json.loads(str[:data_size - 1].decode('utf-8'))
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_data) + 0, __pyx_v_data_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_data) + 0, __pyx_v_data_size - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":228
+    /* "pyjls/binding.pyx":230
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  *         return str[:data_size - 1].decode('utf-8')
  *     elif storage_type == c_jls.JLS_STORAGE_TYPE_BINARY:             # <<<<<<<<<<<<<<
  *         return data[:data_size]
  *     else:
  */
     break;
     default:
 
-    /* "pyjls/binding.pyx":231
+    /* "pyjls/binding.pyx":233
  *         return data[:data_size]
  *     else:
  *         return json.loads(str[:data_size - 1].decode('utf-8'))             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_json); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_loads); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_str, 0, (__pyx_v_data_size - 1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_str, 0, (__pyx_v_data_size - 1), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
     break;
   }
 
-  /* "pyjls/binding.pyx":224
+  /* "pyjls/binding.pyx":226
  * 
  * 
  * cdef _storage_unpack(uint8_t storage_type, const uint8_t * data, uint32_t data_size):             # <<<<<<<<<<<<<<
  *     cdef const char * str = <const char *> data
  *     if storage_type == c_jls.JLS_STORAGE_TYPE_STRING:
  */
 
@@ -5111,15 +5170,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":234
+/* "pyjls/binding.pyx":236
  * 
  * 
  * def utc_to_jls(utc):             # <<<<<<<<<<<<<<
  *     """Convert from python UTC timestamp to jls timestamp."""
  *     return int((utc - _UTC_OFFSET) * SECOND)
  */
 
@@ -5145,41 +5204,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("utc_to_jls", 0);
 
-  /* "pyjls/binding.pyx":236
+  /* "pyjls/binding.pyx":238
  * def utc_to_jls(utc):
  *     """Convert from python UTC timestamp to jls timestamp."""
  *     return int((utc - _UTC_OFFSET) * SECOND)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UTC_OFFSET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UTC_OFFSET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Subtract(__pyx_v_utc, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Subtract(__pyx_v_utc, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SECOND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SECOND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":234
+  /* "pyjls/binding.pyx":236
  * 
  * 
  * def utc_to_jls(utc):             # <<<<<<<<<<<<<<
  *     """Convert from python UTC timestamp to jls timestamp."""
  *     return int((utc - _UTC_OFFSET) * SECOND)
  */
 
@@ -5192,15 +5251,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":239
+/* "pyjls/binding.pyx":241
  * 
  * 
  * def jls_to_utc(timestamp):             # <<<<<<<<<<<<<<
  *     """Convert from jls timestamp to python UTC timestamp."""
  *     return (timestamp / SECOND) + _UTC_OFFSET
  */
 
@@ -5226,38 +5285,38 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("jls_to_utc", 0);
 
-  /* "pyjls/binding.pyx":241
+  /* "pyjls/binding.pyx":243
  * def jls_to_utc(timestamp):
  *     """Convert from jls timestamp to python UTC timestamp."""
  *     return (timestamp / SECOND) + _UTC_OFFSET             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SECOND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SECOND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_v_timestamp, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Divide(__pyx_v_timestamp, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UTC_OFFSET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UTC_OFFSET); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":239
+  /* "pyjls/binding.pyx":241
  * 
  * 
  * def jls_to_utc(timestamp):             # <<<<<<<<<<<<<<
  *     """Convert from jls timestamp to python UTC timestamp."""
  *     return (timestamp / SECOND) + _UTC_OFFSET
  */
 
@@ -5270,15 +5329,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":244
+/* "pyjls/binding.pyx":246
  * 
  * 
  * def _handle_rc(name, rc):             # <<<<<<<<<<<<<<
  *     if rc == 0:
  *         return
  */
 
@@ -5313,32 +5372,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_handle_rc", 1, 2, 2, 1); __PYX_ERR(0, 244, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_handle_rc", 1, 2, 2, 1); __PYX_ERR(0, 246, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_handle_rc") < 0)) __PYX_ERR(0, 244, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_handle_rc") < 0)) __PYX_ERR(0, 246, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_rc = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_handle_rc", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 244, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_handle_rc", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 246, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding._handle_rc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_18_handle_rc(__pyx_self, __pyx_v_name, __pyx_v_rc);
 
@@ -5361,139 +5420,139 @@
   Py_UCS4 __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_rc", 0);
 
-  /* "pyjls/binding.pyx":245
+  /* "pyjls/binding.pyx":247
  * 
  * def _handle_rc(name, rc):
  *     if rc == 0:             # <<<<<<<<<<<<<<
  *         return
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  */
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_rc, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_rc, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":246
+    /* "pyjls/binding.pyx":248
  * def _handle_rc(name, rc):
  *     if rc == 0:
  *         return             # <<<<<<<<<<<<<<
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  *     rc_descr = c_jls.jls_error_code_description(rc).decode('utf-8')
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "pyjls/binding.pyx":245
+    /* "pyjls/binding.pyx":247
  * 
  * def _handle_rc(name, rc):
  *     if rc == 0:             # <<<<<<<<<<<<<<
  *         return
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  */
   }
 
-  /* "pyjls/binding.pyx":247
+  /* "pyjls/binding.pyx":249
  *     if rc == 0:
  *         return
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')             # <<<<<<<<<<<<<<
  *     rc_descr = c_jls.jls_error_code_description(rc).decode('utf-8')
  *     raise RuntimeError(f'{name} {rc_name}[{rc}]: {rc_descr}')
  */
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_rc); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_rc); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 249, __pyx_L1_error)
   __pyx_t_4 = jls_error_code_name(__pyx_t_3);
-  __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_4, 0, strlen(__pyx_t_4), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_rc_name = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":248
+  /* "pyjls/binding.pyx":250
  *         return
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  *     rc_descr = c_jls.jls_error_code_description(rc).decode('utf-8')             # <<<<<<<<<<<<<<
  *     raise RuntimeError(f'{name} {rc_name}[{rc}]: {rc_descr}')
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_rc); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_v_rc); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
   __pyx_t_5 = jls_error_code_description(__pyx_t_3);
-  __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_c_string(__pyx_t_5, 0, strlen(__pyx_t_5), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_rc_descr = __pyx_t_1;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":249
+  /* "pyjls/binding.pyx":251
  *     rc_name = c_jls.jls_error_code_name(rc).decode('utf-8')
  *     rc_descr = c_jls.jls_error_code_description(rc).decode('utf-8')
  *     raise RuntimeError(f'{name} {rc_name}[{rc}]: {rc_descr}')             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = PyTuple_New(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_6 = 0;
   __pyx_t_7 = 127;
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_8);
   __pyx_t_8 = 0;
   __Pyx_INCREF(__pyx_kp_u_);
   __pyx_t_6 += 1;
   __Pyx_GIVEREF(__pyx_kp_u_);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_);
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc_name, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_8);
   __pyx_t_8 = 0;
-  __Pyx_INCREF(__pyx_kp_u__5);
+  __Pyx_INCREF(__pyx_kp_u__6);
   __pyx_t_6 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__5);
-  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__5);
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_kp_u__6);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__6);
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_8);
   __pyx_t_8 = 0;
-  __Pyx_INCREF(__pyx_kp_u__6);
+  __Pyx_INCREF(__pyx_kp_u__7);
   __pyx_t_6 += 3;
-  __Pyx_GIVEREF(__pyx_kp_u__6);
-  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_kp_u__6);
-  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc_descr, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_kp_u__7);
+  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_kp_u__7);
+  __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_rc_descr, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
   __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_8);
   PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_t_8);
   __pyx_t_8 = 0;
-  __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_1, 7, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_1, 7, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_RuntimeError, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(0, 249, __pyx_L1_error)
+  __PYX_ERR(0, 251, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":244
+  /* "pyjls/binding.pyx":246
  * 
  * 
  * def _handle_rc(name, rc):             # <<<<<<<<<<<<<<
  *     if rc == 0:
  *         return
  */
 
@@ -5507,20 +5566,20 @@
   __Pyx_XDECREF(__pyx_v_rc_name);
   __Pyx_XDECREF(__pyx_v_rc_descr);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":256
+/* "pyjls/binding.pyx":258
  *     cdef c_jls.jls_signal_def_s _signals[_JLS_SIGNAL_COUNT]
  * 
  *     def __init__(self, path: str):             # <<<<<<<<<<<<<<
+ *         cdef c_jls.jls_twr_s ** wr_ptr = &self._wr
  *         cdef int32_t rc
- *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
  */
 
 /* Python wrapper */
 static int __pyx_pw_5pyjls_7binding_6Writer_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_5pyjls_7binding_6Writer_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_path = 0;
   int __pyx_lineno = 0;
@@ -5544,170 +5603,258 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 256, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 258, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_path = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 256, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 258, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 256, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 258, __pyx_L1_error)
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer___init__(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_5pyjls_7binding_6Writer___init__(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self, PyObject *__pyx_v_path) {
+  struct jls_twr_s **__pyx_v_wr_ptr;
   int32_t __pyx_v_rc;
+  __Pyx_memviewslice __pyx_v_path_u8 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_v_path_bytes = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  char const *__pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
+  __Pyx_memviewslice __pyx_t_2 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyjls/binding.pyx":258
+  /* "pyjls/binding.pyx":259
+ * 
  *     def __init__(self, path: str):
+ *         cdef c_jls.jls_twr_s ** wr_ptr = &self._wr             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
- *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR             # <<<<<<<<<<<<<<
- *         rc = c_jls.jls_twr_open(&self._wr, path.encode('utf-8'))
- *         _handle_rc('open', rc)
+ *         cdef const uint8_t[:] path_u8
  */
-  (__pyx_v_self->_signals[0]).signal_type = JLS_SIGNAL_TYPE_VSR;
+  __pyx_v_wr_ptr = (&__pyx_v_self->_wr);
 
-  /* "pyjls/binding.pyx":259
+  /* "pyjls/binding.pyx":262
  *         cdef int32_t rc
+ *         cdef const uint8_t[:] path_u8
+ *         path_bytes = path.encode('utf-8')             # <<<<<<<<<<<<<<
+ *         path_u8 = path_bytes
  *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
- *         rc = c_jls.jls_twr_open(&self._wr, path.encode('utf-8'))             # <<<<<<<<<<<<<<
- *         _handle_rc('open', rc)
- * 
  */
   if (unlikely(__pyx_v_path == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 259, __pyx_L1_error)
+    __PYX_ERR(0, 262, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 259, __pyx_L1_error)
-  __pyx_v_rc = jls_twr_open((&__pyx_v_self->_wr), __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_path_bytes = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "pyjls/binding.pyx":263
+ *         cdef const uint8_t[:] path_u8
+ *         path_bytes = path.encode('utf-8')
+ *         path_u8 = path_bytes             # <<<<<<<<<<<<<<
+ *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
+ *         with nogil:
+ */
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_v_path_bytes, 0); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 263, __pyx_L1_error)
+  __pyx_v_path_u8 = __pyx_t_2;
+  __pyx_t_2.memview = NULL;
+  __pyx_t_2.data = NULL;
+
+  /* "pyjls/binding.pyx":264
+ *         path_bytes = path.encode('utf-8')
+ *         path_u8 = path_bytes
+ *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR             # <<<<<<<<<<<<<<
+ *         with nogil:
+ *             rc = c_jls.jls_twr_open(wr_ptr, <char *> &path_u8[0])
+ */
+  (__pyx_v_self->_signals[0]).signal_type = JLS_SIGNAL_TYPE_VSR;
+
+  /* "pyjls/binding.pyx":265
+ *         path_u8 = path_bytes
+ *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_open(wr_ptr, <char *> &path_u8[0])
+ *         _handle_rc('open', rc)
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
 
-  /* "pyjls/binding.pyx":260
+        /* "pyjls/binding.pyx":266
  *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
- *         rc = c_jls.jls_twr_open(&self._wr, path.encode('utf-8'))
+ *         with nogil:
+ *             rc = c_jls.jls_twr_open(wr_ptr, <char *> &path_u8[0])             # <<<<<<<<<<<<<<
+ *         _handle_rc('open', rc)
+ * 
+ */
+        __pyx_t_3 = 0;
+        __pyx_t_4 = -1;
+        if (__pyx_t_3 < 0) {
+          __pyx_t_3 += __pyx_v_path_u8.shape[0];
+          if (unlikely(__pyx_t_3 < 0)) __pyx_t_4 = 0;
+        } else if (unlikely(__pyx_t_3 >= __pyx_v_path_u8.shape[0])) __pyx_t_4 = 0;
+        if (unlikely(__pyx_t_4 != -1)) {
+          __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_4);
+          __PYX_ERR(0, 266, __pyx_L4_error)
+        }
+        __pyx_v_rc = jls_twr_open(__pyx_v_wr_ptr, ((char *)(&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_path_u8.data + __pyx_t_3 * __pyx_v_path_u8.strides[0]) ))))));
+      }
+
+      /* "pyjls/binding.pyx":265
+ *         path_u8 = path_bytes
+ *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_open(wr_ptr, <char *> &path_u8[0])
+ *         _handle_rc('open', rc)
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L4_error: {
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "pyjls/binding.pyx":267
+ *         with nogil:
+ *             rc = c_jls.jls_twr_open(wr_ptr, <char *> &path_u8[0])
  *         _handle_rc('open', rc)             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = NULL;
-  __pyx_t_6 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 267, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_7 = NULL;
+  __pyx_t_4 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
+    if (likely(__pyx_t_7)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_6 = 1;
+      __Pyx_DECREF_SET(__pyx_t_5, function);
+      __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_open, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyFunction_Check(__pyx_t_5)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_open, __pyx_t_6};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_open, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_open, __pyx_t_6};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 260, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (__pyx_t_5) {
-      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 267, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    if (__pyx_t_7) {
+      __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_open);
     __Pyx_GIVEREF(__pyx_n_u_open);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_n_u_open);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
-    __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_4, __pyx_n_u_open);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_4, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":256
+  /* "pyjls/binding.pyx":258
  *     cdef c_jls.jls_signal_def_s _signals[_JLS_SIGNAL_COUNT]
  * 
  *     def __init__(self, path: str):             # <<<<<<<<<<<<<<
+ *         cdef c_jls.jls_twr_s ** wr_ptr = &self._wr
  *         cdef int32_t rc
- *         self._signals[0].signal_type = c_jls.JLS_SIGNAL_TYPE_VSR
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_2, 1);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
   __Pyx_AddTraceback("pyjls.binding.Writer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_path_u8, 1);
+  __Pyx_XDECREF(__pyx_v_path_bytes);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":262
+/* "pyjls/binding.pyx":269
  *         _handle_rc('open', rc)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -5725,42 +5872,42 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_2__enter__(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "pyjls/binding.pyx":263
+  /* "pyjls/binding.pyx":270
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, type, value, traceback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":262
+  /* "pyjls/binding.pyx":269
  *         _handle_rc('open', rc)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":265
+/* "pyjls/binding.pyx":272
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -5797,40 +5944,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 265, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 272, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_traceback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 265, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 272, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 265, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 272, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_type = values[0];
     __pyx_v_value = values[1];
     __pyx_v_traceback = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 265, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 272, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_4__exit__(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_type, __pyx_v_value, __pyx_v_traceback);
 
@@ -5846,41 +5993,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "pyjls/binding.pyx":266
+  /* "pyjls/binding.pyx":273
  * 
  *     def __exit__(self, type, value, traceback):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 273, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":265
+  /* "pyjls/binding.pyx":272
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -5895,20 +6042,20 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":268
+/* "pyjls/binding.pyx":275
  *         self.close()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
- *         c_jls.jls_twr_close(self._wr)
- * 
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_7close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_7close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5917,48 +6064,95 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_6close(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self) {
+  struct jls_twr_s *__pyx_v_wr;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
+  struct jls_twr_s *__pyx_t_1;
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "pyjls/binding.pyx":269
+  /* "pyjls/binding.pyx":276
  * 
  *     def close(self):
- *         c_jls.jls_twr_close(self._wr)             # <<<<<<<<<<<<<<
+ *         cdef c_jls.jls_twr_s * wr = self._wr             # <<<<<<<<<<<<<<
+ *         with nogil:
+ *             c_jls.jls_twr_close(wr)
+ */
+  __pyx_t_1 = __pyx_v_self->_wr;
+  __pyx_v_wr = __pyx_t_1;
+
+  /* "pyjls/binding.pyx":277
+ *     def close(self):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             c_jls.jls_twr_close(wr)
+ * 
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "pyjls/binding.pyx":278
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:
+ *             c_jls.jls_twr_close(wr)             # <<<<<<<<<<<<<<
  * 
  *     def flush(self):
  */
-  (void)(jls_twr_close(__pyx_v_self->_wr));
+        (void)(jls_twr_close(__pyx_v_wr));
+      }
+
+      /* "pyjls/binding.pyx":277
+ *     def close(self):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             c_jls.jls_twr_close(wr)
+ * 
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L5:;
+      }
+  }
 
-  /* "pyjls/binding.pyx":268
+  /* "pyjls/binding.pyx":275
  *         self.close()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
- *         c_jls.jls_twr_close(self._wr)
- * 
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":271
- *         c_jls.jls_twr_close(self._wr)
+/* "pyjls/binding.pyx":280
+ *             c_jls.jls_twr_close(wr)
  * 
  *     def flush(self):             # <<<<<<<<<<<<<<
- *         c_jls.jls_twr_flush(self._wr)
- * 
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_9flush(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_9flush(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5967,44 +6161,91 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_8flush(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self) {
+  struct jls_twr_s *__pyx_v_wr;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
+  struct jls_twr_s *__pyx_t_1;
   __Pyx_RefNannySetupContext("flush", 0);
 
-  /* "pyjls/binding.pyx":272
+  /* "pyjls/binding.pyx":281
  * 
  *     def flush(self):
- *         c_jls.jls_twr_flush(self._wr)             # <<<<<<<<<<<<<<
+ *         cdef c_jls.jls_twr_s * wr = self._wr             # <<<<<<<<<<<<<<
+ *         with nogil:
+ *             c_jls.jls_twr_flush(wr)
+ */
+  __pyx_t_1 = __pyx_v_self->_wr;
+  __pyx_v_wr = __pyx_t_1;
+
+  /* "pyjls/binding.pyx":282
+ *     def flush(self):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             c_jls.jls_twr_flush(wr)
+ * 
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "pyjls/binding.pyx":283
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:
+ *             c_jls.jls_twr_flush(wr)             # <<<<<<<<<<<<<<
  * 
  *     def source_def(self, source_id, name=None, vendor=None, model=None, version=None, serial_number=None):
  */
-  (void)(jls_twr_flush(__pyx_v_self->_wr));
+        (void)(jls_twr_flush(__pyx_v_wr));
+      }
 
-  /* "pyjls/binding.pyx":271
- *         c_jls.jls_twr_close(self._wr)
+      /* "pyjls/binding.pyx":282
+ *     def flush(self):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             c_jls.jls_twr_flush(wr)
  * 
- *     def flush(self):             # <<<<<<<<<<<<<<
- *         c_jls.jls_twr_flush(self._wr)
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "pyjls/binding.pyx":280
+ *             c_jls.jls_twr_close(wr)
  * 
+ *     def flush(self):             # <<<<<<<<<<<<<<
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         with nogil:
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":274
- *         c_jls.jls_twr_flush(self._wr)
+/* "pyjls/binding.pyx":285
+ *             c_jls.jls_twr_flush(wr)
  * 
  *     def source_def(self, source_id, name=None, vendor=None, model=None, version=None, serial_number=None):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s s
  */
 
 /* Python wrapper */
@@ -6082,15 +6323,15 @@
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_serial_number);
           if (value) { values[5] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "source_def") < 0)) __PYX_ERR(0, 274, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "source_def") < 0)) __PYX_ERR(0, 285, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
@@ -6110,15 +6351,15 @@
     __pyx_v_vendor = values[2];
     __pyx_v_model = values[3];
     __pyx_v_version = values[4];
     __pyx_v_serial_number = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("source_def", 0, 1, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 274, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("source_def", 0, 1, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 285, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.source_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_10source_def(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_source_id, __pyx_v_name, __pyx_v_vendor, __pyx_v_model, __pyx_v_version, __pyx_v_serial_number);
 
@@ -6150,228 +6391,228 @@
   int __pyx_t_11;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("source_def", 0);
 
-  /* "pyjls/binding.pyx":277
+  /* "pyjls/binding.pyx":288
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s s
  *         name_b = _encode_str(name)             # <<<<<<<<<<<<<<
  *         vendor_b = _encode_str(vendor)
  *         model_b = _encode_str(model)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_name_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":278
+  /* "pyjls/binding.pyx":289
  *         cdef c_jls.jls_source_def_s s
  *         name_b = _encode_str(name)
  *         vendor_b = _encode_str(vendor)             # <<<<<<<<<<<<<<
  *         model_b = _encode_str(model)
  *         version_b = _encode_str(version)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_vendor) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_vendor);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_vendor_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":279
+  /* "pyjls/binding.pyx":290
  *         name_b = _encode_str(name)
  *         vendor_b = _encode_str(vendor)
  *         model_b = _encode_str(model)             # <<<<<<<<<<<<<<
  *         version_b = _encode_str(version)
  *         serial_number_b = _encode_str(serial_number)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_model) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_model);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 279, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_model_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":280
+  /* "pyjls/binding.pyx":291
  *         vendor_b = _encode_str(vendor)
  *         model_b = _encode_str(model)
  *         version_b = _encode_str(version)             # <<<<<<<<<<<<<<
  *         serial_number_b = _encode_str(serial_number)
  *         s.source_id = source_id
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_version) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_version);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 280, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_version_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":281
+  /* "pyjls/binding.pyx":292
  *         model_b = _encode_str(model)
  *         version_b = _encode_str(version)
  *         serial_number_b = _encode_str(serial_number)             # <<<<<<<<<<<<<<
  *         s.source_id = source_id
  *         s.name = name_b
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_serial_number) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_serial_number);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_serial_number_b = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":282
+  /* "pyjls/binding.pyx":293
  *         version_b = _encode_str(version)
  *         serial_number_b = _encode_str(serial_number)
  *         s.source_id = source_id             # <<<<<<<<<<<<<<
  *         s.name = name_b
  *         s.vendor = vendor_b
  */
-  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_source_id); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_source_id); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 293, __pyx_L1_error)
   __pyx_v_s.source_id = __pyx_t_4;
 
-  /* "pyjls/binding.pyx":283
+  /* "pyjls/binding.pyx":294
  *         serial_number_b = _encode_str(serial_number)
  *         s.source_id = source_id
  *         s.name = name_b             # <<<<<<<<<<<<<<
  *         s.vendor = vendor_b
  *         s.model = model_b
  */
-  __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_v_name_b); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_v_name_b); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L1_error)
   __pyx_v_s.name = __pyx_t_5;
 
-  /* "pyjls/binding.pyx":284
+  /* "pyjls/binding.pyx":295
  *         s.source_id = source_id
  *         s.name = name_b
  *         s.vendor = vendor_b             # <<<<<<<<<<<<<<
  *         s.model = model_b
  *         s.version = version_b
  */
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_v_vendor_b); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_v_vendor_b); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 295, __pyx_L1_error)
   __pyx_v_s.vendor = __pyx_t_6;
 
-  /* "pyjls/binding.pyx":285
+  /* "pyjls/binding.pyx":296
  *         s.name = name_b
  *         s.vendor = vendor_b
  *         s.model = model_b             # <<<<<<<<<<<<<<
  *         s.version = version_b
  *         s.serial_number = serial_number_b
  */
-  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_v_model_b); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_v_model_b); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 296, __pyx_L1_error)
   __pyx_v_s.model = __pyx_t_7;
 
-  /* "pyjls/binding.pyx":286
+  /* "pyjls/binding.pyx":297
  *         s.vendor = vendor_b
  *         s.model = model_b
  *         s.version = version_b             # <<<<<<<<<<<<<<
  *         s.serial_number = serial_number_b
  *         rc = c_jls.jls_twr_source_def(self._wr, &s)
  */
-  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_version_b); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_v_version_b); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 297, __pyx_L1_error)
   __pyx_v_s.version = __pyx_t_8;
 
-  /* "pyjls/binding.pyx":287
+  /* "pyjls/binding.pyx":298
  *         s.model = model_b
  *         s.version = version_b
  *         s.serial_number = serial_number_b             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_twr_source_def(self._wr, &s)
  *         _handle_rc('source_def', rc)
  */
-  __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_v_serial_number_b); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_v_serial_number_b); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 298, __pyx_L1_error)
   __pyx_v_s.serial_number = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":288
+  /* "pyjls/binding.pyx":299
  *         s.version = version_b
  *         s.serial_number = serial_number_b
  *         rc = c_jls.jls_twr_source_def(self._wr, &s)             # <<<<<<<<<<<<<<
  *         _handle_rc('source_def', rc)
  * 
  */
   __pyx_v_rc = jls_twr_source_def(__pyx_v_self->_wr, (&__pyx_v_s));
 
-  /* "pyjls/binding.pyx":289
+  /* "pyjls/binding.pyx":300
  *         s.serial_number = serial_number_b
  *         rc = c_jls.jls_twr_source_def(self._wr, &s)
  *         _handle_rc('source_def', rc)             # <<<<<<<<<<<<<<
  * 
  *     def source_def_from_struct(self, s: SourceDef):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 289, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_10 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -6380,50 +6621,50 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_11 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_u_source_def, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_n_u_source_def, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 289, __pyx_L1_error)
+    __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
     if (__pyx_t_10) {
       __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_source_def);
     __Pyx_GIVEREF(__pyx_n_u_source_def);
     PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_n_u_source_def);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":274
- *         c_jls.jls_twr_flush(self._wr)
+  /* "pyjls/binding.pyx":285
+ *             c_jls.jls_twr_flush(wr)
  * 
  *     def source_def(self, source_id, name=None, vendor=None, model=None, version=None, serial_number=None):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s s
  */
 
   /* function exit code */
@@ -6444,15 +6685,15 @@
   __Pyx_XDECREF(__pyx_v_version_b);
   __Pyx_XDECREF(__pyx_v_serial_number_b);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":291
+/* "pyjls/binding.pyx":302
  *         _handle_rc('source_def', rc)
  * 
  *     def source_def_from_struct(self, s: SourceDef):             # <<<<<<<<<<<<<<
  *         return self.source_def(s.source_id,
  *                                name=s.name,
  */
 
@@ -6477,111 +6718,111 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("source_def_from_struct", 0);
 
-  /* "pyjls/binding.pyx":292
+  /* "pyjls/binding.pyx":303
  * 
  *     def source_def_from_struct(self, s: SourceDef):
  *         return self.source_def(s.source_id,             # <<<<<<<<<<<<<<
  *                                name=s.name,
  *                                vendor=s.vendor,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_source_def); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_source_def); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_source_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_source_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":293
+  /* "pyjls/binding.pyx":304
  *     def source_def_from_struct(self, s: SourceDef):
  *         return self.source_def(s.source_id,
  *                                name=s.name,             # <<<<<<<<<<<<<<
  *                                vendor=s.vendor,
  *                                model=s.model,
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":294
+  /* "pyjls/binding.pyx":305
  *         return self.source_def(s.source_id,
  *                                name=s.name,
  *                                vendor=s.vendor,             # <<<<<<<<<<<<<<
  *                                model=s.model,
  *                                version=s.version,
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_vendor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 294, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_vendor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_vendor, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_vendor, __pyx_t_4) < 0) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":295
+  /* "pyjls/binding.pyx":306
  *                                name=s.name,
  *                                vendor=s.vendor,
  *                                model=s.model,             # <<<<<<<<<<<<<<
  *                                version=s.version,
  *                                serial_number=s.serial_number)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_model); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_model); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_model, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_model, __pyx_t_4) < 0) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":296
+  /* "pyjls/binding.pyx":307
  *                                vendor=s.vendor,
  *                                model=s.model,
  *                                version=s.version,             # <<<<<<<<<<<<<<
  *                                serial_number=s.serial_number)
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_version); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_version); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_version, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_version, __pyx_t_4) < 0) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":297
+  /* "pyjls/binding.pyx":308
  *                                model=s.model,
  *                                version=s.version,
  *                                serial_number=s.serial_number)             # <<<<<<<<<<<<<<
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_serial_number); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_serial_number); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_serial_number, __pyx_t_4) < 0) __PYX_ERR(0, 293, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_serial_number, __pyx_t_4) < 0) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":292
+  /* "pyjls/binding.pyx":303
  * 
  *     def source_def_from_struct(self, s: SourceDef):
  *         return self.source_def(s.source_id,             # <<<<<<<<<<<<<<
  *                                name=s.name,
  *                                vendor=s.vendor,
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":291
+  /* "pyjls/binding.pyx":302
  *         _handle_rc('source_def', rc)
  * 
  *     def source_def_from_struct(self, s: SourceDef):             # <<<<<<<<<<<<<<
  *         return self.source_def(s.source_id,
  *                                name=s.name,
  */
 
@@ -6595,15 +6836,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":299
+/* "pyjls/binding.pyx":310
  *                                serial_number=s.serial_number)
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,             # <<<<<<<<<<<<<<
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  */
 
@@ -6632,37 +6873,37 @@
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_signal_id,&__pyx_n_s_source_id,&__pyx_n_s_signal_type,&__pyx_n_s_data_type,&__pyx_n_s_sample_rate,&__pyx_n_s_samples_per_data,&__pyx_n_s_sample_decimate_factor,&__pyx_n_s_entries_per_summary,&__pyx_n_s_summary_decimate_factor,&__pyx_n_s_annotation_decimate_factor,&__pyx_n_s_utc_decimate_factor,&__pyx_n_s_name,&__pyx_n_s_units,0};
     PyObject* values[13] = {0,0,0,0,0,0,0,0,0,0,0,0,0};
     values[2] = ((PyObject *)Py_None);
     values[3] = ((PyObject *)Py_None);
     values[4] = ((PyObject *)Py_None);
 
-    /* "pyjls/binding.pyx":300
+    /* "pyjls/binding.pyx":311
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,             # <<<<<<<<<<<<<<
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  *                    name=None, units=None):
  */
     values[5] = ((PyObject *)Py_None);
     values[6] = ((PyObject *)Py_None);
     values[7] = ((PyObject *)Py_None);
 
-    /* "pyjls/binding.pyx":301
+    /* "pyjls/binding.pyx":312
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,             # <<<<<<<<<<<<<<
  *                    name=None, units=None):
  *         cdef int32_t rc
  */
     values[8] = ((PyObject *)Py_None);
     values[9] = ((PyObject *)Py_None);
     values[10] = ((PyObject *)Py_None);
 
-    /* "pyjls/binding.pyx":302
+    /* "pyjls/binding.pyx":313
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  *                    name=None, units=None):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_signal_def_s * s
  */
     values[11] = ((PyObject *)Py_None);
@@ -6705,15 +6946,15 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_source_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("signal_def", 0, 2, 13, 1); __PYX_ERR(0, 299, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("signal_def", 0, 2, 13, 1); __PYX_ERR(0, 310, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_type);
           if (value) { values[2] = value; kw_args--; }
         }
@@ -6775,15 +7016,15 @@
         case 12:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_units);
           if (value) { values[12] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "signal_def") < 0)) __PYX_ERR(0, 299, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "signal_def") < 0)) __PYX_ERR(0, 310, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case 13: values[12] = PyTuple_GET_ITEM(__pyx_args, 12);
         CYTHON_FALLTHROUGH;
         case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
         CYTHON_FALLTHROUGH;
@@ -6823,23 +7064,23 @@
     __pyx_v_annotation_decimate_factor = values[9];
     __pyx_v_utc_decimate_factor = values[10];
     __pyx_v_name = values[11];
     __pyx_v_units = values[12];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("signal_def", 0, 2, 13, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 299, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("signal_def", 0, 2, 13, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 310, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.signal_def", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_14signal_def(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_source_id, __pyx_v_signal_type, __pyx_v_data_type, __pyx_v_sample_rate, __pyx_v_samples_per_data, __pyx_v_sample_decimate_factor, __pyx_v_entries_per_summary, __pyx_v_summary_decimate_factor, __pyx_v_annotation_decimate_factor, __pyx_v_utc_decimate_factor, __pyx_v_name, __pyx_v_units);
 
-  /* "pyjls/binding.pyx":299
+  /* "pyjls/binding.pyx":310
  *                                serial_number=s.serial_number)
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,             # <<<<<<<<<<<<<<
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  */
 
@@ -6873,371 +7114,371 @@
   PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signal_def", 0);
   __Pyx_INCREF(__pyx_v_data_type);
 
-  /* "pyjls/binding.pyx":305
+  /* "pyjls/binding.pyx":316
  *         cdef int32_t rc
  *         cdef c_jls.jls_signal_def_s * s
  *         s = &self._signals[signal_id]             # <<<<<<<<<<<<<<
  *         if data_type is None:
  *             data_type = DataType.F32
  */
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 305, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
   __pyx_v_s = (&(__pyx_v_self->_signals[__pyx_t_1]));
 
-  /* "pyjls/binding.pyx":306
+  /* "pyjls/binding.pyx":317
  *         cdef c_jls.jls_signal_def_s * s
  *         s = &self._signals[signal_id]
  *         if data_type is None:             # <<<<<<<<<<<<<<
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):
  */
   __pyx_t_2 = (__pyx_v_data_type == Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "pyjls/binding.pyx":307
+    /* "pyjls/binding.pyx":318
  *         s = &self._signals[signal_id]
  *         if data_type is None:
  *             data_type = DataType.F32             # <<<<<<<<<<<<<<
  *         elif isinstance(data_type, str):
  *             data_type = _data_type_as_enum[data_type]
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataType); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DataType); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_F32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 307, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_F32); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_data_type, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":306
+    /* "pyjls/binding.pyx":317
  *         cdef c_jls.jls_signal_def_s * s
  *         s = &self._signals[signal_id]
  *         if data_type is None:             # <<<<<<<<<<<<<<
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):
  */
     goto __pyx_L3;
   }
 
-  /* "pyjls/binding.pyx":308
+  /* "pyjls/binding.pyx":319
  *         if data_type is None:
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):             # <<<<<<<<<<<<<<
  *             data_type = _data_type_as_enum[data_type]
  *         s.signal_id = signal_id
  */
   __pyx_t_3 = PyUnicode_Check(__pyx_v_data_type); 
   __pyx_t_2 = (__pyx_t_3 != 0);
   if (__pyx_t_2) {
 
-    /* "pyjls/binding.pyx":309
+    /* "pyjls/binding.pyx":320
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):
  *             data_type = _data_type_as_enum[data_type]             # <<<<<<<<<<<<<<
  *         s.signal_id = signal_id
  *         s.source_id = source_id
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 309, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_data_type_as_enum); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 309, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_v_data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_data_type, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":308
+    /* "pyjls/binding.pyx":319
  *         if data_type is None:
  *             data_type = DataType.F32
  *         elif isinstance(data_type, str):             # <<<<<<<<<<<<<<
  *             data_type = _data_type_as_enum[data_type]
  *         s.signal_id = signal_id
  */
   }
   __pyx_L3:;
 
-  /* "pyjls/binding.pyx":310
+  /* "pyjls/binding.pyx":321
  *         elif isinstance(data_type, str):
  *             data_type = _data_type_as_enum[data_type]
  *         s.signal_id = signal_id             # <<<<<<<<<<<<<<
  *         s.source_id = source_id
  *         s.signal_type = 0 if signal_type is None else int(signal_type)
  */
-  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_6 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 310, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_6 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 321, __pyx_L1_error)
   __pyx_v_s->signal_id = __pyx_t_6;
 
-  /* "pyjls/binding.pyx":311
+  /* "pyjls/binding.pyx":322
  *             data_type = _data_type_as_enum[data_type]
  *         s.signal_id = signal_id
  *         s.source_id = source_id             # <<<<<<<<<<<<<<
  *         s.signal_type = 0 if signal_type is None else int(signal_type)
  *         s.data_type = data_type
  */
-  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_source_id); if (unlikely((__pyx_t_6 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_source_id); if (unlikely((__pyx_t_6 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 322, __pyx_L1_error)
   __pyx_v_s->source_id = __pyx_t_6;
 
-  /* "pyjls/binding.pyx":312
+  /* "pyjls/binding.pyx":323
  *         s.signal_id = signal_id
  *         s.source_id = source_id
  *         s.signal_type = 0 if signal_type is None else int(signal_type)             # <<<<<<<<<<<<<<
  *         s.data_type = data_type
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)
  */
   __pyx_t_2 = (__pyx_v_signal_type == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_7 = 0;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 312, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 323, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_t_4); if (unlikely((__pyx_t_8 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 312, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_t_4); if (unlikely((__pyx_t_8 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_7 = __pyx_t_8;
   }
   __pyx_v_s->signal_type = __pyx_t_7;
 
-  /* "pyjls/binding.pyx":313
+  /* "pyjls/binding.pyx":324
  *         s.source_id = source_id
  *         s.signal_type = 0 if signal_type is None else int(signal_type)
  *         s.data_type = data_type             # <<<<<<<<<<<<<<
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)
  */
-  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_v_data_type); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_uint32_t(__pyx_v_data_type); if (unlikely((__pyx_t_9 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 324, __pyx_L1_error)
   __pyx_v_s->data_type = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":314
+  /* "pyjls/binding.pyx":325
  *         s.signal_type = 0 if signal_type is None else int(signal_type)
  *         s.data_type = data_type
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)             # <<<<<<<<<<<<<<
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)
  */
   __pyx_t_2 = (__pyx_v_sample_rate == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_sample_rate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_sample_rate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 325, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 325, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->sample_rate = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":315
+  /* "pyjls/binding.pyx":326
  *         s.data_type = data_type
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)             # <<<<<<<<<<<<<<
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)
  */
   __pyx_t_2 = (__pyx_v_samples_per_data == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x186A0;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_samples_per_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 315, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_samples_per_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 315, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->samples_per_data = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":316
+  /* "pyjls/binding.pyx":327
  *         s.sample_rate = 0 if sample_rate is None else int(sample_rate)
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)             # <<<<<<<<<<<<<<
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)
  */
   __pyx_t_2 = (__pyx_v_sample_decimate_factor == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x64;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_sample_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_sample_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 327, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 327, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->sample_decimate_factor = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":317
+  /* "pyjls/binding.pyx":328
  *         s.samples_per_data = 100000 if samples_per_data is None else int(samples_per_data)
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)             # <<<<<<<<<<<<<<
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)
  */
   __pyx_t_2 = (__pyx_v_entries_per_summary == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x4E20;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_entries_per_summary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_entries_per_summary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 328, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->entries_per_summary = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":318
+  /* "pyjls/binding.pyx":329
  *         s.sample_decimate_factor = 100 if sample_decimate_factor is None else int(sample_decimate_factor)
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)             # <<<<<<<<<<<<<<
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)
  */
   __pyx_t_2 = (__pyx_v_summary_decimate_factor == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x64;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_summary_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 318, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_summary_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 318, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->summary_decimate_factor = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":319
+  /* "pyjls/binding.pyx":330
  *         s.entries_per_summary = 20000 if entries_per_summary is None else int(entries_per_summary)
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)             # <<<<<<<<<<<<<<
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)
  *         name_b = _encode_str(name)
  */
   __pyx_t_2 = (__pyx_v_annotation_decimate_factor == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x64;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_annotation_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_annotation_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->annotation_decimate_factor = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":320
+  /* "pyjls/binding.pyx":331
  *         s.summary_decimate_factor = 100 if summary_decimate_factor is None else int(summary_decimate_factor)
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)             # <<<<<<<<<<<<<<
  *         name_b = _encode_str(name)
  *         units_b = _encode_str(units)
  */
   __pyx_t_2 = (__pyx_v_utc_decimate_factor == Py_None);
   if ((__pyx_t_2 != 0)) {
     __pyx_t_9 = 0x64;
   } else {
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_utc_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_v_utc_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 320, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 331, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_10;
   }
   __pyx_v_s->utc_decimate_factor = __pyx_t_9;
 
-  /* "pyjls/binding.pyx":321
+  /* "pyjls/binding.pyx":332
  *         s.annotation_decimate_factor = 100 if annotation_decimate_factor is None else int(annotation_decimate_factor)
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)
  *         name_b = _encode_str(name)             # <<<<<<<<<<<<<<
  *         units_b = _encode_str(units)
  *         s.name = name_b
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 321, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_11, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 321, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_name_b = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":322
+  /* "pyjls/binding.pyx":333
  *         s.utc_decimate_factor = 100 if utc_decimate_factor is None else int(utc_decimate_factor)
  *         name_b = _encode_str(name)
  *         units_b = _encode_str(units)             # <<<<<<<<<<<<<<
  *         s.name = name_b
  *         s.units = units_b
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 322, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_encode_str); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_11 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_11)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_11, __pyx_v_units) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_units);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 322, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_units_b = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":323
+  /* "pyjls/binding.pyx":334
  *         name_b = _encode_str(name)
  *         units_b = _encode_str(units)
  *         s.name = name_b             # <<<<<<<<<<<<<<
  *         s.units = units_b
  *         rc = c_jls.jls_twr_signal_def(self._wr, s)
  */
-  __pyx_t_12 = __Pyx_PyObject_AsString(__pyx_v_name_b); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_AsString(__pyx_v_name_b); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L1_error)
   __pyx_v_s->name = __pyx_t_12;
 
-  /* "pyjls/binding.pyx":324
+  /* "pyjls/binding.pyx":335
  *         units_b = _encode_str(units)
  *         s.name = name_b
  *         s.units = units_b             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_twr_signal_def(self._wr, s)
  *         _handle_rc('signal_def', rc)
  */
-  __pyx_t_13 = __Pyx_PyObject_AsString(__pyx_v_units_b); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 324, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyObject_AsString(__pyx_v_units_b); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 335, __pyx_L1_error)
   __pyx_v_s->units = __pyx_t_13;
 
-  /* "pyjls/binding.pyx":325
+  /* "pyjls/binding.pyx":336
  *         s.name = name_b
  *         s.units = units_b
  *         rc = c_jls.jls_twr_signal_def(self._wr, s)             # <<<<<<<<<<<<<<
  *         _handle_rc('signal_def', rc)
  * 
  */
   __pyx_v_rc = jls_twr_signal_def(__pyx_v_self->_wr, __pyx_v_s);
 
-  /* "pyjls/binding.pyx":326
+  /* "pyjls/binding.pyx":337
  *         s.units = units_b
  *         rc = c_jls.jls_twr_signal_def(self._wr, s)
  *         _handle_rc('signal_def', rc)             # <<<<<<<<<<<<<<
  * 
  *     def signal_def_from_struct(self, s: SignalDef):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_11 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __pyx_t_14 = NULL;
   __pyx_t_15 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_14)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -7246,49 +7487,49 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_15 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_n_u_signal_def, __pyx_t_11};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_14, __pyx_n_u_signal_def, __pyx_t_11};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   {
-    __pyx_t_16 = PyTuple_New(2+__pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_16 = PyTuple_New(2+__pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_16);
     if (__pyx_t_14) {
       __Pyx_GIVEREF(__pyx_t_14); PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_14); __pyx_t_14 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_signal_def);
     __Pyx_GIVEREF(__pyx_n_u_signal_def);
     PyTuple_SET_ITEM(__pyx_t_16, 0+__pyx_t_15, __pyx_n_u_signal_def);
     __Pyx_GIVEREF(__pyx_t_11);
     PyTuple_SET_ITEM(__pyx_t_16, 1+__pyx_t_15, __pyx_t_11);
     __pyx_t_11 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_16, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":299
+  /* "pyjls/binding.pyx":310
  *                                serial_number=s.serial_number)
  * 
  *     def signal_def(self, signal_id, source_id, signal_type=None, data_type=None, sample_rate=None,             # <<<<<<<<<<<<<<
  *                    samples_per_data=None, sample_decimate_factor=None, entries_per_summary=None,
  *                    summary_decimate_factor=None, annotation_decimate_factor=None, utc_decimate_factor=None,
  */
 
@@ -7308,15 +7549,15 @@
   __Pyx_XDECREF(__pyx_v_units_b);
   __Pyx_XDECREF(__pyx_v_data_type);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":328
+/* "pyjls/binding.pyx":339
  *         _handle_rc('signal_def', rc)
  * 
  *     def signal_def_from_struct(self, s: SignalDef):             # <<<<<<<<<<<<<<
  *         return self.signal_def(s.signal_id,
  *                                s.source_id,
  */
 
@@ -7341,204 +7582,204 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("signal_def_from_struct", 0);
 
-  /* "pyjls/binding.pyx":329
+  /* "pyjls/binding.pyx":340
  * 
  *     def signal_def_from_struct(self, s: SignalDef):
  *         return self.signal_def(s.signal_id,             # <<<<<<<<<<<<<<
  *                                s.source_id,
  *                                signal_type=s.signal_type,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_signal_def); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_signal_def); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_signal_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_signal_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "pyjls/binding.pyx":330
+  /* "pyjls/binding.pyx":341
  *     def signal_def_from_struct(self, s: SignalDef):
  *         return self.signal_def(s.signal_id,
  *                                s.source_id,             # <<<<<<<<<<<<<<
  *                                signal_type=s.signal_type,
  *                                data_type=s.data_type,
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_source_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_source_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "pyjls/binding.pyx":329
+  /* "pyjls/binding.pyx":340
  * 
  *     def signal_def_from_struct(self, s: SignalDef):
  *         return self.signal_def(s.signal_id,             # <<<<<<<<<<<<<<
  *                                s.source_id,
  *                                signal_type=s.signal_type,
  */
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":331
+  /* "pyjls/binding.pyx":342
  *         return self.signal_def(s.signal_id,
  *                                s.source_id,
  *                                signal_type=s.signal_type,             # <<<<<<<<<<<<<<
  *                                data_type=s.data_type,
  *                                sample_rate=s.sample_rate,
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 331, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_type, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_type, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":332
+  /* "pyjls/binding.pyx":343
  *                                s.source_id,
  *                                signal_type=s.signal_type,
  *                                data_type=s.data_type,             # <<<<<<<<<<<<<<
  *                                sample_rate=s.sample_rate,
  *                                samples_per_data=s.samples_per_data,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_data_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data_type, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data_type, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":333
+  /* "pyjls/binding.pyx":344
  *                                signal_type=s.signal_type,
  *                                data_type=s.data_type,
  *                                sample_rate=s.sample_rate,             # <<<<<<<<<<<<<<
  *                                samples_per_data=s.samples_per_data,
  *                                sample_decimate_factor=s.sample_decimate_factor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_sample_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_sample_rate); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_rate, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_rate, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":334
+  /* "pyjls/binding.pyx":345
  *                                data_type=s.data_type,
  *                                sample_rate=s.sample_rate,
  *                                samples_per_data=s.samples_per_data,             # <<<<<<<<<<<<<<
  *                                sample_decimate_factor=s.sample_decimate_factor,
  *                                entries_per_summary=s.entries_per_summary,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_samples_per_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_samples_per_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_samples_per_data, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_samples_per_data, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":335
+  /* "pyjls/binding.pyx":346
  *                                sample_rate=s.sample_rate,
  *                                samples_per_data=s.samples_per_data,
  *                                sample_decimate_factor=s.sample_decimate_factor,             # <<<<<<<<<<<<<<
  *                                entries_per_summary=s.entries_per_summary,
  *                                summary_decimate_factor=s.summary_decimate_factor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_sample_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_sample_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":336
+  /* "pyjls/binding.pyx":347
  *                                samples_per_data=s.samples_per_data,
  *                                sample_decimate_factor=s.sample_decimate_factor,
  *                                entries_per_summary=s.entries_per_summary,             # <<<<<<<<<<<<<<
  *                                summary_decimate_factor=s.summary_decimate_factor,
  *                                annotation_decimate_factor=s.annotation_decimate_factor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_entries_per_summary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_entries_per_summary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_entries_per_summary, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_entries_per_summary, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":337
+  /* "pyjls/binding.pyx":348
  *                                sample_decimate_factor=s.sample_decimate_factor,
  *                                entries_per_summary=s.entries_per_summary,
  *                                summary_decimate_factor=s.summary_decimate_factor,             # <<<<<<<<<<<<<<
  *                                annotation_decimate_factor=s.annotation_decimate_factor,
  *                                utc_decimate_factor=s.utc_decimate_factor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_summary_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_summary_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_summary_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_summary_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":338
+  /* "pyjls/binding.pyx":349
  *                                entries_per_summary=s.entries_per_summary,
  *                                summary_decimate_factor=s.summary_decimate_factor,
  *                                annotation_decimate_factor=s.annotation_decimate_factor,             # <<<<<<<<<<<<<<
  *                                utc_decimate_factor=s.utc_decimate_factor,
  *                                name=s.name,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_annotation_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_annotation_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotation_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotation_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":339
+  /* "pyjls/binding.pyx":350
  *                                summary_decimate_factor=s.summary_decimate_factor,
  *                                annotation_decimate_factor=s.annotation_decimate_factor,
  *                                utc_decimate_factor=s.utc_decimate_factor,             # <<<<<<<<<<<<<<
  *                                name=s.name,
  *                                units=s.units)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_utc_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 339, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_utc_decimate_factor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_utc_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_utc_decimate_factor, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":340
+  /* "pyjls/binding.pyx":351
  *                                annotation_decimate_factor=s.annotation_decimate_factor,
  *                                utc_decimate_factor=s.utc_decimate_factor,
  *                                name=s.name,             # <<<<<<<<<<<<<<
  *                                units=s.units)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 351, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":341
+  /* "pyjls/binding.pyx":352
  *                                utc_decimate_factor=s.utc_decimate_factor,
  *                                name=s.name,
  *                                units=s.units)             # <<<<<<<<<<<<<<
  * 
  *     def user_data(self, chunk_meta, data):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_units); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_units); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_units, __pyx_t_2) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_units, __pyx_t_2) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":329
+  /* "pyjls/binding.pyx":340
  * 
  *     def signal_def_from_struct(self, s: SignalDef):
  *         return self.signal_def(s.signal_id,             # <<<<<<<<<<<<<<
  *                                s.source_id,
  *                                signal_type=s.signal_type,
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 340, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":328
+  /* "pyjls/binding.pyx":339
  *         _handle_rc('signal_def', rc)
  * 
  *     def signal_def_from_struct(self, s: SignalDef):             # <<<<<<<<<<<<<<
  *         return self.signal_def(s.signal_id,
  *                                s.source_id,
  */
 
@@ -7552,20 +7793,20 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":343
+/* "pyjls/binding.pyx":354
  *                                units=s.units)
  * 
  *     def user_data(self, chunk_meta, data):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
- *         storage_type, payload, payload_length = _storage_pack(data)
+ *         cdef uint16_t chunk_meta_u16 = chunk_meta
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_19user_data(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_19user_data(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_chunk_meta = 0;
   PyObject *__pyx_v_data = 0;
@@ -7594,253 +7835,372 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_chunk_meta)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("user_data", 1, 2, 2, 1); __PYX_ERR(0, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("user_data", 1, 2, 2, 1); __PYX_ERR(0, 354, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "user_data") < 0)) __PYX_ERR(0, 343, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "user_data") < 0)) __PYX_ERR(0, 354, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_chunk_meta = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("user_data", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 343, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("user_data", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 354, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.user_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_18user_data(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_chunk_meta, __pyx_v_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_18user_data(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self, PyObject *__pyx_v_chunk_meta, PyObject *__pyx_v_data) {
   int32_t __pyx_v_rc;
-  PyObject *__pyx_v_storage_type = NULL;
-  PyObject *__pyx_v_payload = NULL;
-  PyObject *__pyx_v_payload_length = NULL;
+  uint16_t __pyx_v_chunk_meta_u16;
+  enum jls_storage_type_e __pyx_v_storage_type;
+  __Pyx_memviewslice __pyx_v_payload_u8 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  uint8_t const *__pyx_v_payload_u8_ptr;
+  uint32_t __pyx_v_payload_length;
+  struct jls_twr_s *__pyx_v_wr;
+  PyObject *__pyx_v_payload_bytes = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
+  uint16_t __pyx_t_1;
+  struct jls_twr_s *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *(*__pyx_t_6)(PyObject *);
-  uint16_t __pyx_t_7;
-  enum jls_storage_type_e __pyx_t_8;
-  uint8_t const *__pyx_t_9;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *(*__pyx_t_8)(PyObject *);
+  enum jls_storage_type_e __pyx_t_9;
   uint32_t __pyx_t_10;
-  int __pyx_t_11;
+  __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_t_12;
+  Py_ssize_t __pyx_t_13;
+  int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("user_data", 0);
 
-  /* "pyjls/binding.pyx":345
+  /* "pyjls/binding.pyx":356
  *     def user_data(self, chunk_meta, data):
  *         cdef int32_t rc
- *         storage_type, payload, payload_length = _storage_pack(data)             # <<<<<<<<<<<<<<
- *         rc = c_jls.jls_twr_user_data(self._wr, chunk_meta, storage_type, payload, payload_length)
- *         _handle_rc('user_data', rc)
+ *         cdef uint16_t chunk_meta_u16 = chunk_meta             # <<<<<<<<<<<<<<
+ *         cdef c_jls.jls_storage_type_e storage_type
+ *         cdef const uint8_t[:] payload_u8
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_storage_pack); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_chunk_meta); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
+  __pyx_v_chunk_meta_u16 = __pyx_t_1;
+
+  /* "pyjls/binding.pyx":359
+ *         cdef c_jls.jls_storage_type_e storage_type
+ *         cdef const uint8_t[:] payload_u8
+ *         cdef const uint8_t * payload_u8_ptr = NULL             # <<<<<<<<<<<<<<
+ *         cdef uint32_t payload_length
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ */
+  __pyx_v_payload_u8_ptr = NULL;
+
+  /* "pyjls/binding.pyx":361
+ *         cdef const uint8_t * payload_u8_ptr = NULL
+ *         cdef uint32_t payload_length
+ *         cdef c_jls.jls_twr_s * wr = self._wr             # <<<<<<<<<<<<<<
+ *         storage_type, payload_bytes, payload_length = _storage_pack(data)
+ *         payload_u8 = payload_bytes
+ */
+  __pyx_t_2 = __pyx_v_self->_wr;
+  __pyx_v_wr = __pyx_t_2;
+
+  /* "pyjls/binding.pyx":362
+ *         cdef uint32_t payload_length
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         storage_type, payload_bytes, payload_length = _storage_pack(data)             # <<<<<<<<<<<<<<
+ *         payload_u8 = payload_bytes
+ *         if 0 != payload_length:
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_storage_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_data);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
-    PyObject* sequence = __pyx_t_1;
+  __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 362, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
+    PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 345, __pyx_L1_error)
+      __PYX_ERR(0, 362, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
-      __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
-    } else {
-      __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
-      __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
-      __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
+      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
+      __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
+      __pyx_t_6 = PyTuple_GET_ITEM(sequence, 2); 
+    } else {
+      __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
+      __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
+      __pyx_t_6 = PyList_GET_ITEM(sequence, 2); 
     }
-    __Pyx_INCREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_t_5);
+    __Pyx_INCREF(__pyx_t_6);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 345, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 362, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
     #endif
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 345, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext;
-    index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
-    __Pyx_GOTREF(__pyx_t_2);
-    index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
-    __Pyx_GOTREF(__pyx_t_3);
-    index = 2; __pyx_t_4 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L3_unpacking_failed;
+    __pyx_t_7 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 362, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_8 = Py_TYPE(__pyx_t_7)->tp_iternext;
+    index = 0; __pyx_t_4 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_4)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 345, __pyx_L1_error)
-    __pyx_t_6 = NULL;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    index = 1; __pyx_t_5 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_5)) goto __pyx_L3_unpacking_failed;
+    __Pyx_GOTREF(__pyx_t_5);
+    index = 2; __pyx_t_6 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_6)) goto __pyx_L3_unpacking_failed;
+    __Pyx_GOTREF(__pyx_t_6);
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 3) < 0) __PYX_ERR(0, 362, __pyx_L1_error)
+    __pyx_t_8 = NULL;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_6 = NULL;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_8 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 345, __pyx_L1_error)
+    __PYX_ERR(0, 362, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
-  __pyx_v_storage_type = __pyx_t_2;
-  __pyx_t_2 = 0;
-  __pyx_v_payload = __pyx_t_3;
-  __pyx_t_3 = 0;
-  __pyx_v_payload_length = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_t_9 = ((enum jls_storage_type_e)__Pyx_PyInt_As_enum__jls_storage_type_e(__pyx_t_4)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_t_6); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_v_storage_type = __pyx_t_9;
+  __pyx_v_payload_bytes = __pyx_t_5;
+  __pyx_t_5 = 0;
+  __pyx_v_payload_length = __pyx_t_10;
 
-  /* "pyjls/binding.pyx":346
- *         cdef int32_t rc
- *         storage_type, payload, payload_length = _storage_pack(data)
- *         rc = c_jls.jls_twr_user_data(self._wr, chunk_meta, storage_type, payload, payload_length)             # <<<<<<<<<<<<<<
+  /* "pyjls/binding.pyx":363
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         storage_type, payload_bytes, payload_length = _storage_pack(data)
+ *         payload_u8 = payload_bytes             # <<<<<<<<<<<<<<
+ *         if 0 != payload_length:
+ *             payload_u8_ptr = &payload_u8[0]
+ */
+  __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_v_payload_bytes, 0); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_v_payload_u8 = __pyx_t_11;
+  __pyx_t_11.memview = NULL;
+  __pyx_t_11.data = NULL;
+
+  /* "pyjls/binding.pyx":364
+ *         storage_type, payload_bytes, payload_length = _storage_pack(data)
+ *         payload_u8 = payload_bytes
+ *         if 0 != payload_length:             # <<<<<<<<<<<<<<
+ *             payload_u8_ptr = &payload_u8[0]
+ *         with nogil:
+ */
+  __pyx_t_12 = ((0 != __pyx_v_payload_length) != 0);
+  if (__pyx_t_12) {
+
+    /* "pyjls/binding.pyx":365
+ *         payload_u8 = payload_bytes
+ *         if 0 != payload_length:
+ *             payload_u8_ptr = &payload_u8[0]             # <<<<<<<<<<<<<<
+ *         with nogil:
+ *             rc = c_jls.jls_twr_user_data(wr, chunk_meta_u16, storage_type, payload_u8_ptr, payload_length)
+ */
+    __pyx_t_13 = 0;
+    __pyx_t_14 = -1;
+    if (__pyx_t_13 < 0) {
+      __pyx_t_13 += __pyx_v_payload_u8.shape[0];
+      if (unlikely(__pyx_t_13 < 0)) __pyx_t_14 = 0;
+    } else if (unlikely(__pyx_t_13 >= __pyx_v_payload_u8.shape[0])) __pyx_t_14 = 0;
+    if (unlikely(__pyx_t_14 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_14);
+      __PYX_ERR(0, 365, __pyx_L1_error)
+    }
+    __pyx_v_payload_u8_ptr = (&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_payload_u8.data + __pyx_t_13 * __pyx_v_payload_u8.strides[0]) ))));
+
+    /* "pyjls/binding.pyx":364
+ *         storage_type, payload_bytes, payload_length = _storage_pack(data)
+ *         payload_u8 = payload_bytes
+ *         if 0 != payload_length:             # <<<<<<<<<<<<<<
+ *             payload_u8_ptr = &payload_u8[0]
+ *         with nogil:
+ */
+  }
+
+  /* "pyjls/binding.pyx":366
+ *         if 0 != payload_length:
+ *             payload_u8_ptr = &payload_u8[0]
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_user_data(wr, chunk_meta_u16, storage_type, payload_u8_ptr, payload_length)
+ * 
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "pyjls/binding.pyx":367
+ *             payload_u8_ptr = &payload_u8[0]
+ *         with nogil:
+ *             rc = c_jls.jls_twr_user_data(wr, chunk_meta_u16, storage_type, payload_u8_ptr, payload_length)             # <<<<<<<<<<<<<<
+ * 
  *         _handle_rc('user_data', rc)
+ */
+        __pyx_v_rc = jls_twr_user_data(__pyx_v_wr, __pyx_v_chunk_meta_u16, __pyx_v_storage_type, __pyx_v_payload_u8_ptr, __pyx_v_payload_length);
+      }
+
+      /* "pyjls/binding.pyx":366
+ *         if 0 != payload_length:
+ *             payload_u8_ptr = &payload_u8[0]
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_user_data(wr, chunk_meta_u16, storage_type, payload_u8_ptr, payload_length)
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_chunk_meta); if (unlikely((__pyx_t_7 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
-  __pyx_t_8 = ((enum jls_storage_type_e)__Pyx_PyInt_As_enum__jls_storage_type_e(__pyx_v_storage_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_PyObject_AsUString(__pyx_v_payload); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyInt_As_uint32_t(__pyx_v_payload_length); if (unlikely((__pyx_t_10 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
-  __pyx_v_rc = jls_twr_user_data(__pyx_v_self->_wr, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10);
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L8;
+        }
+        __pyx_L8:;
+      }
+  }
 
-  /* "pyjls/binding.pyx":347
- *         storage_type, payload, payload_length = _storage_pack(data)
- *         rc = c_jls.jls_twr_user_data(self._wr, chunk_meta, storage_type, payload, payload_length)
+  /* "pyjls/binding.pyx":369
+ *             rc = c_jls.jls_twr_user_data(wr, chunk_meta_u16, storage_type, payload_u8_ptr, payload_length)
+ * 
  *         _handle_rc('user_data', rc)             # <<<<<<<<<<<<<<
  * 
  *     def fsr_f32(self, signal_id, sample_id, data):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 347, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = NULL;
-  __pyx_t_11 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_2)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_2);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = NULL;
+  __pyx_t_14 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
-      __pyx_t_11 = 1;
+      __Pyx_DECREF_SET(__pyx_t_6, function);
+      __pyx_t_14 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_n_u_user_data, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyFunction_Check(__pyx_t_6)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_user_data, __pyx_t_5};
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_14, 2+__pyx_t_14); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_n_u_user_data, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_user_data, __pyx_t_5};
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_14, 2+__pyx_t_14); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (__pyx_t_2) {
-      __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2); __pyx_t_2 = NULL;
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_14); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    if (__pyx_t_4) {
+      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_user_data);
     __Pyx_GIVEREF(__pyx_n_u_user_data);
-    PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_11, __pyx_n_u_user_data);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_11, __pyx_t_3);
-    __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_14, __pyx_n_u_user_data);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_14, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":343
+  /* "pyjls/binding.pyx":354
  *                                units=s.units)
  * 
  *     def user_data(self, chunk_meta, data):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
- *         storage_type, payload, payload_length = _storage_pack(data)
+ *         cdef uint16_t chunk_meta_u16 = chunk_meta
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_11, 1);
   __Pyx_AddTraceback("pyjls.binding.Writer.user_data", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_storage_type);
-  __Pyx_XDECREF(__pyx_v_payload);
-  __Pyx_XDECREF(__pyx_v_payload_length);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_payload_u8, 1);
+  __Pyx_XDECREF(__pyx_v_payload_bytes);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":349
+/* "pyjls/binding.pyx":371
  *         _handle_rc('user_data', rc)
  * 
  *     def fsr_f32(self, signal_id, sample_id, data):             # <<<<<<<<<<<<<<
  *         return self.fsr(signal_id, sample_id, data)
  * 
  */
 
@@ -7877,40 +8237,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, 1); __PYX_ERR(0, 349, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, 1); __PYX_ERR(0, 371, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, 2); __PYX_ERR(0, 349, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, 2); __PYX_ERR(0, 371, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr_f32") < 0)) __PYX_ERR(0, 349, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr_f32") < 0)) __PYX_ERR(0, 371, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
     __pyx_v_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 349, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fsr_f32", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 371, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.fsr_f32", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_20fsr_f32(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_data);
 
@@ -7928,23 +8288,23 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fsr_f32", 0);
 
-  /* "pyjls/binding.pyx":350
+  /* "pyjls/binding.pyx":372
  * 
  *     def fsr_f32(self, signal_id, sample_id, data):
  *         return self.fsr(signal_id, sample_id, data)             # <<<<<<<<<<<<<<
  * 
  *     def fsr(self, signal_id, sample_id, data):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fsr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_fsr); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7953,52 +8313,52 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_4 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 3+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(3+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_signal_id);
     __Pyx_GIVEREF(__pyx_v_signal_id);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_signal_id);
     __Pyx_INCREF(__pyx_v_sample_id);
     __Pyx_GIVEREF(__pyx_v_sample_id);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_sample_id);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_4, __pyx_v_data);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 372, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":349
+  /* "pyjls/binding.pyx":371
  *         _handle_rc('user_data', rc)
  * 
  *     def fsr_f32(self, signal_id, sample_id, data):             # <<<<<<<<<<<<<<
  *         return self.fsr(signal_id, sample_id, data)
  * 
  */
 
@@ -8012,20 +8372,20 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":352
+/* "pyjls/binding.pyx":374
  *         return self.fsr(signal_id, sample_id, data)
  * 
  *     def fsr(self, signal_id, sample_id, data):             # <<<<<<<<<<<<<<
- *         cdef int32_t rc
- *         cdef np.uint8_t [::1] u8
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_23fsr(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_23fsr(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_signal_id = 0;
   PyObject *__pyx_v_sample_id = 0;
@@ -8057,400 +8417,474 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 1); __PYX_ERR(0, 352, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 1); __PYX_ERR(0, 374, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 2); __PYX_ERR(0, 352, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 2); __PYX_ERR(0, 374, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr") < 0)) __PYX_ERR(0, 352, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr") < 0)) __PYX_ERR(0, 374, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
     __pyx_v_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 352, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 374, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.fsr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_22fsr(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_22fsr(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_sample_id, PyObject *__pyx_v_data) {
+  struct jls_twr_s *__pyx_v_wr;
+  uint16_t __pyx_v_signal_id_u16;
+  int64_t __pyx_v_sample_id_i64;
   int32_t __pyx_v_rc;
   __Pyx_memviewslice __pyx_v_u8 = { 0, 0, { 0 }, { 0 }, { 0 } };
   uint32_t __pyx_v_data_type;
   uint32_t __pyx_v_entry_size_bits;
   uint32_t __pyx_v_length;
   PyObject *__pyx_v_np_type = NULL;
   PyObject *__pyx_v_data_u8 = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  Py_ssize_t __pyx_t_1;
-  uint32_t __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  long __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  Py_UCS4 __pyx_t_7;
+  struct jls_twr_s *__pyx_t_1;
+  uint16_t __pyx_t_2;
+  int64_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  uint32_t __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  long __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  __Pyx_memviewslice __pyx_t_10 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  uint16_t __pyx_t_11;
-  int64_t __pyx_t_12;
-  Py_ssize_t __pyx_t_13;
-  int __pyx_t_14;
-  PyObject *__pyx_t_15 = NULL;
+  int __pyx_t_9;
+  Py_UCS4 __pyx_t_10;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  __Pyx_memviewslice __pyx_t_13 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  Py_ssize_t __pyx_t_14;
+  int __pyx_t_15;
+  PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fsr", 0);
 
-  /* "pyjls/binding.pyx":359
+  /* "pyjls/binding.pyx":375
+ * 
+ *     def fsr(self, signal_id, sample_id, data):
+ *         cdef c_jls.jls_twr_s * wr = self._wr             # <<<<<<<<<<<<<<
+ *         cdef uint16_t signal_id_u16 = signal_id
+ *         cdef int64_t sample_id_i64 = sample_id
+ */
+  __pyx_t_1 = __pyx_v_self->_wr;
+  __pyx_v_wr = __pyx_t_1;
+
+  /* "pyjls/binding.pyx":376
+ *     def fsr(self, signal_id, sample_id, data):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id             # <<<<<<<<<<<<<<
+ *         cdef int64_t sample_id_i64 = sample_id
+ *         cdef int32_t rc
+ */
+  __pyx_t_2 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_2 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_v_signal_id_u16 = __pyx_t_2;
+
+  /* "pyjls/binding.pyx":377
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
+ *         cdef int64_t sample_id_i64 = sample_id             # <<<<<<<<<<<<<<
+ *         cdef int32_t rc
+ *         cdef np.uint8_t [::1] u8
+ */
+  __pyx_t_3 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_3 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_v_sample_id_i64 = __pyx_t_3;
+
+  /* "pyjls/binding.pyx":384
  *         cdef uint32_t length
  * 
  *         data_type = self._signals[signal_id].data_type             # <<<<<<<<<<<<<<
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  */
-  __pyx_t_1 = __Pyx_PyIndex_AsSsize_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 359, __pyx_L1_error)
-  __pyx_t_2 = (__pyx_v_self->_signals[__pyx_t_1]).data_type;
-  __pyx_v_data_type = __pyx_t_2;
+  __pyx_t_4 = __Pyx_PyIndex_AsSsize_t(__pyx_v_signal_id); if (unlikely((__pyx_t_4 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_t_5 = (__pyx_v_self->_signals[__pyx_t_4]).data_type;
+  __pyx_v_data_type = __pyx_t_5;
 
-  /* "pyjls/binding.pyx":360
+  /* "pyjls/binding.pyx":385
  * 
  *         data_type = self._signals[signal_id].data_type
  *         entry_size_bits = (data_type >> 8) & 0xff             # <<<<<<<<<<<<<<
  *         np_type = _data_type_map[data_type & 0xffff]
  *         if np_type != data.dtype:
  */
   __pyx_v_entry_size_bits = ((__pyx_v_data_type >> 8) & 0xff);
 
-  /* "pyjls/binding.pyx":361
+  /* "pyjls/binding.pyx":386
  *         data_type = self._signals[signal_id].data_type
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]             # <<<<<<<<<<<<<<
  *         if np_type != data.dtype:
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_data_type_map); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 361, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = (__pyx_v_data_type & 0xffff);
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_3, __pyx_t_4, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 361, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_np_type = __pyx_t_5;
-  __pyx_t_5 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_data_type_map); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_7 = (__pyx_v_data_type & 0xffff);
+  __pyx_t_8 = __Pyx_GetItemInt(__pyx_t_6, __pyx_t_7, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_v_np_type = __pyx_t_8;
+  __pyx_t_8 = 0;
 
-  /* "pyjls/binding.pyx":362
+  /* "pyjls/binding.pyx":387
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  *         if np_type != data.dtype:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  *         data_u8 = data.view(dtype=np.uint8)
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 362, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_v_np_type, __pyx_t_5, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 362, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 362, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(__pyx_t_6)) {
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dtype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_6 = PyObject_RichCompare(__pyx_v_np_type, __pyx_t_8, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (unlikely(__pyx_t_9)) {
 
-    /* "pyjls/binding.pyx":363
+    /* "pyjls/binding.pyx":388
  *         np_type = _data_type_map[data_type & 0xffff]
  *         if np_type != data.dtype:
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')             # <<<<<<<<<<<<<<
  *         data_u8 = data.view(dtype=np.uint8)
  *         u8 = data_u8
  */
-    __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = 0;
-    __pyx_t_7 = 127;
+    __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = 0;
+    __pyx_t_10 = 127;
     __Pyx_INCREF(__pyx_kp_u_Data_type_mismatch);
-    __pyx_t_1 += 19;
+    __pyx_t_4 += 19;
     __Pyx_GIVEREF(__pyx_kp_u_Data_type_mismatch);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_Data_type_mismatch);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dtype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 363, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 363, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
-    __pyx_t_1 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_8);
-    __pyx_t_8 = 0;
-    __Pyx_INCREF(__pyx_kp_u__7);
-    __pyx_t_1 += 4;
-    __Pyx_GIVEREF(__pyx_kp_u__7);
-    PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u__7);
-    __pyx_t_8 = __Pyx_PyObject_FormatSimple(__pyx_v_np_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 363, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) > __pyx_t_7) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_8) : __pyx_t_7;
-    __pyx_t_1 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_8);
-    __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_t_8);
-    __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyUnicode_Join(__pyx_t_3, 4, __pyx_t_1, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 363, __pyx_L1_error)
+    PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_kp_u_Data_type_mismatch);
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_dtype); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 363, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_11 = __Pyx_PyObject_FormatSimple(__pyx_t_8, __pyx_empty_unicode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 363, __pyx_L1_error)
+    __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_11) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_11) : __pyx_t_10;
+    __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_11);
+    __Pyx_GIVEREF(__pyx_t_11);
+    PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_11);
+    __pyx_t_11 = 0;
+    __Pyx_INCREF(__pyx_kp_u__8);
+    __pyx_t_4 += 4;
+    __Pyx_GIVEREF(__pyx_kp_u__8);
+    PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_kp_u__8);
+    __pyx_t_11 = __Pyx_PyObject_FormatSimple(__pyx_v_np_type, __pyx_empty_unicode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_11) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_11) : __pyx_t_10;
+    __pyx_t_4 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_11);
+    __Pyx_GIVEREF(__pyx_t_11);
+    PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_11);
+    __pyx_t_11 = 0;
+    __pyx_t_11 = __Pyx_PyUnicode_Join(__pyx_t_6, 4, __pyx_t_4, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+    __Pyx_Raise(__pyx_t_6, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __PYX_ERR(0, 388, __pyx_L1_error)
 
-    /* "pyjls/binding.pyx":362
+    /* "pyjls/binding.pyx":387
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  *         if np_type != data.dtype:             # <<<<<<<<<<<<<<
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  *         data_u8 = data.view(dtype=np.uint8)
  */
   }
 
-  /* "pyjls/binding.pyx":364
+  /* "pyjls/binding.pyx":389
  *         if np_type != data.dtype:
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  *         data_u8 = data.view(dtype=np.uint8)             # <<<<<<<<<<<<<<
  *         u8 = data_u8
  *         length = len(data)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_view); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 364, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 364, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_data, __pyx_n_s_view); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 364, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uint8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 364, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 364, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 364, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint8); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_v_data_u8 = __pyx_t_9;
-  __pyx_t_9 = 0;
+  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __pyx_v_data_u8 = __pyx_t_12;
+  __pyx_t_12 = 0;
 
-  /* "pyjls/binding.pyx":365
+  /* "pyjls/binding.pyx":390
  *             raise ValueError(f'Data type mismatch {data.dtype} != {np_type}')
  *         data_u8 = data.view(dtype=np.uint8)
  *         u8 = data_u8             # <<<<<<<<<<<<<<
  *         length = len(data)
  *         if entry_size_bits == 4:
  */
-  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_data_u8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 365, __pyx_L1_error)
-  __pyx_v_u8 = __pyx_t_10;
-  __pyx_t_10.memview = NULL;
-  __pyx_t_10.data = NULL;
+  __pyx_t_13 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_data_u8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_13.memview)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_v_u8 = __pyx_t_13;
+  __pyx_t_13.memview = NULL;
+  __pyx_t_13.data = NULL;
 
-  /* "pyjls/binding.pyx":366
+  /* "pyjls/binding.pyx":391
  *         data_u8 = data.view(dtype=np.uint8)
  *         u8 = data_u8
  *         length = len(data)             # <<<<<<<<<<<<<<
  *         if entry_size_bits == 4:
  *             length *= 2
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 366, __pyx_L1_error)
-  __pyx_v_length = __pyx_t_1;
+  __pyx_t_4 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_v_length = __pyx_t_4;
 
-  /* "pyjls/binding.pyx":367
+  /* "pyjls/binding.pyx":392
  *         u8 = data_u8
  *         length = len(data)
  *         if entry_size_bits == 4:             # <<<<<<<<<<<<<<
  *             length *= 2
  *         elif entry_size_bits == 1:
  */
   switch (__pyx_v_entry_size_bits) {
     case 4:
 
-    /* "pyjls/binding.pyx":368
+    /* "pyjls/binding.pyx":393
  *         length = len(data)
  *         if entry_size_bits == 4:
  *             length *= 2             # <<<<<<<<<<<<<<
  *         elif entry_size_bits == 1:
  *             length *= 8
  */
     __pyx_v_length = (__pyx_v_length * 2);
 
-    /* "pyjls/binding.pyx":367
+    /* "pyjls/binding.pyx":392
  *         u8 = data_u8
  *         length = len(data)
  *         if entry_size_bits == 4:             # <<<<<<<<<<<<<<
  *             length *= 2
  *         elif entry_size_bits == 1:
  */
     break;
     case 1:
 
-    /* "pyjls/binding.pyx":370
+    /* "pyjls/binding.pyx":395
  *             length *= 2
  *         elif entry_size_bits == 1:
  *             length *= 8             # <<<<<<<<<<<<<<
- *         rc = c_jls.jls_twr_fsr(self._wr, signal_id, sample_id, &u8[0], length)
- *         _handle_rc('fsr', rc)
+ *         with nogil:
+ *             rc = c_jls.jls_twr_fsr(wr, signal_id_u16, sample_id_i64, &u8[0], length)
  */
     __pyx_v_length = (__pyx_v_length * 8);
 
-    /* "pyjls/binding.pyx":369
+    /* "pyjls/binding.pyx":394
  *         if entry_size_bits == 4:
  *             length *= 2
  *         elif entry_size_bits == 1:             # <<<<<<<<<<<<<<
  *             length *= 8
- *         rc = c_jls.jls_twr_fsr(self._wr, signal_id, sample_id, &u8[0], length)
+ *         with nogil:
  */
     break;
     default: break;
   }
 
-  /* "pyjls/binding.pyx":371
+  /* "pyjls/binding.pyx":396
  *         elif entry_size_bits == 1:
  *             length *= 8
- *         rc = c_jls.jls_twr_fsr(self._wr, signal_id, sample_id, &u8[0], length)             # <<<<<<<<<<<<<<
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_fsr(wr, signal_id_u16, sample_id_i64, &u8[0], length)
+ *         _handle_rc('fsr', rc)
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "pyjls/binding.pyx":397
+ *             length *= 8
+ *         with nogil:
+ *             rc = c_jls.jls_twr_fsr(wr, signal_id_u16, sample_id_i64, &u8[0], length)             # <<<<<<<<<<<<<<
  *         _handle_rc('fsr', rc)
  * 
  */
-  __pyx_t_11 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_11 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
-  __pyx_t_12 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_12 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
-  __pyx_t_13 = 0;
-  __pyx_t_14 = -1;
-  if (__pyx_t_13 < 0) {
-    __pyx_t_13 += __pyx_v_u8.shape[0];
-    if (unlikely(__pyx_t_13 < 0)) __pyx_t_14 = 0;
-  } else if (unlikely(__pyx_t_13 >= __pyx_v_u8.shape[0])) __pyx_t_14 = 0;
-  if (unlikely(__pyx_t_14 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_14);
-    __PYX_ERR(0, 371, __pyx_L1_error)
-  }
-  __pyx_v_rc = jls_twr_fsr(__pyx_v_self->_wr, __pyx_t_11, __pyx_t_12, (&(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_u8.data) + __pyx_t_13)) )))), __pyx_v_length);
+        __pyx_t_14 = 0;
+        __pyx_t_15 = -1;
+        if (__pyx_t_14 < 0) {
+          __pyx_t_14 += __pyx_v_u8.shape[0];
+          if (unlikely(__pyx_t_14 < 0)) __pyx_t_15 = 0;
+        } else if (unlikely(__pyx_t_14 >= __pyx_v_u8.shape[0])) __pyx_t_15 = 0;
+        if (unlikely(__pyx_t_15 != -1)) {
+          __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_15);
+          __PYX_ERR(0, 397, __pyx_L5_error)
+        }
+        __pyx_v_rc = jls_twr_fsr(__pyx_v_wr, __pyx_v_signal_id_u16, __pyx_v_sample_id_i64, (&(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_u8.data) + __pyx_t_14)) )))), __pyx_v_length);
+      }
 
-  /* "pyjls/binding.pyx":372
+      /* "pyjls/binding.pyx":396
+ *         elif entry_size_bits == 1:
  *             length *= 8
- *         rc = c_jls.jls_twr_fsr(self._wr, signal_id, sample_id, &u8[0], length)
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_fsr(wr, signal_id_u16, sample_id_i64, &u8[0], length)
+ *         _handle_rc('fsr', rc)
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L6;
+        }
+        __pyx_L5_error: {
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L6:;
+      }
+  }
+
+  /* "pyjls/binding.pyx":398
+ *         with nogil:
+ *             rc = c_jls.jls_twr_fsr(wr, signal_id_u16, sample_id_i64, &u8[0], length)
  *         _handle_rc('fsr', rc)             # <<<<<<<<<<<<<<
  * 
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 372, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 372, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = NULL;
-  __pyx_t_14 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-      __Pyx_INCREF(__pyx_t_5);
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_8 = NULL;
+  __pyx_t_15 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_11);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+      __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_8, function);
-      __pyx_t_14 = 1;
+      __Pyx_DECREF_SET(__pyx_t_11, function);
+      __pyx_t_15 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_8)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_fsr, __pyx_t_3};
-    __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_14, 2+__pyx_t_14); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyFunction_Check(__pyx_t_11)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_u_fsr, __pyx_t_6};
+    __pyx_t_12 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 398, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_fsr, __pyx_t_3};
-    __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_14, 2+__pyx_t_14); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_11)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_n_u_fsr, __pyx_t_6};
+    __pyx_t_12 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 398, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_15 = PyTuple_New(2+__pyx_t_14); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 372, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_15);
-    if (__pyx_t_5) {
-      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_5); __pyx_t_5 = NULL;
+    __pyx_t_16 = PyTuple_New(2+__pyx_t_15); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 398, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_16);
+    if (__pyx_t_8) {
+      __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_t_8); __pyx_t_8 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_fsr);
     __Pyx_GIVEREF(__pyx_n_u_fsr);
-    PyTuple_SET_ITEM(__pyx_t_15, 0+__pyx_t_14, __pyx_n_u_fsr);
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_15, 1+__pyx_t_14, __pyx_t_3);
-    __pyx_t_3 = 0;
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_15, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 372, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
-    __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+    PyTuple_SET_ITEM(__pyx_t_16, 0+__pyx_t_15, __pyx_n_u_fsr);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_16, 1+__pyx_t_15, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_16, NULL); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 398, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
   }
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-  /* "pyjls/binding.pyx":352
+  /* "pyjls/binding.pyx":374
  *         return self.fsr(signal_id, sample_id, data)
  * 
  *     def fsr(self, signal_id, sample_id, data):             # <<<<<<<<<<<<<<
- *         cdef int32_t rc
- *         cdef np.uint8_t [::1] u8
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_10, 1);
-  __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_13, 1);
+  __Pyx_XDECREF(__pyx_t_16);
   __Pyx_AddTraceback("pyjls.binding.Writer.fsr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_u8, 1);
   __Pyx_XDECREF(__pyx_v_np_type);
   __Pyx_XDECREF(__pyx_v_data_u8);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":374
+/* "pyjls/binding.pyx":400
  *         _handle_rc('fsr', rc)
  * 
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):             # <<<<<<<<<<<<<<
- *         cdef int32_t rc
- *         if isinstance(annotation_type, str):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_25annotation(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_25annotation(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_signal_id = 0;
   PyObject *__pyx_v_timestamp = 0;
@@ -8491,43 +8925,43 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timestamp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 1); __PYX_ERR(0, 374, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 1); __PYX_ERR(0, 400, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_y)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 2); __PYX_ERR(0, 374, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 2); __PYX_ERR(0, 400, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_annotation_type)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 3); __PYX_ERR(0, 374, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 3); __PYX_ERR(0, 400, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_group_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 4); __PYX_ERR(0, 374, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 4); __PYX_ERR(0, 400, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 5); __PYX_ERR(0, 374, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, 5); __PYX_ERR(0, 400, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "annotation") < 0)) __PYX_ERR(0, 374, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "annotation") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 6) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -8540,387 +8974,539 @@
     __pyx_v_y = values[2];
     __pyx_v_annotation_type = values[3];
     __pyx_v_group_id = values[4];
     __pyx_v_data = values[5];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 374, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("annotation", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 400, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.annotation", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_24annotation(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_timestamp, __pyx_v_y, __pyx_v_annotation_type, __pyx_v_group_id, __pyx_v_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_24annotation(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_timestamp, PyObject *__pyx_v_y, PyObject *__pyx_v_annotation_type, PyObject *__pyx_v_group_id, PyObject *__pyx_v_data) {
+  struct jls_twr_s *__pyx_v_wr;
+  uint16_t __pyx_v_signal_id_u16;
+  int64_t __pyx_v_timestamp_i64;
+  uint8_t __pyx_v_group_id_u8;
+  float __pyx_v_y_f32;
+  enum jls_annotation_type_e __pyx_v_annotation_type_e;
+  enum jls_storage_type_e __pyx_v_storage_type;
+  __Pyx_memviewslice __pyx_v_payload_u8 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  uint32_t __pyx_v_payload_length;
   int32_t __pyx_v_rc;
-  PyObject *__pyx_v_storage_type = NULL;
   PyObject *__pyx_v_payload = NULL;
-  PyObject *__pyx_v_payload_length = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_t_2;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *(*__pyx_t_8)(PyObject *);
-  int __pyx_t_9;
-  uint16_t __pyx_t_10;
-  int64_t __pyx_t_11;
-  float __pyx_t_12;
-  enum jls_annotation_type_e __pyx_t_13;
-  uint8_t __pyx_t_14;
+  struct jls_twr_s *__pyx_t_1;
+  uint16_t __pyx_t_2;
+  int64_t __pyx_t_3;
+  uint8_t __pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_t_6;
+  float __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  enum jls_annotation_type_e __pyx_t_12;
+  PyObject *__pyx_t_13 = NULL;
+  PyObject *(*__pyx_t_14)(PyObject *);
   enum jls_storage_type_e __pyx_t_15;
-  uint8_t const *__pyx_t_16;
-  uint32_t __pyx_t_17;
+  uint32_t __pyx_t_16;
+  __Pyx_memviewslice __pyx_t_17 = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_t_18;
+  Py_ssize_t __pyx_t_19;
+  int __pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("annotation", 0);
   __Pyx_INCREF(__pyx_v_y);
   __Pyx_INCREF(__pyx_v_annotation_type);
 
-  /* "pyjls/binding.pyx":376
+  /* "pyjls/binding.pyx":401
+ * 
+ *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):
+ *         cdef c_jls.jls_twr_s * wr = self._wr             # <<<<<<<<<<<<<<
+ *         cdef uint16_t signal_id_u16 = signal_id
+ *         cdef int64_t timestamp_i64 = timestamp
+ */
+  __pyx_t_1 = __pyx_v_self->_wr;
+  __pyx_v_wr = __pyx_t_1;
+
+  /* "pyjls/binding.pyx":402
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id             # <<<<<<<<<<<<<<
+ *         cdef int64_t timestamp_i64 = timestamp
+ *         cdef uint8_t group_id_u8 = group_id
+ */
+  __pyx_t_2 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_2 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_v_signal_id_u16 = __pyx_t_2;
+
+  /* "pyjls/binding.pyx":403
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
+ *         cdef int64_t timestamp_i64 = timestamp             # <<<<<<<<<<<<<<
+ *         cdef uint8_t group_id_u8 = group_id
+ *         cdef float y_f32
+ */
+  __pyx_t_3 = __Pyx_PyInt_As_int64_t(__pyx_v_timestamp); if (unlikely((__pyx_t_3 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_v_timestamp_i64 = __pyx_t_3;
+
+  /* "pyjls/binding.pyx":404
+ *         cdef uint16_t signal_id_u16 = signal_id
+ *         cdef int64_t timestamp_i64 = timestamp
+ *         cdef uint8_t group_id_u8 = group_id             # <<<<<<<<<<<<<<
+ *         cdef float y_f32
+ *         cdef c_jls.jls_annotation_type_e annotation_type_e
+ */
+  __pyx_t_4 = __Pyx_PyInt_As_uint8_t(__pyx_v_group_id); if (unlikely((__pyx_t_4 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_v_group_id_u8 = __pyx_t_4;
+
+  /* "pyjls/binding.pyx":412
  *         cdef int32_t rc
+ * 
+ *         if y is None:             # <<<<<<<<<<<<<<
+ *             y_f32 = NAN
+ *         else:
+ */
+  __pyx_t_5 = (__pyx_v_y == Py_None);
+  __pyx_t_6 = (__pyx_t_5 != 0);
+  if (__pyx_t_6) {
+
+    /* "pyjls/binding.pyx":413
+ * 
+ *         if y is None:
+ *             y_f32 = NAN             # <<<<<<<<<<<<<<
+ *         else:
+ *             y_f32 = y
+ */
+    __pyx_v_y_f32 = NAN;
+
+    /* "pyjls/binding.pyx":412
+ *         cdef int32_t rc
+ * 
+ *         if y is None:             # <<<<<<<<<<<<<<
+ *             y_f32 = NAN
+ *         else:
+ */
+    goto __pyx_L3;
+  }
+
+  /* "pyjls/binding.pyx":415
+ *             y_f32 = NAN
+ *         else:
+ *             y_f32 = y             # <<<<<<<<<<<<<<
+ *         if isinstance(annotation_type, str):
+ *             annotation_type = _annotation_map[annotation_type.lower()]
+ */
+  /*else*/ {
+    __pyx_t_7 = __pyx_PyFloat_AsFloat(__pyx_v_y); if (unlikely((__pyx_t_7 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_v_y_f32 = __pyx_t_7;
+  }
+  __pyx_L3:;
+
+  /* "pyjls/binding.pyx":416
+ *         else:
+ *             y_f32 = y
  *         if isinstance(annotation_type, str):             # <<<<<<<<<<<<<<
  *             annotation_type = _annotation_map[annotation_type.lower()]
- *         storage_type, payload, payload_length = _storage_pack(data)
+ *         annotation_type_e = annotation_type
  */
-  __pyx_t_1 = PyUnicode_Check(__pyx_v_annotation_type); 
-  __pyx_t_2 = (__pyx_t_1 != 0);
-  if (__pyx_t_2) {
+  __pyx_t_6 = PyUnicode_Check(__pyx_v_annotation_type); 
+  __pyx_t_5 = (__pyx_t_6 != 0);
+  if (__pyx_t_5) {
 
-    /* "pyjls/binding.pyx":377
- *         cdef int32_t rc
+    /* "pyjls/binding.pyx":417
+ *             y_f32 = y
  *         if isinstance(annotation_type, str):
  *             annotation_type = _annotation_map[annotation_type.lower()]             # <<<<<<<<<<<<<<
+ *         annotation_type_e = annotation_type
  *         storage_type, payload, payload_length = _storage_pack(data)
- *         if y is None or not np.isfinite(y):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_annotation_map); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_annotation_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_6);
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_annotation_map); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_annotation_type, __pyx_n_s_lower); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
+      __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
+      if (likely(__pyx_t_11)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+        __Pyx_INCREF(__pyx_t_11);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_10, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 377, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF_SET(__pyx_v_annotation_type, __pyx_t_5);
-    __pyx_t_5 = 0;
+    __pyx_t_9 = (__pyx_t_11) ? __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_11) : __Pyx_PyObject_CallNoArg(__pyx_t_10);
+    __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+    if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF_SET(__pyx_v_annotation_type, __pyx_t_10);
+    __pyx_t_10 = 0;
 
-    /* "pyjls/binding.pyx":376
- *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):
- *         cdef int32_t rc
+    /* "pyjls/binding.pyx":416
+ *         else:
+ *             y_f32 = y
  *         if isinstance(annotation_type, str):             # <<<<<<<<<<<<<<
  *             annotation_type = _annotation_map[annotation_type.lower()]
- *         storage_type, payload, payload_length = _storage_pack(data)
+ *         annotation_type_e = annotation_type
  */
   }
 
-  /* "pyjls/binding.pyx":378
+  /* "pyjls/binding.pyx":418
  *         if isinstance(annotation_type, str):
  *             annotation_type = _annotation_map[annotation_type.lower()]
+ *         annotation_type_e = annotation_type             # <<<<<<<<<<<<<<
+ *         storage_type, payload, payload_length = _storage_pack(data)
+ *         payload_u8 = payload
+ */
+  __pyx_t_12 = ((enum jls_annotation_type_e)__Pyx_PyInt_As_enum__jls_annotation_type_e(__pyx_v_annotation_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_v_annotation_type_e = __pyx_t_12;
+
+  /* "pyjls/binding.pyx":419
+ *             annotation_type = _annotation_map[annotation_type.lower()]
+ *         annotation_type_e = annotation_type
  *         storage_type, payload, payload_length = _storage_pack(data)             # <<<<<<<<<<<<<<
+ *         payload_u8 = payload
  *         if y is None or not np.isfinite(y):
- *             y = NAN
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_storage_pack); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_3);
+  __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_storage_pack); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_8 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_9);
+    if (likely(__pyx_t_8)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+      __Pyx_INCREF(__pyx_t_8);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_4, function);
+      __Pyx_DECREF_SET(__pyx_t_9, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_data);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if ((likely(PyTuple_CheckExact(__pyx_t_5))) || (PyList_CheckExact(__pyx_t_5))) {
-    PyObject* sequence = __pyx_t_5;
+  __pyx_t_10 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_8, __pyx_v_data) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_data);
+  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  if ((likely(PyTuple_CheckExact(__pyx_t_10))) || (PyList_CheckExact(__pyx_t_10))) {
+    PyObject* sequence = __pyx_t_10;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 378, __pyx_L1_error)
+      __PYX_ERR(0, 419, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
-      __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
-      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
-      __pyx_t_6 = PyTuple_GET_ITEM(sequence, 2); 
-    } else {
-      __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
-      __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
-      __pyx_t_6 = PyList_GET_ITEM(sequence, 2); 
-    }
-    __Pyx_INCREF(__pyx_t_4);
-    __Pyx_INCREF(__pyx_t_3);
-    __Pyx_INCREF(__pyx_t_6);
+      __pyx_t_9 = PyTuple_GET_ITEM(sequence, 0); 
+      __pyx_t_8 = PyTuple_GET_ITEM(sequence, 1); 
+      __pyx_t_11 = PyTuple_GET_ITEM(sequence, 2); 
+    } else {
+      __pyx_t_9 = PyList_GET_ITEM(sequence, 0); 
+      __pyx_t_8 = PyList_GET_ITEM(sequence, 1); 
+      __pyx_t_11 = PyList_GET_ITEM(sequence, 2); 
+    }
+    __Pyx_INCREF(__pyx_t_9);
+    __Pyx_INCREF(__pyx_t_8);
+    __Pyx_INCREF(__pyx_t_11);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 378, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 378, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 378, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_9 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __pyx_t_8 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_11 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_11);
     #endif
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_7 = PyObject_GetIter(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 378, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_8 = Py_TYPE(__pyx_t_7)->tp_iternext;
-    index = 0; __pyx_t_4 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_4)) goto __pyx_L4_unpacking_failed;
-    __Pyx_GOTREF(__pyx_t_4);
-    index = 1; __pyx_t_3 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_3)) goto __pyx_L4_unpacking_failed;
-    __Pyx_GOTREF(__pyx_t_3);
-    index = 2; __pyx_t_6 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_6)) goto __pyx_L4_unpacking_failed;
-    __Pyx_GOTREF(__pyx_t_6);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 3) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
-    __pyx_t_8 = NULL;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    goto __pyx_L5_unpacking_done;
-    __pyx_L4_unpacking_failed:;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_8 = NULL;
+    __pyx_t_13 = PyObject_GetIter(__pyx_t_10); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_13);
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_14 = Py_TYPE(__pyx_t_13)->tp_iternext;
+    index = 0; __pyx_t_9 = __pyx_t_14(__pyx_t_13); if (unlikely(!__pyx_t_9)) goto __pyx_L5_unpacking_failed;
+    __Pyx_GOTREF(__pyx_t_9);
+    index = 1; __pyx_t_8 = __pyx_t_14(__pyx_t_13); if (unlikely(!__pyx_t_8)) goto __pyx_L5_unpacking_failed;
+    __Pyx_GOTREF(__pyx_t_8);
+    index = 2; __pyx_t_11 = __pyx_t_14(__pyx_t_13); if (unlikely(!__pyx_t_11)) goto __pyx_L5_unpacking_failed;
+    __Pyx_GOTREF(__pyx_t_11);
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_14(__pyx_t_13), 3) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_14 = NULL;
+    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    goto __pyx_L6_unpacking_done;
+    __pyx_L5_unpacking_failed:;
+    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    __pyx_t_14 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 378, __pyx_L1_error)
-    __pyx_L5_unpacking_done:;
+    __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_L6_unpacking_done:;
   }
-  __pyx_v_storage_type = __pyx_t_4;
-  __pyx_t_4 = 0;
-  __pyx_v_payload = __pyx_t_3;
-  __pyx_t_3 = 0;
-  __pyx_v_payload_length = __pyx_t_6;
-  __pyx_t_6 = 0;
+  __pyx_t_15 = ((enum jls_storage_type_e)__Pyx_PyInt_As_enum__jls_storage_type_e(__pyx_t_9)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 419, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_16 = __Pyx_PyInt_As_uint32_t(__pyx_t_11); if (unlikely((__pyx_t_16 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 419, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __pyx_v_storage_type = __pyx_t_15;
+  __pyx_v_payload = __pyx_t_8;
+  __pyx_t_8 = 0;
+  __pyx_v_payload_length = __pyx_t_16;
 
-  /* "pyjls/binding.pyx":379
- *             annotation_type = _annotation_map[annotation_type.lower()]
+  /* "pyjls/binding.pyx":420
+ *         annotation_type_e = annotation_type
  *         storage_type, payload, payload_length = _storage_pack(data)
+ *         payload_u8 = payload             # <<<<<<<<<<<<<<
+ *         if y is None or not np.isfinite(y):
+ *             y = NAN
+ */
+  __pyx_t_17 = __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(__pyx_v_payload, 0); if (unlikely(!__pyx_t_17.memview)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_v_payload_u8 = __pyx_t_17;
+  __pyx_t_17.memview = NULL;
+  __pyx_t_17.data = NULL;
+
+  /* "pyjls/binding.pyx":421
+ *         storage_type, payload, payload_length = _storage_pack(data)
+ *         payload_u8 = payload
  *         if y is None or not np.isfinite(y):             # <<<<<<<<<<<<<<
  *             y = NAN
- *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
+ *         with nogil:
  */
-  __pyx_t_1 = (__pyx_v_y == Py_None);
-  __pyx_t_9 = (__pyx_t_1 != 0);
-  if (!__pyx_t_9) {
+  __pyx_t_6 = (__pyx_v_y == Py_None);
+  __pyx_t_18 = (__pyx_t_6 != 0);
+  if (!__pyx_t_18) {
   } else {
-    __pyx_t_2 = __pyx_t_9;
-    goto __pyx_L7_bool_binop_done;
+    __pyx_t_5 = __pyx_t_18;
+    goto __pyx_L8_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 379, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_isfinite); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __pyx_t_11 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
+    __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_8);
+    if (likely(__pyx_t_11)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_11);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __Pyx_DECREF_SET(__pyx_t_8, function);
     }
   }
-  __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_v_y) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_y);
-  __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 379, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 379, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_1 = ((!__pyx_t_9) != 0);
-  __pyx_t_2 = __pyx_t_1;
-  __pyx_L7_bool_binop_done:;
-  if (__pyx_t_2) {
+  __pyx_t_10 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_11, __pyx_v_y) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_y);
+  __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+  if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely(__pyx_t_18 < 0)) __PYX_ERR(0, 421, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_6 = ((!__pyx_t_18) != 0);
+  __pyx_t_5 = __pyx_t_6;
+  __pyx_L8_bool_binop_done:;
+  if (__pyx_t_5) {
 
-    /* "pyjls/binding.pyx":380
- *         storage_type, payload, payload_length = _storage_pack(data)
+    /* "pyjls/binding.pyx":422
+ *         payload_u8 = payload
  *         if y is None or not np.isfinite(y):
  *             y = NAN             # <<<<<<<<<<<<<<
- *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
- *             group_id, storage_type, payload, payload_length)
+ *         with nogil:
+ *             rc = c_jls.jls_twr_annotation(wr, signal_id_u16, timestamp_i64, y_f32,
  */
-    __pyx_t_5 = PyFloat_FromDouble(NAN); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 380, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF_SET(__pyx_v_y, __pyx_t_5);
-    __pyx_t_5 = 0;
+    __pyx_t_10 = PyFloat_FromDouble(NAN); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF_SET(__pyx_v_y, __pyx_t_10);
+    __pyx_t_10 = 0;
 
-    /* "pyjls/binding.pyx":379
- *             annotation_type = _annotation_map[annotation_type.lower()]
+    /* "pyjls/binding.pyx":421
  *         storage_type, payload, payload_length = _storage_pack(data)
+ *         payload_u8 = payload
  *         if y is None or not np.isfinite(y):             # <<<<<<<<<<<<<<
  *             y = NAN
- *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
+ *         with nogil:
  */
   }
 
-  /* "pyjls/binding.pyx":381
+  /* "pyjls/binding.pyx":423
  *         if y is None or not np.isfinite(y):
  *             y = NAN
- *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,             # <<<<<<<<<<<<<<
- *             group_id, storage_type, payload, payload_length)
- *         _handle_rc('annotation', rc)
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_annotation(wr, signal_id_u16, timestamp_i64, y_f32,
+ *                 annotation_type_e,
  */
-  __pyx_t_10 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_10 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_PyInt_As_int64_t(__pyx_v_timestamp); if (unlikely((__pyx_t_11 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
-  __pyx_t_12 = __pyx_PyFloat_AsFloat(__pyx_v_y); if (unlikely((__pyx_t_12 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
-  __pyx_t_13 = ((enum jls_annotation_type_e)__Pyx_PyInt_As_enum__jls_annotation_type_e(__pyx_v_annotation_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 381, __pyx_L1_error)
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
 
-  /* "pyjls/binding.pyx":382
- *             y = NAN
- *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
- *             group_id, storage_type, payload, payload_length)             # <<<<<<<<<<<<<<
+        /* "pyjls/binding.pyx":426
+ *             rc = c_jls.jls_twr_annotation(wr, signal_id_u16, timestamp_i64, y_f32,
+ *                 annotation_type_e,
+ *                 group_id_u8, storage_type, &payload_u8[0], payload_length)             # <<<<<<<<<<<<<<
  *         _handle_rc('annotation', rc)
  * 
  */
-  __pyx_t_14 = __Pyx_PyInt_As_uint8_t(__pyx_v_group_id); if (unlikely((__pyx_t_14 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
-  __pyx_t_15 = ((enum jls_storage_type_e)__Pyx_PyInt_As_enum__jls_storage_type_e(__pyx_v_storage_type)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
-  __pyx_t_16 = __Pyx_PyObject_AsUString(__pyx_v_payload); if (unlikely((!__pyx_t_16) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
-  __pyx_t_17 = __Pyx_PyInt_As_uint32_t(__pyx_v_payload_length); if (unlikely((__pyx_t_17 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 382, __pyx_L1_error)
+        __pyx_t_19 = 0;
+        __pyx_t_20 = -1;
+        if (__pyx_t_19 < 0) {
+          __pyx_t_19 += __pyx_v_payload_u8.shape[0];
+          if (unlikely(__pyx_t_19 < 0)) __pyx_t_20 = 0;
+        } else if (unlikely(__pyx_t_19 >= __pyx_v_payload_u8.shape[0])) __pyx_t_20 = 0;
+        if (unlikely(__pyx_t_20 != -1)) {
+          __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_20);
+          __PYX_ERR(0, 426, __pyx_L11_error)
+        }
+
+        /* "pyjls/binding.pyx":424
+ *             y = NAN
+ *         with nogil:
+ *             rc = c_jls.jls_twr_annotation(wr, signal_id_u16, timestamp_i64, y_f32,             # <<<<<<<<<<<<<<
+ *                 annotation_type_e,
+ *                 group_id_u8, storage_type, &payload_u8[0], payload_length)
+ */
+        __pyx_v_rc = jls_twr_annotation(__pyx_v_wr, __pyx_v_signal_id_u16, __pyx_v_timestamp_i64, __pyx_v_y_f32, __pyx_v_annotation_type_e, __pyx_v_group_id_u8, __pyx_v_storage_type, (&(*((uint8_t const  *) ( /* dim=0 */ (__pyx_v_payload_u8.data + __pyx_t_19 * __pyx_v_payload_u8.strides[0]) )))), __pyx_v_payload_length);
+      }
 
-  /* "pyjls/binding.pyx":381
+      /* "pyjls/binding.pyx":423
  *         if y is None or not np.isfinite(y):
  *             y = NAN
- *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,             # <<<<<<<<<<<<<<
- *             group_id, storage_type, payload, payload_length)
- *         _handle_rc('annotation', rc)
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_annotation(wr, signal_id_u16, timestamp_i64, y_f32,
+ *                 annotation_type_e,
  */
-  __pyx_v_rc = jls_twr_annotation(__pyx_v_self->_wr, __pyx_t_10, __pyx_t_11, __pyx_t_12, __pyx_t_13, __pyx_t_14, __pyx_t_15, __pyx_t_16, __pyx_t_17);
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L12;
+        }
+        __pyx_L11_error: {
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L12:;
+      }
+  }
 
-  /* "pyjls/binding.pyx":383
- *         rc = c_jls.jls_twr_annotation(self._wr, signal_id, timestamp, y, annotation_type,
- *             group_id, storage_type, payload, payload_length)
+  /* "pyjls/binding.pyx":427
+ *                 annotation_type_e,
+ *                 group_id_u8, storage_type, &payload_u8[0], payload_length)
  *         _handle_rc('annotation', rc)             # <<<<<<<<<<<<<<
  * 
  *     def utc(self, signal_id, sample_id, utc_i64):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 383, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 383, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = NULL;
-  __pyx_t_18 = 0;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_11 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_9 = NULL;
+  __pyx_t_20 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
+    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
+    if (likely(__pyx_t_9)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_9);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_18 = 1;
+      __Pyx_DECREF_SET(__pyx_t_8, function);
+      __pyx_t_20 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_annotation, __pyx_t_6};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_18, 2+__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyFunction_Check(__pyx_t_8)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_n_u_annotation, __pyx_t_11};
+    __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_20, 2+__pyx_t_20); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 427, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_annotation, __pyx_t_6};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_18, 2+__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_8)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_n_u_annotation, __pyx_t_11};
+    __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_8, __pyx_temp+1-__pyx_t_20, 2+__pyx_t_20); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 427, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_18); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 383, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (__pyx_t_4) {
-      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
+    __pyx_t_13 = PyTuple_New(2+__pyx_t_20); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 427, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_13);
+    if (__pyx_t_9) {
+      __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_9); __pyx_t_9 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_annotation);
     __Pyx_GIVEREF(__pyx_n_u_annotation);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_18, __pyx_n_u_annotation);
-    __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_18, __pyx_t_6);
-    __pyx_t_6 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_20, __pyx_n_u_annotation);
+    __Pyx_GIVEREF(__pyx_t_11);
+    PyTuple_SET_ITEM(__pyx_t_13, 1+__pyx_t_20, __pyx_t_11);
+    __pyx_t_11 = 0;
+    __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_8, __pyx_t_13, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 427, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "pyjls/binding.pyx":374
+  /* "pyjls/binding.pyx":400
  *         _handle_rc('fsr', rc)
  * 
  *     def annotation(self, signal_id, timestamp, y, annotation_type, group_id, data):             # <<<<<<<<<<<<<<
- *         cdef int32_t rc
- *         if isinstance(annotation_type, str):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_13);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_17, 1);
   __Pyx_AddTraceback("pyjls.binding.Writer.annotation", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_storage_type);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_payload_u8, 1);
   __Pyx_XDECREF(__pyx_v_payload);
-  __Pyx_XDECREF(__pyx_v_payload_length);
   __Pyx_XDECREF(__pyx_v_y);
   __Pyx_XDECREF(__pyx_v_annotation_type);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":385
+/* "pyjls/binding.pyx":429
  *         _handle_rc('annotation', rc)
  * 
  *     def utc(self, signal_id, sample_id, utc_i64):             # <<<<<<<<<<<<<<
- *         cdef int32_t rc
- *         rc = c_jls.jls_twr_utc(self._wr, signal_id, sample_id, utc_i64)
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_27utc(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_pw_5pyjls_7binding_6Writer_27utc(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_signal_id = 0;
   PyObject *__pyx_v_sample_id = 0;
@@ -8952,92 +9538,168 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 1); __PYX_ERR(0, 385, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 1); __PYX_ERR(0, 429, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_utc_i64)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 2); __PYX_ERR(0, 385, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 2); __PYX_ERR(0, 429, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "utc") < 0)) __PYX_ERR(0, 385, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "utc") < 0)) __PYX_ERR(0, 429, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
     __pyx_v_utc_i64 = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 385, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 429, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Writer.utc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Writer_26utc(((struct __pyx_obj_5pyjls_7binding_Writer *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_utc_i64);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Writer_26utc(struct __pyx_obj_5pyjls_7binding_Writer *__pyx_v_self, PyObject *__pyx_v_signal_id, PyObject *__pyx_v_sample_id, PyObject *__pyx_v_utc_i64) {
+  struct jls_twr_s *__pyx_v_wr;
+  uint16_t __pyx_v_signal_id_u16;
+  int64_t __pyx_v_sample_id_i64;
+  int64_t __pyx_v_utc_i64c;
   int32_t __pyx_v_rc;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  uint16_t __pyx_t_1;
-  int64_t __pyx_t_2;
+  struct jls_twr_s *__pyx_t_1;
+  uint16_t __pyx_t_2;
   int64_t __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("utc", 0);
 
-  /* "pyjls/binding.pyx":387
+  /* "pyjls/binding.pyx":430
+ * 
+ *     def utc(self, signal_id, sample_id, utc_i64):
+ *         cdef c_jls.jls_twr_s * wr = self._wr             # <<<<<<<<<<<<<<
+ *         cdef uint16_t signal_id_u16 = signal_id
+ *         cdef int64_t sample_id_i64 = sample_id
+ */
+  __pyx_t_1 = __pyx_v_self->_wr;
+  __pyx_v_wr = __pyx_t_1;
+
+  /* "pyjls/binding.pyx":431
  *     def utc(self, signal_id, sample_id, utc_i64):
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id             # <<<<<<<<<<<<<<
+ *         cdef int64_t sample_id_i64 = sample_id
+ *         cdef int64_t utc_i64c = utc_i64
+ */
+  __pyx_t_2 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_2 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_v_signal_id_u16 = __pyx_t_2;
+
+  /* "pyjls/binding.pyx":432
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
+ *         cdef int64_t sample_id_i64 = sample_id             # <<<<<<<<<<<<<<
+ *         cdef int64_t utc_i64c = utc_i64
  *         cdef int32_t rc
- *         rc = c_jls.jls_twr_utc(self._wr, signal_id, sample_id, utc_i64)             # <<<<<<<<<<<<<<
+ */
+  __pyx_t_3 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_3 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_v_sample_id_i64 = __pyx_t_3;
+
+  /* "pyjls/binding.pyx":433
+ *         cdef uint16_t signal_id_u16 = signal_id
+ *         cdef int64_t sample_id_i64 = sample_id
+ *         cdef int64_t utc_i64c = utc_i64             # <<<<<<<<<<<<<<
+ *         cdef int32_t rc
+ *         with nogil:
+ */
+  __pyx_t_3 = __Pyx_PyInt_As_int64_t(__pyx_v_utc_i64); if (unlikely((__pyx_t_3 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_v_utc_i64c = __pyx_t_3;
+
+  /* "pyjls/binding.pyx":435
+ *         cdef int64_t utc_i64c = utc_i64
+ *         cdef int32_t rc
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_utc(wr, signal_id_u16, sample_id_i64, utc_i64c)
+ *         _handle_rc('utc', rc)
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "pyjls/binding.pyx":436
+ *         cdef int32_t rc
+ *         with nogil:
+ *             rc = c_jls.jls_twr_utc(wr, signal_id_u16, sample_id_i64, utc_i64c)             # <<<<<<<<<<<<<<
  *         _handle_rc('utc', rc)
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyInt_As_int64_t(__pyx_v_utc_i64); if (unlikely((__pyx_t_3 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_v_rc = jls_twr_utc(__pyx_v_self->_wr, __pyx_t_1, __pyx_t_2, __pyx_t_3);
+        __pyx_v_rc = jls_twr_utc(__pyx_v_wr, __pyx_v_signal_id_u16, __pyx_v_sample_id_i64, __pyx_v_utc_i64c);
+      }
 
-  /* "pyjls/binding.pyx":388
+      /* "pyjls/binding.pyx":435
+ *         cdef int64_t utc_i64c = utc_i64
  *         cdef int32_t rc
- *         rc = c_jls.jls_twr_utc(self._wr, signal_id, sample_id, utc_i64)
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             rc = c_jls.jls_twr_utc(wr, signal_id_u16, sample_id_i64, utc_i64c)
+ *         _handle_rc('utc', rc)
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "pyjls/binding.pyx":437
+ *         with nogil:
+ *             rc = c_jls.jls_twr_utc(wr, signal_id_u16, sample_id_i64, utc_i64c)
  *         _handle_rc('utc', rc)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 437, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 437, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -9046,54 +9708,54 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_utc, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_utc, __pyx_t_6};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_utc);
     __Pyx_GIVEREF(__pyx_n_u_utc);
     PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_n_u_utc);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyjls/binding.pyx":385
+  /* "pyjls/binding.pyx":429
  *         _handle_rc('annotation', rc)
  * 
  *     def utc(self, signal_id, sample_id, utc_i64):             # <<<<<<<<<<<<<<
- *         cdef int32_t rc
- *         rc = c_jls.jls_twr_utc(self._wr, signal_id, sample_id, utc_i64)
+ *         cdef c_jls.jls_twr_s * wr = self._wr
+ *         cdef uint16_t signal_id_u16 = signal_id
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
@@ -9139,15 +9801,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -9195,15 +9857,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -9218,15 +9880,15 @@
   __Pyx_AddTraceback("pyjls.binding.Writer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":395
+/* "pyjls/binding.pyx":444
  *     cdef object cbk_fn
  * 
  *     def __init__(self, is_fsr, cbk_fn):             # <<<<<<<<<<<<<<
  *         self.is_fsr = is_fsr
  *         self.cbk_fn = cbk_fn
  */
 
@@ -9260,32 +9922,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_is_fsr)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cbk_fn)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 395, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 444, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 395, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 444, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_is_fsr = values[0];
     __pyx_v_cbk_fn = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 395, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 444, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.AnnotationCallback.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_18AnnotationCallback___init__(((struct __pyx_obj_5pyjls_7binding_AnnotationCallback *)__pyx_v_self), __pyx_v_is_fsr, __pyx_v_cbk_fn);
 
@@ -9299,38 +9961,38 @@
   __Pyx_RefNannyDeclarations
   uint8_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyjls/binding.pyx":396
+  /* "pyjls/binding.pyx":445
  * 
  *     def __init__(self, is_fsr, cbk_fn):
  *         self.is_fsr = is_fsr             # <<<<<<<<<<<<<<
  *         self.cbk_fn = cbk_fn
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_is_fsr); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_is_fsr); if (unlikely((__pyx_t_1 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 445, __pyx_L1_error)
   __pyx_v_self->is_fsr = __pyx_t_1;
 
-  /* "pyjls/binding.pyx":397
+  /* "pyjls/binding.pyx":446
  *     def __init__(self, is_fsr, cbk_fn):
  *         self.is_fsr = is_fsr
  *         self.cbk_fn = cbk_fn             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_INCREF(__pyx_v_cbk_fn);
   __Pyx_GIVEREF(__pyx_v_cbk_fn);
   __Pyx_GOTREF(__pyx_v_self->cbk_fn);
   __Pyx_DECREF(__pyx_v_self->cbk_fn);
   __pyx_v_self->cbk_fn = __pyx_v_cbk_fn;
 
-  /* "pyjls/binding.pyx":395
+  /* "pyjls/binding.pyx":444
  *     cdef object cbk_fn
  * 
  *     def __init__(self, is_fsr, cbk_fn):             # <<<<<<<<<<<<<<
  *         self.is_fsr = is_fsr
  *         self.cbk_fn = cbk_fn
  */
 
@@ -9639,15 +10301,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":405
+/* "pyjls/binding.pyx":454
  *     cdef object _signals
  * 
  *     def __init__(self, path: str):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s * sources
  */
 
@@ -9676,32 +10338,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 405, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 454, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_path = ((PyObject*)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 405, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 454, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 405, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 454, __pyx_L1_error)
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader___init__(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -9741,71 +10403,71 @@
   char const *__pyx_t_18;
   int __pyx_t_19;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyjls/binding.pyx":411
+  /* "pyjls/binding.pyx":460
  *         cdef uint16_t count
  *         cdef int64_t samples
  *         self._sources: Mapping[int, SourceDef] = {}             # <<<<<<<<<<<<<<
  *         self._signals: Mapping[int, SignalDef] = {}
  *         rc = c_jls.jls_rd_open(&self._rd, path.encode('utf-8'))
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_sources);
   __Pyx_DECREF(__pyx_v_self->_sources);
   __pyx_v_self->_sources = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":412
+  /* "pyjls/binding.pyx":461
  *         cdef int64_t samples
  *         self._sources: Mapping[int, SourceDef] = {}
  *         self._signals: Mapping[int, SignalDef] = {}             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_rd_open(&self._rd, path.encode('utf-8'))
  *         _handle_rc('open', rc)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_signals);
   __Pyx_DECREF(__pyx_v_self->_signals);
   __pyx_v_self->_signals = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":413
+  /* "pyjls/binding.pyx":462
  *         self._sources: Mapping[int, SourceDef] = {}
  *         self._signals: Mapping[int, SignalDef] = {}
  *         rc = c_jls.jls_rd_open(&self._rd, path.encode('utf-8'))             # <<<<<<<<<<<<<<
  *         _handle_rc('open', rc)
  * 
  */
   if (unlikely(__pyx_v_path == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 413, __pyx_L1_error)
+    __PYX_ERR(0, 462, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_t_1); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 462, __pyx_L1_error)
   __pyx_v_rc = jls_rd_open((&__pyx_v_self->_rd), __pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":414
+  /* "pyjls/binding.pyx":463
  *         self._signals: Mapping[int, SignalDef] = {}
  *         rc = c_jls.jls_rd_open(&self._rd, path.encode('utf-8'))
  *         _handle_rc('open', rc)             # <<<<<<<<<<<<<<
  * 
  *         rc = c_jls.jls_rd_sources(self._rd, &sources, &count)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -9814,67 +10476,67 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_open, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_n_u_open, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_open);
     __Pyx_GIVEREF(__pyx_n_u_open);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_n_u_open);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":416
+  /* "pyjls/binding.pyx":465
  *         _handle_rc('open', rc)
  * 
  *         rc = c_jls.jls_rd_sources(self._rd, &sources, &count)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_sources', rc)
  *         for i in range(count):
  */
   __pyx_v_rc = jls_rd_sources(__pyx_v_self->_rd, (&__pyx_v_sources), (&__pyx_v_count));
 
-  /* "pyjls/binding.pyx":417
+  /* "pyjls/binding.pyx":466
  * 
  *         rc = c_jls.jls_rd_sources(self._rd, &sources, &count)
  *         _handle_rc('rd_sources', rc)             # <<<<<<<<<<<<<<
  *         for i in range(count):
  *             source_def = SourceDef(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -9883,192 +10545,192 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_sources, __pyx_t_7};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_sources, __pyx_t_7};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   } else
   #endif
   {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 466, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_sources);
     __Pyx_GIVEREF(__pyx_n_u_rd_sources);
     PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_n_u_rd_sources);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_t_7);
     __pyx_t_7 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 466, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":418
+  /* "pyjls/binding.pyx":467
  *         rc = c_jls.jls_rd_sources(self._rd, &sources, &count)
  *         _handle_rc('rd_sources', rc)
  *         for i in range(count):             # <<<<<<<<<<<<<<
  *             source_def = SourceDef(
  *                 source_id=sources[i].source_id,
  */
   __pyx_t_8 = __pyx_v_count;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pyjls/binding.pyx":419
+    /* "pyjls/binding.pyx":468
  *         _handle_rc('rd_sources', rc)
  *         for i in range(count):
  *             source_def = SourceDef(             # <<<<<<<<<<<<<<
  *                 source_id=sources[i].source_id,
  *                 name=sources[i].name.decode('utf-8'),
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SourceDef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SourceDef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "pyjls/binding.pyx":420
+    /* "pyjls/binding.pyx":469
  *         for i in range(count):
  *             source_def = SourceDef(
  *                 source_id=sources[i].source_id,             # <<<<<<<<<<<<<<
  *                 name=sources[i].name.decode('utf-8'),
  *                 vendor=sources[i].vendor.decode('utf-8'),
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 420, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyInt_From_uint16_t((__pyx_v_sources[__pyx_v_i]).source_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_uint16_t((__pyx_v_sources[__pyx_v_i]).source_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_id, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_id, __pyx_t_5) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":421
+    /* "pyjls/binding.pyx":470
  *             source_def = SourceDef(
  *                 source_id=sources[i].source_id,
  *                 name=sources[i].name.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 vendor=sources[i].vendor.decode('utf-8'),
  *                 model=sources[i].model.decode('utf-8'),
  */
     __pyx_t_11 = (__pyx_v_sources[__pyx_v_i]).name;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_11, 0, strlen(__pyx_t_11), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 421, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_11, 0, strlen(__pyx_t_11), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_5) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":422
+    /* "pyjls/binding.pyx":471
  *                 source_id=sources[i].source_id,
  *                 name=sources[i].name.decode('utf-8'),
  *                 vendor=sources[i].vendor.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 model=sources[i].model.decode('utf-8'),
  *                 version=sources[i].version.decode('utf-8'),
  */
     __pyx_t_12 = (__pyx_v_sources[__pyx_v_i]).vendor;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_12, 0, strlen(__pyx_t_12), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_12, 0, strlen(__pyx_t_12), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 471, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vendor, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_vendor, __pyx_t_5) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":423
+    /* "pyjls/binding.pyx":472
  *                 name=sources[i].name.decode('utf-8'),
  *                 vendor=sources[i].vendor.decode('utf-8'),
  *                 model=sources[i].model.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 version=sources[i].version.decode('utf-8'),
  *                 serial_number=sources[i].serial_number.decode('utf-8'))
  */
     __pyx_t_13 = (__pyx_v_sources[__pyx_v_i]).model;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_13, 0, strlen(__pyx_t_13), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 423, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_13, 0, strlen(__pyx_t_13), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 472, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_model, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_model, __pyx_t_5) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":424
+    /* "pyjls/binding.pyx":473
  *                 vendor=sources[i].vendor.decode('utf-8'),
  *                 model=sources[i].model.decode('utf-8'),
  *                 version=sources[i].version.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 serial_number=sources[i].serial_number.decode('utf-8'))
  *             self._sources[sources[i].source_id] = source_def
  */
     __pyx_t_14 = (__pyx_v_sources[__pyx_v_i]).version;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_14, 0, strlen(__pyx_t_14), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 424, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_14, 0, strlen(__pyx_t_14), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 473, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_version, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_version, __pyx_t_5) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":425
+    /* "pyjls/binding.pyx":474
  *                 model=sources[i].model.decode('utf-8'),
  *                 version=sources[i].version.decode('utf-8'),
  *                 serial_number=sources[i].serial_number.decode('utf-8'))             # <<<<<<<<<<<<<<
  *             self._sources[sources[i].source_id] = source_def
  * 
  */
     __pyx_t_15 = (__pyx_v_sources[__pyx_v_i]).serial_number;
-    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_15, 0, strlen(__pyx_t_15), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 425, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_decode_c_string(__pyx_t_15, 0, strlen(__pyx_t_15), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 474, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_serial_number, __pyx_t_5) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_serial_number, __pyx_t_5) < 0) __PYX_ERR(0, 469, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":419
+    /* "pyjls/binding.pyx":468
  *         _handle_rc('rd_sources', rc)
  *         for i in range(count):
  *             source_def = SourceDef(             # <<<<<<<<<<<<<<
  *                 source_id=sources[i].source_id,
  *                 name=sources[i].name.decode('utf-8'),
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_source_def, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":426
+    /* "pyjls/binding.pyx":475
  *                 version=sources[i].version.decode('utf-8'),
  *                 serial_number=sources[i].serial_number.decode('utf-8'))
  *             self._sources[sources[i].source_id] = source_def             # <<<<<<<<<<<<<<
  * 
  *         rc = c_jls.jls_rd_signals(self._rd, &signals, &count)
  */
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->_sources, (__pyx_v_sources[__pyx_v_i]).source_id, __pyx_v_source_def, uint16_t, 0, __Pyx_PyInt_From_uint16_t, 0, 0, 1) < 0)) __PYX_ERR(0, 426, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->_sources, (__pyx_v_sources[__pyx_v_i]).source_id, __pyx_v_source_def, uint16_t, 0, __Pyx_PyInt_From_uint16_t, 0, 0, 1) < 0)) __PYX_ERR(0, 475, __pyx_L1_error)
   }
 
-  /* "pyjls/binding.pyx":428
+  /* "pyjls/binding.pyx":477
  *             self._sources[sources[i].source_id] = source_def
  * 
  *         rc = c_jls.jls_rd_signals(self._rd, &signals, &count)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_signals', rc)
  *         for i in range(count):
  */
   __pyx_v_rc = jls_rd_signals(__pyx_v_self->_rd, (&__pyx_v_signals), (&__pyx_v_count));
 
-  /* "pyjls/binding.pyx":429
+  /* "pyjls/binding.pyx":478
  * 
  *         rc = c_jls.jls_rd_signals(self._rd, &signals, &count)
  *         _handle_rc('rd_signals', rc)             # <<<<<<<<<<<<<<
  *         for i in range(count):
  *             signal_id = signals[i].signal_id
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -10077,303 +10739,303 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_rd_signals, __pyx_t_1};
-    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 429, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_n_u_rd_signals, __pyx_t_1};
-    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 429, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 429, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_signals);
     __Pyx_GIVEREF(__pyx_n_u_rd_signals);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_n_u_rd_signals);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 429, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "pyjls/binding.pyx":430
+  /* "pyjls/binding.pyx":479
  *         rc = c_jls.jls_rd_signals(self._rd, &signals, &count)
  *         _handle_rc('rd_signals', rc)
  *         for i in range(count):             # <<<<<<<<<<<<<<
  *             signal_id = signals[i].signal_id
  *             signal_def = SignalDef(
  */
   __pyx_t_8 = __pyx_v_count;
   __pyx_t_9 = __pyx_t_8;
   for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
     __pyx_v_i = __pyx_t_10;
 
-    /* "pyjls/binding.pyx":431
+    /* "pyjls/binding.pyx":480
  *         _handle_rc('rd_signals', rc)
  *         for i in range(count):
  *             signal_id = signals[i].signal_id             # <<<<<<<<<<<<<<
  *             signal_def = SignalDef(
  *                 signal_id=signal_id,
  */
     __pyx_t_16 = (__pyx_v_signals[__pyx_v_i]).signal_id;
     __pyx_v_signal_id = __pyx_t_16;
 
-    /* "pyjls/binding.pyx":432
+    /* "pyjls/binding.pyx":481
  *         for i in range(count):
  *             signal_id = signals[i].signal_id
  *             signal_def = SignalDef(             # <<<<<<<<<<<<<<
  *                 signal_id=signal_id,
  *                 source_id=signals[i].source_id,
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SignalDef); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 432, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_SignalDef); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 481, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
 
-    /* "pyjls/binding.pyx":433
+    /* "pyjls/binding.pyx":482
  *             signal_id = signals[i].signal_id
  *             signal_def = SignalDef(
  *                 signal_id=signal_id,             # <<<<<<<<<<<<<<
  *                 source_id=signals[i].source_id,
  *                 signal_type=signals[i].signal_type,
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(14); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(14); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_signal_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_signal_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_id, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_id, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":434
+    /* "pyjls/binding.pyx":483
  *             signal_def = SignalDef(
  *                 signal_id=signal_id,
  *                 source_id=signals[i].source_id,             # <<<<<<<<<<<<<<
  *                 signal_type=signals[i].signal_type,
  *                 data_type=signals[i].data_type,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t((__pyx_v_signals[__pyx_v_i]).source_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 434, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t((__pyx_v_signals[__pyx_v_i]).source_id); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 483, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_id, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_source_id, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":435
+    /* "pyjls/binding.pyx":484
  *                 signal_id=signal_id,
  *                 source_id=signals[i].source_id,
  *                 signal_type=signals[i].signal_type,             # <<<<<<<<<<<<<<
  *                 data_type=signals[i].data_type,
  *                 sample_rate=signals[i].sample_rate,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_signals[__pyx_v_i]).signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint8_t((__pyx_v_signals[__pyx_v_i]).signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_type, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_signal_type, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":436
+    /* "pyjls/binding.pyx":485
  *                 source_id=signals[i].source_id,
  *                 signal_type=signals[i].signal_type,
  *                 data_type=signals[i].data_type,             # <<<<<<<<<<<<<<
  *                 sample_rate=signals[i].sample_rate,
  *                 samples_per_data=signals[i].samples_per_data,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 485, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data_type, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_data_type, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":437
+    /* "pyjls/binding.pyx":486
  *                 signal_type=signals[i].signal_type,
  *                 data_type=signals[i].data_type,
  *                 sample_rate=signals[i].sample_rate,             # <<<<<<<<<<<<<<
  *                 samples_per_data=signals[i].samples_per_data,
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).sample_rate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).sample_rate); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_rate, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_rate, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":438
+    /* "pyjls/binding.pyx":487
  *                 data_type=signals[i].data_type,
  *                 sample_rate=signals[i].sample_rate,
  *                 samples_per_data=signals[i].samples_per_data,             # <<<<<<<<<<<<<<
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,
  *                 entries_per_summary=signals[i].entries_per_summary,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).samples_per_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).samples_per_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_samples_per_data, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_samples_per_data, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":439
+    /* "pyjls/binding.pyx":488
  *                 sample_rate=signals[i].sample_rate,
  *                 samples_per_data=signals[i].samples_per_data,
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,             # <<<<<<<<<<<<<<
  *                 entries_per_summary=signals[i].entries_per_summary,
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).sample_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).sample_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 488, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":440
+    /* "pyjls/binding.pyx":489
  *                 samples_per_data=signals[i].samples_per_data,
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,
  *                 entries_per_summary=signals[i].entries_per_summary,             # <<<<<<<<<<<<<<
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).entries_per_summary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).entries_per_summary); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_entries_per_summary, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_entries_per_summary, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":441
+    /* "pyjls/binding.pyx":490
  *                 sample_decimate_factor=signals[i].sample_decimate_factor,
  *                 entries_per_summary=signals[i].entries_per_summary,
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,             # <<<<<<<<<<<<<<
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).summary_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 441, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).summary_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 490, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_summary_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_summary_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":442
+    /* "pyjls/binding.pyx":491
  *                 entries_per_summary=signals[i].entries_per_summary,
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,             # <<<<<<<<<<<<<<
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,
  *                 sample_id_offset=signals[i].sample_id_offset,
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).annotation_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 442, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).annotation_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotation_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_annotation_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":443
+    /* "pyjls/binding.pyx":492
  *                 summary_decimate_factor=signals[i].summary_decimate_factor,
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,             # <<<<<<<<<<<<<<
  *                 sample_id_offset=signals[i].sample_id_offset,
  *                 name=signals[i].name.decode('utf-8'),
  */
-    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).utc_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 443, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint32_t((__pyx_v_signals[__pyx_v_i]).utc_decimate_factor); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_utc_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_utc_decimate_factor, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":444
+    /* "pyjls/binding.pyx":493
  *                 annotation_decimate_factor=signals[i].annotation_decimate_factor,
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,
  *                 sample_id_offset=signals[i].sample_id_offset,             # <<<<<<<<<<<<<<
  *                 name=signals[i].name.decode('utf-8'),
  *                 units=signals[i].units.decode('utf-8'))
  */
-    __pyx_t_4 = __Pyx_PyInt_From_int64_t((__pyx_v_signals[__pyx_v_i]).sample_id_offset); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 444, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int64_t((__pyx_v_signals[__pyx_v_i]).sample_id_offset); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 493, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_id_offset, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_sample_id_offset, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":445
+    /* "pyjls/binding.pyx":494
  *                 utc_decimate_factor=signals[i].utc_decimate_factor,
  *                 sample_id_offset=signals[i].sample_id_offset,
  *                 name=signals[i].name.decode('utf-8'),             # <<<<<<<<<<<<<<
  *                 units=signals[i].units.decode('utf-8'))
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:
  */
     __pyx_t_17 = (__pyx_v_signals[__pyx_v_i]).name;
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_17, 0, strlen(__pyx_t_17), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_17, 0, strlen(__pyx_t_17), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":446
+    /* "pyjls/binding.pyx":495
  *                 sample_id_offset=signals[i].sample_id_offset,
  *                 name=signals[i].name.decode('utf-8'),
  *                 units=signals[i].units.decode('utf-8'))             # <<<<<<<<<<<<<<
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  */
     __pyx_t_18 = (__pyx_v_signals[__pyx_v_i]).units;
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_18, 0, strlen(__pyx_t_18), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 446, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_t_18, 0, strlen(__pyx_t_18), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 495, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_units, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_units, __pyx_t_4) < 0) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":432
+    /* "pyjls/binding.pyx":481
  *         for i in range(count):
  *             signal_id = signals[i].signal_id
  *             signal_def = SignalDef(             # <<<<<<<<<<<<<<
  *                 signal_id=signal_id,
  *                 source_id=signals[i].source_id,
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 481, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF_SET(__pyx_v_signal_def, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pyjls/binding.pyx":447
+    /* "pyjls/binding.pyx":496
  *                 name=signals[i].name.decode('utf-8'),
  *                 units=signals[i].units.decode('utf-8'))
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:             # <<<<<<<<<<<<<<
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  *                 _handle_rc('rd_fsr_length', rc)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_signal_def, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_signal_def, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_5 = PyObject_RichCompare(__pyx_t_4, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_19 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_19 < 0)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_19 < 0)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (__pyx_t_19) {
 
-      /* "pyjls/binding.pyx":448
+      /* "pyjls/binding.pyx":497
  *                 units=signals[i].units.decode('utf-8'))
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)             # <<<<<<<<<<<<<<
  *                 _handle_rc('rd_fsr_length', rc)
  *                 signal_def.length = samples
  */
       __pyx_v_rc = jls_rd_fsr_length(__pyx_v_self->_rd, __pyx_v_signal_id, (&__pyx_v_samples));
 
-      /* "pyjls/binding.pyx":449
+      /* "pyjls/binding.pyx":498
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  *                 _handle_rc('rd_fsr_length', rc)             # <<<<<<<<<<<<<<
  *                 signal_def.length = samples
  *             self._signals[signal_id] = signal_def
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 498, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_1 = NULL;
       __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_1)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -10382,80 +11044,80 @@
           __Pyx_DECREF_SET(__pyx_t_3, function);
           __pyx_t_6 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_n_u_rd_fsr_length, __pyx_t_4};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
         PyObject *__pyx_temp[3] = {__pyx_t_1, __pyx_n_u_rd_fsr_length, __pyx_t_4};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else
       #endif
       {
-        __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 449, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         if (__pyx_t_1) {
           __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_1); __pyx_t_1 = NULL;
         }
         __Pyx_INCREF(__pyx_n_u_rd_fsr_length);
         __Pyx_GIVEREF(__pyx_n_u_rd_fsr_length);
         PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_n_u_rd_fsr_length);
         __Pyx_GIVEREF(__pyx_t_4);
         PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
         __pyx_t_4 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 449, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 498, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "pyjls/binding.pyx":450
+      /* "pyjls/binding.pyx":499
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  *                 _handle_rc('rd_fsr_length', rc)
  *                 signal_def.length = samples             # <<<<<<<<<<<<<<
  *             self._signals[signal_id] = signal_def
  * 
  */
-      __pyx_t_5 = __Pyx_PyInt_From_int64_t(__pyx_v_samples); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 450, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int64_t(__pyx_v_samples); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 499, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_PyObject_SetAttrStr(__pyx_v_signal_def, __pyx_n_s_length, __pyx_t_5) < 0) __PYX_ERR(0, 450, __pyx_L1_error)
+      if (__Pyx_PyObject_SetAttrStr(__pyx_v_signal_def, __pyx_n_s_length, __pyx_t_5) < 0) __PYX_ERR(0, 499, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "pyjls/binding.pyx":447
+      /* "pyjls/binding.pyx":496
  *                 name=signals[i].name.decode('utf-8'),
  *                 units=signals[i].units.decode('utf-8'))
  *             if signal_def.signal_type == c_jls.JLS_SIGNAL_TYPE_FSR:             # <<<<<<<<<<<<<<
  *                 rc = c_jls.jls_rd_fsr_length(self._rd, signal_id, &samples)
  *                 _handle_rc('rd_fsr_length', rc)
  */
     }
 
-    /* "pyjls/binding.pyx":451
+    /* "pyjls/binding.pyx":500
  *                 _handle_rc('rd_fsr_length', rc)
  *                 signal_def.length = samples
  *             self._signals[signal_id] = signal_def             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->_signals, __pyx_v_signal_id, __pyx_v_signal_def, uint16_t, 0, __Pyx_PyInt_From_uint16_t, 0, 0, 1) < 0)) __PYX_ERR(0, 451, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_self->_signals, __pyx_v_signal_id, __pyx_v_signal_def, uint16_t, 0, __Pyx_PyInt_From_uint16_t, 0, 0, 1) < 0)) __PYX_ERR(0, 500, __pyx_L1_error)
   }
 
-  /* "pyjls/binding.pyx":405
+  /* "pyjls/binding.pyx":454
  *     cdef object _signals
  * 
  *     def __init__(self, path: str):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef c_jls.jls_source_def_s * sources
  */
 
@@ -10473,15 +11135,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_source_def);
   __Pyx_XDECREF(__pyx_v_signal_def);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":453
+/* "pyjls/binding.pyx":502
  *             self._signals[signal_id] = signal_def
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -10499,42 +11161,42 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_2__enter__(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "pyjls/binding.pyx":454
+  /* "pyjls/binding.pyx":503
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, type, value, traceback):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":453
+  /* "pyjls/binding.pyx":502
  *             self._signals[signal_id] = signal_def
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":456
+/* "pyjls/binding.pyx":505
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -10571,40 +11233,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 456, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 505, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_traceback)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 456, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 505, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 456, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 505, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_type = values[0];
     __pyx_v_value = values[1];
     __pyx_v_traceback = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 456, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 505, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_4__exit__(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_type, __pyx_v_value, __pyx_v_traceback);
 
@@ -10620,41 +11282,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "pyjls/binding.pyx":457
+  /* "pyjls/binding.pyx":506
  * 
  *     def __exit__(self, type, value, traceback):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":456
+  /* "pyjls/binding.pyx":505
  *         return self
  * 
  *     def __exit__(self, type, value, traceback):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -10669,15 +11331,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":459
+/* "pyjls/binding.pyx":508
  *         self.close()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         c_jls.jls_rd_close(self._rd)
  * 
  */
 
@@ -10695,39 +11357,39 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_6close(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "pyjls/binding.pyx":460
+  /* "pyjls/binding.pyx":509
  * 
  *     def close(self):
  *         c_jls.jls_rd_close(self._rd)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   jls_rd_close(__pyx_v_self->_rd);
 
-  /* "pyjls/binding.pyx":459
+  /* "pyjls/binding.pyx":508
  *         self.close()
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         c_jls.jls_rd_close(self._rd)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":463
+/* "pyjls/binding.pyx":512
  * 
  *     @property
  *     def sources(self) -> Mapping[int, SourceDef]:             # <<<<<<<<<<<<<<
  *         return self._sources
  * 
  */
 
@@ -10745,42 +11407,42 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_7sources___get__(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyjls/binding.pyx":464
+  /* "pyjls/binding.pyx":513
  *     @property
  *     def sources(self) -> Mapping[int, SourceDef]:
  *         return self._sources             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_sources);
   __pyx_r = __pyx_v_self->_sources;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":463
+  /* "pyjls/binding.pyx":512
  * 
  *     @property
  *     def sources(self) -> Mapping[int, SourceDef]:             # <<<<<<<<<<<<<<
  *         return self._sources
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":467
+/* "pyjls/binding.pyx":516
  * 
  *     @property
  *     def signals(self) -> Mapping[int, SignalDef]:             # <<<<<<<<<<<<<<
  *         return self._signals
  * 
  */
 
@@ -10798,42 +11460,42 @@
 }
 
 static PyObject *__pyx_pf_5pyjls_7binding_6Reader_7signals___get__(struct __pyx_obj_5pyjls_7binding_Reader *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "pyjls/binding.pyx":468
+  /* "pyjls/binding.pyx":517
  *     @property
  *     def signals(self) -> Mapping[int, SignalDef]:
  *         return self._signals             # <<<<<<<<<<<<<<
  * 
  *     def fsr(self, signal_id, start_sample_id, length):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_signals);
   __pyx_r = __pyx_v_self->_signals;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":467
+  /* "pyjls/binding.pyx":516
  * 
  *     @property
  *     def signals(self) -> Mapping[int, SignalDef]:             # <<<<<<<<<<<<<<
  *         return self._signals
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":470
+/* "pyjls/binding.pyx":519
  *         return self._signals
  * 
  *     def fsr(self, signal_id, start_sample_id, length):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef np.uint8_t [::1] u8
  */
 
@@ -10870,40 +11532,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 1); __PYX_ERR(0, 470, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 1); __PYX_ERR(0, 519, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_length)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 2); __PYX_ERR(0, 470, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, 2); __PYX_ERR(0, 519, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr") < 0)) __PYX_ERR(0, 470, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr") < 0)) __PYX_ERR(0, 519, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_start_sample_id = values[1];
     __pyx_v_length = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 470, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fsr", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 519, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.fsr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_8fsr(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_start_sample_id, __pyx_v_length);
 
@@ -10939,271 +11601,271 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fsr", 0);
 
-  /* "pyjls/binding.pyx":476
+  /* "pyjls/binding.pyx":525
  *         cdef uint32_t entry_size_bits
  *         cdef uint32_t u8_length
  *         cdef uint16_t signal_id_u16 = signal_id             # <<<<<<<<<<<<<<
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t length_i64 = length
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 525, __pyx_L1_error)
   __pyx_v_signal_id_u16 = __pyx_t_1;
 
-  /* "pyjls/binding.pyx":477
+  /* "pyjls/binding.pyx":526
  *         cdef uint32_t u8_length
  *         cdef uint16_t signal_id_u16 = signal_id
  *         cdef int64_t start_sample_id_i64 = start_sample_id             # <<<<<<<<<<<<<<
  *         cdef int64_t length_i64 = length
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_start_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 477, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_start_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 526, __pyx_L1_error)
   __pyx_v_start_sample_id_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":478
+  /* "pyjls/binding.pyx":527
  *         cdef uint16_t signal_id_u16 = signal_id
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t length_i64 = length             # <<<<<<<<<<<<<<
  * 
  *         data_type = self._signals[signal_id].data_type
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_length); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_length); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 527, __pyx_L1_error)
   __pyx_v_length_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":480
+  /* "pyjls/binding.pyx":529
  *         cdef int64_t length_i64 = length
  * 
  *         data_type = self._signals[signal_id].data_type             # <<<<<<<<<<<<<<
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  */
-  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->_signals, __pyx_v_signal_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->_signals, __pyx_v_signal_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_data_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 529, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 529, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_data_type = __pyx_t_5;
 
-  /* "pyjls/binding.pyx":481
+  /* "pyjls/binding.pyx":530
  * 
  *         data_type = self._signals[signal_id].data_type
  *         entry_size_bits = (data_type >> 8) & 0xff             # <<<<<<<<<<<<<<
  *         np_type = _data_type_map[data_type & 0xffff]
  *         u8_length = length
  */
   __pyx_v_entry_size_bits = ((__pyx_v_data_type >> 8) & 0xff);
 
-  /* "pyjls/binding.pyx":482
+  /* "pyjls/binding.pyx":531
  *         data_type = self._signals[signal_id].data_type
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]             # <<<<<<<<<<<<<<
  *         u8_length = length
  *         if entry_size_bits == 4:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_data_type_map); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_data_type_map); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_6 = (__pyx_v_data_type & 0xffff);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_4, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_4, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_np_type = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":483
+  /* "pyjls/binding.pyx":532
  *         entry_size_bits = (data_type >> 8) & 0xff
  *         np_type = _data_type_map[data_type & 0xffff]
  *         u8_length = length             # <<<<<<<<<<<<<<
  *         if entry_size_bits == 4:
  *             u8_length = (length + 1) // 2
  */
-  __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_v_length); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_v_length); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 532, __pyx_L1_error)
   __pyx_v_u8_length = __pyx_t_5;
 
-  /* "pyjls/binding.pyx":484
+  /* "pyjls/binding.pyx":533
  *         np_type = _data_type_map[data_type & 0xffff]
  *         u8_length = length
  *         if entry_size_bits == 4:             # <<<<<<<<<<<<<<
  *             u8_length = (length + 1) // 2
  *         elif entry_size_bits == 1:
  */
   switch (__pyx_v_entry_size_bits) {
     case 4:
 
-    /* "pyjls/binding.pyx":485
+    /* "pyjls/binding.pyx":534
  *         u8_length = length
  *         if entry_size_bits == 4:
  *             u8_length = (length + 1) // 2             # <<<<<<<<<<<<<<
  *         elif entry_size_bits == 1:
  *             u8_length = (length + 7) // 8
  */
-    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 485, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 534, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_3, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 485, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_3, __pyx_int_2, 2, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 534, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 485, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_4); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 534, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_u8_length = __pyx_t_5;
 
-    /* "pyjls/binding.pyx":484
+    /* "pyjls/binding.pyx":533
  *         np_type = _data_type_map[data_type & 0xffff]
  *         u8_length = length
  *         if entry_size_bits == 4:             # <<<<<<<<<<<<<<
  *             u8_length = (length + 1) // 2
  *         elif entry_size_bits == 1:
  */
     break;
     case 1:
 
-    /* "pyjls/binding.pyx":487
+    /* "pyjls/binding.pyx":536
  *             u8_length = (length + 1) // 2
  *         elif entry_size_bits == 1:
  *             u8_length = (length + 7) // 8             # <<<<<<<<<<<<<<
  *         else:
  *             u8_length *= entry_size_bits // 8
  */
-    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_7, 7, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_v_length, __pyx_int_7, 7, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 536, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_4, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_FloorDivideObjC(__pyx_t_4, __pyx_int_8, 8, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 536, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 487, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_uint32_t(__pyx_t_3); if (unlikely((__pyx_t_5 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 536, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_u8_length = __pyx_t_5;
 
-    /* "pyjls/binding.pyx":486
+    /* "pyjls/binding.pyx":535
  *         if entry_size_bits == 4:
  *             u8_length = (length + 1) // 2
  *         elif entry_size_bits == 1:             # <<<<<<<<<<<<<<
  *             u8_length = (length + 7) // 8
  *         else:
  */
     break;
     default:
 
-    /* "pyjls/binding.pyx":489
+    /* "pyjls/binding.pyx":538
  *             u8_length = (length + 7) // 8
  *         else:
  *             u8_length *= entry_size_bits // 8             # <<<<<<<<<<<<<<
  * 
  *         data_u8 = np.empty(u8_length, dtype=np.uint8)
  */
     __pyx_v_u8_length = (__pyx_v_u8_length * __Pyx_div_long(__pyx_v_entry_size_bits, 8));
     break;
   }
 
-  /* "pyjls/binding.pyx":491
+  /* "pyjls/binding.pyx":540
  *             u8_length *= entry_size_bits // 8
  * 
  *         data_u8 = np.empty(u8_length, dtype=np.uint8)             # <<<<<<<<<<<<<<
  *         data = data_u8.view(dtype=np_type)
  *         u8 = data_u8
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_u8_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_u8_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_uint8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 491, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_9) < 0) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 491, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, __pyx_t_3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 540, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_data_u8 = __pyx_t_9;
   __pyx_t_9 = 0;
 
-  /* "pyjls/binding.pyx":492
+  /* "pyjls/binding.pyx":541
  * 
  *         data_u8 = np.empty(u8_length, dtype=np.uint8)
  *         data = data_u8.view(dtype=np_type)             # <<<<<<<<<<<<<<
  *         u8 = data_u8
  *         with nogil:
  */
-  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_u8, __pyx_n_s_view); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 492, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_data_u8, __pyx_n_s_view); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 541, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 541, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_v_np_type) < 0) __PYX_ERR(0, 492, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 492, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_v_np_type) < 0) __PYX_ERR(0, 541, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 541, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_data = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":493
+  /* "pyjls/binding.pyx":542
  *         data_u8 = np.empty(u8_length, dtype=np.uint8)
  *         data = data_u8.view(dtype=np_type)
  *         u8 = data_u8             # <<<<<<<<<<<<<<
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  */
-  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_data_u8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(__pyx_v_data_u8, PyBUF_WRITABLE); if (unlikely(!__pyx_t_10.memview)) __PYX_ERR(0, 542, __pyx_L1_error)
   __pyx_v_u8 = __pyx_t_10;
   __pyx_t_10.memview = NULL;
   __pyx_t_10.data = NULL;
 
-  /* "pyjls/binding.pyx":494
+  /* "pyjls/binding.pyx":543
  *         data = data_u8.view(dtype=np_type)
  *         u8 = data_u8
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  *         _handle_rc('rd_fsr', rc)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjls/binding.pyx":495
+        /* "pyjls/binding.pyx":544
  *         u8 = data_u8
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_fsr', rc)
  *         return data
  */
         __pyx_t_11 = 0;
         __pyx_t_12 = -1;
         if (__pyx_t_11 < 0) {
           __pyx_t_11 += __pyx_v_u8.shape[0];
           if (unlikely(__pyx_t_11 < 0)) __pyx_t_12 = 0;
         } else if (unlikely(__pyx_t_11 >= __pyx_v_u8.shape[0])) __pyx_t_12 = 0;
         if (unlikely(__pyx_t_12 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_12);
-          __PYX_ERR(0, 495, __pyx_L4_error)
+          __PYX_ERR(0, 544, __pyx_L4_error)
         }
         __pyx_v_rc = jls_rd_fsr(__pyx_v_self->_rd, __pyx_v_signal_id_u16, __pyx_v_start_sample_id_i64, (&(*((__pyx_t_5numpy_uint8_t *) ( /* dim=0 */ ((char *) (((__pyx_t_5numpy_uint8_t *) __pyx_v_u8.data) + __pyx_t_11)) )))), __pyx_v_length_i64);
       }
 
-      /* "pyjls/binding.pyx":494
+      /* "pyjls/binding.pyx":543
  *         data = data_u8.view(dtype=np_type)
  *         u8 = data_u8
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  *         _handle_rc('rd_fsr', rc)
  */
       /*finally:*/ {
@@ -11221,24 +11883,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyjls/binding.pyx":496
+  /* "pyjls/binding.pyx":545
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  *         _handle_rc('rd_fsr', rc)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_9 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 496, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 545, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __pyx_t_4 = NULL;
   __pyx_t_12 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11247,61 +11909,61 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_12 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_fsr, __pyx_t_9};
-    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 496, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 545, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_fsr, __pyx_t_9};
-    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 496, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 545, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 496, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 545, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_fsr);
     __Pyx_GIVEREF(__pyx_n_u_rd_fsr);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_12, __pyx_n_u_rd_fsr);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_12, __pyx_t_9);
     __pyx_t_9 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 496, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 545, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":497
+  /* "pyjls/binding.pyx":546
  *             rc = c_jls.jls_rd_fsr(self._rd, signal_id_u16, start_sample_id_i64, &u8[0], length_i64)
  *         _handle_rc('rd_fsr', rc)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def fsr_statistics(self, signal_id, start_sample_id, increment, length):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":470
+  /* "pyjls/binding.pyx":519
  *         return self._signals
  * 
  *     def fsr(self, signal_id, start_sample_id, length):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         cdef np.uint8_t [::1] u8
  */
 
@@ -11321,15 +11983,15 @@
   __Pyx_XDECREF(__pyx_v_data_u8);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":499
+/* "pyjls/binding.pyx":548
  *         return data
  * 
  *     def fsr_statistics(self, signal_id, start_sample_id, increment, length):             # <<<<<<<<<<<<<<
  *         """Read FSR statistics.
  * 
  */
 
@@ -11370,31 +12032,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 1); __PYX_ERR(0, 499, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 1); __PYX_ERR(0, 548, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_increment)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 2); __PYX_ERR(0, 499, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 2); __PYX_ERR(0, 548, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_length)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 3); __PYX_ERR(0, 499, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, 3); __PYX_ERR(0, 548, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr_statistics") < 0)) __PYX_ERR(0, 499, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "fsr_statistics") < 0)) __PYX_ERR(0, 548, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -11403,15 +12065,15 @@
     __pyx_v_signal_id = values[0];
     __pyx_v_start_sample_id = values[1];
     __pyx_v_increment = values[2];
     __pyx_v_length = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 499, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fsr_statistics", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 548, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.fsr_statistics", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_10fsr_statistics(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_start_sample_id, __pyx_v_increment, __pyx_v_length);
 
@@ -11442,126 +12104,126 @@
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fsr_statistics", 0);
 
-  /* "pyjls/binding.pyx":511
+  /* "pyjls/binding.pyx":560
  *         cdef int32_t rc
  *         cdef np.float64_t [:, :] c_data
  *         cdef uint16_t signal_id_u16 = signal_id             # <<<<<<<<<<<<<<
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t increment_i64 = increment
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 560, __pyx_L1_error)
   __pyx_v_signal_id_u16 = __pyx_t_1;
 
-  /* "pyjls/binding.pyx":512
+  /* "pyjls/binding.pyx":561
  *         cdef np.float64_t [:, :] c_data
  *         cdef uint16_t signal_id_u16 = signal_id
  *         cdef int64_t start_sample_id_i64 = start_sample_id             # <<<<<<<<<<<<<<
  *         cdef int64_t increment_i64 = increment
  *         cdef int64_t length_i64 = length
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_start_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_start_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L1_error)
   __pyx_v_start_sample_id_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":513
+  /* "pyjls/binding.pyx":562
  *         cdef uint16_t signal_id_u16 = signal_id
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t increment_i64 = increment             # <<<<<<<<<<<<<<
  *         cdef int64_t length_i64 = length
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_increment); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_increment); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 562, __pyx_L1_error)
   __pyx_v_increment_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":514
+  /* "pyjls/binding.pyx":563
  *         cdef int64_t start_sample_id_i64 = start_sample_id
  *         cdef int64_t increment_i64 = increment
  *         cdef int64_t length_i64 = length             # <<<<<<<<<<<<<<
  * 
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_length); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_length); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 563, __pyx_L1_error)
   __pyx_v_length_i64 = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":516
+  /* "pyjls/binding.pyx":565
  *         cdef int64_t length_i64 = length
  * 
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)             # <<<<<<<<<<<<<<
  *         c_data = data
  *         with nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_COUNT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__jls_summary_fsr_e(JLS_SUMMARY_FSR_COUNT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_length);
   __Pyx_GIVEREF(__pyx_v_length);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_length);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 516, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 565, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_data = __pyx_t_7;
   __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":517
+  /* "pyjls/binding.pyx":566
  * 
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)
  *         c_data = data             # <<<<<<<<<<<<<<
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  */
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5numpy_float64_t(__pyx_v_data, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 517, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5numpy_float64_t(__pyx_v_data, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 566, __pyx_L1_error)
   __pyx_v_c_data = __pyx_t_8;
   __pyx_t_8.memview = NULL;
   __pyx_t_8.data = NULL;
 
-  /* "pyjls/binding.pyx":518
+  /* "pyjls/binding.pyx":567
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)
  *         c_data = data
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  *                                              increment_i64, &c_data[0, 0], length_i64)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pyjls/binding.pyx":520
+        /* "pyjls/binding.pyx":569
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  *                                              increment_i64, &c_data[0, 0], length_i64)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_fsr_statistics', rc)
  *         return data
  */
         __pyx_t_9 = 0;
@@ -11573,28 +12235,28 @@
         } else if (unlikely(__pyx_t_9 >= __pyx_v_c_data.shape[0])) __pyx_t_11 = 0;
         if (__pyx_t_10 < 0) {
           __pyx_t_10 += __pyx_v_c_data.shape[1];
           if (unlikely(__pyx_t_10 < 0)) __pyx_t_11 = 1;
         } else if (unlikely(__pyx_t_10 >= __pyx_v_c_data.shape[1])) __pyx_t_11 = 1;
         if (unlikely(__pyx_t_11 != -1)) {
           __Pyx_RaiseBufferIndexErrorNogil(__pyx_t_11);
-          __PYX_ERR(0, 520, __pyx_L4_error)
+          __PYX_ERR(0, 569, __pyx_L4_error)
         }
 
-        /* "pyjls/binding.pyx":519
+        /* "pyjls/binding.pyx":568
  *         c_data = data
  *         with nogil:
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,             # <<<<<<<<<<<<<<
  *                                              increment_i64, &c_data[0, 0], length_i64)
  *         _handle_rc('rd_fsr_statistics', rc)
  */
         __pyx_v_rc = jls_rd_fsr_statistics(__pyx_v_self->_rd, __pyx_v_signal_id_u16, __pyx_v_start_sample_id_i64, __pyx_v_increment_i64, (&(*((__pyx_t_5numpy_float64_t *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_c_data.data + __pyx_t_9 * __pyx_v_c_data.strides[0]) ) + __pyx_t_10 * __pyx_v_c_data.strides[1]) )))), __pyx_v_length_i64);
       }
 
-      /* "pyjls/binding.pyx":518
+      /* "pyjls/binding.pyx":567
  *         data = np.empty((length, c_jls.JLS_SUMMARY_FSR_COUNT), dtype=np.float64)
  *         c_data = data
  *         with nogil:             # <<<<<<<<<<<<<<
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  *                                              increment_i64, &c_data[0, 0], length_i64)
  */
       /*finally:*/ {
@@ -11612,24 +12274,24 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pyjls/binding.pyx":521
+  /* "pyjls/binding.pyx":570
  *             rc = c_jls.jls_rd_fsr_statistics(self._rd, signal_id_u16, start_sample_id_i64,
  *                                              increment_i64, &c_data[0, 0], length_i64)
  *         _handle_rc('rd_fsr_statistics', rc)             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 521, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_11 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -11638,61 +12300,61 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_11 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_fsr_statistics, __pyx_t_3};
-    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 570, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_fsr_statistics, __pyx_t_3};
-    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 570, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 521, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 570, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_fsr_statistics);
     __Pyx_GIVEREF(__pyx_n_u_rd_fsr_statistics);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_11, __pyx_n_u_rd_fsr_statistics);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_11, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 570, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyjls/binding.pyx":522
+  /* "pyjls/binding.pyx":571
  *                                              increment_i64, &c_data[0, 0], length_i64)
  *         _handle_rc('rd_fsr_statistics', rc)
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def annotations(self, signal_id, timestamp, cbk_fn):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":499
+  /* "pyjls/binding.pyx":548
  *         return data
  * 
  *     def fsr_statistics(self, signal_id, start_sample_id, increment, length):             # <<<<<<<<<<<<<<
  *         """Read FSR statistics.
  * 
  */
 
@@ -11710,15 +12372,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_c_data, 1);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":524
+/* "pyjls/binding.pyx":573
  *         return data
  * 
  *     def annotations(self, signal_id, timestamp, cbk_fn):             # <<<<<<<<<<<<<<
  *         """Read annotations from a signal.
  * 
  */
 
@@ -11756,40 +12418,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timestamp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, 1); __PYX_ERR(0, 524, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, 1); __PYX_ERR(0, 573, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cbk_fn)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, 2); __PYX_ERR(0, 524, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, 2); __PYX_ERR(0, 573, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "annotations") < 0)) __PYX_ERR(0, 524, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "annotations") < 0)) __PYX_ERR(0, 573, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_timestamp = values[1];
     __pyx_v_cbk_fn = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 524, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("annotations", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 573, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.annotations", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_12annotations(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_timestamp, __pyx_v_cbk_fn);
 
@@ -11813,76 +12475,76 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("annotations", 0);
 
-  /* "pyjls/binding.pyx":534
+  /* "pyjls/binding.pyx":583
  *         """
  *         cdef int32_t rc
  *         is_fsr = self._signals[signal_id].signal_type == c_jls.JLS_SIGNAL_TYPE_FSR             # <<<<<<<<<<<<<<
  *         user_data = AnnotationCallback(is_fsr, cbk_fn)
  *         rc = c_jls.jls_rd_annotations(self._rd, signal_id, timestamp, _annotation_cbk_fn, <void *> user_data)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->_signals, __pyx_v_signal_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->_signals, __pyx_v_signal_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_signal_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__jls_signal_type_e(JLS_SIGNAL_TYPE_FSR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 583, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_is_fsr = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":535
+  /* "pyjls/binding.pyx":584
  *         cdef int32_t rc
  *         is_fsr = self._signals[signal_id].signal_type == c_jls.JLS_SIGNAL_TYPE_FSR
  *         user_data = AnnotationCallback(is_fsr, cbk_fn)             # <<<<<<<<<<<<<<
  *         rc = c_jls.jls_rd_annotations(self._rd, signal_id, timestamp, _annotation_cbk_fn, <void *> user_data)
  *         _handle_rc('rd_annotations', rc)
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_is_fsr);
   __Pyx_GIVEREF(__pyx_v_is_fsr);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_is_fsr);
   __Pyx_INCREF(__pyx_v_cbk_fn);
   __Pyx_GIVEREF(__pyx_v_cbk_fn);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_cbk_fn);
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5pyjls_7binding_AnnotationCallback), __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 535, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_5pyjls_7binding_AnnotationCallback), __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_user_data = ((struct __pyx_obj_5pyjls_7binding_AnnotationCallback *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":536
+  /* "pyjls/binding.pyx":585
  *         is_fsr = self._signals[signal_id].signal_type == c_jls.JLS_SIGNAL_TYPE_FSR
  *         user_data = AnnotationCallback(is_fsr, cbk_fn)
  *         rc = c_jls.jls_rd_annotations(self._rd, signal_id, timestamp, _annotation_cbk_fn, <void *> user_data)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_annotations', rc)
  * 
  */
-  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 536, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyInt_As_int64_t(__pyx_v_timestamp); if (unlikely((__pyx_t_5 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 536, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_4 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 585, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int64_t(__pyx_v_timestamp); if (unlikely((__pyx_t_5 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 585, __pyx_L1_error)
   __pyx_v_rc = jls_rd_annotations(__pyx_v_self->_rd, __pyx_t_4, __pyx_t_5, __pyx_f_5pyjls_7binding__annotation_cbk_fn, ((void *)__pyx_v_user_data));
 
-  /* "pyjls/binding.pyx":537
+  /* "pyjls/binding.pyx":586
  *         user_data = AnnotationCallback(is_fsr, cbk_fn)
  *         rc = c_jls.jls_rd_annotations(self._rd, signal_id, timestamp, _annotation_cbk_fn, <void *> user_data)
  *         _handle_rc('rd_annotations', rc)             # <<<<<<<<<<<<<<
  * 
  *     def user_data(self, cbk_fn):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 537, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 537, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -11891,49 +12553,49 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_rd_annotations, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 537, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_rd_annotations, __pyx_t_2};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 537, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 537, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 586, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_annotations);
     __Pyx_GIVEREF(__pyx_n_u_rd_annotations);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_rd_annotations);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 537, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":524
+  /* "pyjls/binding.pyx":573
  *         return data
  * 
  *     def annotations(self, signal_id, timestamp, cbk_fn):             # <<<<<<<<<<<<<<
  *         """Read annotations from a signal.
  * 
  */
 
@@ -11952,15 +12614,15 @@
   __Pyx_XDECREF(__pyx_v_is_fsr);
   __Pyx_XDECREF((PyObject *)__pyx_v_user_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":539
+/* "pyjls/binding.pyx":588
  *         _handle_rc('rd_annotations', rc)
  * 
  *     def user_data(self, cbk_fn):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_user_data(self._rd, _user_data_cbk_fn, <void *> cbk_fn)
  */
 
@@ -11988,33 +12650,33 @@
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("user_data", 0);
 
-  /* "pyjls/binding.pyx":541
+  /* "pyjls/binding.pyx":590
  *     def user_data(self, cbk_fn):
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_user_data(self._rd, _user_data_cbk_fn, <void *> cbk_fn)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_user_data', rc)
  * 
  */
   __pyx_v_rc = jls_rd_user_data(__pyx_v_self->_rd, __pyx_f_5pyjls_7binding__user_data_cbk_fn, ((void *)__pyx_v_cbk_fn));
 
-  /* "pyjls/binding.pyx":542
+  /* "pyjls/binding.pyx":591
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_user_data(self._rd, _user_data_cbk_fn, <void *> cbk_fn)
  *         _handle_rc('rd_user_data', rc)             # <<<<<<<<<<<<<<
  * 
  *     def utc(self, signal_id, sample_id, cbk_fn):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -12023,49 +12685,49 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_user_data, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_n_u_rd_user_data, __pyx_t_3};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 542, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_user_data);
     __Pyx_GIVEREF(__pyx_n_u_rd_user_data);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_n_u_rd_user_data);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 542, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":539
+  /* "pyjls/binding.pyx":588
  *         _handle_rc('rd_annotations', rc)
  * 
  *     def user_data(self, cbk_fn):             # <<<<<<<<<<<<<<
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_user_data(self._rd, _user_data_cbk_fn, <void *> cbk_fn)
  */
 
@@ -12082,15 +12744,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":544
+/* "pyjls/binding.pyx":593
  *         _handle_rc('rd_user_data', rc)
  * 
  *     def utc(self, signal_id, sample_id, cbk_fn):             # <<<<<<<<<<<<<<
  *         """Read the sample_id / utc pairs from a FSR signal.
  * 
  */
 
@@ -12128,40 +12790,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 1); __PYX_ERR(0, 544, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 1); __PYX_ERR(0, 593, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cbk_fn)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 2); __PYX_ERR(0, 544, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, 2); __PYX_ERR(0, 593, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "utc") < 0)) __PYX_ERR(0, 544, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "utc") < 0)) __PYX_ERR(0, 593, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
     __pyx_v_cbk_fn = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 544, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("utc", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 593, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.utc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_16utc(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id, __pyx_v_cbk_fn);
 
@@ -12183,35 +12845,35 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("utc", 0);
 
-  /* "pyjls/binding.pyx":556
+  /* "pyjls/binding.pyx":605
  *         """
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_utc(self._rd, signal_id, sample_id, _utc_cbk_fn, <void *> cbk_fn)             # <<<<<<<<<<<<<<
  *         _handle_rc('rd_utc', rc)
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 556, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 556, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 605, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 605, __pyx_L1_error)
   __pyx_v_rc = jls_rd_utc(__pyx_v_self->_rd, __pyx_t_1, __pyx_t_2, __pyx_f_5pyjls_7binding__utc_cbk_fn, ((void *)__pyx_v_cbk_fn));
 
-  /* "pyjls/binding.pyx":557
+  /* "pyjls/binding.pyx":606
  *         cdef int32_t rc
  *         rc = c_jls.jls_rd_utc(self._rd, signal_id, sample_id, _utc_cbk_fn, <void *> cbk_fn)
  *         _handle_rc('rd_utc', rc)             # <<<<<<<<<<<<<<
  * 
  *     def sample_id_to_timestamp(self, signal_id, sample_id):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -12220,49 +12882,49 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_rd_utc, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_rd_utc, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 557, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_rd_utc);
     __Pyx_GIVEREF(__pyx_n_u_rd_utc);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_rd_utc);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 557, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":544
+  /* "pyjls/binding.pyx":593
  *         _handle_rc('rd_user_data', rc)
  * 
  *     def utc(self, signal_id, sample_id, cbk_fn):             # <<<<<<<<<<<<<<
  *         """Read the sample_id / utc pairs from a FSR signal.
  * 
  */
 
@@ -12279,15 +12941,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":559
+/* "pyjls/binding.pyx":608
  *         _handle_rc('rd_utc', rc)
  * 
  *     def sample_id_to_timestamp(self, signal_id, sample_id):             # <<<<<<<<<<<<<<
  *         """Convert sample_id to UTC timestamp for FSR signals.
  * 
  */
 
@@ -12322,32 +12984,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("sample_id_to_timestamp", 1, 2, 2, 1); __PYX_ERR(0, 559, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("sample_id_to_timestamp", 1, 2, 2, 1); __PYX_ERR(0, 608, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sample_id_to_timestamp") < 0)) __PYX_ERR(0, 559, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sample_id_to_timestamp") < 0)) __PYX_ERR(0, 608, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_sample_id = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("sample_id_to_timestamp", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 559, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("sample_id_to_timestamp", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 608, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.sample_id_to_timestamp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_18sample_id_to_timestamp(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_sample_id);
 
@@ -12370,35 +13032,35 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sample_id_to_timestamp", 0);
 
-  /* "pyjls/binding.pyx":568
+  /* "pyjls/binding.pyx":617
  *         """
  *         cdef int64_t utc_timestamp
  *         rc = c_jls.jls_rd_sample_id_to_timestamp(self._rd, signal_id, sample_id, &utc_timestamp)             # <<<<<<<<<<<<<<
  *         _handle_rc('sample_id_to_timestamp', rc)
  *         return utc_timestamp
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 568, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 617, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_sample_id); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 617, __pyx_L1_error)
   __pyx_v_rc = jls_rd_sample_id_to_timestamp(__pyx_v_self->_rd, __pyx_t_1, __pyx_t_2, (&__pyx_v_utc_timestamp));
 
-  /* "pyjls/binding.pyx":569
+  /* "pyjls/binding.pyx":618
  *         cdef int64_t utc_timestamp
  *         rc = c_jls.jls_rd_sample_id_to_timestamp(self._rd, signal_id, sample_id, &utc_timestamp)
  *         _handle_rc('sample_id_to_timestamp', rc)             # <<<<<<<<<<<<<<
  *         return utc_timestamp
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 618, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -12407,63 +13069,63 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_sample_id_to_timestamp, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 618, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_sample_id_to_timestamp, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 618, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 618, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_sample_id_to_timestamp);
     __Pyx_GIVEREF(__pyx_n_u_sample_id_to_timestamp);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_sample_id_to_timestamp);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 618, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":570
+  /* "pyjls/binding.pyx":619
  *         rc = c_jls.jls_rd_sample_id_to_timestamp(self._rd, signal_id, sample_id, &utc_timestamp)
  *         _handle_rc('sample_id_to_timestamp', rc)
  *         return utc_timestamp             # <<<<<<<<<<<<<<
  * 
  *     def timestamp_to_sample_id(self, signal_id, utc_timestamp):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_v_utc_timestamp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 570, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_v_utc_timestamp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":559
+  /* "pyjls/binding.pyx":608
  *         _handle_rc('rd_utc', rc)
  * 
  *     def sample_id_to_timestamp(self, signal_id, sample_id):             # <<<<<<<<<<<<<<
  *         """Convert sample_id to UTC timestamp for FSR signals.
  * 
  */
 
@@ -12478,15 +13140,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":572
+/* "pyjls/binding.pyx":621
  *         return utc_timestamp
  * 
  *     def timestamp_to_sample_id(self, signal_id, utc_timestamp):             # <<<<<<<<<<<<<<
  *         """Convert UTC timestamp to sample_id for FSR signals.
  * 
  */
 
@@ -12521,32 +13183,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_signal_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_utc_timestamp)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("timestamp_to_sample_id", 1, 2, 2, 1); __PYX_ERR(0, 572, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("timestamp_to_sample_id", 1, 2, 2, 1); __PYX_ERR(0, 621, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "timestamp_to_sample_id") < 0)) __PYX_ERR(0, 572, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "timestamp_to_sample_id") < 0)) __PYX_ERR(0, 621, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_signal_id = values[0];
     __pyx_v_utc_timestamp = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("timestamp_to_sample_id", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 572, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("timestamp_to_sample_id", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 621, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyjls.binding.Reader.timestamp_to_sample_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_5pyjls_7binding_6Reader_20timestamp_to_sample_id(((struct __pyx_obj_5pyjls_7binding_Reader *)__pyx_v_self), __pyx_v_signal_id, __pyx_v_utc_timestamp);
 
@@ -12569,35 +13231,35 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("timestamp_to_sample_id", 0);
 
-  /* "pyjls/binding.pyx":581
+  /* "pyjls/binding.pyx":630
  *         """
  *         cdef int64_t sample_id
  *         rc = c_jls.jls_rd_timestamp_to_sample_id(self._rd, signal_id, utc_timestamp, &sample_id)             # <<<<<<<<<<<<<<
  *         _handle_rc('timestamp_to_sample_id', rc)
  *         return sample_id
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 581, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_utc_timestamp); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint16_t(__pyx_v_signal_id); if (unlikely((__pyx_t_1 == ((uint16_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_utc_timestamp); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
   __pyx_v_rc = jls_rd_timestamp_to_sample_id(__pyx_v_self->_rd, __pyx_t_1, __pyx_t_2, (&__pyx_v_sample_id));
 
-  /* "pyjls/binding.pyx":582
+  /* "pyjls/binding.pyx":631
  *         cdef int64_t sample_id
  *         rc = c_jls.jls_rd_timestamp_to_sample_id(self._rd, signal_id, utc_timestamp, &sample_id)
  *         _handle_rc('timestamp_to_sample_id', rc)             # <<<<<<<<<<<<<<
  *         return sample_id
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_handle_rc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 582, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int32_t(__pyx_v_rc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -12606,63 +13268,63 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_timestamp_to_sample_id, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 631, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_n_u_timestamp_to_sample_id, __pyx_t_5};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 631, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 582, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 631, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_n_u_timestamp_to_sample_id);
     __Pyx_GIVEREF(__pyx_n_u_timestamp_to_sample_id);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_n_u_timestamp_to_sample_id);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 582, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 631, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyjls/binding.pyx":583
+  /* "pyjls/binding.pyx":632
  *         rc = c_jls.jls_rd_timestamp_to_sample_id(self._rd, signal_id, utc_timestamp, &sample_id)
  *         _handle_rc('timestamp_to_sample_id', rc)
  *         return sample_id             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_v_sample_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_v_sample_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 632, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":572
+  /* "pyjls/binding.pyx":621
  *         return utc_timestamp
  * 
  *     def timestamp_to_sample_id(self, signal_id, utc_timestamp):             # <<<<<<<<<<<<<<
  *         """Convert UTC timestamp to sample_id for FSR signals.
  * 
  */
 
@@ -12711,15 +13373,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -12767,15 +13429,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -12790,15 +13452,15 @@
   __Pyx_AddTraceback("pyjls.binding.Reader.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":586
+/* "pyjls/binding.pyx":635
  * 
  * 
  * cdef int32_t _annotation_cbk_fn(void * user_data, const c_jls.jls_annotation_s * annotation):             # <<<<<<<<<<<<<<
  *     obj: AnnotationCallback = <object> user_data
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  */
 
@@ -12827,121 +13489,121 @@
   PyObject *__pyx_t_15 = NULL;
   int32_t __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_annotation_cbk_fn", 0);
 
-  /* "pyjls/binding.pyx":587
+  /* "pyjls/binding.pyx":636
  * 
  * cdef int32_t _annotation_cbk_fn(void * user_data, const c_jls.jls_annotation_s * annotation):
  *     obj: AnnotationCallback = <object> user_data             # <<<<<<<<<<<<<<
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  *     y = annotation[0].y
  */
-  if (!(likely(((((PyObject *)__pyx_v_user_data)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_user_data), __pyx_ptype_5pyjls_7binding_AnnotationCallback))))) __PYX_ERR(0, 587, __pyx_L1_error)
+  if (!(likely(((((PyObject *)__pyx_v_user_data)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_user_data), __pyx_ptype_5pyjls_7binding_AnnotationCallback))))) __PYX_ERR(0, 636, __pyx_L1_error)
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_obj = ((struct __pyx_obj_5pyjls_7binding_AnnotationCallback *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":588
+  /* "pyjls/binding.pyx":637
  * cdef int32_t _annotation_cbk_fn(void * user_data, const c_jls.jls_annotation_s * annotation):
  *     obj: AnnotationCallback = <object> user_data
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)             # <<<<<<<<<<<<<<
  *     y = annotation[0].y
  *     timestamp = annotation[0].timestamp
  */
-  __pyx_t_1 = __pyx_f_5pyjls_7binding__storage_unpack((__pyx_v_annotation[0]).storage_type, (__pyx_v_annotation[0]).data, (__pyx_v_annotation[0]).data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5pyjls_7binding__storage_unpack((__pyx_v_annotation[0]).storage_type, (__pyx_v_annotation[0]).data, (__pyx_v_annotation[0]).data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 637, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_data = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":589
+  /* "pyjls/binding.pyx":638
  *     obj: AnnotationCallback = <object> user_data
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  *     y = annotation[0].y             # <<<<<<<<<<<<<<
  *     timestamp = annotation[0].timestamp
  *     if not obj.is_fsr:
  */
-  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_annotation[0]).y); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble((__pyx_v_annotation[0]).y); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 638, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_y = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":590
+  /* "pyjls/binding.pyx":639
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  *     y = annotation[0].y
  *     timestamp = annotation[0].timestamp             # <<<<<<<<<<<<<<
  *     if not obj.is_fsr:
  *         timestamp = annotation[0].timestamp
  */
   __pyx_t_2 = (__pyx_v_annotation[0]).timestamp;
   __pyx_v_timestamp = __pyx_t_2;
 
-  /* "pyjls/binding.pyx":591
+  /* "pyjls/binding.pyx":640
  *     y = annotation[0].y
  *     timestamp = annotation[0].timestamp
  *     if not obj.is_fsr:             # <<<<<<<<<<<<<<
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):
  */
   __pyx_t_3 = ((!(__pyx_v_obj->is_fsr != 0)) != 0);
   if (__pyx_t_3) {
 
-    /* "pyjls/binding.pyx":592
+    /* "pyjls/binding.pyx":641
  *     timestamp = annotation[0].timestamp
  *     if not obj.is_fsr:
  *         timestamp = annotation[0].timestamp             # <<<<<<<<<<<<<<
  *     if not isfinite(y):
  *         y = None
  */
     __pyx_t_2 = (__pyx_v_annotation[0]).timestamp;
     __pyx_v_timestamp = __pyx_t_2;
 
-    /* "pyjls/binding.pyx":591
+    /* "pyjls/binding.pyx":640
  *     y = annotation[0].y
  *     timestamp = annotation[0].timestamp
  *     if not obj.is_fsr:             # <<<<<<<<<<<<<<
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):
  */
   }
 
-  /* "pyjls/binding.pyx":593
+  /* "pyjls/binding.pyx":642
  *     if not obj.is_fsr:
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):             # <<<<<<<<<<<<<<
  *         y = None
  *     try:
  */
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_y); if (unlikely((__pyx_t_4 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_v_y); if (unlikely((__pyx_t_4 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(0, 642, __pyx_L1_error)
   __pyx_t_3 = ((!(isfinite(__pyx_t_4) != 0)) != 0);
   if (__pyx_t_3) {
 
-    /* "pyjls/binding.pyx":594
+    /* "pyjls/binding.pyx":643
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):
  *         y = None             # <<<<<<<<<<<<<<
  *     try:
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  */
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_y, Py_None);
 
-    /* "pyjls/binding.pyx":593
+    /* "pyjls/binding.pyx":642
  *     if not obj.is_fsr:
  *         timestamp = annotation[0].timestamp
  *     if not isfinite(y):             # <<<<<<<<<<<<<<
  *         y = None
  *     try:
  */
   }
 
-  /* "pyjls/binding.pyx":595
+  /* "pyjls/binding.pyx":644
  *     if not isfinite(y):
  *         y = None
  *     try:             # <<<<<<<<<<<<<<
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:
  */
   {
@@ -12949,26 +13611,26 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
     __Pyx_XGOTREF(__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_t_7);
     /*try:*/ {
 
-      /* "pyjls/binding.pyx":596
+      /* "pyjls/binding.pyx":645
  *         y = None
  *     try:
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)             # <<<<<<<<<<<<<<
  *     except Exception:
  *         logging.getLogger(__name__).exception('in annotation callback')
  */
-      __pyx_t_8 = __Pyx_PyInt_From_int64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 596, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyInt_From_int64_t(__pyx_v_timestamp); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 645, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyInt_From_uint8_t((__pyx_v_annotation[0]).annotation_type); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 596, __pyx_L5_error)
+      __pyx_t_9 = __Pyx_PyInt_From_uint8_t((__pyx_v_annotation[0]).annotation_type); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 645, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyInt_From_uint8_t((__pyx_v_annotation[0]).group_id); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 596, __pyx_L5_error)
+      __pyx_t_10 = __Pyx_PyInt_From_uint8_t((__pyx_v_annotation[0]).group_id); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 645, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_INCREF(__pyx_v_obj->cbk_fn);
       __pyx_t_11 = __pyx_v_obj->cbk_fn; __pyx_t_12 = NULL;
       __pyx_t_13 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_12)) {
@@ -12978,35 +13640,35 @@
           __Pyx_DECREF_SET(__pyx_t_11, function);
           __pyx_t_13 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_11)) {
         PyObject *__pyx_temp[6] = {__pyx_t_12, __pyx_t_8, __pyx_v_y, __pyx_t_9, __pyx_t_10, __pyx_v_data};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 5+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 596, __pyx_L5_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 5+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L5_error)
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_11)) {
         PyObject *__pyx_temp[6] = {__pyx_t_12, __pyx_t_8, __pyx_v_y, __pyx_t_9, __pyx_t_10, __pyx_v_data};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 5+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 596, __pyx_L5_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_13, 5+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L5_error)
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       } else
       #endif
       {
-        __pyx_t_14 = PyTuple_New(5+__pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 596, __pyx_L5_error)
+        __pyx_t_14 = PyTuple_New(5+__pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 645, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_14);
         if (__pyx_t_12) {
           __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_12); __pyx_t_12 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_8);
         PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_13, __pyx_t_8);
         __Pyx_INCREF(__pyx_v_y);
@@ -13018,23 +13680,23 @@
         PyTuple_SET_ITEM(__pyx_t_14, 3+__pyx_t_13, __pyx_t_10);
         __Pyx_INCREF(__pyx_v_data);
         __Pyx_GIVEREF(__pyx_v_data);
         PyTuple_SET_ITEM(__pyx_t_14, 4+__pyx_t_13, __pyx_v_data);
         __pyx_t_8 = 0;
         __pyx_t_9 = 0;
         __pyx_t_10 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 596, __pyx_L5_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       }
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_v_rc = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "pyjls/binding.pyx":595
+      /* "pyjls/binding.pyx":644
  *     if not isfinite(y):
  *         y = None
  *     try:             # <<<<<<<<<<<<<<
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:
  */
     }
@@ -13047,80 +13709,80 @@
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
     __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "pyjls/binding.pyx":597
+    /* "pyjls/binding.pyx":646
  *     try:
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:             # <<<<<<<<<<<<<<
  *         logging.getLogger(__name__).exception('in annotation callback')
  *         return 1
  */
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("pyjls.binding._annotation_cbk_fn", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_11, &__pyx_t_14) < 0) __PYX_ERR(0, 597, __pyx_L7_except_error)
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_11, &__pyx_t_14) < 0) __PYX_ERR(0, 646, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_GOTREF(__pyx_t_14);
 
-      /* "pyjls/binding.pyx":598
+      /* "pyjls/binding.pyx":647
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:
  *         logging.getLogger(__name__).exception('in annotation callback')             # <<<<<<<<<<<<<<
  *         return 1
  *     return 1 if bool(rc) else 0
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logging); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 598, __pyx_L7_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_logging); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 647, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 598, __pyx_L7_except_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_getLogger); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 647, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_name_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 598, __pyx_L7_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_name_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 647, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_15 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_15)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_15);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_12, function);
         }
       }
       __pyx_t_9 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_15, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_8);
       __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 598, __pyx_L7_except_error)
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 647, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_exception); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 598, __pyx_L7_except_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_exception); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 647, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_t_9 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_12))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_12);
         if (likely(__pyx_t_9)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_9);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_12, function);
         }
       }
       __pyx_t_10 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_9, __pyx_kp_u_in_annotation_callback) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_kp_u_in_annotation_callback);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 598, __pyx_L7_except_error)
+      if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 647, __pyx_L7_except_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-      /* "pyjls/binding.pyx":599
+      /* "pyjls/binding.pyx":648
  *     except Exception:
  *         logging.getLogger(__name__).exception('in annotation callback')
  *         return 1             # <<<<<<<<<<<<<<
  *     return 1 if bool(rc) else 0
  * 
  */
       __pyx_r = 1;
@@ -13128,15 +13790,15 @@
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
       goto __pyx_L8_except_return;
     }
     goto __pyx_L7_except_error;
     __pyx_L7_except_error:;
 
-    /* "pyjls/binding.pyx":595
+    /* "pyjls/binding.pyx":644
  *     if not isfinite(y):
  *         y = None
  *     try:             # <<<<<<<<<<<<<<
  *         rc = obj.cbk_fn(timestamp, y, annotation[0].annotation_type, annotation[0].group_id, data)
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_5);
@@ -13149,31 +13811,31 @@
     __Pyx_XGIVEREF(__pyx_t_6);
     __Pyx_XGIVEREF(__pyx_t_7);
     __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
     goto __pyx_L0;
     __pyx_L10_try_end:;
   }
 
-  /* "pyjls/binding.pyx":600
+  /* "pyjls/binding.pyx":649
  *         logging.getLogger(__name__).exception('in annotation callback')
  *         return 1
  *     return 1 if bool(rc) else 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 600, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 649, __pyx_L1_error)
   if (((!(!__pyx_t_3)) != 0)) {
     __pyx_t_16 = 1;
   } else {
     __pyx_t_16 = 0;
   }
   __pyx_r = __pyx_t_16;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":586
+  /* "pyjls/binding.pyx":635
  * 
  * 
  * cdef int32_t _annotation_cbk_fn(void * user_data, const c_jls.jls_annotation_s * annotation):             # <<<<<<<<<<<<<<
  *     obj: AnnotationCallback = <object> user_data
  *     data = _storage_unpack(annotation[0].storage_type, annotation[0].data, annotation[0].data_size)
  */
 
@@ -13194,15 +13856,15 @@
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_y);
   __Pyx_XDECREF(__pyx_v_rc);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":603
+/* "pyjls/binding.pyx":652
  * 
  * 
  * cdef int32_t _user_data_cbk_fn(void * user_data, uint16_t chunk_meta, c_jls.jls_storage_type_e storage_type,             # <<<<<<<<<<<<<<
  *         uint8_t * data, uint32_t data_size):
  *     cbk_fn = <object> user_data
  */
 
@@ -13221,46 +13883,46 @@
   int32_t __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_user_data_cbk_fn", 0);
 
-  /* "pyjls/binding.pyx":605
+  /* "pyjls/binding.pyx":654
  * cdef int32_t _user_data_cbk_fn(void * user_data, uint16_t chunk_meta, c_jls.jls_storage_type_e storage_type,
  *         uint8_t * data, uint32_t data_size):
  *     cbk_fn = <object> user_data             # <<<<<<<<<<<<<<
  *     d = _storage_unpack(storage_type, data, data_size)
  *     rc = cbk_fn(chunk_meta, d)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_cbk_fn = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":606
+  /* "pyjls/binding.pyx":655
  *         uint8_t * data, uint32_t data_size):
  *     cbk_fn = <object> user_data
  *     d = _storage_unpack(storage_type, data, data_size)             # <<<<<<<<<<<<<<
  *     rc = cbk_fn(chunk_meta, d)
  *     return 1 if bool(rc) else 0
  */
-  __pyx_t_1 = __pyx_f_5pyjls_7binding__storage_unpack(__pyx_v_storage_type, __pyx_v_data, __pyx_v_data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_5pyjls_7binding__storage_unpack(__pyx_v_storage_type, __pyx_v_data, __pyx_v_data_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_d = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":607
+  /* "pyjls/binding.pyx":656
  *     cbk_fn = <object> user_data
  *     d = _storage_unpack(storage_type, data, data_size)
  *     rc = cbk_fn(chunk_meta, d)             # <<<<<<<<<<<<<<
  *     return 1 if bool(rc) else 0
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_chunk_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_chunk_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 656, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_cbk_fn);
   __pyx_t_3 = __pyx_v_cbk_fn; __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -13270,66 +13932,66 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_d};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 656, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_d};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 656, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 656, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_t_2);
     __Pyx_INCREF(__pyx_v_d);
     __Pyx_GIVEREF(__pyx_v_d);
     PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_v_d);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 656, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_rc = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":608
+  /* "pyjls/binding.pyx":657
  *     d = _storage_unpack(storage_type, data, data_size)
  *     rc = cbk_fn(chunk_meta, d)
  *     return 1 if bool(rc) else 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 608, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 657, __pyx_L1_error)
   if (((!(!__pyx_t_8)) != 0)) {
     __pyx_t_7 = 1;
   } else {
     __pyx_t_7 = 0;
   }
   __pyx_r = __pyx_t_7;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":603
+  /* "pyjls/binding.pyx":652
  * 
  * 
  * cdef int32_t _user_data_cbk_fn(void * user_data, uint16_t chunk_meta, c_jls.jls_storage_type_e storage_type,             # <<<<<<<<<<<<<<
  *         uint8_t * data, uint32_t data_size):
  *     cbk_fn = <object> user_data
  */
 
@@ -13346,15 +14008,15 @@
   __Pyx_XDECREF(__pyx_v_cbk_fn);
   __Pyx_XDECREF(__pyx_v_d);
   __Pyx_XDECREF(__pyx_v_rc);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyjls/binding.pyx":611
+/* "pyjls/binding.pyx":660
  * 
  * 
  * cdef int32_t _utc_cbk_fn(void * user_data, const c_jls.jls_utc_summary_entry_s * utc, uint32_t size):             # <<<<<<<<<<<<<<
  *     cdef uint32_t idx
  *     cbk_fn = <object> user_data
  */
 
@@ -13376,130 +14038,130 @@
   int32_t __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_utc_cbk_fn", 0);
 
-  /* "pyjls/binding.pyx":613
+  /* "pyjls/binding.pyx":662
  * cdef int32_t _utc_cbk_fn(void * user_data, const c_jls.jls_utc_summary_entry_s * utc, uint32_t size):
  *     cdef uint32_t idx
  *     cbk_fn = <object> user_data             # <<<<<<<<<<<<<<
  *     entries = np.empty((size, 2), dtype=np.int64)
  *     for idx in range(size):
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_user_data);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_cbk_fn = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyjls/binding.pyx":614
+  /* "pyjls/binding.pyx":663
  *     cdef uint32_t idx
  *     cbk_fn = <object> user_data
  *     entries = np.empty((size, 2), dtype=np.int64)             # <<<<<<<<<<<<<<
  *     for idx in range(size):
  *         entries[idx, 0] = utc[idx].sample_id
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_2);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 614, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_entries = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "pyjls/binding.pyx":615
+  /* "pyjls/binding.pyx":664
  *     cbk_fn = <object> user_data
  *     entries = np.empty((size, 2), dtype=np.int64)
  *     for idx in range(size):             # <<<<<<<<<<<<<<
  *         entries[idx, 0] = utc[idx].sample_id
  *         entries[idx, 1] = utc[idx].timestamp
  */
   __pyx_t_6 = __pyx_v_size;
   __pyx_t_7 = __pyx_t_6;
   for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
     __pyx_v_idx = __pyx_t_8;
 
-    /* "pyjls/binding.pyx":616
+    /* "pyjls/binding.pyx":665
  *     entries = np.empty((size, 2), dtype=np.int64)
  *     for idx in range(size):
  *         entries[idx, 0] = utc[idx].sample_id             # <<<<<<<<<<<<<<
  *         entries[idx, 1] = utc[idx].timestamp
  *     rc = cbk_fn(entries)
  */
-    __pyx_t_5 = __Pyx_PyInt_From_int64_t((__pyx_v_utc[__pyx_v_idx]).sample_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int64_t((__pyx_v_utc[__pyx_v_idx]).sample_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint32_t(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_0);
     __pyx_t_3 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_entries, __pyx_t_1, __pyx_t_5) < 0)) __PYX_ERR(0, 616, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_entries, __pyx_t_1, __pyx_t_5) < 0)) __PYX_ERR(0, 665, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "pyjls/binding.pyx":617
+    /* "pyjls/binding.pyx":666
  *     for idx in range(size):
  *         entries[idx, 0] = utc[idx].sample_id
  *         entries[idx, 1] = utc[idx].timestamp             # <<<<<<<<<<<<<<
  *     rc = cbk_fn(entries)
  *     return 1 if bool(rc) else 0
  */
-    __pyx_t_5 = __Pyx_PyInt_From_int64_t((__pyx_v_utc[__pyx_v_idx]).timestamp); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 617, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int64_t((__pyx_v_utc[__pyx_v_idx]).timestamp); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 666, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 617, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_idx); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 666, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 617, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 666, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_1);
     __pyx_t_1 = 0;
-    if (unlikely(PyObject_SetItem(__pyx_v_entries, __pyx_t_3, __pyx_t_5) < 0)) __PYX_ERR(0, 617, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(__pyx_v_entries, __pyx_t_3, __pyx_t_5) < 0)) __PYX_ERR(0, 666, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
 
-  /* "pyjls/binding.pyx":618
+  /* "pyjls/binding.pyx":667
  *         entries[idx, 0] = utc[idx].sample_id
  *         entries[idx, 1] = utc[idx].timestamp
  *     rc = cbk_fn(entries)             # <<<<<<<<<<<<<<
  *     return 1 if bool(rc) else 0
  */
   __Pyx_INCREF(__pyx_v_cbk_fn);
   __pyx_t_3 = __pyx_v_cbk_fn; __pyx_t_1 = NULL;
@@ -13510,35 +14172,35 @@
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_5 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_v_entries) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_entries);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 618, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_rc = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "pyjls/binding.pyx":619
+  /* "pyjls/binding.pyx":668
  *         entries[idx, 1] = utc[idx].timestamp
  *     rc = cbk_fn(entries)
  *     return 1 if bool(rc) else 0             # <<<<<<<<<<<<<<
  */
-  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_v_rc); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 668, __pyx_L1_error)
   if (((!(!__pyx_t_10)) != 0)) {
     __pyx_t_9 = 1;
   } else {
     __pyx_t_9 = 0;
   }
   __pyx_r = __pyx_t_9;
   goto __pyx_L0;
 
-  /* "pyjls/binding.pyx":611
+  /* "pyjls/binding.pyx":660
  * 
  * 
  * cdef int32_t _utc_cbk_fn(void * user_data, const c_jls.jls_utc_summary_entry_s * utc, uint32_t size):             # <<<<<<<<<<<<<<
  *     cdef uint32_t idx
  *     cbk_fn = <object> user_data
  */
 
@@ -13662,15 +14324,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x03191f0, 0xbf06ca6, 0x802df30):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x03191f0, 0xbf06ca6, 0x802df30) = (cbk_fn, is_fsr))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__12, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__13, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x03191f0, 0xbf06ca6, 0x802df30):
@@ -14498,15 +15160,15 @@
       /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -14630,15 +15292,15 @@
       /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -14762,15 +15424,15 @@
       /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -15186,15 +15848,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -15218,15 +15880,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -15345,15 +16007,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -15619,15 +16281,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(1, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -15863,15 +16525,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -16597,15 +17259,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -16653,15 +17315,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -18382,15 +19044,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -19430,15 +20092,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(1, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -19792,15 +20454,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -20341,15 +21003,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -20458,15 +21120,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__26, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__27, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -21496,15 +22158,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -21552,15 +22214,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -21909,17 +22571,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__29);
-            __Pyx_GIVEREF(__pyx_slice__29);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__29);
+            __Pyx_INCREF(__pyx_slice__30);
+            __Pyx_GIVEREF(__pyx_slice__30);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__30);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -21944,15 +22606,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__29); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__30); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -22084,17 +22746,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__29);
-        __Pyx_GIVEREF(__pyx_slice__29);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__29);
+        __Pyx_INCREF(__pyx_slice__30);
+        __Pyx_GIVEREF(__pyx_slice__30);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__30);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -22213,15 +22875,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(1, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -24397,15 +25059,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -24453,15 +25115,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -27730,15 +28392,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__33, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__34, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -28130,15 +28792,15 @@
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
 
 static PyObject *__pyx_tp_new_5pyjls_7binding_AnnotationCallback(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5pyjls_7binding_AnnotationCallback *p;
   PyObject *o;
@@ -28252,15 +28914,15 @@
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
 
 static PyObject *__pyx_tp_new_5pyjls_7binding_Reader(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5pyjls_7binding_Reader *p;
   PyObject *o;
@@ -28406,15 +29068,15 @@
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
@@ -28598,15 +29260,15 @@
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
@@ -28720,15 +29382,15 @@
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
@@ -28984,15 +29646,15 @@
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
@@ -29133,15 +29795,15 @@
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
@@ -29275,19 +29937,21 @@
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_u_W, __pyx_k_W, sizeof(__pyx_k_W), 0, 1, 0, 1},
   {&__pyx_n_s_WARNING, __pyx_k_WARNING, sizeof(__pyx_k_WARNING), 0, 0, 1, 1},
   {&__pyx_n_s_Writer, __pyx_k_Writer, sizeof(__pyx_k_Writer), 0, 0, 1, 1},
   {&__pyx_n_u_Writer, __pyx_k_Writer, sizeof(__pyx_k_Writer), 0, 1, 0, 1},
   {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
+  {&__pyx_kp_b__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 0, 0, 0},
   {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
-  {&__pyx_kp_u__42, __pyx_k__42, sizeof(__pyx_k__42), 0, 1, 0, 0},
-  {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
+  {&__pyx_kp_u__43, __pyx_k__43, sizeof(__pyx_k__43), 0, 1, 0, 0},
+  {&__pyx_kp_b__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 0, 0},
   {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
   {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
+  {&__pyx_kp_u__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 1, 0, 0},
   {&__pyx_n_s_all, __pyx_k_all, sizeof(__pyx_k_all), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_u_annotation, __pyx_k_annotation, sizeof(__pyx_k_annotation), 0, 1, 0, 1},
   {&__pyx_n_s_annotation_decimate_factor, __pyx_k_annotation_decimate_factor, sizeof(__pyx_k_annotation_decimate_factor), 0, 0, 1, 1},
   {&__pyx_n_s_annotation_map, __pyx_k_annotation_map, sizeof(__pyx_k_annotation_map), 0, 0, 1, 1},
   {&__pyx_n_s_annotation_type, __pyx_k_annotation_type, sizeof(__pyx_k_annotation_type), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
@@ -29508,18 +30172,18 @@
   {&__pyx_n_u_vertical_marker, __pyx_k_vertical_marker, sizeof(__pyx_k_vertical_marker), 0, 1, 0, 1},
   {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
   {&__pyx_n_u_vmarker, __pyx_k_vmarker, sizeof(__pyx_k_vmarker), 0, 1, 0, 1},
   {&__pyx_n_s_y, __pyx_k_y, sizeof(__pyx_k_y), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 249, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 388, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 467, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 152, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
   return 0;
@@ -29544,460 +30208,460 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_self__wr_cannot_be_converted_to); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_self__wr_cannot_be_converted_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._wr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_self__wr_cannot_be_converted_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_self__wr_cannot_be_converted_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__10);
+  __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_self__rd_cannot_be_converted_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_self__rd_cannot_be_converted_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
   /* "(tree fragment)":4
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._rd cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_self__rd_cannot_be_converted_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_tuple__12 = PyTuple_Pack(3, __pyx_int_3248624, __pyx_int_200305830, __pyx_int_134405936); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_self__rd_cannot_be_converted_to); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_3248624, __pyx_int_200305830, __pyx_int_134405936); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 944, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 944, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "../../../bin/Python3_8_10/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 950, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__26 = PyTuple_New(1); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
+  __pyx_tuple__27 = PyTuple_New(1); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__26, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  PyTuple_SET_ITEM(__pyx_tuple__27, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__29 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__29)) __PYX_ERR(1, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__29);
-  __Pyx_GIVEREF(__pyx_slice__29);
+  __pyx_slice__30 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__30)) __PYX_ERR(1, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__30);
+  __Pyx_GIVEREF(__pyx_slice__30);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_tuple__33 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__34 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "pyjls/binding.pyx":50
  * 
  * 
  * def _data_type_def(basetype, size, q):             # <<<<<<<<<<<<<<
  *     return (basetype & 0x0f) | ((size & 0xff) << 8) | ((q & 0xff) << 16)
  * 
  */
-  __pyx_tuple__34 = PyTuple_Pack(3, __pyx_n_s_basetype, __pyx_n_s_size, __pyx_n_s_q); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_def, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(3, __pyx_n_s_basetype, __pyx_n_s_size, __pyx_n_s_q); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_def, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 50, __pyx_L1_error)
 
   /* "pyjls/binding.pyx":120
  * 
  * 
  * def _populate_data_type():             # <<<<<<<<<<<<<<
  *     for key, value in list(_data_type_as_enum.items()):
  *         _data_type_as_enum[value] = value
  */
-  __pyx_tuple__36 = PyTuple_Pack(2, __pyx_n_s_key, __pyx_n_s_value); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 120, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_populate_data_type, 120, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(2, __pyx_n_s_key, __pyx_n_s_value); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_populate_data_type, 120, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 120, __pyx_L1_error)
 
   /* "pyjls/binding.pyx":130
  * 
  * 
  * def data_type_as_enum(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_enum[data_type]
  * 
  */
-  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_n_s_data_type); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 130, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_as_enum_2, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_n_s_data_type); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_as_enum_2, 130, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 130, __pyx_L1_error)
 
   /* "pyjls/binding.pyx":134
  * 
  * 
  * def data_type_as_str(data_type):             # <<<<<<<<<<<<<<
  *     return _data_type_as_str[data_type]
  * 
  */
-  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_n_s_data_type); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_as_str_2, 134, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_n_s_data_type); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_data_type_as_str_2, 134, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 134, __pyx_L1_error)
 
   /* "pyjls/binding.pyx":199
  * 
  * 
  * def jls_inject_log(level, filename, line, msg):             # <<<<<<<<<<<<<<
  *     cdef char * c_msg
  *     location = ':'.join([filename, str(line), ''])
  */
-  __pyx_tuple__43 = PyTuple_Pack(6, __pyx_n_s_level, __pyx_n_s_filename, __pyx_n_s_line, __pyx_n_s_msg, __pyx_n_s_c_msg, __pyx_n_s_location); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 199, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__43);
-  __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(4, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_jls_inject_log, 199, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_tuple__44 = PyTuple_Pack(6, __pyx_n_s_level, __pyx_n_s_filename, __pyx_n_s_line, __pyx_n_s_msg, __pyx_n_s_c_msg, __pyx_n_s_location); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__44);
+  __Pyx_GIVEREF(__pyx_tuple__44);
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(4, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_jls_inject_log, 199, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 199, __pyx_L1_error)
 
   /* "pyjls/binding.pyx":207
  * 
  * 
  * def _encode_str(s):             # <<<<<<<<<<<<<<
  *     if s is None:
  *         s = ''
  */
-  __pyx_tuple__45 = PyTuple_Pack(1, __pyx_n_s_s_2); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 207, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_encode_str, 207, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __pyx_tuple__46 = PyTuple_Pack(1, __pyx_n_s_s_2); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 207, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
+  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_encode_str, 207, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 207, __pyx_L1_error)
 
   /* "pyjls/binding.pyx":213
  * 
  * 
  * def _storage_pack(data):             # <<<<<<<<<<<<<<
- *     if isinstance(data, str):
- *         s = _encode_str(data)
+ *     if data is None:
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
  */
-  __pyx_tuple__47 = PyTuple_Pack(2, __pyx_n_s_data, __pyx_n_s_s_2); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 213, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__47);
-  __Pyx_GIVEREF(__pyx_tuple__47);
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_storage_pack, 213, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_tuple__48 = PyTuple_Pack(2, __pyx_n_s_data, __pyx_n_s_s_2); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_storage_pack, 213, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 213, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":234
+  /* "pyjls/binding.pyx":236
  * 
  * 
  * def utc_to_jls(utc):             # <<<<<<<<<<<<<<
  *     """Convert from python UTC timestamp to jls timestamp."""
  *     return int((utc - _UTC_OFFSET) * SECOND)
  */
-  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_n_s_utc); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 234, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__49);
-  __Pyx_GIVEREF(__pyx_tuple__49);
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__49, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_utc_to_jls, 234, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_tuple__50 = PyTuple_Pack(1, __pyx_n_s_utc); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__50);
+  __Pyx_GIVEREF(__pyx_tuple__50);
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_utc_to_jls, 236, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 236, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":239
+  /* "pyjls/binding.pyx":241
  * 
  * 
  * def jls_to_utc(timestamp):             # <<<<<<<<<<<<<<
  *     """Convert from jls timestamp to python UTC timestamp."""
  *     return (timestamp / SECOND) + _UTC_OFFSET
  */
-  __pyx_tuple__51 = PyTuple_Pack(1, __pyx_n_s_timestamp); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 239, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__51);
-  __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_codeobj__52 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__51, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_jls_to_utc, 239, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__52)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(1, __pyx_n_s_timestamp); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_jls_to_utc, 241, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 241, __pyx_L1_error)
 
-  /* "pyjls/binding.pyx":244
+  /* "pyjls/binding.pyx":246
  * 
  * 
  * def _handle_rc(name, rc):             # <<<<<<<<<<<<<<
  *     if rc == 0:
  *         return
  */
-  __pyx_tuple__53 = PyTuple_Pack(4, __pyx_n_s_name, __pyx_n_s_rc, __pyx_n_s_rc_name, __pyx_n_s_rc_descr); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 244, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__53);
-  __Pyx_GIVEREF(__pyx_tuple__53);
-  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__53, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_handle_rc, 244, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(4, __pyx_n_s_name, __pyx_n_s_rc, __pyx_n_s_rc_name, __pyx_n_s_rc_descr); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__54);
+  __Pyx_GIVEREF(__pyx_tuple__54);
+  __pyx_codeobj__55 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__54, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyjls_binding_pyx, __pyx_n_s_handle_rc, 246, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__55)) __PYX_ERR(0, 246, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_AnnotationCallback(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__55 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__55);
-  __Pyx_GIVEREF(__pyx_tuple__55);
-  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AnnotationCallbac, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__56);
+  __Pyx_GIVEREF(__pyx_tuple__56);
+  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__56, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AnnotationCallbac, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__57 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__57);
-  __Pyx_GIVEREF(__pyx_tuple__57);
+  __pyx_tuple__58 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__58);
+  __Pyx_GIVEREF(__pyx_tuple__58);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__58 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__58);
-  __Pyx_GIVEREF(__pyx_tuple__58);
+  __pyx_tuple__59 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__59);
+  __Pyx_GIVEREF(__pyx_tuple__59);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__59 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(1, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__59);
-  __Pyx_GIVEREF(__pyx_tuple__59);
+  __pyx_tuple__60 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__60);
+  __Pyx_GIVEREF(__pyx_tuple__60);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__60 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__60);
-  __Pyx_GIVEREF(__pyx_tuple__60);
+  __pyx_tuple__61 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__61);
+  __Pyx_GIVEREF(__pyx_tuple__61);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__61 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(1, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__61);
-  __Pyx_GIVEREF(__pyx_tuple__61);
+  __pyx_tuple__62 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__62);
+  __Pyx_GIVEREF(__pyx_tuple__62);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__62 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__62);
-  __Pyx_GIVEREF(__pyx_tuple__62);
-  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__62, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__63);
+  __Pyx_GIVEREF(__pyx_tuple__63);
+  __pyx_codeobj__64 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__63, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__64)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -30069,43 +30733,43 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5pyjls_7binding_Writer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5pyjls_7binding_Writer.tp_dictoffset && __pyx_type_5pyjls_7binding_Writer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5pyjls_7binding_Writer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Writer, (PyObject *)&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Writer, (PyObject *)&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_Writer) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
   __pyx_ptype_5pyjls_7binding_Writer = &__pyx_type_5pyjls_7binding_Writer;
-  if (PyType_Ready(&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 440, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5pyjls_7binding_AnnotationCallback.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5pyjls_7binding_AnnotationCallback.tp_dictoffset && __pyx_type_5pyjls_7binding_AnnotationCallback.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5pyjls_7binding_AnnotationCallback.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnnotationCallback, (PyObject *)&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AnnotationCallback, (PyObject *)&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 440, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_AnnotationCallback) < 0) __PYX_ERR(0, 440, __pyx_L1_error)
   __pyx_ptype_5pyjls_7binding_AnnotationCallback = &__pyx_type_5pyjls_7binding_AnnotationCallback;
-  if (PyType_Ready(&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_5pyjls_7binding_Reader.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_5pyjls_7binding_Reader.tp_dictoffset && __pyx_type_5pyjls_7binding_Reader.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_5pyjls_7binding_Reader.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Reader, (PyObject *)&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Reader, (PyObject *)&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_5pyjls_7binding_Reader) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
   __pyx_ptype_5pyjls_7binding_Reader = &__pyx_type_5pyjls_7binding_Reader;
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 106, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
@@ -30167,70 +30831,39 @@
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
@@ -32402,15 +33035,15 @@
   __pyx_t_2 = __Pyx_PyDict_NewPresized(10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_logging); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_CRITICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u__42, __pyx_t_3) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_kp_u__43, __pyx_t_3) < 0) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pyjls/binding.pyx":161
  * _log_level_map = {
  *     '!': logging.CRITICAL,
  *     'A': logging.CRITICAL,             # <<<<<<<<<<<<<<
  *     'C': logging.CRITICAL,
@@ -32709,56 +33342,56 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode_str, __pyx_t_2) < 0) __PYX_ERR(0, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pyjls/binding.pyx":213
  * 
  * 
  * def _storage_pack(data):             # <<<<<<<<<<<<<<
- *     if isinstance(data, str):
- *         s = _encode_str(data)
+ *     if data is None:
+ *         return c_jls.JLS_STORAGE_TYPE_BINARY, b'', 0
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_13_storage_pack, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_storage_pack, __pyx_t_2) < 0) __PYX_ERR(0, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":234
+  /* "pyjls/binding.pyx":236
  * 
  * 
  * def utc_to_jls(utc):             # <<<<<<<<<<<<<<
  *     """Convert from python UTC timestamp to jls timestamp."""
  *     return int((utc - _UTC_OFFSET) * SECOND)
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_15utc_to_jls, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_15utc_to_jls, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_utc_to_jls, __pyx_t_2) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_utc_to_jls, __pyx_t_2) < 0) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":239
+  /* "pyjls/binding.pyx":241
  * 
  * 
  * def jls_to_utc(timestamp):             # <<<<<<<<<<<<<<
  *     """Convert from jls timestamp to python UTC timestamp."""
  *     return (timestamp / SECOND) + _UTC_OFFSET
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_17jls_to_utc, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_17jls_to_utc, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_jls_to_utc, __pyx_t_2) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_jls_to_utc, __pyx_t_2) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyjls/binding.pyx":244
+  /* "pyjls/binding.pyx":246
  * 
  * 
  * def _handle_rc(name, rc):             # <<<<<<<<<<<<<<
  *     if rc == 0:
  *         return
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_19_handle_rc, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_5pyjls_7binding_19_handle_rc, NULL, __pyx_n_s_pyjls_binding); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_handle_rc, __pyx_t_2) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_handle_rc, __pyx_t_2) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_AnnotationCallback(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
@@ -32793,71 +33426,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__57, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__58, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__58, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__59, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__59, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__60, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__60, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__61, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__61, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__62, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":317
@@ -34296,14 +34929,25 @@
 
 /* BufferIndexError */
 static void __Pyx_RaiseBufferIndexError(int axis) {
   PyErr_Format(PyExc_IndexError,
      "Out of bounds on buffer access (axis %d)", axis);
 }
 
+/* BufferIndexErrorNogil */
+static void __Pyx_RaiseBufferIndexErrorNogil(int axis) {
+    #ifdef WITH_THREAD
+    PyGILState_STATE gilstate = PyGILState_Ensure();
+    #endif
+    __Pyx_RaiseBufferIndexError(axis);
+    #ifdef WITH_THREAD
+    PyGILState_Release(gilstate);
+    #endif
+}
+
 /* MemviewSliceInit */
 static int
 __Pyx_init_memviewslice(struct __pyx_memoryview_obj *memview,
                         int ndim,
                         __Pyx_memviewslice *memviewslice,
                         int memview_is_new_reference)
 {
@@ -34818,25 +35462,14 @@
 static CYTHON_INLINE long __Pyx_div_long(long a, long b) {
     long q = a / b;
     long r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
-/* BufferIndexErrorNogil */
-static void __Pyx_RaiseBufferIndexErrorNogil(int axis) {
-    #ifdef WITH_THREAD
-    PyGILState_STATE gilstate = PyGILState_Ensure();
-    #endif
-    __Pyx_RaiseBufferIndexError(axis);
-    #ifdef WITH_THREAD
-    PyGILState_Release(gilstate);
-    #endif
-}
-
 /* ExtTypeTest */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
@@ -35566,18 +36199,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
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
@@ -35623,22 +36256,22 @@
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
@@ -36830,14 +37463,37 @@
     retval = -1;
 no_fail:
     __Pyx_RefNannyFinishContext();
     return retval;
 }
 
 /* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds_nn_uint8_t__const__(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 1,
+                                                 &__Pyx_TypeInfo_nn_uint8_t__const__, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* ObjectToMemviewSlice */
   static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_nn___pyx_t_5numpy_uint8_t(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
     int retcode;
     if (obj == Py_None) {
         result.memview = (struct __pyx_memoryview_obj *) Py_None;
@@ -37348,15 +38004,15 @@
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
@@ -37658,15 +38314,15 @@
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
@@ -37892,15 +38548,15 @@
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
@@ -38126,15 +38782,15 @@
                         } else if (8 * sizeof(uint16_t) >= 4 * PyLong_SHIFT) {
                             return (uint16_t) (((((((((uint16_t)digits[3]) << PyLong_SHIFT) | (uint16_t)digits[2]) << PyLong_SHIFT) | (uint16_t)digits[1]) << PyLong_SHIFT) | (uint16_t)digits[0]));
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
@@ -38322,15 +38978,15 @@
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
@@ -38518,15 +39174,15 @@
                         } else if (8 * sizeof(enum jls_storage_type_e) >= 4 * PyLong_SHIFT) {
                             return (enum jls_storage_type_e) (((((((((enum jls_storage_type_e)digits[3]) << PyLong_SHIFT) | (enum jls_storage_type_e)digits[2]) << PyLong_SHIFT) | (enum jls_storage_type_e)digits[1]) << PyLong_SHIFT) | (enum jls_storage_type_e)digits[0]));
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
@@ -38654,52 +39310,14 @@
     return (enum jls_storage_type_e) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to enum jls_storage_type_e");
     return (enum jls_storage_type_e) -1;
 }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
   static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
@@ -38752,15 +39370,15 @@
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
@@ -38888,14 +39506,52 @@
     return (int64_t) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int64_t");
     return (int64_t) -1;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE enum jls_annotation_type_e __Pyx_PyInt_As_enum__jls_annotation_type_e(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum jls_annotation_type_e neg_one = (enum jls_annotation_type_e) -1, const_zero = (enum jls_annotation_type_e) 0;
@@ -38948,15 +39604,15 @@
                         } else if (8 * sizeof(enum jls_annotation_type_e) >= 4 * PyLong_SHIFT) {
                             return (enum jls_annotation_type_e) (((((((((enum jls_annotation_type_e)digits[3]) << PyLong_SHIFT) | (enum jls_annotation_type_e)digits[2]) << PyLong_SHIFT) | (enum jls_annotation_type_e)digits[1]) << PyLong_SHIFT) | (enum jls_annotation_type_e)digits[0]));
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
@@ -39296,15 +39952,15 @@
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

### Comparing `pyjls-0.6.3/pyjls/entry_points/__init__.py` & `pyjls-0.7.0/pyjls/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/entry_points/annotate.py` & `pyjls-0.7.0/pyjls/entry_points/annotate.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/entry_points/export.py` & `pyjls-0.7.0/pyjls/entry_points/export.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/entry_points/info.py` & `pyjls-0.7.0/pyjls/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/structs.py` & `pyjls-0.7.0/pyjls/structs.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/test/__init__.py` & `pyjls-0.7.0/pyjls/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/test/test_binding.py` & `pyjls-0.7.0/pyjls/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/v1/__init__.py` & `pyjls-0.7.0/pyjls/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyjls/version.py` & `pyjls-0.7.0/pyjls/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.6.3"
+__version__ = "0.7.0"
 
 __title__ = "pyjls"
 __description__ = 'Joulescope™ file format'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjls-0.6.3/pyjls.egg-info/PKG-INFO` & `pyjls-0.7.0/pyjls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.6.3
+Version: 0.7.0
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.6.3/pyjls.egg-info/SOURCES.txt` & `pyjls-0.7.0/pyjls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/pyproject.toml` & `pyjls-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/setup.py` & `pyjls-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/backend_posix.c` & `pyjls-0.7.0/src/backend_posix.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/backend_win.c` & `pyjls-0.7.0/src/backend_win.c`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             0,                      // use default creation flags
             NULL);                  // returns the thread identifier
     if (!self->thread) {
         jls_bkt_finalize(self);
         wr->bk = NULL;
         return NULL;
     }
-    if (!SetThreadPriority(self->thread, THREAD_PRIORITY_BELOW_NORMAL)) {
+    if (!SetThreadPriority(self->thread, THREAD_PRIORITY_ABOVE_NORMAL)) {
         JLS_LOGW("Could not reduce thread priority: %d", (int) GetLastError());
     }
     return self;
 }
 
 void jls_bkt_finalize(struct jls_bkt_s * self) {
     if (self) {
```

### Comparing `pyjls-0.6.3/src/bit_shift.c` & `pyjls-0.7.0/src/bit_shift.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/crc32c_arm_neon.c` & `pyjls-0.7.0/src/crc32c_arm_neon.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/crc32c_intel_sse4.c` & `pyjls-0.7.0/src/crc32c_intel_sse4.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/crc32c_sw.c` & `pyjls-0.7.0/src/crc32c_sw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/datatype.c` & `pyjls-0.7.0/src/datatype.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/ec.c` & `pyjls-0.7.0/src/ec.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/log.c` & `pyjls-0.7.0/src/log.c`

 * *Files 18% similar despite different names*

```diff
@@ -58,7 +58,27 @@
         cbk_ = handler;
     }
 }
 
 JLS_API void jls_log_unregister(void) {
     jls_log_register(NULL);
 }
+
+JLS_API const char * jls_log_level_to_str(int8_t level) {
+    if (level < 0) {
+        return "OFF";
+    }
+    if (level >= JLS_LOG_LEVEL_ALL) {
+        return jls_log_level_str[JLS_LOG_LEVEL_ALL];
+    }
+    return jls_log_level_str[level];
+}
+
+JLS_API char jls_log_level_to_char(int8_t level) {
+    if (level < 0) {
+        return '*';
+    }
+    if (level >= JLS_LOG_LEVEL_ALL) {
+        return jls_log_level_char[JLS_LOG_LEVEL_ALL];
+    }
+    return jls_log_level_char[level];
+}
```

### Comparing `pyjls-0.6.3/src/msg_ring_buffer.c` & `pyjls-0.7.0/src/msg_ring_buffer.c`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,22 @@
 void jls_mrb_clear(struct jls_mrb_s * self) {
     self->head = 0;
     self->tail = 0;
     self->count = 0;
     memset(self->buf, 0, self->buf_size);
 }
 
+uint32_t jls_mrb_used_bytes(struct jls_mrb_s * self) {
+    if (self->head > self->tail) {
+        return self->head - self->tail;
+    } else {
+        return (self-> head + self->buf_size) - self->tail;
+    }
+}
+
 static inline uint8_t * add_sz(uint8_t * p, uint32_t sz) {
     p[0] = sz & 0xff;
     p[1] = (sz >> 8) & 0xff;
     p[2] = (sz >> 16) & 0xff;
     p[3] = (sz >> 24) & 0xff;
     return (p + 4);
 }
```

### Comparing `pyjls-0.6.3/src/raw.c` & `pyjls-0.7.0/src/raw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/rd_fsr.c` & `pyjls-0.7.0/src/rd_fsr.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/reader.c` & `pyjls-0.7.0/src/reader.c`

 * *Files 0% similar despite different names*

```diff
@@ -595,14 +595,15 @@
     if (jls_raw_version(self->raw).s.major < 1) {
         JLS_LOGE("version < 1.x.x no longer supported");
         return JLS_ERROR_UNSUPPORTED_FILE;
     }
 
     int64_t end_pos = jls_raw_chunk_tell_end(self->raw);
     if (!end_pos) {
+        JLS_LOGW("not properly closed");
         // Not properly closed.  Indices & summary may be incomplete.
         // for most applications, will want to launch file reconstruction tool
         return JLS_ERROR_MESSAGE_INTEGRITY;
     }
 
     ROE(scan(self));
     *instance = self;
@@ -764,44 +765,48 @@
         }
     }
     if (!offset) {
         return JLS_ERROR_NOT_FOUND;
     }
 
     for (int lvl = initial_level; lvl > level; --lvl) {
-        JLS_LOGD3("signal %d, level %d, offset=%" PRIi64, (int) signal_id, lvl, offset);
-
         // compute the step size in samples between each index entry.
         int64_t step_size = signal_def->samples_per_data;  // each data chunk
         if (lvl > 1) {
             step_size *= signal_def->entries_per_summary /
                     (signal_def->samples_per_data / signal_def->sample_decimate_factor);
         }
         for (int k = 3; k <= lvl; ++k) {
             step_size *= signal_def->summary_decimate_factor;
         }
+        JLS_LOGD3("signal %d, level %d, offset=%" PRIi64 ", step_size=%" PRIi64,
+                 (int) signal_id, lvl, offset, step_size);
         ROE(jls_raw_chunk_seek(self->raw, offset));
         ROE(rd(self));
         if (self->chunk_cur.hdr.tag != JLS_TAG_TRACK_FSR_INDEX) {
             JLS_LOGW("seek tag mismatch: %d", (int) self->chunk_cur.hdr.tag);
         }
 
         struct jls_fsr_index_s * r = (struct jls_fsr_index_s *) self->payload.start;
         int64_t chunk_timestamp = r->header.timestamp;
         int64_t chunk_entries = r->header.entry_count;
+        JLS_LOGD3("timestamp=%" PRIi64 ", entries=%" PRIi64, chunk_timestamp, chunk_entries);
         uint8_t * p_end = (uint8_t *) &r->offsets[r->header.entry_count];
 
         if ((size_t) (p_end - self->payload.start) > self->payload.length) {
             JLS_LOGE("invalid payload length");
             return JLS_ERROR_PARAMETER_INVALID;
         }
 
         int64_t idx = (sample_id - chunk_timestamp) / step_size;
         if ((idx < 0) || (idx >= chunk_entries)) {
-            JLS_LOGE("invalid index: %" PRIi64 " >= %" PRIi64, idx, chunk_entries);
+            JLS_LOGE("invalid index signal %d, level %d, sample_id=%"
+                     PRIi64 " offset=%" PRIi64 ": %" PRIi64 " >= %" PRIi64,
+                     (int) signal_id, lvl, sample_id,
+                     offset, idx, chunk_entries);
             return JLS_ERROR_IO;
         }
         offset = r->offsets[idx];
     }
 
     ROE(jls_raw_chunk_seek(self->raw, offset));
     return 0;
@@ -1129,25 +1134,26 @@
                 f64_to_stats(&stats_next, f64_summary->data[src_offset], incr_remaining);
             }
             jls_statistics_combine(&stats_accum, &stats_accum, &stats_next);
             stats_to_f64(data, &stats_accum);
             data += JLS_SUMMARY_FSR_COUNT;
             --data_length;
             int64_t incr = step_size - incr_remaining;
-            if (incr) {
-                if (is_f32) {
-                    f32_to_stats(&stats_accum, f32_summary->data[src_offset], incr);
-                } else {
-                    f64_to_stats(&stats_accum, f64_summary->data[src_offset], incr);
-                }
-                incr_remaining = increment - incr;
-            } else {
+            if (incr < 0) {
+                JLS_LOGE("internal error");
+                incr = 0;
                 jls_statistics_reset(&stats_accum);
-                incr_remaining = increment;
+            } else if (incr == 0) {
+                jls_statistics_reset(&stats_accum);
+            } else if (is_f32) {
+                f32_to_stats(&stats_accum, f32_summary->data[src_offset], incr);
+            } else {
+                f64_to_stats(&stats_accum, f64_summary->data[src_offset], incr);
             }
+            incr_remaining = increment - incr;
         } else {
             if (is_f32) {
                 f32_to_stats(&stats_next, f32_summary->data[src_offset], step_size);
             } else {
                 f64_to_stats(&stats_next, f64_summary->data[src_offset], step_size);
             }
             jls_statistics_combine(&stats_accum, &stats_accum, &stats_next);
```

### Comparing `pyjls-0.6.3/src/statistics.c` & `pyjls-0.7.0/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/threaded_writer.c` & `pyjls-0.7.0/src/threaded_writer.c`

 * *Files 16% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 #include "jls/cdef.h"
 #include "jls/ec.h"
 #include "jls/log.h"
 #include "jls/time.h"
 #include "jls/writer.h"
 #include <stdlib.h>
 #include <string.h>
+#include <inttypes.h>
 
 
-#define MRB_BUFFER_SIZE (100000000)
+#define MRB_BUFFER_SIZE (64 * 1024 * 1024)
 
 
 struct jls_twr_s {
     struct jls_bkt_s * bk;  // REQUIRED first entry
     struct jls_wr_s * wr;
     volatile int quit;
     volatile uint64_t flush_send_id;
@@ -94,40 +95,48 @@
         "user_data",
         "fsr",
         "annotation",
         "utc",
 };
 
 int32_t jls_twr_run(struct jls_twr_s * self) {
-    uint32_t msg_size;
-    uint8_t * msg;
+    uint32_t msg_size = 0;
+    uint8_t * msg = NULL;
     struct msg_header_s hdr;
     uint8_t * payload;
     int32_t rc = 0;
+    struct jls_time_counter_s counter_start = jls_time_counter();
+    struct jls_time_counter_s counter_end;
+    struct jls_time_counter_s counter_prev = counter_start;
+    uint64_t duration_ms;
 
-    if (!self->bk) {
-        JLS_LOGE("backend null on entry");
-    }
-
+    JLS_LOGI("run start");
     while (!self->quit) {
-        if (!self->bk) {
-            JLS_LOGE("backend null");
-            jls_bkt_sleep_ms(500);
+        if (NULL == self->bk) {
+            JLS_LOGE("backend null, quit");  // should never happen
+            self->quit = true;
             continue;
         }
         jls_bkt_msg_wait(self->bk);
-        if (jls_bkt_msg_lock(self->bk)) {
-            continue;
-        }
-        while (!self->quit) {
+        while (1) {
+            jls_bkt_msg_lock(self->bk);
+            if (NULL != msg) {
+                jls_mrb_pop(&self->mrb, &msg_size);
+            }
             msg = jls_mrb_peek(&self->mrb, &msg_size);
             jls_bkt_msg_unlock(self->bk);
             if (!msg) {
                 break;
             }
+            counter_start = jls_time_counter();
+            if (((counter_start.value - counter_prev.value) / counter_start.frequency) >= 1) {
+                JLS_LOGD2("twr %" PRIu32 " msgs (%" PRIu32 " of %" PRIu32 " bytes)",
+                          self->mrb.count, jls_mrb_used_bytes(&self->mrb), self->mrb.buf_size);
+                counter_prev = counter_start;
+            }
             payload = msg + sizeof(hdr);
             uint32_t payload_sz = msg_size - sizeof(hdr);
 
             memcpy(&hdr, msg, sizeof(hdr));
             rc = 0;
 
             jls_bkt_process_lock(self->bk);
@@ -156,39 +165,42 @@
                     break;
                 case MSG_UTC:
                     rc = jls_wr_utc(self->wr, hdr.h.utc.signal_id, hdr.h.utc.sample_id, hdr.h.utc.utc);
                 default:
                     break;
             }
             jls_bkt_process_unlock(self->bk);
+            counter_end = jls_time_counter();
+            duration_ms = (1000 * (counter_end.value - counter_start.value)) / counter_end.frequency;
+            if (duration_ms > 250) {
+                JLS_LOGW("thread msg %d:%s took %" PRIu64 " ms",
+                         (int) hdr.msg_type,
+                         (hdr.msg_type < MSG_ITEM_COUNT) ? message_str[hdr.msg_type] : "unknown",
+                         duration_ms);
+            }
 
             if (rc) {
                 JLS_LOGW("thread msg %d:%s returned %d:%s",
                          (int) hdr.msg_type,
                          (hdr.msg_type < MSG_ITEM_COUNT) ? message_str[hdr.msg_type] : "unknown",
                          (int) rc, jls_error_code_name(rc));
             }
-
-            while (!self->quit && jls_bkt_msg_lock(self->bk)) {
-                // retry
-            }
-            jls_mrb_pop(&self->mrb, &msg_size);
-            // stay locked
         }
     }
+    JLS_LOGI("run done");
     return 0;
 }
 
 int32_t jls_twr_open(struct jls_twr_s ** instance, const char * path) {
     struct jls_wr_s * wr;
     struct jls_twr_s * self;
     ROE(jls_wr_open(&wr, path));
 
     self = malloc(sizeof(struct jls_twr_s) + MRB_BUFFER_SIZE);
-    if (!self) {
+    if (NULL == self) {
         JLS_LOGE("jls_twr_open malloc failed");
         jls_wr_close(wr);
         return JLS_ERROR_NOT_ENOUGH_MEMORY;
     }
     self->quit = 0;
     self->wr = wr;
     self->flush_send_id = 0;
@@ -245,25 +257,28 @@
             return JLS_ERROR_TIMED_OUT;
         }
     }
     return 0;
 }
 
 int32_t jls_twr_close(struct jls_twr_s * self) {
-    int rc = 0;
     if (self) {
+        JLS_LOGI("jls_twr_close start");
         struct msg_header_s hdr = { .msg_type = MSG_CLOSE };
-        jls_twr_flush(self);
         msg_send(self, &hdr, NULL, 0);
         jls_bkt_finalize(self->bk);
-        rc = jls_wr_close(self->wr);
+        JLS_LOGI("jls_bkt_finalize done");
+        // jls_wr_flush(self->wr);  // takes too long & blocks UI
+        // JLS_LOGI("jls_wr_flush done");
+        jls_wr_close(self->wr);
         self->wr = NULL;
         free(self);
+        JLS_LOGI("jls_wr_close done");
     }
-    return rc;
+    return 0;
 }
 
 int32_t jls_twr_source_def(struct jls_twr_s * self, const struct jls_source_def_s * source) {
     jls_bkt_process_lock(self->bk);
     int32_t rv = jls_wr_source_def(self->wr, source);
     jls_bkt_process_unlock(self->bk);
     return rv;
```

### Comparing `pyjls-0.6.3/src/wr_fsr.c` & `pyjls-0.7.0/src/wr_fsr.c`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
     uint8_t * p_end = (uint8_t *) dst->summary->data[dst->summary->header.entry_count];
     uint32_t payload_len = (uint32_t) (p_end - p_start);
     ROE(jls_wr_summary_prv(self->wr, self->def.signal_id, JLS_TRACK_TYPE_FSR, level, p_start, payload_len));
     ROE(summaryN(self, level + 1, pos_next));
 
     // compute new timestamp for that level
     int64_t skip = dst->summary_entries * self->def.sample_decimate_factor;
-    if (level > 1) {
+    for (uint8_t lvl = 2; lvl <= level; ++lvl) {
         skip *= self->def.summary_decimate_factor;
     }
     dst->index->header.timestamp += skip;
     dst->index->header.entry_count = 0;
     dst->summary->header.timestamp += skip;
     dst->summary->header.entry_count = 0;
     return 0;
@@ -337,23 +337,30 @@
     }
 
     *instance = self;
     return 0;
 }
 
 int32_t jls_wr_fsr_close(struct jls_wr_fsr_s * self) {
+    int32_t rc;
     if (self) {
         if (self->data) {
-            wr_data(self);  // write remaining sample data
+            rc = wr_data(self);  // write remaining sample data
+            if (rc) {
+                JLS_LOGE("wr_data returned %" PRIi32, rc);
+            }
             JLS_LOGD1("%d sample_buffer free %p", (int) self->def.signal_id, (void *) self->data);
             sample_buffer_free(self);
         }
 
         for (size_t i = 1; i < JLS_SUMMARY_LEVEL_COUNT; ++i) {
-            summary_close(self, (uint8_t) i);
+            rc = summary_close(self, (uint8_t) i);
+            if (rc) {
+                JLS_LOGE("summary_close(%d) returned %" PRIi32, (int) i, rc);
+            }
         }
         free(self);
     }
     return 0;
 }
 
 static void summary_entry_add(struct jls_wr_fsr_s * self, uint8_t level,
```

### Comparing `pyjls-0.6.3/src/wr_ts.c` & `pyjls-0.7.0/src/wr_ts.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.6.3/src/writer.c` & `pyjls-0.7.0/src/writer.c`

 * *Files identical despite different names*

