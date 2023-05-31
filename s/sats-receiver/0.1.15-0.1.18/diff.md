# Comparing `tmp/sats_receiver-0.1.15.tar.gz` & `tmp/sats_receiver-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sats_receiver-0.1.15.tar", last modified: Tue May 30 17:44:29 2023, max compression
+gzip compressed data, was "sats_receiver-0.1.18.tar", last modified: Wed May 31 17:15:35 2023, max compression
```

## Comparing `sats_receiver-0.1.15.tar` & `sats_receiver-0.1.18.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/sats_receiver/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/async_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/sats_receiver/gr_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/gr_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/gr_modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/gr_modules/demodulators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/sats_receiver/gr_modules/epb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/gr_modules/epb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/gr_modules/epb/sstv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/gr_modules/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/gr_modules/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/librtlsdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/observer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/sats_receiver/systems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/systems/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/systems/sstv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/tle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/sats_receiver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/sats_receiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-30 17:44:29.000000 sats_receiver-0.1.15/sats_receiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-30 17:44:29.000000 sats_receiver-0.1.15/sats_receiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:44:29.000000 sats_receiver-0.1.15/sats_receiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 17:44:29.000000 sats_receiver-0.1.15/sats_receiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 17:44:29.000000 sats_receiver-0.1.15/sats_receiver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:29.636129 sats_receiver-0.1.15/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/tests/test_async_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-30 17:44:15.000000 sats_receiver-0.1.15/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.366345 sats_receiver-0.1.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-31 17:15:35.366345 sats_receiver-0.1.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/async_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver/gr_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/demodulators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver/gr_modules/epb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/epb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/epb/prober.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/epb/sstv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/gr_modules/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/librtlsdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/observer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/systems/apt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/systems/sstv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/tle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/sats_receiver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/sats_receiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 17:15:35.000000 sats_receiver-0.1.18/sats_receiver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:15:35.366345 sats_receiver-0.1.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:35.362345 sats_receiver-0.1.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/tests/test_async_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-31 17:15:23.000000 sats_receiver-0.1.18/tests/test_utils.py
```

### Comparing `sats_receiver-0.1.15/LICENSE` & `sats_receiver-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/PKG-INFO` & `sats_receiver-0.1.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sats_receiver
-Version: 0.1.15
+Version: 0.1.18
 Summary: Satellites data receiver based on GNU Radio
 Home-page: https://github.com/baskiton/sats-receiver
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sats_receiver-0.1.15/README.md` & `sats_receiver-0.1.18/README.md`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/__main__.py` & `sats_receiver-0.1.18/sats_receiver/__main__.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/async_signal.py` & `sats_receiver-0.1.18/sats_receiver/async_signal.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/gr_modules/decoders.py` & `sats_receiver-0.1.18/sats_receiver/gr_modules/decoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,15 @@
 class SstvDecoder(Decoder):
     _FREQ_1 = (1900 - 1200) / 2
 
     def __init__(self,
                  sat_name: str,
                  samp_rate: Union[int, float],
                  out_dir: pathlib.Path,
-                 observer: Observer,
+                 observer: Observer = None,
                  do_sync=True,
                  wsr=16000):
         super(SstvDecoder, self).__init__('SSTV Decoder', sat_name, samp_rate, out_dir)
 
         self.observer = observer
         self.do_sync = do_sync
         self.wsr = wsr
@@ -349,16 +349,16 @@
                 2500,       # high_cutoff_freq
                 200,        # transition_width
                 gr.fft.window.WIN_HAMMING,
                 6.76))
         self.frs = gr.blocks.rotator_cc(2 * math.pi * -(1900 - self._FREQ_1) / samp_rate)
         self.quad_demod = gr.analog.quadrature_demod_cf((samp_rate / (2 * math.pi * self._FREQ_1)))
         self.rsp = gr.filter.rational_resampler_fcc(
-                interpolation=samp_rate // resamp_gcd,
-                decimation=wsr // resamp_gcd,
+                interpolation=wsr // resamp_gcd,
+                decimation=samp_rate // resamp_gcd,
                 taps=[],
                 fractional_bw=0
         )
         self.correllator = gr.digital.corr_est_cc(hdr, hdr_pix_width, 1, 0.4, gr.digital.THRESHOLD_ABSOLUTE)
         self.ctf_out = gr.blocks.complex_to_float()
         self.out_add_const = gr.blocks.add_const_ff(450 / self._FREQ_1)
         self.out_multiply_const = gr.blocks.multiply_const_ff(self._FREQ_1 / (750 + 450))
@@ -381,15 +381,18 @@
         self.connect(
             (self.correllator, 1),
             self.ctf_corr,
             self.corr_peak_detector,
             (self.sstv_epb, self.sstv_epb.PEAKS_IN),
         )
 
-        latlonalt = str(observer.lat), str(observer.lon), observer.elev
+        if observer is None:
+            latlonalt = None
+        else:
+            latlonalt = str(observer.lat), str(observer.lon), observer.elev
         self.base_kw.update(observer_latlonalt=latlonalt)
 
     def start(self):
         # super(SstvDecoder, self).start()
         utils.unlink(self.tmp_file)
 
     def finalize(self, executor, fin_key: str):
@@ -397,30 +400,33 @@
         sstv_rr: list[sstv.SstvRecognizer] = self.sstv_epb.finalize()
         executor.execute(self._sstv_finalize, **self.base_kw, sstv_rr=sstv_rr, fin_key=fin_key)
 
     @staticmethod
     def _sstv_finalize(log: logging.Logger,
                        sat_name: str,
                        out_dir: pathlib.Path,
-                       observer_latlonalt: tuple[str, str, Union[int, float]],
+                       observer_latlonalt: Optional[tuple[str, str, Union[int, float]]],
                        sstv_rr: list[sstv.SstvRecognizer],
                        fin_key: str) -> tuple[str, str, list[tuple[pathlib.Path, dt.datetime]]]:
         log.debug('finalizing...')
 
-        observer = ephem.Observer()
-        observer.lat, observer.lon, observer.elev = observer_latlonalt
+        if observer_latlonalt:
+            observer = ephem.Observer()
+            observer.lat, observer.lon, observer.elev = observer_latlonalt
+
         fn_dt = []
         sz_sum = 0
         for i in sstv_rr:
             img = i.get_image()
             if not img:
                 continue
 
-            log.debug('add GPSInfo EXIF')
-            img = utils.img_add_exif(img, observer=observer)
+            if observer_latlonalt:
+                log.debug('add GPSInfo EXIF')
+                img = utils.img_add_exif(img, observer=observer)
             exif = img.getexif()
 
             sstv_mode = exif.get_ifd(ExifTags.IFD.Exif).get(ExifTags.Base.UserComment, 'SSTV')
             end_time = exif.get(ExifTags.Base.DateTime)
             end_time = (dt.datetime.strptime(end_time, '%Y:%m:%d %H:%M:%S')
                         if end_time
                         else dt.datetime.utcnow())
```

### Comparing `sats_receiver-0.1.15/sats_receiver/gr_modules/demodulators.py` & `sats_receiver-0.1.18/sats_receiver/gr_modules/demodulators.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/gr_modules/epb/sstv.py` & `sats_receiver-0.1.18/sats_receiver/gr_modules/epb/sstv.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/gr_modules/modules.py` & `sats_receiver-0.1.18/sats_receiver/gr_modules/modules.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/gr_modules/receiver.py` & `sats_receiver-0.1.18/sats_receiver/gr_modules/receiver.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/librtlsdr.py` & `sats_receiver-0.1.18/sats_receiver/librtlsdr.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/manager.py` & `sats_receiver-0.1.18/sats_receiver/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sats_receiver.observer import Observer
 from sats_receiver.tle import Tle
 from sats_receiver.utils import Scheduler, SysUsage
 
 
 class Executor(mp.Process):
     def __init__(self, q: mp.Queue = None, sysu_intv=SysUsage.DEFAULT_INTV):
-        super().__init__(daemon=False, name=self.__class__.__name__)
+        super().__init__(daemon=True, name=self.__class__.__name__)
 
         self.q = q
         self.sysu_intv = sysu_intv
         self.rd, self.wr = mp.Pipe(False)
 
     def _setup_process(self):
         logger = logging.getLogger()
```

### Comparing `sats_receiver-0.1.15/sats_receiver/observer.py` & `sats_receiver-0.1.18/sats_receiver/observer.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/systems/apt.py` & `sats_receiver-0.1.18/sats_receiver/systems/apt.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/systems/sstv.py` & `sats_receiver-0.1.18/sats_receiver/systems/sstv.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,15 @@
                                      srate=self.srate,
                                      do_sync=self.do_sync)
                     self.state = self._STATE_GET_LINE
                     res = self.STATUS_FOUND
 
             elif self.state == self._STATE_GET_LINE:
                 if self.sstv.feed(data):
-                    self.state = self._STATE_0
+                    self.stop()
                     return self.STATUS_DONE
                 break
 
         return res
 
     def get_image(self) -> Optional[Image.Image]:
         if self.sstv:
```

### Comparing `sats_receiver-0.1.15/sats_receiver/tle.py` & `sats_receiver-0.1.18/sats_receiver/tle.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/sats_receiver/utils.py` & `sats_receiver-0.1.18/sats_receiver/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,20 +299,24 @@
     return math.atan2(
         math.sin(delta_lon),
         math.cos(lat_a) * math.tan(lat_b) - math.sin(lat_a) * math.cos(delta_lon)
     )
 
 
 def mktmp(dir: pathlib.Path = None, prefix: str = None, suffix='.tmp') -> pathlib.Path:
+    if dir:
+        dir.mkdir(parents=True, exist_ok=True)
     f = tempfile.NamedTemporaryFile(dir=dir, prefix=prefix, suffix=suffix, delete=False)
     f.close()
     return pathlib.Path(f.name)
 
 
 def mktmp2(mode='w+b', buffering=-1, dir: pathlib.Path = None, prefix: str = None, suffix='.tmp'):
+    if dir:
+        dir.mkdir(parents=True, exist_ok=True)
     return tempfile.NamedTemporaryFile(mode=mode,
                                        buffering=buffering,
                                        dir=dir,
                                        prefix=prefix,
                                        suffix=suffix,
                                        delete=False)
```

### Comparing `sats_receiver-0.1.15/sats_receiver.egg-info/PKG-INFO` & `sats_receiver-0.1.18/sats_receiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sats-receiver
-Version: 0.1.15
+Version: 0.1.18
 Summary: Satellites data receiver based on GNU Radio
 Home-page: https://github.com/baskiton/sats-receiver
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sats_receiver-0.1.15/sats_receiver.egg-info/SOURCES.txt` & `sats_receiver-0.1.18/sats_receiver.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 sats_receiver.egg-info/top_level.txt
 sats_receiver/gr_modules/__init__.py
 sats_receiver/gr_modules/decoders.py
 sats_receiver/gr_modules/demodulators.py
 sats_receiver/gr_modules/modules.py
 sats_receiver/gr_modules/receiver.py
 sats_receiver/gr_modules/epb/__init__.py
+sats_receiver/gr_modules/epb/prober.py
 sats_receiver/gr_modules/epb/sstv.py
 sats_receiver/systems/__init__.py
 sats_receiver/systems/apt.py
 sats_receiver/systems/sstv.py
 tests/__init__.py
 tests/test_async_signal.py
 tests/test_decoders.py
```

### Comparing `sats_receiver-0.1.15/setup.py` & `sats_receiver-0.1.18/setup.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/tests/test_async_signal.py` & `sats_receiver-0.1.18/tests/test_async_signal.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.15/tests/test_decoders.py` & `sats_receiver-0.1.18/tests/test_decoders.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import gnuradio.gr
 import numpy as np
 
 from PIL import Image, ExifTags
 from sats_receiver import utils
 from sats_receiver.manager import Executor
 from sats_receiver.gr_modules.decoders import Decoder, SstvDecoder
+from sats_receiver.gr_modules.epb.prober import Prober
 from sats_receiver.observer import Observer
 
 
 HERE = pathlib.Path(__file__).parent
 FILES = HERE / 'files'
 TIMEOUT = support.SHORT_TIMEOUT
 
@@ -83,32 +84,34 @@
                  decoder: Decoder):
         self.prefix = self.__class__.__name__
         self.log = logging.getLogger(self.prefix)
 
         super(DecoderTopBlock, self).__init__('DecoderTopBlock', catch_exceptions=False)
 
         self.executor = DecoderExecutor(ret_wr)
-        self.executor.start()
-        atexit.register(lambda x: (x.stop(), x.join()), self.executor)
 
         self.blocks_wavfile_source = gr.blocks.wavfile_source(str(wav_fp), False)
+        self.prober = Prober()
         self.blocks_float_to_complex = gr.blocks.float_to_complex(1)
         self.decoder = decoder
 
-        ##################################################
-        # Connections
-        ##################################################
         self.connect(
             self.blocks_wavfile_source,
             self.blocks_float_to_complex,
             self.decoder,
         )
+        self.connect(
+            self.blocks_wavfile_source,
+            self.prober,
+        )
 
     def start(self, max_noutput_items=10000000):
         self.log.info('START')
+        self.executor.start()
+        atexit.register(lambda x: (x.stop(), x.join()), self.executor)
         self.decoder.start()
         super(DecoderTopBlock, self).start(max_noutput_items)
 
     def stop(self):
         self.log.info('STOP')
         super(DecoderTopBlock, self).stop()
 
@@ -162,15 +165,18 @@
                                'elevation': alt,
                                'weather': False}),
             do_sync=1,
             wsr=sstv_wsr,
         )
         self.tb = DecoderTopBlock(wav_fp, self.ret_wr, decoder)
         self.tb.start()
-        time.sleep(TIMEOUT)
+
+        while self.tb.prober.changes():
+            time.sleep(self.tb.prober.measure_s)
+
         self.tb.stop()
         self.tb.wait()
 
         x = self.ret_rd.poll(TIMEOUT)
         self.assertTrue(x)
 
         x = self.ret_rd.recv()
```

### Comparing `sats_receiver-0.1.15/tests/test_utils.py` & `sats_receiver-0.1.18/tests/test_utils.py`

 * *Files identical despite different names*

