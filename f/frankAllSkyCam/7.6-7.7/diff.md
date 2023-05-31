# Comparing `tmp/frankAllSkyCam-7.6.tar.gz` & `tmp/frankAllSkyCam-7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-7.6.tar", last modified: Fri May 26 14:13:34 2023, max compression
+gzip compressed data, was "frankAllSkyCam-7.7.tar", last modified: Wed May 31 20:59:12 2023, max compression
```

## Comparing `frankAllSkyCam-7.6.tar` & `frankAllSkyCam-7.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-26 14:13:34.512561 frankAllSkyCam-7.6/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-05-26 14:13:34.512561 frankAllSkyCam-7.6/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-26 14:13:34.512561 frankAllSkyCam-7.6/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-05-26 14:08:50.402887 frankAllSkyCam-7.6/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3825 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-05-26 14:08:09.723223 frankAllSkyCam-7.6/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3419 2023-05-26 14:08:09.723223 frankAllSkyCam-7.6/frankAllSkyCam/config.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-05-26 14:08:09.723223 frankAllSkyCam-7.6/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     1830 2023-05-26 14:08:09.723223 frankAllSkyCam-7.6/frankAllSkyCam/drawtext.py
--rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/exposurecalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/fileManager.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/index.py
--rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/sqmexp.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)    16387 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/sqmreader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-05-26 14:08:09.727223 frankAllSkyCam-7.6/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-7.6/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1845 2023-05-26 07:24:08.764028 frankAllSkyCam-7.6/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-31 20:59:12.263035 frankAllSkyCam-7.7/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-05-31 20:59:12.263035 frankAllSkyCam-7.7/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-31 20:59:12.263035 frankAllSkyCam-7.7/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-05-31 18:24:49.869152 frankAllSkyCam-7.7/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4534 2023-05-31 18:21:22.019090 frankAllSkyCam-7.7/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-05-31 18:21:22.011090 frankAllSkyCam-7.7/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3058 2023-05-31 18:21:22.011090 frankAllSkyCam-7.7/frankAllSkyCam/config.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-05-31 18:21:22.011090 frankAllSkyCam-7.7/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2232 2023-05-31 18:21:22.015090 frankAllSkyCam-7.7/frankAllSkyCam/drawtext.py
+-rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-05-31 18:21:22.015090 frankAllSkyCam-7.7/frankAllSkyCam/exposurecalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-05-31 18:21:22.015090 frankAllSkyCam-7.7/frankAllSkyCam/fileManager.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2823 2023-05-31 18:21:22.015090 frankAllSkyCam-7.7/frankAllSkyCam/getextdata.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-05-31 18:21:22.015090 frankAllSkyCam-7.7/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-05-31 18:21:22.015090 frankAllSkyCam-7.7/frankAllSkyCam/index.py
+-rwxr--r--   0 pi        (1000) pi        (1000)     1068 2023-05-31 18:21:22.019090 frankAllSkyCam-7.7/frankAllSkyCam/shelly_temp.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-05-31 18:21:22.019090 frankAllSkyCam-7.7/frankAllSkyCam/sqmexp.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)    16387 2023-05-31 18:21:22.019090 frankAllSkyCam-7.7/frankAllSkyCam/sqmreader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-05-31 18:21:22.019090 frankAllSkyCam-7.7/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-05-31 18:21:22.023090 frankAllSkyCam-7.7/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-05-31 18:21:22.023090 frankAllSkyCam-7.7/frankAllSkyCam/test_sqm.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-05-31 18:21:22.023090 frankAllSkyCam-7.7/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-05-31 18:21:22.023090 frankAllSkyCam-7.7/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-05-31 18:21:22.023090 frankAllSkyCam-7.7/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-7.7/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-05-31 18:24:36.593276 frankAllSkyCam-7.7/setup.py
```

### Comparing `frankAllSkyCam-7.6/PKG-INFO` & `frankAllSkyCam-7.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 7.6
+Version: 7.7
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/7.6.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/7.7.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/__main__.py` & `frankAllSkyCam-7.7/frankAllSkyCam/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import datetime
 from fractions import Fraction
 import time
 from pytz import timezone
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
-from frankAllSkyCam import imageHeader, fileManager, drawtext
+from frankAllSkyCam import imageHeader, fileManager, drawtext, getextdata
 
 config = ConfigParser()
 configFileName = fileManager.getConfigFileName()
 config.read(configFileName)
 appPath = os.path.expanduser("~") + "/frankAllSkyCam/"
 
 time_zone = str(config['site']['time_zone'])
@@ -27,20 +27,30 @@
 horiz = str(config['resolution']['horiz'])
 vert = str(config['resolution']['vert'])
 rotation = int(config['resolution']['picture_rotation'])
 picture_rotation = str(config['resolution']['picture_rotation'])
 
 additional_params = str(config['libcamera']['additional_params'])
 
-font_size = int(config['font']['font_size'])
+font_size   = int(config['font']['font_size'])
 font_colorR = int(config['font']['font_colorR'])
 font_colorG = int(config['font']['font_colorG'])
 font_colorB = int(config['font']['font_colorB'])
 font_color = [font_colorR,font_colorG,font_colorB]
 
+et_use         = str(config['extra_text']['et_use'])
+et_x_pos       = int(config['extra_text']['et_x_pos'])
+et_y_pos       = int(config['extra_text']['et_y_pos'])
+et_font_size   = int(config['extra_text']['et_font_size'])
+et_font_colorR = int(config['extra_text']['et_font_colorR'])
+et_font_colorG = int(config['extra_text']['et_font_colorG'])
+et_font_colorB = int(config['extra_text']['et_font_colorB'])
+et_font_color = [et_font_colorR,et_font_colorG,et_font_colorB]
+
+
 sqm_le = config['sqm']['use_sqm_le']
 
 isFTP = str(config['ftp']['isFTP'])=='True'
 FTP_server = str(config['ftp']['FTP_server'])
 FTP_login = str(config['ftp']['FTP_login'])
 FTP_pass = str(config['ftp']['FTP_pass'])
 FTP_uploadFolder = str(config['ftp']['FTP_uploadFolder'])
@@ -91,16 +101,23 @@
        print(killcmd)
 
        #launch the command line
        print(command)
        os.system(command)
 
        print("Image captured")
+
+       extra_text = [""]
+       if et_use =="y":
+          #extra_text needed
+          extra_string = getextdata.getData()
+          extra_text = [extra_string, et_font_size, et_font_color, et_x_pos, et_y_pos]
+
        # print watermark
-       drawtext.printWatermark(s, jpg_file_name, font_size, font_color, sqm_le, rotation)
+       drawtext.printWatermark(s, jpg_file_name, font_size, font_color, sqm_le, rotation, extra_text)
 
        #generate /update alive.txt to say we are still alive
        textcommand = "touch " + logFolder +  "/alive.txt"
        os.system(textcommand)
 
        pass
     except:
```

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-7.7/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/config.py` & `frankAllSkyCam-7.7/frankAllSkyCam/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 ########################################
 # frankAllSkyCam
 # configuration file -  config.txt
 #
 # please adjust according to your needs
-# see inline comments and documentation
+# see comments and documentation
 ########################################
 
 [system]
 # where will be stored images - relative path to frankAllSkyCam
 otuputFolder= img
 
 # directory where to save logs
 logFolder = log
 
-# local web folder in which the allSyCam picture will be generated
-# in case of apache webserver, you can use this:
-#outputLocalWebFile = /var/www/html/img/skycam.jpg
-outputLocalWebFile = /home/pi/frankAllSkyCam/skycam.jpg
+# local web folder where to save the skycam.jpg
+outputLocalWebFile = /var/www/html/img/skycam.jpg
 
 #how many days you want to keep jpgs
-# after #days_retention days, the folder /home/pi/frankAllSkyCam/img/yyyyMMdd will be removed
 days_retention = 3
 
-#watchdog will reboot if after xx minutes no <outputLocalWebFile> image has been generated
+#watchdog will reboot if after x minutes no image has been generated
 rebootAfter = 15
 
 [site]
 #the following label will be printed on the image
 inte = www.astrobrallo.com
 latitude = 44.73
 longitude = 9.31
-# select the timezone according to pytz timezones list (google it)
 time_zone = Europe/Rome
 
 [resolution]
 # may use  1024 x 768
 horiz = 800
 vert = 600
-
-# picture rotation (degrees)
 picture_rotation = 0
 
 [libcamera]
 # may personalize the libcamara params.
-# please DO NOT set: -o, -n, --height, --width, --meter average, --shutter, --immediate
+# please DO NOT set --shutter, --immediate
 # parameters will be used only when exposure > 0
-additional_params = --gain 18 --awbgains 2.2,1.8
+additional_params = --gain 14 --awbgains 2.2,1.6 --contrast 1.5
+
 
 [timelapse]
 # if True, timelapse from sunset to sunrise will be generated  Otherwise, not.
 nightTL = True
 
 # if True, 24h timelapse from 9am to 9am next day will be generated. Otherwise, not.
 fullTL = True
@@ -67,54 +62,63 @@
 [font]
 #when 1024x768 you can increase it
 font_size = 18
 font_colorR = 0
 font_colorG = 255
 font_colorB = 255
 
+[extra_text]
+et_use= n
+et_font_size = 18
+et_font_colorR = 0
+et_font_colorG = 255
+et_font_colorB = 255
+et_x_pos = 5
+et_y_pos = 80
+
+
 [exposure]
 # max night exposure in seconds
-#    for urban sky, suggested value is 4
-#    for dark sky, suggested value is 55-60 (I found 55 secs ok for sqm 21,3).
+#  for urban sky, suggested value is 4
+#  for dark sky, suggested value is 55-60 (I found 55 secs ok for sqm 21,3).
+#  this value only limits the max exposure. The calculated or real SQM will drive exposure
 esp_secs =60
 
 [offset]
-# offset dawn and dusk in minutes
+# minutes to offset dawn and dusk for optimal exposure
 dawn = 0
 dusk = 0
 
 [ftp]
 # if True, allSkyCam image, timelapse and startrails
 #will be uploaded on your FTP Server
 isFTP=False
 
-# ftp server parameters
-FTP_server=yourFTP.com
-FTP_login=yourusername
-FTP_pass=yourpass
-FTP_uploadFolder =/images/allsky
+# ftp parameters, to upload the allSkyCam image to your FTP server
+FTP_server=yourftpserver.com
+FTP_login=username
+FTP_pass=password
+FTP_uploadFolder =/public_html
 
-# filename (.jpg will be automatically added)
-FTP_filenameAllSkyImgJPG = allskycam
+# uploaded file name (e.g.,allskycam.jpg)
+FTP_filenameAllSkyImgJPG = img/allskycam
 
 # allskycam_night.mp4 will be generated if nightTL = True
 # allskycam_24h.mp4 will be generated if fullTL = True
-# current setting: timelapse will be uploaded in /videos/frankAllSkyCam/
-FTP_fileNameTimelapseMP4 = /videos/frankAllSkycam
+FTP_fileNameTimelapseMP4 = /video/frankAllSkycam
 
-# starTrail.jpg will be generated in the following position
-# every day a new startrail image will overwrite the previous image
-FTP_fileNameStarTrailJPG = /startrails/starTrail.jpg
+# starTrail.jpg will be generated
+FTP_fileNameStarTrailJPG = /startrail/startrail.jpg
 
 [sqm]
-# directory where to save sqm info. It will be under the frankAllSkyCam
+# directory where to save sqm info
 sqmFolder = sqm
 # would you use the SQM-LE ? y/n
 use_sqm_le = n
-# would you log your SQM values ? y/n - THIS LOG WILL NOT BE ROTATED ! PAY ATTENTION TO FILE SIZE
+# would you log your SQM ? y/n
 sqmLog = n
 # keep sqmDebug = n
 sqmDebug = n
 # in case you have SQM-LE, put your IP/port
 ip_address = 192.168.2.59
 port = 10001
```

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/crontab.py` & `frankAllSkyCam-7.7/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-7.7/frankAllSkyCam/drawtext.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 
 from PIL import Image
 from PIL import ImageFont
 from PIL import ImageDraw
 
 
-def printWatermark(s, nomefile, font_size, fc, sqm_le, rotation):
+def printWatermark(s, nomefile, font_size, fc, sqm_le, rotation, extra_text):
     data      = s[0]
     ora       = s[1]
     inte      = s[2]
     TL        = s[4]
     moon_rise = s[5]
     moon_set  = s[6]
     srise     = s[7]
@@ -63,9 +63,26 @@
     stringa = "Night Start "+ NS +"\nNight End "+ NE + stringa_sqm + str(round(sqm,2))
     drawing.text(pos, stringa, fill=colore, font=font)
 
     pos=(630,535)
     stringa = "Moonrise " + moon_rise + "\nMoonset " + moon_set + "\n" + str(fract) + "% | " + phase
     drawing.text(pos, stringa, fill=colore, font=font)
 
+    if len(extra_text) > 1:
+
+       et_pos=(extra_text[3],extra_text[4])
+       et_stringa = extra_text[0]
+
+       et_colore =(extra_text[2][0],extra_text[2][1],extra_text[2][2])
+
+       if sqm>18:
+          et_colore = colore
+
+       et_font = ImageFont.truetype("DejaVuSerif.ttf", extra_text[1])
+       drawing.text(et_pos, et_stringa, fill=et_colore, font=et_font)
+
+
+
     photo.save(nomefile)
     return
+
+
```

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/exposurecalc.py` & `frankAllSkyCam-7.7/frankAllSkyCam/exposurecalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-7.7/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-7.7/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/sqmreader.py` & `frankAllSkyCam-7.7/frankAllSkyCam/sqmreader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/startrail.py` & `frankAllSkyCam-7.7/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-7.7/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/test_sqm.py` & `frankAllSkyCam-7.7/frankAllSkyCam/test_sqm.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-7.7/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-7.7/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.6/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-7.7/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

