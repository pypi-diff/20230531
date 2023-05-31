# Comparing `tmp/aleph-message-0.3.2.tar.gz` & `tmp/aleph-message-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-message-0.3.2.tar", last modified: Fri Mar 10 15:28:53 2023, max compression
+gzip compressed data, was "aleph-message-0.4.0a1.tar", last modified: Wed May 31 12:38:01 2023, max compression
```

## Comparing `aleph-message-0.3.2.tar` & `aleph-message-0.4.0a1.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxrwxr-x   0 odesenfans  (1000) odesenfans  (1000)        0 2023-03-10 15:28:53.376451 aleph-message-0.3.2/
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)     1062 2022-05-30 13:08:32.000000 aleph-message-0.3.2/LICENSE
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)     1978 2023-03-10 15:28:53.376451 aleph-message-0.3.2/PKG-INFO
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)     1458 2023-03-10 15:05:17.000000 aleph-message-0.3.2/README.md
-drwxrwxr-x   0 odesenfans  (1000) odesenfans  (1000)        0 2023-03-10 15:28:53.372450 aleph-message-0.3.2/aleph_message/
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)       46 2022-05-30 13:08:32.000000 aleph-message-0.3.2/aleph_message/__init__.py
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)       44 2022-09-20 14:02:16.000000 aleph-message-0.3.2/aleph_message/exceptions.py
-drwxrwxr-x   0 odesenfans  (1000) odesenfans  (1000)        0 2023-03-10 15:28:53.376451 aleph-message-0.3.2/aleph_message/models/
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)    11673 2023-03-10 15:18:43.000000 aleph-message-0.3.2/aleph_message/models/__init__.py
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)      698 2022-09-20 14:02:16.000000 aleph-message-0.3.2/aleph_message/models/abstract.py
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)     1930 2023-01-20 15:42:36.000000 aleph-message-0.3.2/aleph_message/models/item_hash.py
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)     6056 2023-03-10 15:05:17.000000 aleph-message-0.3.2/aleph_message/models/program.py
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)      483 2023-03-10 15:05:17.000000 aleph-message-0.3.2/aleph_message/status.py
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)      304 2023-01-20 15:42:36.000000 aleph-message-0.3.2/aleph_message/utils.py
-drwxrwxr-x   0 odesenfans  (1000) odesenfans  (1000)        0 2023-03-10 15:28:53.372450 aleph-message-0.3.2/aleph_message.egg-info/
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)     1978 2023-03-10 15:28:53.000000 aleph-message-0.3.2/aleph_message.egg-info/PKG-INFO
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)      443 2023-03-10 15:28:53.000000 aleph-message-0.3.2/aleph_message.egg-info/SOURCES.txt
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)        1 2023-03-10 15:28:53.000000 aleph-message-0.3.2/aleph_message.egg-info/dependency_links.txt
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)       42 2023-03-10 15:28:53.000000 aleph-message-0.3.2/aleph_message.egg-info/requires.txt
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)       14 2023-03-10 15:28:53.000000 aleph-message-0.3.2/aleph_message.egg-info/top_level.txt
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)       38 2023-03-10 15:28:53.376451 aleph-message-0.3.2/setup.cfg
--rw-rw-r--   0 odesenfans  (1000) odesenfans  (1000)     1334 2023-03-10 15:23:54.000000 aleph-message-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-01-12 17:02:10.000000 aleph-message-0.4.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.991991 aleph-message-0.4.0a1/aleph_message/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-01-12 17:02:10.000000 aleph-message-0.4.0a1/aleph_message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/aleph_message/models/
+-rw-r--r--   0 root         (0) root         (0)    12676 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-01-12 17:02:10.000000 aleph-message-0.4.0a1/aleph_message/models/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/aleph_message/models/execution/
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/abstract.py
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/base.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/environment.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-31 12:29:26.000000 aleph-message-0.4.0a1/aleph_message/models/execution/instance.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/program.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-05-31 12:29:26.000000 aleph-message-0.4.0a1/aleph_message/models/execution/volume.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/item_hash.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/status.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.991991 aleph-message-0.4.0a1/aleph_message.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-31 12:31:55.000000 aleph-message-0.4.0a1/setup.py
```

### Comparing `aleph-message-0.3.2/LICENSE` & `aleph-message-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-message-0.3.2/PKG-INFO` & `aleph-message-0.4.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: aleph-message
-Version: 0.3.2
+Version: 0.4.0a1
 Summary: Aleph.im message specification 
 Home-page: https://github.com/aleph-im/aleph-message
 Author: Hugo Herter
 Author-email: git@hugoherter.com
 License: MIT
 Keywords: aleph.im message validation specification
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Distributed Computing
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -39,21 +40,23 @@
 
 ```shell
 pip install aleph-message
 ```
 
 ```python
 import requests
-from aleph_message import Message
+from aleph_message import parse_message
 from pydantic import ValidationError
 
 ALEPH_API_SERVER = "https://official.aleph.cloud"
 MESSAGE_ITEM_HASH = "9b21eb870d01bf64d23e1d4475e342c8f958fcd544adc37db07d8281da070b00"
 
 message_dict = requests.get(ALEPH_API_SERVER + "/api/v0/messages.json?hashes=" + MESSAGE_ITEM_HASH).json()
 
 try:
-    message = Message(**message_dict["messages"][0])
+    message = parse_message(message_dict["messages"][0])
     print(message.sender)
 except ValidationError as e:
     print(e.json(indent=4))
 ```
+
+
```

### Comparing `aleph-message-0.3.2/README.md` & `aleph-message-0.4.0a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 ```shell
 pip install aleph-message
 ```
 
 ```python
 import requests
-from aleph_message import Message
+from aleph_message import parse_message
 from pydantic import ValidationError
 
 ALEPH_API_SERVER = "https://official.aleph.cloud"
 MESSAGE_ITEM_HASH = "9b21eb870d01bf64d23e1d4475e342c8f958fcd544adc37db07d8281da070b00"
 
 message_dict = requests.get(ALEPH_API_SERVER + "/api/v0/messages.json?hashes=" + MESSAGE_ITEM_HASH).json()
 
 try:
-    message = Message(**message_dict["messages"][0])
+    message = parse_message(message_dict["messages"][0])
     print(message.sender)
 except ValidationError as e:
     print(e.json(indent=4))
 ```
```

### Comparing `aleph-message-0.3.2/aleph_message/models/__init__.py` & `aleph-message-0.4.0a1/aleph_message/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import json
 from copy import copy
 from enum import Enum
 from hashlib import sha256
 from json import JSONDecodeError
 from pathlib import Path
-from typing import List, Dict, Any, Optional, Union, NewType
-
-from .item_hash import ItemHash, ItemType
-
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal
+from typing import (
+    Any,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Type,
+    Union,
+)
 
 from pydantic import BaseModel, Extra, Field, validator
+from typing_extensions import TypeAlias
 
 from .abstract import BaseContent
-from .program import ProgramContent
+from .execution.instance import InstanceContent
+from .execution.program import ProgramContent
+from .item_hash import ItemHash, ItemType
 
 
 class Chain(str, Enum):
     """Supported chains"""
 
     AVAX = "AVAX"
     BSC = "BSC"
@@ -43,14 +47,15 @@
 class MessageType(str, Enum):
     """Message types supported by Aleph"""
 
     post = "POST"
     aggregate = "AGGREGATE"
     store = "STORE"
     program = "PROGRAM"
+    instance = "INSTANCE"
     forget = "FORGET"
 
 
 class MongodbId(BaseModel):
     """PyAleph returns an internal MongoDB id"""
 
     oid: str = Field(alias="$oid")
@@ -86,15 +91,17 @@
 
     chain: Chain
     height: int
     hash: Union[str, MessageConfirmationHash]
     # These two optional fields are introduced in recent versions of CCNs. They should
     # remain optional until the corresponding CCN upload (0.4.0) is widely uploaded.
     time: Optional[float] = None
-    publisher: Optional[str] = Field(default=None, description="The address that published the transaction.")
+    publisher: Optional[str] = Field(
+        default=None, description="The address that published the transaction."
+    )
 
     class Config:
         extra = Extra.forbid
 
 
 class AggregateContentKey(BaseModel):
     name: str
@@ -209,26 +216,27 @@
     content: BaseContent = Field(description="Content of the message, ready to be used")
 
     forgotten_by: Optional[List[str]]
 
     @validator("item_content")
     def check_item_content(cls, v: Optional[str], values):
         item_type = values["item_type"]
-        if item_type == ItemType.inline:
+        if v is None:
+            return None
+        elif item_type == ItemType.inline:
             try:
                 json.loads(v)
             except JSONDecodeError:
                 raise ValueError(
                     "Field 'item_content' does not appear to be valid JSON"
                 )
         else:
-            if v is not None:
-                raise ValueError(
-                    f"Field 'item_content' cannot be defined when 'item_type' == '{item_type}'"
-                )
+            raise ValueError(
+                f"Field 'item_content' cannot be defined when 'item_type' == '{item_type}'"
+            )
         return v
 
     @validator("item_hash")
     def check_item_hash(cls, v, values):
         item_type = values["item_type"]
         if item_type == ItemType.inline:
             item_content: str = values["item_content"]
@@ -308,33 +316,58 @@
                 for key, value in item_content.items():
                     if vdict[key] != value:
                         print(f"{key}: {vdict[key]} != {value}")
                 raise ValueError("Content and item_content differ")
         return v
 
 
-message_types = (
+class InstanceMessage(BaseMessage):
+    type: Literal[MessageType.instance]
+    content: InstanceContent
+
+
+AlephMessage: TypeAlias = Union[
     PostMessage,
     AggregateMessage,
     StoreMessage,
     ProgramMessage,
+    InstanceMessage,
     ForgetMessage,
-)
+]
 
-AlephMessage = NewType("AlephMessage", Union[message_types])
+AlephMessageType: TypeAlias = Union[
+    Type[PostMessage],
+    Type[AggregateMessage],
+    Type[StoreMessage],
+    Type[ProgramMessage],
+    Type[InstanceMessage],
+    Type[ForgetMessage],
+]
 
+message_classes: List[AlephMessageType] = [
+    PostMessage,
+    AggregateMessage,
+    StoreMessage,
+    ProgramMessage,
+    InstanceMessage,
+    ForgetMessage,
+]
 
-def Message(**message_dict: Dict) -> AlephMessage:
+ExecutableContent: TypeAlias = Union[InstanceContent, ProgramContent]
+ExecutableMessage: TypeAlias = Union[InstanceMessage, ProgramMessage]
+
+
+def parse_message(message_dict: Dict) -> AlephMessage:
     """Returns the message class corresponding to the type of message."""
-    for message_class in message_types:
+    for message_class in message_classes:
         message_type: MessageType = MessageType(
             message_class.__annotations__["type"].__args__[0]
         )
         if message_dict["type"] == message_type:
-            return message_class(**message_dict)
+            return message_class.parse_obj(message_dict)
     else:
         raise ValueError(f"Unknown message type {message_dict['type']}")
 
 
 def add_item_content_and_hash(message_dict: Dict, inplace: bool = False):
     if not inplace:
         message_dict = copy(message_dict)
@@ -345,45 +378,57 @@
     message_dict["item_hash"] = sha256(
         message_dict["item_content"].encode()
     ).hexdigest()
     return message_dict
 
 
 def create_new_message(
-    message_dict: Dict, factory: Union[Message, AlephMessage] = Message
+    message_dict: Dict,
+    factory: Optional[AlephMessageType] = None,
 ) -> AlephMessage:
     """Create a new message from a dict.
     Computes the 'item_content' and 'item_hash' fields.
     """
-    return factory(**add_item_content_and_hash(message_dict))
+    message_content = add_item_content_and_hash(message_dict)
+    if factory:
+        return factory.parse_obj(message_content)
+    else:
+        return parse_message(message_content)
 
 
 def create_message_from_json(
-    json_data: str, factory: Union[Message, AlephMessage] = Message
+    json_data: str,
+    factory: Optional[AlephMessageType] = None,
 ) -> AlephMessage:
     """Create a new message from a JSON encoded string.
     Computes the 'item_content' and 'item_hash' fields.
     """
     message_dict = json.loads(json_data)
-    add_item_content_and_hash(message_dict, inplace=True)
-    return factory(**message_dict)
+    message_content = add_item_content_and_hash(message_dict, inplace=True)
+    if factory:
+        return factory.parse_obj(message_content)
+    else:
+        return parse_message(message_content)
 
 
 def create_message_from_file(
-    filepath: Path, factory: Union[Message, AlephMessage] = Message, decoder=json
+    filepath: Path, factory: Optional[AlephMessageType] = None, decoder=json
 ) -> AlephMessage:
     """Create a new message from an encoded file.
     Expects json by default, but allows other decoders with a method `.load()`
     that takes a file descriptor.
     Computes the 'item_content' and 'item_hash' fields.
     """
     with open(filepath) as fd:
         message_dict = decoder.load(fd)
-    add_item_content_and_hash(message_dict, inplace=True)
-    return factory(**message_dict)
+    message_content = add_item_content_and_hash(message_dict, inplace=True)
+    if factory:
+        return factory.parse_obj(message_content)
+    else:
+        return parse_message(message_content)
 
 
 class MessagesResponse(BaseModel):
     """Response from an Aleph node API."""
 
     messages: List[AlephMessage]
     pagination_page: int
```

### Comparing `aleph-message-0.3.2/aleph_message/models/abstract.py` & `aleph-message-0.4.0a1/aleph_message/models/abstract.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.3.2/aleph_message/models/item_hash.py` & `aleph-message-0.4.0a1/aleph_message/models/item_hash.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 from enum import Enum
 from functools import lru_cache
 
-try:
-    from typing import Literal
-except ImportError:
-    from typing_extensions import Literal
-
 from ..exceptions import UnknownHashError
 
 
 class ItemType(str, Enum):
     """Item storage options"""
 
     inline = "inline"
```

### Comparing `aleph-message-0.3.2/aleph_message.egg-info/PKG-INFO` & `aleph-message-0.4.0a1/aleph_message.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: aleph-message
-Version: 0.3.2
+Version: 0.4.0a1
 Summary: Aleph.im message specification 
 Home-page: https://github.com/aleph-im/aleph-message
 Author: Hugo Herter
 Author-email: git@hugoherter.com
 License: MIT
 Keywords: aleph.im message validation specification
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Distributed Computing
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -39,21 +40,23 @@
 
 ```shell
 pip install aleph-message
 ```
 
 ```python
 import requests
-from aleph_message import Message
+from aleph_message import parse_message
 from pydantic import ValidationError
 
 ALEPH_API_SERVER = "https://official.aleph.cloud"
 MESSAGE_ITEM_HASH = "9b21eb870d01bf64d23e1d4475e342c8f958fcd544adc37db07d8281da070b00"
 
 message_dict = requests.get(ALEPH_API_SERVER + "/api/v0/messages.json?hashes=" + MESSAGE_ITEM_HASH).json()
 
 try:
-    message = Message(**message_dict["messages"][0])
+    message = parse_message(message_dict["messages"][0])
     print(message.sender)
 except ValidationError as e:
     print(e.json(indent=4))
 ```
+
+
```

### Comparing `aleph-message-0.3.2/setup.py` & `aleph-message-0.4.0a1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(name='aleph-message',
-      version='0.3.2',
+      version='0.4.0a1',
       description='Aleph.im message specification ',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Hugo Herter',
       author_email='git@hugoherter.com',
       url='https://github.com/aleph-im/aleph-message',
-      packages=['aleph_message', 'aleph_message.models'],
+      packages=['aleph_message', 'aleph_message.models', 'aleph_message.models.execution'],
       package_data={"aleph_message": ["py.typed"],
-                    "aleph_message.models": ["py.typed"]},
+                    "aleph_message.models": ["py.typed"],
+                    "aleph_message.models.execution": ["py.typed"]},
       data_files=[],
       install_requires=[
           'pydantic~=1.10.5',
           'typing_extensions~=4.5.0',
       ],
       license='MIT',
       platform='any',
```

