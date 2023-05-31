# Comparing `tmp/komora_syncer-2.4.tar.gz` & `tmp/komora_syncer-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komora_syncer-2.4.tar", last modified: Wed May 31 10:59:22 2023, max compression
+gzip compressed data, was "komora_syncer-2.5.tar", last modified: Wed May 31 12:02:43 2023, max compression
```

## Comparing `komora_syncer-2.4.tar` & `komora_syncer-2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-31 10:59:22.059531 komora_syncer-2.4/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1378 2023-05-31 10:59:22.059531 komora_syncer-2.4/PKG-INFO
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      529 2022-04-28 10:08:08.000000 komora_syncer-2.4/README.md
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-31 10:59:22.049531 komora_syncer-2.4/komora_syncer/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       28 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/__init__.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3342 2023-05-31 10:51:22.000000 komora_syncer-2.4/komora_syncer/__main__.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3162 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/config.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-31 10:59:22.059531 komora_syncer-2.4/komora_syncer/connections/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      713 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/connections/NetboxConnection.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/connections/__init__.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-31 10:59:22.059531 komora_syncer-2.4/komora_syncer/helpers/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/helpers/__init__.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      221 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/helpers/utils.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-31 10:59:22.059531 komora_syncer-2.4/komora_syncer/models/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     6467 2023-05-31 10:49:21.000000 komora_syncer-2.4/komora_syncer/models/Synchronizer.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/__init__.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-31 10:59:22.059531 komora_syncer-2.4/komora_syncer/models/komora/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     8478 2023-05-31 10:04:31.000000 komora_syncer-2.4/komora_syncer/models/komora/KomoraApi.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/__init__.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      747 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/address.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     4500 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/contact.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1048 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/device.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      271 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/district.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      520 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/location.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      381 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/municipality.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1304 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/organization.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      171 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/region.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     2042 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/site.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      230 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/komora/site_contact.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-31 10:59:22.059531 komora_syncer-2.4/komora_syncer/models/netbox/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     4949 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/netbox/NbDevice.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3386 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/netbox/NbLocation.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3770 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/netbox/NbRegion.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     6052 2022-07-13 11:09:12.000000 komora_syncer-2.4/komora_syncer/models/netbox/NbSite.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     3854 2023-05-31 10:04:31.000000 komora_syncer-2.4/komora_syncer/models/netbox/NbTenant.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)      235 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/netbox/NetboxBase.py
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        0 2022-04-28 10:08:08.000000 komora_syncer-2.4/komora_syncer/models/netbox/__init__.py
-drwxr-xr-x   0 jankrupa  (1000) jankrupa  (1000)        0 2023-05-31 10:59:22.059531 komora_syncer-2.4/komora_syncer.egg-info/
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1378 2023-05-31 10:59:22.000000 komora_syncer-2.4/komora_syncer.egg-info/PKG-INFO
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1338 2023-05-31 10:59:22.000000 komora_syncer-2.4/komora_syncer.egg-info/SOURCES.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        1 2023-05-31 10:59:22.000000 komora_syncer-2.4/komora_syncer.egg-info/dependency_links.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       62 2023-05-31 10:59:22.000000 komora_syncer-2.4/komora_syncer.egg-info/entry_points.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)        1 2022-07-13 11:11:13.000000 komora_syncer-2.4/komora_syncer.egg-info/not-zip-safe
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       81 2023-05-31 10:59:22.000000 komora_syncer-2.4/komora_syncer.egg-info/requires.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       14 2023-05-31 10:59:22.000000 komora_syncer-2.4/komora_syncer.egg-info/top_level.txt
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)       38 2023-05-31 10:59:22.059531 komora_syncer-2.4/setup.cfg
--rw-r--r--   0 jankrupa  (1000) jankrupa  (1000)     1853 2023-05-31 10:57:50.000000 komora_syncer-2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:02:43.036782 komora_syncer-2.5/
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-31 12:02:43.036782 komora_syncer-2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2022-02-03 09:20:26.000000 komora_syncer-2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:02:43.032781 komora_syncer-2.5/komora_syncer/
+-rw-r--r--   0 root         (0) root         (0)       28 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-05-31 11:32:20.000000 komora_syncer-2.5/komora_syncer/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3162 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:02:43.032781 komora_syncer-2.5/komora_syncer/connections/
+-rw-r--r--   0 root         (0) root         (0)      713 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/connections/NetboxConnection.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/connections/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:02:43.032781 komora_syncer-2.5/komora_syncer/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      221 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/helpers/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:02:43.032781 komora_syncer-2.5/komora_syncer/models/
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-05-31 11:32:20.000000 komora_syncer-2.5/komora_syncer/models/Synchronizer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:02:43.036782 komora_syncer-2.5/komora_syncer/models/komora/
+-rw-r--r--   0 root         (0) root         (0)     8617 2023-05-31 12:02:41.000000 komora_syncer-2.5/komora_syncer/models/komora/KomoraApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/models/komora/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      747 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/address.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/contact.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/device.py
+-rw-r--r--   0 root         (0) root         (0)      271 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/district.py
+-rw-r--r--   0 root         (0) root         (0)      520 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/location.py
+-rw-r--r--   0 root         (0) root         (0)      381 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/municipality.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/organization.py
+-rw-r--r--   0 root         (0) root         (0)      171 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/region.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2022-03-31 12:40:18.000000 komora_syncer-2.5/komora_syncer/models/komora/site.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-03-28 07:12:55.000000 komora_syncer-2.5/komora_syncer/models/komora/site_contact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:02:43.036782 komora_syncer-2.5/komora_syncer/models/netbox/
+-rw-r--r--   0 root         (0) root         (0)     4949 2022-02-28 11:43:18.000000 komora_syncer-2.5/komora_syncer/models/netbox/NbDevice.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/models/netbox/NbLocation.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2022-03-31 12:40:18.000000 komora_syncer-2.5/komora_syncer/models/netbox/NbRegion.py
+-rw-r--r--   0 root         (0) root         (0)     6052 2022-07-13 11:08:37.000000 komora_syncer-2.5/komora_syncer/models/netbox/NbSite.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-05-31 12:02:41.000000 komora_syncer-2.5/komora_syncer/models/netbox/NbTenant.py
+-rw-r--r--   0 root         (0) root         (0)      235 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/models/netbox/NetboxBase.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-03 09:20:26.000000 komora_syncer-2.5/komora_syncer/models/netbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:02:43.032781 komora_syncer-2.5/komora_syncer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-31 12:02:43.000000 komora_syncer-2.5/komora_syncer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-05-31 12:02:43.000000 komora_syncer-2.5/komora_syncer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:02:43.000000 komora_syncer-2.5/komora_syncer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-31 12:02:43.000000 komora_syncer-2.5/komora_syncer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-03 09:25:55.000000 komora_syncer-2.5/komora_syncer.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-31 12:02:43.000000 komora_syncer-2.5/komora_syncer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-31 12:02:43.000000 komora_syncer-2.5/komora_syncer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 12:02:43.036782 komora_syncer-2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-05-31 12:02:41.000000 komora_syncer-2.5/setup.py
```

### Comparing `komora_syncer-2.4/PKG-INFO` & `komora_syncer-2.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 Metadata-Version: 2.1
 Name: komora_syncer
-Version: 2.4
+Version: 2.5
 Summary: Synchronize data between Komora and Netbox applications
 Home-page: https://gitlab.cesnet.cz/701/done/netbox_komora_syncer
 Author: Jan Krupa
 Author-email: jan.krupa@cesnet.cz
 License: UNKNOWN
+Description: Netbox and Komora synchronizer
+        ===
+        
+        `komora_syncer` is a tool to synchronize data between Komora and Netbox application 
+        
+        Installation
+        ------------
+        - `git clone` this repository
+        - `pip install .`
+        - setup configuration files [config.yml, logging.ini]
+           - paths: 
+              - ~/.config/komora_syncer/
+              - /etc/komora_syncer/config.yml
+              - Or can be set with the variable `--config`. Example: `komora_syncer --config ./configuration_folder synchronize`
+        
+        
+        Run
+        ---
+        
+        - `komora_syncer`
+        
+        komora_syncer requires at least Python 3.6.
+        
 Keywords: netbox,komora
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-
-Netbox and Komora synchronizer
-===
-
-`komora_syncer` is a tool to synchronize data between Komora and Netbox application 
-
-Installation
-------------
-- `git clone` this repository
-- `pip install .`
-- setup configuration files [config.yml, logging.ini]
-   - paths: 
-      - ~/.config/komora_syncer/
-      - /etc/komora_syncer/config.yml
-      - Or can be set with the variable `--config`. Example: `komora_syncer --config ./configuration_folder synchronize`
-
-
-Run
----
-
-- `komora_syncer`
-
-komora_syncer requires at least Python 3.6.
-
-
```

### Comparing `komora_syncer-2.4/README.md` & `komora_syncer-2.5/README.md`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/__main__.py` & `komora_syncer-2.5/komora_syncer/__main__.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/config.py` & `komora_syncer-2.5/komora_syncer/config.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/connections/NetboxConnection.py` & `komora_syncer-2.5/komora_syncer/connections/NetboxConnection.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/Synchronizer.py` & `komora_syncer-2.5/komora_syncer/models/Synchronizer.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/komora/KomoraApi.py` & `komora_syncer-2.5/komora_syncer/models/komora/KomoraApi.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from komora_syncer.models.komora.region import Region
 from komora_syncer.models.komora.district import District
 from komora_syncer.models.komora.municipality import Municipality
 from komora_syncer.models.komora.site import Site
 from komora_syncer.models.komora.device import Device
 from komora_syncer.models.komora.contact import Contact
 
+from komora_syncer.helpers.utils import build_tenant_name
+
 import hmac
 import hashlib
 import time
 import base64
 import urllib.parse
 import json
 import time
@@ -96,20 +98,21 @@
             logger.exception("Unable to poll organizations from Komora")
             logger.debug(f"URL: {url}")
             raise e
         else:
             response = response.json()
 
         # TODO: unique cids
-        unique_cids = []
+        unique_cids_names = []
         for organization in response.get("data", []):
-            if organization['clientId'] not in unique_cids:
-                unique_cids.append(organization['clientId'])
+            cid_name = build_tenant_name(organization['clientId'], organization['name'])
+            if cid_name not in unique_cids_names:
+                unique_cids_names.append(cid_name)
             else:
-                logger.critical(f"Duplicated CID: {organization}")
+                logger.critical(f"Duplicated CID and Name: {cid_name}")
                 continue
             self.organizations.append(Organization(**organization))
 
         return self.organizations
 
     def get_regions(self):
         if self.regions:
```

### Comparing `komora_syncer-2.4/komora_syncer/models/komora/address.py` & `komora_syncer-2.5/komora_syncer/models/komora/address.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/komora/contact.py` & `komora_syncer-2.5/komora_syncer/models/komora/contact.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/komora/device.py` & `komora_syncer-2.5/komora_syncer/models/komora/device.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/komora/location.py` & `komora_syncer-2.5/komora_syncer/models/komora/location.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/komora/organization.py` & `komora_syncer-2.5/komora_syncer/models/komora/organization.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/komora/site.py` & `komora_syncer-2.5/komora_syncer/models/komora/site.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/netbox/NbDevice.py` & `komora_syncer-2.5/komora_syncer/models/netbox/NbDevice.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/netbox/NbLocation.py` & `komora_syncer-2.5/komora_syncer/models/netbox/NbLocation.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/netbox/NbRegion.py` & `komora_syncer-2.5/komora_syncer/models/netbox/NbRegion.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/netbox/NbSite.py` & `komora_syncer-2.5/komora_syncer/models/netbox/NbSite.py`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/komora_syncer/models/netbox/NbTenant.py` & `komora_syncer-2.5/komora_syncer/models/netbox/NbTenant.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,16 @@
 
     def update(self, nb_tenant):
         try:
             if nb_tenant.update(self.get_params()):
                 self.api_object = nb_tenant
                 logger.info(f"Tenant: {self.name} updated successfuly")
         except Exception as e:
-            logger.error(e)
-            raise e
+            logger.error(f"{e} {nb_tenant.name} {nb_tenant.id}")
+
 
     def synchronize(self):
         tenant = self.find()
 
         if tenant:
             self.update(tenant)
         else:
```

### Comparing `komora_syncer-2.4/komora_syncer.egg-info/PKG-INFO` & `komora_syncer-2.5/komora_syncer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 Metadata-Version: 2.1
 Name: komora-syncer
-Version: 2.4
+Version: 2.5
 Summary: Synchronize data between Komora and Netbox applications
 Home-page: https://gitlab.cesnet.cz/701/done/netbox_komora_syncer
 Author: Jan Krupa
 Author-email: jan.krupa@cesnet.cz
 License: UNKNOWN
+Description: Netbox and Komora synchronizer
+        ===
+        
+        `komora_syncer` is a tool to synchronize data between Komora and Netbox application 
+        
+        Installation
+        ------------
+        - `git clone` this repository
+        - `pip install .`
+        - setup configuration files [config.yml, logging.ini]
+           - paths: 
+              - ~/.config/komora_syncer/
+              - /etc/komora_syncer/config.yml
+              - Or can be set with the variable `--config`. Example: `komora_syncer --config ./configuration_folder synchronize`
+        
+        
+        Run
+        ---
+        
+        - `komora_syncer`
+        
+        komora_syncer requires at least Python 3.6.
+        
 Keywords: netbox,komora
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
-
-Netbox and Komora synchronizer
-===
-
-`komora_syncer` is a tool to synchronize data between Komora and Netbox application 
-
-Installation
-------------
-- `git clone` this repository
-- `pip install .`
-- setup configuration files [config.yml, logging.ini]
-   - paths: 
-      - ~/.config/komora_syncer/
-      - /etc/komora_syncer/config.yml
-      - Or can be set with the variable `--config`. Example: `komora_syncer --config ./configuration_folder synchronize`
-
-
-Run
----
-
-- `komora_syncer`
-
-komora_syncer requires at least Python 3.6.
-
-
```

### Comparing `komora_syncer-2.4/komora_syncer.egg-info/SOURCES.txt` & `komora_syncer-2.5/komora_syncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `komora_syncer-2.4/setup.py` & `komora_syncer-2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
       include_package_data=True,
       keywords="netbox,komora",
       packages=find_packages(),
       setup_requires=setup_requirements,
       test_suite="tests",
       tests_require=test_requirements,
       url="https://gitlab.cesnet.cz/701/done/netbox_komora_syncer",
-      version='2.4',
+      version='2.5',
       zip_safe=False,
       python_requires='>=3.6, <4',
       entry_points={
           'console_scripts': [
             'komora_syncer=komora_syncer.__main__:cli',
             ]
       },
```

