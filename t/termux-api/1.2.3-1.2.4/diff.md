# Comparing `tmp/termux-api-1.2.3.tar.gz` & `tmp/termux-api-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termux-api-1.2.3.tar", last modified: Wed Jun 29 16:58:18 2022, max compression
+gzip compressed data, was "termux-api-1.2.4.tar", last modified: Wed May 31 16:26:08 2023, max compression
```

## Comparing `termux-api-1.2.3.tar` & `termux-api-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-06-29 16:58:18.343990 termux-api-1.2.3/
--rw-rw-rw-   0        0        0     1086 2022-06-29 16:50:46.000000 termux-api-1.2.3/LICENSE
--rw-rw-rw-   0        0        0     3529 2022-06-29 16:58:18.343990 termux-api-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2022-06-29 16:50:46.000000 termux-api-1.2.3/README.md
--rw-rw-rw-   0        0        0       42 2022-06-29 16:58:18.343990 termux-api-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      689 2022-06-29 16:46:33.000000 termux-api-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-29 16:58:18.325267 termux-api-1.2.3/termux/
--rw-rw-rw-   0        0        0     3440 2021-09-11 07:58:07.000000 termux-api-1.2.3/termux/API.py
--rw-rw-rw-   0        0        0      657 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Camera.py
--rw-rw-rw-   0        0        0      516 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Clipboard.py
--rw-rw-rw-   0        0        0     1351 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Media.py
--rw-rw-rw-   0        0        0     1277 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Microphone.py
--rw-rw-rw-   0        0        0     1242 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Notification.py
--rw-rw-rw-   0        0        0     2272 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Scheduler.py
--rw-rw-rw-   0        0        0     2463 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Sensors.py
--rw-rw-rw-   0        0        0     1076 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Share.py
--rw-rw-rw-   0        0        0     1109 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/TTS.py
--rw-rw-rw-   0        0        0      810 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Telephony.py
--rw-rw-rw-   0        0        0     4784 2021-09-11 07:44:44.000000 termux-api-1.2.3/termux/UI.py
--rw-rw-rw-   0        0        0      626 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/Wifi.py
--rw-rw-rw-   0        0        0      816 2022-06-29 16:50:46.000000 termux-api-1.2.3/termux/__init__.py
--rw-rw-rw-   0        0        0     1195 2022-06-29 16:46:33.000000 termux-api-1.2.3/termux/android.py
-drwxrwxrwx   0        0        0        0 2022-06-29 16:58:18.343990 termux-api-1.2.3/termux_api.egg-info/
--rw-rw-rw-   0        0        0     3529 2022-06-29 16:58:17.000000 termux-api-1.2.3/termux_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2022-06-29 16:58:18.000000 termux-api-1.2.3/termux_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-29 16:58:17.000000 termux-api-1.2.3/termux_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-06-29 16:58:17.000000 termux-api-1.2.3/termux_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 16:26:08.644661 termux-api-1.2.4/
+-rw-rw-rw-   0        0        0     1086 2022-06-29 16:50:48.000000 termux-api-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0     3621 2023-05-31 16:26:08.643661 termux-api-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3060 2022-06-30 07:05:02.000000 termux-api-1.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 16:26:08.644661 termux-api-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-05-31 16:21:50.000000 termux-api-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:26:08.637656 termux-api-1.2.4/termux/
+-rw-rw-rw-   0        0        0     3513 2023-05-31 16:21:50.000000 termux-api-1.2.4/termux/API.py
+-rw-rw-rw-   0        0        0      661 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Camera.py
+-rw-rw-rw-   0        0        0      520 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Clipboard.py
+-rw-rw-rw-   0        0        0     1269 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Media.py
+-rw-rw-rw-   0        0        0     1293 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Microphone.py
+-rw-rw-rw-   0        0        0     1237 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Notification.py
+-rw-rw-rw-   0        0        0     2284 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Scheduler.py
+-rw-rw-rw-   0        0        0     2241 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Sensors.py
+-rw-rw-rw-   0        0        0     1105 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Share.py
+-rw-rw-rw-   0        0        0     1112 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/TTS.py
+-rw-rw-rw-   0        0        0      814 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Telephony.py
+-rw-rw-rw-   0        0        0     4732 2023-05-31 16:21:50.000000 termux-api-1.2.4/termux/UI.py
+-rw-rw-rw-   0        0        0      455 2023-05-31 16:21:50.000000 termux-api-1.2.4/termux/Wake.py
+-rw-rw-rw-   0        0        0      638 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/Wifi.py
+-rw-rw-rw-   0        0        0      871 2023-05-31 16:21:50.000000 termux-api-1.2.4/termux/__init__.py
+-rw-rw-rw-   0        0        0     1195 2022-06-30 07:05:02.000000 termux-api-1.2.4/termux/android.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:26:08.642661 termux-api-1.2.4/termux_api.egg-info/
+-rw-rw-rw-   0        0        0     3621 2023-05-31 16:26:08.000000 termux-api-1.2.4/termux_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-05-31 16:26:08.000000 termux-api-1.2.4/termux_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 16:26:08.000000 termux-api-1.2.4/termux_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 16:26:08.000000 termux-api-1.2.4/termux_api.egg-info/top_level.txt
```

### Comparing `termux-api-1.2.3/LICENSE` & `termux-api-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `termux-api-1.2.3/PKG-INFO` & `termux-api-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-api
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package for accessing termux-api
 Home-page: https://github.com/shajul/termux-api.git
 Author: drshajul
 Author-email: drshajul@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 
 Most of the [termux-api implementations](https://wiki.termux.com/wiki/Termux:API) are directly available.
 The API.generic() method gives direct access to any other method that has not yet been implemented.
 
 ## Special thanks
 Thanks to termux and termux-api for making all this possible.
 This module is heavily inspired by https://github.com/azwyane/pimux, though the code has been 
-almost completely re-written and now is much more comprehensive.  
+almost completely re-written and now is much more comprehensive. Also, special thanks for recent contribution from [Young-Lord](https://github.com/Young-Lord)
 This project is originally located at [termux-api](https://github.com/shajul/termux-api)
 
 ## Table of Contents
 - [Requirements](#Requirements)
 - [Installation](#Installation)
 - [Features](#Features)
 - [Contributing](#Contributing)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: termux-api Version: 1.2.3 Summary: A package for
+Metadata-Version: 2.1 Name: termux-api Version: 1.2.4 Summary: A package for
 accessing termux-api Home-page: https://github.com/shajul/termux-api.git
 Author: drshajul Author-email: drshajul@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # termux-api [!
 [Build Status](http://img.shields.io/travis/badges/
 badgerbadgerbadger.svg?style=flat-square)](https://github.com/shajul/termux-
@@ -11,28 +11,30 @@
 API) This provides a way to get native access in Python to Android device
 functionality as API. Most of the [termux-api implementations](https://
 wiki.termux.com/wiki/Termux:API) are directly available. The API.generic()
 method gives direct access to any other method that has not yet been
 implemented. ## Special thanks Thanks to termux and termux-api for making all
 this possible. This module is heavily inspired by https://github.com/azwyane/
 pimux, though the code has been almost completely re-written and now is much
-more comprehensive. This project is originally located at [termux-api](https://
-github.com/shajul/termux-api) ## Table of Contents - [Requirements]
-(#Requirements) - [Installation](#Installation) - [Features](#Features) -
-[Contributing](#Contributing) ## Requirements - Termux app - Termux-api (both
-app and package) - Python installed in termux ($ pkg install python) ##
-Installation ð  Android install through termux: ### Method-1 **Install by
-pip** The stable version is available in the Pypi, which you can download by:
-``` $ python3 -m pip install termux-api ``` ### Method-2 You can always get the
-latest version of termux-api maintained here in the github. - Clone this repo
-to your local machine(termux) using `https://github.com/shajul/termux-api.git`
-Goto to your terminal and type: ```sh $ git clone https://github.com/shajul/
-termux-api.git $ python3 -m pip install wheel $ python3 -m pip install dist/
-termux_api*.whl ``` Or you can add this to site packages by first building it
-first: ``` $ python3 setup.py sdist bdist_wheel $ python3 -m pip install -e
+more comprehensive. Also, special thanks for recent contribution from [Young-
+Lord](https://github.com/Young-Lord) This project is originally located at
+[termux-api](https://github.com/shajul/termux-api) ## Table of Contents -
+[Requirements](#Requirements) - [Installation](#Installation) - [Features]
+(#Features) - [Contributing](#Contributing) ## Requirements - Termux app -
+Termux-api (both app and package) - Python installed in termux ($ pkg install
+python) ## Installation ð  Android install through termux: ### Method-
+1 **Install by pip** The stable version is available in the Pypi, which you can
+download by: ``` $ python3 -m pip install termux-api ``` ### Method-2 You can
+always get the latest version of termux-api maintained here in the github. -
+Clone this repo to your local machine(termux) using `https://github.com/shajul/
+termux-api.git` Goto to your terminal and type: ```sh $ git clone https://
+github.com/shajul/termux-api.git $ python3 -m pip install wheel $ python3 -
+m pip install dist/termux_api*.whl ``` Or you can add this to site packages by
+first building it first: ``` $ python3 setup.py sdist bdist_wheel $ python3 -
+m pip install -e
 .whl> ``` Finally, you have it installed. ## Run the project Now to run the
 termux-api type in your terminal: ```bash $ python >>> import termux >>>
 termux.API.vibrate() >>> help(termux.API) #for available methods ``` Avaliable
 modules are API, Camera, Clipboard, Media, Microphone, Notification, Scheduler,
 Sensors, Share, Telephony, TTS, UI, Wifi OR ```bash $ python >>> from termux
 import  >>> API.vibrate() >>> help(API) # for details of available methods ```
 ## Contributing ### Step 1 - Option 1 - ð´ Fork this repo! - Option 2 - ð¯
```

### Comparing `termux-api-1.2.3/README.md` & `termux-api-1.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Most of the [termux-api implementations](https://wiki.termux.com/wiki/Termux:API) are directly available.
 The API.generic() method gives direct access to any other method that has not yet been implemented.
 
 ## Special thanks
 Thanks to termux and termux-api for making all this possible.
 This module is heavily inspired by https://github.com/azwyane/pimux, though the code has been 
-almost completely re-written and now is much more comprehensive.  
+almost completely re-written and now is much more comprehensive. Also, special thanks for recent contribution from [Young-Lord](https://github.com/Young-Lord)
 This project is originally located at [termux-api](https://github.com/shajul/termux-api)
 
 ## Table of Contents
 - [Requirements](#Requirements)
 - [Installation](#Installation)
 - [Features](#Features)
 - [Contributing](#Contributing)
```

#### html2text {}

```diff
@@ -5,28 +5,30 @@
 API) This provides a way to get native access in Python to Android device
 functionality as API. Most of the [termux-api implementations](https://
 wiki.termux.com/wiki/Termux:API) are directly available. The API.generic()
 method gives direct access to any other method that has not yet been
 implemented. ## Special thanks Thanks to termux and termux-api for making all
 this possible. This module is heavily inspired by https://github.com/azwyane/
 pimux, though the code has been almost completely re-written and now is much
-more comprehensive. This project is originally located at [termux-api](https://
-github.com/shajul/termux-api) ## Table of Contents - [Requirements]
-(#Requirements) - [Installation](#Installation) - [Features](#Features) -
-[Contributing](#Contributing) ## Requirements - Termux app - Termux-api (both
-app and package) - Python installed in termux ($ pkg install python) ##
-Installation ð  Android install through termux: ### Method-1 **Install by
-pip** The stable version is available in the Pypi, which you can download by:
-``` $ python3 -m pip install termux-api ``` ### Method-2 You can always get the
-latest version of termux-api maintained here in the github. - Clone this repo
-to your local machine(termux) using `https://github.com/shajul/termux-api.git`
-Goto to your terminal and type: ```sh $ git clone https://github.com/shajul/
-termux-api.git $ python3 -m pip install wheel $ python3 -m pip install dist/
-termux_api*.whl ``` Or you can add this to site packages by first building it
-first: ``` $ python3 setup.py sdist bdist_wheel $ python3 -m pip install -e
+more comprehensive. Also, special thanks for recent contribution from [Young-
+Lord](https://github.com/Young-Lord) This project is originally located at
+[termux-api](https://github.com/shajul/termux-api) ## Table of Contents -
+[Requirements](#Requirements) - [Installation](#Installation) - [Features]
+(#Features) - [Contributing](#Contributing) ## Requirements - Termux app -
+Termux-api (both app and package) - Python installed in termux ($ pkg install
+python) ## Installation ð  Android install through termux: ### Method-
+1 **Install by pip** The stable version is available in the Pypi, which you can
+download by: ``` $ python3 -m pip install termux-api ``` ### Method-2 You can
+always get the latest version of termux-api maintained here in the github. -
+Clone this repo to your local machine(termux) using `https://github.com/shajul/
+termux-api.git` Goto to your terminal and type: ```sh $ git clone https://
+github.com/shajul/termux-api.git $ python3 -m pip install wheel $ python3 -
+m pip install dist/termux_api*.whl ``` Or you can add this to site packages by
+first building it first: ``` $ python3 setup.py sdist bdist_wheel $ python3 -
+m pip install -e
 .whl> ``` Finally, you have it installed. ## Run the project Now to run the
 termux-api type in your terminal: ```bash $ python >>> import termux >>>
 termux.API.vibrate() >>> help(termux.API) #for available methods ``` Avaliable
 modules are API, Camera, Clipboard, Media, Microphone, Notification, Scheduler,
 Sensors, Share, Telephony, TTS, UI, Wifi OR ```bash $ python >>> from termux
 import  >>> API.vibrate() >>> help(API) # for details of available methods ```
 ## Contributing ### Step 1 - Option 1 - ð´ Fork this repo! - Option 2 - ð¯
```

### Comparing `termux-api-1.2.3/setup.py` & `termux-api-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="termux-api", 
-    version="1.2.3",
+    version="1.2.4",
     author="drshajul",
     author_email="drshajul@gmail.com",
     description="A package for accessing termux-api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shajul/termux-api.git",
     packages=setuptools.find_packages(),
```

### Comparing `termux-api-1.2.3/termux/Camera.py` & `termux-api-1.2.4/termux/Camera.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from .android import execute
 from datetime import datetime
 
 def info():
     '''
     Returns camera info in JSON format
     '''
-    return execute("termux-camera-info")
+    return execute(["termux-camera-info"])
 
 def takephoto(cid=0, saveas=None):
     '''
     Take a picture
 
     Parameters
     ----------
     cid: camera id (int), default is 0
     saveas: output file name (str), default is <timestamp>.jpg
     '''
-    if saveas == None:
+    if saveas is None:
         saveas = datetime.now().strftime("%Y%m%d_%H%M%S") + '.jpg'
-    return execute(f"termux-camera-photo -c {cid} {saveas}")
+    return execute(["termux-camera-photo", "-c", cid, saveas])
```

### Comparing `termux-api-1.2.3/termux/Clipboard.py` & `termux-api-1.2.4/termux/Clipboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 from .android import execute
 
 def getclipboard():
    '''
    Returns value stored in the clipboard.
    '''
-   return execute("termux-clipboard-get")
+   return execute(["termux-clipboard-get"])
 
 def setclipboard(newClip: str = " "):
     '''
     Set new value to clipboard
 
     Parameters
     ----------
     newClip: (optional) - new clipboard text (default is empty string)
     '''
-    return execute("termux-clipboard-set", stdin=newClip)
+    return execute(["termux-clipboard-set"], stdin=newClip)
```

### Comparing `termux-api-1.2.3/termux/Microphone.py` & `termux-api-1.2.4/termux/Microphone.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,26 +27,27 @@
     '''   
 
     params = {
       "encoder": "-e",
       "bitrate": "-b",
       "rate": "-r",
       "count": "-c"   
-    }; opt = ""
+    }
+    opt = []
     if len(kwargs) == 0:
-      opt = "-d"
+      opt += ["-d"]
     else: 
       for k,v in kwargs.items():
-        opt += f"{params[k]} {v} "
-    return execute(f"termux-microphone-record -f {file} -l {limit} {opt}")
+        opt += [params[k], v]
+    return execute(["termux-microphone-record", "-f", file, "-l", limit] + opt)
 
 def info():
     '''
     Get recording information
     '''
-    return execute("termux-microphone-record -i")
+    return execute(["termux-microphone-record", "-i"])
 
 def stop():
     '''
     Quits recording 
     '''
-    return execute("termux-microphone-record -q")
+    return execute(["termux-microphone-record", "-q"])
```

### Comparing `termux-api-1.2.3/termux/Notification.py` & `termux-api-1.2.4/termux/Notification.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 from .android import execute
 
 def remove(nid: int):
     '''
     Remove notificaiton with the given id
     '''
-    return execute(f"termux-notification-remove {nid}")
+    return execute(["termux-notification-remove", nid])
 
 
 def notify(title: str, content: str, nid: int = 1, args: tuple = (), kwargs: dict = {}):
     '''
     Create a notification
 
     Parameters
@@ -24,19 +24,19 @@
         required to remove notification
     args: (optional) A tuple of arguments, eg ("ongoing", "sound")
     kwargs: (optional) A dict of args, eg {"led-color": "ff00ff"}
     
     For more info visit
         [termux wiki](https://wiki.termux.com/wiki/Termux-notification)
     '''
-    cargs = kargs = ""
+    cargs = kargs = []
     if len(args) > 0:
         for v in args:
-            cargs += f"-{v} " if (len(v) == 1) else f"--{v} "
+            cargs.append(f"-{v}" if (len(v) == 1) else f"--{v}")
     
     if len(kwargs) > 0:
         for k,v in kwargs.items():
-            kargs += (f"-{k} " if (len(k) == 1) else f"--{k} ") + f'"{v}" '
+            kargs += [(f"-{k}" if (len(k) == 1) else f"--{k}"), str(v)]
 
     opts = cargs + kargs
 
-    return execute(f'termux-notification -t "{title}" -c "{content}" -i "{str(nid)}" {opts}')
+    return execute(["termux-notification", "-t", title, "-c", content, "-i", nid] + opts)
```

### Comparing `termux-api-1.2.3/termux/Scheduler.py` & `termux-api-1.2.4/termux/Scheduler.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,50 +3,53 @@
     cancel    - Cancel job with given id
     cancelAll - Cancel all jobs
     listAll   - list pending jobs
     schedule  - schedule new job
 '''
 from .android import execute
 
-def _makeopt(str): 
+def _makeopt(str):
+    '''
+    Convert var like "batteryNotLow" to argument like "battery-not-low".
+    '''
     res = [str[0].lower()] 
     for c in str[1:]: 
         if c in ('ABCDEFGHIJKLMNOPQRSTUVWXYZ'): 
             res.append('-') 
             res.append(c.lower()) 
         else: 
             res.append(c) 
     return ''.join(res) 
 
-def cancel(id: int):
+def cancel(jid: int):
     '''
     Cancel job with the given id
     '''
-    return execute(f"termux-job-scheduler --cancel {id}")
+    return execute(["termux-job-scheduler", "--cancel", jid])
 
 def cancelAll():
     '''
     Cancel all jobs
     '''
-    return execute("termux-job-scheduler --cancel-all")
+    return execute(["termux-job-scheduler", "--cancel-all"])
 
 def listAll():
     '''
     List pending jobs
     '''
-    return execute("termux-job-scheduler -p")
+    return execute(["termux-job-scheduler", "-p"])
 
-def schedule(script: str, id: int, **kwargs):
+def schedule(script: str, jid: int, **kwargs):
     '''
     Schedule a script to run at specified intervals. 
 
     Parameters
     ----------
     script :str         path of script to be called
-    id :int             overwrites previous job if same id
+    jid :int            overwrites previous job if same id
     periodMs :int       milliseconds (default 0 means once).
                           Since Android N, the minimum period
                           is 900,000ms (15 minutes).
     network :str        run only when network type available 
                           (default any)
                           any|unmetered|cellular|not_roaming|none
     batteryNotLow :bool run only when battery is not low
@@ -54,20 +57,19 @@
     storageNotLow :bool run only when storage is not low
                           default false (>= Android O)
     charging :bool      run only when charging, default false
     persisted :bool     survive reboots, default false
     triggerContentUri  :str  (>= Android N)
     triggerContentFlag :int  default 1, (>= Android N)
     '''
-    kargs = ""
+    kargs = []
     
     if len(kwargs) > 0:
         for k,v in kwargs.items():
+            kargs.append("--" + _makeopt(k))
             if type(v) is bool:
-                kargs += f"--{_makeopt(k)} " + f'{str(v).lower()} '
-            elif type(v) is int:
-                kargs += f"--{_makeopt(k)} " + f'{v} '
+                kargs.append(str(v).lower())
             else:
-                kargs += f"--{_makeopt(k)} " + f'"{v}" '
+                kargs.append(v)
 
-    return execute(f'termux-job-scheduler -s "{script}" --job-id {str(id)} {kargs}')
+    return execute(["termux-job-scheduler", "-s", script, "--job-id", jid] + kargs)
```

### Comparing `termux-api-1.2.3/termux/Sensors.py` & `termux-api-1.2.4/termux/Sensors.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,75 +5,67 @@
     sensors - Lists available sensors on the device
     cleanup - Performs cleanup releasing sensor resources.
     sensorsData - Output specific sensor(s) data. (limit = 1)
     allSensorsData - Output all sensors data (limit = 1)
     liveSaveLog - Live sensor data to stdout and to log file.    
 '''
 
-from .android import execute,liveSave
+from .android import execute, liveSave
 
 def sensors():
     '''
     Lists available sensors on the device.
     '''
-    return execute("termux-sensor -l")
+    return execute(["termux-sensor", "-l"])
 
 def cleanup():
     '''
     Performs cleanup releasing sensor resources.
     '''
-    return execute("termux-sensor -c")
+    return execute(["termux-sensor", "-c"])
 
 def sensorsData(*args):
     '''
     Output specific sensor(s) data. (JSON)
     You can pass multiple sensor names as arguments.
     As live data is not useful when calling from 
     python, only one reading is retrieved by this method.
     If you need continous data, you can create a 
     loop in python
     '''
-    sname=tuple(args)
+    sname = tuple(args)
     if not sname:
-        return "At least one sensor name required. \nFor finding sensor name call sensors() method"
+        raise ValueError("At least one sensor name required.\nFor finding sensor name call sensors() method.")
     else:
-        sensornames=""
-        for v in sname:
-            sensornames += v + ","      
-        return execute(f"termux-sensor -n 1 -s {sensornames[0:-1]}")
+        sensorNames = ','.join(sname)
+        return execute(["termux-sensor", "-n", "1", "-s", sensorNames])
 
 
 def allSensorsData():
     '''
     Method to print sensor data all at once.
     As live data is not useful when calling from 
     python, only one reading is retrieved by this method.
     If you need continous data, you can create a 
     loop in python
     '''
-    return execute("termux-sensor -n 1 -a")
+    return execute(["termux-sensor", "-n", "1", "-a"])
 
 
 def liveSaveLog(sensors, logfile = 'sensors.log', delay = 1000, limit = 60):
     '''
     Live sensor data to stdout and to log file.
 
     Parameters
     ----------
-    sensors = tuple of sensors to query data for (or string sensor)
+    sensors = tuple|list of sensors to query data for (or string sensor)
     logfile = file to log to (default is 'sensors.log')
     delay = delay between querying sensor (default 1000 ms)
     limit = number of time to query (default 60, 0 for no limit)
 
     Example:
     > > > sensors = 'gravity', 'Orientation'
     > > > liveSaveLog( sensors , limit = 10 )
     '''
-    if type(sensors) is tuple:
-        sensornames=""
-        for v in sensors:
-            sensornames += v + ","      
-        liveSave(f"termux-sensor -d {delay} -n {limit} -s {sensornames[0:-1]}", logfile)
-    elif type(sensors) is str:
-        liveSave(f"termux-sensor -d {delay} -n {limit} -s {sensors}", logfile)
-    else:
-        return 'Invalid sensors argument'
+    if type(sensors) in (tuple, list):
+        sensors = ",".join(sensors)
+    liveSave(["termux-sensor", "-d", delay, "-n", limit, "-s", sensors], logfile)
```

### Comparing `termux-api-1.2.3/termux/Share.py` & `termux-api-1.2.4/termux/Share.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,33 +10,33 @@
   Share text
 
   Parameters
   ----------
   action = edit/send/view (default: send)
   defaultReciever  = default receiver instead of showing a chooser
   '''
-  opt = f"-a {action}"
+  opt = ["-a", action]
   if defaultReciever:
-    opt += " -d"
-  
-  return execute(f'echo "{text}" | termux-share {opt}')
+    opt.append("-d")
+  return execute(["termux-share"] + opt, stdin=text)
 
 def file(filepath: str, action = "send", defaultReciever = False, contentType = None, title = None):
   '''
-  Share text
+  Share file
 
   Parameters
   ----------
+  filepath = file to share
   action = edit/send/view (default: send)
-  defaultReciever  = default receiver instead of showing a chooser
+  defaultReciever = default receiver instead of showing a chooser
   contentType = eg, "text/plain" (default: guessed from file extension)
   title = title to share (default: None)
   '''
-  opt = f"-a {action}"
+  opt = ["-a", action]
   if defaultReciever:
-    opt += " -d"
+    opt.append("-d")
   if contentType is not None:
-    opt += " -c {contentType}"
+    opt += ["-c", contentType]
   if title is not None:
-    opt += " -t {title}"
+    opt += ["-t", title]
   
-  return execute(f'termux-share {opt} "{filepath}"')
+  return execute(["termux-share"] + opt + [filepath])
```

### Comparing `termux-api-1.2.3/termux/TTS.py` & `termux-api-1.2.4/termux/TTS.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 from .android import execute
 
 def tts_info():
     '''
     Get tts-engines info (JSON format).
     '''
-    return execute("termux-tts-engines")
+    return execute(["termux-tts-engines"])
 
 
 def tts_speak(text, **kwargs):
     '''
     Text to speech.  
 
     Parameters
@@ -26,20 +26,21 @@
     stream: (optional) audio stream to use
     region: (optional) language region
     variant: (optional) language variant 
     for more info visit [termux wiki](https://wiki.termux.com/wiki/Termux-tts-speak)
 
     TODO: Implement os.mkfifo() and os.pipe() 
     '''
-    opts = ""; params = {
+    opts = []
+    params = {
         "engine" : "e",
         "language" : "l",
         "region" : "n",
         "variant" : "v",
         "pitch" : "p",
         "rate" : "r",
         "stream" : "s"}
     
     for k,v in kwargs.items():
-        opts += f'-{params[k]} "{v}" '
+        opts += ['-'+params[k], v]
     
-    return execute(f"termux-tts-speak {opts} {text}")
+    return execute(["termux-tts-speak"] + opts +[text])
```

### Comparing `termux-api-1.2.3/termux/Telephony.py` & `termux-api-1.2.4/termux/Telephony.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 '''
 
 from .android import execute
 
 def __dir__():
     return ['call', 'cellinfo', 'deviceinfo']
 
-def call(phone_number :str):
+def call(phone_number: str):
     '''
     Makes a phone call to number passed as an argument
     '''
-    return execute(f"termux-telephony-call {phone_number}")
+    return execute(["termux-telephony-call", phone_number])
 
 def cellinfo():
     '''
     Get information about all observed cell information
     from all radios on the device including the primary
     and neighboring cells. (JSON format)
     '''
-    return execute("termux-telephony-cellinfo")
+    return execute(["termux-telephony-cellinfo"])
 
 def deviceinfo():
     '''
     Get information about the telephony device. 
     '''
-    return execute("termux-telephony-displayinfo")
+    return execute(["termux-telephony-displayinfo"])
```

### Comparing `termux-api-1.2.3/termux/UI.py` & `termux-api-1.2.4/termux/UI.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,161 +10,151 @@
     spinner - Pick a single value from a dropdown spinner
     speech - Obtain speech using device microphone
     text - Input text
     toast - Show text as toast (transient popup) 
 '''
 from .android import execute
 
-def __radiolike(func,opts,title):
-  v = "-v "
-  for f in opts:
-    v += f'"{f}",'
-  v = v[0:-1]
+def __radiolike(func: str, opts: list | tuple, title: str):
+  v = ["-v"]
+  v.append(','.join([str(i) for i in opts]))
   if title is not None:
-    v += f' -t "{title}"'
-  return execute(f"termux-dialog {func} {v}")
+    v += ["-t", title]
+  return execute(["termux-dialog", func] + v)
 
-def __hintlike(func,hint,title):
-  opts = ""
+def __hintlike(func: str, hint: str, title: str):
+  opts = []
   if hint is not None:
-    opts += f'-i "{hint}" '
+    opts += ["-i", hint]
   if title is not None:
-    opts += f'-t "{title}"'
-  return execute(f"termux-dialog {func} {opts}")
+    opts += ["-t", title]
+  return execute(["termux-dialog", func] + opts)
    
 
 
 def confirm(hint: str = None, title: str = None):
   '''Show confirmation dialog
 
     hint - text hint (optional)
     title - set title of dialog (optional)
   '''
-  return __hintlike("confirm",hint,title)
+  return __hintlike("confirm", hint, title)
 
 def speech(hint :str = None, title :str = None):
   '''Obtain speech using device microphone
 
     hint - text hint (optional)
     title - set title of dialog (optional)
   '''
-  return __hintlike("speech",hint,title)
+  return __hintlike("speech", hint, title)
 
 
 def counter(rangeTuple :tuple = None, title :str = None):
   '''Pick a number in specified range
 
     rangeTuple - tuple of 3 numbers (min, max, start) (optional)
     title - set title of dialog (optional)
   '''
-  r = "-r "
-  for f in rangeTuple:
-    r += f'{f},'
-  r = r[0:-1]
+  r = ["-r", ','.join([str(i) for i in rangeTuple])]
   if title is not None:
-    r += f' -t "{title}"'
-  return execute(f"termux-dialog counter {r}")
+    r += ["-t", title]
+  return execute(["termux-dialog", "counter"] + r)
 
-def date(format :str = None, title :str = None):
+def date(format: str = None, title: str = None):
   '''Pick a date
 
     format - SimpleDateFormat (optional) eg "dd-MM-yyyy"
     title - set title of dialog (optional)
   '''
-  opts = ""
+  opts = []
   if format is not None:
-    opts += f'-d "{format}" '
+    opts += ["-d", format]
   if title is not None:
-    opts += f'-t "{title}"'
-  return execute(f"termux-dialog date {opts}")
+    opts += ["-t", title]
+  return execute(["termux-dialog", "date"] + opts)
 
 def time(title: str = None):
   '''Pick a time value
   
     title - set title of dialog (optional)
   '''
-  return __hintlike("time",hint = None,title = title)
+  return __hintlike("time", hint = None, title = title)
 
 
-def checkbox(opts: tuple, title :str = None):
+def checkbox(opts: tuple, title: str = None):
   '''Select multiple values using checkboxes
 
     opts - tuple of options to use (required)
     title - set title of dialog (optional)
   '''
-  return __radiolike('checkbox',opts,title)
+  return __radiolike('checkbox', opts, title)
 
-def radio(opts: tuple, title :str = None):
+def radio(opts: tuple, title: str = None):
   '''Pick a single value from radio buttons
 
     opts - tuple of options to use (required)
     title - set title of dialog (optional)
   '''
-  return __radiolike('radio',opts,title)
+  return __radiolike('radio', opts, title)
 
-def sheet(opts: tuple, title :str = None):
+def sheet(opts: tuple, title: str = None):
   '''Pick a value from sliding bottom sheet
 
     opts - tuple of options to use (required)
     title - set title of dialog (optional)
   '''
-  return __radiolike('sheet',opts,title)
+  return __radiolike('sheet', opts, title)
 
-def spinner(opts: tuple, title :str = None):
+def spinner(opts: tuple, title: str = None):
   '''Pick a single value from a dropdown spinner
 
     opts - tuple of options to use (required)
     title - set title of dialog (optional)
   '''
-  return __radiolike('spinner',opts,title)
+  return __radiolike('spinner', opts, title)
 
-def text(hint :str = None, multiline: bool = None, number: bool = None, password: bool = None, title :str = None):
+def text(hint: str = None, multiline: bool = None, number: bool = None, password: bool = None, title: str = None):
   '''Text input
 
     hint - text hint (optional)
     multiline - multiline input (optional)*
     number - number input (optional)*
     password - password input (optional)
     title - set title of dialog (optional)
 
     * cannot use together 
   '''
   if (multiline is not None) and (number is not None):
-    return "Cannot use multiline and number together" 
-  opts = ""
+    raise ValueError("Cannot use multiline and number together.")
+  opts = []
   if multiline is not None: 
-    opts += "-m "
+    opts.append("-m")
   if number is not None:
-    opts += "-n "
+    opts.append("-n")
   if password is not None:
-    opts += "-p "
+    opts.append("-p")
   if hint is not None:
-    opts += f'-i "{hint}" '
+    opts += ["-i", hint]
   if title is not None:
-    opts += f'-t "{title}"'
-  return execute(f"termux-dialog text {opts}")
+    opts += ["-t", title]
+  return execute("termux-dialog", "text", opts)
 
-def toast(text: str, bgcolor :str = None, color: str = None, position: str = None, short: bool = False):
-  '''Show a toast message
+def toast(text: str, short: bool = False, **kwargs):
+    '''Show a toast message
 
     text = Text to show toast
+    short = only show the toast for a short while (default: false)
     bgcolor = background color (default: gray)
     color = text color (default: white)
     position = [top, middle, or bottom] (default: middle)
-    short = only show the toast for a short while (default: false)
-  '''
-  opts = {
-    "bgcolor": "-b",
-    "color": "-c",
-    "position": "-g"
-  }
-
-  options = ""
-  for f in opts.keys():
-      if eval(f) is not None:
-          options += f"{opts[f]} {eval(f)} "
-
-  if short is not None:
-      options += "-s"
-
-  r = execute(f'termux-toast {options} "{text}"')
-  return r[1]
+    '''
+    params = {
+      "bgcolor": "b",
+      "color": "c",
+      "position": "g"
+    }
+    opts = []
+    for k,v in kwargs.items():
+        opts += ['-'+params[k], v]
+    if short:
+        opts.append("-s")
+    return execute(["termux-toast"] + opts + [text])
```

### Comparing `termux-api-1.2.3/termux/Wifi.py` & `termux-api-1.2.4/termux/Wifi.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 '''
 from .android import execute
 
 def on():
     '''
     Enable WiFi
     '''
-    return execute("termux-wifi-enable true")
+    return execute(["termux-wifi-enable", "true"])
 
 def off():
     '''
     Disable WiFi
     '''
-    return execute("termux-wifi-enable false")
+    return execute(["termux-wifi-enable", "false"])
 
 def info():
     '''
     Return wifi connection info (json format)
     '''
-    return execute(f"termux-wifi-connectioninfo")
+    return execute(["termux-wifi-connectioninfo"])
 
 def scaninfo():
     '''
     Return last wifi scan info (json format)
     '''
-    return execute(f"termux-wifi-scaninfo")
+    return execute(["termux-wifi-scaninfo"])
```

### Comparing `termux-api-1.2.3/termux/__init__.py` & `termux-api-1.2.4/termux/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-'''
-Termux API python wrapper
-
-Available modules are:
-  termux.API - Misc API methods, including generic call
-  termux.Camera
-  termux.Clipboard
-  termux.Media - Playback and media scanner
-  termux.Microphone
-  termux.Notification
-  termux.Scheduler - Job Scheduler
-  termux.Sensors
-  termux.Share
-  termux.Telephony - make call, info of device and network
-  termux.TTS - Text to speech
-  termux.UI - Dialog Widgets and Toast
-  termux.Wifi
-
-For information about available methods, use
-  help(termux.<modulename>)
-'''
-
-from . import API, Camera, Clipboard, Sensors, TTS, Wifi, Notification, Media, Microphone, Scheduler, Share, Telephony, UI
-
-
-__all__ = sorted(["API", "Sensors", "Camera", "Clipboard", "TTS", "Wifi", "Notification",
-                  "Media", "Microphone", "Scheduler", "Share", "Telephony", "UI"])
+'''
+Termux API python wrapper
+
+Available modules are:
+  termux.API - Misc API methods, including generic call
+  termux.Camera
+  termux.Clipboard
+  termux.Media - Playback and media scanner
+  termux.Microphone
+  termux.Notification
+  termux.Scheduler - Job Scheduler
+  termux.Sensors
+  termux.Share
+  termux.Telephony - make call, info of device and network
+  termux.TTS - Text to speech
+  termux.UI - Dialog Widgets and Toast
+  termux.Wifi
+  termux.Wake
+
+For information about available methods, use
+  help(termux.<modulename>)
+'''
+
+from . import API, Camera, Clipboard, Sensors, TTS, Wifi, Notification, Media, Microphone, Scheduler, Share, Telephony, UI, Wake
+
+
+__all__ = sorted(["API", "Sensors", "Camera", "Clipboard", "TTS", "Wifi", "Notification",
+                  "Media", "Microphone", "Scheduler", "Share", "Telephony", "UI", "Wake"])
```

### Comparing `termux-api-1.2.3/termux/android.py` & `termux-api-1.2.4/termux/android.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import subprocess, json
 from sys import stdout
-import shlex
 
 def liveSave(func: str, logfile: str = 'sensors.log'):
     """Display live data to the screen and
        saving the computed data to sensor.log file.
     """
     with open(logfile, 'wb') as f:
-        p = subprocess.Popen(func, stdout=subprocess.PIPE,shell=True)
+        p = subprocess.Popen(func, stdout=subprocess.PIPE)
         for c in iter(lambda: p.stdout.read(1), b''):
-            a=c.decode("utf-8") #to write to stdout needs to be decoded
+            a = c.decode("utf-8") #to write to stdout needs to be decoded
             stdout.write(a)
             f.write(c)    #needs to write in byte like format
 
 
-def execute(func: str, stdin: str = ""):
+def execute(func: list, stdin: str = ""):
     '''Interface to shell
 
     Returns:
         tuple: returnCode = 0 for success, > 0 error, -N for signal N
         output = string, JSON string or None
         err = error message or None
     '''
-    fSplit = shlex.split(func) # secure call
+    func = [str(i) if type(i) in (int, float) else i for i in func]
     p = subprocess.Popen(
-            fSplit,
+            func,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             shell=False,
             text=True)
     output, err = p.communicate(stdin)
     try:
```

### Comparing `termux-api-1.2.3/termux_api.egg-info/PKG-INFO` & `termux-api-1.2.4/termux_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termux-api
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package for accessing termux-api
 Home-page: https://github.com/shajul/termux-api.git
 Author: drshajul
 Author-email: drshajul@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 
 Most of the [termux-api implementations](https://wiki.termux.com/wiki/Termux:API) are directly available.
 The API.generic() method gives direct access to any other method that has not yet been implemented.
 
 ## Special thanks
 Thanks to termux and termux-api for making all this possible.
 This module is heavily inspired by https://github.com/azwyane/pimux, though the code has been 
-almost completely re-written and now is much more comprehensive.  
+almost completely re-written and now is much more comprehensive. Also, special thanks for recent contribution from [Young-Lord](https://github.com/Young-Lord)
 This project is originally located at [termux-api](https://github.com/shajul/termux-api)
 
 ## Table of Contents
 - [Requirements](#Requirements)
 - [Installation](#Installation)
 - [Features](#Features)
 - [Contributing](#Contributing)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: termux-api Version: 1.2.3 Summary: A package for
+Metadata-Version: 2.1 Name: termux-api Version: 1.2.4 Summary: A package for
 accessing termux-api Home-page: https://github.com/shajul/termux-api.git
 Author: drshajul Author-email: drshajul@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # termux-api [!
 [Build Status](http://img.shields.io/travis/badges/
 badgerbadgerbadger.svg?style=flat-square)](https://github.com/shajul/termux-
@@ -11,28 +11,30 @@
 API) This provides a way to get native access in Python to Android device
 functionality as API. Most of the [termux-api implementations](https://
 wiki.termux.com/wiki/Termux:API) are directly available. The API.generic()
 method gives direct access to any other method that has not yet been
 implemented. ## Special thanks Thanks to termux and termux-api for making all
 this possible. This module is heavily inspired by https://github.com/azwyane/
 pimux, though the code has been almost completely re-written and now is much
-more comprehensive. This project is originally located at [termux-api](https://
-github.com/shajul/termux-api) ## Table of Contents - [Requirements]
-(#Requirements) - [Installation](#Installation) - [Features](#Features) -
-[Contributing](#Contributing) ## Requirements - Termux app - Termux-api (both
-app and package) - Python installed in termux ($ pkg install python) ##
-Installation ð  Android install through termux: ### Method-1 **Install by
-pip** The stable version is available in the Pypi, which you can download by:
-``` $ python3 -m pip install termux-api ``` ### Method-2 You can always get the
-latest version of termux-api maintained here in the github. - Clone this repo
-to your local machine(termux) using `https://github.com/shajul/termux-api.git`
-Goto to your terminal and type: ```sh $ git clone https://github.com/shajul/
-termux-api.git $ python3 -m pip install wheel $ python3 -m pip install dist/
-termux_api*.whl ``` Or you can add this to site packages by first building it
-first: ``` $ python3 setup.py sdist bdist_wheel $ python3 -m pip install -e
+more comprehensive. Also, special thanks for recent contribution from [Young-
+Lord](https://github.com/Young-Lord) This project is originally located at
+[termux-api](https://github.com/shajul/termux-api) ## Table of Contents -
+[Requirements](#Requirements) - [Installation](#Installation) - [Features]
+(#Features) - [Contributing](#Contributing) ## Requirements - Termux app -
+Termux-api (both app and package) - Python installed in termux ($ pkg install
+python) ## Installation ð  Android install through termux: ### Method-
+1 **Install by pip** The stable version is available in the Pypi, which you can
+download by: ``` $ python3 -m pip install termux-api ``` ### Method-2 You can
+always get the latest version of termux-api maintained here in the github. -
+Clone this repo to your local machine(termux) using `https://github.com/shajul/
+termux-api.git` Goto to your terminal and type: ```sh $ git clone https://
+github.com/shajul/termux-api.git $ python3 -m pip install wheel $ python3 -
+m pip install dist/termux_api*.whl ``` Or you can add this to site packages by
+first building it first: ``` $ python3 setup.py sdist bdist_wheel $ python3 -
+m pip install -e
 .whl> ``` Finally, you have it installed. ## Run the project Now to run the
 termux-api type in your terminal: ```bash $ python >>> import termux >>>
 termux.API.vibrate() >>> help(termux.API) #for available methods ``` Avaliable
 modules are API, Camera, Clipboard, Media, Microphone, Notification, Scheduler,
 Sensors, Share, Telephony, TTS, UI, Wifi OR ```bash $ python >>> from termux
 import  >>> API.vibrate() >>> help(API) # for details of available methods ```
 ## Contributing ### Step 1 - Option 1 - ð´ Fork this repo! - Option 2 - ð¯
```

