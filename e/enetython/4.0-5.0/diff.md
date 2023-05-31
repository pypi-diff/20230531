# Comparing `tmp/enetython-4.0.tar.gz` & `tmp/enetython-5.0.tar.gz`

## Comparing `enetython-4.0.tar` & `enetython-5.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:25:58.000000 enetython-4.0/
--rw-rw----   0 root         (0) everybody  (9997)     1571 2023-05-31 19:24:34.000000 enetython-4.0/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      171 2023-05-31 19:25:58.000000 enetython-4.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1422 2023-05-31 19:24:34.000000 enetython-4.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:29:27.000000 enetython-4.0/enet/
--rw-rw----   0 root         (0) everybody  (9997)      971 2023-05-31 19:24:33.000000 enetython-4.0/enet/callbacks.c
--rw-rw----   0 root         (0) everybody  (9997)    21286 2023-05-31 19:24:33.000000 enetython-4.0/enet/compress.c
--rw-rw----   0 root         (0) everybody  (9997)    18406 2023-05-31 19:24:33.000000 enetython-4.0/enet/host.c
--rw-rw----   0 root         (0) everybody  (9997)     1579 2023-05-31 19:24:34.000000 enetython-4.0/enet/list.c
--rw-rw----   0 root         (0) everybody  (9997)     6334 2023-05-31 19:24:34.000000 enetython-4.0/enet/packet.c
--rw-rw----   0 root         (0) everybody  (9997)    38985 2023-05-31 19:24:34.000000 enetython-4.0/enet/peer.c
--rw-rw----   0 root         (0) everybody  (9997)    71138 2023-05-31 19:24:34.000000 enetython-4.0/enet/protocol.c
--rw-rw----   0 root         (0) everybody  (9997)    14774 2023-05-31 19:24:34.000000 enetython-4.0/enet/unix.c
--rw-rw----   0 root         (0) everybody  (9997)    10921 2023-05-31 19:24:34.000000 enetython-4.0/enet/win32.c
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:29:27.000000 enetython-4.0/enet/enet/
--rw-rw----   0 root         (0) everybody  (9997)      522 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/callbacks.h
--rw-rw----   0 root         (0) everybody  (9997)    26262 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/enet.h
--rw-rw----   0 root         (0) everybody  (9997)     1099 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/list.h
--rw-rw----   0 root         (0) everybody  (9997)     5748 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/protocol.h
--rw-rw----   0 root         (0) everybody  (9997)      530 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/time.h
--rw-rw----   0 root         (0) everybody  (9997)      347 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/types.h
--rw-rw----   0 root         (0) everybody  (9997)     1346 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/unix.h
--rw-rw----   0 root         (0) everybody  (9997)      303 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/utility.h
--rw-rw----   0 root         (0) everybody  (9997)     1490 2023-03-17 05:33:41.000000 enetython-4.0/enet/enet/win32.h
--rw-rw----   0 root         (0) everybody  (9997)    34114 2023-05-31 19:24:34.000000 enetython-4.0/enet.pyx
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:25:58.000000 enetython-4.0/enetython.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      171 2023-05-31 19:25:58.000000 enetython-4.0/enetython.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      338 2023-05-31 19:25:58.000000 enetython-4.0/enetython.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-31 19:25:58.000000 enetython-4.0/enetython.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       13 2023-05-31 19:25:58.000000 enetython-4.0/enetython.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-31 19:25:58.000000 enetython-4.0/enetython.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       76 2023-05-31 19:24:34.000000 enetython-4.0/pyproject.toml
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-31 19:25:58.000000 enetython-4.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1311 2023-05-31 19:24:34.000000 enetython-4.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:43:20.000000 enetython-5.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1571 2023-05-31 19:24:34.000000 enetython-5.0/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      171 2023-05-31 19:43:20.000000 enetython-5.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1422 2023-05-31 19:24:34.000000 enetython-5.0/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:44:47.000000 enetython-5.0/enet/
+-rw-rw----   0 root         (0) everybody  (9997)      971 2023-05-31 19:24:33.000000 enetython-5.0/enet/callbacks.c
+-rw-rw----   0 root         (0) everybody  (9997)    21286 2023-05-31 19:24:33.000000 enetython-5.0/enet/compress.c
+-rw-rw----   0 root         (0) everybody  (9997)    18406 2023-05-31 19:24:33.000000 enetython-5.0/enet/host.c
+-rw-rw----   0 root         (0) everybody  (9997)     1579 2023-05-31 19:24:34.000000 enetython-5.0/enet/list.c
+-rw-rw----   0 root         (0) everybody  (9997)     6334 2023-05-31 19:24:34.000000 enetython-5.0/enet/packet.c
+-rw-rw----   0 root         (0) everybody  (9997)    38985 2023-05-31 19:24:34.000000 enetython-5.0/enet/peer.c
+-rw-rw----   0 root         (0) everybody  (9997)    71138 2023-05-31 19:24:34.000000 enetython-5.0/enet/protocol.c
+-rw-rw----   0 root         (0) everybody  (9997)    14774 2023-05-31 19:24:34.000000 enetython-5.0/enet/unix.c
+-rw-rw----   0 root         (0) everybody  (9997)    10921 2023-05-31 19:24:34.000000 enetython-5.0/enet/win32.c
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:44:47.000000 enetython-5.0/enet/include/
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:44:47.000000 enetython-5.0/enet/include/enet/
+-rw-rw----   0 root         (0) everybody  (9997)      522 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/callbacks.h
+-rw-rw----   0 root         (0) everybody  (9997)    26262 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/enet.h
+-rw-rw----   0 root         (0) everybody  (9997)     1099 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/list.h
+-rw-rw----   0 root         (0) everybody  (9997)     5748 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/protocol.h
+-rw-rw----   0 root         (0) everybody  (9997)      530 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/time.h
+-rw-rw----   0 root         (0) everybody  (9997)      347 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/types.h
+-rw-rw----   0 root         (0) everybody  (9997)     1346 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/unix.h
+-rw-rw----   0 root         (0) everybody  (9997)      303 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/utility.h
+-rw-rw----   0 root         (0) everybody  (9997)     1490 2023-03-17 05:33:41.000000 enetython-5.0/enet/include/enet/win32.h
+-rw-rw----   0 root         (0) everybody  (9997)    34114 2023-05-31 19:24:34.000000 enetython-5.0/enet.pyx
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-31 19:43:20.000000 enetython-5.0/enetython.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      171 2023-05-31 19:43:20.000000 enetython-5.0/enetython.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      338 2023-05-31 19:43:20.000000 enetython-5.0/enetython.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-31 19:43:20.000000 enetython-5.0/enetython.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       13 2023-05-31 19:43:20.000000 enetython-5.0/enetython.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-05-31 19:43:20.000000 enetython-5.0/enetython.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       76 2023-05-31 19:24:34.000000 enetython-5.0/pyproject.toml
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-31 19:43:20.000000 enetython-5.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1311 2023-05-31 19:39:10.000000 enetython-5.0/setup.py
```

### Comparing `enetython-4.0/LICENSE` & `enetython-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enetython-4.0/README.md` & `enetython-5.0/README.md`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/callbacks.c` & `enetython-5.0/enet/callbacks.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/compress.c` & `enetython-5.0/enet/compress.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/host.c` & `enetython-5.0/enet/host.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/list.c` & `enetython-5.0/enet/list.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/packet.c` & `enetython-5.0/enet/packet.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/peer.c` & `enetython-5.0/enet/peer.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/protocol.c` & `enetython-5.0/enet/protocol.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/unix.c` & `enetython-5.0/enet/unix.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/win32.c` & `enetython-5.0/enet/win32.c`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/enet/callbacks.h` & `enetython-5.0/enet/include/enet/callbacks.h`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/enet/enet.h` & `enetython-5.0/enet/include/enet/enet.h`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/enet/list.h` & `enetython-5.0/enet/include/enet/list.h`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/enet/protocol.h` & `enetython-5.0/enet/include/enet/protocol.h`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/enet/time.h` & `enetython-5.0/enet/include/enet/time.h`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/enet/unix.h` & `enetython-5.0/enet/include/enet/unix.h`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet/enet/win32.h` & `enetython-5.0/enet/include/enet/win32.h`

 * *Files identical despite different names*

### Comparing `enetython-4.0/enet.pyx` & `enetython-5.0/enet.pyx`

 * *Files identical despite different names*

### Comparing `enetython-4.0/setup.py` & `enetython-5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 requirements = [
 	"cython>=0.25"
 ]
 
 setup(
 	name = "enetython",
-	version = "4.0",
+	version = "5.0",
 	description = "A python wrapper for the ENet library",
 	author = "aresch",
 	author_email = "andrewresch@gmail.com",
 	cmdclass = {"build_ext": build_ext},
 	ext_modules = ext_modules,
 	install_requires = requirements
 )
```

