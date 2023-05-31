# Comparing `tmp/nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4.tar.gz` & `tmp/nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4.tar` & `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      561 2023-04-04 02:04:33.420750 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1255 2023-02-11 15:17:21.566208 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/README.md
--rw-r--r--   0        0        0     3295 2023-04-04 02:04:33.428752 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/src/nonebot_plugin_gocqhttp_cross_machine_upload_file/__init__.py
--rw-r--r--   0        0        0      497 2022-12-23 08:47:07.646836 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/src/nonebot_plugin_gocqhttp_cross_machine_upload_file/config.py
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      561 2023-05-31 13:20:10.136487 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1255 2023-02-11 15:17:21.566208 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/README.md
+-rw-r--r--   0        0        0     2763 2023-05-31 13:51:12.987805 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/src/nonebot_plugin_gocqhttp_cross_machine_upload_file/__init__.py
+-rw-r--r--   0        0        0      497 2022-12-23 08:47:07.646836 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/src/nonebot_plugin_gocqhttp_cross_machine_upload_file/config.py
+-rw-r--r--   0        0        0      132 2023-05-31 13:20:10.153488 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/src/nonebot_plugin_gocqhttp_cross_machine_upload_file/errors.py
+-rw-r--r--   0        0        0     1358 2023-05-31 13:20:10.164488 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/src/nonebot_plugin_gocqhttp_cross_machine_upload_file/file_manager.py
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/pyproject.toml` & `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gocqhttp-cross-machine-upload-file"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "nonebot_plugin_gocqhttp_cross_machine_upload_file", from = "src" }
 ]
```

### Comparing `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/README.md` & `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/src/nonebot_plugin_gocqhttp_cross_machine_upload_file/__init__.py` & `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/src/nonebot_plugin_gocqhttp_cross_machine_upload_file/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,78 @@
-import time
 from os import PathLike
 from typing import Union, AsyncIterable, Iterator
-from uuid import uuid4
 
-from fastapi import FastAPI, Path
-from nonebot import get_app
-from nonebot.adapters.onebot.v11 import Bot, MessageEvent, PrivateMessageEvent, GroupMessageEvent
-from starlette.responses import Response, FileResponse, StreamingResponse
+from nonebot import logger
+from nonebot.adapters.onebot.v11 import Bot, Event
 
 from .config import conf
+from .errors import UnsupportedDriverError
 
-_files = {}
+try:
+    from .file_manager import put_file, del_file
 
-_app: FastAPI = get_app()
+    init_failed = False
+except UnsupportedDriverError as e:
+    logger.error(e)
+    put_file = None
+    del_file = None
+    init_failed = True
 
 
-@_app.get("/file_center/{file_id}")
-async def get_file(file_id: str = Path()):
-    data = _files.get(file_id, None)
-    if data is None:
-        return Response(status_code=404)
-
-    data, path = data
-
-    if data is not None:
-        if isinstance(data, (bytes, str)):
-            return Response(data)
-        else:
-            return StreamingResponse(data)
-    else:
-        return FileResponse(path)
-
-
-async def upload_file(bot: Bot, event: MessageEvent, filename: str,
+async def upload_file(bot: Bot, event: Event, filename: str,
                       data: Union[None, bytes, str,
                                   AsyncIterable[Union[str, bytes]],
                                   Iterator[Union[str, bytes]]] = None,
                       path: Union[None, str, PathLike[str]] = None):
-    if isinstance(event, PrivateMessageEvent):
-        await upload_private_file(bot, event.user_id, filename, data, path)
-    elif isinstance(event, GroupMessageEvent):
-        await upload_group_file(bot, event.group_id, filename, data, path)
+    user_id = getattr(event, "user_id", None)
+    group_id = getattr(event, "group_id", None)
+
+    if group_id is not None:
+        await upload_group_file(bot, group_id, filename, data, path)
+    elif user_id is not None:
+        await upload_private_file(bot, user_id, filename, data, path)
     else:
         raise TypeError(event)
 
 
 async def upload_group_file(bot: Bot, group_id: int, filename: str,
                             data: Union[None, bytes, str,
                                         AsyncIterable[Union[str, bytes]],
                                         Iterator[Union[str, bytes]]] = None,
                             path: Union[None, str, PathLike[str]] = None):
-    if not data and not path:
-        raise ValueError("either data or path must be provided")
+    if init_failed:
+        raise UnsupportedDriverError()
 
-    file_id = str(uuid4()).replace('-', '')
-    _files[file_id] = (data, path)
+    file_id = put_file(data, path)
 
     download_result = await bot.download_file(
         url=f"http://{conf.callback_host}:{conf.callback_port}/file_center/{file_id}",
         thread_count=1
     )
 
     await bot.upload_group_file(group_id=group_id,
                                 file=download_result["file"],
                                 name=filename)
 
-    del _files[file_id]
+    del_file(file_id)
 
 
 async def upload_private_file(bot: Bot, user_id: int, filename: str,
                               data: Union[None, bytes, str,
                                           AsyncIterable[Union[str, bytes]],
                                           Iterator[Union[str, bytes]]] = None,
                               path: Union[None, str, PathLike[str]] = None):
-    if not data and not path:
-        raise ValueError("either data or path must be provided")
+    if init_failed:
+        raise UnsupportedDriverError()
 
-    file_id = str(uuid4()).replace('-', '')
-    _files[file_id] = (data, path)
+    file_id = put_file(data, path)
 
     download_result = await bot.download_file(
         url=f"http://{conf.callback_host}:{conf.callback_port}/file_center/{file_id}",
         thread_count=1
     )
 
     await bot.upload_private_file(user_id=user_id,
                                   file=download_result["file"],
                                   name=filename)
 
-    del _files[file_id]
+    del_file(file_id)
```

### Comparing `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.4/PKG-INFO` & `nonebot_plugin_gocqhttp_cross_machine_upload_file-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gocqhttp-cross-machine-upload-file
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

