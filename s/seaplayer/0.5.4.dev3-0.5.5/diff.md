# Comparing `tmp/seaplayer-0.5.4.dev3.tar.gz` & `tmp/seaplayer-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplayer-0.5.4.dev3.tar", max compression
+gzip compressed data, was "seaplayer-0.5.5.tar", max compression
```

## Comparing `seaplayer-0.5.4.dev3.tar` & `seaplayer-0.5.5.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.4.dev3/LICENSE
--rw-r--r--   0        0        0     1652 2023-05-27 17:07:14.285094 seaplayer-0.5.4.dev3/pyproject.toml
--rw-r--r--   0        0        0     1336 2023-05-23 03:20:59.345209 seaplayer-0.5.4.dev3/README.md
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev3/seaplayer/__init__.py
--rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev3/seaplayer/__main__.py
--rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.4.dev3/seaplayer/assets/image-not-found.png
--rw-r--r--   0        0        0      264 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev3/seaplayer/codecs/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev3/seaplayer/codecs/Any.py
--rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev3/seaplayer/codecs/FLAC.py
--rw-r--r--   0        0        0     2946 2023-05-25 07:17:50.819139 seaplayer-0.5.4.dev3/seaplayer/codecs/MIDI.py
--rw-r--r--   0        0        0      473 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev3/seaplayer/codecs/MP3.py
--rw-r--r--   0        0        0      475 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev3/seaplayer/codecs/OGG.py
--rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.4.dev3/seaplayer/codecs/WAV.py
--rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev3/seaplayer/codeсbase.py
--rw-r--r--   0        0        0     6188 2023-05-27 18:01:34.042639 seaplayer-0.5.4.dev3/seaplayer/config.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.4.dev3/seaplayer/css/configurate.css
--rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev3/seaplayer/css/objects.css
--rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev3/seaplayer/css/seaplayer.css
--rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev3/seaplayer/css/unknown.css
--rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.4.dev3/seaplayer/exceptions.py
--rw-r--r--   0        0        0     1413 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev3/seaplayer/functions.py
--rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.4.dev3/seaplayer/modules/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-27 17:36:06.594476 seaplayer-0.5.4.dev3/seaplayer/modules/colorizer.py
--rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev3/seaplayer/objects/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.4.dev3/seaplayer/objects/Configurate.py
--rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.4.dev3/seaplayer/objects/DataOptions.py
--rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev3/seaplayer/objects/Image.py
--rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.4.dev3/seaplayer/objects/Input.py
--rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.4.dev3/seaplayer/objects/Log.py
--rw-r--r--   0        0        0     5701 2023-05-27 17:49:37.836036 seaplayer-0.5.4.dev3/seaplayer/objects/MusicList.py
--rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev3/seaplayer/objects/Notification.py
--rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev3/seaplayer/objects/ProgressBar.py
--rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.4.dev3/seaplayer/plug/__init__.py
--rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.4.dev3/seaplayer/plug/__main__.py
--rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.4.dev3/seaplayer/plug/cli/__init__.py
--rw-r--r--   0        0        0     5259 2023-05-27 12:11:55.197047 seaplayer-0.5.4.dev3/seaplayer/plug/cli/cli.py
--rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.4.dev3/seaplayer/plug/cli/exceptions.py
--rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.4.dev3/seaplayer/plug/cli/functions.py
--rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.4.dev3/seaplayer/plug/cli/vars.py
--rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.4.dev3/seaplayer/plug/pluginbase.py
--rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.4.dev3/seaplayer/plug/pluginbase.pyi
--rw-r--r--   0        0        0     8688 2023-05-26 22:50:40.897429 seaplayer-0.5.4.dev3/seaplayer/plug/pluginloader.py
--rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.4.dev3/seaplayer/plug/pluginloader.pyi
--rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev3/seaplayer/screens/__init__.py
--rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.4.dev3/seaplayer/screens/Configurate.py
--rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.4.dev3/seaplayer/screens/Unknown.py
--rw-r--r--   0        0        0    20323 2023-05-27 19:52:25.382634 seaplayer-0.5.4.dev3/seaplayer/seaplayer.py
--rw-r--r--   0        0        0       91 2023-05-27 09:37:18.022755 seaplayer-0.5.4.dev3/seaplayer/types/__init__.py
--rw-r--r--   0        0        0     1576 2023-05-27 12:03:27.045912 seaplayer-0.5.4.dev3/seaplayer/types/Cache.py
--rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev3/seaplayer/types/Convert.py
--rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.4.dev3/seaplayer/types/MusicList.py
--rw-r--r--   0        0        0     1525 2023-05-27 17:07:22.141538 seaplayer-0.5.4.dev3/seaplayer/units.py
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 seaplayer-0.5.4.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-23 03:20:59.344210 seaplayer-0.5.5/LICENSE
+-rw-r--r--   0        0        0     1692 2023-05-31 18:38:23.622208 seaplayer-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1324 2023-05-28 16:32:50.014284 seaplayer-0.5.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.348294 seaplayer-0.5.5/seaplayer/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-23 03:20:59.348294 seaplayer-0.5.5/seaplayer/__main__.py
+-rw-r--r--   0        0        0    14705 2023-05-23 03:20:59.348294 seaplayer-0.5.5/seaplayer/assets/image-not-found.png
+-rw-r--r--   0        0        0      316 2023-05-30 22:43:00.213825 seaplayer-0.5.5/seaplayer/codecs/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-30 20:24:25.780892 seaplayer-0.5.5/seaplayer/codecs/Any.py
+-rw-r--r--   0        0        0     2916 2023-05-31 18:29:02.746094 seaplayer-0.5.5/seaplayer/codecs/AnySound.py
+-rw-r--r--   0        0        0      477 2023-05-23 03:20:59.349294 seaplayer-0.5.5/seaplayer/codecs/FLAC.py
+-rw-r--r--   0        0        0     1160 2023-05-30 22:41:35.103481 seaplayer-0.5.5/seaplayer/codecs/MIDI.py
+-rw-r--r--   0        0        0      487 2023-05-29 15:31:51.602929 seaplayer-0.5.5/seaplayer/codecs/MP3.py
+-rw-r--r--   0        0        0      475 2023-05-30 22:33:59.986095 seaplayer-0.5.5/seaplayer/codecs/OGG.py
+-rw-r--r--   0        0        0     2388 2023-05-31 18:35:21.569274 seaplayer-0.5.5/seaplayer/codecs/URLS.py
+-rw-r--r--   0        0        0      593 2023-05-23 03:20:59.349294 seaplayer-0.5.5/seaplayer/codecs/WAV.py
+-rw-r--r--   0        0        0     1924 2023-05-23 03:20:59.350294 seaplayer-0.5.5/seaplayer/codeсbase.py
+-rw-r--r--   0        0        0     6188 2023-05-27 18:01:34.042639 seaplayer-0.5.5/seaplayer/config.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.350294 seaplayer-0.5.5/seaplayer/css/configurate.css
+-rw-r--r--   0        0        0     1585 2023-05-23 03:20:59.351294 seaplayer-0.5.5/seaplayer/css/objects.css
+-rw-r--r--   0        0        0      595 2023-05-23 03:20:59.351294 seaplayer-0.5.5/seaplayer/css/seaplayer.css
+-rw-r--r--   0        0        0      278 2023-05-23 03:20:59.351294 seaplayer-0.5.5/seaplayer/css/unknown.css
+-rw-r--r--   0        0        0      382 2023-05-23 03:20:59.351294 seaplayer-0.5.5/seaplayer/exceptions.py
+-rw-r--r--   0        0        0     1460 2023-05-31 18:26:10.280817 seaplayer-0.5.5/seaplayer/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:20:59.353307 seaplayer-0.5.5/seaplayer/modules/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-27 17:36:06.594476 seaplayer-0.5.5/seaplayer/modules/colorizer.py
+-rw-r--r--   0        0        0      376 2023-05-25 17:39:02.081110 seaplayer-0.5.5/seaplayer/objects/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 07:17:50.820137 seaplayer-0.5.5/seaplayer/objects/Configurate.py
+-rw-r--r--   0        0        0     1421 2023-05-25 17:39:02.081110 seaplayer-0.5.5/seaplayer/objects/DataOptions.py
+-rw-r--r--   0        0        0     3006 2023-05-23 03:20:59.354294 seaplayer-0.5.5/seaplayer/objects/Image.py
+-rw-r--r--   0        0        0     1126 2023-05-23 03:20:59.354294 seaplayer-0.5.5/seaplayer/objects/Input.py
+-rw-r--r--   0        0        0     1287 2023-05-26 21:36:55.785380 seaplayer-0.5.5/seaplayer/objects/Log.py
+-rw-r--r--   0        0        0     5701 2023-05-27 17:49:37.836036 seaplayer-0.5.5/seaplayer/objects/MusicList.py
+-rw-r--r--   0        0        0      787 2023-05-23 03:20:59.355309 seaplayer-0.5.5/seaplayer/objects/Notification.py
+-rw-r--r--   0        0        0     1269 2023-05-23 03:20:59.355309 seaplayer-0.5.5/seaplayer/objects/ProgressBar.py
+-rw-r--r--   0        0        0       86 2023-05-23 03:20:59.355309 seaplayer-0.5.5/seaplayer/plug/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-26 18:16:55.016730 seaplayer-0.5.5/seaplayer/plug/__main__.py
+-rw-r--r--   0        0        0       21 2023-05-26 19:51:28.701684 seaplayer-0.5.5/seaplayer/plug/cli/__init__.py
+-rw-r--r--   0        0        0     5259 2023-05-27 12:11:55.197047 seaplayer-0.5.5/seaplayer/plug/cli/cli.py
+-rw-r--r--   0        0        0      582 2023-05-26 20:10:17.518991 seaplayer-0.5.5/seaplayer/plug/cli/exceptions.py
+-rw-r--r--   0        0        0     1937 2023-05-26 18:16:55.018728 seaplayer-0.5.5/seaplayer/plug/cli/functions.py
+-rw-r--r--   0        0        0      133 2023-05-26 19:55:28.316980 seaplayer-0.5.5/seaplayer/plug/cli/vars.py
+-rw-r--r--   0        0        0      817 2023-05-26 22:40:27.692911 seaplayer-0.5.5/seaplayer/plug/pluginbase.py
+-rw-r--r--   0        0        0      759 2023-05-26 18:16:55.019724 seaplayer-0.5.5/seaplayer/plug/pluginbase.pyi
+-rw-r--r--   0        0        0     8688 2023-05-28 16:09:52.376773 seaplayer-0.5.5/seaplayer/plug/pluginloader.py
+-rw-r--r--   0        0        0     2692 2023-05-26 18:16:55.020726 seaplayer-0.5.5/seaplayer/plug/pluginloader.pyi
+-rw-r--r--   0        0        0       84 2023-05-23 03:20:59.356797 seaplayer-0.5.5/seaplayer/screens/__init__.py
+-rw-r--r--   0        0        0     8542 2023-05-25 17:39:02.083097 seaplayer-0.5.5/seaplayer/screens/Configurate.py
+-rw-r--r--   0        0        0     1002 2023-05-23 03:20:59.356797 seaplayer-0.5.5/seaplayer/screens/Unknown.py
+-rw-r--r--   0        0        0    21058 2023-05-31 18:44:14.903020 seaplayer-0.5.5/seaplayer/seaplayer.py
+-rw-r--r--   0        0        0       91 2023-05-27 09:37:18.022755 seaplayer-0.5.5/seaplayer/types/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-27 12:03:27.045912 seaplayer-0.5.5/seaplayer/types/Cache.py
+-rw-r--r--   0        0        0     2624 2023-05-23 03:20:59.357805 seaplayer-0.5.5/seaplayer/types/Convert.py
+-rw-r--r--   0        0        0     1589 2023-05-23 03:20:59.357805 seaplayer-0.5.5/seaplayer/types/MusicList.py
+-rw-r--r--   0        0        0     1520 2023-05-31 18:44:23.825849 seaplayer-0.5.5/seaplayer/units.py
+-rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 seaplayer-0.5.5/PKG-INFO
```

### Comparing `seaplayer-0.5.4.dev3/LICENSE` & `seaplayer-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/pyproject.toml` & `seaplayer-0.5.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SeaPlayer"
-version = "0.5.4.dev3"
+version = "0.5.5"
 description = "SeaPlayer is a player that works in the terminal."
 repository = "https://github.com/romanin-rf/SeaPlayer"
 authors = ["Romanin <semina054@gmail.com>"]
 keywords = ["tui", "player", "seaplayer", "wav", "mp3", "ogg", "midi"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
@@ -42,14 +42,16 @@
 typing-inspect = "^0.8.0"
 ripix = ">=2.2.3"
 platformdirs = "^3.5.1"
 pydantic = "^1.10.7"
 click = "^8.1.3"
 poetry = {version = "^1.5.0", optional = true}
 pyinstaller = {version = "^5.11.0", optional = true}
+validators = "^0.20.0"
+urlopen2 = "^1.1.0"
 
 
 [tool.poetry.extras]
 build = ["poetry", "pyinstaller"]
 
 
 [build-system]
```

### Comparing `seaplayer-0.5.4.dev3/README.md` & `seaplayer-0.5.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -23,10 +23,9 @@
 
 You need to [install the FluidSynth](https://github.com/FluidSynth/fluidsynth/wiki/Download) package in order to playback `MIDI`.
 
 ## Using
 ```shell
 python -m seaplayer # Method for `downloaded repository` or `installed via pip`
 ```
-
-![MainScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/e4b2ee2c-9061-47ff-8818-a480b3a79a5e)
-![ConfigurateScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/ad84eafb-2324-4036-81c3-81df9138025a)
+![MainScreen-v0.5.4](https://github.com/romanin-rf/SeaPlayer/assets/60302782/5be6c2cb-5602-4c85-a3be-ae36a90e71e4)
+![ConfigurateScreen-v0.5.4](https://github.com/romanin-rf/SeaPlayer/assets/60302782/922c7112-2259-47d1-9619-488855e14c2c)
```

### Comparing `seaplayer-0.5.4.dev3/seaplayer/assets/image-not-found.png` & `seaplayer-0.5.5/seaplayer/assets/image-not-found.png`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/codecs/Any.py` & `seaplayer-0.5.5/seaplayer/codecs/Any.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import hashlib
 import aiofiles
 # > Sound Works
-from playsoundsimple import Sound
+from .AnySound import AnySound
 # > Typing
 from typing import Optional
 # > Local Imports
 from ..codeсbase import CodecBase
 
 
 class AnyCodec(CodecBase):
     codec_name: str = "Any"
     
     # ! Initialized
     def __init__(self, path: str, sound_device_id: Optional[int]=None, **kwargs) -> None:
         self.name = os.path.abspath(path)
-        self._sound = Sound(self.name, device_id=sound_device_id)
+        self._sound = AnySound(self.name, device_id=sound_device_id)
     
     def __sha1__(self, buffer_size: int) -> str:
         sha1 = hashlib.sha1()
         with open(self.name, "rb") as file:
             while True:
                 data = file.read(buffer_size)
                 if not data: break
```

### Comparing `seaplayer-0.5.4.dev3/seaplayer/codecs/MIDI.py` & `seaplayer-0.5.5/seaplayer/codecs/AnySound.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import asyncio
 import aiofiles
 import subprocess
 from tempfile import mkstemp
+# > IO's
+from urlopen2 import URLFile
 # > Sound Works
 from playsoundsimple import Sound
 from playsoundsimple.units import SOUND_FONTS_PATH, FLUID_SYNTH_PATH
 from playsoundsimple.exceptions import FileTypeError
 from playsoundsimple.player import SoundFP, get_sound_filepath
-# > Typing Import
+# > Typing
 from typing import Optional
-# > Local Imports
-from .Any import AnyCodec
 
-
-# ! Codec Types
-class MIDISound(Sound):
+# ! Main Class
+class AnySound(Sound):
+    @staticmethod
     async def aio_from_midi(
         fp: SoundFP,
         sound_fonts_path: Optional[str]=None,
         **kwargs
     ):
         path, is_temp = get_sound_filepath(fp, filetype=".midi")
         sound_fonts_path = sound_fonts_path or SOUND_FONTS_PATH
@@ -32,16 +32,17 @@
         )
         await process.wait()
         
         if is_temp:
             try: os.remove(path)
             except: pass
         
-        return Sound(npath, **{"is_temp": True, **kwargs})
+        return AnySound(npath, **{"is_temp": True, **kwargs})
     
+    @staticmethod
     def from_midi(
         fp: SoundFP,
         sound_fonts_path: Optional[str]=None,
         **kwargs
     ):
         path, is_temp = get_sound_filepath(fp, filetype=".midi")
         sound_fonts_path = sound_fonts_path or SOUND_FONTS_PATH
@@ -53,35 +54,38 @@
             stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
         )
         
         if is_temp:
             try: os.remove(path)
             except: pass
         
-        return Sound(npath, **{"is_temp": True, **kwargs})
-
-# ! Codec
-class MIDICodec(AnyCodec):
-    codec_name: str = "MIDI"
+        return AnySound(npath, **{"is_temp": True, **kwargs})
     
-    # ! Testing
     @staticmethod
-    def is_this_codec(path: str) -> bool:
-        with open(path, 'rb') as file:
-            return file.read(4) == b"MThd"
-    
-    @staticmethod
-    async def aio_is_this_codec(path: str) -> bool:
-        async with aiofiles.open(path, 'rb') as file:
-            return await file.read(4) == b"MThd"
-    
-    # ! Initialized
-    def __init__(self, path: str, aio_init: bool=False, sound_device_id: Optional[int]=None, **kwargs) -> None:
-        self.name = os.path.abspath(path)
-        if not aio_init:
-            self._sound = MIDISound.from_midi(self.name, device_id=sound_device_id, **kwargs)
+    def from_url(
+        url: str,
+        download_buffer_size: int=65536,
+        **kwargs
+    ):
+        path = mkstemp(suffix=".bin")[1]
+        
+        with URLFile(url) as urlfile:
+            with open(path, "wb") as tempfile:
+                while len(data:=urlfile.read(download_buffer_size)) != 0:
+                    tempfile.write(data)
+        
+        return AnySound(path, **{"is_temp": True, **kwargs})
     
     @staticmethod
-    async def __aio_init__(path: str, sound_device_id: Optional[int]=None, **kwargs):
-        self = MIDICodec(path, aio_init=True)
-        self._sound = await MIDISound.aio_from_midi(self.name, device_id=sound_device_id, **kwargs)
-        return self
+    async def aio_from_url(
+        url: str,
+        download_buffer_size: int=65536,
+        **kwargs
+    ):
+        path = mkstemp(suffix=".bin")[1]
+        
+        with URLFile(url) as urlfile:
+            async with aiofiles.open(path, "wb") as tempfile:
+                while len(data:=urlfile.read(download_buffer_size)) != 0:
+                    await tempfile.write(data)
+        
+        return AnySound(path, **{"is_temp": True, **kwargs})
```

### Comparing `seaplayer-0.5.4.dev3/seaplayer/codecs/WAV.py` & `seaplayer-0.5.5/seaplayer/codecs/WAV.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/codeсbase.py` & `seaplayer-0.5.5/seaplayer/codeсbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/config.py` & `seaplayer-0.5.5/seaplayer/config.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/css/objects.css` & `seaplayer-0.5.5/seaplayer/css/objects.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/css/seaplayer.css` & `seaplayer-0.5.5/seaplayer/css/seaplayer.css`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/functions.py` & `seaplayer-0.5.5/seaplayer/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import asyncio
 import aiofiles
 from io import BytesIO
 # > Image Works
 from PIL import Image
 # > Typing
-from typing import Literal, Tuple, Optional, Iterable, TypeVar
+from typing import Literal, Tuple, Optional, Iterable, TypeVar, AsyncGenerator, Any
 # > Local Imports
 from .codeсbase import CodecBase
 
 # ! Types
 T = TypeVar("T")
 
 # ! Async Functions
-async def aiter(it: Iterable[T]):
+async def aiter(it: Iterable[T]) -> AsyncGenerator[T, Any]:
     for i in it:
         await asyncio.sleep(0)
         yield i
 
 async def get_bar_status() -> Tuple[str, Optional[float], Optional[float]]: return "", None, None
 
 async def aio_is_midi_file(filepath: str):
```

### Comparing `seaplayer-0.5.4.dev3/seaplayer/modules/colorizer.py` & `seaplayer-0.5.5/seaplayer/modules/colorizer.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/objects/Configurate.py` & `seaplayer-0.5.5/seaplayer/objects/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/objects/DataOptions.py` & `seaplayer-0.5.5/seaplayer/objects/DataOptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/objects/Image.py` & `seaplayer-0.5.5/seaplayer/objects/Image.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/objects/Input.py` & `seaplayer-0.5.5/seaplayer/objects/Input.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/objects/Log.py` & `seaplayer-0.5.5/seaplayer/objects/Log.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/objects/MusicList.py` & `seaplayer-0.5.5/seaplayer/objects/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/objects/Notification.py` & `seaplayer-0.5.5/seaplayer/objects/Notification.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/objects/ProgressBar.py` & `seaplayer-0.5.5/seaplayer/objects/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/plug/cli/cli.py` & `seaplayer-0.5.5/seaplayer/plug/cli/cli.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/plug/cli/exceptions.py` & `seaplayer-0.5.5/seaplayer/plug/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/plug/cli/functions.py` & `seaplayer-0.5.5/seaplayer/plug/cli/functions.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/plug/pluginbase.py` & `seaplayer-0.5.5/seaplayer/plug/pluginbase.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/plug/pluginbase.pyi` & `seaplayer-0.5.5/seaplayer/plug/pluginbase.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/plug/pluginloader.py` & `seaplayer-0.5.5/seaplayer/plug/pluginloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def enable_plugin_by_name_id(self, name_id: str) -> None:
         self.config.plugins_enable[name_id] = True
         self.refresh()
 
 # ! Plugin Loader Class
 class PluginLoader:
     __title__: str = "PluginLoader"
-    __version__: str = "0.1.3"
+    __version__: str = "0.1.4"
     __author__: str = "Romanin"
     __email__: str = "semina054@gmail.com"
 
     def __init__(
         self,
         app,
         plugins_dirpath: Optional[Union[str, Path]]=None,
```

### Comparing `seaplayer-0.5.4.dev3/seaplayer/plug/pluginloader.pyi` & `seaplayer-0.5.5/seaplayer/plug/pluginloader.pyi`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/screens/Configurate.py` & `seaplayer-0.5.5/seaplayer/screens/Configurate.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/screens/Unknown.py` & `seaplayer-0.5.5/seaplayer/screens/Unknown.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/seaplayer.py` & `seaplayer-0.5.5/seaplayer/seaplayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,46 +49,47 @@
     ENABLE_PLUGIN_SYSTEM,
     CACHE_DIRPATH
 )
 # > Plugin System Init
 if ENABLE_PLUGIN_SYSTEM:
     from .plug import PluginLoader
 
-# ! Main Functions
-def build_bindings(config: SeaPlayerConfig):
-    yield Binding(config.key_quit, "quit", "Quit")
-    yield Binding("c,с", "push_screen('configurate')", "Configurate")
-    if config.log_menu_enable:
-        yield Binding("l,д", "app.toggle_class('.log-menu', '-hidden')", 'Logs')
-    yield Binding(config.key_rewind_back, "minus_rewind", f"Rewind -{config.rewind_count_seconds} sec")
-    yield Binding(config.key_rewind_forward, "plus_rewind", f"Rewind +{config.rewind_count_seconds} sec")
-    yield Binding(config.key_volume_down, "minus_volume", f"Volume -{round(config.volume_change_percent*100)}%")
-    yield Binding(config.key_volume_up, "plus_volume", f"Volume +{round(config.volume_change_percent*100)}%")
-    yield Binding("ctrl+s", "screenshot", "Screenshot")
-    yield Binding(UNKNOWN_OPEN_KEY, "push_screen('unknown')", "None", show=False)
-
 # ! Main
 class SeaPlayer(App):
+    # ! Pre-Initialization Functions
+    def build_bindings(config: SeaPlayerConfig):
+        yield Binding(config.key_quit, "quit", "Quit")
+        yield Binding("c,с", "push_screen('configurate')", "Configurate")
+        if config.log_menu_enable:
+            yield Binding("l,д", "app.toggle_class('.log-menu', '-hidden')", 'Logs')
+        yield Binding(config.key_rewind_back, "minus_rewind", f"Rewind -{config.rewind_count_seconds} sec")
+        yield Binding(config.key_rewind_forward, "plus_rewind", f"Rewind +{config.rewind_count_seconds} sec")
+        yield Binding(config.key_volume_down, "minus_volume", f"Volume -{round(config.volume_change_percent*100)}%")
+        yield Binding(config.key_volume_up, "plus_volume", f"Volume +{round(config.volume_change_percent*100)}%")
+        yield Binding("ctrl+s", "screenshot", "Screenshot")
+        yield Binding(UNKNOWN_OPEN_KEY, "push_screen('unknown')", "None", show=False)
+    
     # ! Textual Configuration
     TITLE = f"{__title__} v{__version__}"
     CSS_PATH = [
         os.path.join(CSS_LOCALDIR, "seaplayer.css"),
         os.path.join(CSS_LOCALDIR, "configurate.css"),
         os.path.join(CSS_LOCALDIR, "unknown.css"),
         os.path.join(CSS_LOCALDIR, "objects.css")
     ]
     SCREENS = {
         "unknown": Unknown(id="screen_unknown"),
         "configurate": Configurate(id="screen_configurate")
     }
     
-    # ! SeaPlayer Configuration & Hanlders
+    # ! SeaPlayer Configuration
     cache = Cacher(CACHE_DIRPATH)
     config = SeaPlayerConfig(CONFIG_FILEPATH)
     max_volume_percent: float = config.max_volume_percent
+    image_type: Optional[Union[Type[AsyncImageLabel], Type[StandartImageLabel]]] = None
     
     # ! Textual Keys Configuration
     BINDINGS = list(build_bindings(config))
     
     # ! Template Configuration
     currect_sound_uuid: Optional[str] = None
     currect_sound: Optional[CodecBase] = None
@@ -133,14 +134,15 @@
     # ! Nofy's
     def nofy(
         self,
         text: str,
         life_time: float=3,
         dosk: Literal["bottom", "left", "right", "top"]="top"
     ) -> None:
+        """"""
         self.screen.mount(Nofy(text, life_time, dosk))
     
     async def aio_nofy(
         self,
         text: str,
         life_time: float=3,
         dosk: Literal["bottom", "left", "right", "top"]="top"
@@ -161,57 +163,66 @@
         text: str,
         dosk: Literal["bottom", "left", "right", "top"]="top"
     ) -> CallNofy:
         cn = CallNofy(text, dosk)
         await self.screen.mount(cn)
         return cn
 
-    # ! Functions, Workers and other...
+    # ! Get Current Sound
     def gcs(self) -> Optional[CodecBase]:
         if (self.currect_sound is None) and (self.currect_sound_uuid is not None):
             self.currect_sound = self.music_list_view.music_list.get(self.currect_sound_uuid)
         return self.currect_sound
     
     async def aio_gcs(self):
         if (self.currect_sound is None) and (self.currect_sound_uuid is not None):
             self.currect_sound = await self.music_list_view.music_list.aio_get(self.currect_sound_uuid)
         return self.currect_sound
 
-    async def get_sound_seek(self) -> Tuple[str, Optional[float], Optional[float]]:
-        if (sound:=await self.aio_gcs()) is not None:
-            pos = sound.get_pos()
-            minutes, seconds = round(pos // 60), round(pos % 60)
-            return f"{minutes}:{str(seconds).rjust(2,'0')} | {str(round(sound.get_volume()*100)).rjust(3)}%", pos, sound.duration
-        return "0:00 |   0%", None, None
-    
+    # ! Get Current Sound Status Text
     def get_sound_selected_label_text(self, sound: Optional[CodecBase]=None) -> str:
         if sound is None:
             sound = self.gcs()
         if sound is not None:
             return f"({check_status(sound)}): {get_sound_basename(sound)}"
         return "<sound not selected>"
     
     async def aio_get_sound_selected_label_text(self, sound: Optional[CodecBase]=None) -> str:
         if sound is None:
             sound = await self.aio_gcs()
         if sound is not None:
             return f"({check_status(sound)}): {get_sound_basename(sound)}"
         return "<sound not selected>"
     
+    # ! Update Selected Label Text
     def update_select_label(self, sound: Optional[CodecBase]=None) -> None:
         self.music_selected_label.update(self.get_sound_selected_label_text(sound))
     
     async def aio_update_select_label(self, sound: Optional[CodecBase]=None) -> None:
         self.music_selected_label.update(await self.aio_get_sound_selected_label_text(sound))
     
-    def gpms(self, modes: Tuple[str, str, str]=("(MODE): PLAY", "(MODE): REPLAY SOUND", "(MODE): REPLAY LIST")) -> str: return modes[self.playback_mode]
+    # ! Switch Mode Button
+    def gpms(self, modes: Tuple[str, str, str]=("(MODE): PLAY", "(MODE): REPLAY SOUND", "(MODE): REPLAY LIST")) -> str:
+        return modes[self.playback_mode]
+
     def switch_playback_mode(self) -> None:
-        if self.playback_mode == 2: self.playback_mode = 0
-        else: self.playback_mode += 1
+        if self.playback_mode == 2:
+            self.playback_mode = 0
+        else:
+            self.playback_mode += 1
     
+    # ! Callback Functions
+    async def get_sound_seek(self) -> Tuple[str, Optional[float], Optional[float]]:
+        if (sound:=await self.aio_gcs()) is not None:
+            pos = sound.get_pos()
+            minutes, seconds = round(pos // 60), round(pos % 60)
+            return f"{minutes}:{str(seconds).rjust(2,'0')} | {str(round(sound.get_volume()*100)).rjust(3)}%", pos, sound.duration
+        return "0:00 |   0%", None, None
+    
+    # ! Loop Functions
     async def update_loop_playback(self) -> None:
         while self.started:
             if (sound:=await self.aio_gcs()) is not None:
                 status = check_status(sound)
                 if (self.last_playback_status is not None) and (self.last_playback_status != status):
                     await self.aio_update_select_label(sound)
                 
@@ -227,14 +238,15 @@
                             await self.music_list_view.aio_select_list_item_from_sound_uuid(sound_uuid)
                             sound.play()
                             self.info(f"Playing the next sound: {repr(sound)}")
                 
                 self.last_playback_status = status
             await asyncio.sleep(0.2)
     
+    # ! Mounting Function
     def compose(self) -> ComposeResult:
         # * Other
         self.info("---")
         self.info(f"{__title__} v{__version__} from {__author__} ({__email__})")
         self.info(f"Source          : {__url__}")
         self.info(f"Codecs          : {repr(self.CODECS)}")
         self.info(f"Config Path     : {repr(self.config.filepath)}")
@@ -245,29 +257,39 @@
         # * Play Screen
         self.music_play_screen = Static(classes="screen-box")
         self.music_play_screen.border_title = "Player"
         
         # * Image Object Init
         self.music_selected_label = Label(self.get_sound_selected_label_text(), classes="music-selected-label")
         if self.config.image_update_method == "sync":
-            self.music_image = StandartImageLabel(Image.open(IMGPATH_IMAGE_NOT_FOUND), resample=RESAMPLING_SAFE[self.config.image_resample_method])
+            self.image_type = StandartImageLabel
         elif self.config.image_update_method == "async":
-            self.music_image = AsyncImageLabel(Image.open(IMGPATH_IMAGE_NOT_FOUND), resample=RESAMPLING_SAFE[self.config.image_resample_method])
+            self.image_type = AsyncImageLabel
         else:
             raise RuntimeError("The configuration 'image_update_method' is incorrect.")
+        
+        self.music_image = self.image_type(
+            Image.open(IMGPATH_IMAGE_NOT_FOUND),
+            resample=RESAMPLING_SAFE[self.config.image_resample_method]
+        )
         self.info(f"The picture from the media file is rendered using the {repr(self.config.image_update_method)} method.")
         
         # * Compositions Screen
         self.music_list_screen = Static(classes="screen-box")
         self.music_list_screen.border_title = "Playlist"
         
         self.music_list_view = MusicListView()
         
-        async def _spm(input: InputField, value: Any) -> None: await self.submit_plus_sound(value)
-        self.music_list_add_input = InputField(submit=_spm, placeholder="Filepath / Search Mask", classes="music-list-screen-add-input")
+        async def _spm(input: InputField, value: Any) -> None:
+            await self.submit_plus_sound(value)
+        self.music_list_add_input = InputField(
+            submit=_spm,
+            placeholder="Filepath / Search Mask / URL",
+            classes="music-list-screen-add-input"
+        )
         
         # * Adding
         yield Header()
         with self.music_play_screen:
             with Vertical():
                 with Static(classes="player-visual-panel"):
                     yield self.music_image
@@ -298,19 +320,69 @@
                 self.plugin_loader.on_compose,
                 name="ON_COMPOSE",
                 group="PluginLoader",
                 description="<method PluginLoader.on_compose>"
             )
         self.info("---")
     
+    # ! Currect Sound Controls
+    async def currect_sound_stop(self, sound: Optional[CodecBase]=None):
+        if sound is None: sound = await self.aio_gcs()
+        if sound is not None:
+            self.last_playback_status = "Stoped"
+            sound.stop()
+    
+    async def currect_sound_play(self, sound: Optional[CodecBase]=None):
+        if sound is None: sound = await self.aio_gcs()
+        if sound is not None:
+            self.last_playback_status = "Playing"
+            sound.play()
+    
+    async def currect_sound_pause(self, sound: Optional[CodecBase]=None):
+        if sound is None: sound = await self.aio_gcs()
+        if sound is not None:
+            self.last_playback_status = "Paused"
+            sound.pause()
+    
+    async def currect_sound_unpause(self, sound: Optional[CodecBase]=None):
+        if sound is None: sound = await self.aio_gcs()
+        if sound is not None:
+            self.last_playback_status = "Playing"
+            sound.unpause()
+    
+    # ! Sound Controls
+    async def set_sound_for_playback(
+        self,
+        sound_uuid: Optional[str],
+        playback_mode_blocked: Optional[bool]=None
+    ) -> Optional[CodecBase]:
+        if playback_mode_blocked is not None:
+            self.playback_mode_blocked = playback_mode_blocked
+        if sound_uuid is not None:
+            if not self.playback_mode_blocked:
+                sound = await self.aio_gcs()
+                await self.currect_sound_stop(sound)
+            self.playback_mode_blocked = False
+            
+            sound = await self.music_list_view.aio_get_sound(sound_uuid)
+            if sound is not None:
+                sound.set_volume(self.currect_volume)
+                await self.music_image.update_image(image_from_bytes(sound.icon_data))
+                self.info(f"A new sound has been selected: {repr(sound)}")
+            
+            self.currect_sound = sound
+            self.currect_sound_uuid = sound_uuid if self.currect_sound is not None else None
+            
+            await self.aio_update_select_label(sound)
+            return sound
+    
     async def add_sounds_to_list(self) -> None:
         added_oks = 0
-        loading_nofy = await self.aio_callnofy(
-            f"Found [cyan]{len(self.last_paths_globalized)}[/cyan] values. Loading..."
-        )
+        loading_nofy = await self.aio_callnofy(f"Found [cyan]{len(self.last_paths_globalized)}[/cyan] values. Loading...")
+        
         async for path in aiter(self.last_paths_globalized):
             sound = None
             async for codec in aiter(self.CODECS):
                 try:
                     if await codec.aio_is_this_codec(path):
                         if not hasattr(codec, "__aio_init__"):
                             try:
@@ -329,46 +401,23 @@
                                 await self.music_list_view.aio_add_sound(sound)
                                 self.info(f"Song added: {repr(sound)}")
                                 added_oks += 1
                                 break
                 except FileNotFoundError:
                     self.error(f"The file does not exist or is a directory: {repr(path)}")
                     break
-                except Exception as e:
-                    self.exception(e)
+                except OSError: pass
+                except Exception as e: self.exception(e)
             if sound is None:
                 self.error(f"The sound could not be loaded: {repr(path)}")
         await loading_nofy.remove()
         self.info(f"Added [cyan]{added_oks}[/cyan] songs!")
         await self.aio_nofy(f"Added [cyan]{added_oks}[/cyan] songs!")
     
-    async def currect_sound_stop(self, sound: Optional[CodecBase]=None):
-        if sound is None: sound = await self.aio_gcs()
-        if sound is not None:
-            self.last_playback_status = "Stoped"
-            sound.stop()
-    
-    async def currect_sound_play(self, sound: Optional[CodecBase]=None):
-        if sound is None: sound = await self.aio_gcs()
-        if sound is not None:
-            self.last_playback_status = "Playing"
-            sound.play()
-    
-    async def currect_sound_pause(self, sound: Optional[CodecBase]=None):
-        if sound is None: sound = await self.aio_gcs()
-        if sound is not None:
-            self.last_playback_status = "Paused"
-            sound.pause()
-    
-    async def currect_sound_unpause(self, sound: Optional[CodecBase]=None):
-        if sound is None: sound = await self.aio_gcs()
-        if sound is not None:
-            self.last_playback_status = "Playing"
-            sound.unpause()
-    
+    # ! Button Actions
     async def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "switch-playback-mode":
             self.switch_playback_mode()
             event.button.label = self.gpms()
     
     @on(Button.Pressed, "#button-pause")
     async def bp_pause_unpause(self) -> None:
@@ -384,58 +433,40 @@
                     await self.currect_sound_unpause(sound)
                 else:
                     await self.currect_sound_stop(sound)
             else:
                 await self.currect_sound_play(sound)
             await self.aio_update_select_label(sound)
     
+    # ! Input Submits
     async def submit_plus_sound(self, value: str) -> None:
         if value.replace(" ", "") != "":
-            try: self.last_paths_globalized = glob.glob(value, recursive=self.config.recursive_search)
-            except: self.last_paths_globalized = [ value ]
+            try:
+                self.last_paths_globalized = glob.glob(value, recursive=self.config.recursive_search)
+            except:
+                self.last_paths_globalized = [ value ]
+            if len(self.last_paths_globalized) == 0:
+                self.last_paths_globalized = [ value ]
             self.info(f"Submit 'plus_sound' values: {repr(self.last_paths_globalized)}")
             if len(self.last_paths_globalized) > 0:
                 self.run_worker(
                     self.add_sounds_to_list,
                     name="ADD_SOUND",
                     group="PLAYLIST_UPDATE",
                     description="The process of adding sounds to a playlist."
                 )
     
-    async def set_sound_for_playback(
-        self,
-        sound_uuid: Optional[str],
-        playback_mode_blocked: Optional[bool]=None
-    ) -> Optional[CodecBase]:
-        if playback_mode_blocked is not None:
-            self.playback_mode_blocked = playback_mode_blocked
-        if sound_uuid is not None:
-            if not self.playback_mode_blocked:
-                sound = await self.aio_gcs()
-                await self.currect_sound_stop(sound)
-            self.playback_mode_blocked = False
-            
-            sound = await self.music_list_view.aio_get_sound(sound_uuid)
-            if sound is not None:
-                sound.set_volume(self.currect_volume)
-                await self.music_image.update_image(image_from_bytes(sound.icon_data))
-                self.info(f"A new sound has been selected: {repr(sound)}")
-            
-            self.currect_sound = sound
-            self.currect_sound_uuid = sound_uuid if self.currect_sound is not None else None
-            
-            await self.aio_update_select_label(sound)
-            return sound
-    
+    # ! Other Actions
     async def on_list_view_selected(self, selected: MusicListView.Selected):
         if isinstance(selected.item, MusicListViewItem):
             sound_uuid = getattr(selected.item, "sound_uuid", None)
             if (sound_uuid != self.currect_sound_uuid) or (self.currect_sound_uuid is None):
                 await self.set_sound_for_playback(sound_uuid)
     
+    # ! Keys Actions
     async def action_plus_rewind(self):
         if (sound:=await self.aio_gcs()) is not None:
             sound.set_pos(sound.get_pos()+self.config.rewind_count_seconds)
     
     async def action_minus_rewind(self):
         if (sound:=await self.aio_gcs()) is not None:
             sound.set_pos(sound.get_pos()-self.config.rewind_count_seconds)
@@ -462,12 +493,13 @@
         if ENABLE_PLUGIN_SYSTEM:
             await self.plugin_loader.on_quit()
         if (sound:=await self.aio_gcs()) is not None:
             sound.unpause()
             sound.stop()
         return await super().action_quit()
 
+    # ! Other
     def run(self, *args, **kwargs):
         if ENABLE_PLUGIN_SYSTEM:
             self.plugin_loader.on_run()
         super().run(*args, **kwargs)
```

### Comparing `seaplayer-0.5.4.dev3/seaplayer/types/Cache.py` & `seaplayer-0.5.5/seaplayer/types/Cache.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/types/Convert.py` & `seaplayer-0.5.5/seaplayer/types/Convert.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/types/MusicList.py` & `seaplayer-0.5.5/seaplayer/types/MusicList.py`

 * *Files identical despite different names*

### Comparing `seaplayer-0.5.4.dev3/seaplayer/units.py` & `seaplayer-0.5.5/seaplayer/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from platformdirs import user_config_dir
 # > Image Works
 from PIL.Image import Resampling
 
 # ! Metadata
 __title__ = "SeaPlayer"
-__version__ = "0.5.4.dev3"
+__version__ = "0.5.5"
 __author__ = "Romanin"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/romanin-rf/SeaPlayer"
 
 # ! Paths
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     LOCALDIR = os.path.dirname(sys.executable)
```

### Comparing `seaplayer-0.5.4.dev3/PKG-INFO` & `seaplayer-0.5.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaplayer
-Version: 0.5.4.dev3
+Version: 0.5.5
 Summary: SeaPlayer is a player that works in the terminal.
 Home-page: https://github.com/romanin-rf/SeaPlayer
 License: MIT
 Keywords: tui,player,seaplayer,wav,mp3,ogg,midi
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -29,14 +29,16 @@
 Requires-Dist: properties-py (==1.1.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyinstaller (>=5.11.0,<6.0.0) ; extra == "build"
 Requires-Dist: rich (>=13.3.5)
 Requires-Dist: ripix (>=2.2.3)
 Requires-Dist: textual (>=0.26.0)
 Requires-Dist: typing-inspect (>=0.8.0,<0.9.0)
+Requires-Dist: urlopen2 (>=1.1.0,<2.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
 Project-URL: Repository, https://github.com/romanin-rf/SeaPlayer
 Description-Content-Type: text/markdown
 
 <div id="header" align="center">
     <img src="https://github.com/romanin-rf/SeaPlayer/assets/60302782/937adcc4-f547-440c-8139-a5f15bffa157" alt="Icon" width="300">
 </div>
 <div id="header" align="center"><h1>SeaPlayer</h1></div>
@@ -61,11 +63,10 @@
 
 You need to [install the FluidSynth](https://github.com/FluidSynth/fluidsynth/wiki/Download) package in order to playback `MIDI`.
 
 ## Using
 ```shell
 python -m seaplayer # Method for `downloaded repository` or `installed via pip`
 ```
-
-![MainScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/e4b2ee2c-9061-47ff-8818-a480b3a79a5e)
-![ConfigurateScreen-v0.4.3.dev1](https://github.com/romanin-rf/SeaPlayer/assets/60302782/ad84eafb-2324-4036-81c3-81df9138025a)
+![MainScreen-v0.5.4](https://github.com/romanin-rf/SeaPlayer/assets/60302782/5be6c2cb-5602-4c85-a3be-ae36a90e71e4)
+![ConfigurateScreen-v0.5.4](https://github.com/romanin-rf/SeaPlayer/assets/60302782/922c7112-2259-47d1-9619-488855e14c2c)
```

