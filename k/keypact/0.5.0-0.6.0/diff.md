# Comparing `tmp/keypact-0.5.0.tar.gz` & `tmp/keypact-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.5.0.tar", last modified: Wed May 31 14:56:53 2023, max compression
+gzip compressed data, was "keypact-0.6.0.tar", last modified: Wed May 31 15:46:23 2023, max compression
```

## Comparing `keypact-0.5.0.tar` & `keypact-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:53.915442 keypact-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 14:56:44.000000 keypact-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-31 14:56:53.915442 keypact-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-31 14:56:44.000000 keypact-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:56:53.915442 keypact-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 14:56:44.000000 keypact-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:53.911441 keypact-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:53.911441 keypact-0.5.0/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 14:56:44.000000 keypact-0.5.0/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-31 14:56:44.000000 keypact-0.5.0/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:53.915442 keypact-0.5.0/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:23.406116 keypact-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 15:46:09.000000 keypact-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-31 15:46:23.406116 keypact-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-31 15:46:09.000000 keypact-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:46:23.406116 keypact-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 15:46:09.000000 keypact-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:23.406116 keypact-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:23.406116 keypact-0.6.0/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 15:46:09.000000 keypact-0.6.0/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-31 15:46:09.000000 keypact-0.6.0/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:46:23.406116 keypact-0.6.0/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 15:46:23.000000 keypact-0.6.0/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.5.0/LICENSE` & `keypact-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.5.0/PKG-INFO` & `keypact-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.5.0
+Version: 0.6.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -12,14 +12,16 @@
         ## Features
         - Multithread Support
         - Simultaneous Writing
         - Easy to use
         - Easy to integrate
         - Easy to deploy
         - Able to saving files
+        - Able to compressing datas
+        - Able to storing pyton objects (Pickle)
         
         
         ## Installation
         You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
```

### Comparing `keypact-0.5.0/README.md` & `keypact-0.6.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 ## Features
 - Multithread Support
 - Simultaneous Writing
 - Easy to use
 - Easy to integrate
 - Easy to deploy
 - Able to saving files
+- Able to compressing datas
+- Able to storing pyton objects (Pickle)
 
 
 ## Installation
 You can install KeyPact by pip3:
 
 ```console
 pip3 install keypact
```

### Comparing `keypact-0.5.0/setup.py` & `keypact-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.5.0',
+version='0.6.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
 packages=["keypact"],
 package_dir={'':'src'},
 install_requires=[
-    "fire==0.5.0"
+    "fire==0.5.0",
+    "mgzip==0.2.1"
 ],
 entry_points = {
     'console_scripts': ['keypact=keypact.keypact:main'],
 },
 python_requires=">= 3",
 zip_safe=False)
```

### Comparing `keypact-0.5.0/src/keypact/keypact.py` & `keypact-0.6.0/src/keypact/keypact.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import pickle
 
 import fire
 
 import time
 from shutil import move, copy
 
+import mgzip
+
+
 class KeyPact:
 
     def __init__(self, name):
         self.name = name
         self.hashed_name = sha256(name.encode()).hexdigest()
         self.location = os.path.join(os.getcwd(), "kp-" + self.hashed_name)
 
@@ -25,34 +28,45 @@
     def initialize(self):
         try: 
             os.makedirs(self.location)
         except OSError:
             if not os.path.isdir(self.location):
                 raise
 
-    def set(self, key: str, value, type_of_value="str") -> str:
+    def set(self, key: str, value, type_of_value: str ="str", compress: bool=False) -> str:
         self.counter += 1
         
         
 
 
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
 
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
         key_location_loading = os.path.join(self.location, key_location+".l")
         key_location_loading_indicator = os.path.join(self.location, key_location+".li")
 
         key_location_reading_indicator = os.path.join(self.location, key_location+".re")
+        key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
         
 
+        if compress:
+            # create key_location_compress_indicator
+            with open(key_location_compress_indicator, "wb") as f:
+                f.write(b"1")
+
+            with mgzip.open(key_location_loading, "wb") as f:
+                pickle.dump({"key":key,"value":value, "type":type}, f)
+        
+        else:
+            with open(key_location_loading, "wb") as f:
+                pickle.dump({"key":key,"value":value, "type":type}, f)
+
 
-        with open(key_location_loading, "wb") as f:
-            pickle.dump({"key":key,"value":value, "type":type}, f)
 
 
         #Create a file that inform is loading
         with open(key_location_loading_indicator, "wb") as f:
             f.write(b"1")
 
         while os.path.exists(key_location_reading_indicator):
@@ -96,14 +110,15 @@
 
 
     def get(self, key: str, custom_key_location: str = None):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest()) if custom_key_location == None else custom_key_location
 
         key_location_loading_indicator = os.path.join(self.location, key_location+".li")
         key_location_reading_indicator = os.path.join(self.location, key_location+".re")
+        key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
         while os.path.exists(key_location_loading_indicator):
             time.sleep(0.1)
 
 
 
         if not os.path.isfile(os.path.join(self.location, key_location)):
@@ -111,52 +126,74 @@
 
         total_result = None
 
         try:
             
             with open(key_location_reading_indicator, "wb") as f:
                 f.write(b"1")
-            with open(os.path.join(self.location, key_location), "rb") as f:
-                result = pickle.load(f)
-                try:
-                    total_result = result["value"]
-                except TypeError:
-                    total_result = result
+            if os.path.exists(key_location_compress_indicator):
+                with mgzip.open(os.path.join(self.location, key_location), "rb") as f:
+                    result = pickle.load(f)
+                    try:
+                        total_result = result["value"]
+                    except TypeError:
+                        total_result = result
+            else:
+                with open(os.path.join(self.location, key_location), "rb") as f:
+                    result = pickle.load(f)
+                    try:
+                        total_result = result["value"]
+                    except TypeError:
+                        total_result = result
         except EOFError or FileNotFoundError:
             pass
 
         if os.path.isfile(key_location_reading_indicator):
             os.remove(key_location_reading_indicator)
 
         return total_result
 
     def get_key(self, key_location: str):
        
-
+        key_location_compress_indicator = os.path.join(self.location, key_location+".co")
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
         total_result = None
 
         try:
-            with open(os.path.join(self.location, key_location), "rb") as f:
-                result = pickle.load(f)
-                if not "type" in result:
-                    result["type"] = "str"
-                try:
-                    total_result = result["key"]
-                except TypeError:
-                    total_result = False
+            if os.path.exists(key_location_compress_indicator):
+                with mgzip.open(os.path.join(self.location, key_location), "rb") as f:
+                    result = pickle.load(f)
+                    if not "type" in result:
+                        result["type"] = "str"
+                    try:
+                        total_result = result["key"]
+                    except TypeError:
+                        total_result = False            
+            else:
+                with open(os.path.join(self.location, key_location), "rb") as f:
+                    result = pickle.load(f)
+                    if not "type" in result:
+                        result["type"] = "str"
+                    try:
+                        total_result = result["key"]
+                    except TypeError:
+                        total_result = False
         except EOFError or FileNotFoundError:
             pass            
         return total_result
 
     def delete(self, key: str):
         key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
 
+        key_location_compress_indicator = os.path.join(self.location, key_location+".co")
+
         try:
+            if os.path.exists(key_location_compress_indicator):
+                os.remove(os.path.join(self.location, key_location_compress_indicator))
             os.remove(os.path.join(self.location, key_location))
         except OSError:
             pass
 
     def delete_file(self, key: str):
         
 
@@ -171,17 +208,37 @@
     def delete_all(self):
         for key in self.dict():
             self.delete(key)
 
     def dict(self):
         result ={}
         for key in os.listdir(self.location):
-            the_key = self.get_key(key)
-            if not the_key is None:
-                if the_key != False:
-                    result_of_key = self.get(the_key)
-                    if not result_of_key is None:
-                        result[the_key] = result_of_key
+            if not "." in key:
+                the_key = self.get_key(key)
+                if not the_key is None:
+                    if the_key != False:
+                        result_of_key = self.get(the_key)
+                        if not result_of_key is None:
+                            result[the_key] = result_of_key
         return result
 
+    def size_all(self):
+        #Calculate self.location size
+        total_size = 0
+
+        for dirpath, dirnames, filenames in os.walk(self.location):
+            for f in filenames:
+                fp = os.path.join(dirpath, f)
+                total_size += os.path.getsize(fp)
+
+        return total_size
+    
+    def size(self, key: str):
+        key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
+
+        key_location_compress_indicator = os.path.join(self.location, key_location+".co")
+
+        return os.path.getsize(os.path.join(self.location, key_location))
+
+
 def main():
     fire.Fire(KeyPact)
```

### Comparing `keypact-0.5.0/src/keypact.egg-info/PKG-INFO` & `keypact-0.6.0/src/keypact.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.5.0
+Version: 0.6.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -12,14 +12,16 @@
         ## Features
         - Multithread Support
         - Simultaneous Writing
         - Easy to use
         - Easy to integrate
         - Easy to deploy
         - Able to saving files
+        - Able to compressing datas
+        - Able to storing pyton objects (Pickle)
         
         
         ## Installation
         You can install KeyPact by pip3:
         
         ```console
         pip3 install keypact
```

