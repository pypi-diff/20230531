# Comparing `tmp/poe_api-0.4.2-py3-none-any.whl.zip` & `tmp/poe_api-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 39396 bytes, number of entries: 41
--rw-r--r--  2.0 unx    19451 b- defN 23-May-30 22:47 poe.py
+Zip file size: 39457 bytes, number of entries: 41
+-rw-r--r--  2.0 unx    19695 b- defN 23-May-31 05:27 poe.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-May-27 23:16 poe_graphql/AddHumanMessageMutation.graphql
 -rw-r--r--  2.0 unx      373 b- defN 23-May-27 23:16 poe_graphql/AddMessageBreakMutation.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/AutoSubscriptionMutation.graphql
 -rw-r--r--  2.0 unx       97 b- defN 23-May-27 23:16 poe_graphql/BioFragment.graphql
 -rw-r--r--  2.0 unx       73 b- defN 23-May-27 23:16 poe_graphql/ChatAddedSubscription.graphql
 -rw-r--r--  2.0 unx      100 b- defN 23-May-27 23:16 poe_graphql/ChatFragment.graphql
 -rw-r--r--  2.0 unx     6971 b- defN 23-May-27 23:16 poe_graphql/ChatListPaginationQuery.graphql
@@ -31,13 +31,13 @@
 -rw-r--r--  2.0 unx      147 b- defN 23-May-27 23:16 poe_graphql/SummarizeQuotePostQuery.graphql
 -rw-r--r--  2.0 unx      180 b- defN 23-May-27 23:16 poe_graphql/SummarizeSharePostQuery.graphql
 -rw-r--r--  2.0 unx      368 b- defN 23-May-27 23:16 poe_graphql/UserSnippetFragment.graphql
 -rw-r--r--  2.0 unx      400 b- defN 23-May-27 23:16 poe_graphql/ViewerInfoQuery.graphql
 -rw-r--r--  2.0 unx     1038 b- defN 23-May-27 23:16 poe_graphql/ViewerStateFragment.graphql
 -rw-r--r--  2.0 unx      657 b- defN 23-May-27 23:16 poe_graphql/ViewerStateUpdatedSubscription.graphql
 -rw-r--r--  2.0 unx        0 b- defN 23-May-27 23:16 poe_graphql/__init__.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-30 22:49 poe_api-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    17489 b- defN 23-May-30 22:49 poe_api-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 22:49 poe_api-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-30 22:49 poe_api-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3866 b- defN 23-May-30 22:49 poe_api-0.4.2.dist-info/RECORD
-41 files, 97351 bytes uncompressed, 33022 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-31 05:29 poe_api-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17489 b- defN 23-May-31 05:29 poe_api-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 05:29 poe_api-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-31 05:29 poe_api-0.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3866 b- defN 23-May-31 05:29 poe_api-0.4.3.dist-info/RECORD
+41 files, 97595 bytes uncompressed, 33083 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -102,23 +102,23 @@
 
 Filename: poe_graphql/ViewerStateUpdatedSubscription.graphql
 Comment: 
 
 Filename: poe_graphql/__init__.py
 Comment: 
 
-Filename: poe_api-0.4.2.dist-info/LICENSE
+Filename: poe_api-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: poe_api-0.4.2.dist-info/METADATA
+Filename: poe_api-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: poe_api-0.4.2.dist-info/WHEEL
+Filename: poe_api-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: poe_api-0.4.2.dist-info/top_level.txt
+Filename: poe_api-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: poe_api-0.4.2.dist-info/RECORD
+Filename: poe_api-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## poe.py

```diff
@@ -1,9 +1,10 @@
 import re, json, random, logging, time, queue, threading, traceback, hashlib, string, random, os
-import tls_client as requests
+import requests
+import tls_client as requests_tls
 import secrets
 import websocket
 import uuid
 from pathlib import Path
 from urllib.parse import urlparse
 
 parent_path = Path(__file__).resolve().parent
@@ -94,15 +95,19 @@
   gql_recv_url = "https://poe.com/api/receive_POST"
   home_url = "https://poe.com"
   settings_url = "https://poe.com/api/settings"
   
   def __init__(self, token, proxy=None, headers=headers, device_id=None, client_identifier=client_identifier):
     self.device_id = device_id
     self.proxy = proxy
-    self.session = requests.Session(client_identifier=client_identifier)
+    
+    if client_identifier:
+      self.session = requests_tls.Session(client_identifier=client_identifier)
+    else:
+      self.session = requests.Session()
         
     if proxy:
       self.session.proxies = {
         "http": self.proxy,
         "https": self.proxy
       }
       logger.info(f"Proxy enabled: {self.proxy}")
@@ -386,16 +391,20 @@
     except Exception:
       logger.error(traceback.format_exc())
       self.disconnect_ws()
       self.connect_ws()
 
   def send_message(self, chatbot, message, with_chat_break=False, timeout=20):
     # if there is another active message, wait until it has finished sending
+    timer = 0
     while None in self.active_messages.values():
       time.sleep(0.01)
+      timer += 0.01
+      if timer > timeout:
+        raise RuntimeError("Timed out waiting for other messages to send.")
 
     # None indicates that a message is still in progress
     self.active_messages["pending"] = None
 
     logger.info(f"Sending message to {chatbot}: {message}")
 
     # reconnect websocket
@@ -470,15 +479,15 @@
       if not chatbot in self.bots:
         chat_data = self.get_bot(chatbot)
       else:
         chat_data = self.get_bot(self.bot_names[chatbot])
 
       if not chat_data["messagesConnection"]["edges"]:
         return []
-      messages = chat_data["messagesConnection"]["edges"][count:]
+      messages = chat_data["messagesConnection"]["edges"][-count:]
       cursor = chat_data["messagesConnection"]["pageInfo"]["startCursor"]
       count -= len(messages)
 
     cursor = str(cursor)
     if count > 50:
       messages = self.get_message_history(chatbot, count=50, cursor=cursor) + messages
       while count > 0:
```

## Comparing `poe_api-0.4.2.dist-info/LICENSE` & `poe_api-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `poe_api-0.4.2.dist-info/METADATA` & `poe_api-0.4.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-api
-Version: 0.4.2
+Version: 0.4.3
 Summary: A reverse engineered API wrapper for Quora's Poe
 Home-page: https://github.com/ading2210/poe-api
 Author: ading2210
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

## Comparing `poe_api-0.4.2.dist-info/RECORD` & `poe_api-0.4.3.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-poe.py,sha256=Rh6EQ2giIip3wVofmfXKaYkauNwL6CH9by1mNPKxlgo,19451
+poe.py,sha256=ddlz8BtzN1Xyi_ZqyDrVVobSrKoqyOtmHjTBmb5Mseo,19695
 poe_graphql/AddHumanMessageMutation.graphql,sha256=Va4SoysKE2qPlJfbwoKp6mNv0vs5hnVR20g8hPvAxdY,1093
 poe_graphql/AddMessageBreakMutation.graphql,sha256=0XrqSAgAkG5vCFwBALRpoAgUDSFM9XUB5wBy5Iou9c8,373
 poe_graphql/AutoSubscriptionMutation.graphql,sha256=3i8EnqwUrjOcJ2Hxly-lKhwPBJdbpO99POiM_K6jVD4,180
 poe_graphql/BioFragment.graphql,sha256=3ZdXaPtuHK38bG10WFH6bvpebcyrTLu5fs-ddtfLjf0,97
 poe_graphql/ChatAddedSubscription.graphql,sha256=NFLZJAwi0V2WQea1oelyRUrtNrwOE58NOeX8ChzVE10,73
 poe_graphql/ChatFragment.graphql,sha256=NFVSvT3NdYlEquue3yTHPu9ezCIgx6k1OXJZo2ytIzU,100
 poe_graphql/ChatListPaginationQuery.graphql,sha256=-jtpUwcHsF8nEXQcxLe9gFycYuKRVDBjGNFiH-nPL98,6971
@@ -30,12 +30,12 @@
 poe_graphql/SummarizeQuotePostQuery.graphql,sha256=V4PQ1XkEDCsVR3z7h4SLsonZsWG7RptFd6JPwlGwOvE,147
 poe_graphql/SummarizeSharePostQuery.graphql,sha256=iCN8oiUUp2jfsiBxmsTA7k3_60E0MNwA5gnNrhnYpJc,180
 poe_graphql/UserSnippetFragment.graphql,sha256=Eg8rK7XM6-HqVJkpEBY0bJaYqF-FdDdWdg-Jj3VTnF0,368
 poe_graphql/ViewerInfoQuery.graphql,sha256=Xtn-VGGiknKgrW81s7YfIJwhmilobrSqiCObpoJdYfw,400
 poe_graphql/ViewerStateFragment.graphql,sha256=aicUJncsRpPBh_L2xqDv0aHcUIPIsDrDFPfDs3jcFoU,1038
 poe_graphql/ViewerStateUpdatedSubscription.graphql,sha256=1dPs0WuOLl4ybZXm4bUF60eVc94O10EkKOtqnQYODic,657
 poe_graphql/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-poe_api-0.4.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-poe_api-0.4.2.dist-info/METADATA,sha256=H5ax5ciNYJJkzkCqIx36fCheL5NM1XzFD2pyQyvdcI4,17489
-poe_api-0.4.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-poe_api-0.4.2.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
-poe_api-0.4.2.dist-info/RECORD,,
+poe_api-0.4.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+poe_api-0.4.3.dist-info/METADATA,sha256=PcB14p_3SRBdU5pOmW5lFJQAR9IktOiAu2Zyqyv7GzY,17489
+poe_api-0.4.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+poe_api-0.4.3.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
+poe_api-0.4.3.dist-info/RECORD,,
```

