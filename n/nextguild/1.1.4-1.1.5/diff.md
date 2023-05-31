# Comparing `tmp/nextguild-1.1.4.tar.gz` & `tmp/nextguild-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.1.4.tar", last modified: Wed May 17 13:18:14 2023, max compression
+gzip compressed data, was "nextguild-1.1.5.tar", last modified: Wed May 31 09:33:38 2023, max compression
```

## Comparing `nextguild-1.1.4.tar` & `nextguild-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:18:14.220418 nextguild-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 13:18:01.000000 nextguild-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-17 13:18:14.220418 nextguild-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-17 13:18:01.000000 nextguild-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:18:14.220418 nextguild-1.1.4/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    38255 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-17 13:18:01.000000 nextguild-1.1.4/nextguild/reaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:18:14.220418 nextguild-1.1.4/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-17 13:18:14.000000 nextguild-1.1.4/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-17 13:18:14.000000 nextguild-1.1.4/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:18:14.000000 nextguild-1.1.4/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 13:18:14.000000 nextguild-1.1.4/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-17 13:18:01.000000 nextguild-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:18:14.220418 nextguild-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:33:38.419720 nextguild-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 09:33:23.000000 nextguild-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-31 09:33:38.419720 nextguild-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-31 09:33:23.000000 nextguild-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:33:38.419720 nextguild-1.1.5/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 09:33:23.000000 nextguild-1.1.5/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-31 09:33:23.000000 nextguild-1.1.5/nextguild/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40968 2023-05-31 09:33:23.000000 nextguild-1.1.5/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-31 09:33:23.000000 nextguild-1.1.5/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-31 09:33:23.000000 nextguild-1.1.5/nextguild/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-31 09:33:23.000000 nextguild-1.1.5/nextguild/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-31 09:33:23.000000 nextguild-1.1.5/nextguild/reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:33:38.419720 nextguild-1.1.5/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-31 09:33:38.000000 nextguild-1.1.5/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-31 09:33:38.000000 nextguild-1.1.5/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:33:38.000000 nextguild-1.1.5/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:33:38.000000 nextguild-1.1.5/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-31 09:33:23.000000 nextguild-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:33:38.419720 nextguild-1.1.5/setup.cfg
```

### Comparing `nextguild-1.1.4/LICENSE` & `nextguild-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.4/PKG-INFO` & `nextguild-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.4
+Version: 1.1.5
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.1.4/README.md` & `nextguild-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.4/nextguild/channel.py` & `nextguild-1.1.5/nextguild/channel.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.4/nextguild/client.py` & `nextguild-1.1.5/nextguild/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,23 +184,29 @@
     def create_channel(
             self,
             name: str,
             channel_type,
             server_id: str,
             group_id: str = None,
             category_id: int = None,
-            is_public: bool = False
+            is_public: bool = False,
+            parent_id: str = None,
+            message_id: str = None
     ):
         data = {'name': name, 'type': channel_type}
         if category_id:
             data.update({'categoryId': category_id})
         if group_id:
             data.update({'group_id': group_id})
         if server_id:
             data.update({'server_id': server_id})
+        if parent_id:
+            data.update({'parentId': parent_id})
+        if message_id:
+            data.update({'messageId': message_id})
         data.update({"isPublic": str(is_public).lower()})
         response = self.request(
             'POST',
             f'{self.base_url}/channels',
             json=data
         )
         return response
@@ -319,14 +325,96 @@
             user_id: str
     ):
         response = self.request(
             'POST',
             f'{self.base_url}/servers/{server_id}/bans/{user_id}'
         )
         return response
+    
+    def create_role(
+            self,
+            server_id: str,
+            name: str,
+            is_displayed_separately: bool = False,
+            is_self_assignable: bool = False,
+            is_mentionable: bool = False,
+            permissions: list[str] = [],
+            colors = []
+    ):
+        data = {
+            'name': name,
+            'isDisplayedSeparately': str(is_displayed_separately).lower(),
+            'isSelfAssignable': str(is_self_assignable).lower(),
+            'isMentionable': str(is_mentionable).lower(),
+            'permissions': permissions,
+            'colors': colors
+                }
+        response = self.request(
+            'POST',
+            f'{self.base_url}/servers/{server_id}/roles',
+            json=data
+        )
+        return response
+    
+    def get_role(
+            self,
+            server_id: str,
+            role_id: int
+    ):
+        response = self.request(
+            'GET',
+            f'{self.base_url}/servers/{server_id}/roles/{role_id}'
+        )
+        return response
+    
+    def get_roles(
+            self,
+            server_id: str
+    ):
+        response = self.request(
+            'GET',
+            f'{self.base_url}/servers/{server_id}/roles'
+        )
+        return response
+    
+    def update_role(
+            self,
+            server_id: str,
+            role_id: int,
+            name: str = None,
+            is_displayed_separately: bool = False,
+            is_self_assignable: bool = False,
+            is_mentionable: bool = False,
+            permissions: list[str] = [],
+            colors = []
+    ):
+        response = self.request(
+            'PATCH',
+            f'{self.base_url}/servers/{server_id}/roles/{role_id}',
+            json={
+                'name': name,
+                'isDisplayedSeparately': str(is_displayed_separately).lower(),
+                'isSelfAssignable': str(is_self_assignable).lower(),
+                'isMentionable': str(is_mentionable).lower(),
+                'permissions': permissions,
+                'colors': colors
+            }
+        )
+        return response
+    
+    def delete_role(
+            self,
+            server_id: str,
+            role_id: int
+    ):
+        response = self.request(
+            'DELETE',
+            f'{self.base_url}/servers/{server_id}/roles/{role_id}'
+        )
+        return response
 
     def add_role(
             self,
             server_id: str,
             user_id: str,
             role_id: int
     ):
@@ -1379,16 +1467,19 @@
 
     def delete_group(self, server_id: str, group_id: str):
         response = self.request('DELETE', f'{self.base_url}/servers/{server_id}/groups/{group_id}')
         return response
 
 
 
-    def update_status(self, content: str, emote_id: int):
-        response = self.request('PUT', f'{self.base_url}/users/@me/status', json={'content': content, 'emoteId': emote_id})
+    def update_status(self, content: str, emote_id: int, expires_at: str = None):
+        json = {'content': content, 'emoteId': emote_id}
+        if expires_at:
+            json.update({'expiresAt': expires_at})
+        response = self.request('PUT', f'{self.base_url}/users/@me/status', json=json)
         return response
 
 
     def delete_status(self):
         response = self.request('DELETE', f'{self.base_url}/users/@me/status')
         return response
```

### Comparing `nextguild-1.1.4/nextguild/embed.py` & `nextguild-1.1.5/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.4/nextguild/events.py` & `nextguild-1.1.5/nextguild/events.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.4/nextguild/message.py` & `nextguild-1.1.5/nextguild/message.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.4/nextguild/reaction.py` & `nextguild-1.1.5/nextguild/reaction.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.4/nextguild.egg-info/PKG-INFO` & `nextguild-1.1.5/nextguild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.4
+Version: 1.1.5
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.1.4/pyproject.toml` & `nextguild-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

