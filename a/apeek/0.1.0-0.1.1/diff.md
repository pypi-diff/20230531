# Comparing `tmp/apeek-0.1.0.tar.gz` & `tmp/apeek-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apeek-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "apeek-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apeek-0.1.0.tar` & `apeek-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2653 2023-05-20 03:19:21.967235 apeek-0.1.0/README.md
--rw-r--r--   0        0        0     1325 2023-05-20 03:19:21.967235 apeek-0.1.0/apeek/__init__.py
--rw-r--r--   0        0        0     2423 2023-05-20 03:19:21.967235 apeek-0.1.0/apeek/__main__.py
--rw-r--r--   0        0        0     2246 2023-05-20 03:19:21.967235 apeek-0.1.0/apeek/waveform.py
--rw-r--r--   0        0        0     1635 2023-05-20 03:19:21.967235 apeek-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3570 1970-01-01 00:00:00.000000 apeek-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2654 2023-05-31 00:31:07.986267 apeek-0.1.1/README.md
+-rw-r--r--   0        0        0     1347 2023-05-31 00:31:07.986267 apeek-0.1.1/apeek/__init__.py
+-rw-r--r--   0        0        0     2412 2023-05-31 00:31:07.986267 apeek-0.1.1/apeek/__main__.py
+-rw-r--r--   0        0        0     2867 2023-05-31 00:31:07.986267 apeek-0.1.1/apeek/waveform.py
+-rw-r--r--   0        0        0     1635 2023-05-31 00:31:07.986267 apeek-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3571 1970-01-01 00:00:00.000000 apeek-0.1.1/PKG-INFO
```

### Comparing `apeek-0.1.0/README.md` & `apeek-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,7 +21,8 @@
           █████████████████████████████████████▄██ ██ ▆▆ ▄                                           
          ▇████████████████████████████████████████ ██ ██ █▄                                          
         ▁█████████████████████████████████████████▇██▅██▅██ ▆▃ ▁                                     
                            max ↑                                                                     
 DUR: 0.60 seconds @ 22050Fs // Peak: -2.39 dBFS at 0.31 secs                                         
 ```
 ![Screenshot](docs/apeek.png)
+
```

### Comparing `apeek-0.1.0/apeek/__init__.py` & `apeek-0.1.1/apeek/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
 apeek is a package for creating audio waveform previews.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 from typing import List
 
 import numpy as np
 
-from .waveform import WaveformData, WaveformDataSettings, ScalingFactor
+from .waveform import WaveformData, WaveformDataSettings, ScalingFactor, default_settings
 
-def rectified_unicode_waveform_charmatrix(data: np.array, height: int, bg: str = "·") -> List[List[str]]:
+def rectified_unicode_waveform_charmatrix(data: np.ndarray, height: int, bg: str = "·") -> List[List[str]]:
     """ 
     Create a grid of strs for a rectified waveform bargraph
     """
     BLOCK_CHARS = list(f"{bg}▁▂▃▄▅▆▇")
     FULL_BLOCK = "█"
     levels = height * (len(BLOCK_CHARS))
 
     retval = []
 
-    for i, sample_pair in enumerate(data):
+    for _, sample_pair in enumerate(data):
         rectified_value = max(abs(sample_pair[0]), abs(sample_pair[1]))
         leveled_value = int(rectified_value * levels)
         
         full, partial = divmod(leveled_value, len(BLOCK_CHARS))
         blank = height - full
 
         retval += [list( FULL_BLOCK * full + BLOCK_CHARS[partial] + BLOCK_CHARS[0] * blank)]
 
     return retval
 
 
-def unicode_waveform(data: np.array, height: int) -> str:
+def unicode_waveform(data: np.ndarray, height: int) -> str:
     
     char_matrix = rectified_unicode_waveform_charmatrix(data, height)
     
     # transpose
     retval_lines = list()
     for j in reversed(range(height)):
         this_line = ""
```

### Comparing `apeek-0.1.0/apeek/__main__.py` & `apeek-0.1.1/apeek/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 apeek main
 """
 
 import pydub
 import apeek
-from apeek import WaveformData, WaveformDataSettings, ScalingFactor
+from apeek import WaveformData, ScalingFactor, default_settings
 
 import sys
 import shutil
 import math
 import optparse
 
 def main():
@@ -31,27 +31,27 @@
     parser.add_option("-a","--absolute", help="Do not normalize waveform",
                       default=False, action='store_true')
 
     (options, args) = parser.parse_args()
 
     for file in args:
         audio = pydub.AudioSegment.from_file(file)
-        settings = WaveformDataSettings.default()
+        settings = default_settings()
 
         if options.scaling == "linear":
             settings['scaling'] = ScalingFactor.LINEAR
         else:
             settings['scaling'] = ScalingFactor.ROOT
         
         settings['normalized'] = True
 
         if options.absolute:
             settings['normalized'] = False
 
-        result = WaveformData.create_waveform_data(audio, time_bins=options.width, settings=settings)
+        result = WaveformData.create_waveform_data(audio, time_bin_count=options.width, settings=settings)
         text = apeek.unicode_waveform(result.value_pairs, height=options.height)
 
         if len(args) > 1:
             print(file + ":")
 
         sys.stdout.write(text)
         sys.stdout.write("\n")
```

### Comparing `apeek-0.1.0/apeek/waveform.py` & `apeek-0.1.1/apeek/waveform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,95 @@
 import numpy as np
 from pydub import AudioSegment
 
-from math import sqrt
 from enum import Enum
 from dataclasses import dataclass
-from typing import Tuple, TypedDict
+from typing import TypedDict, Optional, cast
 
 
 class ScalingFactor(Enum):
     LINEAR = 0
     ROOT = 1
 
 
 class WaveformDataSettings(TypedDict):
     scaling: 'ScalingFactor'
     normalized: bool
+    
 
-    @classmethod
-    def default(cls):
-        return cls(scaling=ScalingFactor.ROOT, normalized=True)
+def default_settings():
+    return WaveformDataSettings(scaling=ScalingFactor.ROOT, normalized=True)
 
 
 @dataclass
 class WaveformData:
     """
     Data collected from an AudioSegment to be used for drawing a waveform.
     """
-    value_pairs: np.array
+    value_pairs: np.ndarray 
     max_index: int
     max_sample: int
     max_value: float
     full_code_value: float
+    samples_per_bin: int
 
     @classmethod
     def create_waveform_data(cls,
                              audio: AudioSegment, 
-                             time_bins: int, 
-                             settings: WaveformDataSettings = WaveformDataSettings.default()) -> 'WaveformData':
+                             time_bin_count: Optional[int],
+                             bin_length: Optional[int] = None,
+                             settings: WaveformDataSettings = default_settings()) -> 'WaveformData':
         """
         Create a numpy array for use in drawing a waveform overview.
      
         """
+
         samples = audio.get_array_of_samples()
-        bit_depth = audio.sample_width
-        window_length = int(len(samples) / time_bins)
+        channel_count = audio.channels
+        assert isinstance(channel_count,int)
+        
+        frame_count = len(samples) // channel_count
+
+        if time_bin_count is not None:
+            window_length = (frame_count // time_bin_count) * channel_count
+        elif bin_length is not None:
+            window_length = bin_length
+            time_bin_count = (frame_count // bin_length) * channel_count
+        else:
+            assert False
 
-        retval = np.zeros((time_bins, 2))
+        retval = np.zeros((time_bin_count, 2))
         
         max_index = 0
         max_value = 0.0
         max_sample = 0
-        for i in range(time_bins):
+        for i in range(time_bin_count):
             window = samples[i * window_length : (i + 1) * window_length]
             retval[i] = (np.max(window),np.min(window))
             magnitude = np.max(np.abs(window))
             if magnitude > max_value:
                 max_index = i
-                max_sample = np.argmax(np.abs(window)) + i * window_length
+                max_sample = cast(int, np.argmax(np.abs(window)) + i * window_length)
                 max_value = magnitude
-        
+
+
+        bit_depth = audio.sample_width
+        assert isinstance(bit_depth,int) 
         full_code_value = (2 ** (bit_depth * 8 - 1)) 
         retval = retval / full_code_value
 
         if settings['normalized']:
             sample_max = np.max(retval)
             sample_min = np.min(retval)
             scale_max = max(abs(sample_max), abs(sample_min))
-            retval = retval / scale_max
+            if scale_max != 0:
+                retval = retval / scale_max
 
         if settings['scaling'] == ScalingFactor.ROOT:
             signs = np.sign(retval)
             absval = np.sqrt(np.fabs(retval))
-            retval = retval * signs
+            retval = absval * signs
 
-        return cls(retval, max_index, max_sample, max_value, full_code_value)
+        return cls(retval, max_index, max_sample, 
+                   max_value, full_code_value, samples_per_bin=window_length)
```

### Comparing `apeek-0.1.0/pyproject.toml` & `apeek-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apeek-0.1.0/PKG-INFO` & `apeek-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeek
-Version: 0.1.0
+Version: 0.1.1
 Summary: apeek is a package for creating audio waveform previews.
 Keywords: waveform,metadata,audio,console
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia
@@ -45,7 +45,8 @@
          ▇████████████████████████████████████████ ██ ██ █▄                                          
         ▁█████████████████████████████████████████▇██▅██▅██ ▆▃ ▁                                     
                            max ↑                                                                     
 DUR: 0.60 seconds @ 22050Fs // Peak: -2.39 dBFS at 0.31 secs                                         
 ```
 ![Screenshot](docs/apeek.png)
 
+
```

