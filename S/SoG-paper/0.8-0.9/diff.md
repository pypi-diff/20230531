# Comparing `tmp/SoG-paper-0.8.tar.gz` & `tmp/SoG-paper-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SoG-paper-0.8.tar", last modified: Wed Aug  3 21:43:55 2022, max compression
+gzip compressed data, was "SoG-paper-0.9.tar", last modified: Thu Aug  4 17:52:44 2022, max compression
```

## Comparing `SoG-paper-0.8.tar` & `SoG-paper-0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-03 21:43:55.291852 SoG-paper-0.8/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      246 2022-07-20 13:48:06.000000 SoG-paper-0.8/.gitlab-ci.yml
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      948 2022-08-03 21:42:52.000000 SoG-paper-0.8/CHANGES.rst
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    34478 2022-07-20 20:15:53.000000 SoG-paper-0.8/LICENSE
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      229 2022-07-19 21:04:43.000000 SoG-paper-0.8/MANIFEST.in
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      622 2022-08-03 21:43:55.291677 SoG-paper-0.8/PKG-INFO
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     1176 2019-06-19 21:33:24.000000 SoG-paper-0.8/README.md
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-03 21:43:55.284201 SoG-paper-0.8/SoG/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)       55 2022-07-21 20:21:16.000000 SoG-paper-0.8/SoG/__init__.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-03 21:43:55.284859 SoG-paper-0.8/SoG/test/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    25799 2019-07-03 01:14:15.000000 SoG-paper-0.8/SoG/test/SoG_manuscript_generator_test.ipynb
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    16617 2022-07-18 19:50:13.000000 SoG-paper-0.8/SoG/test/SoG_manuscript_generator_test.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-03 21:43:55.285682 SoG-paper-0.8/SoG/test/files/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     6148 2022-07-20 00:08:42.000000 SoG-paper-0.8/SoG/test/files/.DS_Store
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     2186 2022-07-19 20:34:11.000000 SoG-paper-0.8/SoG/test/files/macro_GW_GRB.tex
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-03 21:43:55.286222 SoG-paper-0.8/SoG/tex/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-07-21 20:00:09.000000 SoG-paper-0.8/SoG/tex/__init__.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-03 21:43:55.289785 SoG-paper-0.8/SoG/tex/files/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)   137428 2022-07-19 15:42:57.000000 SoG-paper-0.8/SoG/tex/files/LSC_Aug2017_Virgo_Aug2017_GBM_SPIACS-aas.tex
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    20348 2022-07-19 18:34:12.000000 SoG-paper-0.8/SoG/tex/files/SoG_LIV.bib
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    22354 2022-08-03 20:03:44.000000 SoG-paper-0.8/SoG/tex/files/SoG_LIV_arxiv_aps.tex
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     5855 2019-06-19 21:33:24.000000 SoG-paper-0.8/SoG/tex/files/aas_macros.sty
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    35165 2021-07-08 21:13:48.000000 SoG-paper-0.8/SoG/tex/files/aip.bst
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     1299 2022-07-19 15:43:35.000000 SoG-paper-0.8/SoG/tex/files/notation_macros.tex
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    15681 2022-07-24 03:12:31.000000 SoG-paper-0.8/SoG/tex/files/ulem.sty
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    22060 2022-08-03 20:03:42.000000 SoG-paper-0.8/SoG/tex/generate_upload_pdf.py
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-03 21:43:55.290720 SoG-paper-0.8/SoG_paper.egg-info/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      622 2022-08-03 21:43:54.000000 SoG-paper-0.8/SoG_paper.egg-info/PKG-INFO
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      777 2022-08-03 21:43:55.000000 SoG-paper-0.8/SoG_paper.egg-info/SOURCES.txt
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        1 2022-08-03 21:43:54.000000 SoG-paper-0.8/SoG_paper.egg-info/dependency_links.txt
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        4 2022-08-03 21:43:55.000000 SoG-paper-0.8/SoG_paper.egg-info/namespace_packages.txt
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      130 2022-08-03 21:43:55.000000 SoG-paper-0.8/SoG_paper.egg-info/requires.txt
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        4 2022-08-03 21:43:55.000000 SoG-paper-0.8/SoG_paper.egg-info/top_level.txt
-drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-03 21:43:55.291410 SoG-paper-0.8/bin/
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     6148 2022-07-19 20:11:36.000000 SoG-paper-0.8/bin/.DS_Store
--rwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)     2427 2022-07-21 19:34:36.000000 SoG-paper-0.8/bin/SoG_generate_pdf
--rwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)     2428 2022-07-21 19:34:38.000000 SoG-paper-0.8/bin/SoG_upload_pdf
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)       38 2022-08-03 21:43:55.291902 SoG-paper-0.8/setup.cfg
--rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     2109 2022-08-03 20:03:38.000000 SoG-paper-0.8/setup.py
+drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-04 17:52:44.240858 SoG-paper-0.9/
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      246 2022-07-20 13:48:06.000000 SoG-paper-0.9/.gitlab-ci.yml
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     1110 2022-08-04 17:21:57.000000 SoG-paper-0.9/CHANGES.rst
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    34478 2022-07-20 20:15:53.000000 SoG-paper-0.9/LICENSE
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      229 2022-07-19 21:04:43.000000 SoG-paper-0.9/MANIFEST.in
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      622 2022-08-04 17:52:44.240620 SoG-paper-0.9/PKG-INFO
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     1176 2019-06-19 21:33:24.000000 SoG-paper-0.9/README.md
+drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-04 17:52:44.234468 SoG-paper-0.9/SoG/
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)       55 2022-07-21 20:21:16.000000 SoG-paper-0.9/SoG/__init__.py
+drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-04 17:52:44.235178 SoG-paper-0.9/SoG/test/
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    25799 2019-07-03 01:14:15.000000 SoG-paper-0.9/SoG/test/SoG_manuscript_generator_test.ipynb
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    16617 2022-07-18 19:50:13.000000 SoG-paper-0.9/SoG/test/SoG_manuscript_generator_test.py
+drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-04 17:52:44.236194 SoG-paper-0.9/SoG/test/files/
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     6148 2022-07-20 00:08:42.000000 SoG-paper-0.9/SoG/test/files/.DS_Store
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     2186 2022-07-19 20:34:11.000000 SoG-paper-0.9/SoG/test/files/macro_GW_GRB.tex
+drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-04 17:52:44.236556 SoG-paper-0.9/SoG/tex/
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-07-21 20:00:09.000000 SoG-paper-0.9/SoG/tex/__init__.py
+drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-04 17:52:44.238928 SoG-paper-0.9/SoG/tex/files/
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)   137428 2022-07-19 15:42:57.000000 SoG-paper-0.9/SoG/tex/files/LSC_Aug2017_Virgo_Aug2017_GBM_SPIACS-aas.tex
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    20348 2022-07-19 18:34:12.000000 SoG-paper-0.9/SoG/tex/files/SoG_LIV.bib
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    22354 2022-08-03 20:03:44.000000 SoG-paper-0.9/SoG/tex/files/SoG_LIV_arxiv_aps.tex
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     5855 2019-06-19 21:33:24.000000 SoG-paper-0.9/SoG/tex/files/aas_macros.sty
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    35165 2021-07-08 21:13:48.000000 SoG-paper-0.9/SoG/tex/files/aip.bst
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     1299 2022-07-19 15:43:35.000000 SoG-paper-0.9/SoG/tex/files/notation_macros.tex
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    15681 2022-07-24 03:12:31.000000 SoG-paper-0.9/SoG/tex/files/ulem.sty
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)    21739 2022-08-04 17:22:10.000000 SoG-paper-0.9/SoG/tex/generate_upload_pdf.py
+drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-04 17:52:44.239697 SoG-paper-0.9/SoG_paper.egg-info/
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      622 2022-08-04 17:52:43.000000 SoG-paper-0.9/SoG_paper.egg-info/PKG-INFO
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      777 2022-08-04 17:52:44.000000 SoG-paper-0.9/SoG_paper.egg-info/SOURCES.txt
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        1 2022-08-04 17:52:43.000000 SoG-paper-0.9/SoG_paper.egg-info/dependency_links.txt
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        4 2022-08-04 17:52:43.000000 SoG-paper-0.9/SoG_paper.egg-info/namespace_packages.txt
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)      117 2022-08-04 17:52:43.000000 SoG-paper-0.9/SoG_paper.egg-info/requires.txt
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)        4 2022-08-04 17:52:43.000000 SoG-paper-0.9/SoG_paper.egg-info/top_level.txt
+drwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)        0 2022-08-04 17:52:44.240285 SoG-paper-0.9/bin/
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     6148 2022-07-19 20:11:36.000000 SoG-paper-0.9/bin/.DS_Store
+-rwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)     2591 2022-08-04 17:22:09.000000 SoG-paper-0.9/bin/SoG_generate_pdf
+-rwxr-xr-x   0 brandonpiotrzkowski   (502) staff       (20)     2593 2022-08-04 17:22:08.000000 SoG-paper-0.9/bin/SoG_upload_pdf
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)       38 2022-08-04 17:52:44.240907 SoG-paper-0.9/setup.cfg
+-rw-r--r--   0 brandonpiotrzkowski   (502) staff       (20)     2085 2022-08-04 17:22:07.000000 SoG-paper-0.9/setup.py
```

### Comparing `SoG-paper-0.8/LICENSE` & `SoG-paper-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/PKG-INFO` & `SoG-paper-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SoG-paper
-Version: 0.8
+Version: 0.9
 Summary: Low-latency manuscript of speed of gravity measurement
 Home-page: https://git.ligo.org/olivier.minazzoli/sog_liv_manuscript_template
 Author: Brandon Piotrzkowski
 Author-email: brandon.piotrzkowski@ligo.org
 License: GNU General Public License Version 3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SoG-paper-0.8/README.md` & `SoG-paper-0.9/README.md`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/test/SoG_manuscript_generator_test.ipynb` & `SoG-paper-0.9/SoG/test/SoG_manuscript_generator_test.ipynb`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/test/SoG_manuscript_generator_test.py` & `SoG-paper-0.9/SoG/test/SoG_manuscript_generator_test.py`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/test/files/.DS_Store` & `SoG-paper-0.9/SoG/test/files/.DS_Store`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/test/files/macro_GW_GRB.tex` & `SoG-paper-0.9/SoG/test/files/macro_GW_GRB.tex`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/tex/files/LSC_Aug2017_Virgo_Aug2017_GBM_SPIACS-aas.tex` & `SoG-paper-0.9/SoG/tex/files/LSC_Aug2017_Virgo_Aug2017_GBM_SPIACS-aas.tex`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/tex/files/SoG_LIV.bib` & `SoG-paper-0.9/SoG/tex/files/SoG_LIV.bib`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/tex/files/SoG_LIV_arxiv_aps.tex` & `SoG-paper-0.9/SoG/tex/files/SoG_LIV_arxiv_aps.tex`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/tex/files/aas_macros.sty` & `SoG-paper-0.9/SoG/tex/files/aas_macros.sty`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/tex/files/aip.bst` & `SoG-paper-0.9/SoG/tex/files/aip.bst`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/tex/files/notation_macros.tex` & `SoG-paper-0.9/SoG/tex/files/notation_macros.tex`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/tex/files/ulem.sty` & `SoG-paper-0.9/SoG/tex/files/ulem.sty`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/SoG/tex/generate_upload_pdf.py` & `SoG-paper-0.9/SoG/tex/generate_upload_pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 from astropy.cosmology import z_at_value
 from astropy.time import Time
 from astropy.utils.data import download_file
 from datetime import date, datetime, timedelta
 import gcn
 from gracedb_sdk import Client
 import healpy as hp
-from ligo.gracedb.rest import GraceDb
 from ligo.raven import search
 import ligo.skymap.distance
 from ligo.skymap.io import fits
 import lxml.etree
 import numpy as np
 from scipy.special import sph_harm, erfinv
 from tqdm import tqdm
 
 
 #  Get path to working directory
 path = os.path.dirname(os.path.abspath(__file__)) + '/files/'
 
+
 def p_value_from_skymaps(skymap_1, skymap_2, n_background=100):
     """Calculate probability of sky maps being from a random coincidence
        using the sky map overlap integral as an intermediate statistic. 
     
     Parameters
     ----------
     skymap_1: array
@@ -84,55 +84,58 @@
         overlap = search.skymap_overlap_integral(skymap_1['PROBDENSITY'],
                                                  skymap_2_rot,
                                                  se_skymap_uniq=skymap_1['UNIQ'])
         overlaps.append(overlap)
     
     return p_value(real_overlap, overlaps)
 
-def generate_macrofile(superevent_id, gracedb_url='https://gracedb.ligo.org/api/'):
+
+def generate_macrofile(superevent_id, gracedb=None):
     """Create macrofile that contains relevant data from superevent
        and preferred external event, to be potentially used to generate
        the pdf of the manuscript.
     
     Parameters
     ----------
     superevent_id: str
         GraceDB ID of the superevent
-    gracedb_url: str
-        URL of the GraceDB server's API e.g. https://gracedb.ligo.org/api/
+    gracedb: str
+        SDK REST API client
     """
 
-    #  Set up APIs for both the REST and sdk clients
-    gracedb_api = GraceDb(gracedb_url)
-    gracedb_sdk = Client(gracedb_url)
-    superevent = gracedb_api.superevent(superevent_id).json()
+    #  Initiate instance of GraceDb if not given
+    if gracedb is None:
+        gracedb = Client()
+
+    #  Grab superevent
+    superevent = gracedb.superevents[superevent_id].get()
 
     #  Grab latest voevent   
-    voevent_url = gracedb_sdk.superevents[superevent_id].voevents.get()[-1]['links']['file']
-    voevent_payload = gracedb_sdk.superevents[superevent_id].files[voevent_url.split('/')[-1]].get()
+    voevent_url = gracedb.superevents[superevent_id].voevents.get()[-1]['links']['file']
+    voevent_payload = gracedb.superevents[superevent_id].files[voevent_url.split('/')[-1]].get()
     root = lxml.etree.fromstring(voevent_payload.read())
 
     params = {elem.attrib['name']:
                 elem.attrib['value']
                 for elem in root.iterfind('.//Param')}
 
     #  Extract skymap
     if 'skymap_fits' in params:
         #  Read the HEALPix sky map and the FITS header.
         kwargs = {'mode': 'w+b'}
         #  Load multi-ordered sky map
         skyfilename = params['skymap_fits'].split('/')[-1].replace('fits.gz', 'multiorder.fits')
         with tempfile.NamedTemporaryFile(**kwargs) as skymapfile:
-            skymap_raw = gracedb_sdk.events[superevent_id].files[skyfilename].get()
+            skymap_raw = gracedb.events[superevent_id].files[skyfilename].get()
             skymapfile.write(skymap_raw.read())
             skymap_multi = fits.read_sky_map(skymapfile.name, moc=True)
         #  Load flattened sky maps
         skyfilename = params['skymap_fits'].split('/')[-1].replace('multiorder.fits', 'fits.gz')
         with tempfile.NamedTemporaryFile(**kwargs) as skymapfile:
-            skymap_raw = gracedb_sdk.events[superevent_id].files[skyfilename].get()
+            skymap_raw = gracedb.events[superevent_id].files[skyfilename].get()
             skymapfile.write(skymap_raw.read())
             skymap, header = hp.read_map(skymapfile.name, h=True)
             prob, distmu, distsigma, distnorm = hp.read_map(skymapfile.name, field = [0, 1, 2, 3])
         
     else:
         sys.exit('No skymap available')
         
@@ -284,29 +287,29 @@
     else:
         print('\\newcommand{\\pipesup}{\\issue{Pipeline}}\n', file = f)
 
     #  Grab external event
     emevent_id = superevent['em_type']
     FAR_GW = superevent['far']
         
-    external_event = gracedb_api.event(emevent_id).json()
+    external_event = gracedb.events[emevent_id].get()
     em_GPS_time = external_event['gpstime'] 
     EM_observer = external_event['extra_attributes']['GRB']['how_description']
     GRBevent = external_event['graceid']
     em_pipeline = external_event['pipeline']
     dto = em_GPS_time - t0_GPS
 
     print('\\newcommand{\\partners}{\\raven{%s}}' % (EM_observer), file = f) # Name of who made the GRB detection
 
     if 'skymap_fits' in params:
         # Read the HEALPix sky map and the FITS header.
         ext_skyfilename = em_pipeline.lower() + '_skymap.fits.gz'
         kwargs = {'mode': 'w+b'}
         with tempfile.NamedTemporaryFile(**kwargs) as skymapfile:
-            skymap_raw = gracedb_sdk.events[emevent_id].files[ext_skyfilename].get()
+            skymap_raw = gracedb.events[emevent_id].files[ext_skyfilename].get()
             skymapfile.write(skymap_raw.read())
             skymapfile.flush()
             skymapfile.seek(0)
             try:
                 ext_skymap, header = fits.read_sky_map(skymapfile.name)
             except KeyError:
                 ext_skymap, header = hp.read_map(skymapfile.name, h=True)
@@ -385,39 +388,39 @@
     print('\\newcommand{\\saal}{\\raven{%.0f \\times 10^{%.0i} }}' % (nbbmin_base, nbbmin_exp), file = f)
     print('\\newcommand{\\mTdelay}{\\raven{%.2f}}' % (dto), file = f)
     print('\\newcommand{\\deltaTdelay}{\\issue{%.2f}}' % (dterror), file = f)
 
     f.close()
 
 
-def generate_pdf(superevent_id, gracedb_url='https://gracedb.ligo.org/api/',
+def generate_pdf(superevent_id, gracedb=None,
                  keep_local_copy=False, compress_files=False,
                  use_latexmk=True, use_test_macrofile=False):
     """Generate pdf of manuscript using macrofile.
     
     Parameters
     ----------
     superevent_id: str
         GraceDB ID of the superevent
-    gracedb_url: str
-        URL of the GraceDB server's API e.g. https://gracedb.ligo.org/api/
+    gracedb: str
+        SDK REST API client
     keep_local_copy: bool
         If True, keeps copy of pdf in local directory
     compress_files: bool
         If True, creates and tarball of all files
     use_latemk: bool
         If True, uses latexmk instead of pdflatex to generate pdf
     use_test_macrofile: bool
         If True, uses local test copy of macro file rather than querying GraceDB
     """
 
     #  Create macrofile to generate manusrcipt from 
     if not use_test_macrofile:
         #  Query GraceDB to generate macrofile
-        generate_macrofile(superevent_id, gracedb_url=gracedb_url)
+        generate_macrofile(superevent_id, gracedb=gracedb)
     else:
         #  Use macrofile from test
         print(path)
         commandLine = subprocess.Popen(['cp', '../../test/files/macro_GW_GRB.tex', '.'], cwd=path)
         commandLine.communicate()
 
     if use_latexmk:
@@ -454,60 +457,61 @@
     os.unlink(path + 'SoG_LIV_arxiv_aps.aux')
     os.unlink(path + 'SoG_LIV_arxiv_aps.out')
     os.unlink(path + 'SoG_LIV_arxiv_aps.bbl')
     os.unlink(path + 'SoG_LIV_arxiv_aps.blg')
     os.unlink(path + 'SoG_LIV_arxiv_apsNotes.bib')
     
 
-def upload_pdf(superevent_id, gracedb_url='https://gracedb.ligo.org/api/',
+def upload_pdf(superevent_id, gracedb=None,
                keep_local_copy=False, compress_files=False,  
                use_latexmk=True, use_test_macrofile=False):
     """Generate and upload pdf to superevent.
     
     Parameters
     ----------
     superevent_id: str
         GraceDB ID of the superevent
-    gracedb_url: str
-        URL of the GraceDB server's API e.g. https://gracedb.ligo.org/api/
+    gracedb: str
+        SDK REST API client
     keep_local_copy: bool
         If True, keeps copy of pdf (and tarball of files if compressed) in local directory
     compress_files: bool
         If True, creates and uploads tarball of all files
     use_latemk: bool
         If True, uses latexmk instead of pdflatex to generate pdf
     use_test_macrofile: bool
         If True, uses local test copy of macro file rather than querying GraceDB
     """
     
     #  Create manuscript
-    generate_pdf(superevent_id, gracedb_url=gracedb_url,
+    generate_pdf(superevent_id, gracedb=gracedb,
                  keep_local_copy=keep_local_copy,
                  compress_files=compress_files,
                  use_test_macrofile=use_test_macrofile)
 
-    #  Prepare gracedb client to upload to
-    gracedb_sdk = Client(gracedb_url)
+    #  Initiate instance of GraceDb if not given
+    if gracedb is None:
+        gracedb = Client()
 
     #  Open and upload pdf file to gracedb superevent
     with open(path + 'SoG_LIV_arxiv_aps.pdf', 'rb') as file:
-        gracedb_sdk.superevents[superevent_id].logs.create(
+        gracedb.superevents[superevent_id].logs.create(
             comment="Measurement of speed of gravity manuscript",
             filename="SoG_LIV_arxiv_aps.pdf",
             filecontents=file,
             tags=["ext_coinc"]
         )
 
     #  Remove local copy in working directory
     os.unlink(path + 'SoG_LIV_arxiv_aps.pdf')
 
     #  Upload tarball of all files
     if compress_files:
         with open('SoG_LIV_files.tar.gz', 'rb') as file:
-            gracedb_sdk.superevents[superevent_id].logs.create(
+            gracedb.superevents[superevent_id].logs.create(
                 comment="Files for speed of gravity manuscript",
                 filename="SoG_LIV_files.tar.gz",
                 filecontents=file,
                 tags=["ext_coinc"]
             )
 
         #  Remove if not needed
```

### Comparing `SoG-paper-0.8/SoG_paper.egg-info/PKG-INFO` & `SoG-paper-0.9/SoG_paper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SoG-paper
-Version: 0.8
+Version: 0.9
 Summary: Low-latency manuscript of speed of gravity measurement
 Home-page: https://git.ligo.org/olivier.minazzoli/sog_liv_manuscript_template
 Author: Brandon Piotrzkowski
 Author-email: brandon.piotrzkowski@ligo.org
 License: GNU General Public License Version 3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SoG-paper-0.8/SoG_paper.egg-info/SOURCES.txt` & `SoG-paper-0.9/SoG_paper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/bin/.DS_Store` & `SoG-paper-0.9/bin/.DS_Store`

 * *Files identical despite different names*

### Comparing `SoG-paper-0.8/bin/SoG_generate_pdf` & `SoG-paper-0.9/bin/SoG_generate_pdf`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,19 @@
 #
 
 """
 Script to generate pdf file of speed of gravity manuscript.
 """
 __author__ = "Brandon Piotrzkowski <brandon.piotrzkowski@ligo.org>"
 
+import argparse
+from gracedb_sdk import Client
+
 from SoG.tex.generate_upload_pdf import generate_pdf
 
-import argparse
 
 #  Command line options.
 parser = argparse.ArgumentParser(description='Perform query of GraceDB')
 parser.add_argument("-i", "--graceid", metavar="(S,MS)XXXXXX",
                     default=None,
                     help="GraceDB ID of superevent (required)"),
 parser.add_argument("-u", "--gracedb_url", metavar="https://gracedb.ligo.org/api/",
@@ -45,10 +47,14 @@
 parser.add_argument("-L", "--use_latexmk", dest="use_latexmk", action="store_true",
                     help="Use latexmk instead of pdflatex to create pdf."),
 parser.add_argument("-t", "--use_test_macrofile", dest="use_test_macrofile", action="store_true",
                     help="Use local test macro file rather than querying GraceDB.")
 args = parser.parse_args()
 print(args)
 
+#  Load gracedb_sdk client
+gracedb = Client(args.gracedb_url)
+
 #  Run function from repository
-generate_pdf(args.graceid, args.gracedb_url, args.keep_local_copy, 
-             args.compress_files, args.use_latexmk, args.use_test_macrofile)
+generate_pdf(args.graceid, gracedb=gracedb, keep_local_copy=args.keep_local_copy,
+           compress_files=args.compress_files, use_latexmk=args.use_latexmk,
+           use_test_macrofile=args.use_test_macrofile)
```

### Comparing `SoG-paper-0.8/bin/SoG_upload_pdf` & `SoG-paper-0.9/bin/SoG_upload_pdf`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 #
 
 """
 Script to generate pdf file of speed of gravity manuscript.
 """
 __author__ = "Brandon Piotrzkowski <brandon.piotrzkowski@ligo.org>"
 
-from SoG.tex.generate_upload_pdf import upload_pdf
-
 import argparse
+from gracedb_sdk import Client
+
+from SoG.tex.generate_upload_pdf import upload_pdf
 
 #  Command line options.
 parser = argparse.ArgumentParser(description='Perform query of GraceDB')
 parser.add_argument("-i", "--graceid", metavar="(S,MS)XXXXXX",
                     default=None,
                     help="GraceDB ID of superevent (required)"),
 parser.add_argument("-u", "--gracedb_url", metavar="https://gracedb.ligo.org/api/",
@@ -45,10 +46,14 @@
 parser.add_argument("-L", "--use_latexmk", dest="use_latexmk", action="store_true",
                     help="Use latexmk instead of pdflatex to create pdf."),
 parser.add_argument("-t", "--use_test_macrofile", dest="use_test_macrofile", action="store_true",
                     help="Use local test macro file rather than querying GraceDB.")
 args = parser.parse_args()
 print(args)
 
+#  Load gracedb_sdk client
+gracedb = Client(args.gracedb_url)
+
 #  Run function from repository
-upload_pdf(args.graceid, args.gracedb_url, args.keep_local_copy, 
-           args.compress_files, args.use_latexmk, args.use_test_macrofile)
+upload_pdf(args.graceid, gracedb=gracedb, keep_local_copy=args.keep_local_copy,
+           compress_files=args.compress_files, use_latexmk=args.use_latexmk,
+           use_test_macrofile=args.use_test_macrofile)
```

### Comparing `SoG-paper-0.8/setup.py` & `SoG-paper-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='SoG-paper',
-    version='0.8',
+    version='0.9',
     url='https://git.ligo.org/olivier.minazzoli/sog_liv_manuscript_template',
     author='Brandon Piotrzkowski',
     author_email='brandon.piotrzkowski@ligo.org',
     description='Low-latency manuscript of speed of gravity measurement',
     license='GNU General Public License Version 3',
     classifiers=(
         "Programming Language :: Python :: 3",
@@ -47,15 +47,14 @@
     scripts=[
         'bin/SoG_generate_pdf',
         'bin/SoG_upload_pdf',
     ],
     install_requires=[
         'numpy>=1.14.5',
         'healpy!=1.12.0',   # FIXME: https://github.com/healpy/healpy/pull/457
-        'ligo-gracedb',
         'gracedb-sdk',
         'matplotlib',
         'astropy',
         'scipy>=0.7.2',
         'ligo.skymap>=0.1.1',
         'lxml',
         'gcn',
```

