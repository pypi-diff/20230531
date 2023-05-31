# Comparing `tmp/powerling-api-sdk-0.1.3.tar.gz` & `tmp/powerling-api-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerling-api-sdk-0.1.3.tar", last modified: Tue Jul 19 15:46:48 2022, max compression
+gzip compressed data, was "powerling-api-sdk-0.1.4.tar", last modified: Wed May 31 15:54:31 2023, max compression
```

## Comparing `powerling-api-sdk-0.1.3.tar` & `powerling-api-sdk-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 grcpils    (501) staff       (20)        0 2022-07-19 15:46:48.493909 powerling-api-sdk-0.1.3/
--rw-r--r--   0 grcpils    (501) staff       (20)    35148 2022-05-03 14:25:42.000000 powerling-api-sdk-0.1.3/LICENSE
--rw-r--r--   0 grcpils    (501) staff       (20)     4636 2022-07-19 15:46:48.493969 powerling-api-sdk-0.1.3/PKG-INFO
--rw-r--r--   0 grcpils    (501) staff       (20)     3993 2022-06-09 10:05:14.000000 powerling-api-sdk-0.1.3/README.md
--rw-r--r--   0 grcpils    (501) staff       (20)        0 2022-05-03 14:26:00.000000 powerling-api-sdk-0.1.3/pyproject.toml
--rw-r--r--   0 grcpils    (501) staff       (20)      742 2022-07-19 15:46:48.494197 powerling-api-sdk-0.1.3/setup.cfg
-drwxr-xr-x   0 grcpils    (501) staff       (20)        0 2022-07-19 15:46:48.489252 powerling-api-sdk-0.1.3/src/
-drwxr-xr-x   0 grcpils    (501) staff       (20)        0 2022-07-19 15:46:48.491017 powerling-api-sdk-0.1.3/src/powerling_api_sdk.egg-info/
--rw-r--r--   0 grcpils    (501) staff       (20)     4636 2022-07-19 15:46:48.000000 powerling-api-sdk-0.1.3/src/powerling_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 grcpils    (501) staff       (20)      588 2022-07-19 15:46:48.000000 powerling-api-sdk-0.1.3/src/powerling_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 grcpils    (501) staff       (20)        1 2022-07-19 15:46:48.000000 powerling-api-sdk-0.1.3/src/powerling_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 grcpils    (501) staff       (20)        9 2022-07-19 15:46:48.000000 powerling-api-sdk-0.1.3/src/powerling_api_sdk.egg-info/requires.txt
--rw-r--r--   0 grcpils    (501) staff       (20)       13 2022-07-19 15:46:48.000000 powerling-api-sdk-0.1.3/src/powerling_api_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 grcpils    (501) staff       (20)        0 2022-07-19 15:46:48.492306 powerling-api-sdk-0.1.3/src/powerlingapi/
--rw-r--r--   0 grcpils    (501) staff       (20)     1839 2022-07-08 07:50:23.000000 powerling-api-sdk-0.1.3/src/powerlingapi/File.py
--rw-r--r--   0 grcpils    (501) staff       (20)     3883 2022-05-30 14:48:46.000000 powerling-api-sdk-0.1.3/src/powerlingapi/Form.py
--rw-r--r--   0 grcpils    (501) staff       (20)     2887 2022-05-30 14:21:17.000000 powerling-api-sdk-0.1.3/src/powerlingapi/Order.py
--rw-r--r--   0 grcpils    (501) staff       (20)      129 2022-05-30 13:26:16.000000 powerling-api-sdk-0.1.3/src/powerlingapi/__init__.py
-drwxr-xr-x   0 grcpils    (501) staff       (20)        0 2022-07-19 15:46:48.493656 powerling-api-sdk-0.1.3/src/powerlingapi/exceptions/
--rw-r--r--   0 grcpils    (501) staff       (20)       75 2022-05-27 13:32:30.000000 powerling-api-sdk-0.1.3/src/powerlingapi/exceptions/__init__.py
--rw-r--r--   0 grcpils    (501) staff       (20)      322 2022-05-30 14:23:07.000000 powerling-api-sdk-0.1.3/src/powerlingapi/exceptions/api.py
--rw-r--r--   0 grcpils    (501) staff       (20)      487 2022-05-27 15:28:58.000000 powerling-api-sdk-0.1.3/src/powerlingapi/exceptions/file.py
--rw-r--r--   0 grcpils    (501) staff       (20)      791 2022-05-30 14:48:41.000000 powerling-api-sdk-0.1.3/src/powerlingapi/exceptions/form.py
--rw-r--r--   0 grcpils    (501) staff       (20)      450 2022-05-30 14:22:31.000000 powerling-api-sdk-0.1.3/src/powerlingapi/exceptions/order.py
--rw-r--r--   0 grcpils    (501) staff       (20)     2620 2022-07-15 16:09:58.000000 powerling-api-sdk-0.1.3/src/powerlingapi/powerlingapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:31.702198 powerling-api-sdk-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)    35148 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4955 2023-05-31 15:54:31.702198 powerling-api-sdk-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4312 2023-05-31 15:54:22.000000 powerling-api-sdk-0.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:54:22.000000 powerling-api-sdk-0.1.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-05-31 15:54:31.702198 powerling-api-sdk-0.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:31.698197 powerling-api-sdk-0.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:31.698197 powerling-api-sdk-0.1.4/src/powerling_api_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4955 2023-05-31 15:54:31.000000 powerling-api-sdk-0.1.4/src/powerling_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-31 15:54:31.000000 powerling-api-sdk-0.1.4/src/powerling_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:54:31.000000 powerling-api-sdk-0.1.4/src/powerling_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-31 15:54:31.000000 powerling-api-sdk-0.1.4/src/powerling_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 15:54:31.000000 powerling-api-sdk-0.1.4/src/powerling_api_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:31.698197 powerling-api-sdk-0.1.4/src/powerlingapi/
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/File.py
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/Form.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/Order.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:54:31.702198 powerling-api-sdk-0.1.4/src/powerlingapi/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/exceptions/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/exceptions/file.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/exceptions/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/exceptions/order.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-05-31 12:50:50.000000 powerling-api-sdk-0.1.4/src/powerlingapi/powerlingapi.py
```

### Comparing `powerling-api-sdk-0.1.3/LICENSE` & `powerling-api-sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `powerling-api-sdk-0.1.3/PKG-INFO` & `powerling-api-sdk-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerling-api-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK for Powerling API
 Author: Powerling
 Author-email: contact@powerling.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -141,14 +141,26 @@
 
   url = "https://exemple.com/callback"
 
   # [get an order with id or create new one]
   order.add_callback(url)
 ```
 
+#### Get analysis
+
+```py
+from powerlingapi import PowerlingApi
+
+def main():
+  # [initialization...]
+
+  # [get an order with id or create new one]
+  order.get_analysis()
+```
+
 #### Add binary file
 
 ```py
 from powerlingapi import PowerlingApi
 from powerlingapi import exceptions
 from powerlingapi import Form
 
@@ -249,7 +261,19 @@
   # [initialization...]
 
   url = "https://exemple.com/callback"
 
   # [get a file]
   file.add_callback(url)
 ```
+
+#### Get analysis
+
+```py
+from powerlingapi import PowerlingApi
+
+def main():
+  # [initialization...]
+
+  # [get a file]
+  file.get_analysis()
+```
```

### Comparing `powerling-api-sdk-0.1.3/README.md` & `powerling-api-sdk-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -123,14 +123,26 @@
 
   url = "https://exemple.com/callback"
 
   # [get an order with id or create new one]
   order.add_callback(url)
 ```
 
+#### Get analysis
+
+```py
+from powerlingapi import PowerlingApi
+
+def main():
+  # [initialization...]
+
+  # [get an order with id or create new one]
+  order.get_analysis()
+```
+
 #### Add binary file
 
 ```py
 from powerlingapi import PowerlingApi
 from powerlingapi import exceptions
 from powerlingapi import Form
 
@@ -230,8 +242,20 @@
 def main():
   # [initialization...]
 
   url = "https://exemple.com/callback"
 
   # [get a file]
   file.add_callback(url)
+```
+
+#### Get analysis
+
+```py
+from powerlingapi import PowerlingApi
+
+def main():
+  # [initialization...]
+
+  # [get a file]
+  file.get_analysis()
 ```
```

### Comparing `powerling-api-sdk-0.1.3/setup.cfg` & `powerling-api-sdk-0.1.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = powerling-api-sdk
-version = 0.1.3
+version = 0.1.4
 author = Powerling
 author_email = contact@powerling.com
 description = SDK for Powerling API
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
```

### Comparing `powerling-api-sdk-0.1.3/src/powerling_api_sdk.egg-info/PKG-INFO` & `powerling-api-sdk-0.1.4/src/powerling_api_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerling-api-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: SDK for Powerling API
 Author: Powerling
 Author-email: contact@powerling.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -141,14 +141,26 @@
 
   url = "https://exemple.com/callback"
 
   # [get an order with id or create new one]
   order.add_callback(url)
 ```
 
+#### Get analysis
+
+```py
+from powerlingapi import PowerlingApi
+
+def main():
+  # [initialization...]
+
+  # [get an order with id or create new one]
+  order.get_analysis()
+```
+
 #### Add binary file
 
 ```py
 from powerlingapi import PowerlingApi
 from powerlingapi import exceptions
 from powerlingapi import Form
 
@@ -249,7 +261,19 @@
   # [initialization...]
 
   url = "https://exemple.com/callback"
 
   # [get a file]
   file.add_callback(url)
 ```
+
+#### Get analysis
+
+```py
+from powerlingapi import PowerlingApi
+
+def main():
+  # [initialization...]
+
+  # [get a file]
+  file.get_analysis()
+```
```

### Comparing `powerling-api-sdk-0.1.3/src/powerling_api_sdk.egg-info/SOURCES.txt` & `powerling-api-sdk-0.1.4/src/powerling_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `powerling-api-sdk-0.1.3/src/powerlingapi/File.py` & `powerling-api-sdk-0.1.4/src/powerlingapi/File.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,9 +59,17 @@
     """
     ### Parameters:
     `callback_url` : str
       The callback url.
     ### Returns:
     `None`: The callback is added.
     """
-    res = self.session.post(self.url + 'order/' + str(self.orderid) + '/file/' + str(self.id), data={'url': callback_url})
+    res = self.session.post(self.url + 'order/' + str(self.orderid) + '/file/' + str(self.id) + '/request-callback', data={'url': callback_url})
+    return res.json()
+
+  def get_analysis(self):
+    """
+    ### Returns:
+    `dict`: The file analysis.
+    """
+    res = self.session.get(self.url + 'order/' + str(self.orderid) + '/file/' + str(self.id) + '/analysis')
     return res.json()
```

### Comparing `powerling-api-sdk-0.1.3/src/powerlingapi/Form.py` & `powerling-api-sdk-0.1.4/src/powerlingapi/Form.py`

 * *Files identical despite different names*

### Comparing `powerling-api-sdk-0.1.3/src/powerlingapi/Order.py` & `powerling-api-sdk-0.1.4/src/powerlingapi/Order.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-from operator import concat
 from typing import List, Union
 
 from .File import File
 from . import Form
 from . import exceptions
 
 class Order():
@@ -115,8 +114,16 @@
     ### Parameters:
     `callback_url` : str
       The callback url.
 
     ### Returns:
     `None`
     """
-    res = self.session.post(self.url + 'order/' + str(self.id) + '/add-callback', data={'url': callback_url})
+    res = self.session.post(self.url + 'order/' + str(self.id) + '/request-callback', data={'url': callback_url})
+
+  def get_analysis(self) -> dict:
+    """
+    ### Returns:
+    `dict`: The analysis informations.
+    """
+    res = self.session.get(self.url + 'order/' + str(self.id) + '/analysis')
+    return res.json()
```

### Comparing `powerling-api-sdk-0.1.3/src/powerlingapi/exceptions/form.py` & `powerling-api-sdk-0.1.4/src/powerlingapi/exceptions/form.py`

 * *Files identical despite different names*

### Comparing `powerling-api-sdk-0.1.3/src/powerlingapi/powerlingapi.py` & `powerling-api-sdk-0.1.4/src/powerlingapi/powerlingapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     """
     ### Parameters:
     `bearer` : str
       The bearer token to use for the API.
 
     ### Notes:
         This method just set the bearer token in the session.
-        No verification is done.
     """
     self.session.headers.update({'Authorization': 'Bearer ' + bearer})
     try:
       self.account()
     except Exception:
       self.session.headers.clear()
       raise exceptions.api.InvalidCredentials
```

