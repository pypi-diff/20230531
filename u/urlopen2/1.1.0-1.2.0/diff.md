# Comparing `tmp/urlopen2-1.1.0.tar.gz` & `tmp/urlopen2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlopen2-1.1.0.tar", max compression
+gzip compressed data, was "urlopen2-1.2.0.tar", max compression
```

## Comparing `urlopen2-1.1.0.tar` & `urlopen2-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2023-05-29 07:15:28.083692 urlopen2-1.1.0/LICENSE
--rw-r--r--   0        0        0      409 2023-05-30 21:57:21.073750 urlopen2-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      525 2023-05-30 21:50:54.886233 urlopen2-1.1.0/README.md
--rw-r--r--   0        0        0       28 2023-05-29 06:42:37.689478 urlopen2-1.1.0/urlopen2/__init__.py
--rw-r--r--   0        0        0     2773 2023-05-30 22:18:03.908542 urlopen2-1.1.0/urlopen2/urlfile.py
--rw-r--r--   0        0        0      732 2023-05-30 22:18:49.779305 urlopen2-1.1.0/urlopen2/urlfile.pyi
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 urlopen2-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-29 07:15:28.083692 urlopen2-1.2.0/LICENSE
+-rw-r--r--   0        0        0      424 2023-05-31 17:54:45.332712 urlopen2-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      532 2023-05-30 22:23:41.505539 urlopen2-1.2.0/README.md
+-rw-r--r--   0        0        0       28 2023-05-29 06:42:37.689478 urlopen2-1.2.0/urlopen2/__init__.py
+-rw-r--r--   0        0        0     3709 2023-05-31 18:14:15.226337 urlopen2-1.2.0/urlopen2/urlfile.py
+-rw-r--r--   0        0        0      946 2023-05-31 17:54:45.333702 urlopen2-1.2.0/urlopen2/urlfile.pyi
+-rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 urlopen2-1.2.0/PKG-INFO
```

### Comparing `urlopen2-1.1.0/LICENSE` & `urlopen2-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `urlopen2-1.1.0/README.md` & `urlopen2-1.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # urlopen2
 ## Description
-Improvement for the `urlopen` function.request.
+Improvement for the `urllib.request.urlopen` function.
 
 ## Install
 ```shell
 pip install urlopen2
 ```
 
 ## Using
```

### Comparing `urlopen2-1.1.0/urlopen2/urlfile.pyi` & `urlopen2-1.2.0/urlopen2/urlfile.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,30 @@
         url: str,
         *,
         buffer: Optional[IO[bytes]]=None,
         **kwargs
     ) -> None: ...
     
     @property
+    def length(self) -> Optional[int]: ...
+    @property
+    def downloaded(self) -> int: ...
+    @property
     def name(self) -> str: ...
     @property
     def mode(self) -> str: ...
     @property
     def closed(self) -> bool: ...
     @property
     def full(self) -> bool: ...
     
+    def fulling(self) -> None:
+        """Full topload of the file to the buffer."""
+        ...
+
     def readable(self) -> bool: ...
     def seekable(self) -> bool: ...
     def writable(self) -> bool: ...
     
     def tell(self) -> int: ...
     def seek(self, offset: int, whence: int=0) -> int: ...
     def read(self, n: int=-1) -> bytes: ...
```

### Comparing `urlopen2-1.1.0/PKG-INFO` & `urlopen2-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: urlopen2
-Version: 1.1.0
-Summary: Improvement for the `urlopen` function.
+Version: 1.2.0
+Summary: Improvement for the `urllib.request.urlopen` function.
 License: MIT
 Keywords: urlopen,urllib.request,urlfile,readable,seekable
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # urlopen2
 ## Description
-Improvement for the `urlopen` function.request.
+Improvement for the `urllib.request.urlopen` function.
 
 ## Install
 ```shell
 pip install urlopen2
 ```
 
 ## Using
```

