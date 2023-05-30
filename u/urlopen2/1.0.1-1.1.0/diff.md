# Comparing `tmp/urlopen2-1.0.1.tar.gz` & `tmp/urlopen2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlopen2-1.0.1.tar", max compression
+gzip compressed data, was "urlopen2-1.1.0.tar", max compression
```

## Comparing `urlopen2-1.0.1.tar` & `urlopen2-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2023-05-29 07:15:28.083692 urlopen2-1.0.1/LICENSE
--rw-r--r--   0        0        0      409 2023-05-29 09:38:35.642659 urlopen2-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      514 2023-05-29 08:06:49.944797 urlopen2-1.0.1/README.md
--rw-r--r--   0        0        0       28 2023-05-29 06:42:37.689478 urlopen2-1.0.1/urlopen2/__init__.py
--rw-r--r--   0        0        0     2751 2023-05-29 09:35:54.223369 urlopen2-1.0.1/urlopen2/urlfile.py
--rw-r--r--   0        0        0      720 2023-05-29 07:40:28.892802 urlopen2-1.0.1/urlopen2/urlfile.pyi
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 urlopen2-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-29 07:15:28.083692 urlopen2-1.1.0/LICENSE
+-rw-r--r--   0        0        0      409 2023-05-30 21:57:21.073750 urlopen2-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      525 2023-05-30 21:50:54.886233 urlopen2-1.1.0/README.md
+-rw-r--r--   0        0        0       28 2023-05-29 06:42:37.689478 urlopen2-1.1.0/urlopen2/__init__.py
+-rw-r--r--   0        0        0     2773 2023-05-30 22:18:03.908542 urlopen2-1.1.0/urlopen2/urlfile.py
+-rw-r--r--   0        0        0      732 2023-05-30 22:18:49.779305 urlopen2-1.1.0/urlopen2/urlfile.pyi
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 urlopen2-1.1.0/PKG-INFO
```

### Comparing `urlopen2-1.0.1/LICENSE` & `urlopen2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urlopen2-1.0.1/README.md` & `urlopen2-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 pip install urlopen2
 ```
 
 ## Using
 ```python
 from urlopen2 import URLFile
 
-with URLFile("https://example.com/file.bin") as f:
+url = "https://example.com/file.bin"
+
+with URLFile(url) as f:
     f.read(128)
     # In this case, 128 bytes of the file will be loaded.
     f.seek(0)
     # Move the caret to the beginning of the file
     data = f.read(128) 
     # Since we are taking the same 128 bytes that have already been loaded, they will be received from the buffer.
```

### Comparing `urlopen2-1.0.1/urlopen2/urlfile.py` & `urlopen2-1.1.0/urlopen2/urlfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from io import IOBase, BytesIO, BufferedRandom
 from urllib.request import urlopen
+from io import BytesIO, BufferedRandom, RawIOBase
 # > Typing
 from typing import Optional, Union
 
 # ! Main
-class URLFile(IOBase):
+class URLFile(RawIOBase):
     def __init__(
         self,
         url: str,
         *,
         buffer: Optional[Union[BytesIO, BufferedRandom]]=None,
         **kwargs
     ) -> None:
@@ -16,15 +16,15 @@
         self._buffer = buffer or BytesIO()
         self._furl = urlopen(self._name, **kwargs)
         self._full: bool = False
     
     @property
     def name(self) -> str: return self._name
     @property
-    def mode(self) -> str: return "r"
+    def mode(self) -> str: return "rb"
     @property
     def closed(self) -> bool: return self._buffer.closed
     @property
     def full(self) -> bool: return self._full
     
     def readable(self) -> bool: return True
     def seekable(self) -> bool: return True
@@ -58,32 +58,32 @@
             self._buffer.seek(0, 2)
             while len(data:=self._furl.read(65536)) > 0:
                 self._buffer.write(data)
             self._furl.close()
             self._full = True
             self._buffer.seek(ct)
     
-    def read(self, n: int=-1):
+    def read(self, n: int=-1) -> bytes:
         if n is None:
             n = -1
         if not self._full:
             if n > 0:
                 s = n - (self._getsize() - self.tell())
                 if s > 0:
                     self._topload(s)
             elif n < 0:
                 self._fullload()
         return self._buffer.read(n)
     
-    def seek(self, offset: int, whence: int=0) -> None:
+    def seek(self, offset: int, whence: int=0) -> int:
         if (offset > 0) and (not self._full):
             if whence == 0:
                 s = self._getsize() - offset
                 if s > 0:
                     self._topload(s)
             elif whence == 1:
                 s = offset - (self._getsize() - self.tell())
                 if s > 0:
                     self._topload(s)
             elif whence == 2:
                 self._fullload()
-        self._buffer.seek(offset, whence)
+        return self._buffer.seek(offset, whence)
```

### Comparing `urlopen2-1.0.1/urlopen2/urlfile.pyi` & `urlopen2-1.1.0/urlopen2/urlfile.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from io import IOBase
+from io import RawIOBase
 from typing import Optional, IO
 
-
-class URLFile(IOBase):
+class URLFile(RawIOBase):
     def __init__(
         self,
         url: str,
         *,
         buffer: Optional[IO[bytes]]=None,
         **kwargs
     ) -> None: ...
@@ -21,11 +20,11 @@
     def full(self) -> bool: ...
     
     def readable(self) -> bool: ...
     def seekable(self) -> bool: ...
     def writable(self) -> bool: ...
     
     def tell(self) -> int: ...
-    def seek(self, offset: int, whence: int=0) -> None: ...
-    def read(self, n: int=-1): ...
+    def seek(self, offset: int, whence: int=0) -> int: ...
+    def read(self, n: int=-1) -> bytes: ...
     
     def close(self) -> None: ...
```

### Comparing `urlopen2-1.0.1/PKG-INFO` & `urlopen2-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlopen2
-Version: 1.0.1
+Version: 1.1.0
 Summary: Improvement for the `urlopen` function.
 License: MIT
 Keywords: urlopen,urllib.request,urlfile,readable,seekable
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,17 @@
 pip install urlopen2
 ```
 
 ## Using
 ```python
 from urlopen2 import URLFile
 
-with URLFile("https://example.com/file.bin") as f:
+url = "https://example.com/file.bin"
+
+with URLFile(url) as f:
     f.read(128)
     # In this case, 128 bytes of the file will be loaded.
     f.seek(0)
     # Move the caret to the beginning of the file
     data = f.read(128) 
     # Since we are taking the same 128 bytes that have already been loaded, they will be received from the buffer.
```

