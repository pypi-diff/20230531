# Comparing `tmp/lib_for_messanger-0.3.tar.gz` & `tmp/lib_for_messanger-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_for_messanger-0.3.tar", last modified: Wed May 31 16:25:35 2023, max compression
+gzip compressed data, was "lib_for_messanger-0.4.tar", last modified: Wed May 31 19:19:19 2023, max compression
```

## Comparing `lib_for_messanger-0.3.tar` & `lib_for_messanger-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.3/README.md
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/lib_for_messanger/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.3/lib_for_messanger/__init__.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)     1371 2023-05-31 15:33:04.000000 lib_for_messanger-0.3/lib_for_messanger/chat.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 00:43:42.000000 lib_for_messanger-0.3/lib_for_messanger/file_service.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-0.3/lib_for_messanger/message.py
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      786 2023-05-31 00:43:42.000000 lib_for_messanger-0.3/lib_for_messanger/user.py
-drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/lib_for_messanger.egg-info/
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 16:25:35.000000 lib_for_messanger-0.3/lib_for_messanger.egg-info/PKG-INFO
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-05-31 16:25:35.000000 lib_for_messanger-0.3/lib_for_messanger.egg-info/SOURCES.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-05-31 16:25:35.000000 lib_for_messanger-0.3/lib_for_messanger.egg-info/dependency_links.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-05-31 16:25:35.000000 lib_for_messanger-0.3/lib_for_messanger.egg-info/top_level.txt
--rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-05-31 16:25:35.201420 lib_for_messanger-0.3/setup.cfg
--rw-rw-r--   0 kirill    (1000) kirill    (1000)      479 2023-05-31 16:25:26.000000 lib_for_messanger-0.3/setup.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 19:19:19.787801 lib_for_messanger-0.4/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 19:19:19.787801 lib_for_messanger-0.4/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       25 2023-05-31 00:47:59.000000 lib_for_messanger-0.4/README.md
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 19:19:19.787801 lib_for_messanger-0.4/lib_for_messanger/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      113 2023-05-31 00:43:42.000000 lib_for_messanger-0.4/lib_for_messanger/__init__.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)     1371 2023-05-31 15:33:04.000000 lib_for_messanger-0.4/lib_for_messanger/chat.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      918 2023-05-31 19:15:38.000000 lib_for_messanger-0.4/lib_for_messanger/file_service.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      963 2023-05-31 16:17:51.000000 lib_for_messanger-0.4/lib_for_messanger/message.py
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      786 2023-05-31 00:43:42.000000 lib_for_messanger-0.4/lib_for_messanger/user.py
+drwxrwxr-x   0 kirill    (1000) kirill    (1000)        0 2023-05-31 19:19:19.787801 lib_for_messanger-0.4/lib_for_messanger.egg-info/
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      355 2023-05-31 19:19:19.000000 lib_for_messanger-0.4/lib_for_messanger.egg-info/PKG-INFO
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      327 2023-05-31 19:19:19.000000 lib_for_messanger-0.4/lib_for_messanger.egg-info/SOURCES.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)        1 2023-05-31 19:19:19.000000 lib_for_messanger-0.4/lib_for_messanger.egg-info/dependency_links.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       18 2023-05-31 19:19:19.000000 lib_for_messanger-0.4/lib_for_messanger.egg-info/top_level.txt
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)       38 2023-05-31 19:19:19.787801 lib_for_messanger-0.4/setup.cfg
+-rw-rw-r--   0 kirill    (1000) kirill    (1000)      478 2023-05-31 19:18:14.000000 lib_for_messanger-0.4/setup.py
```

### Comparing `lib_for_messanger-0.3/lib_for_messanger/chat.py` & `lib_for_messanger-0.4/lib_for_messanger/chat.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.3/lib_for_messanger/file_service.py` & `lib_for_messanger-0.4/lib_for_messanger/file_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,25 @@
     def __init__(self, file_path, data_list, object_class):
         path = os.path.join(file_path)
 
         self.__file_path = file_path
         self.__data_list = data_list
 
         if not os.path.isfile(path):
-            my_file = open(file_path, "w+")
+            my_file = open(file_path, "w")
             my_file.write("[]")
             my_file.close()
         else:
             with open(self.__file_path, "r") as file:
                 json_array = json.load(file)
                 for json_object in json_array:
                     self.__data_list.append(object_class.from_json_object(json_object))
 
                 print(self.__data_list)
 
     def save_data(self):
-        with open(self.__file_path, "r+") as file:
+        with open(self.__file_path, "w") as file:
             json_array = []
             for el in self.__data_list:
                 json_array.append(el.to_json_object())
-            print(json_array)
+            # print(json_array)
             json.dump(json_array, file)
```

### Comparing `lib_for_messanger-0.3/lib_for_messanger/message.py` & `lib_for_messanger-0.4/lib_for_messanger/message.py`

 * *Files identical despite different names*

### Comparing `lib_for_messanger-0.3/lib_for_messanger/user.py` & `lib_for_messanger-0.4/lib_for_messanger/user.py`

 * *Files identical despite different names*

