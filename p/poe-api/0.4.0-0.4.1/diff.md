# Comparing `tmp/poe_api-0.4.0-py3-none-any.whl.zip` & `tmp/poe_api-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 39114 bytes, number of entries: 41
--rw-r--r--  2.0 unx    19184 b- defN 23-May-28 02:21 poe.py
+Zip file size: 39387 bytes, number of entries: 41
+-rw-r--r--  2.0 unx    19452 b- defN 23-May-30 16:46 poe.py
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
--rw-r--r--  2.0 unx    35149 b- defN 23-May-28 03:21 poe_api-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    16887 b- defN 23-May-28 03:21 poe_api-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-28 03:21 poe_api-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-28 03:21 poe_api-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3866 b- defN 23-May-28 03:21 poe_api-0.4.0.dist-info/RECORD
-41 files, 96482 bytes uncompressed, 32740 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-30 17:12 poe_api-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17489 b- defN 23-May-30 17:12 poe_api-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 17:12 poe_api-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-30 17:12 poe_api-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3866 b- defN 23-May-30 17:12 poe_api-0.4.1.dist-info/RECORD
+41 files, 97352 bytes uncompressed, 33013 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -102,23 +102,23 @@
 
 Filename: poe_graphql/ViewerStateUpdatedSubscription.graphql
 Comment: 
 
 Filename: poe_graphql/__init__.py
 Comment: 
 
-Filename: poe_api-0.4.0.dist-info/LICENSE
+Filename: poe_api-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: poe_api-0.4.0.dist-info/METADATA
+Filename: poe_api-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: poe_api-0.4.0.dist-info/WHEEL
+Filename: poe_api-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: poe_api-0.4.0.dist-info/top_level.txt
+Filename: poe_api-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: poe_api-0.4.0.dist-info/RECORD
+Filename: poe_api-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## poe.py

```diff
@@ -213,14 +213,21 @@
     for thread in threads:
       thread.join()
     
     self.bots = bots
     self.bot_names = self.get_bot_names()          
     return bots
   
+  def get_bot_by_codename(self, bot_codename):
+    if bot_codename in self.bots:
+      return self.bots[bot_codename]
+    
+    #todo: cache this so it isn't re-downloaded every time
+    return self.get_bot(bot_codename)
+
   def get_bot_names(self):
     bot_names = {}
     for bot_nickname in self.bots:
       bot_obj = self.bots[bot_nickname]["defaultBotObject"]
       bot_names[bot_nickname] = bot_obj["displayName"]
     return bot_names
   
@@ -247,15 +254,15 @@
       bots = [node["node"] for node in result["edges"]]
       return {
         "bots": bots,
         "end_cursor": result["pageInfo"]["endCursor"],
       }
   
   def get_remaining_messages(self, chatbot):
-    chat_data = self.get_bot(self.bot_names[chatbot])
+    chat_data = self.get_bot_by_codename(chatbot)
     return chat_data["defaultBotObject"]["messageLimit"]["numMessagesRemaining"]
       
   def get_channel_data(self, channel=None):
     logger.info("Downloading channel data...")
     r = request_with_retries(self.session.get, self.settings_url)
     data = r.json()
 
@@ -393,19 +400,15 @@
 
     # reconnect websocket
     if not self.ws_connected:
       self.disconnect_ws()
       self.setup_connection()
       self.connect_ws()
     
-    if chatbot in self.bots:
-      chat_id = self.bots[chatbot]["chatId"]
-    else:
-      chat_id = self.get_bot(chatbot)["chatId"]
-
+    chat_id = self.get_bot_by_codename(chatbot)["chatId"]
     message_data = self.send_query("SendMessageMutation", {
       "bot": chatbot,
       "query": message,
       "chatId": chat_id,
       "source": None,
       "clientNonce": generate_nonce(),
       "sdid": self.device_id,
@@ -451,24 +454,28 @@
 
     del self.active_messages[human_message_id]
     del self.message_queues[human_message_id]
   
   def send_chat_break(self, chatbot):
     logger.info(f"Sending chat break to {chatbot}")
     result = self.send_query("AddMessageBreakMutation", {
-      "chatId": self.bots[chatbot]["chatId"]}
+      "chatId": self.get_bot_by_codename(chatbot)["chatId"]}
     )
     return result["data"]["messageBreakCreate"]["message"]
 
   def get_message_history(self, chatbot, count=25, cursor=None):
     logger.info(f"Downloading {count} messages from {chatbot}")
-
+    
     messages = []
     if cursor == None:
-      chat_data = self.get_bot(self.bot_names[chatbot])
+      if not chatbot in self.bots:
+        chat_data = self.get_bot(chatbot)
+      else:
+        chat_data = self.get_bot(self.bot_names[chatbot])
+
       if not chat_data["messagesConnection"]["edges"]:
         return []
       messages = chat_data["messagesConnection"]["edges"][:count]
       cursor = chat_data["messagesConnection"]["pageInfo"]["startCursor"]
       count -= len(messages)
 
     cursor = str(cursor)
@@ -482,15 +489,15 @@
       return messages
     elif count <= 0:
       return messages
 
     result = self.send_query("ChatListPaginationQuery", {
       "count": count,
       "cursor": cursor,
-      "id": self.bots[chatbot]["id"]
+      "id": self.get_bot_by_codename(chatbot)["id"]
     })
     query_messages = result["data"]["node"]["messagesConnection"]["edges"]
     messages = query_messages + messages
     return messages
 
   def delete_message(self, message_ids):
     logger.info(f"Deleting messages: {message_ids}")
```

## Comparing `poe_api-0.4.0.dist-info/LICENSE` & `poe_api-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `poe_api-0.4.0.dist-info/METADATA` & `poe_api-0.4.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poe-api
-Version: 0.4.0
+Version: 0.4.1
 Summary: A reverse engineered API wrapper for Quora's Poe
 Home-page: https://github.com/ading2210/poe-api
 Author: ading2210
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -52,29 +52,32 @@
  - Download bot list
  - Send messages
  - Stream bot responses
  - Clear conversation context
  - Download conversation history
  - Delete messages
  - Purge an entire conversation
+ - Create custom bots
+ - Edit your custom bots
+ - Use pre-existing third party bots
 
 ## Installation:
 You can install this library by running the following command:
 ```
 pip3 install poe-api
 ```
 
 ## Documentation:
 Examples can be found in the `/examples` directory. To run these examples, pass in your token as a command-line argument.
 ```
 python3 examples/temporary_message.py "TOKEN_HERE"
 ```
 
 ### Finding Your Token:
-Log into [Poe](https://poe.com) on any web browser, then open your browser's developer tools (also known as "inspect") and look for the value of the `p-b` cookie in the following menus:
+Log into [Poe](https://poe.com) on any desktop web browser, then open your browser's developer tools (also known as "inspect") and look for the value of the `p-b` cookie in the following menus:
  - Chromium: Devtools > Application > Cookies > poe.com
  - Firefox: Devtools > Storage > Cookies
  - Safari: Devtools > Storage > Cookies
 
 ### Using the Client:
 To use this library, simply import `poe` and create a `poe.Client` instance. The Client class accepts the following arguments:
  - `token` - The token to use. 
@@ -114,15 +117,15 @@
   "a2_2": "Claude+"
 }
 """
 ```
 
 Note that, on free accounts, Claude+ (a2_2) has a limit of 3 messages per day and GPT-4 (beaver) has a limit of 1 message per day. Claude-instant-100k (c2_100k) is completely inaccessible for free accounts. For all the other chatbots, there seems to be a rate limit of 10 messages per minute.
 
-#### Using 3rd Party Bots
+#### Using 3rd Party Bots:
 To get a list of 3rd party bots, use `client.explore_bots`, which accepts the following arguments:
  - `end_cursor = None` - The cursor to use when fetching the list. 
  - `count = 25` - The number of bots that is returned.
 
 The function will return a dict containing a list of bots and the cursor for the next page:
 ```python
 print(json.dumps(client.explore_bots(count=1), indent=2))
@@ -191,23 +194,23 @@
 
 Bot API related arguments:
  - `api_key = None` - The new API key for the bot. 
  - `api_url = None` - The new API URL for the bot.
 
 A full example of how to create and edit bots is located at `examples/create_bot.py`.
 ```python
-edit_result = client.edit_bot(1086981, "bot_handle_here", base_model="beaver")
+edit_result = client.edit_bot(1086981, "bot_handle_here", base_model="a2")
 ```
 
 #### Sending Messages:
 You can use the `client.send_message` function to send a message to a chatbot, which accepts the following arguments:
  - `chatbot` - The codename of the chatbot. (example: `capybara`)
  - `message` - The message to send to the chatbot.
  - `with_chat_break = False` - Whether the conversation context should be cleared.
- - `timeout = 20` - The max number of seconds in between recieved chunks until a `RuntimeError` is raised. 
+ - `timeout = 20` - The max number of seconds in between received chunks until a `RuntimeError` is raised. 
 
 The function is a generator which returns the most recent version of the generated message whenever it is updated.
 
 Streamed Example:
 ```python
 message = "Summarize the GNU GPL v3"
 for chunk in client.send_message("capybara", message):
@@ -335,39 +338,53 @@
   "Sec-Fetch-Mode": "cors",
   "Sec-Fetch-Site": "same-origin"
 }
 ```
 
 Previously, this was done through `poe.user_agent`, but that variable is now completely ignored.
 
-You'd also want to change `poe.client_identifier` to match the user-agent that you have set. See the [Python-TLS-Client documentation](https://github.com/FlorianREGAZ/Python-Tls-Client#examples) for some examples.
+You'd also want to change `poe.client_identifier` to match the user-agent that you have set. See the [Python-TLS-Client documentation](https://github.com/FlorianREGAZ/Python-Tls-Client#examples) for some sample values. Keep in mind that spoofing Chrome/Firefox versions >= 110 may be detectable. 
+```python
+poe.client_identifier = "chrome_107"
+```
 
 ### Setting a Custom Device ID:
 If you want to change the device ID that is being spoofed, you can use the `poe.set_device_id`, which accepts the following arguments:
- - `user_id` - The user ID of the account you want to change the device ID for.
- - `device_id` - The new device ID. This is a standard 32 character UUID string.
+ - `user_id` - The user ID of the account you want to change the device ID for. The user ID can be found at `client.viewer["poeUser"]["id"]`.
+ - `device_id` - The new device ID. This is a 32 character UUID string in the following format: `xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx`
+
+```python
+poe.set_device_id("UGMlVXqlcLYyMOATMDsKNTMz", "6d659b04-043a-41f8-97c7-fb7d7fe9ad34")
+```
 
 The device IDs are saved to `~/.config/poe-api/device_id.json` on Unix-like systems, and `C:\Users\<user>\AppData\Roaming\poe-api\device_id.json` on Windows.
 
 Additionally, the `poe.get_device_id` function or `client.device_id` can be used to retrieve the saved device ID.
+```python
+>>> poe.get_device_id("UGMlVXqlcLYyMOATMDsKNTMz")
+#6d659b04-043a-41f8-97c7-fb7d7fe9ad34
+
+>>> client.device_id
+#6d659b04-043a-41f8-97c7-fb7d7fe9ad34
+```
 
 ## Copyright: 
 This program is licensed under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.txt). Most code, with the exception of the GraphQL queries, has been written by me, [ading2210](https://github.com/ading2210).
 
 Reverse engineering the `poe-tag-id` header has been done by [xtekky](https://github.com/xtekky) in [PR #39](https://github.com/ading2210/poe-api/pull/39).
 
 The `client.get_remaining_messages` function was written by [Snowad14](https://github.com/Snowad14) in [PR #46](https://github.com/ading2210/poe-api/pull/46).
 
 Detection avoidance and fetching the third party bots has been done by [acheong08](https://github.com/acheong08/) in [PR #79](https://github.com/ading2210/poe-api/pull/79).
 
-Most of the GraphQL queries are taken from [muharamdani/poe](https://github.com/muharamdani/poe), which is licenced under the ISC License. 
+Most of the GraphQL queries are taken from [muharamdani/poe](https://github.com/muharamdani/poe), which is licensed under the ISC License. 
 
 ### Copyright Notice:
 ```
-ading2210/poe-api: a reverse engineered Python API wrapepr for Quora's Poe
+ading2210/poe-api: a reverse engineered Python API wrapper for Quora's Poe
 Copyright (C) 2023 ading2210
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

## Comparing `poe_api-0.4.0.dist-info/RECORD` & `poe_api-0.4.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-poe.py,sha256=6wxy5KVw_Pon-cL2Jm0X8U6FbO8st9o37mlD0qoQDXA,19184
+poe.py,sha256=4qbDOrvFjeYg66Q8dQCEdbptmodia4RDXrBbWWrPXJU,19452
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
-poe_api-0.4.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-poe_api-0.4.0.dist-info/METADATA,sha256=_dHhhhIPAmBaim6Pr2aa0p3HnFa32Hsl9ChTFHYOpS8,16887
-poe_api-0.4.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-poe_api-0.4.0.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
-poe_api-0.4.0.dist-info/RECORD,,
+poe_api-0.4.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+poe_api-0.4.1.dist-info/METADATA,sha256=93o2Ng9_Ft-X805mQSXslByoKXr2G1OOtOwK3fTXeqI,17489
+poe_api-0.4.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+poe_api-0.4.1.dist-info/top_level.txt,sha256=7Sk_jA5I5n3fNZ1671pcBau4TWZLe6UXCEnCD5NhGGI,16
+poe_api-0.4.1.dist-info/RECORD,,
```

