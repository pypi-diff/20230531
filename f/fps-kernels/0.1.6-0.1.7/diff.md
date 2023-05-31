# Comparing `tmp/fps_kernels-0.1.6.tar.gz` & `tmp/fps_kernels-0.1.7.tar.gz`

## Comparing `fps_kernels-0.1.6.tar` & `fps_kernels-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/main.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/COPYING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/main.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/COPYING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.1.7/PKG-INFO
```

### Comparing `fps_kernels-0.1.6/fps_kernels/main.py` & `fps_kernels-0.1.7/fps_kernels/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 import asyncio
-import logging
 from collections.abc import AsyncGenerator
 from pathlib import Path
 from typing import Optional
 
 from asphalt.core import Component, Context, context_teardown
 
 from jupyverse_api.auth import Auth
@@ -12,17 +11,14 @@
 from jupyverse_api.kernels import Kernels, KernelsConfig
 from jupyverse_api.yjs import Yjs
 from jupyverse_api.app import App
 
 from .routes import _Kernels
 
 
-logger = logging.getLogger("kernels")
-
-
 class KernelsComponent(Component):
     def __init__(self, **kwargs):
         self.kernels_config = KernelsConfig(**kwargs)
 
     @context_teardown
     async def start(
         self,
```

### Comparing `fps_kernels-0.1.6/fps_kernels/routes.py` & `fps_kernels-0.1.7/fps_kernels/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 import uuid
 from http import HTTPStatus
 from pathlib import Path
 from typing import Dict, List, Optional, Set, Tuple
 
 from fastapi import HTTPException, Response
 from fastapi.responses import FileResponse
@@ -20,14 +21,17 @@
 from .kernel_server.server import (
     AcceptedWebSocket,
     KernelServer,
     kernels,
 )
 
 
+logger = logging.getLogger("kernels")
+
+
 class _Kernels(Kernels):
     def __init__(
         self,
         app: App,
         kernels_config: KernelsConfig,
         auth: Auth,
         frontend_config: FrontendConfig,
@@ -142,17 +146,22 @@
         user: User,
     ):
         create_session = CreateSession(**(await request.json()))
         kernel_id = create_session.kernel.id
         kernel_name = create_session.kernel.name
         if kernel_name is not None:
             # launch a new ("internal") kernel
+            kernel_cwd = Path(create_session.path).parent
+            while True:
+                if kernel_cwd.is_dir():
+                    break
+                kernel_cwd = kernel_cwd.parent
             kernel_server = KernelServer(
                 kernelspec_path=Path(find_kernelspec(kernel_name)).as_posix(),
-                kernel_cwd=str(Path(create_session.path).parent),
+                kernel_cwd=str(kernel_cwd),
             )
             kernel_id = str(uuid.uuid4())
             kernels[kernel_id] = {"name": kernel_name, "server": kernel_server, "driver": None}
             await kernel_server.start()
         elif kernel_id is not None:
             # external kernel
             kernel_name = kernels[kernel_id]["name"]
@@ -227,15 +236,15 @@
     ):
         if self.yjs is None:
             raise RuntimeError("Cannot execute without a Yjs plugin.")
 
         r = await request.json()
         execution = Execution(**r)
         if kernel_id in kernels:
-            ynotebook = self.yjs.websocket_server.get_room(execution.document_id).document
+            ynotebook = self.yjs.get_document(execution.document_id)
             cell = ynotebook.get_cell(execution.cell_idx)
             cell["outputs"] = []
 
             kernel = kernels[kernel_id]
             if not kernel["driver"]:
                 kernel["driver"] = driver = KernelDriver(
                     kernelspec_path=Path(find_kernelspec(kernel["name"])).as_posix(),
```

### Comparing `fps_kernels-0.1.6/fps_kernels/kernel_driver/connect.py` & `fps_kernels-0.1.7/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/fps_kernels/kernel_driver/driver.py` & `fps_kernels-0.1.7/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/fps_kernels/kernel_driver/kernelspec.py` & `fps_kernels-0.1.7/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/fps_kernels/kernel_driver/message.py` & `fps_kernels-0.1.7/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/fps_kernels/kernel_driver/paths.py` & `fps_kernels-0.1.7/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/fps_kernels/kernel_server/message.py` & `fps_kernels-0.1.7/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/fps_kernels/kernel_server/server.py` & `fps_kernels-0.1.7/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/.gitignore` & `fps_kernels-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/COPYING.md` & `fps_kernels-0.1.7/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/pyproject.toml` & `fps_kernels-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.6/PKG-INFO` & `fps_kernels-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_kernels
-Version: 0.1.6
+Version: 0.1.7
 Summary: An FPS plugin for the kernels API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

