# Comparing `tmp/dgl_client-0.3.3.tar.gz` & `tmp/dgl_client-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.3.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.3.3.tar` & `dgl_client-0.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       36 2023-05-26 06:08:29.040320 dgl_client-0.3.3/.gitignore
--rw-r--r--   0        0        0       69 2023-05-26 06:08:29.040320 dgl_client-0.3.3/README.md
--rw-r--r--   0        0        0       64 2023-05-29 12:39:21.928517 dgl_client-0.3.3/dgl_client/__init__.py
--rw-r--r--   0        0        0     6572 2023-05-29 12:32:58.816519 dgl_client-0.3.3/dgl_client/api_cli.py
--rw-r--r--   0        0        0     3928 2023-05-29 11:12:10.896537 dgl_client-0.3.3/dgl_client/main.py
--rw-r--r--   0        0        0        0 2023-05-26 06:08:29.040320 dgl_client-0.3.3/dgl_client/utils.py
--rw-r--r--   0        0        0      456 2023-05-29 12:39:34.988517 dgl_client-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 06:08:29.040320 dgl_client-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0      952 2023-05-29 11:23:50.236534 dgl_client-0.3.3/tests/create_token.py
--rw-r--r--   0        0        0     2074 2023-05-29 08:36:18.388573 dgl_client-0.3.3/tests/test_decode.py
--rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 dgl_client-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-05-30 14:01:06.441529 dgl_client-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.3.4/README.md
+-rw-r--r--   0        0        0       64 2023-05-31 10:23:58.053231 dgl_client-0.3.4/dgl_client/__init__.py
+-rw-r--r--   0        0        0     6998 2023-05-31 10:18:45.716426 dgl_client-0.3.4/dgl_client/api_cli.py
+-rw-r--r--   0        0        0     4308 2023-05-31 10:23:38.774668 dgl_client-0.3.4/dgl_client/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775226 dgl_client-0.3.4/dgl_client/utils.py
+-rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.3.4/notebook.ipynb
+-rw-r--r--   0        0        0      456 2023-05-30 07:01:38.905722 dgl_client-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-30 07:01:38.905943 dgl_client-0.3.4/tests/create_token.py
+-rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 dgl_client-0.3.4/PKG-INFO
```

### Comparing `dgl_client-0.3.3/dgl_client/api_cli.py` & `dgl_client-0.3.4/dgl_client/api_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
               "Refresh": f"{rtok}"
               },
       )
       response.raise_for_status()
       new_tok = response.json()
     except:
       raise
-    logger.info("New token is %s"%str(new_tok))
+    logger.debug("New token is %s"%str(new_tok))
 
     return new_tok
 
 def ak2token(endp, access_key):
     logger.info("Logging in using access_key...")
     new_tok = None
     try:
@@ -70,15 +70,15 @@
               "TrustedClient": f"{access_key}"
               },
       )
       response.raise_for_status()
       new_tok = response.json()
     except:
       raise
-    logger.info("New token is %s"%str(new_tok))
+    logger.debug("New token is %s"%str(new_tok))
 
     return new_tok
 
 
 class APIClient:
     def __init__(self, backend_url, http_client=requests):
         self.backend_url = backend_url
@@ -108,14 +108,30 @@
             headers=self.auth_headers,
         )
         response.raise_for_status()
         self.chat_id = response.json()["id"]
         self.message_id = None
         return self.chat_id
 
+    def list_chats(self):
+        response = self.http_client.get(
+            f"{self.backend_url}/chats",
+            json={},
+            headers=self.auth_headers,
+        )
+        response.raise_for_status()
+        res = response.json()
+
+        bag = []
+        if "chats" in res:
+            for chat in res["chats"]:
+                bag.append((chat["id"], chat["title"]))
+
+        return bag
+
     def get_available_models(self):
         response = self.http_client.get(
             f"{self.backend_url}/configs/model_configs",
             headers=self.auth_headers,
         )
         response.raise_for_status()
         return [model["name"] for model in response.json()]
@@ -201,11 +217,11 @@
                     else:
                         logger.debug(f"Message event type but no message? {data=}")    
                 elif event_type == "error":
                     raise RuntimeError(data["error"])
                 elif event_type == "pending":
                     logger.debug(f"Message pending. {data=}")
                 else:
-                    print("UNKNOWN!!!")
+                    print("Received unknown event_type!!!")
                     print(data)
```

### Comparing `dgl_client-0.3.3/dgl_client/main.py` & `dgl_client-0.3.4/dgl_client/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,20 +22,35 @@
   logger.info("Available models %s"%str(available_models))
 
   available_wkf = client.get_available_workflows()
   logger.info("Available workflows %s"%str(available_wkf))
 
   return available_models, available_wkf
 
+def list_chats(args):
+  client = get_client(args)
+  do_login(args, client)
+  chats = client.list_chats()
+  logger.info("Found %d existing chats"%(len(chats)))
+
+  for chat in chats:
+    print("* %s - %s"%(chat[0],chat[1][:25]))
+
+  return chats
+
 def main_ls(args):
   match args.resource:
     case "models":
       list_models(args)
     case "model":
       list_models(args)      
+    case "chats":
+      list_chats(args)            
+    #case "messages":
+    #  list_messages(args)            
     case _:
       logger.error("Resource not found!")
 
 def do_login(args, client):
   if args.access_key:
     client.login(args.access_key)
     # if os.path.exists(args.token_file):
@@ -81,25 +96,25 @@
     DGL_API_ENDPOINT = os.environ["DGL_API_ENDPOINT"]
 
   parser = argparse.ArgumentParser(description='DigLife API Client.')
   parser.add_argument('--logdir', type=str, default="logs/",
                       help='Where to store logs')
   parser.add_argument('--endpoint', type=str, default=DGL_API_ENDPOINT,
                       help='Endpoint for the inference')
+  parser.add_argument('-k','--access_key', type=str, required=True,
+                      help='Access keys to authenticate to the API')                      
 
   subparsers = parser.add_subparsers(help='You can choose between different commands')
   chat_p = subparsers.add_parser('chat', help='chat with the assistants')
   chat_p.set_defaults(func=main_chat)
 
   chat_p.add_argument('message', type=str, 
                       help='say something to the model')
   chat_p.add_argument('-c','--chat-id', type=str,
                       help='Continue previous chat')
-  chat_p.add_argument('-k','--access_key', type=str, required=True,
-                      help='Access keys to authenticate to the API')
   chat_p.add_argument('-m','--model', type=str, required=True,
                       help='Which model do you want to talk to?')
   chat_p.add_argument('-i','--interactive', action='store_true',
                       help='Run interactive chat')
   
   config_p = subparsers.add_parser('ls', help='List resources')
   config_p.add_argument('resource', type=str,
```

### Comparing `dgl_client-0.3.3/tests/create_token.py` & `dgl_client-0.3.4/tests/create_token.py`

 * *Files identical despite different names*

