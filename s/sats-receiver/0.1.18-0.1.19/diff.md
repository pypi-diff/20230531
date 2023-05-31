# Comparing `tmp/sats_receiver-0.1.18.tar.gz` & `tmp/sats_receiver-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sats_receiver-0.1.18.tar", last modified: Wed May 31 17:15:35 2023, max compression
+gzip compressed data, was "sats_receiver-0.1.19.tar", last modified: Wed May 31 20:26:30 2023, max compression
```

## Comparing `sats_receiver-0.1.18.tar` & `sats_receiver-0.1.19.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.366345 sats_receiver-0.1.18/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-31 17:15:35.366345 sats_receiver-0.1.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/async_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver/gr_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/demodulators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver/gr_modules/epb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/epb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/epb/prober.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/epb/sstv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/librtlsdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/observer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver/systems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/systems/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/systems/sstv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/tle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:15:35.366345 sats_receiver-0.1.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/tests/test_async_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/async_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver/gr_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/demodulators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver/gr_modules/epb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/epb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/epb/prober.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/epb/sstv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/librtlsdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/observer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/systems/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/systems/sstv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/tle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/tests/test_async_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/tests/test_utils.py
```

### Comparing `sats_receiver-0.1.18/LICENSE` & `sats_receiver-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/PKG-INFO` & `sats_receiver-0.1.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sats_receiver
-Version: 0.1.18
+Version: 0.1.19
 Summary: Satellites data receiver based on GNU Radio
 Home-page: https://github.com/baskiton/sats-receiver
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sats_receiver-0.1.18/README.md` & `sats_receiver-0.1.19/README.md`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/__main__.py` & `sats_receiver-0.1.19/sats_receiver/__main__.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/async_signal.py` & `sats_receiver-0.1.19/sats_receiver/async_signal.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/gr_modules/decoders.py` & `sats_receiver-0.1.19/sats_receiver/gr_modules/decoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
             exif = img.getexif()
 
             sstv_mode = exif.get_ifd(ExifTags.IFD.Exif).get(ExifTags.Base.UserComment, 'SSTV')
             end_time = exif.get(ExifTags.Base.DateTime)
             end_time = (dt.datetime.strptime(end_time, '%Y:%m:%d %H:%M:%S')
                         if end_time
                         else dt.datetime.utcnow())
-            res_fn = out_dir / end_time.strftime(f'{sat_name}_{sstv_mode}_%Y-%m-%d_%H-%M-%S,%f.png')
+            res_fn = out_dir / end_time.strftime(f'{sat_name}_{sstv_mode}_%Y-%m-%d_%H-%M-%S,%f_{fin_key}.png')
 
             img.save(res_fn, exif=exif)
 
             fn_dt.append((res_fn, end_time))
             sz = res_fn.stat().st_size
             sz_sum += sz
             log.info('finish: %s (%s)', res_fn, utils.numbi_disp(sz))
```

### Comparing `sats_receiver-0.1.18/sats_receiver/gr_modules/demodulators.py` & `sats_receiver-0.1.19/sats_receiver/gr_modules/demodulators.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/gr_modules/epb/prober.py` & `sats_receiver-0.1.19/sats_receiver/gr_modules/epb/prober.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/gr_modules/epb/sstv.py` & `sats_receiver-0.1.19/sats_receiver/gr_modules/epb/sstv.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/gr_modules/modules.py` & `sats_receiver-0.1.19/sats_receiver/gr_modules/modules.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/gr_modules/receiver.py` & `sats_receiver-0.1.19/sats_receiver/gr_modules/receiver.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/librtlsdr.py` & `sats_receiver-0.1.19/sats_receiver/librtlsdr.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/manager.py` & `sats_receiver-0.1.19/sats_receiver/manager.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/observer.py` & `sats_receiver-0.1.19/sats_receiver/observer.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/systems/apt.py` & `sats_receiver-0.1.19/sats_receiver/systems/apt.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/systems/sstv.py` & `sats_receiver-0.1.19/sats_receiver/systems/sstv.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/tle.py` & `sats_receiver-0.1.19/sats_receiver/tle.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver/utils.py` & `sats_receiver-0.1.19/sats_receiver/utils.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/sats_receiver.egg-info/PKG-INFO` & `sats_receiver-0.1.19/sats_receiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sats-receiver
-Version: 0.1.18
+Version: 0.1.19
 Summary: Satellites data receiver based on GNU Radio
 Home-page: https://github.com/baskiton/sats-receiver
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sats_receiver-0.1.18/sats_receiver.egg-info/SOURCES.txt` & `sats_receiver-0.1.19/sats_receiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/setup.py` & `sats_receiver-0.1.19/setup.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/tests/test_async_signal.py` & `sats_receiver-0.1.19/tests/test_async_signal.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/tests/test_decoders.py` & `sats_receiver-0.1.19/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.18/tests/test_utils.py` & `sats_receiver-0.1.19/tests/test_utils.py`

 * *Files identical despite different names*

