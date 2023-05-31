# Comparing `tmp/lib_for_messanger-0.1.tar.gz` & `tmp/lib_for_messanger-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_for_messanger-0.1.tar", last modified: Wed May 31 01:06:53 2023, max compression
+gzip compressed data, was "lib_for_messanger-0.2.tar", last modified: Wed May 31 15:47:04 2023, max compression
```

## Comparing `lib_for_messanger-0.1.tar` & `lib_for_messanger-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 01:06:53.490088 lib_for_messanger-0.1/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      400 2023-05-31 01:06:53.490088 lib_for_messanger-0.1/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.1/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 01:06:53.490088 lib_for_messanger-0.1/lib_for_messanger/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.1/lib_for_messanger/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1370 2023-05-31 00:43:42.000000 lib_for_messanger-0.1/lib_for_messanger/chat.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 00:43:42.000000 lib_for_messanger-0.1/lib_for_messanger/file_service.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      893 2023-05-31 00:43:42.000000 lib_for_messanger-0.1/lib_for_messanger/message.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      786 2023-05-31 00:43:42.000000 lib_for_messanger-0.1/lib_for_messanger/user.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 01:06:53.490088 lib_for_messanger-0.1/lib_for_messanger.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      400 2023-05-31 01:06:53.000000 lib_for_messanger-0.1/lib_for_messanger.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-05-31 01:06:53.000000 lib_for_messanger-0.1/lib_for_messanger.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-05-31 01:06:53.000000 lib_for_messanger-0.1/lib_for_messanger.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-05-31 01:06:53.000000 lib_for_messanger-0.1/lib_for_messanger.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-05-31 01:06:53.490088 lib_for_messanger-0.1/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      479 2023-05-31 01:03:16.000000 lib_for_messanger-0.1/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 15:47:04.143905 lib_for_messanger-0.2/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 15:47:04.143905 lib_for_messanger-0.2/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.2/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 15:47:04.139905 lib_for_messanger-0.2/lib_for_messanger/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.2/lib_for_messanger/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1371 2023-05-31 15:33:04.000000 lib_for_messanger-0.2/lib_for_messanger/chat.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 00:43:42.000000 lib_for_messanger-0.2/lib_for_messanger/file_service.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      893 2023-05-31 00:43:42.000000 lib_for_messanger-0.2/lib_for_messanger/message.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      786 2023-05-31 00:43:42.000000 lib_for_messanger-0.2/lib_for_messanger/user.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 15:47:04.143905 lib_for_messanger-0.2/lib_for_messanger.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 15:47:04.000000 lib_for_messanger-0.2/lib_for_messanger.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-05-31 15:47:04.000000 lib_for_messanger-0.2/lib_for_messanger.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-05-31 15:47:04.000000 lib_for_messanger-0.2/lib_for_messanger.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-05-31 15:47:04.000000 lib_for_messanger-0.2/lib_for_messanger.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-05-31 15:47:04.143905 lib_for_messanger-0.2/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      479 2023-05-31 15:35:33.000000 lib_for_messanger-0.2/setup.py
```

### Comparing `lib_for_messanger-0.1/lib_for_messanger/chat.py` & `lib_for_messanger-0.2/lib_for_messanger/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,11 +34,11 @@
     def from_json_object(json_object):
         chat = Chat("", "", "")
 
         chat.__chat_name = json_object["chat_name"]
         chat.__chat_admin_name = json_object["chat_admin_name"]
         chat.__chat_password = json_object["chat_password"]
         chat.__members = json_object["chat_admin_name"]
-        chat.__messages_id = json_object["message_id"]
+        chat.__messages_id = json_object["messages_id"]
 
         return chat
```

### Comparing `lib_for_messanger-0.1/lib_for_messanger/file_service.py` & `lib_for_messanger-0.2/lib_for_messanger/file_service.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.1/lib_for_messanger/message.py` & `lib_for_messanger-0.2/lib_for_messanger/message.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.1/lib_for_messanger/user.py` & `lib_for_messanger-0.2/lib_for_messanger/user.py`

 * *Files identical despite different names*

