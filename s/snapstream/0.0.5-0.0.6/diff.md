# Comparing `tmp/snapstream-0.0.5.tar.gz` & `tmp/snapstream-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapstream-0.0.5.tar", max compression
+gzip compressed data, was "snapstream-0.0.6.tar", max compression
```

## Comparing `snapstream-0.0.5.tar` & `snapstream-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-05-20 14:25:54.488845 snapstream-0.0.5/LICENSE
--rw-r--r--   0        0        0     2536 2023-05-20 14:25:54.488845 snapstream-0.0.5/README.md
--rw-r--r--   0        0        0     2034 2023-05-20 14:26:06.372835 snapstream-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2277 2023-05-20 14:25:54.492845 snapstream-0.0.5/snapstream/__init__.py
--rw-r--r--   0        0        0     7897 2023-05-20 14:25:54.492845 snapstream-0.0.5/snapstream/__main__.py
--rw-r--r--   0        0        0     9781 2023-05-20 14:25:54.492845 snapstream-0.0.5/snapstream/caching.py
--rw-r--r--   0        0        0     2562 2023-05-20 14:25:54.492845 snapstream-0.0.5/snapstream/codecs.py
--rw-r--r--   0        0        0    10542 2023-05-20 14:25:54.496845 snapstream-0.0.5/snapstream/core.py
--rw-r--r--   0        0        0     3255 2023-05-20 14:25:54.496845 snapstream-0.0.5/snapstream/utils.py
--rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-31 05:19:52.000025 snapstream-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2536 2023-05-31 05:19:52.000025 snapstream-0.0.6/README.md
+-rw-r--r--   0        0        0     2034 2023-05-31 05:20:03.196342 snapstream-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2277 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/__init__.py
+-rw-r--r--   0        0        0     7897 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/__main__.py
+-rw-r--r--   0        0        0     9781 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/caching.py
+-rw-r--r--   0        0        0     2562 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/codecs.py
+-rw-r--r--   0        0        0    10677 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/core.py
+-rw-r--r--   0        0        0     3255 2023-05-31 05:19:52.004025 snapstream-0.0.6/snapstream/utils.py
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 snapstream-0.0.6/PKG-INFO
```

### Comparing `snapstream-0.0.5/LICENSE` & `snapstream-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.5/README.md` & `snapstream-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.5/pyproject.toml` & `snapstream-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snapstream"
-version = "0.0.5"
+version = "0.0.6"
 description = "Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions."
 authors = ["Menziess <stefan_schenk@hotmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Menziess/snapstream"
 documentation = "https://snapstream.readthedocs.io"
 license = "MIT"
 keywords = ["kafka", "pubsub"]
```

### Comparing `snapstream-0.0.5/snapstream/__init__.py` & `snapstream-0.0.6/snapstream/__init__.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.5/snapstream/__main__.py` & `snapstream-0.0.6/snapstream/__main__.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.5/snapstream/caching.py` & `snapstream-0.0.6/snapstream/caching.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.5/snapstream/codecs.py` & `snapstream-0.0.6/snapstream/codecs.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.5/snapstream/core.py` & `snapstream-0.0.6/snapstream/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
     try:
         yield consume()
     finally:
         c.close()
 
 
-def _producer_handler(p, topic, dry, codec):
+def _producer_handler(p, topic, poll_timeout, codec, dry):
     def callback(err, msg):
         if err is not None:
             logger.error(f'Failed to deliver message: {err}.')
             # Raise exception by default
             raise KafkaException(err)
         else:
             logger.debug(f'Produced to topic: {msg.topic()}.')
@@ -210,29 +210,31 @@
         if codec:
             logger.debug(f'Encoding using codec: {topic}.')
             val = codec.encode(val)
         if dry:
             logger.warning(f'Skipped sending message to {topic} [dry=True].')
             return
         p.produce(topic=topic, key=key, value=val, *args, **kwargs, callback=callback)
+        p.poll(poll_timeout)
     return produce
 
 
 @contextmanager
 def get_producer(
     topic: str,
     conf: dict,
     dry=False,
     codec: Optional[ICodec] = None,
+    poll_timeout: float = 1.0,
     flush_timeout: float = -1.0,
     pusher=_producer_handler
 ) -> Iterator[Callable[[Any, Any], None]]:
     """Yield kafka produce method."""
     p = Producer(conf, logger=logger)
-    yield pusher(p, topic, dry, codec)
+    yield pusher(p, topic, poll_timeout, codec, dry)
     logger.debug(f'Flushing messages to kafka, flush_timeout={flush_timeout}.')
     p.flush(flush_timeout)
 
 
 class Topic(ITopic):
     """Act as a consumer and producer.
 
@@ -331,15 +333,16 @@
                     continue
                 yield msg
 
     def __call__(self, val, key=None, *args, **kwargs) -> None:
         """Produce to topic."""
         self._producer_ctx = (
             self._producer_ctx
-            or get_producer(self.name, self.conf, self.dry, self.codec, self.flush_timeout, self.pusher)
+            or get_producer(self.name, self.conf, self.dry, self.codec,
+                            self.poll_timeout, self.flush_timeout, self.pusher)
         )
         self.producer = (
             self.producer or
             self._producer_ctx.__enter__()
         )
         self.producer(key, val, *args, **kwargs)
```

### Comparing `snapstream-0.0.5/snapstream/utils.py` & `snapstream-0.0.6/snapstream/utils.py`

 * *Files identical despite different names*

### Comparing `snapstream-0.0.5/PKG-INFO` & `snapstream-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapstream
-Version: 0.0.5
+Version: 0.0.6
 Summary: Streamline your Kafka data processing, this tool aims to standardize streaming data from multiple Kafka clusters. With a pub-sub approach, multiple functions can easily subscribe to incoming messages, serialization can be specified per topic, and data is automatically processed by data sink functions.
 Home-page: https://github.com/Menziess/snapstream
 License: MIT
 Keywords: kafka,pubsub
 Author: Menziess
 Author-email: stefan_schenk@hotmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

