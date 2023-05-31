# Comparing `tmp/fps_yjs-0.1.6.tar.gz` & `tmp/fps_yjs-0.1.7.tar.gz`

## Comparing `fps_yjs-0.1.6.tar` & `fps_yjs-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/fps_yjs/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/fps_yjs/py.typed
--rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/fps_yjs/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/COPYING.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/fps_yjs/py.typed
+-rw-r--r--   0        0        0    14935 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/fps_yjs/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/COPYING.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/README.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fps_yjs-0.1.7/PKG-INFO
```

### Comparing `fps_yjs-0.1.6/fps_yjs/main.py` & `fps_yjs-0.1.7/fps_yjs/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from collections.abc import AsyncGenerator
 from typing import Optional
 
 from asphalt.core import Component, Context, context_teardown
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth
 from jupyverse_api.contents import Contents
@@ -25,9 +26,10 @@
         ctx.add_resource(yjs, types=Yjs)
 
         # start indexing in the background
         contents.file_id_manager
 
         yield
 
+        yjs.room_manager.stop()
         contents.file_id_manager.stop_watching_files.set()
         await contents.file_id_manager.stopped_watching_files.wait()
```

### Comparing `fps_yjs-0.1.6/fps_yjs/routes.py` & `fps_yjs-0.1.7/fps_yjs/routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,106 @@
+from __future__ import annotations
+
 import asyncio
+import logging
 from datetime import datetime
-from pathlib import Path
-from typing import Optional, Tuple, cast
+from functools import partial
+from typing import Dict
 from uuid import uuid4
 
 from fastapi import (
     HTTPException,
     Request,
     Response,
     WebSocketDisconnect,
     status,
 )
-from jupyter_ydoc import ydocs as YDOCS  # type: ignore
+from jupyter_ydoc import ydocs as YDOCS
+from jupyter_ydoc.ybasedoc import YBaseDoc
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.contents import Contents
 from jupyverse_api.yjs import Yjs
 from jupyverse_api.yjs.models import CreateDocumentSession
+from websockets.exceptions import ConnectionClosedOK
 from ypy_websocket.websocket_server import WebsocketServer, YRoom
-from ypy_websocket.ystore import BaseYStore, SQLiteYStore, YDocNotFound
+from ypy_websocket.ystore import SQLiteYStore, YDocNotFound
 from ypy_websocket.yutils import YMessageType, YSyncMessageType
 
 YFILE = YDOCS["file"]
 AWARENESS = 1
-RENAME_SESSION = 127
 SERVER_SESSION = uuid4().hex
+logger = logging.getLogger("yjs")
 
 
 class JupyterSQLiteYStore(SQLiteYStore):
-    db_path = ".jupyter_ystore.db"
+    db_path = ".jupyter_ystore.db"  # FIXME: pass in config
 
 
 class _Yjs(Yjs):
     def __init__(
         self,
         app: App,
         auth: Auth,
         contents: Contents,
     ) -> None:
         super().__init__(app=app, auth=auth)
         self.contents = contents
-        self.websocket_server = YDocWebSocketHandler.websocket_server
-
-    async def serve_room(self, websocket_permissions, path):
-        if websocket_permissions is None:
-            return
-        websocket, permissions = websocket_permissions
-        await websocket.accept()
-        socket = YDocWebSocketHandler(
-            WebsocketAdapter(websocket, path), path, permissions, self.contents
-        )
-        await socket.serve()
-
-    async def yjs_websocket(
-        self,
-        path,
-        websocket_permissions,
-    ):
-        await self.serve_room(websocket_permissions, path)
+        self.room_manager = RoomManager(contents)
 
     async def collaboration_room_websocket(
         self,
         path,
         websocket_permissions,
     ):
-        await self.serve_room(websocket_permissions, path)
+        if websocket_permissions is None:
+            return
+        websocket, permissions = websocket_permissions
+        await websocket.accept()
+        ypy_websocket = YpyWebsocket(websocket, path)
+        await self.room_manager.serve(ypy_websocket, permissions)
 
     async def create_roomid(
         self,
         path,
         request: Request,
         response: Response,
         user: User,
     ):
         # we need to process the request manually
         # see https://github.com/tiangolo/fastapi/issues/3373#issuecomment-1306003451
         create_document_session = CreateDocumentSession(**(await request.json()))
         idx = await self.contents.file_id_manager.get_id(path)
+        res = {
+            "format": create_document_session.format,
+            "type": create_document_session.type,
+            "sessionId": SERVER_SESSION,
+        }
         if idx is not None:
-            return {
-                "format": create_document_session.format,
-                "type": create_document_session.type,
-                "fileId": idx,
-                "sessionId": SERVER_SESSION,
-            }
+            res["fileId"] = idx
+            return res
 
         idx = await self.contents.file_id_manager.index(path)
         if idx is None:
             raise HTTPException(status_code=404, detail=f"File {path} does not exist")
 
         response.status_code = status.HTTP_201_CREATED
-        return {
-            "format": create_document_session.format,
-            "type": create_document_session.type,
-            "fileId": idx,
-            "sessionId": SERVER_SESSION,
-        }
+        res["fileId"] = idx
+        return res
+
+    def get_document(self, document_id: str) -> YBaseDoc:
+        return self.room_manager.documents[document_id]
 
 
 def to_datetime(iso_date: str) -> datetime:
     return datetime.fromisoformat(iso_date.rstrip("Z"))
 
 
-class WebsocketAdapter:
-    """An adapter to make a Starlette's WebSocket look like a ypy-websocket's WebSocket"""
+class YpyWebsocket:
+    """An wrapper to make a Starlette's WebSocket look like a ypy-websocket's WebSocket"""
 
     def __init__(self, websocket, path: str):
         self._websocket = websocket
         self._path = path
 
     @property
     def path(self) -> str:
@@ -124,232 +117,250 @@
         try:
             message = await self._websocket.receive_bytes()
         except WebSocketDisconnect:
             raise StopAsyncIteration()
         return message
 
     async def send(self, message):
-        await self._websocket.send_bytes(message)
+        try:
+            await self._websocket.send_bytes(message)
+        except ConnectionClosedOK:
+            return
 
     async def recv(self):
         return await self._websocket.receive_bytes()
 
 
-class DocumentRoom(YRoom):
-    """A Y room for a possibly stored document (e.g. a notebook)."""
-
-    is_transient = False
-
-    def __init__(self, type: str, ystore: BaseYStore):
-        super().__init__(ready=False, ystore=ystore)
-        self.type = type
-        self.cleaner = None
-        self.watcher = None
-        self.document = YDOCS.get(type, YFILE)(self.ydoc)
-
-
-class TransientRoom(YRoom):
-    """A Y room for sharing state (e.g. awareness)."""
-
-    is_transient = True
-
+class RoomManager:
+    contents: Contents
+    documents: Dict[str, YBaseDoc]
+    watchers: Dict[str, asyncio.Task]
+    savers: Dict[str, asyncio.Task]
+    cleaners: Dict[YRoom, asyncio.Task]
+    last_modified: Dict[str, datetime]
+    websocket_server: JupyterWebsocketServer
+    lock: asyncio.Lock
 
-class JupyterWebsocketServer(WebsocketServer):
-    def get_room(self, path: str) -> YRoom:
-        if path not in self.rooms.keys():
-            if path.count(":") >= 2:
-                # it is a stored document (e.g. a notebook)
-                file_format, file_type, file_path = path.split(":", 2)
-                p = Path(file_path)
-                updates_file_path = (p.parent / f".{file_type}:{p.name}.y").as_posix()
-                ystore = JupyterSQLiteYStore(path=updates_file_path)  # FIXME: pass in config
-                self.rooms[path] = DocumentRoom(file_type, ystore)
-            else:
-                # it is a transient document (e.g. awareness)
-                self.rooms[path] = TransientRoom()
-        return self.rooms[path]
-
-
-class YDocWebSocketHandler:
-    saving_document: Optional[asyncio.Task]
-    websocket_server = JupyterWebsocketServer(rooms_ready=False, auto_clean_rooms=False)
-
-    def __init__(self, websocket, path, permissions, contents: Contents):
-        self.websocket = websocket
+    def __init__(self, contents: Contents):
         self.contents = contents
-        self.can_write = permissions is None or "write" in permissions.get("yjs", [])
+        self.documents = {}  # a dictionary of room_name:document
+        self.watchers = {}  # a dictionary of file_id:task
+        self.savers = {}  # a dictionary of file_id:task
+        self.cleaners = {}  # a dictionary of room:task
+        self.last_modified = {}  # a dictionary of file_id:last_modification_date
+        self.websocket_server = JupyterWebsocketServer(rooms_ready=False, auto_clean_rooms=False)
         self.lock = asyncio.Lock()
-        self.room = self.websocket_server.get_room(self.websocket.path)
-        self.set_file_info(path)
 
-    async def get_file_info(self) -> Tuple[str, str, str]:
-        room_name = self.websocket_server.get_room_name(self.room)
-        file_format, file_type, file_id = room_name.split(":", 2)
-        file_path = await self.contents.file_id_manager.get_path(file_id)
-        room = cast(DocumentRoom, self.room)
-        if file_path is None:
-            raise RuntimeError(f"File {room.document.path} cannot be found anymore")
-        if file_path != room.document.path:
-            room.document.path = file_path
-        return file_format, file_type, file_path
-
-    def set_file_info(self, value: str) -> None:
-        self.websocket_server.rename_room(value, from_room=self.room)
-        self.websocket.path = value
-
-    async def serve(self):
-        self.set_file_info(self.websocket.path)
-        self.saving_document = None
-        self.room.on_message = self.on_message
-
-        # cancel the deletion of the room if it was scheduled
-        if not self.room.is_transient and self.room.cleaner is not None:
-            self.room.cleaner.cancel()
-
-        if not self.room.is_transient and not self.room.ready:
-            file_format, file_type, file_path = await self.get_file_info()
-            is_notebook = file_type == "notebook"
-            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
-            self.last_modified = to_datetime(model.last_modified)
-            # check again if ready, because loading the file is async
-            if not self.room.ready:
-                # try to apply Y updates from the YStore for this document
-                try:
-                    await self.room.ystore.apply_updates(self.room.ydoc)
-                    read_from_source = False
-                except YDocNotFound:
-                    # YDoc not found in the YStore, create the document from
-                    # the source file (no change history)
-                    read_from_source = True
-                if not read_from_source:
-                    # if YStore updates and source file are out-of-sync, resync updates
-                    # with source
-                    if self.room.document.source != model.content:
+    def stop(self):
+        for watcher in self.watchers.values():
+            watcher.cancel()
+        for saver in self.savers.values():
+            saver.cancel()
+        for cleaner in self.cleaners.values():
+            cleaner.cancel()
+
+    async def serve(self, websocket: YpyWebsocket, permissions) -> None:
+        room = self.websocket_server.get_room(websocket.path)
+        can_write = permissions is None or "write" in permissions.get("yjs", [])
+        room.on_message = partial(self.filter_message, can_write)
+        is_stored_document = websocket.path.count(":") >= 2
+        if is_stored_document:
+            assert room.ystore is not None
+            file_format, file_type, file_id = websocket.path.split(":", 2)
+            if room in self.cleaners:
+                # cleaning the room was scheduled because there was no client left
+                # cancel that since there is a new client
+                self.cleaners[room].cancel()
+            if not room.ready:
+                file_path = await self.contents.file_id_manager.get_path(file_id)
+                logger.info(f"Opening collaboration room: {websocket.path} ({file_path})")
+                document = YDOCS.get(file_type, YFILE)(room.ydoc)
+                self.documents[websocket.path] = document
+                is_notebook = file_type == "notebook"
+                async with self.lock:
+                    model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+                assert model.last_modified is not None
+                self.last_modified[file_id] = to_datetime(model.last_modified)
+                if not room.ready:
+                    # try to apply Y updates from the YStore for this document
+                    try:
+                        await room.ystore.apply_updates(room.ydoc)
+                        read_from_source = False
+                    except YDocNotFound:
+                        # YDoc not found in the YStore, create the document from
+                        # the source file (no change history)
                         read_from_source = True
-                if read_from_source:
-                    self.room.document.source = model.content
-                    await self.room.ystore.encode_state_as_update(self.room.ydoc)
-
-                self.room.document.dirty = False
-                self.room.ready = True
-                self.room.watcher = asyncio.create_task(self.watch_file())
-                # save the document when changed
-                self.room.document.observe(self.on_document_change)
+                    if not read_from_source:
+                        # if YStore updates and source file are out-of-sync, resync updates
+                        # with source
+                        if document.source != model.content:
+                            read_from_source = True
+                    if read_from_source:
+                        document.source = model.content
+                        await room.ystore.encode_state_as_update(room.ydoc)
+
+                    document.dirty = False
+                    room.ready = True
+                    # save the document to file when changed
+                    document.observe(partial(self.on_document_change, file_id, file_type, document))
+                    # update the document when file changes
+                    if file_id not in self.watchers:
+                        self.watchers[file_id] = asyncio.create_task(
+                            self.watch_file(file_type, file_id, document)
+                        )
 
-        await self.websocket_server.serve(self.websocket)
-        if not self.room.is_transient and not self.room.clients:
+        await self.websocket_server.serve(websocket)
+
+        if is_stored_document and not room.clients:
             # no client in this room after we disconnect
-            # keep the document for a while in case someone reconnects
-            self.room.cleaner = asyncio.create_task(self.clean_room())
+            self.cleaners[room] = asyncio.create_task(self.maybe_clean_room(room, websocket.path))
 
-    async def on_message(self, message: bytes) -> bool:
+    async def filter_message(self, can_write: bool, message: bytes) -> bool:
         """
         Called whenever a message is received, before forwarding it to other clients.
 
-        :param message: received message
+        :param can_write: True if updating the document is permitted, False otherwise.
+        :param message: received message.
         :returns: True if the message must be discarded, False otherwise (default: False).
         """
         skip = False
         byte = message[0]
         msg = message[1:]
-        if byte == RENAME_SESSION:
-            # The client moved the document to a different location. After receiving this
-            # message, we make the current document available under a different url.
-            # The other clients are automatically notified of this change because
-            # the path is shared through the Yjs document as well.
-            new_room_name = msg.decode("utf-8")
-            self.set_file_info(new_room_name)
-            self.websocket_server.rename_room(new_room_name, from_room=self.room)
-            # send rename acknowledge
-            await self.websocket.send(bytes([RENAME_SESSION, 1]))
-        elif byte == AWARENESS:
+        if byte == AWARENESS:
             # changes = self.room.awareness.get_changes(msg)
             # # filter out message depending on changes
             # skip = True
             pass
         elif byte == YMessageType.SYNC:
-            if not self.can_write and msg[0] == YSyncMessageType.SYNC_UPDATE:
+            if not can_write and msg[0] == YSyncMessageType.SYNC_UPDATE:
                 skip = True
         else:
             skip = True
         return skip
 
-    async def watch_file(self):
-        file_format, file_type, file_path = await self.get_file_info()
+    async def get_file_path(self, file_id: str, document) -> str | None:
+        file_path = await self.contents.file_id_manager.get_path(file_id)
+        if file_path is None:
+            return
+        if file_path != document.path:
+            document.path = file_path
+        return file_path
+
+    async def watch_file(self, file_type: str, file_id: str, document: YBaseDoc) -> None:
+        file_path = await self.get_file_path(file_id, document)
+        assert file_path is not None
+        logger.debug(f"Watching file: {file_path}")
         while True:
             watcher = self.contents.file_id_manager.watch(file_path)
             async for changes in watcher:
-                file_format, file_type, new_file_path = await self.get_file_info()
+                new_file_path = await self.get_file_path(file_id, document)
+                if new_file_path is None:
+                    continue
                 if new_file_path != file_path:
                     # file was renamed
                     self.contents.file_id_manager.unwatch(file_path, watcher)
                     file_path = new_file_path
-                    break
-                await self.maybe_load_document()
+                    # break
+                await self.maybe_load_file(file_type, file_path, file_id)
 
-    async def maybe_load_document(self):
-        file_format, file_type, file_path = await self.get_file_info()
+    async def maybe_load_file(self, file_type: str, file_path: str, file_id: str) -> None:
         async with self.lock:
             model = await self.contents.read_content(file_path, False)
         # do nothing if the file was saved by us
-        if self.last_modified < to_datetime(model.last_modified):
+        assert model.last_modified is not None
+        if self.last_modified[file_id] < to_datetime(model.last_modified):
+            # the file was not saved by us, update the shared document(s)
             is_notebook = file_type == "notebook"
-            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
-            self.room.document.source = model.content
-            self.last_modified = to_datetime(model.last_modified)
-
-    async def clean_room(self) -> None:
-        await asyncio.sleep(60)  # FIXME: pass in config
-        room = cast(DocumentRoom, self.room)
-        if room.watcher:
-            room.watcher.cancel()
-        room.document.unobserve()
-        self.websocket_server.delete_room(room=room)
+            async with self.lock:
+                model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+            assert model.last_modified is not None
+            documents = [v for k, v in self.documents.items() if k.split(":", 2)[2] == file_id]
+            for document in documents:
+                document.source = model.content
+            self.last_modified[file_id] = to_datetime(model.last_modified)
 
-    def on_document_change(self, target, event):
+    def on_document_change(
+        self, file_id: str, file_type: str, document: YBaseDoc, target, event
+    ) -> None:
         if target == "state" and "dirty" in event.keys:
             dirty = event.keys["dirty"]["newValue"]
             if not dirty:
                 # we cleared the dirty flag, nothing to save
                 return
         # unobserve and observe again because the structure of the document may have changed
         # e.g. a new cell added to a notebook
-        self.room.document.unobserve()
-        self.room.document.observe(self.on_document_change)
-        if self.saving_document is not None and not self.saving_document.done():
-            # the document is being saved, cancel that
-            self.saving_document.cancel()
-            self.saving_document = None
-        self.saving_document = asyncio.create_task(self.maybe_save_document())
+        document.unobserve()
+        document.observe(partial(self.on_document_change, file_id, file_type, document))
+        if file_id in self.savers:
+            self.savers[file_id].cancel()
+        self.savers[file_id] = asyncio.create_task(
+            self.maybe_save_document(file_id, file_type, document)
+        )
 
-    async def maybe_save_document(self):
+    async def maybe_save_document(self, file_id: str, file_type: str, document: YBaseDoc) -> None:
         # save after 1 second of inactivity to prevent too frequent saving
-        await asyncio.sleep(1)
+        await asyncio.sleep(1)  # FIXME: pass in config
         # if the room cannot be found, don't save
         try:
-            file_format, file_type, file_path = await self.get_file_info()
-        except Exception:
+            file_path = await self.get_file_path(file_id, document)
+        except BaseException:
             return
+        assert file_path is not None
         is_notebook = file_type == "notebook"
         async with self.lock:
             model = await self.contents.read_content(file_path, True, as_json=is_notebook)
-        if self.last_modified < to_datetime(model.last_modified):
+        assert model.last_modified is not None
+        if self.last_modified[file_id] < to_datetime(model.last_modified):
             # file changed on disk, let's revert
-            self.room.document.source = model.content
-            self.last_modified = to_datetime(model.last_modified)
+            document.source = model.content
+            self.last_modified[file_id] = to_datetime(model.last_modified)
             return
-        if model.content != self.room.document.source:
+        if model.content != document.source:
             # don't save if not needed
             # this also prevents the dirty flag from bouncing between windows of
             # the same document opened as different types (e.g. notebook/text editor)
             format = "json" if file_type == "notebook" else "text"
             content = {
-                "content": self.room.document.source,
+                "content": document.source,
                 "format": format,
                 "path": file_path,
                 "type": file_type,
             }
             async with self.lock:
                 await self.contents.write_content(content)
                 model = await self.contents.read_content(file_path, False)
-                self.last_modified = to_datetime(model.last_modified)
-        self.room.document.dirty = False
+            assert model.last_modified is not None
+            self.last_modified[file_id] = to_datetime(model.last_modified)
+        document.dirty = False
+        # we're done saving, remove the saver
+        del self.savers[file_id]
+
+    async def maybe_clean_room(self, room, ws_path: str) -> None:
+        file_id = ws_path.split(":", 2)[2]
+        # keep the document for a while in case someone reconnects
+        await asyncio.sleep(60)  # FIXME: pass in config
+        document = self.documents[ws_path]
+        document.unobserve()
+        del self.documents[ws_path]
+        documents = [v for k, v in self.documents.items() if k.split(":", 2)[2] == file_id]
+        if not documents:
+            self.watchers[file_id].cancel()
+            del self.watchers[file_id]
+        room_name = self.websocket_server.get_room_name(room)
+        self.websocket_server.delete_room(room=room)
+        file_path = await self.get_file_path(file_id, document)
+        logger.info(f"Closing collaboration room: {room_name} ({file_path})")
+
+
+class JupyterWebsocketServer(WebsocketServer):
+    def get_room(self, ws_path: str) -> YRoom:
+        if ws_path not in self.rooms:
+            if ws_path.count(":") >= 2:
+                # it is a stored document (e.g. a notebook)
+                file_format, file_type, file_id = ws_path.split(":", 2)
+                updates_file_path = f".{file_type}:{file_id}.y"
+                ystore = JupyterSQLiteYStore(path=updates_file_path)  # FIXME: pass in config
+                self.rooms[ws_path] = YRoom(ready=False, ystore=ystore)
+            else:
+                # it is a transient document (e.g. awareness)
+                self.rooms[ws_path] = YRoom()
+        return self.rooms[ws_path]
```

### Comparing `fps_yjs-0.1.6/.gitignore` & `fps_yjs-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.6/COPYING.md` & `fps_yjs-0.1.7/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.6/pyproject.toml` & `fps_yjs-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.6/PKG-INFO` & `fps_yjs-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_yjs
-Version: 0.1.6
+Version: 0.1.7
 Summary: An FPS plugin for the Yjs API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

