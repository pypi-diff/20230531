# Comparing `tmp/lib_for_messanger-0.2.tar.gz` & `tmp/lib_for_messanger-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_for_messanger-0.2.tar", last modified: Wed May 31 15:47:04 2023, max compression
+gzip compressed data, was "lib_for_messanger-0.3.tar", last modified: Wed May 31 16:25:35 2023, max compression
```

## Comparing `lib_for_messanger-0.2.tar` & `lib_for_messanger-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 15:47:04.143905 lib_for_messanger-0.2/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 15:47:04.143905 lib_for_messanger-0.2/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.2/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 15:47:04.139905 lib_for_messanger-0.2/lib_for_messanger/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.2/lib_for_messanger/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1371 2023-05-31 15:33:04.000000 lib_for_messanger-0.2/lib_for_messanger/chat.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 00:43:42.000000 lib_for_messanger-0.2/lib_for_messanger/file_service.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      893 2023-05-31 00:43:42.000000 lib_for_messanger-0.2/lib_for_messanger/message.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      786 2023-05-31 00:43:42.000000 lib_for_messanger-0.2/lib_for_messanger/user.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 15:47:04.143905 lib_for_messanger-0.2/lib_for_messanger.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 15:47:04.000000 lib_for_messanger-0.2/lib_for_messanger.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-05-31 15:47:04.000000 lib_for_messanger-0.2/lib_for_messanger.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-05-31 15:47:04.000000 lib_for_messanger-0.2/lib_for_messanger.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-05-31 15:47:04.000000 lib_for_messanger-0.2/lib_for_messanger.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-05-31 15:47:04.143905 lib_for_messanger-0.2/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      479 2023-05-31 15:35:33.000000 lib_for_messanger-0.2/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.3/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/lib_for_messanger/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.3/lib_for_messanger/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1371 2023-05-31 15:33:04.000000 lib_for_messanger-0.3/lib_for_messanger/chat.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 00:43:42.000000 lib_for_messanger-0.3/lib_for_messanger/file_service.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-0.3/lib_for_messanger/message.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      786 2023-05-31 00:43:42.000000 lib_for_messanger-0.3/lib_for_messanger/user.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/lib_for_messanger.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 16:25:35.000000 lib_for_messanger-0.3/lib_for_messanger.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-05-31 16:25:35.000000 lib_for_messanger-0.3/lib_for_messanger.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-05-31 16:25:35.000000 lib_for_messanger-0.3/lib_for_messanger.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-05-31 16:25:35.000000 lib_for_messanger-0.3/lib_for_messanger.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      479 2023-05-31 16:25:26.000000 lib_for_messanger-0.3/setup.py
```

### Comparing `lib_for_messanger-0.2/lib_for_messanger/chat.py` & `lib_for_messanger-0.3/lib_for_messanger/chat.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.2/lib_for_messanger/file_service.py` & `lib_for_messanger-0.3/lib_for_messanger/file_service.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.2/lib_for_messanger/message.py` & `lib_for_messanger-0.3/lib_for_messanger/message.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,18 +14,18 @@
         return self.__send_date
 
     def get_message_text(self):
         return self.__message_text
 
     def to_json_object(self):
         return {"sender_name": self.__sender_name,
-                "send_date": self.__send_date,
+                "send_date": self.__send_date.strftime("%Y-%m-%d %H:%M:%S"),
                 "message_text": self.__message_text}
 
     @staticmethod
     def from_json_object(json_object):
         message = Message("", "")
         message.__sender_name = json_object["sender_name"]
-        message.__send_date = json_object["send_date"]
+        message.__send_date = datetime.strptime(json_object["send_date"], "%Y-%m-%d %H:%M:%S")
         message.__message_text = json_object["message_text"]
 
         return message
```

### Comparing `lib_for_messanger-0.2/lib_for_messanger/user.py` & `lib_for_messanger-0.3/lib_for_messanger/user.py`

 * *Files identical despite different names*

