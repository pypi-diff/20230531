# Comparing `tmp/aiodiskqueue-0.1.0b2.tar.gz` & `tmp/aiodiskqueue-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0b5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0b2.tar` & `aiodiskqueue-0.1.0b5.tar`

### file list

```diff
@@ -1,33 +1,38 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b2/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b2/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b2/.github/workflows/release.yml
--rw-r--r--   0        0        0      113 2023-05-28 13:27:18.116278 aiodiskqueue-0.1.0b2/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b2/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b2/LICENSE
--rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b2/Makefile
--rw-r--r--   0        0        0     2124 2023-05-29 15:23:28.059933 aiodiskqueue-0.1.0b2/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b2/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b2/docs/_static/custom.css
--rw-r--r--   0        0        0      110 2023-05-28 18:07:59.394553 aiodiskqueue-0.1.0b2/docs/api.rst
--rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b2/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b2/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b2/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b2/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b2/examples/basic_usage.py
--rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b2/examples/multiple_consumers.py
--rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b2/examples/single_consumer.py
--rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0      211 2023-05-29 17:44:16.835425 aiodiskqueue-0.1.0b2/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     8450 2023-05-29 17:46:19.163424 aiodiskqueue-0.1.0b2/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b2/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b2/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b2/tests/__init__.py
--rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b2/tests/factories.py
--rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b2/tests/helpers.py
--rw-r--r--   0        0        0     3158 2023-05-28 14:06:56.951355 aiodiskqueue-0.1.0b2/tests/loadtest.py
--rw-r--r--   0        0        0     7528 2023-05-29 17:32:05.539083 aiodiskqueue-0.1.0b2/tests/test_core.py
--rw-r--r--   0        0        0     2493 2023-05-28 18:39:49.776986 aiodiskqueue-0.1.0b2/tests/test_integration.py
--rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b2/tests/test_utils.py
--rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0b2/tox.ini
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b5/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b5/.github/workflows/main.yml
+-rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      155 2023-05-31 14:37:36.233099 aiodiskqueue-0.1.0b5/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b5/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b5/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b5/Makefile
+-rw-r--r--   0        0        0     2124 2023-05-29 15:23:28.059933 aiodiskqueue-0.1.0b5/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b5/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b5/docs/_static/custom.css
+-rw-r--r--   0        0        0      267 2023-05-30 15:23:45.131006 aiodiskqueue-0.1.0b5/docs/api.rst
+-rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b5/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b5/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b5/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b5/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b5/examples/basic_usage.py
+-rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b5/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b5/examples/single_consumer.py
+-rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-05-31 14:37:36.233099 aiodiskqueue-0.1.0b5/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     4218 2023-05-31 14:37:36.233099 aiodiskqueue-0.1.0b5/src/aiodiskqueue/engines.py
+-rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b5/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0     8386 2023-05-31 14:37:36.233099 aiodiskqueue-0.1.0b5/src/aiodiskqueue/queues.py
+-rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b5/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b5/tests/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b5/tests/factories.py
+-rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b5/tests/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:19:53.541514 aiodiskqueue-0.1.0b5/tests/measurements/__init__.py
+-rw-r--r--   0        0        0    49220 2023-05-31 14:37:36.237100 aiodiskqueue-0.1.0b5/tests/measurements/analysis.ipynb
+-rw-r--r--   0        0        0      370 2023-05-31 14:37:36.237100 aiodiskqueue-0.1.0b5/tests/measurements/config.toml
+-rw-r--r--   0        0        0       17 2023-05-30 10:40:38.676516 aiodiskqueue-0.1.0b5/tests/measurements/requirements.txt
+-rw-r--r--   0        0        0     5825 2023-05-31 14:37:36.237100 aiodiskqueue-0.1.0b5/tests/measurements/run.py
+-rw-r--r--   0        0        0     2495 2023-05-30 13:21:08.625414 aiodiskqueue-0.1.0b5/tests/test_integration.py
+-rw-r--r--   0        0        0     8297 2023-05-31 14:37:36.237100 aiodiskqueue-0.1.0b5/tests/test_queues.py
+-rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b5/tests/test_utils.py
+-rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0b5/tox.ini
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b5/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0b2/.github/workflows/main.yml` & `aiodiskqueue-0.1.0b5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/.github/workflows/release.yml` & `aiodiskqueue-0.1.0b5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/LICENSE` & `aiodiskqueue-0.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/README.rst` & `aiodiskqueue-0.1.0b5/README.rst`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/docs/Makefile` & `aiodiskqueue-0.1.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/docs/conf.py` & `aiodiskqueue-0.1.0b5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/docs/make.bat` & `aiodiskqueue-0.1.0b5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0b5/examples/multiple_consumers.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/examples/single_consumer.py` & `aiodiskqueue-0.1.0b5/examples/single_consumer.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/pyproject.toml` & `aiodiskqueue-0.1.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/src/aiodiskqueue/core.py` & `aiodiskqueue-0.1.0b5/src/aiodiskqueue/queues.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Core implementation of a persistent AsyncIO queue."""
+
 import asyncio
 import logging
-import pickle
 from pathlib import Path
 from typing import Any, Union
 
 import aiofiles
 import aiofiles.os
 
+from aiodiskqueue.engines import PickledList, _StorageEngine
 from aiodiskqueue.exceptions import QueueEmpty, QueueFull
 from aiodiskqueue.utils import NoDirectInstantiation
 
 logger = logging.getLogger(__name__)
 
 
 class Queue(metaclass=NoDirectInstantiation):
@@ -21,29 +22,36 @@
     This file only exists temporarily while there are items in the queue.
 
     This class is not thread safe.
 
     To create a new object the factory method :func:`create` must be used.
     """
 
-    def __init__(self, data_path: Path, maxsize: int, queue: list) -> None:
+    def __init__(
+        self,
+        data_path: Path,
+        maxsize: int,
+        queue: list,
+        storage_engine: _StorageEngine,
+    ) -> None:
         """Direct instantiation would break the persistance feature
         and has therefore been disabled.
 
         :meta private:
         """
         self._data_path = Path(data_path)
         self._maxsize = max(0, maxsize)
         self._queue_lock = asyncio.Lock()
         self._has_new_item = asyncio.Condition()
         self._has_free_slots = asyncio.Condition()
         self._tasks_are_finished = asyncio.Condition()
         self._unfinished_tasks = 0
         self._peak_size = len(queue)  # measuring peak size of the queue
         self._queue = list(queue)
+        self._storage_engine = storage_engine
 
     @property
     def maxsize(self) -> int:
         """Number of items allowed in the queue. 0 means unlimited."""
         return self._maxsize
 
     def empty(self) -> bool:
@@ -129,15 +137,18 @@
         Args:
             item: Any Python object that can be pickled
         """
         async with self._queue_lock:
             if self._maxsize and self.qsize() >= self._maxsize:
                 raise QueueFull
             self._queue.append(item)
-            await self._write_queue()
+            if self._storage_engine.can_append:
+                await self._storage_engine.append_item(item)
+            else:
+                await self._storage_engine.save_all_items(self._queue)
             async with self._tasks_are_finished:
                 self._unfinished_tasks += 1
 
         async with self._has_new_item:
             self._has_new_item.notify()
 
     def qsize(self) -> int:
@@ -166,69 +177,59 @@
                 raise ValueError("task_done() called too many times")
 
             self._unfinished_tasks -= 1
             if self._unfinished_tasks == 0:
                 self._tasks_are_finished.notify_all()
 
     async def _write_queue(self):
-        await self._write_queue_to_path(self._data_path, self._queue)
+        await self._storage_engine.save_all_items(self._queue)
         size = self.qsize()
         self._peak_size = max(self._peak_size, size)
         logger.debug("Wrote queue with %d items: %s", size, self._data_path)
 
-    @staticmethod
-    async def _write_queue_to_path(data_path: Path, queue: list):
-        async with aiofiles.open(
-            data_path, "wb", buffering=0
-        ) as fp:  # buffering is disabled to prevent the unclosed file issue.
-            await fp.write(pickle.dumps(queue))
-
     @classmethod
-    async def _read_queue(cls, data_path: Path) -> list:
-        try:
-            async with aiofiles.open(data_path, "rb", buffering=0) as fp:
-                data = await fp.read()
-        except FileNotFoundError:
-            await cls._write_queue_to_path(data_path, [])  # ensuring early we can write
-            await aiofiles.os.remove(data_path)
-            return []
-
-        try:
-            queue = pickle.loads(data)
-        except pickle.PickleError:
-            backup_path = data_path.with_suffix(".bak")
-            await aiofiles.os.rename(data_path, backup_path)
-            logger.exception(
-                "Data file is corrupt and has been backed up: %s", backup_path
-            )
-            return []
-
-        logger.info(
-            "Resurrecting queue with %d items from: %s",
-            len(queue),
-            data_path,
-        )
-        return queue
-
-    @classmethod
-    async def create(cls, data_path: Union[str, Path], maxsize: int = 0) -> "Queue":
+    async def create(
+        cls,
+        data_path: Union[str, Path],
+        maxsize: int = 0,
+        cls_storage_engine=None,
+    ) -> "Queue":
         """Create a new queue instance.
 
         A data file will be created at the given path if it does not already exist.
 
-        If the data file already exists, if will be used to recreate the queue if possible.
-        Should that fail, the existing data file will be backed up and the queue reset.
+        If the data file already exists, if will be used to recreate the queue
+        if possible. Should that fail, the existing data file will be backed up
+        and the queue reset.
 
         Please note that using two different instances with the same data file
         simultaneously is not recommended as it may lead to data corruption.
 
         Args:
             data_path: Path of the data file for this queue. e.g. `queue.dat`
-            maxsize: If maxsize is less than or equal to zero, the queue size is infinite.
+            maxsize: If maxsize is less than or equal to zero,
+                the queue size is infinite.
                 If it is an integer greater than 0, then put() blocks
                 when the queue reaches maxsize until an item is removed by get().
+            cls_storage_engine: Define the storage engine to be used.
+                Default is :class:`.PickleSequence`.
         """
         data_path = Path(data_path)
         if data_path.suffix == ".bak":
             raise ValueError("Invalid file name: .bak suffix is reserved for backups")
-        queue = await cls._read_queue(data_path)
-        return cls._create(data_path, maxsize, queue)
+
+        if not cls_storage_engine:
+            cls_storage_engine = PickledList
+        else:
+            if not issubclass(cls_storage_engine, _StorageEngine):
+                raise TypeError("Invalid storage engine")
+        storage_engine = cls_storage_engine(data_path)
+        queue = await storage_engine.load_all_items()
+        if not queue:
+            await storage_engine.save_all_items([])  # ensuring early we can write
+            await aiofiles.os.remove(data_path)
+        else:
+            logger.info(
+                "Read %d items from existing data file: %s", len(queue), data_path
+            )
+
+        return cls._create(data_path, maxsize, queue, storage_engine)
```

### Comparing `aiodiskqueue-0.1.0b2/src/aiodiskqueue/utils.py` & `aiodiskqueue-0.1.0b5/src/aiodiskqueue/utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/tests/factories.py` & `aiodiskqueue-0.1.0b5/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/tests/test_core.py` & `aiodiskqueue-0.1.0b5/tests/test_queues.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 
 import aiofiles
 import aiofiles.os
 
 from aiodiskqueue import Queue, QueueEmpty, QueueFull
+from aiodiskqueue.engines import PickledList, PickleSequence
 
 from .factories import ItemFactory
 from .helpers import QueueAsyncioTestCase
 
 
 class TestCreateQueue(QueueAsyncioTestCase):
     async def test_should_create_queue_and_measure_size(self):
@@ -72,14 +73,31 @@
         del queue_1
         # when
         queue_2 = await Queue.create(self.data_path)
         # then
         item_new = await queue_2.get()
         self.assertEqual(item_new, item)
 
+    async def test_should_create_queue_with_storage_engine_1(self):
+        # given
+        q = await Queue.create(self.data_path, cls_storage_engine=PickleSequence)
+        # when/then
+        self.assertIsInstance(q._storage_engine, PickleSequence)
+
+    async def test_should_create_queue_with_storage_engine_2(self):
+        # given
+        q = await Queue.create(self.data_path, cls_storage_engine=PickledList)
+        # when/then
+        self.assertIsInstance(q._storage_engine, PickledList)
+
+    async def test_should_raise_error_when_storage_engine_not_valid(self):
+        # when/then
+        with self.assertRaises(TypeError):
+            await Queue.create(self.data_path, cls_storage_engine=str)
+
 
 class TestPutIntoQueue(QueueAsyncioTestCase):
     async def test_should_put_items_and_measure_size(self):
         # given
         q = await Queue.create(self.data_path)
         # when
         await q.put_nowait(ItemFactory())
```

### Comparing `aiodiskqueue-0.1.0b2/tests/test_integration.py` & `aiodiskqueue-0.1.0b5/tests/test_integration.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,43 +8,43 @@
 
 logger = logging.getLogger(__name__)
 
 
 async def producer(
     source_queue: asyncio.Queue, disk_queue: aiodiskqueue.Queue, num: int
 ):
-    logger.info("Starting producer %d", num)
+    logger.debug("Starting producer %d", num)
     while True:
         try:
             item = source_queue.get_nowait()
         except asyncio.QueueEmpty:
-            logger.info("Stopping producer %d", num)
+            logger.debug("Stopping producer %d", num)
             return
         else:
             await disk_queue.put(item)
 
 
 async def consumer(disk_queue: aiodiskqueue.Queue, result_queue: asyncio.Queue):
-    logger.info("Starting consumer")
+    logger.debug("Starting consumer")
     try:
         while True:
             item = await disk_queue.get()
             await result_queue.put(item)
             await disk_queue.task_done()
     except Exception:
         logger.exception("Consumer error")
 
 
 class TestIntegration(QueueAsyncioTestCase):
     async def test_multiple_consumer_and_producers(self):
         # parameters
-        ITEMS_AMOUNT = 500
-        PRODUCER_AMOUNT = 10
+        ITEMS_AMOUNT = 100
+        PRODUCER_AMOUNT = 5
         CONSUMER_AMOUNT = 2
-        DISKQUEUE_MAXSIZE = 100
+        DISKQUEUE_MAXSIZE = 50
 
         # create queues
         source_queue = asyncio.Queue()
         disk_queue = await aiodiskqueue.Queue.create(
             self.data_path, maxsize=DISKQUEUE_MAXSIZE
         )
         result_queue = asyncio.Queue()
@@ -62,15 +62,15 @@
         producers = [
             producer(source_queue, disk_queue, num + 1)
             for num in range(PRODUCER_AMOUNT)
         ]
         await asyncio.gather(*producers)
 
         # wait for consumers to finish
-        logger.info("Waiting for consumers to complete...")
+        logger.debug("Waiting for consumers to complete...")
         await disk_queue.join()
         for task in consumer_tasks:
             task.cancel()
 
         # Extract result items
         result_items = set()
         while True:
```

### Comparing `aiodiskqueue-0.1.0b2/tests/test_utils.py` & `aiodiskqueue-0.1.0b5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b2/PKG-INFO` & `aiodiskqueue-0.1.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0b2
+Version: 0.1.0b5
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

