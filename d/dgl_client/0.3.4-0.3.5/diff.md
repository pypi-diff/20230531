# Comparing `tmp/dgl_client-0.3.4.tar.gz` & `tmp/dgl_client-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.3.4.tar` & `dgl_client-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0       51 2023-05-30 14:01:06.441529 dgl_client-0.3.4/.gitignore
--rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.3.4/README.md
--rw-r--r--   0        0        0       64 2023-05-31 10:23:58.053231 dgl_client-0.3.4/dgl_client/__init__.py
--rw-r--r--   0        0        0     6998 2023-05-31 10:18:45.716426 dgl_client-0.3.4/dgl_client/api_cli.py
--rw-r--r--   0        0        0     4308 2023-05-31 10:23:38.774668 dgl_client-0.3.4/dgl_client/main.py
--rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775226 dgl_client-0.3.4/dgl_client/utils.py
--rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.3.4/notebook.ipynb
--rw-r--r--   0        0        0      456 2023-05-30 07:01:38.905722 dgl_client-0.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0      952 2023-05-30 07:01:38.905943 dgl_client-0.3.4/tests/create_token.py
--rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 dgl_client-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-05-30 14:01:06.441529 dgl_client-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.3.5/README.md
+-rw-r--r--   0        0        0       64 2023-05-31 17:06:01.123122 dgl_client-0.3.5/dgl_client/__init__.py
+-rw-r--r--   0        0        0     7760 2023-05-31 15:47:31.730669 dgl_client-0.3.5/dgl_client/api_cli.py
+-rw-r--r--   0        0        0     4434 2023-05-31 12:38:59.807362 dgl_client-0.3.5/dgl_client/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775226 dgl_client-0.3.5/dgl_client/utils.py
+-rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.3.5/notebook.ipynb
+-rw-r--r--   0        0        0      456 2023-05-30 07:01:38.905722 dgl_client-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.3.5/tests/__init__.py
+-rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 dgl_client-0.3.5/PKG-INFO
```

### Comparing `dgl_client-0.3.4/README.md` & `dgl_client-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dgl_client-0.3.4/dgl_client/api_cli.py` & `dgl_client-0.3.5/dgl_client/api_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -83,26 +83,27 @@
     def __init__(self, backend_url, http_client=requests):
         self.backend_url = backend_url
         self.http_client = http_client
         self.auth_headers = None
         self.message_id = None
 
     def login(self, access_key):
-        print(access_key)
         atok = ak2token(self.backend_url, access_key)
-
         username = login_check(self.backend_url, atok)
-
         if username:
             logger.info(f"Logged in as {username}")    
             self.auth_headers = {"Authorization": f"Bearer {atok}"}
 
-
-    def continue_chat(self, chat_id):
+    def continue_chat(self, chat_id, message_id=None):
         self.chat_id = chat_id
+        if not message_id:
+            mess = self.list_messages(chat_id)
+            if len(mess) > 0:
+                message_id = mess[0]
+        self.message_id = message_id
         return self.chat_id
 
     def create_chat(self):
         response = self.http_client.post(
             f"{self.backend_url}/chats",
             json={},
             headers=self.auth_headers,
@@ -124,14 +125,28 @@
         bag = []
         if "chats" in res:
             for chat in res["chats"]:
                 bag.append((chat["id"], chat["title"]))
 
         return bag
 
+    def list_messages(self, chat_id):
+        response = self.http_client.get(
+            f"{self.backend_url}/chats/%s"%chat_id,
+            json={},
+            headers=self.auth_headers,
+        )
+        response.raise_for_status()
+        res = response.json()
+        messages = res["messages"]
+        bag = []
+        for message in messages:
+            bag.append(message["id"])
+        return bag        
+
     def get_available_models(self):
         response = self.http_client.get(
             f"{self.backend_url}/configs/model_configs",
             headers=self.auth_headers,
         )
         response.raise_for_status()
         return [model["name"] for model in response.json()]
@@ -141,25 +156,28 @@
             f"{self.backend_url}/configs/workflow_configs",
             headers=self.auth_headers,
         )
         response.raise_for_status()
         return [model["name"] for model in response.json()]
 
     def send_message(self, message, model_config_name, collection=None):
+        print("PARENT:",self.message_id)
         response = self.http_client.post(
             f"{self.backend_url}/chats/{self.chat_id}/prompter_message",
+            #f"http://localhost:12345/chats/{self.chat_id}/prompter_message",            
             json={
                 "parent_id": self.message_id,
                 "content": message,
                 "collection": collection
             },
             headers=self.auth_headers,
         )
         response.raise_for_status()
         prompter_message_id = response.json()["id"]
+        print("MESSAGEID",prompter_message_id)
 
         response = self.http_client.post(
             f"{self.backend_url}/chats/{self.chat_id}/assistant_message",
             json={
                 "parent_id": prompter_message_id,
                 "model_config_name": model_config_name,
                 "sampling_parameters": {
```

### Comparing `dgl_client-0.3.4/dgl_client/main.py` & `dgl_client-0.3.5/dgl_client/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,37 +33,45 @@
   logger.info("Found %d existing chats"%(len(chats)))
 
   for chat in chats:
     print("* %s - %s"%(chat[0],chat[1][:25]))
 
   return chats
 
+def list_messages(args, chat_id):
+  client = get_client(args)
+  do_login(args, client)
+  messages = client.list_messages(chat_id)
+  logger.info("Found %d existing chats"%(len(messages)))
+
+  for message in messages:
+    print(message)
+
+  return messages
+
 def main_ls(args):
   match args.resource:
     case "models":
       list_models(args)
     case "model":
       list_models(args)      
     case "chats":
       list_chats(args)            
-    #case "messages":
-    #  list_messages(args)            
+    case "messages":
+      if args.chat_id:
+        list_messages(args, args.chat_id)
     case _:
       logger.error("Resource not found!")
 
 def do_login(args, client):
   if args.access_key:
     client.login(args.access_key)
-    # if os.path.exists(args.token_file):
-    #   tokens = {}
-    #   with open(args.token_file,"r") as fp:
-    #     tokens = json.load(fp)
-    #   client.login(tokens)
+    return True
 
-  return True
+  return False
 
 def main_chat(args):
   client = get_client(args)
 
   model_config_name = args.model
 
   do_login(args, client)
@@ -98,23 +106,23 @@
   parser = argparse.ArgumentParser(description='DigLife API Client.')
   parser.add_argument('--logdir', type=str, default="logs/",
                       help='Where to store logs')
   parser.add_argument('--endpoint', type=str, default=DGL_API_ENDPOINT,
                       help='Endpoint for the inference')
   parser.add_argument('-k','--access_key', type=str, required=True,
                       help='Access keys to authenticate to the API')                      
+  parser.add_argument('-c','--chat-id', type=str,
+                      help='Continue previous chat')
 
   subparsers = parser.add_subparsers(help='You can choose between different commands')
   chat_p = subparsers.add_parser('chat', help='chat with the assistants')
   chat_p.set_defaults(func=main_chat)
 
   chat_p.add_argument('message', type=str, 
                       help='say something to the model')
-  chat_p.add_argument('-c','--chat-id', type=str,
-                      help='Continue previous chat')
   chat_p.add_argument('-m','--model', type=str, required=True,
                       help='Which model do you want to talk to?')
   chat_p.add_argument('-i','--interactive', action='store_true',
                       help='Run interactive chat')
   
   config_p = subparsers.add_parser('ls', help='List resources')
   config_p.add_argument('resource', type=str,
```

### Comparing `dgl_client-0.3.4/notebook.ipynb` & `dgl_client-0.3.5/notebook.ipynb`

 * *Files identical despite different names*

