# Comparing `tmp/wavinfo-2.2.0.tar.gz` & `tmp/wavinfo-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavinfo-2.2.0.tar", last modified: Sun Feb 26 19:45:23 2023, max compression
+gzip compressed data, was "wavinfo-2.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wavinfo-2.2.0.tar` & `wavinfo-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2545 2022-11-27 03:44:01.701497 wavinfo-2.2.0/README.md
--rw-r--r--   0        0        0     1666 2023-02-26 18:58:40.716641 wavinfo-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      202 2023-02-26 19:35:20.722899 wavinfo-2.2.0/wavinfo/__init__.py
--rw-r--r--   0        0        0     2250 2022-11-27 04:55:19.588942 wavinfo-2.2.0/wavinfo/__main__.py
--rw-r--r--   0        0        0     1418 2022-11-15 19:22:16.989962 wavinfo-2.2.0/wavinfo/rf64_parser.py
--rw-r--r--   0        0        0     2393 2022-11-24 02:47:21.965137 wavinfo-2.2.0/wavinfo/riff_parser.py
--rw-r--r--   0        0        0     3895 2022-11-17 05:00:21.799285 wavinfo-2.2.0/wavinfo/umid_parser.py
--rw-r--r--   0        0        0     6378 2022-11-27 03:28:24.069221 wavinfo-2.2.0/wavinfo/wave_adm_reader.py
--rw-r--r--   0        0        0     4291 2022-12-02 18:32:43.759387 wavinfo-2.2.0/wavinfo/wave_bext_reader.py
--rw-r--r--   0        0        0    18534 2022-11-27 03:31:47.044743 wavinfo-2.2.0/wavinfo/wave_dbmd_reader.py
--rw-r--r--   0        0        0     3541 2022-12-02 18:32:43.760550 wavinfo-2.2.0/wavinfo/wave_info_reader.py
--rw-r--r--   0        0        0     6122 2023-02-26 18:19:16.313061 wavinfo-2.2.0/wavinfo/wave_ixml_reader.py
--rw-r--r--   0        0        0     7221 2023-02-26 18:19:16.315339 wavinfo-2.2.0/wavinfo/wave_reader.py
--rw-r--r--   0        0        0      735 2022-11-27 05:05:41.558061 wavinfo-2.2.0/wavinfo/wavfind.py
--rw-r--r--   0        0        0     3576 1970-01-01 00:00:00.000000 wavinfo-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2547 2023-05-30 23:06:09.661719 wavinfo-2.2.1/README.md
+-rw-r--r--   0        0        0     1666 2023-05-30 23:06:09.661719 wavinfo-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/__main__.py
+-rw-r--r--   0        0        0     1418 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/rf64_parser.py
+-rw-r--r--   0        0        0     2393 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/riff_parser.py
+-rw-r--r--   0        0        0     3895 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/umid_parser.py
+-rw-r--r--   0        0        0     6378 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/wave_adm_reader.py
+-rw-r--r--   0        0        0     4291 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/wave_bext_reader.py
+-rw-r--r--   0        0        0    18534 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/wave_dbmd_reader.py
+-rw-r--r--   0        0        0     3541 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/wave_info_reader.py
+-rw-r--r--   0        0        0     6122 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/wave_ixml_reader.py
+-rw-r--r--   0        0        0     7221 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/wave_reader.py
+-rw-r--r--   0        0        0      735 2023-05-30 23:06:10.069746 wavinfo-2.2.1/wavinfo/wavfind.py
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 wavinfo-2.2.1/PKG-INFO
```

### Comparing `wavinfo-2.2.0/README.md` & `wavinfo-2.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
 * [Broadcast-WAVE][bext] metadata, including embedded program
   loudness, coding history and [SMPTE UMID][smpte_330m2011].
 * [ADM][adm] track metadata and schema, including channel, pack formats, object, content and programme.
 * [Dolby Digital Plus][ebu3285s6] and Dolby Atmos `dbmd` metadata.
 * [iXML][ixml] production recorder metadata, including project, scene, and take tags, recorder notes
   and file family information.
+  * iXML `STEINBERG` sound library attributes.
 * Most of the common [RIFF INFO][info-tags] metadata fields.
 * The __wav format__ is also parsed, so you can access the basic sample rate and channel count
   information.
 
 In progress:
 * Pro Tools __embedded regions__.
-* iXML `STEINBERG` sound library attributes.
 
 [bext]:https://wavinfo.readthedocs.io/en/latest/scopes/bext.html
 [smpte_330m2011]:https://wavinfo.readthedocs.io/en/latest/scopes/bext.html#wavinfo.wave_bext_reader.WavBextReader.umid
 [adm]:https://wavinfo.readthedocs.io/en/latest/scopes/adm.html
 [ebu3285s6]:https://wavinfo.readthedocs.io/en/latest/scopes/dolby.html
 [ixml]:https://wavinfo.readthedocs.io/en/latest/scopes/ixml.html
 [info-tags]:https://wavinfo.readthedocs.io/en/latest/scopes/info.html
```

### Comparing `wavinfo-2.2.0/pyproject.toml` & `wavinfo-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/__main__.py` & `wavinfo-2.2.1/wavinfo/__main__.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/rf64_parser.py` & `wavinfo-2.2.1/wavinfo/rf64_parser.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/riff_parser.py` & `wavinfo-2.2.1/wavinfo/riff_parser.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/umid_parser.py` & `wavinfo-2.2.1/wavinfo/umid_parser.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/wave_adm_reader.py` & `wavinfo-2.2.1/wavinfo/wave_adm_reader.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/wave_bext_reader.py` & `wavinfo-2.2.1/wavinfo/wave_bext_reader.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/wave_dbmd_reader.py` & `wavinfo-2.2.1/wavinfo/wave_dbmd_reader.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/wave_info_reader.py` & `wavinfo-2.2.1/wavinfo/wave_info_reader.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/wave_ixml_reader.py` & `wavinfo-2.2.1/wavinfo/wave_ixml_reader.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/wave_reader.py` & `wavinfo-2.2.1/wavinfo/wave_reader.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/wavinfo/wavfind.py` & `wavinfo-2.2.1/wavinfo/wavfind.py`

 * *Files identical despite different names*

### Comparing `wavinfo-2.2.0/PKG-INFO` & `wavinfo-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavinfo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Probe WAVE Files for iXML, Broadcast-WAVE and other metadata.
 Keywords: waveform,metadata,audio,ebu,smpte,avi,library,film,broadcast
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -37,21 +37,21 @@
 
 * [Broadcast-WAVE][bext] metadata, including embedded program
   loudness, coding history and [SMPTE UMID][smpte_330m2011].
 * [ADM][adm] track metadata and schema, including channel, pack formats, object, content and programme.
 * [Dolby Digital Plus][ebu3285s6] and Dolby Atmos `dbmd` metadata.
 * [iXML][ixml] production recorder metadata, including project, scene, and take tags, recorder notes
   and file family information.
+  * iXML `STEINBERG` sound library attributes.
 * Most of the common [RIFF INFO][info-tags] metadata fields.
 * The __wav format__ is also parsed, so you can access the basic sample rate and channel count
   information.
 
 In progress:
 * Pro Tools __embedded regions__.
-* iXML `STEINBERG` sound library attributes.
 
 [bext]:https://wavinfo.readthedocs.io/en/latest/scopes/bext.html
 [smpte_330m2011]:https://wavinfo.readthedocs.io/en/latest/scopes/bext.html#wavinfo.wave_bext_reader.WavBextReader.umid
 [adm]:https://wavinfo.readthedocs.io/en/latest/scopes/adm.html
 [ebu3285s6]:https://wavinfo.readthedocs.io/en/latest/scopes/dolby.html
 [ixml]:https://wavinfo.readthedocs.io/en/latest/scopes/ixml.html
 [info-tags]:https://wavinfo.readthedocs.io/en/latest/scopes/info.html
```

