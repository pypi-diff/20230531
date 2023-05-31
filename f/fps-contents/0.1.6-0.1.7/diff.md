# Comparing `tmp/fps_contents-0.1.6.tar.gz` & `tmp/fps_contents-0.1.7.tar.gz`

## Comparing `fps_contents-0.1.6.tar` & `fps_contents-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.1.6/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.1.6/fps_contents/__init__.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 fps_contents-0.1.6/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fps_contents-0.1.6/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.1.6/fps_contents/py.typed
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 fps_contents-0.1.6/fps_contents/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_contents-0.1.6/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.1.6/COPYING.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.1.6/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.1.7/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.1.7/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 fps_contents-0.1.7/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fps_contents-0.1.7/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.1.7/fps_contents/py.typed
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 fps_contents-0.1.7/fps_contents/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_contents-0.1.7/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.1.7/COPYING.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.1.7/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.1.7/PKG-INFO
```

### Comparing `fps_contents-0.1.6/fps_contents/fileid.py` & `fps_contents-0.1.7/fps_contents/fileid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import logging
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Set
 from uuid import uuid4
 
 import aiosqlite
 from anyio import Path
 from jupyverse_api import Singleton
 from watchfiles import Change, awatch
 
@@ -31,15 +31,15 @@
 
 class FileIdManager(metaclass=Singleton):
     db_path: str
     initialized: asyncio.Event
     watchers: Dict[str, List[Watcher]]
     lock: asyncio.Lock
 
-    def __init__(self, db_path: str = "fileid.db"):
+    def __init__(self, db_path: str = ".fileid.db"):
         self.db_path = db_path
         self.initialized = asyncio.Event()
         self.watchers = {}
         self.watch_files_task = asyncio.create_task(self.watch_files())
         self.stop_watching_files = asyncio.Event()
         self.stopped_watching_files = asyncio.Event()
         self.lock = asyncio.Lock()
@@ -97,16 +97,16 @@
                     )
                 await db.commit()
                 self.initialized.set()
 
         async for changes in awatch(".", stop_event=self.stop_watching_files):
             async with self.lock:
                 async with aiosqlite.connect(self.db_path) as db:
-                    deleted_paths = []
-                    added_paths = []
+                    deleted_paths = set()
+                    added_paths = set()
                     for change, changed_path in changes:
                         # get relative path
                         changed_path = Path(changed_path).relative_to(await Path().absolute())
                         changed_path_str = str(changed_path)
 
                         if change == Change.deleted:
                             logger.debug("File %s was deleted", changed_path_str)
@@ -143,24 +143,26 @@
                                     continue
                             mtime = (await changed_path.stat()).st_mtime
                             await db.execute(
                                 "UPDATE fileids SET mtime = ? WHERE path = ?",
                                 (mtime, changed_path_str),
                             )
 
-                    for path in deleted_paths + added_paths:
+                    for path in deleted_paths - added_paths:
+                        logger.debug("Unindexing file %s ", path)
                         await db.execute("DELETE FROM fileids WHERE path = ?", (path,))
                     await db.commit()
 
             for change in changes:
                 changed_path = change[1]
                 # get relative path
-                changed_path = str(Path(changed_path).relative_to(await Path().absolute()))
-                for watcher in self.watchers.get(changed_path, []):
-                    watcher.notify(change)
+                relative_changed_path = str(Path(changed_path).relative_to(await Path().absolute()))
+                relative_change = (change[0], relative_changed_path)
+                for watcher in self.watchers.get(relative_changed_path, []):
+                    watcher.notify(relative_change)
 
         self.stopped_watching_files.set()
 
     def watch(self, path: str) -> Watcher:
         watcher = Watcher(path)
         self.watchers.setdefault(path, []).append(watcher)
         return watcher
@@ -180,15 +182,15 @@
         mtime = (await Path(path).stat()).st_mtime
     except FileNotFoundError:
         return None
     return mtime
 
 
 async def maybe_rename(
-    db, changed_path: str, changed_paths: List[str], other_paths: List[str], is_added_path
+    db, changed_path: str, changed_paths: Set[str], other_paths: Set[str], is_added_path: bool
 ) -> None:
     # check if the same file was added/deleted, this would be a rename
     db_or_fs1, db_or_fs2 = db, None
     if is_added_path:
         db_or_fs1, db_or_fs2 = db_or_fs2, db_or_fs1
     mtime1 = await get_mtime(changed_path, db_or_fs1)
     if mtime1 is None:
@@ -200,8 +202,8 @@
             path1, path2 = changed_path, other_path
             if is_added_path:
                 path1, path2 = path2, path1
             logger.debug("File %s was renamed to %s", path1, path2)
             await db.execute("UPDATE fileids SET path = ? WHERE path = ?", (path2, path1))
             other_paths.remove(other_path)
             return
-    changed_paths.append(changed_path)
+    changed_paths.add(changed_path)
```

### Comparing `fps_contents-0.1.6/fps_contents/routes.py` & `fps_contents-0.1.7/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.6/.gitignore` & `fps_contents-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.6/COPYING.md` & `fps_contents-0.1.7/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.6/pyproject.toml` & `fps_contents-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.6/PKG-INFO` & `fps_contents-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_contents
-Version: 0.1.6
+Version: 0.1.7
 Summary: An FPS plugin for the contents API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

