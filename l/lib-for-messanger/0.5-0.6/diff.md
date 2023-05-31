# Comparing `tmp/lib_for_messanger-0.5.tar.gz` & `tmp/lib_for_messanger-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_for_messanger-0.5.tar", last modified: Wed May 31 19:44:49 2023, max compression
+gzip compressed data, was "lib_for_messanger-0.6.tar", last modified: Wed May 31 20:14:36 2023, max compression
```

## Comparing `lib_for_messanger-0.5.tar` & `lib_for_messanger-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 19:44:49.518699 lib_for_messanger-0.5/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 19:44:49.518699 lib_for_messanger-0.5/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.5/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 19:44:49.518699 lib_for_messanger-0.5/lib_for_messanger/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.5/lib_for_messanger/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1363 2023-05-31 19:41:07.000000 lib_for_messanger-0.5/lib_for_messanger/chat.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 19:15:38.000000 lib_for_messanger-0.5/lib_for_messanger/file_service.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-0.5/lib_for_messanger/message.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      786 2023-05-31 00:43:42.000000 lib_for_messanger-0.5/lib_for_messanger/user.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 19:44:49.518699 lib_for_messanger-0.5/lib_for_messanger.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 19:44:49.000000 lib_for_messanger-0.5/lib_for_messanger.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-05-31 19:44:49.000000 lib_for_messanger-0.5/lib_for_messanger.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-05-31 19:44:49.000000 lib_for_messanger-0.5/lib_for_messanger.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-05-31 19:44:49.000000 lib_for_messanger-0.5/lib_for_messanger.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-05-31 19:44:49.518699 lib_for_messanger-0.5/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      478 2023-05-31 19:42:27.000000 lib_for_messanger-0.5/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 20:14:36.886939 lib_for_messanger-0.6/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 20:14:36.886939 lib_for_messanger-0.6/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.6/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 20:14:36.886939 lib_for_messanger-0.6/lib_for_messanger/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.6/lib_for_messanger/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1363 2023-05-31 19:41:07.000000 lib_for_messanger-0.6/lib_for_messanger/chat.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 19:15:38.000000 lib_for_messanger-0.6/lib_for_messanger/file_service.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-0.6/lib_for_messanger/message.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      784 2023-05-31 20:12:00.000000 lib_for_messanger-0.6/lib_for_messanger/user.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 20:14:36.886939 lib_for_messanger-0.6/lib_for_messanger.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 20:14:36.000000 lib_for_messanger-0.6/lib_for_messanger.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-05-31 20:14:36.000000 lib_for_messanger-0.6/lib_for_messanger.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-05-31 20:14:36.000000 lib_for_messanger-0.6/lib_for_messanger.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-05-31 20:14:36.000000 lib_for_messanger-0.6/lib_for_messanger.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-05-31 20:14:36.886939 lib_for_messanger-0.6/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      478 2023-05-31 20:12:55.000000 lib_for_messanger-0.6/setup.py
```

### Comparing `lib_for_messanger-0.5/lib_for_messanger/chat.py` & `lib_for_messanger-0.6/lib_for_messanger/chat.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.5/lib_for_messanger/file_service.py` & `lib_for_messanger-0.6/lib_for_messanger/file_service.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.5/lib_for_messanger/message.py` & `lib_for_messanger-0.6/lib_for_messanger/message.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.5/lib_for_messanger/user.py` & `lib_for_messanger-0.6/lib_for_messanger/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,10 +22,10 @@
                 "chats": self.__chats}
 
     @staticmethod
     def from_json_object(json_object):
         user = User("", "")
         user.__name = json_object["name"]
         user.__password = json_object["password"]
-        user.__chatsId = json_object["chats"]
+        user.__chats = json_object["chats"]
 
         return user
```

