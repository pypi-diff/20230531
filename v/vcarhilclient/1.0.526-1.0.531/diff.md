# Comparing `tmp/vcarhilclient-1.0.526.tar.gz` & `tmp/vcarhilclient-1.0.531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcarhilclient-1.0.526.tar", last modified: Fri May 26 03:15:04 2023, max compression
+gzip compressed data, was "vcarhilclient-1.0.531.tar", last modified: Wed May 31 10:26:07 2023, max compression
```

## Comparing `vcarhilclient-1.0.526.tar` & `vcarhilclient-1.0.531.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 03:15:04.891093 vcarhilclient-1.0.526/
--rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.526/LICENSE
--rw-rw-rw-   0        0        0     2596 2023-05-26 03:15:04.891093 vcarhilclient-1.0.526/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.526/README.md
--rw-rw-rw-   0        0        0       86 2023-05-26 03:15:04.892093 vcarhilclient-1.0.526/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-05-26 03:13:26.000000 vcarhilclient-1.0.526/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:15:04.877619 vcarhilclient-1.0.526/vcarhilclient/
--rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.526/vcarhilclient/Enums.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.526/vcarhilclient/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.526/vcarhilclient/drt_structures.py
--rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.526/vcarhilclient/kunyi_ma.py
--rw-rw-rw-   0        0        0    50548 2023-05-26 02:40:36.000000 vcarhilclient-1.0.526/vcarhilclient/kunyi_mrt.py
--rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.526/vcarhilclient/kunyi_project.py
--rw-rw-rw-   0        0        0    12136 2023-05-24 08:09:40.000000 vcarhilclient-1.0.526/vcarhilclient/kunyi_util.py
--rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.526/vcarhilclient/minio_handld.py
--rw-rw-rw-   0        0        0     2158 2023-05-23 10:04:11.000000 vcarhilclient-1.0.526/vcarhilclient/mrt_strunctures.py
--rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.526/vcarhilclient/signal_daq.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:15:04.889105 vcarhilclient-1.0.526/vcarhilclient.egg-info/
--rw-rw-rw-   0        0        0     2596 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-26 03:15:04.000000 vcarhilclient-1.0.526/vcarhilclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 10:26:07.022249 vcarhilclient-1.0.531/
+-rw-rw-rw-   0        0        0     1090 2022-07-29 01:38:14.000000 vcarhilclient-1.0.531/LICENSE
+-rw-rw-rw-   0        0        0     2644 2023-05-31 10:26:07.022249 vcarhilclient-1.0.531/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-04-26 09:29:14.000000 vcarhilclient-1.0.531/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-31 10:26:07.023248 vcarhilclient-1.0.531/setup.cfg
+-rw-rw-rw-   0        0        0      788 2023-05-31 10:24:02.000000 vcarhilclient-1.0.531/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:26:07.006720 vcarhilclient-1.0.531/vcarhilclient/
+-rw-rw-rw-   0        0        0     6908 2023-05-26 02:40:36.000000 vcarhilclient-1.0.531/vcarhilclient/Enums.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:41:29.000000 vcarhilclient-1.0.531/vcarhilclient/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:02:47.000000 vcarhilclient-1.0.531/vcarhilclient/drt_structures.py
+-rw-rw-rw-   0        0        0    41274 2023-05-23 05:09:06.000000 vcarhilclient-1.0.531/vcarhilclient/kunyi_ma.py
+-rw-rw-rw-   0        0        0    50876 2023-05-31 10:22:11.000000 vcarhilclient-1.0.531/vcarhilclient/kunyi_mrt.py
+-rw-rw-rw-   0        0        0    15331 2023-05-26 02:43:20.000000 vcarhilclient-1.0.531/vcarhilclient/kunyi_project.py
+-rw-rw-rw-   0        0        0    12059 2023-05-31 10:22:11.000000 vcarhilclient-1.0.531/vcarhilclient/kunyi_util.py
+-rw-rw-rw-   0        0        0     3356 2023-05-05 06:01:57.000000 vcarhilclient-1.0.531/vcarhilclient/minio_handld.py
+-rw-rw-rw-   0        0        0     2158 2023-05-23 10:04:11.000000 vcarhilclient-1.0.531/vcarhilclient/mrt_strunctures.py
+-rw-rw-rw-   0        0        0     5422 2023-05-05 09:43:01.000000 vcarhilclient-1.0.531/vcarhilclient/signal_daq.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:26:07.020238 vcarhilclient-1.0.531/vcarhilclient.egg-info/
+-rw-rw-rw-   0        0        0     2644 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 10:26:06.000000 vcarhilclient-1.0.531/vcarhilclient.egg-info/top_level.txt
```

### Comparing `vcarhilclient-1.0.526/LICENSE` & `vcarhilclient-1.0.531/LICENSE`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.526/PKG-INFO` & `vcarhilclient-1.0.531/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.526
+Version: 1.0.531
 Summary: vcarhilclient
-Home-page: 
+Home-page: UNKNOWN
 Author: vcarsystem
 Author-email: service@vcarsystem.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -105,7 +107,9 @@
 assert ec.value == 0
 
 # 18.Delete the experiment
 ec = my_mrt.delete_test_env("envName")
 
 assert ec.value == 0
 
+
+
```

### Comparing `vcarhilclient-1.0.526/README.md` & `vcarhilclient-1.0.531/README.md`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.526/setup.py` & `vcarhilclient-1.0.531/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vcarhilclient",  # 包名
-    version="1.0.526",
+    version="1.0.531",
     author="vcarsystem",
     author_email="service@vcarsystem.com",
     description="vcarhilclient",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `vcarhilclient-1.0.526/vcarhilclient/Enums.py` & `vcarhilclient-1.0.531/vcarhilclient/Enums.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.526/vcarhilclient/kunyi_ma.py` & `vcarhilclient-1.0.531/vcarhilclient/kunyi_ma.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.526/vcarhilclient/kunyi_mrt.py` & `vcarhilclient-1.0.531/vcarhilclient/kunyi_mrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,27 +210,28 @@
         mrt_lib.mrt_download_file.argtypes = [c_void_p, c_char_p, CALLBACK, POINTER(c_uint64)]
         mrt_lib.mrt_download_file.restype = mrt_status_t
         my_callback = CALLBACK(mrt_client.call_back)
         error_code = mrt_lib.mrt_download_file(self.context, path_pointer, my_callback, file_id_pointer)
         return error_code, file_id_pointer.contents.value
 
 
-    def get_input_port_value(self, env_name, instance_name, port_name, signal_data_type, item_count, struct_detail=None, **sub_struct_detail):
+    def get_input_port_value(self, env_name, instance_name, port_name, signal_data_type, item_count=1, struct_detail=None, **sub_struct_detail):
         return self.get_port_value(env_name, instance_name, port_name,
                                    mrt_port_type_t.MRT_INPUT_PORT, signal_data_type, item_count, struct_detail, **sub_struct_detail)
 
-    def get_output_port_value(self, env_name, instance_name, port_name, signal_data_type, item_count, struct_detail=None, **sub_struct_detail):
+    def get_output_port_value(self, env_name, instance_name, port_name, signal_data_type, item_count=1, struct_detail=None, **sub_struct_detail):
         return self.get_port_value(env_name, instance_name, port_name,
                                    mrt_port_type_t.MRT_OUTPUT_PORT, signal_data_type, item_count, struct_detail, **sub_struct_detail)
 
-    def get_measurement_value(self, env_name, instance_name, port_name, signal_data_type, item_count, struct_detail=None, **sub_struct_detail):
+    def get_measurement_value(self, env_name, instance_name, port_name, signal_data_type, item_count=1, struct_detail=None, **sub_struct_detail):
         return self.get_port_value(env_name, instance_name, port_name,
                                     mrt_port_type_t.MRT_MEASUREMENT, signal_data_type, item_count, struct_detail, **sub_struct_detail)
 
-    def get_port_value(self, env_name, instance_name, port_name, port_type, signal_data_type,  item_count, struct_detail, **sub_struct_detail):
+    def get_port_value(self, env_name, instance_name, port_name, port_type, signal_data_type,
+                       item_count, struct_detail, **sub_struct_detail):
         en_bs = env_name.encode('utf-8')
         en_pointer = c_char_p(en_bs)
         in_bs = instance_name.encode('utf-8')
         in_pointer = c_char_p(in_bs)
         pn_bs = port_name.encode('utf-8')
         pn_pointer = c_char_p(pn_bs)
 
@@ -263,22 +264,30 @@
         in_bs = instance_name.encode('utf-8')
         in_pointer = c_char_p(in_bs)
         pn_bs = port_name.encode('utf-8')
         pn_pointer = c_char_p(pn_bs)
 
         python_bytes = kunyi_util.data_to_bytes(signal_type, signal_value, item_count,
                                                 struct_detail, **sub_struct_detail)
-        arr = bytearray.fromhex(python_bytes.hex())
-        char_array = c_char * len(arr)
-        buf_c = char_array.from_buffer(arr)
+        if signal_type  in ["ASCII", "UTF8"]:
+            if len(python_bytes) >= 512:
+                return mrt_status_t.MRT_ERR_INVALID_ARG, None
+            end = b'\0' * (512-len(python_bytes))
+            python_bytes = python_bytes + end
+
+            buf_c = c_char_p(python_bytes)
+            buf_size = 512
+        else:
+            arr = bytearray.fromhex(python_bytes.hex())
+            char_array = c_char * len(arr)
+            buf_c = char_array.from_buffer(arr)
+            buf_size = len(arr)
+            if buf_size == None:
+                return mrt_status_t.MRT_ERR_INVALID_ARG, None
 
-        buf_size = kunyi_util.get_signal_bytes_length(signal_type, item_count,
-                                                      struct_detail, **sub_struct_detail)
-        if buf_size == None:
-            return mrt_status_t.MRT_ERR_INVALID_ARG, None
 
         mrt_lib.mrt_model_write_port.argtypes = [c_void_p, c_char_p, c_char_p, c_char_p,
                                                  c_int32, c_int32, c_int32, c_void_p]
         mrt_lib.mrt_model_write_port.restype = c_int32
         rc = mrt_lib.mrt_model_write_port(self.context, en_pointer, in_pointer, pn_pointer,
                                           port_type[0], 0, buf_size, buf_c)
         return rc
@@ -907,15 +916,17 @@
         mrt_lib.mrt_gen_clr_port_event.restype = mrt_status_t
         error_code = mrt_lib.mrt_gen_clr_port_event(self.context, en_pointer, c_uint64(gen_handle), c_uint32(port_index))
         return error_code
 
     def gen_write_port(self, env_name, gen_handle, port_index, data, data_type, time_interval_ms):
         bs = env_name.encode('utf-8')
         en_pointer = c_char_p(bs)
-        python_bytes = kunyi_util.data_to_bytes(data_type, data, len(data))
+        python_bytes = b''
+        for i in range(len(data)):
+            python_bytes = python_bytes + kunyi_util.data_to_bytes(data_type, data[i], 1)
         arr = bytearray.fromhex(python_bytes.hex())
         char_array = c_char * len(arr)
         buf_c = char_array.from_buffer(arr)
 
         mrt_lib.mrt_gen_write_port.argtypes = [c_void_p, c_char_p, c_uint64, c_uint32,c_void_p,c_uint32,c_uint32]
         mrt_lib.mrt_gen_write_port.restype = c_int32
         res = mrt_lib.mrt_gen_write_port(self.context, en_pointer, c_uint64(gen_handle), c_uint32(port_index)
```

### Comparing `vcarhilclient-1.0.526/vcarhilclient/kunyi_project.py` & `vcarhilclient-1.0.531/vcarhilclient/kunyi_project.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.526/vcarhilclient/kunyi_util.py` & `vcarhilclient-1.0.531/vcarhilclient/kunyi_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
                      "UInt8": 1,
                      "UInt16": 2,
                      "UInt32": 4,
                      "UInt64": 8,
                      "Float": 4,
                      "Double": 8,
                      "Bool": 1,
-                     "ASCII": 1,
-                     "UTF8": 2}
+                     "ASCII": 512,
+                     "UTF8": 512}
 
         if signal_type == "Struct":
             if struct_detail == None:
                 raise Exception("No struct detail for counting the length")
             total_length = 0
             for member in struct_detail["Member"]:
                 if member["Type"] == "Struct":
@@ -106,17 +106,18 @@
 
             for i in range(item_count):
                 bytes_sub = bytes_data[i*single_length:(i+1)*single_length]
                 if datatype in decode_charactor:
                     value = struct.unpack(decode_charactor[datatype],
                                           bytes_sub)[0]
                 elif datatype == "ASCII":
-                    value = bytes_sub.decode("ascii")
+                    value = bytes_sub.decode("ascii").strip('\x00')
                 elif datatype == "UTF8":
-                    value = bytes_sub.decode("utf-8")
+                    value = bytes_sub.decode("utf-8").strip('\x00')
+
                 all_values.append(value)
             if item_count == 1:
                 return all_values[0]
             return all_values
 
 
     @staticmethod
@@ -197,16 +198,15 @@
                     elif datatype == "UTF8":
                         bytes_result = bytes_result + data_value[mi].encode("utf-8")
                         break
                     else:
                         raise Exception("Unsupportted type for counting the bytes")
             else:
                 value = data_value
-                if isinstance(data_value, collections.abc.Sequence):
-                    value = data_value[0]
+
                 if datatype in decode_charactor:
                     bytes_result = bytes_result + struct.pack(decode_charactor[datatype], value)
                 elif datatype == "ASCII":
                     bytes_result = bytes_result + value.encode("ascii")
                 elif datatype == "UTF8":
                     bytes_result = bytes_result + value.encode("utf-8")
                 else:
```

### Comparing `vcarhilclient-1.0.526/vcarhilclient/minio_handld.py` & `vcarhilclient-1.0.531/vcarhilclient/minio_handld.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.526/vcarhilclient/mrt_strunctures.py` & `vcarhilclient-1.0.531/vcarhilclient/mrt_strunctures.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.526/vcarhilclient/signal_daq.py` & `vcarhilclient-1.0.531/vcarhilclient/signal_daq.py`

 * *Files identical despite different names*

### Comparing `vcarhilclient-1.0.526/vcarhilclient.egg-info/PKG-INFO` & `vcarhilclient-1.0.531/vcarhilclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: vcarhilclient
-Version: 1.0.526
+Version: 1.0.531
 Summary: vcarhilclient
-Home-page: 
+Home-page: UNKNOWN
 Author: vcarsystem
 Author-email: service@vcarsystem.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -105,7 +107,9 @@
 assert ec.value == 0
 
 # 18.Delete the experiment
 ec = my_mrt.delete_test_env("envName")
 
 assert ec.value == 0
 
+
+
```

