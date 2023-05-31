# Comparing `tmp/async_adbc-1.0.8.tar.gz` & `tmp/async_adbc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_adbc-1.0.8.tar", max compression
+gzip compressed data, was "async_adbc-1.0.9.tar", max compression
```

## Comparing `async_adbc-1.0.8.tar` & `async_adbc-1.0.9.tar`

### file list

```diff
@@ -1,51 +1,119 @@
--rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.8/async_adbc/__init__.py
--rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.8/async_adbc/adbclient.py
--rw-r--r--   0        0        0     3746 2023-05-22 09:52:07.908716 async_adbc-1.0.8/async_adbc/device.py
--rw-r--r--   0        0        0      187 2023-05-22 01:24:42.225886 async_adbc-1.0.8/async_adbc/exceptions.py
--rw-r--r--   0        0        0      663 2023-05-22 09:51:54.864677 async_adbc-1.0.8/async_adbc/plugins/__init__.py
--rw-r--r--   0        0        0      411 2023-05-18 08:06:58.438375 async_adbc-1.0.8/async_adbc/plugins/am.py
--rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.8/async_adbc/plugins/battery.py
--rw-r--r--   0        0        0    11610 2023-05-22 01:25:37.176656 async_adbc-1.0.8/async_adbc/plugins/cpu.py
--rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.8/async_adbc/plugins/forward.py
--rw-r--r--   0        0        0     3974 2023-05-22 01:24:42.228877 async_adbc-1.0.8/async_adbc/plugins/fps.py
--rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.8/async_adbc/plugins/gpu.py
--rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.8/async_adbc/plugins/input.py
--rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.8/async_adbc/plugins/logcat.py
--rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.8/async_adbc/plugins/mem.py
--rw-r--r--   0        0        0     1988 2023-05-22 10:18:29.986438 async_adbc-1.0.8/async_adbc/plugins/minicap.py
--rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.8/async_adbc/plugins/pm.py
--rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.8/async_adbc/plugins/prop.py
--rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.8/async_adbc/plugins/temp.py
--rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.8/async_adbc/plugins/traffic.py
--rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.8/async_adbc/plugins/utils.py
--rw-r--r--   0        0        0      686 2023-05-22 10:06:35.912810 async_adbc-1.0.8/async_adbc/plugins/wm.py
--rw-r--r--   0        0        0     4481 2023-05-16 07:19:17.701385 async_adbc-1.0.8/async_adbc/protocol.py
--rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.8/async_adbc/service/__init__.py
--rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.8/async_adbc/service/host.py
--rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.8/async_adbc/service/local.py
--rw-r--r--   0        0        0   722896 2023-05-22 08:50:56.899996 async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minicap
--rw-r--r--   0        0        0   722896 2023-05-22 08:50:56.904875 async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minicap-nopie
--rw-r--r--   0        0        0    38464 2023-05-22 08:50:56.906827 async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minitouch
--rw-r--r--   0        0        0    38464 2023-05-22 08:50:56.906827 async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minitouch-nopie
--rw-r--r--   0        0        0    34060 2023-05-22 08:50:56.925390 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi/minitouch
--rw-r--r--   0        0        0    29964 2023-05-22 08:50:56.926347 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi/minitouch-nopie
--rw-r--r--   0        0        0   562792 2023-05-22 08:50:56.913660 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minicap
--rw-r--r--   0        0        0   550504 2023-05-22 08:50:56.919515 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minicap-nopie
--rw-r--r--   0        0        0    29972 2023-05-22 08:50:56.922442 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minitouch
--rw-r--r--   0        0        0    29972 2023-05-22 08:50:56.923419 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minitouch-nopie
--rw-r--r--   0        0        0    71328 2023-05-22 08:50:57.009974 async_adbc-1.0.8/async_adbc/vendor/minicap/mips/minitouch
--rw-r--r--   0        0        0    71280 2023-05-22 08:50:57.012902 async_adbc-1.0.8/async_adbc/vendor/minicap/mips/minitouch-nopie
--rw-r--r--   0        0        0    59992 2023-05-22 08:50:57.014854 async_adbc-1.0.8/async_adbc/vendor/minicap/mips64/minitouch
--rw-r--r--   0        0        0    59992 2023-05-22 08:50:57.015829 async_adbc-1.0.8/async_adbc/vendor/minicap/mips64/minitouch-nopie
--rw-r--r--   0        0        0   992920 2023-05-22 08:50:57.025589 async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minicap
--rw-r--r--   0        0        0   976536 2023-05-22 08:50:57.034373 async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minicap-nopie
--rw-r--r--   0        0        0    38108 2023-05-22 08:50:57.035349 async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minitouch
--rw-r--r--   0        0        0    38108 2023-05-22 08:50:57.036325 async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minitouch-nopie
--rw-r--r--   0        0        0   915840 2023-05-22 08:50:57.047007 async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minicap
--rw-r--r--   0        0        0   915840 2023-05-22 08:50:57.051886 async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minicap-nopie
--rw-r--r--   0        0        0    38728 2023-05-22 08:50:57.053838 async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minitouch
--rw-r--r--   0        0        0    38728 2023-05-22 08:50:57.054814 async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minitouch-nopie
--rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.8/LICENSE
--rw-r--r--   0        0        0      482 2023-05-22 10:19:11.577795 async_adbc-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.8/README.md
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.9/async_adbc/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.9/async_adbc/adbclient.py
+-rw-r--r--   0        0        0     3746 2023-05-22 09:52:07.908716 async_adbc-1.0.9/async_adbc/device.py
+-rw-r--r--   0        0        0      187 2023-05-22 01:24:42.225886 async_adbc-1.0.9/async_adbc/exceptions.py
+-rw-r--r--   0        0        0      663 2023-05-22 09:51:54.864677 async_adbc-1.0.9/async_adbc/plugins/__init__.py
+-rw-r--r--   0        0        0      411 2023-05-18 08:06:58.438375 async_adbc-1.0.9/async_adbc/plugins/am.py
+-rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.9/async_adbc/plugins/battery.py
+-rw-r--r--   0        0        0    11610 2023-05-22 01:25:37.176656 async_adbc-1.0.9/async_adbc/plugins/cpu.py
+-rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.9/async_adbc/plugins/forward.py
+-rw-r--r--   0        0        0     3974 2023-05-22 01:24:42.228877 async_adbc-1.0.9/async_adbc/plugins/fps.py
+-rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.9/async_adbc/plugins/gpu.py
+-rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.9/async_adbc/plugins/input.py
+-rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.9/async_adbc/plugins/logcat.py
+-rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.9/async_adbc/plugins/mem.py
+-rw-r--r--   0        0        0     2320 2023-05-22 10:33:09.322882 async_adbc-1.0.9/async_adbc/plugins/minicap.py
+-rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.9/async_adbc/plugins/pm.py
+-rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.9/async_adbc/plugins/prop.py
+-rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.9/async_adbc/plugins/temp.py
+-rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.9/async_adbc/plugins/traffic.py
+-rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.9/async_adbc/plugins/utils.py
+-rw-r--r--   0        0        0      686 2023-05-22 10:06:35.912810 async_adbc-1.0.9/async_adbc/plugins/wm.py
+-rw-r--r--   0        0        0     4481 2023-05-16 07:19:17.701385 async_adbc-1.0.9/async_adbc/protocol.py
+-rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.9/async_adbc/service/__init__.py
+-rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.9/async_adbc/service/host.py
+-rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.9/async_adbc/service/local.py
+-rw-r--r--   0        0        0   722896 2023-05-22 08:50:56.899996 async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minicap
+-rw-r--r--   0        0        0   722896 2023-05-22 08:50:56.904875 async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minicap-nopie
+-rw-r--r--   0        0        0     5440 2023-05-22 08:50:56.905851 async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    38464 2023-05-22 08:50:56.906827 async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minitouch
+-rw-r--r--   0        0        0    38464 2023-05-22 08:50:56.906827 async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minitouch-nopie
+-rw-r--r--   0        0        0    34060 2023-05-22 08:50:56.925390 async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi/minitouch
+-rw-r--r--   0        0        0    29964 2023-05-22 08:50:56.926347 async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi/minitouch-nopie
+-rw-r--r--   0        0        0   562792 2023-05-22 08:50:56.913660 async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minicap
+-rw-r--r--   0        0        0   550504 2023-05-22 08:50:56.919515 async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minicap-nopie
+-rw-r--r--   0        0        0   226604 2023-05-22 08:50:56.921467 async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    29972 2023-05-22 08:50:56.922442 async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minitouch
+-rw-r--r--   0        0        0    29972 2023-05-22 08:50:56.923419 async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minitouch-nopie
+-rw-r--r--   0        0        0     9688 2023-05-22 08:50:56.928299 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-10/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0     5700 2023-05-22 08:50:56.929275 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-14/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    11385 2023-05-22 08:50:56.930251 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-14/x86/minicap.so
+-rw-r--r--   0        0        0     5700 2023-05-22 08:50:56.932203 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-15/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    11385 2023-05-22 08:50:56.933179 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-15/x86/minicap.so
+-rw-r--r--   0        0        0     9420 2023-05-22 08:50:56.934155 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-16/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    11929 2023-05-22 08:50:56.935131 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-16/x86/minicap.so
+-rw-r--r--   0        0        0    13472 2023-05-22 08:50:56.937083 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-17/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    23907 2023-05-22 08:50:56.938058 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-17/x86/minicap.so
+-rw-r--r--   0        0        0    13492 2023-05-22 08:50:56.939035 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-18/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    23491 2023-05-22 08:50:56.940010 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-18/x86/minicap.so
+-rw-r--r--   0        0        0    13488 2023-05-22 08:50:56.942939 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-19/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    23725 2023-05-22 08:50:56.944892 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-19/x86/minicap.so
+-rw-r--r--   0        0        0    22000 2023-05-22 08:50:56.945867 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-21/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    13492 2023-05-22 08:50:56.946842 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-21/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    21676 2023-05-22 08:50:56.947819 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-21/x86/minicap.so
+-rw-r--r--   0        0        0    26328 2023-05-22 08:50:56.949771 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-21/x86_64/minicap.so
+-rw-r--r--   0        0        0    22000 2023-05-22 08:50:56.950746 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-22/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    13492 2023-05-22 08:50:56.951723 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-22/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    21676 2023-05-22 08:50:56.952698 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-22/x86/minicap.so
+-rw-r--r--   0        0        0    26328 2023-05-22 08:50:56.953675 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-22/x86_64/minicap.so
+-rw-r--r--   0        0        0    22328 2023-05-22 08:50:56.955627 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-23/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    22128 2023-05-22 08:50:56.956603 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-23/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    21932 2023-05-22 08:50:56.957579 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-23/x86/minicap.so
+-rw-r--r--   0        0        0    26688 2023-05-22 08:50:56.958554 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-23/x86_64/minicap.so
+-rw-r--r--   0        0        0    22576 2023-05-22 08:50:56.960507 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-24/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    22100 2023-05-22 08:50:56.961483 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-24/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    21944 2023-05-22 08:50:56.963060 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-24/x86/minicap.so
+-rw-r--r--   0        0        0    26672 2023-05-22 08:50:56.964031 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-24/x86_64/minicap.so
+-rw-r--r--   0        0        0    22576 2023-05-22 08:50:56.965006 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-25/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    22100 2023-05-22 08:50:56.966959 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-25/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    21944 2023-05-22 08:50:56.967935 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-25/x86/minicap.so
+-rw-r--r--   0        0        0    26672 2023-05-22 08:50:56.968911 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-25/x86_64/minicap.so
+-rw-r--r--   0        0        0    23592 2023-05-22 08:50:56.970863 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-26/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    24760 2023-05-22 08:50:56.971838 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-26/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    22588 2023-05-22 08:50:56.972814 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-26/x86/minicap.so
+-rw-r--r--   0        0        0    27280 2023-05-22 08:50:56.973791 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-26/x86_64/minicap.so
+-rw-r--r--   0        0        0    23592 2023-05-22 08:50:56.975742 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-27/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    24784 2023-05-22 08:50:56.977457 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-27/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    22564 2023-05-22 08:50:56.977694 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-27/x86/minicap.so
+-rw-r--r--   0        0        0    27280 2023-05-22 08:50:56.978670 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-27/x86_64/minicap.so
+-rw-r--r--   0        0        0    68736 2023-05-22 08:50:56.980707 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-28/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    28900 2023-05-22 08:50:56.981669 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-28/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    23032 2023-05-22 08:50:56.982645 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-28/x86/minicap.so
+-rw-r--r--   0        0        0    27776 2023-05-22 08:50:56.984597 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-28/x86_64/minicap.so
+-rw-r--r--   0        0        0    29088 2023-05-22 08:50:56.985573 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-29/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    28888 2023-05-22 08:50:56.986550 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-29/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    31868 2023-05-22 08:50:56.987526 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-29/x86/minicap.so
+-rw-r--r--   0        0        0    37272 2023-05-22 08:50:56.989478 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-29/x86_64/minicap.so
+-rw-r--r--   0        0        0    25136 2023-05-22 08:50:56.990454 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-30/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    21360 2023-05-22 08:50:56.991430 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-30/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    21272 2023-05-22 08:50:56.993382 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-30/x86/minicap.so
+-rw-r--r--   0        0        0    23448 2023-05-22 08:50:56.994358 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-30/x86_64/minicap.so
+-rw-r--r--   0        0        0    24488 2023-05-22 08:50:56.996310 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-31/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    20956 2023-05-22 08:50:56.997286 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-31/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    20532 2023-05-22 08:50:56.998262 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-31/x86/minicap.so
+-rw-r--r--   0        0        0    20136 2023-05-22 08:50:56.999238 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-31/x86_64/minicap.so
+-rw-r--r--   0        0        0    24488 2023-05-22 08:50:57.000214 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-32/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    20956 2023-05-22 08:50:57.001189 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-32/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    20532 2023-05-22 08:50:57.003142 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-32/x86/minicap.so
+-rw-r--r--   0        0        0    20136 2023-05-22 08:50:57.004118 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-32/x86_64/minicap.so
+-rw-r--r--   0        0        0    24728 2023-05-22 08:50:57.005094 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-33/arm64-v8a/minicap.so
+-rw-r--r--   0        0        0    21968 2023-05-22 08:50:57.006069 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-33/x86_64/minicap.so
+-rw-r--r--   0        0        0     9688 2023-05-22 08:50:57.008022 async_adbc-1.0.9/async_adbc/vendor/minicap/minicap-shared/aosp/libs/android-9/armeabi-v7a/minicap.so
+-rw-r--r--   0        0        0    71328 2023-05-22 08:50:57.009974 async_adbc-1.0.9/async_adbc/vendor/minicap/mips/minitouch
+-rw-r--r--   0        0        0    71280 2023-05-22 08:50:57.012902 async_adbc-1.0.9/async_adbc/vendor/minicap/mips/minitouch-nopie
+-rw-r--r--   0        0        0    59992 2023-05-22 08:50:57.014854 async_adbc-1.0.9/async_adbc/vendor/minicap/mips64/minitouch
+-rw-r--r--   0        0        0    59992 2023-05-22 08:50:57.015829 async_adbc-1.0.9/async_adbc/vendor/minicap/mips64/minitouch-nopie
+-rw-r--r--   0        0        0   992920 2023-05-22 08:50:57.025589 async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minicap
+-rw-r--r--   0        0        0   976536 2023-05-22 08:50:57.034373 async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minicap-nopie
+-rw-r--r--   0        0        0     5116 2023-05-22 08:50:57.034373 async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minicap.so
+-rw-r--r--   0        0        0    38108 2023-05-22 08:50:57.035349 async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minitouch
+-rw-r--r--   0        0        0    38108 2023-05-22 08:50:57.036325 async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minitouch-nopie
+-rw-r--r--   0        0        0   915840 2023-05-22 08:50:57.047007 async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minicap
+-rw-r--r--   0        0        0   915840 2023-05-22 08:50:57.051886 async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minicap-nopie
+-rw-r--r--   0        0        0     5632 2023-05-22 08:50:57.052862 async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minicap.so
+-rw-r--r--   0        0        0    38728 2023-05-22 08:50:57.053838 async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minitouch
+-rw-r--r--   0        0        0    38728 2023-05-22 08:50:57.054814 async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minitouch-nopie
+-rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.9/LICENSE
+-rw-r--r--   0        0        0      482 2023-05-22 10:33:44.995292 async_adbc-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.9/README.md
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.9/PKG-INFO
```

### Comparing `async_adbc-1.0.8/async_adbc/adbclient.py` & `async_adbc-1.0.9/async_adbc/adbclient.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/device.py` & `async_adbc-1.0.9/async_adbc/device.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/__init__.py` & `async_adbc-1.0.9/async_adbc/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/battery.py` & `async_adbc-1.0.9/async_adbc/plugins/battery.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/cpu.py` & `async_adbc-1.0.9/async_adbc/plugins/cpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/forward.py` & `async_adbc-1.0.9/async_adbc/plugins/forward.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/fps.py` & `async_adbc-1.0.9/async_adbc/plugins/fps.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/gpu.py` & `async_adbc-1.0.9/async_adbc/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/logcat.py` & `async_adbc-1.0.9/async_adbc/plugins/logcat.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/mem.py` & `async_adbc-1.0.9/async_adbc/plugins/mem.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/minicap.py` & `async_adbc-1.0.9/async_adbc/plugins/minicap.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
     async def init(self):
         """
         初始化minicap
         """
 
         exists = await self._device.file_exists("/data/local/tmp/minicap")
+        exists = exists and await self._device.file_exists(
+            "/data/local/temp/minicap.so"
+        )
         if exists:
             return
 
         props = await self._device.properties
         abi = props.get("ro.product.cpu.abi")
         pre_sdk = props.get("ro.build.version.preview_sdk")
         rel_sdk = props.get("ro.build.version.release")
@@ -44,21 +47,27 @@
                 MINICAP_LIBS,
                 f"minicap-shared/aosp/libs/android-{rel_sdk}/{abi}/minicap.so",
             )
 
         await self._device.push(sofile_path, self.PUSH_TO + "/minicap.so", chmode=0o755)
 
     async def get_frame(self):
-        self.init()
+        await self.init()
 
         resolution = await self._device.wm.size()
         size = resolution.override_size
         orientation = await self._device.wm.orientation()
         raw_data = await self._device.shell_raw(
             "LD_LIBRARY_PATH=/data/local/tmp /data/local/tmp/minicap",
             "-P",
             f"{size}@{size}/{orientation}",
             "-s",
         )
 
+        if b"CANNOT LINK EXECUTABLE" in raw_data:
+            raise RuntimeError(raw_data.decode())
+
+        if b"inaccessible or not found" in raw_data:
+            raise RuntimeError(raw_data.decode())
+
         jpg_data = raw_data.split(b"for JPG encoder\n")[-1]
         return jpg_data
```

### Comparing `async_adbc-1.0.8/async_adbc/plugins/pm.py` & `async_adbc-1.0.9/async_adbc/plugins/pm.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/temp.py` & `async_adbc-1.0.9/async_adbc/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/traffic.py` & `async_adbc-1.0.9/async_adbc/plugins/traffic.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/utils.py` & `async_adbc-1.0.9/async_adbc/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/plugins/wm.py` & `async_adbc-1.0.9/async_adbc/plugins/wm.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/protocol.py` & `async_adbc-1.0.9/async_adbc/protocol.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/service/__init__.py` & `async_adbc-1.0.9/async_adbc/service/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/service/host.py` & `async_adbc-1.0.9/async_adbc/service/host.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/service/local.py` & `async_adbc-1.0.9/async_adbc/service/local.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minicap` & `async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minicap`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minicap-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minicap-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minitouch` & `async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minitouch`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minitouch-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/arm64-v8a/minitouch-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi/minitouch` & `async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi/minitouch`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi/minitouch-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi/minitouch-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minicap` & `async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minicap`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minicap-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minicap-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minitouch` & `async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minitouch`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minitouch-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/armeabi-v7a/minitouch-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/mips/minitouch` & `async_adbc-1.0.9/async_adbc/vendor/minicap/mips/minitouch`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/mips/minitouch-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/mips/minitouch-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/mips64/minitouch` & `async_adbc-1.0.9/async_adbc/vendor/minicap/mips64/minitouch`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/mips64/minitouch-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/mips64/minitouch-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minicap` & `async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minicap`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minicap-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minicap-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minitouch` & `async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minitouch`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minitouch-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/x86/minitouch-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minicap` & `async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minicap`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minicap-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minicap-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minitouch` & `async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minitouch`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minitouch-nopie` & `async_adbc-1.0.9/async_adbc/vendor/minicap/x86_64/minitouch-nopie`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/LICENSE` & `async_adbc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.8/PKG-INFO` & `async_adbc-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-adbc
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: kaluluosi
 Author-email: kaluluosi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

