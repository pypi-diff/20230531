# Comparing `tmp/memphis-py-beta-1.0.2.tar.gz` & `tmp/memphis-py-beta-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memphis-py-beta-1.0.2.tar", last modified: Sun Apr 16 13:50:15 2023, max compression
+gzip compressed data, was "dist/memphis-py-beta-1.0.3.tar", last modified: Tue May 30 10:58:37 2023, max compression
```

## Comparing `memphis-py-beta-1.0.2.tar` & `memphis-py-beta-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16297 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12392 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8050 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/consumer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/exceptions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/headers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    30732 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/memphis.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2176 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/message.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13161 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/producer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2190 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/station.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/types.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16297 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16488 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12575 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8079 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/consumer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/exceptions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/headers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    31966 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/memphis.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2174 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/message.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    14111 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/producer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2192 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/station.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/types.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis_py_beta.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16488 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis_py_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis_py_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis_py_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis_py_beta.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/memphis_py_beta.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-05-30 10:58:37.000000 memphis-py-beta-1.0.3/setup.py
```

### Comparing `memphis-py-beta-1.0.2/PKG-INFO` & `memphis-py-beta-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.2
+Version: 1.0.3
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.3.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
@@ -70,14 +70,15 @@
         ```python
         async def main():
           try:
             memphis = Memphis()
             await memphis.connect(
               host="<memphis-host>",
               username="<application-type username>",
+              account_id="<account_id>", # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
               connection_token="<broker-token>", # you will get it on application type user creation
               password="<string>", # depends on how Memphis deployed - default is connection token-based authentication
               port="<port>", # defaults to 6666
               reconnect=True, # defaults to True
               max_reconnect=3, # defaults to 3
               reconnect_interval_ms=1500, # defaults to 1500
               timeout_ms=1500, # defaults to 1500
```

### Comparing `memphis-py-beta-1.0.2/README.md` & `memphis-py-beta-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 ```python
 async def main():
   try:
     memphis = Memphis()
     await memphis.connect(
       host="<memphis-host>",
       username="<application-type username>",
+      account_id="<account_id>", # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
       connection_token="<broker-token>", # you will get it on application type user creation
       password="<string>", # depends on how Memphis deployed - default is connection token-based authentication
       port="<port>", # defaults to 6666
       reconnect=True, # defaults to True
       max_reconnect=3, # defaults to 3
       reconnect_interval_ms=1500, # defaults to 1500
       timeout_ms=1500, # defaults to 1500
```

### Comparing `memphis-py-beta-1.0.2/memphis/__init__.py` & `memphis-py-beta-1.0.3/memphis/__init__.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.2/memphis/consumer.py` & `memphis-py-beta-1.0.3/memphis/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from memphis.exceptions import MemphisError
 from memphis.utils import default_error_handler, get_internal_name
 from memphis.message import Message
 
 
 class Consumer:
     MAX_BATCH_SIZE = 5000
+
     def __init__(
         self,
         connection,
         station_name: str,
         consumer_name,
         consumer_group,
         pull_interval_ms: int,
@@ -41,14 +42,15 @@
         self.start_consume_from_sequence = start_consume_from_sequence
         self.last_messages = last_messages
         self.context = {}
         self.dls_messages = []
         self.dls_current_index = 0
         self.dls_callback_func = None
         self.t_dls = asyncio.create_task(self.__consume_dls())
+        self.t_consume = None
 
     def set_context(self, context):
         """Set a context (dict) that will be passed to each message handler call."""
         self.context = context
 
     def consume(self, callback):
         """Consume events."""
@@ -77,16 +79,15 @@
                     await callback(
                         [], MemphisError("Memphis: TimeoutError"), self.context
                     )
                     continue
                 except Exception as e:
                     if self.connection.is_connection_active:
                         raise MemphisError(str(e)) from e
-                    else:
-                        return
+                    return
             else:
                 break
 
     async def __consume_dls(self):
         subject = get_internal_name(self.station_name)
         consumer_group = get_internal_name(self.consumer_group)
         try:
@@ -95,15 +96,16 @@
                 subscription_name, subscription_name
             )
             async for msg in self.consumer_dls.messages:
                 index_to_insert = self.dls_current_index
                 if index_to_insert >= 10000:
                     index_to_insert %= 10000
                 self.dls_messages.insert(
-                    index_to_insert, Message(msg, self.connection, self.consumer_group)
+                    index_to_insert, Message(
+                        msg, self.connection, self.consumer_group)
                 )
                 self.dls_current_index += 1
                 if self.dls_callback_func != None:
                     await self.dls_callback_func(
                         [Message(msg, self.connection, self.consumer_group)],
                         None,
                         self.context,
@@ -115,43 +117,44 @@
 
     async def fetch(self, batch_size: int = 10):
         """Fetch a batch of messages."""
         messages = []
         if self.connection.is_connection_active:
             try:
                 if batch_size > self.MAX_BATCH_SIZE:
-                    raise MemphisError(f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
+                    raise MemphisError(
+                        f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
                 self.batch_size = batch_size
                 if len(self.dls_messages) > 0:
                     if len(self.dls_messages) <= batch_size:
                         messages = self.dls_messages
                         self.dls_messages = []
                         self.dls_current_index = 0
                     else:
                         messages = self.dls_messages[0:batch_size]
                         del self.dls_messages[0:batch_size]
                         self.dls_current_index -= len(messages)
                     return messages
 
-                durableName = ""
+                durable_name = ""
                 if self.consumer_group != "":
-                    durableName = get_internal_name(self.consumer_group)
+                    durable_name = get_internal_name(self.consumer_group)
                 else:
-                    durableName = get_internal_name(self.consumer_name)
+                    durable_name = get_internal_name(self.consumer_name)
                 subject = get_internal_name(self.station_name)
-                consumer_group = get_internal_name(self.consumer_group)
                 self.psub = await self.connection.broker_connection.pull_subscribe(
-                    subject + ".final", durable=durableName
+                    subject + ".final", durable=durable_name
                 )
                 msgs = await self.psub.fetch(batch_size)
                 for msg in msgs:
-                    messages.append(Message(msg, self.connection, self.consumer_group))
+                    messages.append(
+                        Message(msg, self.connection, self.consumer_group))
                 return messages
             except Exception as e:
-                if not "timeout" in str(e):
+                if "timeout" not in str(e):
                     raise MemphisError(str(e)) from e
         else:
             return messages
 
     async def __ping_consumer(self, callback):
         while True:
             try:
@@ -170,25 +173,26 @@
             self.t_consume.cancel()
         if self.t_dls is not None:
             self.t_dls.cancel()
         if self.t_ping is not None:
             self.t_ping.cancel()
         self.pull_interval_ms = None
         try:
-            destroyConsumerReq = {
+            destroy_consumer_req = {
                 "name": self.consumer_name,
                 "station_name": self.station_name,
-                "username": self.connection.username,
+                "username": self.connection.username
             }
-            consumer_name = json.dumps(destroyConsumerReq, indent=2).encode("utf-8")
+            consumer_name = json.dumps(
+                destroy_consumer_req, indent=2).encode("utf-8")
             res = await self.connection.broker_manager.request(
                 "$memphis_consumer_destructions", consumer_name, timeout=5
             )
             error = res.data.decode("utf-8")
             if error != "" and not "not exist" in error:
                 raise MemphisError(error)
             self.dls_messages.clear()
             internal_station_name = get_internal_name(self.station_name)
             map_key = internal_station_name + "_" + self.consumer_name.lower()
             del self.connection.consumers_map[map_key]
         except Exception as e:
-            raise MemphisError(str(e)) from e
+            raise MemphisError(str(e)) from e
```

### Comparing `memphis-py-beta-1.0.2/memphis/exceptions.py` & `memphis-py-beta-1.0.3/memphis/exceptions.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.2/memphis/headers.py` & `memphis-py-beta-1.0.3/memphis/headers.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.2/memphis/memphis.py` & `memphis-py-beta-1.0.3/memphis/memphis.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,55 +11,51 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import asyncio
 import json
-import random
 import ssl
-import time
-from threading import Timer
-from typing import Callable, Iterable, Union
+from typing import Iterable, Union
 import uuid
+import base64
 
-import graphql
 import nats as broker
 from google.protobuf import descriptor_pb2, descriptor_pool
 from google.protobuf.message_factory import MessageFactory
 from graphql import build_schema as build_graphql_schema
-from graphql import parse as parse_graphql
-from graphql import validate as validate_graphql
-from jsonschema import validate
 from memphis.consumer import Consumer
-from memphis.exceptions import MemphisConnectError, MemphisError, MemphisHeaderError
+from memphis.exceptions import MemphisConnectError, MemphisError
 from memphis.headers import Headers
 from memphis.producer import Producer
 from memphis.station import Station
 from memphis.types import Retention, Storage
 from memphis.utils import get_internal_name, random_bytes
 
 
 class Memphis:
     MAX_BATCH_SIZE = 5000
+    MEMPHIS_GLOBAL_ACCOUNT_NAME = "$memphis"
+
     def __init__(self):
         self.is_connection_active = False
         self.schema_updates_data = {}
         self.schema_updates_subs = {}
         self.producers_per_station = {}
         self.schema_tasks = {}
         self.proto_msgs = {}
         self.graphql_schemas = {}
         self.json_schemas = {}
         self.cluster_configurations = {}
         self.station_schemaverse_to_dls = {}
         self.update_configurations_sub = {}
         self.configuration_tasks = {}
-        self.producers_map = dict()
-        self.consumers_map = dict()
+        self.producers_map = {}
+        self.consumers_map = {}
 
     async def get_msgs_sdk_clients_updates(self, iterable: Iterable):
         try:
             async for msg in iterable:
                 message = msg.data.decode("utf-8")
                 data = json.loads(message)
                 if data["type"] == "send_notification":
@@ -86,60 +82,86 @@
                     self.update_configurations_sub.messages
                 )
             )
             self.configuration_tasks = task
         except Exception as err:
             raise MemphisError(err)
 
+    async def get_broker_manager_connection(self, connection_opts):
+        if "user" in connection_opts:
+            ping_connection_opts = connection_opts
+            ping_connection_opts["allow_reconnect"] = False
+            try:
+                conn = await broker.connect(**ping_connection_opts)
+                await conn.close()
+            except Exception as e:
+                if "authorization violation" in str(e).lower():
+                    try:
+                        ping_connection_opts["user"] = self.username
+                        conn = await broker.connect(**ping_connection_opts)
+                        await conn.close()
+                        connection_opts["user"] = self.username
+                    except Exception as e_1:
+                        raise e_1
+                else:
+                    raise e
+
+        return await broker.connect(**connection_opts)
+
     async def connect(
         self,
         host: str,
         username: str,
+        account_id: int = 1,
         connection_token: str = "",
         password: str = "",
         port: int = 6666,
         reconnect: bool = True,
         max_reconnect: int = 10,
         reconnect_interval_ms: int = 1500,
-        timeout_ms: int = 15000,
+        timeout_ms: int = 2000,
         cert_file: str = "",
         key_file: str = "",
         ca_file: str = "",
     ):
         """Creates connection with Memphis.
         Args:
             host (str): memphis host.
             username (str): user of type root/application.
+            account_id (int): You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
             connection_token (str): connection token.
             password (str): depends on how Memphis deployed - default is connection token-based authentication.
             port (int, optional): port. Defaults to 6666.
             reconnect (bool, optional): whether to do reconnect while connection is lost. Defaults to True.
             max_reconnect (int, optional): The reconnect attempt. Defaults to 3.
             reconnect_interval_ms (int, optional): Interval in milliseconds between reconnect attempts. Defaults to 200.
             timeout_ms (int, optional): connection timeout in milliseconds. Defaults to 15000.
             key_file (string): path to tls key file.
             cert_file (string): path to tls cert file.
             ca_file (string): path to tls ca file.
         """
         self.host = self.__normalize_host(host)
         self.username = username
+        self.account_id = account_id
         self.connection_token = connection_token
         self.password = password
         self.port = port
         self.reconnect = reconnect
         self.max_reconnect = 9 if max_reconnect > 9 else max_reconnect
         self.reconnect_interval_ms = reconnect_interval_ms
         self.timeout_ms = timeout_ms
         self.connection_id = str(uuid.uuid4())
         try:
             if self.connection_token != "" and self.password != "":
-                raise MemphisConnectError("You have to connect with one of the following methods: connection token / password")
+                raise MemphisConnectError(
+                    "You have to connect with one of the following methods: connection token / password")
             if self.connection_token == "" and self.password == "":
-                raise MemphisConnectError("You have to connect with one of the following methods: connection token / password")
-            
+                raise MemphisConnectError(
+                    "You have to connect with one of the following methods: connection token / password")
+
             connection_opts = {
                 "servers": self.host + ":" + str(self.port),
                 "allow_reconnect": self.reconnect,
                 "reconnect_time_wait": self.reconnect_interval_ms / 1000,
                 "connect_timeout": self.timeout_ms / 1000,
                 "max_reconnect_attempts": self.max_reconnect,
                 "name": self.connection_id + "::" + self.username,
@@ -147,36 +169,38 @@
             if cert_file != "" or key_file != "" or ca_file != "":
                 if cert_file == "":
                     raise MemphisConnectError("Must provide a TLS cert file")
                 if key_file == "":
                     raise MemphisConnectError("Must provide a TLS key file")
                 if ca_file == "":
                     raise MemphisConnectError("Must provide a TLS ca file")
-                ssl_ctx = ssl.create_default_context(purpose=ssl.Purpose.SERVER_AUTH)
+                ssl_ctx = ssl.create_default_context(
+                    purpose=ssl.Purpose.SERVER_AUTH)
                 ssl_ctx.load_verify_locations(ca_file)
                 ssl_ctx.load_cert_chain(certfile=cert_file, keyfile=key_file)
                 connection_opts["tls"] = ssl_ctx
                 connection_opts["tls_hostname"] = self.host
             if self.connection_token != "":
-                connection_opts["token"]=self.connection_token
+                connection_opts["token"] = self.connection_token
             else:
-                connection_opts["user"]=self.username
-                connection_opts["password"]=self.password
+                connection_opts["user"] = self.username + \
+                    "$" + str(self.account_id)
+                connection_opts["password"] = self.password
 
-            self.broker_manager = await broker.connect(**connection_opts)
+            self.broker_manager = await self.get_broker_manager_connection(connection_opts)
             await self.sdk_client_updates_listener()
             self.broker_connection = self.broker_manager.jetstream()
             self.is_connection_active = True
         except Exception as e:
             raise MemphisError(str(e))
 
-    async def send_notification(self, title, msg, failedMsg, type):
-        msg = {"title": title, "msg": msg, "type": type, "code": failedMsg}
-        msgToSend = json.dumps(msg).encode("utf-8")
-        await self.broker_manager.publish("$memphis_notifications", msgToSend)
+    async def send_notification(self, title, msg, failed_msg, not_type):
+        msg = {"title": title, "msg": msg, "type": not_type, "code": failed_msg}
+        msg_to_send = json.dumps(msg).encode("utf-8")
+        await self.broker_manager.publish("$memphis_notifications", msg_to_send)
 
     async def station(
         self,
         name: str,
         retention_type: Retention = Retention.MAX_MESSAGE_AGE_SECONDS,
         retention_value: int = 604800,
         storage_type: Storage = Storage.DISK,
@@ -199,84 +223,84 @@
         Returns:
             object: station
         """
         try:
             if not self.is_connection_active:
                 raise MemphisError("Connection is dead")
 
-            createStationReq = {
+            create_station_req = {
                 "name": name,
                 "retention_type": retention_type.value,
                 "retention_value": retention_value,
                 "storage_type": storage_type.value,
                 "replicas": replicas,
                 "idempotency_window_in_ms": idempotency_window_ms,
                 "schema_name": schema_name,
                 "dls_configuration": {
                     "poison": send_poison_msg_to_dls,
                     "Schemaverse": send_schema_failed_msg_to_dls,
                 },
                 "username": self.username,
-                "tiered_storage_enabled": tiered_storage_enabled,
+                "tiered_storage_enabled": tiered_storage_enabled
             }
-            create_station_req_bytes = json.dumps(createStationReq, indent=2).encode(
+            create_station_req_bytes = json.dumps(create_station_req, indent=2).encode(
                 "utf-8"
             )
             err_msg = await self.broker_manager.request(
                 "$memphis_station_creations", create_station_req_bytes, timeout=5
             )
             err_msg = err_msg.data.decode("utf-8")
 
             if err_msg != "":
                 raise MemphisError(err_msg)
             return Station(self, name)
 
         except Exception as e:
             if str(e).find("already exist") != -1:
                 return Station(self, name.lower())
-            else:
-                raise MemphisError(str(e)) from e
+            raise MemphisError(str(e)) from e
 
-    async def attach_schema(self, name, stationName):
+    async def attach_schema(self, name, station_name):
         """Attaches a schema to an existing station.
         Args:
             name (str): schema name.
-            stationName (str): station name.
+            station_name (str): station name.
         Raises:
             Exception: _description_
         """
         try:
-            if name == "" or stationName == "":
+            if name == "" or station_name == "":
                 raise MemphisError("name and station name can not be empty")
-            msg = {"name": name, "station_name": stationName, "username": self.username}
-            msgToSend = json.dumps(msg).encode("utf-8")
+            msg = {"name": name, "station_name": station_name,
+                   "username": self.username}
+            msg_to_send = json.dumps(msg).encode("utf-8")
             err_msg = await self.broker_manager.request(
-                "$memphis_schema_attachments", msgToSend, timeout=5
+                "$memphis_schema_attachments", msg_to_send, timeout=5
             )
             err_msg = err_msg.data.decode("utf-8")
 
             if err_msg != "":
                 raise MemphisError(err_msg)
         except Exception as e:
             raise MemphisError(str(e)) from e
 
-    async def detach_schema(self, stationName):
+    async def detach_schema(self, station_name):
         """Detaches a schema from station.
         Args:
-            stationName (str): station name.
+            station_name (str): station name.
         Raises:
             Exception: _description_
         """
         try:
-            if stationName == "":
+            if station_name == "":
                 raise MemphisError("station name is missing")
-            msg = {"station_name": stationName, "username": self.username}
-            msgToSend = json.dumps(msg).encode("utf-8")
+            msg = {"station_name": station_name, "username": self.username}
+            msg_to_send = json.dumps(msg).encode("utf-8")
             err_msg = await self.broker_manager.request(
-                "$memphis_schema_detachments", msgToSend, timeout=5
+                "$memphis_schema_detachments", msg_to_send, timeout=5
             )
             err_msg = err_msg.data.decode("utf-8")
 
             if err_msg != "":
                 raise MemphisError(err_msg)
         except Exception as e:
             raise MemphisError(str(e)) from e
@@ -307,27 +331,26 @@
                         await sub.unsubscribe()
                 if self.update_configurations_sub is not None:
                     await self.update_configurations_sub.unsubscribe()
                 self.producers_map.clear()
                 for consumer in self.consumers_map:
                     consumer.dls_messages.clear()
                 self.consumers_map.clear()
-        except:
+        except Exception:
             return
 
-    def __generateRandomSuffix(self, name: str) -> str:
+    def __generate_random_suffix(self, name: str) -> str:
         return name + "_" + random_bytes(8)
 
     def __normalize_host(self, host):
         if host.startswith("http://"):
             return host.split("http://")[1]
-        elif host.startswith("https://"):
+        if host.startswith("https://"):
             return host.split("https://")[1]
-        else:
-            return host
+        return host
 
     async def producer(
         self,
         station_name: str,
         producer_name: str,
         generate_random_suffix: bool = False,
     ):
@@ -342,24 +365,24 @@
             _type_: _description_
         """
         try:
             if not self.is_connection_active:
                 raise MemphisError("Connection is dead")
             real_name = producer_name.lower()
             if generate_random_suffix:
-                producer_name = self.__generateRandomSuffix(producer_name)
-            createProducerReq = {
+                producer_name = self.__generate_random_suffix(producer_name)
+            create_producer_req = {
                 "name": producer_name,
                 "station_name": station_name,
                 "connection_id": self.connection_id,
                 "producer_type": "application",
                 "req_version": 1,
-                "username": self.username,
+                "username": self.username
             }
-            create_producer_req_bytes = json.dumps(createProducerReq, indent=2).encode(
+            create_producer_req_bytes = json.dumps(create_producer_req, indent=2).encode(
                 "utf-8"
             )
             create_res = await self.broker_manager.request(
                 "$memphis_producer_creations", create_producer_req_bytes, timeout=5
             )
             create_res = create_res.data.decode("utf-8")
             create_res = json.loads(create_res)
@@ -383,15 +406,16 @@
                     == "protobuf"
                 ):
                     self.parse_descriptor(internal_station_name)
                 if self.schema_updates_data[internal_station_name]["type"] == "json":
                     schema = self.schema_updates_data[internal_station_name][
                         "active_version"
                     ]["schema_content"]
-                    self.json_schemas[internal_station_name] = json.loads(schema)
+                    self.json_schemas[internal_station_name] = json.loads(
+                        schema)
                 elif (
                     self.schema_updates_data[internal_station_name]["type"] == "graphql"
                 ):
                     self.graphql_schemas[internal_station_name] = build_graphql_schema(
                         self.schema_updates_data[internal_station_name][
                             "active_version"
                         ]["schema_content"]
@@ -420,15 +444,15 @@
             descriptor = self.schema_updates_data[station_name]["active_version"][
                 "descriptor"
             ]
             msg_struct_name = self.schema_updates_data[station_name]["active_version"][
                 "message_struct_name"
             ]
             desc_set = descriptor_pb2.FileDescriptorSet()
-            descriptor_bytes = str.encode(descriptor)
+            descriptor_bytes = base64.b64decode(descriptor)
             desc_set.ParseFromString(descriptor_bytes)
             pool = descriptor_pool.DescriptorPool()
             pool.Add(desc_set.file[0])
             pkg_name = desc_set.file[0].package
             msg_name = msg_struct_name
             if pkg_name != "":
                 msg_name = desc_set.file[0].package + "." + msg_struct_name
@@ -497,47 +521,48 @@
         Returns:
             object: consumer
         """
         try:
             if not self.is_connection_active:
                 raise MemphisError("Connection is dead")
             if batch_size > self.MAX_BATCH_SIZE:
-                raise MemphisError(f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
+                raise MemphisError(
+                    f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
             real_name = consumer_name.lower()
             if generate_random_suffix:
-                consumer_name = self.__generateRandomSuffix(consumer_name)
+                consumer_name = self.__generate_random_suffix(consumer_name)
             cg = consumer_name if not consumer_group else consumer_group
 
             if start_consume_from_sequence <= 0:
                 raise MemphisError(
                     "start_consume_from_sequence has to be a positive number"
                 )
 
             if last_messages < -1:
                 raise MemphisError("min value for last_messages is -1")
 
             if start_consume_from_sequence > 1 and last_messages > -1:
                 raise MemphisError(
                     "Consumer creation options can't contain both start_consume_from_sequence and last_messages"
                 )
-            createConsumerReq = {
+            create_consumer_req = {
                 "name": consumer_name,
                 "station_name": station_name,
                 "connection_id": self.connection_id,
                 "consumer_type": "application",
                 "consumers_group": consumer_group,
                 "max_ack_time_ms": max_ack_time_ms,
                 "max_msg_deliveries": max_msg_deliveries,
                 "start_consume_from_sequence": start_consume_from_sequence,
                 "last_messages": last_messages,
                 "req_version": 1,
-                "username": self.username,
+                "username": self.username
             }
 
-            create_consumer_req_bytes = json.dumps(createConsumerReq, indent=2).encode(
+            create_consumer_req_bytes = json.dumps(create_consumer_req, indent=2).encode(
                 "utf-8"
             )
             err_msg = await self.broker_manager.request(
                 "$memphis_consumer_creations", create_consumer_req_bytes, timeout=5
             )
             err_msg = err_msg.data.decode("utf-8")
 
@@ -637,17 +662,19 @@
             last_messages: consume the last N messages, defaults to -1 (all messages in the station).
         Returns:
             list: Message
         """
         try:
             consumer = None
             if not self.is_connection_active:
-                raise MemphisError("Cant fetch messages without being connected!")
+                raise MemphisError(
+                    "Cant fetch messages without being connected!")
             if batch_size > self.MAX_BATCH_SIZE:
-                raise MemphisError(f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
+                raise MemphisError(
+                    f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
             internal_station_name = get_internal_name(station_name)
             consumer_map_key = internal_station_name + "_" + consumer_name.lower()
             if consumer_map_key in self.consumers_map:
                 consumer = self.consumers_map[consumer_map_key]
             else:
                 consumer = await self.consumer(
                     station_name=station_name,
@@ -666,30 +693,29 @@
                 messages = []
             return messages
         except Exception as e:
             raise MemphisError(str(e)) from e
 
     def is_connected(self):
         return self.broker_manager.is_connected
-    
+
     def unset_cached_producer_station(self, station_name):
         try:
             internal_station_name = get_internal_name(station_name)
             for key in list(self.producers_map):
                 producer = self.producers_map[key]
                 if producer.internal_station_name == internal_station_name:
                     del self.producers_map[key]
         except Exception as e:
             raise e
-    
 
     def unset_cached_consumer_station(self, station_name):
         try:
             internal_station_name = get_internal_name(station_name)
             for key in list(self.consumers_map):
                 consumer = self.consumers_map[key]
-                consumer_station_name_internal = get_internal_name(consumer.station_name)
+                consumer_station_name_internal = get_internal_name(
+                    consumer.station_name)
                 if consumer_station_name_internal == internal_station_name:
                     del self.consumers_map[key]
         except Exception as e:
             raise e
-
```

### Comparing `memphis-py-beta-1.0.2/memphis/message.py` & `memphis-py-beta-1.0.3/memphis/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,50 +21,49 @@
                 and "$memphis_pm_cg_name" in self.message.headers
             ):
                 try:
                     msg = {
                         "id": int(self.message.headers["$memphis_pm_id"]),
                         "cg_name": self.message.headers["$memphis_pm_cg_name"],
                     }
-                    msgToAck = json.dumps(msg).encode("utf-8")
+                    msg_to_ack = json.dumps(msg).encode("utf-8")
                     await self.connection.broker_manager.publish(
-                        "$memphis_pm_acks", msgToAck
+                        "$memphis_pm_acks", msg_to_ack
                     )
-                except Exception as er:
-                    raise MemphisConnectError(str(er)) from er
+                except Exception as e_1:
+                    raise MemphisConnectError(str(e_1))
             else:
                 raise MemphisConnectError(str(e)) from e
             return
 
     def get_data(self):
         """Receive the message."""
         try:
             return bytearray(self.message.data)
-        except:
+        except Exception:
             return
 
     def get_headers(self):
         """Receive the headers."""
         try:
             return self.message.headers
-        except:
+        except Exception:
             return
 
     def get_sequence_number(self):
         """Get message sequence number."""
         try:
             return self.message.metadata.sequence.stream
-        except:
+        except Exception:
             return
 
     async def delay(self, delay):
         """Delay and resend the message after delay seconds"""
         if (
             "$memphis_pm_id" in self.message.headers
             and "$memphis_pm_cg_name" in self.message.headers
         ):
             raise MemphisError("cannot delay DLS message")
-        else:
-            try:
-                await self.message.nak(delay=delay)
-            except Exception as e:
-                raise MemphisError(str(e)) from e
+        try:
+            await self.message.nak(delay=delay)
+        except Exception as e:
+            raise MemphisError(str(e)) from e
```

### Comparing `memphis-py-beta-1.0.2/memphis/producer.py` & `memphis-py-beta-1.0.3/memphis/producer.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import time
 from typing import Union
 
 import graphql
 from graphql import parse as parse_graphql
 from graphql import validate as validate_graphql
 from jsonschema import validate
+import google.protobuf.json_format as protobuf_json_format
 from memphis.exceptions import MemphisError, MemphisSchemaError
 from memphis.headers import Headers
 from memphis.utils import get_internal_name
 
-schemaVFailAlertType = "schema_validation_fail_alert"
+schemaverse_fail_alert_type = "schema_validation_fail_alert"
 
 
 class Producer:
     def __init__(
         self, connection, producer_name: str, station_name: str, real_name: str
     ):
         self.connection = connection
@@ -31,59 +32,75 @@
         if self.connection.schema_updates_data[self.internal_station_name] != {}:
             schema_type = self.connection.schema_updates_data[
                 self.internal_station_name
             ]["type"]
             if schema_type == "protobuf":
                 message = self.validate_protobuf(message)
                 return message
-            elif schema_type == "json":
+            if schema_type == "json":
                 message = self.validate_json_schema(message)
                 return message
-            elif schema_type == "graphql":
+            if schema_type == "graphql":
                 message = self.validate_graphql(message)
                 return message
-            elif hasattr(message, "SerializeToString"):
-                msgToSend = message.SerializeToString()
-                return msgToSend
+            if hasattr(message, "SerializeToString"):
+                msg_to_send = message.SerializeToString()
+                return msg_to_send
         elif isinstance(message, str):
             message = message.encode("utf-8")
             return message
         elif isinstance(message, graphql.language.ast.DocumentNode):
             msg = message
             message = str(msg.loc.source.body)
             message = message.encode("utf-8")
             return message
+        elif hasattr(message, "SerializeToString"):
+            msg_to_send = message.SerializeToString()
+            return msg_to_send
         elif not isinstance(message, bytearray) and not isinstance(message, dict):
             raise MemphisSchemaError("Unsupported message type")
         else:
             if isinstance(message, dict):
                 message = bytearray(json.dumps(message).encode("utf-8"))
             return message
 
     def validate_protobuf(self, message):
         proto_msg = self.connection.proto_msgs[self.internal_station_name]
-        msgToSend = ""
+        msg_to_send = ""
         try:
             if isinstance(message, bytearray):
-                msgToSend = bytes(message)
+                msg_to_send = bytes(message)
                 try:
-                    proto_msg.ParseFromString(msgToSend)
+                    proto_msg.ParseFromString(msg_to_send)
                     proto_msg.SerializeToString()
-                    msgToSend = msgToSend.decode("utf-8")
+                    msg_to_send = msg_to_send.decode("utf-8")
                 except Exception as e:
                     if "parsing message" in str(e):
                         e = "Invalid message format, expecting protobuf"
                     raise MemphisSchemaError(str(e))
                 return message
-            elif hasattr(message, "SerializeToString"):
-                msgToSend = message.SerializeToString()
-                proto_msg.ParseFromString(msgToSend)
+            if hasattr(message, "SerializeToString"):
+                msg_to_send = message.SerializeToString()
+                proto_msg.ParseFromString(msg_to_send)
                 proto_msg.SerializeToString()
-                return msgToSend
-
+                try:
+                    proto_msg.ParseFromString(msg_to_send)
+                    proto_msg.SerializeToString()
+                except Exception as e:
+                    if "parsing message" in str(e):
+                        e = "Error parsing protobuf message"
+                    raise MemphisSchemaError(str(e))
+                return msg_to_send
+            elif isinstance(message, dict):
+                try:
+                    protobuf_json_format.ParseDict(message, proto_msg)
+                    msg_to_send = proto_msg.SerializeToString()
+                    return msg_to_send
+                except Exception as e:
+                    raise MemphisSchemaError(str(e))
             else:
                 raise MemphisSchemaError("Unsupported message type")
 
         except Exception as e:
             raise MemphisSchemaError("Schema validation has failed: " + str(e))
 
     def validate_json_schema(self, message):
@@ -156,15 +173,15 @@
             message = await self.validate_msg(message)
 
             memphis_headers = {
                 "$memphis_producedBy": self.producer_name,
                 "$memphis_connectionId": self.connection.connection_id,
             }
 
-            if msg_id is not None:
+            if msg_id is not None and msg_id != "":
                 memphis_headers["msg-id"] = msg_id
 
             if headers is not None:
                 headers = headers.headers
                 headers.update(memphis_headers)
             else:
                 headers = memphis_headers
@@ -195,80 +212,80 @@
                     "Produce operation has failed, please check whether Station/Producer still exist"
                 )
             else:
                 if "Schema validation has failed" in str(
                     e
                 ) or "Unsupported message type" in str(e):
                     if self.connection.schema_updates_data[self.internal_station_name] != {}:
-                        msgToSend = ""
+                        msg_to_send = ""
                         if hasattr(message, "SerializeToString"):
-                            msgToSend = message.SerializeToString().decode("utf-8")
+                            msg_to_send = message.SerializeToString().decode("utf-8")
                         elif isinstance(message, bytearray):
-                            msgToSend = str(message, "utf-8")
+                            msg_to_send = str(message, "utf-8")
                         else:
-                            msgToSend = str(message)
+                            msg_to_send = str(message)
                         if self.connection.station_schemaverse_to_dls[
                             self.internal_station_name
                         ]:
                             unix_time = int(time.time())
 
                             memphis_headers = {
                                 "$memphis_producedBy": self.producer_name,
                                 "$memphis_connectionId": self.connection.connection_id,
                             }
 
-                            if headers != {}:
+                            if headers != {} and not headers == None:
                                 headers = headers.headers
                                 headers.update(memphis_headers)
                             else:
                                 headers = memphis_headers
 
-                            msgToSendEncoded = msgToSend.encode("utf-8")
-                            msgHex = msgToSendEncoded.hex()
+                            msg_to_send_encoded = msg_to_send.encode("utf-8")
+                            msg_hex = msg_to_send_encoded.hex()
                             buf = {
                                 "station_name": self.internal_station_name,
                                 "producer": {
                                     "name": self.producer_name,
                                     "connection_id": self.connection.connection_id,
                                 },
                                 "creation_unix": unix_time,
                                 "message": {
-                                    "data": msgHex,
+                                    "data": msg_hex,
                                     "headers": headers,
                                 },
-                                "validation_error": str(e),
+                                "validation_error": str(e)
                             }
                             buf = json.dumps(buf).encode("utf-8")
                             await self.connection.broker_manager.publish("$memphis_schemaverse_dls", buf)
                             if self.connection.cluster_configurations.get(
                                 "send_notification"
                             ):
                                 await self.connection.send_notification(
                                     "Schema validation has failed",
                                     "Station: "
                                     + self.station_name
                                     + "\nProducer: "
                                     + self.producer_name
                                     + "\nError:"
                                     + str(e),
-                                    msgToSend,
-                                    schemaVFailAlertType,
+                                    msg_to_send,
+                                    schemaverse_fail_alert_type,
                                 )
                 raise MemphisError(str(e)) from e
 
     async def destroy(self):
         """Destroy the producer."""
         try:
-            destroyProducerReq = {
+            destroy_producer_req = {
                 "name": self.producer_name,
                 "station_name": self.station_name,
-                "username": self.connection.username,
+                "username": self.connection.username
             }
 
-            producer_name = json.dumps(destroyProducerReq).encode("utf-8")
+            producer_name = json.dumps(destroy_producer_req).encode("utf-8")
             res = await self.connection.broker_manager.request(
                 "$memphis_producer_destructions", producer_name, timeout=5
             )
             error = res.data.decode("utf-8")
             if error != "" and not "not exist" in error:
                 raise Exception(error)
```

### Comparing `memphis-py-beta-1.0.2/memphis/station.py` & `memphis-py-beta-1.0.3/memphis/station.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def __init__(self, connection, name: str):
         self.connection = connection
         self.name = name.lower()
 
     async def destroy(self):
         """Destroy the station."""
         try:
-            nameReq = {"station_name": self.name, "username": self.connection.username}
-            station_name = json.dumps(nameReq, indent=2).encode("utf-8")
+            name_req = {"station_name": self.name, "username": self.connection.username}
+            station_name = json.dumps(name_req, indent=2).encode("utf-8")
             res = await self.connection.broker_manager.request(
                 "$memphis_station_destructions", station_name, timeout=5
             )
             error = res.data.decode("utf-8")
             if error != "" and not "not exist" in error:
                 raise MemphisError(error)
```

### Comparing `memphis-py-beta-1.0.2/memphis/types.py` & `memphis-py-beta-1.0.3/memphis/types.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.2/memphis/utils.py` & `memphis-py-beta-1.0.3/memphis/utils.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-1.0.2/memphis_py_beta.egg-info/PKG-INFO` & `memphis-py-beta-1.0.3/memphis_py_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 1.0.2
+Version: 1.0.3
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.3.tar.gz
 Description: <div align="center">
           
           ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
@@ -70,14 +70,15 @@
         ```python
         async def main():
           try:
             memphis = Memphis()
             await memphis.connect(
               host="<memphis-host>",
               username="<application-type username>",
+              account_id="<account_id>", # You can find it on the profile page in the Memphis UI. This field should be sent only on the cloud version of Memphis, otherwise it will be ignored
               connection_token="<broker-token>", # you will get it on application type user creation
               password="<string>", # depends on how Memphis deployed - default is connection token-based authentication
               port="<port>", # defaults to 6666
               reconnect=True, # defaults to True
               max_reconnect=3, # defaults to 3
               reconnect_interval_ms=1500, # defaults to 1500
               timeout_ms=1500, # defaults to 1500
```

### Comparing `memphis-py-beta-1.0.2/setup.py` & `memphis-py-beta-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="memphis-py-beta",
     packages=["memphis"],
-    version="1.0.2",
+    version="1.0.3",
     license="Apache-2.0",
     description="A powerful messaging platform for modern developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Memphis.dev",
     author_email="team@memphis.dev",
     url="https://github.com/memphisdev/memphis.py",
-    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz",
+    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.3.tar.gz",
     keywords=["message broker", "devtool", "streaming", "data"],
     install_requires=["asyncio", "nats-py", "protobuf", "jsonschema", "graphql-core"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

