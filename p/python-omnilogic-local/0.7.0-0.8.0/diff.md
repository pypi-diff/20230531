# Comparing `tmp/python_omnilogic_local-0.7.0.tar.gz` & `tmp/python_omnilogic_local-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.7.0.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.8.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.7.0.tar` & `python_omnilogic_local-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1696 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/__init__.py
--rw-r--r--   0        0        0    21453 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3921 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0      164 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     8413 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9968 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-31 03:23:18.064843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0    10185 2023-05-31 03:23:18.064843 python_omnilogic_local-0.7.0/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6325 2023-05-31 03:23:18.064843 python_omnilogic_local-0.7.0/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-31 03:23:18.064843 python_omnilogic_local-0.7.0/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-31 03:23:18.980826 python_omnilogic_local-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-31 19:02:53.205971 python_omnilogic_local-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/__init__.py
+-rw-r--r--   0        0        0    21453 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3921 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0      164 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     8385 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9968 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0    10194 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6338 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-31 19:02:53.209971 python_omnilogic_local-0.8.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5297 2023-05-31 19:02:54.366016 python_omnilogic_local-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2682 1970-01-01 00:00:00.000000 python_omnilogic_local-0.8.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.7.0/README.md` & `python_omnilogic_local-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.7.0/pyomnilogic_local/api.py` & `python_omnilogic_local-0.8.0/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.7.0/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.8.0/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.7.0/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.8.0/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.7.0/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.8.0/pyomnilogic_local/models/mspconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,17 @@
             subdevice = getattr(self, subdevice_name)
             # If our subdevice is a list of subdevices ...
             if isinstance(subdevice, list):
                 for device in subdevice:
                     # ... then call propagate_bow_id on each of them ...
                     if device is not None:
                         device.propagate_bow_id(bow_id)
-            else:
-                # ... otherwise just call it on the single subdevice
-                if subdevice is not None:
-                    subdevice.propagate_bow_id(bow_id)
+            # ... otherwise just call it on the single subdevice
+            elif subdevice is not None:
+                subdevice.propagate_bow_id(bow_id)
 
 
 class MSPSystem(BaseModel):
     omni_type: OmniType = OmniType.SYSTEM
     vsp_speed_format: Literal["RPM", "Percent"] = Field(alias="Msp-Vsp-Speed-Format")
     units: Literal["Standard", "Metric"] = Field(alias="Units")
```

### Comparing `python_omnilogic_local-0.7.0/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.8.0/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.7.0/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.8.0/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.7.0/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.8.0/pyomnilogic_local/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 class OmniLogicMessage:
     header_format = "!LQ4sLBBBB"
     id: int
     type: MessageType
     payload: bytes
     client_type: ClientType = ClientType.SIMPLE
     version: str = "1.19"
-    timestamp: int | None
+    timestamp: int | None = int(time.time())
     reserved_1: int = 0
-    compressed: int = 0
+    compressed: bool = False
     reserved_2: int = 0
 
     def __init__(self, msg_id: int, msg_type: MessageType, payload: str | None = None, version: str = "1.19") -> None:
         self.id = msg_id
         self.type = msg_type
         # If we are speaking the XML API, it seems like we need client_type 0, otherwise we need client_type 1
         self.client_type = ClientType.XML if payload is not None else ClientType.SIMPLE
@@ -39,39 +39,42 @@
 
         self.version = version
 
     def __bytes__(self) -> bytes:
         header = struct.pack(
             self.header_format,
             self.id,  # Msg id
-            int(time.time_ns() / (10**9)),  # Timestamp
+            self.timestamp,
             bytes(self.version, "ascii"),  # version string
             self.type.value,  # OpID/msgType
             self.client_type.value,  # Client type
             0,  # reserved
-            0,  # compressed
+            self.compressed,  # compressed
             0,  # reserved
         )
         return header + self.payload
 
     def __repr__(self) -> str:
         if self.compressed or self.type is MessageType.MSP_BLOCKMESSAGE:
-            return f"ID: {self.id}, Type: {self.type.name}, Compressed: {self.compressed}"
-        return f"ID: {self.id}, Type: {self.type.name}, Compressed: {self.compressed}, Body: {self.payload[:-1].decode('utf-8')}"
+            return f"ID: {self.id}, Type: {self.type.name}, Compressed: {self.compressed}, Client: {self.client_type.name}"
+        return (
+            f"ID: {self.id}, Type: {self.type.name}, Compressed: {self.compressed}, Client: {self.client_type.name}, "
+            f"Body: {self.payload[:-1].decode('utf-8')}"
+        )
 
     @classmethod
     def from_bytes(cls, data: bytes) -> Self:
         # split the header and data
-        header = data[0:24]
+        header = data[:24]
         rdata: bytes = data[24:]
 
         msg_id, tstamp, vers, msg_type, client_type, res1, compressed, res2 = struct.unpack(cls.header_format, header)
-        message = cls(msg_id=msg_id, msg_type=MessageType(msg_type), version=vers)
+        message = cls(msg_id=msg_id, msg_type=MessageType(msg_type), version=vers.decode("utf-8"))
         message.timestamp = tstamp
-        message.client_type = client_type
+        message.client_type = ClientType(int(client_type))
         message.reserved_1 = res1
         # There are some messages that are ALWAYS compressed although they do not return a 1 in their LeadMessage
         message.compressed = compressed == 1 or message.type in [MessageType.MSP_TELEMETRY_UPDATE]
         message.reserved_2 = res2
         message.payload = rdata
 
         return message
@@ -172,15 +175,15 @@
         # self._ensure_sent, but if any subsequent ACKs are sent to us, we need to dump them and wait for a "real" message.
         while message.type in [MessageType.ACK, MessageType.XML_ACK]:
             message = await self.data_queue.get()
 
         await self._send_ack(message.id)
 
         # If the response is too large, the controller will send a LeadMessage indicating how many follow-up messages will be sent
-        if message.type == MessageType.MSP_LEADMESSAGE:
+        if message.type is MessageType.MSP_LEADMESSAGE:
             leadmsg = LeadMessage.from_orm(ET.fromstring(message.payload[:-1]))
 
             _LOGGER.debug("Will receive %s blockmessages", leadmsg.msg_block_count)
 
             # Wait for the block data data
             retval: bytes = b""
             # If we received a LeadMessage, continue to receive messages until we have all of our data
@@ -203,18 +206,15 @@
                 # remove an 8 byte header to get to the payload data
                 data_fragments[resp.id] = resp.payload[8:]
 
             # Reassemble the fragmets in order
             for _, data in sorted(data_fragments.items()):
                 retval += data
 
-        # If we did not receive a LeadMessage, but the message is compressed anyway...
-        elif message.compressed:
-            retval = message.payload
-        # A short response, no LeadMessage and no compression...
+        # We did not receive a LeadMessage, so our payload is just this one packet
         else:
             retval = message.payload
 
         # Decompress the returned data if necessary
         if message.compressed:
             comp_bytes = bytes.fromhex(retval.hex())
             retval = zlib.decompress(comp_bytes)
```

### Comparing `python_omnilogic_local-0.7.0/pyomnilogic_local/types.py` & `python_omnilogic_local-0.8.0/pyomnilogic_local/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     MSP_LEADMESSAGE = 1998
     MSP_BLOCKMESSAGE = 1999
 
 
 class ClientType(Enum):
     XML = 0
     SIMPLE = 1
+    OMNI = 3
 
 
 class OmniType(str, Enum):
     BACKYARD = "Backyard"
     BOW = "BodyOfWater"
     BOW_MSP = "Body-of-water"
     CHLORINATOR = "Chlorinator"
```

### Comparing `python_omnilogic_local-0.7.0/pyproject.toml` & `python_omnilogic_local-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.7.0"
+version = "0.8.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -17,23 +17,28 @@
 
 [tool.poetry.scripts]
 omnilogic = "pyomnilogic_local.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.7"
-pydantic-xml = "^0.6.1"
 xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.0"
 mypy = "^1.2.0"
 pylint = "^2.17.0"
 pydantic = "^1.10.7"
 pytest = "^7.3.1"
+pytest-cov = "^4.1.0"
+
+[tool.pytest.ini_options]
+addopts = [
+    "--import-mode=importlib",
+]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length=140
```

### Comparing `python_omnilogic_local-0.7.0/PKG-INFO` & `python_omnilogic_local-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.7.0
+Version: 0.8.0
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,14 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pydantic-xml (>=0.6.1,<0.7.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/cryptk/python-omnilogic-local
 Description-Content-Type: text/markdown
 
 # Pyomnilogic Local
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.7.0 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.8.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries Requires-Dist: pydantic
-(>=1.10.7,<2.0.0) Requires-Dist: pydantic-xml (>=0.6.1,<0.7.0) Requires-Dist:
-xmltodict (>=0.13.0,<0.14.0) Project-URL: Repository, https://github.com/
-cryptk/python-omnilogic-local Description-Content-Type: text/markdown #
-Pyomnilogic Local
+(>=1.10.7,<2.0.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL:
+Repository, https://github.com/cryptk/python-omnilogic-local Description-
+Content-Type: text/markdown # Pyomnilogic Local
              [PyPI_Version] [Supported Python versions] [License]
 A library implementing the UDP XML Local Control api for Hayward OmniLogic and
 OmniHub pool controllers ## Installation This package is published to pypi at
 https://pypi.org/project/python-omnilogic-local/: `pip install python-
 omnilogic-local` ## Functionality This library is still under development and
 is not yet able to control every function of a Hayward pool controller. The
 implemented functionality is: - Pulling the MSP Config - Polling telemetry -
```

