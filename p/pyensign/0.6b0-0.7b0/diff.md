# Comparing `tmp/pyensign-0.6b0.tar.gz` & `tmp/pyensign-0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyensign-0.6b0.tar", last modified: Wed Apr 26 21:53:45 2023, max compression
+gzip compressed data, was "pyensign-0.7b0.tar", last modified: Wed May 31 20:40:58 2023, max compression
```

## Comparing `pyensign-0.6b0.tar` & `pyensign-0.7b0.tar`

### file list

```diff
@@ -1,45 +1,54 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.953862 pyensign-0.6b0/
--rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-04-19 19:47:14.000000 pyensign-0.6b0/CONTRIBUTING.md
--rw-r--r--   0 patrick    (501) staff       (20)     1329 2023-03-31 21:19:30.000000 pyensign-0.6b0/DESCRIPTION.md
--rw-r--r--   0 patrick    (501) staff       (20)      180 2023-04-07 12:54:37.000000 pyensign-0.6b0/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)      394 2023-03-29 13:11:36.000000 pyensign-0.6b0/Makefile
--rw-r--r--   0 patrick    (501) staff       (20)     2577 2023-04-26 21:53:45.953994 pyensign-0.6b0/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     3307 2023-04-19 19:47:14.000000 pyensign-0.6b0/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.948073 pyensign-0.6b0/pyensign/
--rw-r--r--   0 patrick    (501) staff       (20)      507 2023-03-29 13:11:36.000000 pyensign-0.6b0/pyensign/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.950103 pyensign-0.6b0/pyensign/api/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-04-07 12:54:37.000000 pyensign-0.6b0/pyensign/api/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.951859 pyensign-0.6b0/pyensign/api/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-23 14:22:39.000000 pyensign-0.6b0/pyensign/api/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     5078 2023-03-23 16:52:53.000000 pyensign-0.6b0/pyensign/api/v1beta1/ensign_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)    17926 2023-03-23 16:52:53.000000 pyensign-0.6b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
--rw-r--r--   0 patrick    (501) staff       (20)     2718 2023-03-23 16:52:53.000000 pyensign-0.6b0/pyensign/api/v1beta1/event_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-03-23 14:22:40.000000 pyensign-0.6b0/pyensign/api/v1beta1/groups_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     4296 2023-03-23 16:52:53.000000 pyensign-0.6b0/pyensign/api/v1beta1/topic_pb2.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.952515 pyensign-0.6b0/pyensign/auth/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-04-07 12:54:37.000000 pyensign-0.6b0/pyensign/auth/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     3937 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/auth/client.py
--rw-r--r--   0 patrick    (501) staff       (20)      347 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/auth/tokens.py
--rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-03-31 14:40:41.000000 pyensign-0.6b0/pyensign/connection.py
--rw-r--r--   0 patrick    (501) staff       (20)     8844 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/ensign.py
--rw-r--r--   0 patrick    (501) staff       (20)     1917 2023-03-31 21:19:30.000000 pyensign-0.6b0/pyensign/events.py
--rw-r--r--   0 patrick    (501) staff       (20)     3602 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/exceptions.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.952729 pyensign-0.6b0/pyensign/mimetype/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-04-07 12:54:37.000000 pyensign-0.6b0/pyensign/mimetype/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.953204 pyensign-0.6b0/pyensign/mimetype/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-23 14:22:40.000000 pyensign-0.6b0/pyensign/mimetype/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-03-23 14:22:40.000000 pyensign-0.6b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.953459 pyensign-0.6b0/pyensign/utils/
--rw-r--r--   0 patrick    (501) staff       (20)      983 2023-04-26 21:48:16.000000 pyensign-0.6b0/pyensign/utils/cache.py
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-04-26 21:49:48.000000 pyensign-0.6b0/pyensign/version.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-04-26 21:53:45.949869 pyensign-0.6b0/pyensign.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)     2577 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)      871 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/not-zip-safe
--rw-r--r--   0 patrick    (501) staff       (20)       81 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        9 2023-04-26 21:53:45.000000 pyensign-0.6b0/pyensign.egg-info/top_level.txt
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-03-10 20:05:11.000000 pyensign-0.6b0/pyproject.toml
--rw-r--r--   0 patrick    (501) staff       (20)       80 2023-04-26 21:48:16.000000 pyensign-0.6b0/requirements.txt
--rw-r--r--   0 patrick    (501) staff       (20)       38 2023-04-26 21:53:45.954318 pyensign-0.6b0/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-03-31 22:42:46.000000 pyensign-0.6b0/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.854409 pyensign-0.7b0/
+-rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-05-16 21:00:20.000000 pyensign-0.7b0/CONTRIBUTING.md
+-rw-r--r--   0 patrick    (501) staff       (20)     2360 2023-05-31 19:58:09.000000 pyensign-0.7b0/DESCRIPTION.md
+-rw-r--r--   0 patrick    (501) staff       (20)      180 2023-05-16 21:00:20.000000 pyensign-0.7b0/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)      394 2023-05-16 21:00:20.000000 pyensign-0.7b0/Makefile
+-rw-r--r--   0 patrick    (501) staff       (20)     3752 2023-05-31 20:40:58.854558 pyensign-0.7b0/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     4329 2023-05-31 19:58:28.000000 pyensign-0.7b0/README.md
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.846230 pyensign-0.7b0/pyensign/
+-rw-r--r--   0 patrick    (501) staff       (20)      507 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.848027 pyensign-0.7b0/pyensign/api/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.850724 pyensign-0.7b0/pyensign/api/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7865 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19552 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
+-rw-r--r--   0 patrick    (501) staff       (20)      786 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/event.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7539 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/api/v1beta1/event_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/groups_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4416 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/topic_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.851841 pyensign-0.7b0/pyensign/auth/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3937 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/client.py
+-rw-r--r--   0 patrick    (501) staff       (20)      347 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/tokens.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11976 2023-05-31 18:56:39.000000 pyensign-0.7b0/pyensign/connection.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10517 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/ensign.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1905 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/events.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3601 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/exceptions.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852166 pyensign-0.7b0/pyensign/mimetype/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852581 pyensign-0.7b0/pyensign/mimetype/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5383 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/mimetypes.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852880 pyensign-0.7b0/pyensign/region/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.853269 pyensign-0.7b0/pyensign/region/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7945 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/v1beta1/region_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.854128 pyensign-0.7b0/pyensign/utils/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-31 18:56:39.000000 pyensign-0.7b0/pyensign/utils/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      983 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/utils/cache.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1089 2023-05-31 15:33:49.000000 pyensign-0.7b0/pyensign/utils/tasks.py
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-05-31 19:17:18.000000 pyensign-0.7b0/pyensign/version.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.847769 pyensign-0.7b0/pyensign.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)     3752 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     1076 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/not-zip-safe
+-rw-r--r--   0 patrick    (501) staff       (20)       89 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        9 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyproject.toml
+-rw-r--r--   0 patrick    (501) staff       (20)       88 2023-05-31 18:56:39.000000 pyensign-0.7b0/requirements.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       38 2023-05-31 20:40:58.854916 pyensign-0.7b0/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-05-16 21:00:20.000000 pyensign-0.7b0/setup.py
```

### Comparing `pyensign-0.6b0/CONTRIBUTING.md` & `pyensign-0.7b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyensign-0.6b0/DESCRIPTION.md` & `pyensign-0.7b0/DESCRIPTION.md`

 * *Files 26% similar despite different names*

```diff
@@ -19,22 +19,40 @@
 ```
 
 The `Event` class can be used to create events from the raw data and mimetype.
 
 ```python
 from pyensign.events import Event
 
-event = Event(b'{"temp": 72, "units": "fahrenheit"}', "APPLICATION_JSON")
+event = Event(b'{"temp": 72, "units": "fahrenheit"}', "application/json")
 ```
 
-Publish events to a topic. This function accepts anything that is iterable. Errors are concatenated into a list and returned after all the events have been published.
+Publish events to a topic. This coroutine accepts one or more events, so the following uses are all valid.
 
 ```python
-errors = await client.publish("weather", event)
+await client.publish("weather", event)
+await client.publish("weather", event1, event2)
+await client.publish("weather", [event1, event2])
 ```
 
-Subcribe to a topic or list of topics.
+Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
 
 ```python
-async for event in client.subscribe("weather"):
+topic_id = await client.topic_id("weather")
+async for event in client.subscribe(topic_id):
     print("Received event: {}".format(event))
+```
+
+## Advanced Usage
+
+The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
+
+```python
+async def handle_ack(self, ack):
+    ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
+    print(f"Event committed at {ts}")
+
+async def handle_nack(self, nack):
+    print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
+
+await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
 ```
```

### Comparing `pyensign-0.6b0/PKG-INFO` & `pyensign-0.7b0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.6b0
+Version: 0.7b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.6b0
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
@@ -30,29 +30,47 @@
         ```
         
         The `Event` class can be used to create events from the raw data and mimetype.
         
         ```python
         from pyensign.events import Event
         
-        event = Event(b'{"temp": 72, "units": "fahrenheit"}', "APPLICATION_JSON")
+        event = Event(b'{"temp": 72, "units": "fahrenheit"}', "application/json")
         ```
         
-        Publish events to a topic. This function accepts anything that is iterable. Errors are concatenated into a list and returned after all the events have been published.
+        Publish events to a topic. This coroutine accepts one or more events, so the following uses are all valid.
         
         ```python
-        errors = await client.publish("weather", event)
+        await client.publish("weather", event)
+        await client.publish("weather", event1, event2)
+        await client.publish("weather", [event1, event2])
         ```
         
-        Subcribe to a topic or list of topics.
+        Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
         
         ```python
-        async for event in client.subscribe("weather"):
+        topic_id = await client.topic_id("weather")
+        async for event in client.subscribe(topic_id):
             print("Received event: {}".format(event))
         ```
+        
+        ## Advanced Usage
+        
+        The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
+        
+        ```python
+        async def handle_ack(self, ack):
+            ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
+            print(f"Event committed at {ts}")
+        
+        async def handle_nack(self, nack):
+            print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
+        
+        await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
+        ```
 Keywords: python,setup,pypi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pyensign-0.6b0/pyensign/api/v1beta1/ensign_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/topic_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: api/v1beta1/ensign.proto
+# source: api/v1beta1/topic.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from pyensign.api.v1beta1 import event_pb2 as api_dot_v1beta1_dot_event__pb2
-from pyensign.api.v1beta1 import topic_pb2 as api_dot_v1beta1_dot_topic__pb2
-from pyensign.api.v1beta1 import groups_pb2 as api_dot_v1beta1_dot_groups__pb2
+from pyensign.region.v1beta1 import region_pb2 as region_dot_v1beta1_dot_region__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x18\x61pi/v1beta1/ensign.proto\x12\x0e\x65nsign.v1beta1\x1a\x17\x61pi/v1beta1/event.proto\x1a\x17\x61pi/v1beta1/topic.proto\x1a\x18\x61pi/v1beta1/groups.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto"\x95\x01\n\x0bPublication\x12"\n\x03\x61\x63k\x18\x01 \x01(\x0b\x32\x13.ensign.v1beta1.AckH\x00\x12$\n\x04nack\x18\x02 \x01(\x0b\x32\x14.ensign.v1beta1.NackH\x00\x12\x33\n\x0c\x63lose_stream\x18\x03 \x01(\x0b\x32\x1b.ensign.v1beta1.CloseStreamH\x00\x42\x07\n\x05\x65mbed"\x94\x01\n\x0cSubscription\x12"\n\x03\x61\x63k\x18\x01 \x01(\x0b\x32\x13.ensign.v1beta1.AckH\x00\x12$\n\x04nack\x18\x02 \x01(\x0b\x32\x14.ensign.v1beta1.NackH\x00\x12\x31\n\x0bopen_stream\x18\x03 \x01(\x0b\x32\x1a.ensign.v1beta1.OpenStreamH\x00\x42\x07\n\x05\x65mbed"@\n\x03\x41\x63k\x12\n\n\x02id\x18\x01 \x01(\t\x12-\n\tcommitted\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"/\n\x04Nack\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\r\x12\r\n\x05\x65rror\x18\x03 \x01(\t"_\n\nOpenStream\x12\x13\n\x0b\x63onsumer_id\x18\x01 \x01(\t\x12\x0e\n\x06topics\x18\x02 \x03(\t\x12,\n\x05group\x18\x03 \x01(\x0b\x32\x1d.ensign.v1beta1.ConsumerGroup"F\n\x0b\x43loseStream\x12\x0e\n\x06\x65vents\x18\x01 \x01(\x04\x12\x14\n\x0ctopic_offset\x18\x02 \x01(\x04\x12\x11\n\tconsumers\x18\x03 \x01(\x04"T\n\x0bHealthCheck\x12\x10\n\x08\x61ttempts\x18\x01 \x01(\r\x12\x33\n\x0flast_checked_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"\xbb\x02\n\x0cServiceState\x12\x33\n\x06status\x18\x01 \x01(\x0e\x32#.ensign.v1beta1.ServiceState.Status\x12\x0f\n\x07version\x18\x02 \x01(\t\x12)\n\x06uptime\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\nnot_before\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tnot_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"[\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07HEALTHY\x10\x01\x12\r\n\tUNHEALTHY\x10\x02\x12\n\n\x06\x44\x41NGER\x10\x03\x12\x0b\n\x07OFFLINE\x10\x04\x12\x0f\n\x0bMAINTENANCE\x10\x05"6\n\x08PageInfo\x12\x11\n\tpage_size\x18\x01 \x01(\r\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t2\x84\x05\n\x06\x45nsign\x12\x43\n\x07Publish\x12\x15.ensign.v1beta1.Event\x1a\x1b.ensign.v1beta1.Publication"\x00(\x01\x30\x01\x12\x46\n\tSubscribe\x12\x1c.ensign.v1beta1.Subscription\x1a\x15.ensign.v1beta1.Event"\x00(\x01\x30\x01\x12\x44\n\nListTopics\x12\x18.ensign.v1beta1.PageInfo\x1a\x1a.ensign.v1beta1.TopicsPage"\x00\x12=\n\x0b\x43reateTopic\x12\x15.ensign.v1beta1.Topic\x1a\x15.ensign.v1beta1.Topic"\x00\x12?\n\rRetrieveTopic\x12\x15.ensign.v1beta1.Topic\x1a\x15.ensign.v1beta1.Topic"\x00\x12I\n\x0b\x44\x65leteTopic\x12\x18.ensign.v1beta1.TopicMod\x1a\x1e.ensign.v1beta1.TopicTombstone"\x00\x12H\n\nTopicNames\x12\x18.ensign.v1beta1.PageInfo\x1a\x1e.ensign.v1beta1.TopicNamesPage"\x00\x12K\n\x0bTopicExists\x12\x19.ensign.v1beta1.TopicName\x1a\x1f.ensign.v1beta1.TopicExistsInfo"\x00\x12\x45\n\x06Status\x12\x1b.ensign.v1beta1.HealthCheck\x1a\x1c.ensign.v1beta1.ServiceState"\x00\x62\x06proto3'
+    b'\n\x17\x61pi/v1beta1/topic.proto\x12\x0e\x65nsign.v1beta1\x1a\x17\x61pi/v1beta1/event.proto\x1a\x1bregion/v1beta1/region.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\x96\x02\n\x05Topic\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x12\n\nproject_id\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08readonly\x18\x04 \x01(\x08\x12\x0e\n\x06offset\x18\x05 \x01(\x04\x12\x0e\n\x06shards\x18\x06 \x01(\r\x12-\n\nplacements\x18\x0c \x03(\x0b\x32\x19.ensign.v1beta1.Placement\x12#\n\x05types\x18\r \x03(\x0b\x32\x14.ensign.v1beta1.Type\x12+\n\x07\x63reated\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08modified\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp"?\n\tTopicName\x12\x10\n\x08topic_id\x18\x01 \x01(\t\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t"L\n\nTopicsPage\x12%\n\x06topics\x18\x01 \x03(\x0b\x32\x15.ensign.v1beta1.Topic\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t"Y\n\x0eTopicNamesPage\x12.\n\x0btopic_names\x18\x01 \x03(\x0b\x32\x19.ensign.v1beta1.TopicName\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t"~\n\x08TopicMod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x35\n\toperation\x18\x02 \x01(\x0e\x32".ensign.v1beta1.TopicMod.Operation"/\n\tOperation\x12\x08\n\x04NOOP\x10\x00\x12\x0b\n\x07\x41RCHIVE\x10\x01\x12\x0b\n\x07\x44\x45STROY\x10\x02"\x85\x01\n\x0eTopicTombstone\x12\n\n\x02id\x18\x01 \x01(\t\x12\x34\n\x05state\x18\x02 \x01(\x0e\x32%.ensign.v1beta1.TopicTombstone.Status"1\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08READONLY\x10\x01\x12\x0c\n\x08\x44\x45LETING\x10\x02"0\n\x0fTopicExistsInfo\x12\r\n\x05query\x18\x01 \x01(\t\x12\x0e\n\x06\x65xists\x18\x02 \x01(\x08"\x9c\x01\n\tPlacement\x12\r\n\x05\x65poch\x18\x01 \x01(\x04\x12\x32\n\x08sharding\x18\x02 \x01(\x0e\x32 .ensign.v1beta1.ShardingStrategy\x12\'\n\x07regions\x18\x03 \x03(\x0e\x32\x16.region.v1beta1.Region\x12#\n\x05nodes\x18\x04 \x03(\x0b\x32\x14.ensign.v1beta1.Node"x\n\x04Node\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08hostname\x18\x02 \x01(\t\x12\x0e\n\x06quorum\x18\x03 \x01(\x04\x12\r\n\x05shard\x18\x04 \x01(\x04\x12&\n\x06region\x18\x05 \x01(\x0e\x32\x16.region.v1beta1.Region\x12\x0b\n\x03url\x18\x06 \x01(\t*m\n\x10ShardingStrategy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bNO_SHARDING\x10\x01\x12\x17\n\x13\x43ONSISTENT_KEY_HASH\x10\x02\x12\n\n\x06RANDOM\x10\x03\x12\x16\n\x12PUBLISHER_ORDERING\x10\x04\x62\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "api.v1beta1.ensign_pb2", globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "api.v1beta1.topic_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _PUBLICATION._serialized_start = 186
-    _PUBLICATION._serialized_end = 335
-    _SUBSCRIPTION._serialized_start = 338
-    _SUBSCRIPTION._serialized_end = 486
-    _ACK._serialized_start = 488
-    _ACK._serialized_end = 552
-    _NACK._serialized_start = 554
-    _NACK._serialized_end = 601
-    _OPENSTREAM._serialized_start = 603
-    _OPENSTREAM._serialized_end = 698
-    _CLOSESTREAM._serialized_start = 700
-    _CLOSESTREAM._serialized_end = 770
-    _HEALTHCHECK._serialized_start = 772
-    _HEALTHCHECK._serialized_end = 856
-    _SERVICESTATE._serialized_start = 859
-    _SERVICESTATE._serialized_end = 1174
-    _SERVICESTATE_STATUS._serialized_start = 1083
-    _SERVICESTATE_STATUS._serialized_end = 1174
-    _PAGEINFO._serialized_start = 1176
-    _PAGEINFO._serialized_end = 1230
-    _ENSIGN._serialized_start = 1233
-    _ENSIGN._serialized_end = 1877
+    _SHARDINGSTRATEGY._serialized_start = 1240
+    _SHARDINGSTRATEGY._serialized_end = 1349
+    _TOPIC._serialized_start = 131
+    _TOPIC._serialized_end = 409
+    _TOPICNAME._serialized_start = 411
+    _TOPICNAME._serialized_end = 474
+    _TOPICSPAGE._serialized_start = 476
+    _TOPICSPAGE._serialized_end = 552
+    _TOPICNAMESPAGE._serialized_start = 554
+    _TOPICNAMESPAGE._serialized_end = 643
+    _TOPICMOD._serialized_start = 645
+    _TOPICMOD._serialized_end = 771
+    _TOPICMOD_OPERATION._serialized_start = 724
+    _TOPICMOD_OPERATION._serialized_end = 771
+    _TOPICTOMBSTONE._serialized_start = 774
+    _TOPICTOMBSTONE._serialized_end = 907
+    _TOPICTOMBSTONE_STATUS._serialized_start = 858
+    _TOPICTOMBSTONE_STATUS._serialized_end = 907
+    _TOPICEXISTSINFO._serialized_start = 909
+    _TOPICEXISTSINFO._serialized_end = 957
+    _PLACEMENT._serialized_start = 960
+    _PLACEMENT._serialized_end = 1116
+    _NODE._serialized_start = 1118
+    _NODE._serialized_end = 1238
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyensign-0.6b0/pyensign/api/v1beta1/ensign_pb2_grpc.py` & `pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from pyensign.api.v1beta1 import ensign_pb2 as api_dot_v1beta1_dot_ensign__pb2
-from pyensign.api.v1beta1 import event_pb2 as api_dot_v1beta1_dot_event__pb2
 from pyensign.api.v1beta1 import topic_pb2 as api_dot_v1beta1_dot_topic__pb2
 
 
 class EnsignStub(object):
     """The Ensign service is meant to allow publishers (producers) and subscribers
     (consumers) of events to interact with the Ensign eventing system; e.g. this is a
     user-oriented API that is the basis of the user SDKs that we will build. There are
@@ -19,21 +18,21 @@
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Publish = channel.stream_stream(
             "/ensign.v1beta1.Ensign/Publish",
-            request_serializer=api_dot_v1beta1_dot_event__pb2.Event.SerializeToString,
-            response_deserializer=api_dot_v1beta1_dot_ensign__pb2.Publication.FromString,
+            request_serializer=api_dot_v1beta1_dot_ensign__pb2.PublisherRequest.SerializeToString,
+            response_deserializer=api_dot_v1beta1_dot_ensign__pb2.PublisherReply.FromString,
         )
         self.Subscribe = channel.stream_stream(
             "/ensign.v1beta1.Ensign/Subscribe",
-            request_serializer=api_dot_v1beta1_dot_ensign__pb2.Subscription.SerializeToString,
-            response_deserializer=api_dot_v1beta1_dot_event__pb2.Event.FromString,
+            request_serializer=api_dot_v1beta1_dot_ensign__pb2.SubscribeRequest.SerializeToString,
+            response_deserializer=api_dot_v1beta1_dot_ensign__pb2.SubscribeReply.FromString,
         )
         self.ListTopics = channel.unary_unary(
             "/ensign.v1beta1.Ensign/ListTopics",
             request_serializer=api_dot_v1beta1_dot_ensign__pb2.PageInfo.SerializeToString,
             response_deserializer=api_dot_v1beta1_dot_topic__pb2.TopicsPage.FromString,
         )
         self.CreateTopic = channel.unary_unary(
@@ -57,14 +56,19 @@
             response_deserializer=api_dot_v1beta1_dot_topic__pb2.TopicNamesPage.FromString,
         )
         self.TopicExists = channel.unary_unary(
             "/ensign.v1beta1.Ensign/TopicExists",
             request_serializer=api_dot_v1beta1_dot_topic__pb2.TopicName.SerializeToString,
             response_deserializer=api_dot_v1beta1_dot_topic__pb2.TopicExistsInfo.FromString,
         )
+        self.Info = channel.unary_unary(
+            "/ensign.v1beta1.Ensign/Info",
+            request_serializer=api_dot_v1beta1_dot_ensign__pb2.InfoRequest.SerializeToString,
+            response_deserializer=api_dot_v1beta1_dot_ensign__pb2.ProjectInfo.FromString,
+        )
         self.Status = channel.unary_unary(
             "/ensign.v1beta1.Ensign/Status",
             request_serializer=api_dot_v1beta1_dot_ensign__pb2.HealthCheck.SerializeToString,
             response_deserializer=api_dot_v1beta1_dot_ensign__pb2.ServiceState.FromString,
         )
 
 
@@ -133,32 +137,38 @@
 
     def TopicExists(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def Info(self, request, context):
+        """Info provides statistics and metrics describing the state of a project"""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
     def Status(self, request, context):
         """Implements a client-side heartbeat that can also be used by monitoring tools."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
 def add_EnsignServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "Publish": grpc.stream_stream_rpc_method_handler(
             servicer.Publish,
-            request_deserializer=api_dot_v1beta1_dot_event__pb2.Event.FromString,
-            response_serializer=api_dot_v1beta1_dot_ensign__pb2.Publication.SerializeToString,
+            request_deserializer=api_dot_v1beta1_dot_ensign__pb2.PublisherRequest.FromString,
+            response_serializer=api_dot_v1beta1_dot_ensign__pb2.PublisherReply.SerializeToString,
         ),
         "Subscribe": grpc.stream_stream_rpc_method_handler(
             servicer.Subscribe,
-            request_deserializer=api_dot_v1beta1_dot_ensign__pb2.Subscription.FromString,
-            response_serializer=api_dot_v1beta1_dot_event__pb2.Event.SerializeToString,
+            request_deserializer=api_dot_v1beta1_dot_ensign__pb2.SubscribeRequest.FromString,
+            response_serializer=api_dot_v1beta1_dot_ensign__pb2.SubscribeReply.SerializeToString,
         ),
         "ListTopics": grpc.unary_unary_rpc_method_handler(
             servicer.ListTopics,
             request_deserializer=api_dot_v1beta1_dot_ensign__pb2.PageInfo.FromString,
             response_serializer=api_dot_v1beta1_dot_topic__pb2.TopicsPage.SerializeToString,
         ),
         "CreateTopic": grpc.unary_unary_rpc_method_handler(
@@ -182,14 +192,19 @@
             response_serializer=api_dot_v1beta1_dot_topic__pb2.TopicNamesPage.SerializeToString,
         ),
         "TopicExists": grpc.unary_unary_rpc_method_handler(
             servicer.TopicExists,
             request_deserializer=api_dot_v1beta1_dot_topic__pb2.TopicName.FromString,
             response_serializer=api_dot_v1beta1_dot_topic__pb2.TopicExistsInfo.SerializeToString,
         ),
+        "Info": grpc.unary_unary_rpc_method_handler(
+            servicer.Info,
+            request_deserializer=api_dot_v1beta1_dot_ensign__pb2.InfoRequest.FromString,
+            response_serializer=api_dot_v1beta1_dot_ensign__pb2.ProjectInfo.SerializeToString,
+        ),
         "Status": grpc.unary_unary_rpc_method_handler(
             servicer.Status,
             request_deserializer=api_dot_v1beta1_dot_ensign__pb2.HealthCheck.FromString,
             response_serializer=api_dot_v1beta1_dot_ensign__pb2.ServiceState.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -220,16 +235,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.stream_stream(
             request_iterator,
             target,
             "/ensign.v1beta1.Ensign/Publish",
-            api_dot_v1beta1_dot_event__pb2.Event.SerializeToString,
-            api_dot_v1beta1_dot_ensign__pb2.Publication.FromString,
+            api_dot_v1beta1_dot_ensign__pb2.PublisherRequest.SerializeToString,
+            api_dot_v1beta1_dot_ensign__pb2.PublisherReply.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -249,16 +264,16 @@
         timeout=None,
         metadata=None,
     ):
         return grpc.experimental.stream_stream(
             request_iterator,
             target,
             "/ensign.v1beta1.Ensign/Subscribe",
-            api_dot_v1beta1_dot_ensign__pb2.Subscription.SerializeToString,
-            api_dot_v1beta1_dot_event__pb2.Event.FromString,
+            api_dot_v1beta1_dot_ensign__pb2.SubscribeRequest.SerializeToString,
+            api_dot_v1beta1_dot_ensign__pb2.SubscribeReply.FromString,
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
@@ -432,14 +447,43 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def Info(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/ensign.v1beta1.Ensign/Info",
+            api_dot_v1beta1_dot_ensign__pb2.InfoRequest.SerializeToString,
+            api_dot_v1beta1_dot_ensign__pb2.ProjectInfo.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
 
     @staticmethod
     def Status(
         request,
         target,
```

### Comparing `pyensign-0.6b0/pyensign/api/v1beta1/event_pb2.py` & `pyensign-0.7b0/pyensign/api/v1beta1/groups_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: api/v1beta1/event.proto
+# source: api/v1beta1/groups.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from pyensign.mimetype.v1beta1 import (
-    mimetype_pb2 as mimetype_dot_v1beta1_dot_mimetype__pb2,
-)
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17\x61pi/v1beta1/event.proto\x12\x0e\x65nsign.v1beta1\x1a\x1fmimetype/v1beta1/mimetype.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xbe\x03\n\x05\x45vent\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08topic_id\x18\x02 \x01(\t\x12(\n\x08mimetype\x18\x03 \x01(\x0e\x32\x16.mimetype.v1beta1.MIME\x12"\n\x04type\x18\x04 \x01(\x0b\x32\x14.ensign.v1beta1.Type\x12\x0b\n\x03key\x18\x05 \x01(\x0c\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12.\n\nencryption\x18\x07 \x01(\x0b\x32\x1a.ensign.v1beta1.Encryption\x12\x30\n\x0b\x63ompression\x18\x08 \x01(\x0b\x32\x1b.ensign.v1beta1.Compression\x12)\n\tgeography\x18\t \x01(\x0b\x32\x16.ensign.v1beta1.Region\x12,\n\tpublisher\x18\n \x01(\x0b\x32\x19.ensign.v1beta1.Publisher\x12\x17\n\x0fuser_defined_id\x18\x0b \x01(\t\x12+\n\x07\x63reated\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tcommitted\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp"%\n\x04Type\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\r"/\n\nEncryption\x12\x11\n\talgorithm\x18\x01 \x01(\t\x12\x0e\n\x06key_id\x18\x02 \x01(\t" \n\x0b\x43ompression\x12\x11\n\talgorithm\x18\x02 \x01(\t"\x16\n\x06Region\x12\x0c\n\x04name\x18\x01 \x01(\t".\n\tPublisher\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x0e\n\x06ipaddr\x18\x02 \x01(\tb\x06proto3'
-)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61pi/v1beta1/groups.proto\x12\x0e\x65nsign.v1beta1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\"\x91\x03\n\rConsumerGroup\x12\n\n\x02id\x18\x01 \x01(\x0c\x12\x12\n\nproject_id\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x32\n\x08\x64\x65livery\x18\x04 \x01(\x0e\x32 .ensign.v1beta1.DeliverySemantic\x12\x33\n\x10\x64\x65livery_timeout\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x46\n\rtopic_offsets\x18\x0c \x03(\x0b\x32/.ensign.v1beta1.ConsumerGroup.TopicOffsetsEntry\x12\x11\n\tconsumers\x18\r \x03(\x0c\x12+\n\x07\x63reated\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08modified\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x33\n\x11TopicOffsetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01*Z\n\x10\x44\x65liverySemantic\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x10\n\x0c\x41T_MOST_ONCE\x10\x01\x12\x11\n\rAT_LEAST_ONCE\x10\x02\x12\x10\n\x0c\x45XACTLY_ONCE\x10\x03\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "api.v1beta1.event_pb2", globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1beta1.groups_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    _EVENT._serialized_start = 110
-    _EVENT._serialized_end = 556
-    _TYPE._serialized_start = 558
-    _TYPE._serialized_end = 595
-    _ENCRYPTION._serialized_start = 597
-    _ENCRYPTION._serialized_end = 644
-    _COMPRESSION._serialized_start = 646
-    _COMPRESSION._serialized_end = 678
-    _REGION._serialized_start = 680
-    _REGION._serialized_end = 702
-    _PUBLISHER._serialized_start = 704
-    _PUBLISHER._serialized_end = 750
+  DESCRIPTOR._options = None
+  _CONSUMERGROUP_TOPICOFFSETSENTRY._options = None
+  _CONSUMERGROUP_TOPICOFFSETSENTRY._serialized_options = b'8\001'
+  _DELIVERYSEMANTIC._serialized_start=513
+  _DELIVERYSEMANTIC._serialized_end=603
+  _CONSUMERGROUP._serialized_start=110
+  _CONSUMERGROUP._serialized_end=511
+  _CONSUMERGROUP_TOPICOFFSETSENTRY._serialized_start=460
+  _CONSUMERGROUP_TOPICOFFSETSENTRY._serialized_end=511
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyensign-0.6b0/pyensign/auth/client.py` & `pyensign-0.7b0/pyensign/auth/client.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.6b0/pyensign/ensign.py` & `pyensign-0.7b0/pyensign/ensign.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 from ulid import ULID
 
 from pyensign.connection import Client
 from pyensign.utils.cache import Cache
 from pyensign.connection import Connection
 from pyensign.api.v1beta1 import topic_pb2
+from pyensign.api.v1beta1 import ensign_pb2
 from pyensign.auth.client import AuthClient
 from pyensign.exceptions import (
     CacheMissError,
-    EnsignResponseType,
+    EnsignTypeError,
     EnsignTopicCreateError,
     EnsignTopicNotFoundError,
 )
 
 
 class Ensign:
     """
@@ -72,85 +73,108 @@
         self.client = Client(connection)
 
         if disable_topic_cache:
             self.topics = None
         else:
             self.topics = Cache()
 
-    async def publish(self, topic_name, *events):
+    async def publish(
+        self, topic_name, *events, ack_callback=None, nack_callback=None, client_id=""
+    ):
         """
         Publish events to an Ensign topic.
 
         Parameters
         ----------
         topic_name : str
             The name of the topic to publish events to.
 
         events : iterable of events
             The events to publish.
+
+        ack_callback: callable (optional)
+            A callback to be invoked when an ACK message is received from Ensign,
+            indicating that an event was successfully published.
+
+        nack_callback: callable (optional)
+            A callback to be invoked when a NACK message is received from Ensign,
+            indicating that the event could not be published.
+
+        client_id : str (optional)
+            The client ID to use for the publisher. If not provided, a new client ID is
+            generated.
         """
 
         if topic_name == "":
             raise ValueError("topic_name is required")
 
         if len(events) == 0:
             raise ValueError("no events provided")
 
+        if client_id == "":
+            client_id = str(ULID())
+
         # Ensure the topic ID exists by getting or creating it
-        topic_id = ""
+        topic_id = None
         try:
-            topic_id = await self.topic_id(topic_name)
+            id_str = await self.topic_id(topic_name)
+            topic_id = ULID.from_str(id_str)
         except EnsignTopicNotFoundError:
             topic = await self.create_topic(topic_name)
-            topic_id = str(ULID.from_bytes(topic.id))
+            topic_id = ULID.from_bytes(topic.id)
 
         # TODO: Support user-defined generators
         def next():
             for event in events:
-                yield event.proto(topic_id)
+                yield event.proto()
 
-        errors = []
-        async for publication in self.client.publish(next()):
-            rep_type = publication.WhichOneof("embed")
-            if rep_type == "ack":
-                continue
-            elif rep_type == "nack":
-                errors.append(publication.nack)
-            elif rep_type == "close_stream":
-                break
-            else:
-                raise EnsignResponseType(f"unexpected response type: {rep_type}")
-        return errors
+        await self.client.publish(
+            topic_id,
+            next(),
+            ack_callback=ack_callback,
+            nack_callback=nack_callback,
+            client_id=client_id,
+        )
 
-    async def subscribe(self, *topic_ids, consumer_id="", consumer_group=None):
+    async def subscribe(self, *topic_ids, client_id="", query="", consumer_group=None):
         """
         Subscribe to events from the Ensign server.
 
         Parameters
         ----------
         topic_ids : iterable of str
             The topic IDs to subscribe to.
 
-        consumer_id : str (optional)
-            The consumer ID to use for the subscriber.
+        client_id : str (optional)
+            The client ID to use for the subscriber. If not provided, a new client ID
+            is generated.
+
+        query : str (optional)
+            EnSQL query to filter events.
 
         consumer_group : api.v1beta1.groups.ConsumerGroup (optional)
             The consumer group to use for the subscriber.
 
         Yields
         ------
         api.v1beta1.event_pb2.Event
             The events received from the Ensign server.
         """
 
         if len(topic_ids) == 0:
             raise ValueError("no topic IDs provided")
 
+        if client_id == "":
+            client_id = str(ULID())
+
         async for event in self.client.subscribe(
-            topic_ids, consumer_id, consumer_group
+            topic_ids,
+            client_id=client_id,
+            query=query,
+            consumer_group=consumer_group,
         ):
             yield event
 
     async def get_topics(self):
         """
         Get all topics.
 
@@ -278,14 +302,43 @@
         if self.topics is not None and self.topics.exists(name):
             return True
 
         # Check existence using Ensign
         _, exists = await self.client.topic_exists(topic_name=name)
         return exists
 
+    async def info(self, topic_ids=[]):
+        """
+        Get aggregated statistics for topics in the project.
+
+        Parameters
+        ----------
+        topic_ids: list of str (optional)
+            If provided, only aggregate info for the specified topic IDs. Otherwise,
+            the info includes all of the topics in the project.
+
+        Returns
+        -------
+        api.v1beta1.ProjectInfo
+            The aggregated statistics for the topics in the project.
+        """
+
+        if not isinstance(topic_ids, list):
+            raise TypeError(f"expected list of topic IDs, got {type(topic_ids)}")
+
+        # Ensure that only topic IDs are provided
+        topics = []
+        for id in topic_ids:
+            try:
+                topics.append(ULID.from_str(id).bytes)
+            except ValueError:
+                raise ValueError(f"not parseable as a topic ID: {id}")
+
+        return await self.client.info(topics)
+
     async def status(self):
         """
         Check the status of the Ensign server.
 
         Returns
         -------
         str
```

### Comparing `pyensign-0.6b0/pyensign/events.py` & `pyensign-0.7b0/pyensign/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from pyensign.api.v1beta1 import event_pb2
-from pyensign.mimetype.v1beta1 import mimetype_pb2
+import time
+from google.protobuf.timestamp_pb2 import Timestamp
 
-mimetypes = mimetype_pb2.DESCRIPTOR.enum_types_by_name["MIME"].values_by_name
-mimetype_names = mimetypes.keys()
+from pyensign import mimetypes as mtype
+from pyensign.api.v1beta1 import event_pb2
 
 
 class Event:
     """
     Event is an abstraction of an Ensign protocol buffer Event to make it easier to
     create and parse events.
     """
 
-    def __init__(self, data=None, mimetype=None):
+    def __init__(self, data=None, mimetype=mtype.ApplicationJSON, meta={}):
         """
         Create a new Event from a mimetype and data.
 
         Parameters
         ----------
         data : bytes
             The data to use for the event.
         mimetype: str or int
-            The mimetype of the data (e.g. "APPLICATION_JSON").
+            The mimetype of the data (e.g. "application/json").
+        meta: dict (optional)
+            A set of key-value pairs to associate with the event.
         """
 
         if not data:
             raise ValueError("no data provided")
 
-        if not mimetype:
+        if mimetype is None:
             raise ValueError("no mimetype provided")
 
-        # TODO: Support traditionally formatted mimetypes (e.g. application/json)
-        if isinstance(mimetype, str):
-            if mimetype not in mimetypes:
-                raise ValueError(
-                    "invalid mimetype, specify one of: {}".format(mimetype_names)
-                )
-            self.mimetype = mimetypes[mimetype].number
-        else:
-            self.mimetype = mimetype
+        self.mimetype = mtype.parse(mimetype)
 
+        # Fields that the user may want to modify after creation.
         self.data = data
-        self.type = event_pb2.Type(name="Generic", version=1)
+        self.meta = meta
+        self.type = event_pb2.Type(
+            name="Generic", major_version=1, minor_version=0, patch_version=0
+        )
+        self.created = Timestamp(seconds=int(time.time()))
+
+        # Ensure that the protocol buffer representation is valid at the point of
+        # creation.
+        self._proto = self.proto()
 
-    def proto(self, topic_id):
+    def proto(self):
         """
         Return the protocol buffer representation of the event.
 
-        Parameters
-        ----------
-        topic_id : str
-            The topic ID to use when publishing the event.
-
         Returns
         -------
         api.v1beta1.event_pb2.Event
-            The protocol buffer representation of the event with the topic ID set.
+            The protocol buffer representation of the event.
         """
 
-        if not topic_id:
-            raise ValueError("no topic_id provided")
-
+        # TODO: Should we raise type errors and missing field errors to help the user?
         return event_pb2.Event(
-            topic_id=topic_id, data=self.data, mimetype=self.mimetype, type=self.type
+            data=self.data,
+            metadata=self.meta,
+            mimetype=self.mimetype,
+            type=self.type,
+            created=self.created,
         )
```

### Comparing `pyensign-0.6b0/pyensign/exceptions.py` & `pyensign-0.7b0/pyensign/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,17 @@
     """
     Raised when PyEnsign receives a gRPC error from the Ensign server
     """
 
     pass
 
 
-class EnsignResponseType(EnsignError):
+class EnsignTypeError(EnsignError, TypeError):
     """
-    Raised when PyEnsign receives an unexpected message type from the Ensign server
+    Raised when PyEnsign receives an unexpected type in a response message
     """
 
     pass
 
 
 class EnsignAttributeError(EnsignError, AttributeError):
     """
```

### Comparing `pyensign-0.6b0/pyensign/mimetype/v1beta1/mimetype_pb2.py` & `pyensign-0.7b0/pyensign/mimetype/v1beta1/mimetype_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.6b0/pyensign/utils/cache.py` & `pyensign-0.7b0/pyensign/utils/cache.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.6b0/pyensign/version.py` & `pyensign-0.7b0/pyensign/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
-    "minor": 6,
+    "minor": 7,
     "micro": 0,
     "releaselevel": "beta",
     "serial": 0,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `pyensign-0.6b0/pyensign.egg-info/PKG-INFO` & `pyensign-0.7b0/pyensign.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.6b0
+Version: 0.7b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.6b0
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
@@ -30,29 +30,47 @@
         ```
         
         The `Event` class can be used to create events from the raw data and mimetype.
         
         ```python
         from pyensign.events import Event
         
-        event = Event(b'{"temp": 72, "units": "fahrenheit"}', "APPLICATION_JSON")
+        event = Event(b'{"temp": 72, "units": "fahrenheit"}', "application/json")
         ```
         
-        Publish events to a topic. This function accepts anything that is iterable. Errors are concatenated into a list and returned after all the events have been published.
+        Publish events to a topic. This coroutine accepts one or more events, so the following uses are all valid.
         
         ```python
-        errors = await client.publish("weather", event)
+        await client.publish("weather", event)
+        await client.publish("weather", event1, event2)
+        await client.publish("weather", [event1, event2])
         ```
         
-        Subcribe to a topic or list of topics.
+        Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
         
         ```python
-        async for event in client.subscribe("weather"):
+        topic_id = await client.topic_id("weather")
+        async for event in client.subscribe(topic_id):
             print("Received event: {}".format(event))
         ```
+        
+        ## Advanced Usage
+        
+        The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
+        
+        ```python
+        async def handle_ack(self, ack):
+            ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
+            print(f"Event committed at {ts}")
+        
+        async def handle_nack(self, nack):
+            print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
+        
+        await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
+        ```
 Keywords: python,setup,pypi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `pyensign-0.6b0/pyensign.egg-info/SOURCES.txt` & `pyensign-0.7b0/pyensign.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,28 +8,35 @@
 setup.cfg
 setup.py
 pyensign/__init__.py
 pyensign/connection.py
 pyensign/ensign.py
 pyensign/events.py
 pyensign/exceptions.py
+pyensign/mimetypes.py
 pyensign/version.py
 pyensign.egg-info/PKG-INFO
 pyensign.egg-info/SOURCES.txt
 pyensign.egg-info/dependency_links.txt
 pyensign.egg-info/not-zip-safe
 pyensign.egg-info/requires.txt
 pyensign.egg-info/top_level.txt
 pyensign/api/__init__.py
 pyensign/api/v1beta1/__init__.py
 pyensign/api/v1beta1/ensign_pb2.py
 pyensign/api/v1beta1/ensign_pb2_grpc.py
+pyensign/api/v1beta1/event.py
 pyensign/api/v1beta1/event_pb2.py
 pyensign/api/v1beta1/groups_pb2.py
 pyensign/api/v1beta1/topic_pb2.py
 pyensign/auth/__init__.py
 pyensign/auth/client.py
 pyensign/auth/tokens.py
 pyensign/mimetype/__init__.py
 pyensign/mimetype/v1beta1/__init__.py
 pyensign/mimetype/v1beta1/mimetype_pb2.py
-pyensign/utils/cache.py
+pyensign/region/__init__.py
+pyensign/region/v1beta1/__init__.py
+pyensign/region/v1beta1/region_pb2.py
+pyensign/utils/__init__.py
+pyensign/utils/cache.py
+pyensign/utils/tasks.py
```

### Comparing `pyensign-0.6b0/setup.py` & `pyensign-0.7b0/setup.py`

 * *Files identical despite different names*

