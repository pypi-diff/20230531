# Comparing `tmp/otlmow_davie-0.2.tar.gz` & `tmp/otlmow_davie-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otlmow_davie-0.2.tar", last modified: Tue Apr  4 07:35:24 2023, max compression
+gzip compressed data, was "otlmow_davie-0.3.tar", last modified: Wed May 31 21:02:55 2023, max compression
```

## Comparing `otlmow_davie-0.2.tar` & `otlmow_davie-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:35:24.548268 otlmow_davie-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-04 07:35:13.000000 otlmow_davie-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-04-04 07:35:24.548268 otlmow_davie-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-04 07:35:13.000000 otlmow_davie-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:35:24.544268 otlmow_davie-0.2/otlmow_davie/
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/CertRequester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/DavieClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/DavieDomain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/DavieRestClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/Enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/JWTRequester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/RequestHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/RequesterFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/SettingsManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:35:13.000000 otlmow_davie-0.2/otlmow_davie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:35:24.548268 otlmow_davie-0.2/otlmow_davie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-04-04 07:35:24.000000 otlmow_davie-0.2/otlmow_davie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-04 07:35:24.000000 otlmow_davie-0.2/otlmow_davie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:35:24.000000 otlmow_davie-0.2/otlmow_davie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-04 07:35:24.000000 otlmow_davie-0.2/otlmow_davie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-04 07:35:13.000000 otlmow_davie-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:35:24.548268 otlmow_davie-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:02:55.319818 otlmow_davie-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-31 21:02:46.000000 otlmow_davie-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-05-31 21:02:55.319818 otlmow_davie-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-31 21:02:46.000000 otlmow_davie-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:02:55.315818 otlmow_davie-0.3/otlmow_davie/
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/CertRequester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/DavieClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/DavieDomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/DavieRestClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/Enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/JWTRequester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/RequestHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/RequesterFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/SettingsManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 21:02:46.000000 otlmow_davie-0.3/otlmow_davie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:02:55.319818 otlmow_davie-0.3/otlmow_davie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-05-31 21:02:55.000000 otlmow_davie-0.3/otlmow_davie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-31 21:02:55.000000 otlmow_davie-0.3/otlmow_davie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:02:55.000000 otlmow_davie-0.3/otlmow_davie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 21:02:55.000000 otlmow_davie-0.3/otlmow_davie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-31 21:02:46.000000 otlmow_davie-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:02:55.319818 otlmow_davie-0.3/setup.cfg
```

### Comparing `otlmow_davie-0.2/LICENSE` & `otlmow_davie-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `otlmow_davie-0.2/PKG-INFO` & `otlmow_davie-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otlmow_davie
-Version: 0.2
+Version: 0.3
 Author-email: David Vlaminck <david.vlaminck@mow.vlaanderen.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `otlmow_davie-0.2/README.md` & `otlmow_davie-0.3/README.md`

 * *Files identical despite different names*

### Comparing `otlmow_davie-0.2/otlmow_davie/CertRequester.py` & `otlmow_davie-0.3/otlmow_davie/CertRequester.py`

 * *Files identical despite different names*

### Comparing `otlmow_davie-0.2/otlmow_davie/DavieDomain.py` & `otlmow_davie-0.3/otlmow_davie/DavieDomain.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 from typing import Optional
 
-from pydantic import Field
+from pydantic import Field, conlist
 from pydantic import BaseModel as PydanticBaseModel
 
-from otlmow_davie.Enums import AanleveringStatus, AanleveringSubstatus, MethodEnum
+from otlmow_davie.Enums import AanleveringStatus, AanleveringSubstatus, MethodEnum, ExportType, LevelOfGeometry
 
 
 class BaseModel(PydanticBaseModel):
     class Config:
         arbitrary_types_allowed = True
 
 
@@ -42,15 +42,15 @@
 
 
 class AanleveringResultaat(BaseModel):
     """Een aanlevering met zijn links. Deze links geven aan welke acties mogelijk zijn op de aanlevering. Als een
     link ontbreekt op een aanlevering dan betekent dit dat de corresponderende actie niet mogelijk is op de
     aanlevering. """
     aanlevering: Aanlevering
-    links: 	AanleveringHateoasLinks
+    links: AanleveringHateoasLinks
 
     class Config:
         use_enum_values = True
 
 
 class AanleveringCreatie(BaseModel, ABC):
     pass
@@ -98,7 +98,35 @@
 
 class AanleveringBestandResultaat(BaseModel):
     """
     Een bestand met zijn links. Deze links geven aan welke acties mogelijk zijn op het bestand. Als een link
     ontbreekt op een bestand dan betekent dit dat de corresponderende actie niet mogelijk is op het bestand. """
     bestand: AanleveringBestand
     links: AanleveringBestandHateoasLinks
+
+
+class AsIsAanvraagCreatie(BaseModel):
+    """Capteert alle informatie rond het aanmaken van een asis aanvraag voor een aanlevering."""
+    geometrie: Optional[str]
+    exportType: ExportType
+    assetTypes: conlist(str, min_items=1, max_items=50)
+    levelOfGeometry: LevelOfGeometry = LevelOfGeometry.ALLES
+    emailAdres: Optional[str]
+
+
+class AsIsAanvraagHateoasLinks(BaseModel):
+    """De HATEOAS links die van toepassing zijn op een asis aanvraag."""
+    self: Optional[HateoasLink]
+
+
+class AsIsAanvraag(BaseModel):
+    """Groepeert alle informatie van een asis aanvraag van een aanlevering"""
+    id: str
+    aanleveringId: str
+
+
+class AsIsAanvraagResultaat(BaseModel):
+    """Een aanlevering met zijn links. Deze links geven aan welke acties mogelijk zijn op de aanlevering. Als een
+    link ontbreekt op een aanlevering dan betekent dit dat de corresponderende actie niet mogelijk is op de
+    aanlevering. """
+    asisAanvraag: AsIsAanvraag
+    links: Optional[AsIsAanvraagHateoasLinks]
```

### Comparing `otlmow_davie-0.2/otlmow_davie/JWTRequester.py` & `otlmow_davie-0.3/otlmow_davie/JWTRequester.py`

 * *Files identical despite different names*

### Comparing `otlmow_davie-0.2/otlmow_davie/RequestHandler.py` & `otlmow_davie-0.3/otlmow_davie/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `otlmow_davie-0.2/otlmow_davie/RequesterFactory.py` & `otlmow_davie-0.3/otlmow_davie/RequesterFactory.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         first_part_url = ''
         if environment == Environment.prd:
             first_part_url = 'https://services.apps.mow.vlaanderen.be/'
         elif environment == Environment.tei:
             first_part_url = 'https://services.apps-tei.mow.vlaanderen.be/'
         elif environment == Environment.dev:
             first_part_url = 'https://services.apps-dev.mow.vlaanderen.be/'
+        elif environment == Environment.aim:
+            first_part_url = 'https://services-aim.apps-dev.mow.vlaanderen.be/'
 
         if auth_type == AuthenticationType.JWT:
             return JWTRequester(private_key_path=auth_info['key_path'],
                                 client_id=auth_info['client_id'],
                                 first_part_url=first_part_url)
         if auth_type == AuthenticationType.cert:
             return CertRequester(cert_path=auth_info['cert_path'],
```

### Comparing `otlmow_davie-0.2/otlmow_davie.egg-info/PKG-INFO` & `otlmow_davie-0.3/otlmow_davie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otlmow-davie
-Version: 0.2
+Version: 0.3
 Author-email: David Vlaminck <david.vlaminck@mow.vlaanderen.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `otlmow_davie-0.2/pyproject.toml` & `otlmow_davie-0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otlmow_davie"
-version = "0.2"
+version = "0.3"
 authors = [{name = "David Vlaminck", email = "david.vlaminck@mow.vlaanderen.be"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

