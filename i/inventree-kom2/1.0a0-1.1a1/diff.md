# Comparing `tmp/inventree-kom2-1.0a0.tar.gz` & `tmp/inventree-kom2-1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/inventree-kom2/inventree-kom2/dist/.tmp-9ed0kaan/inventree-kom2-1.0a0.tar", last modified: Mon May 29 22:00:06 2023, max compression
+gzip compressed data, was "/home/runner/work/inventree-kom2/inventree-kom2/dist/.tmp-cai_abeg/inventree-kom2-1.1a1.tar", last modified: Wed May 31 21:26:58 2023, max compression
```

## Comparing `inventree-kom2-1.0a0.tar` & `inventree-kom2-1.1a1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 21:59:51.000000 inventree-kom2-1.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-29 21:59:51.000000 inventree-kom2-1.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-29 21:59:51.000000 inventree-kom2-1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/inventree_kom2/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-29 21:59:51.000000 inventree-kom2-1.0a0/src/inventree_kom2/KiCadClasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-29 21:59:51.000000 inventree-kom2-1.0a0/src/inventree_kom2/Kom2Plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-29 21:59:51.000000 inventree-kom2-1.0a0/src/inventree_kom2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/inventree_kom2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/inventree_kom2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/inventree_kom2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/inventree_kom2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/inventree_kom2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/inventree_kom2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 22:00:06.000000 inventree-kom2-1.0a0/src/inventree_kom2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/src/inventree_kom2/KiCadClasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/src/inventree_kom2/Kom2Plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-31 21:26:42.000000 inventree-kom2-1.1a1/src/inventree_kom2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 21:26:58.000000 inventree-kom2-1.1a1/src/inventree_kom2.egg-info/top_level.txt
```

### Comparing `inventree-kom2-1.0a0/PKG-INFO` & `inventree-kom2-1.1a1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-kom2
-Version: 1.0a0
+Version: 1.1a1
 Summary: Use InvenTree with KiCad
 Author-email: Matthias Mair <code@mjmair.com>
 License: MIT license
 Project-URL: Repository, https://github.com/matmair/inventree-kom2
 Project-URL: Bug Tracker, https://github.com/matmair/inventree-kom2/issues
 Keywords: inventree,inventree-plugin,inventree-kom2
 Classifier: Programming Language :: Python :: 3
@@ -35,7 +35,12 @@
 **The server will restart if you enable the plugin**
 
 3. Install and configure Kom2
 A new panel KiCad will appear in the main naviagtion. You can download and setup the latest release of Kom2 from there.
 
 ## License
 This project is licensed as MIT license.
+
+## Current state: beta
+This plugin is in a early state. It is not recommended to use it in production. You can use it to test the functionality (both of the plugin but also kom2) and report bugs, it assumes the data structure of the [demo dataset](https://github.com/inventree/demo-dataset).
+
+There are no instructions for Windows or Linux, feel free to suggest them.
```

### Comparing `inventree-kom2-1.0a0/pyproject.toml` & `inventree-kom2-1.1a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel", "pyyaml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inventree-kom2"
-version =  "1.0a0"
+version =  "1.1a1"
 description="Use InvenTree with KiCad"
 readme = "README.md"
 license = {text = "MIT license"}
 keywords = ["inventree", "inventree-plugin", "inventree-kom2"]
 authors = [
     {name = "Matthias Mair", email =  "code@mjmair.com"}
 ]
```

### Comparing `inventree-kom2-1.0a0/src/inventree_kom2/KiCadClasses.py` & `inventree-kom2-1.1a1/src/inventree_kom2/KiCadClasses.py`

 * *Files identical despite different names*

### Comparing `inventree-kom2-1.0a0/src/inventree_kom2/Kom2Plugin.py` & `inventree-kom2-1.1a1/src/inventree_kom2/Kom2Plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import requests
 from django.http import HttpResponse
 from django.urls import re_path, reverse
 from InvenTree.permissions import auth_exempt
 from plugin import InvenTreePlugin
 from plugin.helpers import render_template
 from plugin.mixins import NavigationMixin, UrlsMixin
+from rest_framework.authtoken.models import Token
+from rest_framework.exceptions import PermissionDenied
 
 from .KiCadClasses import KiCadField, KiCadLibrary, KiCadSetting
 
 
 class Kom2Plugin(UrlsMixin, NavigationMixin, InvenTreePlugin):
     """Use InvenTree with KiCad."""
 
@@ -46,24 +48,30 @@
             for ref in refs:
                 if asset['name'].endswith(ref + '.zip'):
                     ctx[ref.replace('-', '_')] = asset['browser_download_url']
 
         # Render the template
 
         # Set up the settings url
-        ctx['settings_url'] = request.build_absolute_uri(reverse('plugin:inventree-kom2:settings'))
+        token, _ = Token.objects.get_or_create(user=request.user)
+        ctx['settings_url'] = f"{request.build_absolute_uri(reverse('plugin:inventree-kom2:settings'))}?token={token}"
 
         return HttpResponse(render_template(request, 'inventree_kom2/index.html', ctx))
 
     @auth_exempt
     def settings_func(self, request):
         """Show database settings as json."""
         settings = KiCadSetting()
 
-        settings.source.set_connection_string(path="~/Library/kom2/kom2.dylib", username="reader", password="readonly", server=request.build_absolute_uri("/"))
+        if request.GET and request.GET['token']:
+            settings.source.set_connection_string(path="~/Library/kom2/kom2.dylib", token=request.GET['token'], server=request.build_absolute_uri("/"))
+        else:
+            # Create DB user with readonly access
+            # settings.source.set_connection_string(path="~/Library/kom2/kom2.dylib", username="reader", password="readonly", server=request.build_absolute_uri("/"))
+            raise PermissionDenied({"error": "No token provided."})
         lib = KiCadLibrary()
         lib.fields = [
             KiCadField(column="IPN", name="IPN", visible_on_add=False, visible_in_chooser=True, show_name=True, inherit_properties=True),
             KiCadField(column="parameter.Resistance", name="Resistance", visible_on_add=True, visible_in_chooser=True, show_name=True),
             KiCadField(column="parameter.Package", name="Package", visible_on_add=True, visible_in_chooser=True, show_name=False)
         ]
         settings.libraries = [lib]
```

### Comparing `inventree-kom2-1.0a0/src/inventree_kom2.egg-info/PKG-INFO` & `inventree-kom2-1.1a1/src/inventree_kom2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-kom2
-Version: 1.0a0
+Version: 1.1a1
 Summary: Use InvenTree with KiCad
 Author-email: Matthias Mair <code@mjmair.com>
 License: MIT license
 Project-URL: Repository, https://github.com/matmair/inventree-kom2
 Project-URL: Bug Tracker, https://github.com/matmair/inventree-kom2/issues
 Keywords: inventree,inventree-plugin,inventree-kom2
 Classifier: Programming Language :: Python :: 3
@@ -35,7 +35,12 @@
 **The server will restart if you enable the plugin**
 
 3. Install and configure Kom2
 A new panel KiCad will appear in the main naviagtion. You can download and setup the latest release of Kom2 from there.
 
 ## License
 This project is licensed as MIT license.
+
+## Current state: beta
+This plugin is in a early state. It is not recommended to use it in production. You can use it to test the functionality (both of the plugin but also kom2) and report bugs, it assumes the data structure of the [demo dataset](https://github.com/inventree/demo-dataset).
+
+There are no instructions for Windows or Linux, feel free to suggest them.
```

