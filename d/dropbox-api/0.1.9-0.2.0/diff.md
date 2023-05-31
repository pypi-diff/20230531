# Comparing `tmp/dropbox_api-0.1.9.tar.gz` & `tmp/dropbox-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dropbox_api-0.1.9.tar", last modified: Wed Apr 18 20:19:27 2018, max compression
+gzip compressed data, was "dist/dropbox-api-0.2.0.tar", last modified: Wed May 31 18:20:30 2023, max compression
```

## Comparing `dropbox_api-0.1.9.tar` & `dropbox-api-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/dropbox/
--rw-r--r--   0 travis    (2000) travis    (2000)     1406 2018-04-18 20:18:44.000000 dropbox_api-0.1.9/src/dropbox/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2888 2018-04-18 20:18:44.000000 dropbox_api-0.1.9/src/dropbox/base.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5090 2018-04-18 20:18:44.000000 dropbox_api-0.1.9/src/dropbox/file.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1640 2018-04-18 20:18:44.000000 dropbox_api-0.1.9/src/dropbox/shared_link.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1655 2018-04-18 20:18:44.000000 dropbox_api-0.1.9/src/dropbox/user.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/dropbox_api.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      959 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/dropbox_api.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      371 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/dropbox_api.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/dropbox_api.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/dropbox_api.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)        7 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/dropbox_api.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        8 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/src/dropbox_api.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      853 2018-04-18 20:18:44.000000 dropbox_api-0.1.9/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)       67 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     2515 2018-04-18 20:18:44.000000 dropbox_api-0.1.9/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      959 2018-04-18 20:19:27.000000 dropbox_api-0.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox/
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/user.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/shared_link.py
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/base.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/src/dropbox/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 18:20:25.000000 dropbox-api-0.2.0/src/dropbox_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2291 2023-05-31 18:20:30.000000 dropbox-api-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-05-31 18:20:22.000000 dropbox-api-0.2.0/README.md
```

### Comparing `dropbox_api-0.1.9/src/dropbox/__init__.py` & `dropbox-api-0.2.0/src/dropbox/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Dropbox API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Dropbox API.
 #
 # Hive Dropbox API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -24,15 +24,15 @@
 
 __revision__ = "$LastChangedRevision$"
 """ The revision number of the module """
 
 __date__ = "$LastChangedDate$"
 """ The last change date of the module """
 
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import base
 from . import file
```

### Comparing `dropbox_api-0.1.9/src/dropbox/base.py` & `dropbox-api-0.2.0/src/dropbox/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Dropbox API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Dropbox API.
 #
 # Hive Dropbox API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -27,15 +27,15 @@
 
 __revision__ = "$LastChangedRevision$"
 """ The revision number of the module """
 
 __date__ = "$LastChangedDate$"
 """ The last change date of the module """
 
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import appier
 
@@ -44,15 +44,15 @@
 from . import shared_link
 
 BASE_URL = "https://api.dropboxapi.com/2/"
 """ The default base URL to be used when no other
 base URL value is provided to the constructor """
 
 CONTENT_URL = "https://content.dropboxapi.com/2/"
-""" The default content url to be used when no other
+""" The default content URL to be used when no other
 base URL value is provided to the constructor """
 
 ACCESS_TOKEN = None
 """ The default access token to be applied to the
 client when no other is provided """
 
 class API(
```

### Comparing `dropbox_api-0.1.9/src/dropbox/file.py` & `dropbox-api-0.2.0/src/dropbox/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Dropbox API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Dropbox API.
 #
 # Hive Dropbox API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -27,15 +27,15 @@
 
 __revision__ = "$LastChangedRevision$"
 """ The revision number of the module """
 
 __date__ = "$LastChangedDate$"
 """ The last change date of the module """
 
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import json
@@ -118,33 +118,57 @@
                 "Content-Type" : "application/octet-stream",
                 "Dropbox-API-Arg" : json.dumps(params)
             },
             timeout = timeout
         )
         return contents
 
+    def download_file(self, path):
+        url = self.content_url + "files/download"
+        params = dict(path = path)
+        contents, response = self.post(
+            url,
+            headers = {
+                "Dropbox-API-Arg" : json.dumps(params)
+            },
+            handle = True
+        )
+        result_s = response.headers.get("Dropbox-Api-Result", "{}")
+        result = json.loads(result_s)
+        return contents, result
+
     def list_folder_file(
         self,
         path,
         recursive = False,
         include_media_info = False,
         include_deleted = False,
-        include_has_explicit_shared_members = False
+        include_has_explicit_shared_members = False,
+        limit = None,
+        follow = True
     ):
         url = self.base_url + "files/list_folder"
-        contents = self.post(
-            url,
-            data_j = dict(
-                path = path,
-                recursive = recursive,
-                include_media_info = include_media_info,
-                include_deleted = include_deleted,
-                include_has_explicit_shared_members = include_has_explicit_shared_members
-            )
+        data_j = dict(
+            path = path,
+            recursive = recursive,
+            include_media_info = include_media_info,
+            include_deleted = include_deleted,
+            include_has_explicit_shared_members = include_has_explicit_shared_members
         )
+        if limit: data_j["limit"] = limit
+        contents = self.post(url, data_j = data_j)
+        contents_c = contents
+        while True:
+            has_more = contents_c.get("has_more", False)
+            cursor = contents_c.get("cursor", None)
+            if not follow: break
+            if not has_more: break
+            url = self.base_url + "files/list_folder/continue"
+            contents_c = self.post(url, data_j = dict(cursor = cursor))
+            contents["entries"] += contents_c.get("entries", [])
         return contents
 
     def upload_large_file(self, path, target, chunk_size = CHUNK_SIZE):
         cls = self.__class__
         offset = 0
         contents = self.session_start_file()
         session_id = contents["session_id"]
```

### Comparing `dropbox_api-0.1.9/src/dropbox/shared_link.py` & `dropbox-api-0.2.0/src/dropbox/shared_link.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Dropbox API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Dropbox API.
 #
 # Hive Dropbox API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -27,15 +27,15 @@
 
 __revision__ = "$LastChangedRevision$"
 """ The revision number of the module """
 
 __date__ = "$LastChangedDate$"
 """ The last change date of the module """
 
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 class SharedLinkAPI(object):
```

### Comparing `dropbox_api-0.1.9/src/dropbox/user.py` & `dropbox-api-0.2.0/src/dropbox/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Dropbox API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Dropbox API.
 #
 # Hive Dropbox API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -27,15 +27,15 @@
 
 __revision__ = "$LastChangedRevision$"
 """ The revision number of the module """
 
 __date__ = "$LastChangedDate$"
 """ The last change date of the module """
 
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 class UserAPI(object):
```

### Comparing `dropbox_api-0.1.9/setup.py` & `dropbox-api-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Dropbox API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2020 Hive Solutions Lda.
 #
 # This file is part of Hive Dropbox API.
 #
 # Hive Dropbox API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -27,26 +27,26 @@
 
 __revision__ = "$LastChangedRevision$"
 """ The revision number of the module """
 
 __date__ = "$LastChangedDate$"
 """ The last change date of the module """
 
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2020 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
-    name = "dropbox_api",
-    version = "0.1.9",
+    name = "dropbox-api",
+    version = "0.2.0",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Dropbox API Client",
     license = "Apache License, Version 2.0",
     keywords = "dropbox api",
     url = "http://dropbox-api.hive.pt",
     zip_safe = False,
@@ -69,10 +69,13 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6"
-    ]
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7"
+    ],
+    long_description = open(os.path.join(os.path.dirname(__file__), "README.md"), "rb").read().decode("utf-8"),
+    long_description_content_type = "text/markdown"
 )
```

