# Comparing `tmp/ixcom-1.3.5.tar.gz` & `tmp/ixcom-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixcom-1.3.5.tar", last modified: Tue May  2 09:54:36 2023, max compression
+gzip compressed data, was "ixcom-1.3.6.tar", last modified: Wed May 31 12:13:42 2023, max compression
```

## Comparing `ixcom-1.3.5.tar` & `ixcom-1.3.6.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:54:36.542463 ixcom-1.3.5/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-05-02 09:54:00.000000 ixcom-1.3.5/LICENSE
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       22 2023-05-02 09:54:00.000000 ixcom-1.3.5/MANIFEST.in
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-05-02 09:54:36.542463 ixcom-1.3.5/PKG-INFO
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-05-02 09:54:00.000000 ixcom-1.3.5/README.md
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:54:36.542463 ixcom-1.3.5/ixcom/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/__init__.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     9498 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/cmdline.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/commands.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/crc16.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/data.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/exceptions.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/grep.py
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:54:36.538463 ixcom-1.3.5/ixcom/json-files/
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:54:36.542463 ixcom-1.3.5/ixcom/json-files/messages/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2982 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/json-files/messages/0x03_inssol.json
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:54:36.542463 ixcom-1.3.5/ixcom/json-files/parameters/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     4978 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/json-files/parameters/0731_parekf_startupv2.json
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8082 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/json-files/parameters/0760_parekf_imuconfig2.json
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/messages.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/parameters.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    71125 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/parser.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/plugin_messages.py
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42576 2023-05-02 09:54:00.000000 ixcom-1.3.5/ixcom/protocol.py
-drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-02 09:54:36.542463 ixcom-1.3.5/ixcom.egg-info/
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-05-02 09:54:36.000000 ixcom-1.3.5/ixcom.egg-info/PKG-INFO
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      581 2023-05-02 09:54:36.000000 ixcom-1.3.5/ixcom.egg-info/SOURCES.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-05-02 09:54:36.000000 ixcom-1.3.5/ixcom.egg-info/dependency_links.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      189 2023-05-02 09:54:36.000000 ixcom-1.3.5/ixcom.egg-info/entry_points.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-05-02 09:54:36.000000 ixcom-1.3.5/ixcom.egg-info/requires.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-05-02 09:54:36.000000 ixcom-1.3.5/ixcom.egg-info/top_level.txt
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-05-02 09:54:36.542463 ixcom-1.3.5/setup.cfg
--rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2010 2023-05-02 09:54:00.000000 ixcom-1.3.5/setup.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-31 12:13:42.598461 ixcom-1.3.6/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-05-31 12:10:58.000000 ixcom-1.3.6/LICENSE
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       22 2023-05-31 12:10:58.000000 ixcom-1.3.6/MANIFEST.in
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-05-31 12:13:42.598461 ixcom-1.3.6/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-05-31 12:10:58.000000 ixcom-1.3.6/README.md
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-31 12:13:42.598461 ixcom-1.3.6/ixcom/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/__init__.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    10380 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/cmdline.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/commands.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/crc16.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/data.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/exceptions.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/grep.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-31 12:13:42.594461 ixcom-1.3.6/ixcom/json-files/
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-31 12:13:42.598461 ixcom-1.3.6/ixcom/json-files/messages/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2982 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/json-files/messages/0x03_inssol.json
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     4828 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/json-files/messages/0x9A_ekfstddev3.json
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-31 12:13:42.598461 ixcom-1.3.6/ixcom/json-files/parameters/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     4978 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/json-files/parameters/0731_parekf_startupv2.json
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8082 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/json-files/parameters/0760_parekf_imuconfig2.json
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/parameters.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    71385 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/parser.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/plugin_messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42598 2023-05-31 12:10:58.000000 ixcom-1.3.6/ixcom/protocol.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-05-31 12:13:42.598461 ixcom-1.3.6/ixcom.egg-info/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-05-31 12:13:42.000000 ixcom-1.3.6/ixcom.egg-info/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      628 2023-05-31 12:13:42.000000 ixcom-1.3.6/ixcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-05-31 12:13:42.000000 ixcom-1.3.6/ixcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      250 2023-05-31 12:13:42.000000 ixcom-1.3.6/ixcom.egg-info/entry_points.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-05-31 12:13:42.000000 ixcom-1.3.6/ixcom.egg-info/requires.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-05-31 12:13:42.000000 ixcom-1.3.6/ixcom.egg-info/top_level.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-05-31 12:13:42.598461 ixcom-1.3.6/setup.cfg
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2098 2023-05-31 12:10:58.000000 ixcom-1.3.6/setup.py
```

### Comparing `ixcom-1.3.5/LICENSE` & `ixcom-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/PKG-INFO` & `ixcom-1.3.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.3.5
+Version: 1.3.6
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
```

### Comparing `ixcom-1.3.5/README.md` & `ixcom-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/cmdline.py` & `ixcom-1.3.6/ixcom/cmdline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import ixcom
 import time
 import sys
 import struct
 import argparse
 import socket
+import io
+import os
 
 
 class TextFileParser(ixcom.parser.MessageParser):
     def __init__(self, outputfile, skip_parameter=list(), print_request = True):
         super().__init__()
         self.ignore_output = False
         self.outputfile = outputfile
@@ -212,7 +214,25 @@
             
         xcomparser.add_callback(callback)
         xcomparser.process_bytes(args.inputfile.read())
         sys.exit(0)
     except Exception as ex:
         print(ex)
         sys.exit(1)
+
+def remove_partial_msgs(argv = None):
+    parser = argparse.ArgumentParser(description='Removes Partial Messages from XCOMStream')
+    parser.add_argument('inputfile', metavar='inputfile', type=argparse.FileType('rb'), nargs='?',
+                       help='Name of the binary XCOMStream file', default = 'XCOMStream.bin')
+    parser.add_argument('-o', '--output', metavar='output_filename', type=argparse.FileType(mode='wb'),
+                       help='Filename of the output file', default = 'XCOMStream.clean.bin')  
+    args = parser.parse_args()
+    xcomparser = ixcom.parser.MessageSearcher(disable_crc = False)
+
+    iob = io.BytesIO(b'')
+    def r_callback(in_bytes):
+        iob.write(in_bytes)
+
+    xcomparser.add_callback(r_callback)
+    xcomparser.process_bytes(args.inputfile.read())
+    iob.seek(0, os.SEEK_SET)
+    args.output.write(iob.read())
```

### Comparing `ixcom-1.3.5/ixcom/commands.py` & `ixcom-1.3.6/ixcom/commands.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/crc16.py` & `ixcom-1.3.6/ixcom/crc16.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/grep.py` & `ixcom-1.3.6/ixcom/grep.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/json-files/messages/0x03_inssol.json` & `ixcom-1.3.6/ixcom/json-files/messages/0x03_inssol.json`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/json-files/parameters/0731_parekf_startupv2.json` & `ixcom-1.3.6/ixcom/json-files/parameters/0731_parekf_startupv2.json`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/json-files/parameters/0760_parekf_imuconfig2.json` & `ixcom-1.3.6/ixcom/json-files/parameters/0760_parekf_imuconfig2.json`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/messages.py` & `ixcom-1.3.6/ixcom/messages.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/parameters.py` & `ixcom-1.3.6/ixcom/parameters.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.3.5/ixcom/parser.py` & `ixcom-1.3.6/ixcom/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,22 +46,28 @@
             return 0
         else:
             json_hdr_len_pos = 7*4
             return int.from_bytes(inBytes[json_hdr_len_pos:json_hdr_len_pos+4], byteorder='little')
 
     def process_buffer_unsafe(self, buffer):
         current_msg_start_idx = 0
+        last_msg_start_id = -1
         inBytes = memoryview(buffer)
         inbytelen = len(inBytes)
         current_msg_start_idx = self.handle_v5_json(inBytes)
         while current_msg_start_idx + 5 < inbytelen:
+            
             current_msg_length = inBytes[current_msg_start_idx + 4] + 256*inBytes[current_msg_start_idx + 5]
+
             if current_msg_start_idx + current_msg_length > inbytelen: # Message nicht mehr komplett
                 break
             self.publish(inBytes[current_msg_start_idx:current_msg_start_idx+current_msg_length])
+            if current_msg_start_idx <= last_msg_start_id:
+                raise Exception("File is corrupted, try xcom-remove-partial-msgs on XCOMStream file")
+            last_msg_start_id = current_msg_start_idx
             current_msg_start_idx += current_msg_length
 
     def process_bytes(self, inBytes):
         inByteIdx = 0
         while inByteIdx < len(inBytes):
             if self.searcherState == MessageSearcherState.waiting_for_sync:
                 poppedByte = inBytes[inByteIdx]
@@ -763,17 +769,17 @@
 
         Raises:
             ClientTimeoutError: Timeout while waiting for response from the XCOM server
             ResponseError: The response from the system was not 'OK'.
 
         '''
         msgToSend = data.getCommandWithID(data.CMD_LOG_Payload.command_id)
-        msgToSend.payload.data['messageID'] = 3
+        msgToSend.payload.data['messageID'] = msgID
         msgToSend.payload.data['trigger'] = data.LogTrigger.SYNC
-        msgToSend.payload.data['parameter'] = data.LogCommand.CLEAR_ALL
+        msgToSend.payload.data['parameter'] = data.LogCommand.CLEAR
         msgToSend.payload.data['divider'] = 1
         self.send_msg_and_waitfor_okay(msgToSend)
 
     def poll_log(self, msgID):
         '''Polls a log
 
         Polls a log with a specified message ID. Blocks until the log is retrieved and returns
```

### Comparing `ixcom-1.3.5/ixcom/protocol.py` & `ixcom-1.3.6/ixcom/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,22 +841,22 @@
         def build_dtype_list(data, item_list):
             dtype_list = []
             idx_offset = 0
             for idx, fieldname in enumerate(data.keys()):
                 item = item_list[idx+idx_offset]
                 is_nested = False
                 is_nested_list = False
-                is_empty_nested_list = False
+                is_empty_list = False
                 if (type(data[fieldname]) is type(list())):
                     if data[fieldname]:
                         if (type(data[fieldname][0]) is type(dict())):
                             is_nested = True
                             is_nested_list = True
                     else:
-                        is_empty_nested_list = True
+                        is_empty_list = True
                 else:
                     if (type(data[fieldname]) is type(dict())):
                         is_nested = True
                 if is_nested:
                     if is_nested_list:
                         sublist_length = len(data[fieldname][0])
                         dtype_sublist, nested_offset = build_dtype_list(data[fieldname][0],
@@ -866,16 +866,17 @@
                         item_spec = (fieldname, dtype_sublist, nestet_list_length)
                     else:
                         sublist_length = len(data[fieldname])
                         dtype_sublist, nested_offset = build_dtype_list(data[fieldname],
                             item_list[idx+idx_offset:])
                         idx_offset += sublist_length - 1 + nested_offset
                         item_spec = (fieldname, dtype_sublist)
-                elif is_empty_nested_list:
-                    idx_offset -= 1
+                elif is_empty_list:
+                    if item[0] != "0":
+                        idx_offset -= 1
                     item_spec = (fieldname, list())
                 else:
                     item_spec = construct_item_spec_from_msg_def(fieldname, item)
                 dtype_list.append(item_spec)
             return dtype_list, idx_offset
         
         return build_dtype_list(self.data, item_list)[0]
```

### Comparing `ixcom-1.3.5/ixcom.egg-info/PKG-INFO` & `ixcom-1.3.6/ixcom.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.3.5
+Version: 1.3.6
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
```

### Comparing `ixcom-1.3.5/ixcom.egg-info/SOURCES.txt` & `ixcom-1.3.6/ixcom.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,9 +17,10 @@
 ixcom.egg-info/PKG-INFO
 ixcom.egg-info/SOURCES.txt
 ixcom.egg-info/dependency_links.txt
 ixcom.egg-info/entry_points.txt
 ixcom.egg-info/requires.txt
 ixcom.egg-info/top_level.txt
 ixcom/json-files/messages/0x03_inssol.json
+ixcom/json-files/messages/0x9A_ekfstddev3.json
 ixcom/json-files/parameters/0731_parekf_startupv2.json
 ixcom/json-files/parameters/0760_parekf_imuconfig2.json
```

### Comparing `ixcom-1.3.5/setup.py` & `ixcom-1.3.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 
 if __name__ == '__main__':
 
     readmePath = os.path.join(os.path.dirname(__file__), 'README.md')
     long_description = open(readmePath, "rt").read()
 
     setup(name='ixcom',
-          version='1.3.5',
+          version='1.3.6',
           description='Library for communicating with xcom devices over network',
           author='iMAR Navigation GmbH',
           author_email='support@imar-navigation.de',
           url='http://www.imar-navigation.de',
           keywords=['XCOM', 'Inertial navigation', 'INS', 'iMAR', 'iNAT', 'GNSS', 'GPS', 'AHRS'],
           packages=['ixcom'],
           package_data={'': ['ixcom/messages/*.json', 'ixcom/parameters/*.json']},
           include_package_data=True,
           entry_points={
             'console_scripts': [
                         'configdump2txt = ixcom.cmdline:configdump2txt',
                         'monitor2xcom = ixcom.cmdline:monitor2xcom',
                         'xcom_lookup = ixcom.cmdline:xcom_lookup',
                         'split_config = ixcom.cmdline:split_config',
+                        'xcom-remove-partial-msgs = ixcom.cmdline:remove_partial_msgs',
                                 ],
                         },
           install_requires=[
                     'numpy>=1.16.2',
                 ],
           extras_require={
                     'fastcrc': ['fastcrc']
```

