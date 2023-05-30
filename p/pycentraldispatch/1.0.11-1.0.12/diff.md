# Comparing `tmp/pycentraldispatch-1.0.11.tar.gz` & `tmp/pycentraldispatch-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycentraldispatch-1.0.11.tar", last modified: Sun Jan  3 02:39:15 2021, max compression
+gzip compressed data, was "pycentraldispatch-1.0.12.tar", last modified: Tue May 30 22:13:38 2023, max compression
```

## Comparing `pycentraldispatch-1.0.11.tar` & `pycentraldispatch-1.0.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-01-03 02:39:15.381409 pycentraldispatch-1.0.11/
--rw-rw-rw-   0        0        0     1086 2021-01-03 02:37:23.000000 pycentraldispatch-1.0.11/LICENSE
--rw-rw-rw-   0        0        0       25 2021-01-03 02:37:23.000000 pycentraldispatch-1.0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     3741 2021-01-03 02:39:15.365800 pycentraldispatch-1.0.11/PKG-INFO
--rw-rw-rw-   0        0        0     2612 2021-01-03 02:37:23.000000 pycentraldispatch-1.0.11/README.md
-drwxrwxrwx   0        0        0        0 2021-01-03 02:39:15.334534 pycentraldispatch-1.0.11/pycentraldispatch/
--rw-rw-rw-   0        0        0       67 2021-01-03 02:37:23.000000 pycentraldispatch-1.0.11/pycentraldispatch/__init__.py
--rw-rw-rw-   0        0        0     3430 2021-01-03 02:37:23.000000 pycentraldispatch-1.0.11/pycentraldispatch/py_central_dispatch.py
--rw-rw-rw-   0        0        0     2097 2021-01-03 02:37:24.000000 pycentraldispatch-1.0.11/pycentraldispatch/thread_pool.py
-drwxrwxrwx   0        0        0        0 2021-01-03 02:39:15.365800 pycentraldispatch-1.0.11/pycentraldispatch.egg-info/
--rw-rw-rw-   0        0        0     3741 2021-01-03 02:39:14.000000 pycentraldispatch-1.0.11/pycentraldispatch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2021-01-03 02:39:15.000000 pycentraldispatch-1.0.11/pycentraldispatch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-03 02:39:15.000000 pycentraldispatch-1.0.11/pycentraldispatch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2021-01-03 02:39:15.000000 pycentraldispatch-1.0.11/pycentraldispatch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-01-03 02:39:15.381409 pycentraldispatch-1.0.11/setup.cfg
--rw-rw-rw-   0        0        0      742 2021-01-03 02:39:10.000000 pycentraldispatch-1.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:13:38.542027 pycentraldispatch-1.0.12/
+-rw-rw-rw-   0        0        0     1086 2021-09-24 22:16:05.000000 pycentraldispatch-1.0.12/LICENSE
+-rw-rw-rw-   0        0        0       25 2021-09-24 22:16:05.000000 pycentraldispatch-1.0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     3155 2023-05-30 22:13:38.541026 pycentraldispatch-1.0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2612 2021-09-24 22:16:05.000000 pycentraldispatch-1.0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 22:13:38.539026 pycentraldispatch-1.0.12/pycentraldispatch/
+-rw-rw-rw-   0        0        0       67 2021-09-24 22:16:05.000000 pycentraldispatch-1.0.12/pycentraldispatch/__init__.py
+-rw-rw-rw-   0        0        0     3432 2023-05-30 22:12:01.000000 pycentraldispatch-1.0.12/pycentraldispatch/py_central_dispatch.py
+-rw-rw-rw-   0        0        0     2097 2021-09-24 22:16:05.000000 pycentraldispatch-1.0.12/pycentraldispatch/thread_pool.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:13:38.541026 pycentraldispatch-1.0.12/pycentraldispatch.egg-info/
+-rw-rw-rw-   0        0        0     3155 2023-05-30 22:13:38.000000 pycentraldispatch-1.0.12/pycentraldispatch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-30 22:13:38.000000 pycentraldispatch-1.0.12/pycentraldispatch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 22:13:38.000000 pycentraldispatch-1.0.12/pycentraldispatch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-30 22:13:38.000000 pycentraldispatch-1.0.12/pycentraldispatch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 22:13:38.542027 pycentraldispatch-1.0.12/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-05-30 22:12:01.000000 pycentraldispatch-1.0.12/setup.py
```

### Comparing `pycentraldispatch-1.0.11/LICENSE` & `pycentraldispatch-1.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pycentraldispatch-1.0.11/README.md` & `pycentraldispatch-1.0.12/README.md`

 * *Files identical despite different names*

### Comparing `pycentraldispatch-1.0.11/pycentraldispatch/py_central_dispatch.py` & `pycentraldispatch-1.0.12/pycentraldispatch/py_central_dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
       self.__lock.release()
       block(*args, **kwargs)
       # If the queue is serial, continually dispatch blocks one after the
       # other to ensure serial execution on the same thread.
       if self.__is_serial_queue:
         self.__lock.acquire()
         if len(self.__pendingBlocks) > 0:
-          self.__dispatchOneBlock()
+          self.__dispatch_one_block()
         else:
           self.__is_serial_queue_active = False
         self.__lock.release()
     self.__class__.__thread_pool.addBlock(lambda_like_function)
 
   def dispatch_async(self, block, args=(), kwargs={}):
     """Dispatches asyncronously and then returns."""
```

### Comparing `pycentraldispatch-1.0.11/pycentraldispatch/thread_pool.py` & `pycentraldispatch-1.0.12/pycentraldispatch/thread_pool.py`

 * *Files identical despite different names*

### Comparing `pycentraldispatch-1.0.11/setup.py` & `pycentraldispatch-1.0.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycentraldispatch",
-    version="1.0.11",
+    version="1.0.12",
     author="MrHappyAsthma",
     author_email="mrhappyasthma@gmail.com",
     description="A simple Grand Central Dispatch (GCD) inspired API for python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrhappyasthma/PyCentralDispatch",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-)
+)
```

