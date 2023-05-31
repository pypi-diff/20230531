# Comparing `tmp/SciDataContainer-0.5.3-py3-none-any.whl.zip` & `tmp/SciDataContainer-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,21 @@
-Zip file size: 12246 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat     3175 b- defN 23-Mar-24 14:06 scidatacontainer/__init__.py
--rw-rw-rw-  2.0 fat     2536 b- defN 23-Mar-08 22:02 scidatacontainer/config.py
--rw-rw-rw-  2.0 fat    21140 b- defN 23-Mar-24 14:05 scidatacontainer/container.py
--rw-rw-rw-  2.0 fat     3769 b- defN 23-Mar-09 14:17 scidatacontainer/filebase.py
--rw-rw-rw-  2.0 fat     1581 b- defN 23-Mar-09 14:17 scidatacontainer/fileimage.py
--rw-rw-rw-  2.0 fat     1744 b- defN 23-Mar-09 14:17 scidatacontainer/filenumpy.py
--rw-rw-rw-  2.0 fat     1279 b- defN 23-Mar-24 14:10 SciDataContainer-0.5.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-24 14:10 SciDataContainer-0.5.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Mar-24 14:10 SciDataContainer-0.5.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      846 b- defN 23-Mar-24 14:10 SciDataContainer-0.5.3.dist-info/RECORD
-10 files, 36179 bytes uncompressed, 10798 bytes compressed:  70.2%
+Zip file size: 23015 bytes, number of entries: 19
+-rw-rw-rw-  2.0 fat     3485 b- defN 23-May-31 07:39 scidatacontainer/__init__.py
+-rw-rw-rw-  2.0 fat     3243 b- defN 23-May-31 07:39 scidatacontainer/config.py
+-rw-rw-rw-  2.0 fat    24332 b- defN 23-May-31 19:32 scidatacontainer/container.py
+-rw-rw-rw-  2.0 fat     6353 b- defN 23-May-31 07:39 scidatacontainer/filebase.py
+-rw-rw-rw-  2.0 fat     1593 b- defN 23-May-31 07:39 scidatacontainer/fileimage.py
+-rw-rw-rw-  2.0 fat     1756 b- defN 23-May-31 07:39 scidatacontainer/filenumpy.py
+-rw-rw-rw-  2.0 fat     3027 b- defN 23-May-31 18:53 scidatacontainer/tests/__init__.py
+-rw-rw-rw-  2.0 fat     8751 b- defN 23-May-31 18:53 scidatacontainer/tests/_abstract_container_test.py
+-rw-rw-rw-  2.0 fat     1744 b- defN 23-May-31 07:39 scidatacontainer/tests/test_config.py
+-rw-rw-rw-  2.0 fat     2729 b- defN 23-May-31 07:39 scidatacontainer/tests/test_download.py
+-rw-rw-rw-  2.0 fat     3800 b- defN 23-May-31 19:11 scidatacontainer/tests/test_multistep_container.py
+-rw-rw-rw-  2.0 fat      430 b- defN 23-May-31 07:39 scidatacontainer/tests/test_register_class.py
+-rw-rw-rw-  2.0 fat     7549 b- defN 23-May-31 19:12 scidatacontainer/tests/test_single_step_container.py
+-rw-rw-rw-  2.0 fat     4641 b- defN 23-May-31 19:12 scidatacontainer/tests/test_static_container.py
+-rw-rw-rw-  2.0 fat     3322 b- defN 23-May-31 07:39 scidatacontainer/tests/test_upload.py
+-rw-rw-rw-  2.0 fat     1530 b- defN 23-May-31 19:34 SciDataContainer-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 19:34 SciDataContainer-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-31 19:34 SciDataContainer-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1749 b- defN 23-May-31 19:34 SciDataContainer-1.0.0.dist-info/RECORD
+19 files, 80143 bytes uncompressed, 20101 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -12,20 +12,47 @@
 
 Filename: scidatacontainer/fileimage.py
 Comment: 
 
 Filename: scidatacontainer/filenumpy.py
 Comment: 
 
-Filename: SciDataContainer-0.5.3.dist-info/METADATA
+Filename: scidatacontainer/tests/__init__.py
 Comment: 
 
-Filename: SciDataContainer-0.5.3.dist-info/WHEEL
+Filename: scidatacontainer/tests/_abstract_container_test.py
 Comment: 
 
-Filename: SciDataContainer-0.5.3.dist-info/top_level.txt
+Filename: scidatacontainer/tests/test_config.py
 Comment: 
 
-Filename: SciDataContainer-0.5.3.dist-info/RECORD
+Filename: scidatacontainer/tests/test_download.py
+Comment: 
+
+Filename: scidatacontainer/tests/test_multistep_container.py
+Comment: 
+
+Filename: scidatacontainer/tests/test_register_class.py
+Comment: 
+
+Filename: scidatacontainer/tests/test_single_step_container.py
+Comment: 
+
+Filename: scidatacontainer/tests/test_static_container.py
+Comment: 
+
+Filename: scidatacontainer/tests/test_upload.py
+Comment: 
+
+Filename: SciDataContainer-1.0.0.dist-info/METADATA
+Comment: 
+
+Filename: SciDataContainer-1.0.0.dist-info/WHEEL
+Comment: 
+
+Filename: SciDataContainer-1.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: SciDataContainer-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## scidatacontainer/__init__.py

```diff
@@ -19,28 +19,37 @@
 # Users may register other file extensions to file conversion classes
 # using the function register(). See package fileimage as an example for
 # such a conversion class.
 #
 ##########################################################################
 
 from importlib import import_module
-from .filebase import FileBase
-from .container import DataContainer, timestamp
+import typing
+from .filebase import AbstractFile
+from .container import AbstractContainer, timestamp
 from .container import MODELVERSION as modelVersion
 
 suffixes = {}
 classes = {}
 formats = []
 
 
-def register(suffix, fclass, pclass=None):
-
-    """ Register a suffix to a conversion class. If the parameter class
-    is a string, it is interpreted as known suffix and the conversion
-    class of this suffix is registered also for the new one. """
+def register(suffix: str,
+             fclass: typing.Type[AbstractFile],
+             pclass: typing.Type[object] = None):
+    """ Register a suffix to a conversion class.
+
+    If the parameter class is a string, it is interpreted as known suffix and
+    the conversion class of this suffix is registered also for the new one.
+
+    Args:
+        suffix: file suffix to identify this file type.
+        fclass: Conversion class derived from AbstractFile.
+        pclass: Python class that represents this object type.
+    """
 
     if isinstance(fclass, str):
         if not pclass is None:
             raise RuntimeError("Alias %s:%s with default class!" % (suffix, fclass))
         fclass = suffixes[fclass]
 
     # Simple sanity check for the class interface
@@ -73,14 +82,14 @@
         continue
     #print("%s imported" % fullname)
     for suffix, fclass, pclass in module.register:
         register(suffix, fclass, pclass)
 
     
 # Inject certain known file formats into the container class
-class Container(DataContainer):
+class Container(AbstractContainer):
 
     """ Scientific data container. """
 
     _suffixes = suffixes
     _classes = classes
     _formats = formats
```

## scidatacontainer/config.py

```diff
@@ -29,41 +29,56 @@
 #
 ##########################################################################
 
 import os
 import platform
 
 
-def load_config():
+def load_config(config_path: str = None) -> dict:
+    """Get config data from environment variables and config file.
 
-    """ Get config data from environment variables and config file. """
+    This functions prefers values in the scidata config file and potentially
+    overwrites values that are present as environmental variables.
+
+    Usually, users doen't need to call this function. However, it can be used
+    for debugging purposes if the configuration parameters are not as expected.
+
+    Args:
+        str: Path of the config file. If this is None, the default file will
+             be used. This filename is only required for testing.
+
+    Returns:
+        dict: A dictionary containing information strings with keys "author",\
+              "email", "server", "key".
+    """
 
     # Initialize config dictionary
     config = {"author": "", "email": "", "server": "", "key": ""}
 
     # Get default values from environment variables
     for key in config:
         name = "DC_%s" % key.upper()
         if name in os.environ:
             config[key] = os.environ[name]
             
     # Get default values from config file
-    if platform.system() == "Windows":
-        conf = os.path.join(os.path.expanduser("~"), "scidata.cfg")
-    else:
-        conf = os.path.join(os.path.expanduser("~"), ".scidata")
-    if os.path.exists(conf):
-        with open(conf, "r") as fp:
+    if not config_path:
+        if platform.system() == "Windows":
+            config_path = os.path.join(os.path.expanduser("~"), "scidata.cfg")
+        else:
+            config_path = os.path.join(os.path.expanduser("~"), ".scidata")
+
+    if os.path.exists(config_path):
+        with open(config_path, "r") as fp:
             for line in fp.readlines():
                 line = line.strip()
                 if line[:1] == "#":
                     continue
                 line = line.split("=", 1)
                 if len(line) < 2:
                     continue
                 key = line[0].strip().lower()
                 if key in config:
                     config[key] = line[1].strip()
 
     # Return config dictionary
     return config
-
```

## scidatacontainer/container.py

```diff
@@ -7,56 +7,89 @@
 # This module provides the Scientific Data Container as class
 # DataContainer which may be stored or uploaded as a ZIP package
 # containing items (files). Do not use this class directly! Use the
 # class Container provided by the package scidatacontainer instead.
 #
 ##########################################################################
 
+from abc import ABC
 import copy
+from datetime import datetime, timezone
 import hashlib
 import io
 import json
 import requests
-import time
+import typing 
 import uuid
-from zipfile import ZipFile
+from zipfile import ZipFile, ZIP_DEFLATED
 
-from .filebase import FileBase, TextFile, JsonFile
+
+from .filebase import BinaryFile, TextFile, JsonFile
 from .config import load_config
 config = load_config()
 
 # Version of the implemented data model
-MODELVERSION = "0.6"
+MODELVERSION = "1.0"
 
 
 ##########################################################################
 # Timestamp function
 
-def timestamp():
-
-    """ Return the current ISO 8601 compatible timestamp string. """
+def timestamp() -> str:
+    """Return the current ISO 8601 compatible timestamp as string. 
 
-    return time.strftime("%Y-%m-%dT%H:%M:%S%z", time.gmtime(time.time()))
+    Returns:
+        str: timestamp as string
+    """
+    return datetime.now(timezone.utc).isoformat(timespec='seconds')
 
 
 ##########################################################################
 # Data container class
 
-class DataContainer(object):
+class AbstractContainer(ABC):
+    """Scientific data container with minimal file support.
 
-    """ Scientific data container with minimal file support. """
+    The following file types are supported:
+        - .json <-> dict
+        - .txt <-> str
+        - .bin <-> bytes
+    """
 
     _config = config
-    _suffixes = {"json": JsonFile, "txt": TextFile, "bin": FileBase}
-    _classes = {dict: JsonFile, str: TextFile, bytes: FileBase}
+    _suffixes = {"json": JsonFile, "txt": TextFile, "bin": BinaryFile}
+    _classes = {dict: JsonFile, str: TextFile, bytes: BinaryFile}
     _formats = [TextFile]
 
 
-    def __init__(self, items=None, file=None, uuid=None, server=None, key=None):
-
+    def __init__(self,
+                 items: dict = None,
+                 file: str = None,
+                 uuid: str = None,
+                 server: str = None,
+                 key: str = None,
+                 compression: int = ZIP_DEFLATED,
+                 compresslevel: int = -1):
+        """Constructor of a DataContainer object.
+
+        It will try the following in the specified order:
+            - Create a new DataContainer if items is passed as argument.
+            - Load local DataContainer from hard drive if file is passed.
+            - Download a DataContainer from a server if uuid is passed.
+
+        Args:
+            items: Dictionary of items to build a new DataContainer.
+            file: Filename to read a DataContainer from local hard drive.
+            uuid: UUID of a Container to download from a server instance.
+            server: URL of the server instance that has the Container.
+            key: API-Key from the server to identify yourself.
+            compression: Numeric constant for the compression method
+            compresslevel: Level of compression, 0-fastest, 9-best compression
+        """
+            
         # Container must be mutable initially
         self.mutable = True
 
         # Store all items in the container
         if items is not None:
             self._store(items, True, False)
             self.mutable = not self["content.json"]["static"]
@@ -64,19 +97,22 @@
         # Load local container file
         elif file is not None:
             self._read(fn=file)
 
         # Download container from server
         elif uuid is not None:
             self._download(uuid=uuid, server=server, key=key)
-
+        
         # No data source
         else:
             raise RuntimeError("No data!")
 
+        self.compression = compression
+        self.compresslevel = compresslevel
+
 
     def _store(self, items, validate=True, strict=True):
 
         """ Store all items in the container. """
 
         # Add all items in the container
         self._items = {}
@@ -91,14 +127,17 @@
             raise RuntimeError("Item 'content.json' is missing!")
         if "meta.json" not in self:
             raise RuntimeError("Item 'meta.json' is missing!")
         if validate:
             self.validate_content()
             self.validate_meta()
 
+        if self["content.json"]["static"] and not self["content.json"]["hash"]:
+            self.hash()
+
         # Check validity of hash
         if strict and self["content.json"]["hash"]:
             oldhash = self["content.json"]["hash"]
             self.hash()
             if self["content.json"]["hash"] != oldhash:
                 raise RuntimeError("Wrong hash!")
 
@@ -124,24 +163,24 @@
         
         # Get file extension
         ext = path.rsplit(".", 1)[1]
 
         # Unregistered file extension
         if not ext in self._suffixes:
 
-            # Try to convert bytes. Default is FileBase.
+            # Try to convert bytes. Default is BinaryFile.
             if isinstance(data, bytes):
                 for cls in self._formats:
                     try:
                         item = cls(data)
                         break
                     except:
                         pass
                 else:
-                    item = FileBase(data)
+                    item = BinaryFile(data)
 
             # Other Python object must be registered
             else:
                 if type(data) in self._classes:
                     cls = self._classes[type(data)]
                     item = cls(data)
                 else:
@@ -163,17 +202,17 @@
 
         if path in self:
             return self._items[path].data
         raise KeyError("Unknown item '%s'!" % path)
 
 
     def validate_content(self):
-
-        """ Make sure that the item "content.json" exists and contains
-        all required attributes. """
+        """Make sure that the item "content.json" exists and contains
+        all required attributes.
+        """
 
         # Get a copy of the item "content.json"
         content = copy.deepcopy(self["content.json"])
 
         # Keep UUID of a multi-step container and create a new one otherwise
         if "uuid" not in content or not content["uuid"]:
             content["uuid"] = str(uuid.uuid4())
@@ -218,18 +257,18 @@
         ts = timestamp()
 
         # The attribute 'created' is required. It is created
         # automatically for a new dataset.
         if "created" not in content or not content["created"]:
             content["created"] = ts
 
-        # The attribute 'modified' is updated automatically for a
-        # multi-step dataset
-        if "modified" not in content or not content["complete"]:
-            content["modified"] = ts
+        # The attribute 'storageTime' is updated automatically when the
+        # container is stored
+        if "storageTime" not in content or not content["complete"]:
+            content["storageTime"] = ts
 
         # The attribute 'hash' is optional
         if "hash" not in content or not content["hash"]:
             content["hash"] = None
 
         # The attribute 'usedSoftware' is a list of dictionaries, which
         # may be empty. Each dictionary must contain atleast the items
@@ -250,17 +289,17 @@
         content["modelVersion"] = MODELVERSION
 
         # Store the item "content.json"
         self["content.json"] = content
         
 
     def validate_meta(self):
-        
-        """ Make sure that the item "meta.json" exists and contains
-        all required attributes. """
+        """Make sure that the item "meta.json" exists and contains
+        all required attributes.
+        """
 
         # Get a copy of the item "meta.json"
         meta = copy.deepcopy(self["meta.json"])
 
         # Author name is required
         if "author" not in meta:
             meta["author"] = self._config["author"]
@@ -318,42 +357,49 @@
             raise RuntimeError("Immutable container!")
 
         # Delete item        
         if path in self:
             del self._items[path]
             
 
-    def keys(self):
+    def keys(self) -> typing.List[str]:
+        """Return a sorted list of the full paths of all items.
 
-        """ Return a sorted list of the full paths of all items. """
+        Returns:
+            typing.List[str]: List of paths of Container items.
+        """
 
         return sorted(self._items.keys())
 
 
-    def values(self):
+    def values(self) ->typing.List:
+        """Return a list of all item objects.
 
-        """ Return a list of all item objects. """
+        Returns:
+            typing.List: List of item objects of the Container.
+        """
 
         return [self[k] for k in self.keys()]
 
 
     def items(self):
-
-        """ Return this container as a dictionary of item objects. """
+        """Return this container as a dictionary of item objects (key, value)
+        tuples.
+        """
 
         return {k: self[k] for k in self.keys()}
 
 
     def hash(self):
-
-        """ Calculate hash value of this container. """
+        """Calculate and save the hash value of this container.
+        """
 
         # Some attributes of content.json are excluded from the hash
         # calculation
-        save = ("uuid", "created", "modified")
+        save = ("uuid", "created", "storageTime")
         save = {k: self["content.json"][k] for k in save}
         for key in save:
             self["content.json"][key] = None
         self["content.json"]["hash"] = None
 
         # Calculate and store hash of this container
         hashes = [self._items[p].hash() for p in sorted(self.items())]
@@ -362,100 +408,129 @@
 
         # Restore excluded attributes
         for key, value in save.items():
             self["content.json"][key] = value
 
         # Make container immutable
         self.mutable = False
+        self["content.json"]["storageTime"] = timestamp()
 
 
     def freeze(self):
-
-        """ Calculate the hash value of this container and make it
+        """Calculate the hash value of this container and make it
         static. The container cannot be modified any more when this
         method was called once. """
 
         self["content.json"]["static"] = True
         self["content.json"]["complete"] = True
         self.hash()
 
 
     def release(self):
-
-        """ Make this container mutable. If it was immutable, this
-        method will create a new UUID and initialize the attributes
-        replaces, created, modified and modelVersion in the item
-        "content.json". It will also delete an existing hash and make it
-        a single-step container. """
+        """Make this container mutable. If it was immutable, this method
+        will create a new UUID and initialize the attributes replaces,
+        createdstorageTime and modelVersion in the item "content.json".
+        It will also delete an existing hash and make it a new
+        container. """
 
         # Do nothing if the container is already mutable
         if self.mutable:
             return
         self.mutable = True
         
         # Remove and initialize certain container attributes
         content = self["content.json"]
         content["static"] = False
         content["complete"] = True
-        for key in ("uuid", "replaces", "created", "modified", "hash"):
+        for key in ("uuid", "replaces", "created", "storageTime", "hash"):
             content.pop(key, None)
         self.validate_content()
         
 
     def encode(self):
-
         """ Encode container as ZIP package. Return package as binary
-        string. """
+        string.
+        """
 
         items = {p: self._items[p].encode() for p in self.items()}
         with io.BytesIO() as f:
-            with ZipFile(f, "w") as fp:
+            with ZipFile(f, "w",
+                         compression=self.compression,
+                         compresslevel=self.compresslevel) as fp:
                 for path in sorted(items.keys()):
                     fp.writestr(path, items[path])
             f.seek(0)
             data = f.read()
         return data
     
 
-    def decode(self, data, validate=True, strict=True):
-
-        """ Take ZIP package as binary string. Read items from the
-        package and store them in this object. """
+    def decode(self, data:bytes, validate: bool = True, strict: bool = True):
+        """Take ZIP package as binary string. Read items from the
+        package and store them in this object.
+
+        Arguments:
+            data: Bytestring containing the ZIP DataContainer.
+            validate: If true, validate the content.
+            strict: If true, validate the hash, too.
+        """
         
         with io.BytesIO() as f:
             f.write(data)
             f.seek(0)
             with ZipFile(f, "r") as fp:
                 items = {p: fp.read(p) for p in fp.namelist()}
         self._store(items, validate, strict)
 
         
-    def write(self, fn, data=None):
+    def write(self, fn: str, data:bytes = None):
+        """Write the container to a ZIP package file.
 
-        """ Write the container to a ZIP package file. """
+        If data is passed to the function, data will be written to the file.
+        Otherwise the byte representation of the class instance will be written
+        to the file, which is what you typically want.
+
+        Args:
+            fn: Filename of export file.
+            data: If given, data to write to the file.
+        """
 
+        if self.mutable:
+            self["content.json"]["storageTime"] = timestamp()
         if data is None:
             data = self.encode()
         with open(fn, "wb") as fp:
             fp.write(data)
         self.mutable = not (self["content.json"]["static"] or self["content.json"]["complete"])
 
 
     def _read(self, fn, strict=True):
-
-        """ Read a ZIP package file and store it as container in this
-        object. """
+        """Read a ZIP package file and store it as container in this
+        object.
+        """
 
         with open(fn, "rb") as fp:
             data = fp.read()
         self.decode(data, False, strict)
         self.mutable = not (self["content.json"]["static"] or self["content.json"]["complete"])
 
-
-    def upload(self, data=None, strict=True, server=None, key=None):
+    def upload(self,
+               data: bytes = None,
+               server: str = None,
+               key: str = None):
+        """Create a ZIP archive of the DataContainer and upload it to a server.
+
+        If data is passed to the function, data will be written to the file.
+        Otherwise the byte representation of the class instance will be written
+        to the file, which is what you typically want.
+        
+        Args:
+            data: If given, data to write to the file.
+            server: URL of the server.
+            key: API Key from the server to identify yourself.
+        """
 
         # Server name is required and must be provided either via config
         # file, environment variable or method parameter
         if server is None:
             server = self._config["server"]
         if not server:
             raise RuntimeError("Server URL is missing!")
@@ -464,14 +539,16 @@
         # file, environment variable or method parameter
         if key is None:
             key = self._config["key"]
         if not key:
             raise RuntimeError("Server API key is missing!")
 
         # Upload container as byte string
+        if self.mutable:
+            self["content.json"]["storageTime"] = timestamp()
         if data is None:
             data = self.encode()
         try:
             response = requests.post(server + "/api/datasets/",
                                      files={"uploadfile": data},
                                      headers={"Authorization": "Token " + key})
         except:
@@ -577,31 +654,27 @@
 
         content = self["content.json"]
         meta = self["meta.json"]
 
         if content["static"]:
             ctype = "Static Container"
         elif content["complete"]:
-            if content["created"] == content["modified"]:
-                ctype = "Single-Step Container"
-            else:
-                ctype = "Closed Multi-Step Container"
+            ctype = "Complete Container"
         else:
-            ctype = "Open Multi-Step Container"
+            ctype = "Incomplete Container"
 
         s = [ctype]
         ptype = content["containerType"]
         name = ptype["name"]
         if "id" in ptype:
             name = "%s %s (%s)" % (name, ptype["version"], ptype["id"])
-        s.append("  type:     " + name)
-        s.append("  uuid:     " + content["uuid"])
+        s.append("  type:        " + name)
+        s.append("  uuid:        " + content["uuid"])
         if content["replaces"]:
-            s.append("  replaces: " + content["replaces"])
+            s.append("  replaces:    " + content["replaces"])
         if content["hash"]:
-            s.append("  hash:     " + content["hash"])
-        s.append("  created:  " + content["created"])
-        if "Multi" in ctype:
-            s.append("  modified: " + content["modified"])
-        s.append("  author:   " + meta["author"])
+            s.append("  hash:        " + content["hash"])
+        s.append("  created:     " + content["created"])
+        s.append("  storageTime: " + content["storageTime"])
+        s.append("  author:      " + meta["author"])
 
         return "\n".join(s)
```

## scidatacontainer/filebase.py

```diff
@@ -1,135 +1,203 @@
 ##########################################################################
 # Copyright (c) 2023 Reinhard Caspary                                    #
 # <reinhard.caspary@phoenixd.uni-hannover.de>                            #
 # This program is free software under the terms of the MIT license.      #
 ##########################################################################
 #
-# This module provides the base data conversion class FileBase and
+# This module provides the base data conversion class AbstractFile and
 # standard text conversion classes. All data conversion classes should
-# inherit from FileBase and must provide three methods:
+# inherit from AbstractFile and must provide three methods:
 #
 # encode(): Return data encoded as bytes string.
 # decode(data): Decode and store given bytes string data.
 # hash(): Return SHA256 hash from data as hex string.
 #
 # The hash implementation shoud make sure that semantically equivalent
 # data results in the same hash.
 #
 ##########################################################################
 
+from abc import ABC, abstractmethod
 import hashlib
 import json
+import typing
 
 
 ##########################################################################
 # Data conversion classes
 
-class FileBase(object):
-
-    """ Basic class for bytes data. """
+class AbstractFile(ABC):
+    """Base class for converting datatypes to their file representation."""
 
     def __init__(self, data):
-
-        """ Store data. """
-
+        """Constructor to create an instance of the converter class. """
         if isinstance(data, bytes):
             self.decode(data)
         else:
             self.data = data
 
-    def hash(self):
-
-        """ Return hex digest of SHA256 hash. """
-
+    def hash(self) -> str:
+        """Return hex digest of SHA256 hash.
+        
+        Returns:
+            str: Hex digest of this object as string.
+        """
         return hashlib.sha256(self.encode()).hexdigest()
 
-    def encode(self):
-
-        """ Return encoded data as bytes string. """
-
+    @abstractmethod
+    def encode(self) -> bytes:
+        """Encode the Container content to bytes. This is an abstract method
+        and it needs to be overwritten by inheriting class.
+
+        Returns:
+            bytes: Byte string representation of the object.
+        """
+        pass
+
+    @abstractmethod
+    def decode(self, data: bytes):
+        """Decode the Container content from bytes. This is an abstract method
+        and it neets to be overwritten by inheriting class.
+        """
+        pass
+
+
+class BinaryFile(AbstractFile):
+    """Data conversion class for a binary file."""
+
+    def encode(self) -> bytes:
+        """Return byte string stored in this class.
+
+        Returns:
+            bytes: Byte string representation of the object.
+        """
         return self.data
 
-    def decode(self, data):
-
-        """ Decode and store data from bytes string. """
-
+    def decode(self, data: bytes):
+        """Store bytes in this class."""
         self.data = data
 
 
-class TextFile(FileBase):
-
-    """ Data conversion class for a text file. """
-
+class TextFile(AbstractFile):
+    """ Data conversion class for a text file.
+    """
     charset = "utf8"
+    """charset (str): Character encoding used for translation from text to\
+                      bytes."""
 
-    def encode(self):
+    def encode(self) -> bytes:
+        """ Encode text to bytes string.
 
-        """ Encode text to bytes string. """
+        Returns:
+            bytes: Byte string representation of the object.
+        """
 
         return bytes(self.data, self.charset)
 
-    def decode(self, data):
 
+    def decode(self, data: bytes):
         """ Decode text from given bytes string. """
 
         self.data = data.decode(self.charset)
         
 
-class JsonFile(FileBase):
+class JsonFile(AbstractFile):
 
     """ Data conversion class for a JSON file represented as Python
     dictionary. """
 
     indent = 4
+    """indent (int): Indentation of exported JSON files."""
     charset = "utf8"
+    """charset (str): Character encoding used for translation from text to\
+                      bytes."""
 
-    def sortit(self, data):
-
+    def sortit(self, data: typing.Union[dict, list, tuple]) -> str:
         """ Return compact string representation with keys of all
-        sub-dictionaries sorted. """
+        sub-dictionaries sorted.
+
+        Args:
+            data: Dictionary, list or tuple to convert to string"
+
+        Returns:
+            str: String representation of `data`
+        """
 
         if isinstance(data, dict):
             keys = sorted(data.keys())
             data = [k + ": " + self.sortit(data[k]) for k in keys]
             data = ", ".join(data)
             data = "{" + data + "}"
             return data
         elif isinstance(data, (list, tuple)):
             data = [self.sortit(v) for v in data]
             data = ", ".join(data)
             data = "[" + data + "]"
             return data
         return repr(data)
 
-    def hash(self):
-
-        """ Return hex digest of the SHA256 hash calculated from the
+    def hash(self) -> str:
+        """Return hex digest of the SHA256 hash calculated from the
         sorted compact representation. This should result in the same
-        hash for semantically equal data dictionaries. """
+        hash for semantically equal data dictionaries.
+
+        Returns:
+            str: Hex digest of this object as string.
+        """
 
         data = bytes(self.sortit(self.data), self.charset)
         return hashlib.sha256(data).hexdigest()
 
-    def encode(self):
-
-        """ Convert dictionary to pretty string representation with
-        indentation and return it as bytes string. """
+    def encode(self) -> bytes:
+        """Convert dictionary to pretty string representation with
+        indentation and return it as bytes string.
+
+        Returns:
+            bytes: Byte string representation of the object.
+        """
 
         data = json.dumps(self.data, sort_keys=True, indent=self.indent)
         return bytes(data, self.charset)
 
-    def decode(self, data):
+    def decode(self, data: bytes):
 
         """ Decode dictionary from given bytes string. """
 
         self.data = json.loads(data.decode(self.charset))
 
 
+class TabSeparatedValuesFile(AbstractFile):
+    """ Data conversion class for a tab-separated value file.
+    """
+    charset = "utf8"
+    """charset (str): Character encoding used for translation from a list of\
+                      lists to bytes."""
+
+    def encode(self) -> bytes:
+        """ Encode 2D array (list of lists) to bytes string.
+
+        Returns:
+            bytes: Byte string representation of the object.
+        """
+        s = '\n'.join(['\t'.join([str(v) for v in l]) for l in self.data])
+
+        return bytes(s, self.charset)
+
+    def decode(self, data: bytes):
+        """Decode 2D array (list of lists) from given bytes string.
+
+        """
+
+        s = data.decode(self.charset)
+        self.data = [[float(x) for x in l.split('\t')] for l in s.split('\n')]
+
+
 register = [
-    ("bin", FileBase, bytes),
+    ("bin", BinaryFile, bytes),
     ("json", JsonFile, dict),
     ("txt", TextFile, str),
     ("log", TextFile, None),
     ("pgm", "txt", None),
+    ("tsv", TabSeparatedValuesFile, None),
     ]
```

## scidatacontainer/fileimage.py

```diff
@@ -1,33 +1,33 @@
 ##########################################################################
 # Copyright (c) 2023 Reinhard Caspary                                    #
 # <reinhard.caspary@phoenixd.uni-hannover.de>                            #
 # This program is free software under the terms of the MIT license.      #
 ##########################################################################
 #
 # This module provides data conversion classes for image files. All
-# data conversion classes should inherit from filebase.FileBase and must
+# data conversion classes should inherit from filebase.AbstractFile and must
 # provide three methods:
 #
 # encode(): Return data encoded as bytes string.
 # decode(data): Decode and store given bytes string data.
 # hash(): Return SHA256 hash from data as hex string.
 #
 # The hash implementation shoud make sure that semantically equivalent
 # data results in the same hash.
 #
 ##########################################################################
 
 import cv2 as cv
 import numpy as np
 
-from .filebase import FileBase
+from .filebase import AbstractFile
 
 
-class PngFile(FileBase):
+class PngFile(AbstractFile):
 
     """ Data conversion class for PNG image. """
 
     def encode(self):
 
         """ Convert image to bytes string. """
```

## scidatacontainer/filenumpy.py

```diff
@@ -1,32 +1,32 @@
 ##########################################################################
 # Copyright (c) 2023 Reinhard Caspary                                    #
 # <reinhard.caspary@phoenixd.uni-hannover.de>                            #
 # This program is free software under the terms of the MIT license.      #
 ##########################################################################
 #
 # This module provides data conversion classes for image files. All
-# data conversion classes should inherit from filebase.FileBase and must
+# data conversion classes should inherit from filebase.AbstractFile and must
 # provide three methods:
 #
 # encode(): Return data encoded as bytes string.
 # decode(data): Decode and store given bytes string data.
 # hash(): Return SHA256 hash from data as hex string.
 #
 # The hash implementation shoud make sure that semantically equivalent
 # data results in the same hash.
 #
 ##########################################################################
 
 import numpy as np
 
-from .filebase import FileBase
+from .filebase import AbstractFile
 
 
-class NpyFile(FileBase):
+class NpyFile(AbstractFile):
 
     """ Data conversion class for NumPy arrays (ndarray). """
 
     allow_pickle = False
 
     def encode(self):
```

## Comparing `SciDataContainer-0.5.3.dist-info/METADATA` & `SciDataContainer-1.0.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciDataContainer
-Version: 0.5.3
+Version: 1.0.0
 Summary: A container class for the storage of scientific data together with meta data
 Home-page: https://github.com/reincas/scidatacontainer
 Author: Reinhard Caspary
 Author-email: reinhard.caspary@phoenixd.uni-hannover.de
 License: MIT License
 Keywords: Research Data Management,Data Container,Meta Data
 Classifier: Programming Language :: Python :: 3
@@ -25,7 +25,19 @@
 
 ## Installation
 
 The easiest way to install the latest version of [`SciDataContainer`](https://pypi.org/project/scidatacontainer/) is using PIP:
 ```
 >>> pip install SciDataContainer
 ```
+
+## Tests
+
+The tests require the [`coverage`](https://pypi.org/project/coverage/) python package. Run:
+```
+>>> make report
+```
+to get a command line coverage report. It's also possible to create a HTML report:
+```
+>>> make htmlreport
+```
+
```

