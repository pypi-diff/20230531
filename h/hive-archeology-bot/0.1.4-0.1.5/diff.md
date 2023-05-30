# Comparing `tmp/hive-archeology-bot-0.1.4.tar.gz` & `tmp/hive-archeology-bot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-archeology-bot-0.1.4.tar", last modified: Tue May 30 16:33:58 2023, max compression
+gzip compressed data, was "hive-archeology-bot-0.1.5.tar", last modified: Tue May 30 22:29:17 2023, max compression
```

## Comparing `hive-archeology-bot-0.1.4.tar` & `hive-archeology-bot-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 16:33:58.003673 hive-archeology-bot-0.1.4/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.4/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 16:33:58.003673 hive-archeology-bot-0.1.4/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2104 2023-05-19 19:43:04.000000 hive-archeology-bot-0.1.4/README.md
--rwxr-xr-x   0 rob       (1000) rob       (1000)    20514 2023-05-30 16:32:42.000000 hive-archeology-bot-0.1.4/hive_archeology.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 16:33:58.003673 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       10 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-30 16:33:58.003673 hive-archeology-bot-0.1.4/setup.cfg
--rwxr-xr-x   0 rob       (1000) rob       (1000)     1125 2023-05-22 09:18:10.000000 hive-archeology-bot-0.1.4/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 22:29:17.274253 hive-archeology-bot-0.1.5/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.5/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 22:29:17.274253 hive-archeology-bot-0.1.5/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2104 2023-05-19 19:43:04.000000 hive-archeology-bot-0.1.5/README.md
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    20940 2023-05-30 22:17:32.000000 hive-archeology-bot-0.1.5/hive_archeology.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 22:29:17.274253 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 22:29:16.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-30 22:29:17.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-30 22:29:16.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-30 22:29:16.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       19 2023-05-30 22:29:17.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-30 22:29:17.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-30 22:29:17.274253 hive-archeology-bot-0.1.5/setup.cfg
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     1137 2023-05-30 22:29:00.000000 hive-archeology-bot-0.1.5/setup.py
```

### Comparing `hive-archeology-bot-0.1.4/LICENSE` & `hive-archeology-bot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.4/PKG-INFO` & `hive-archeology-bot-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
 Platform: UNKNOWN
```

### Comparing `hive-archeology-bot-0.1.4/README.md` & `hive-archeology-bot-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.4/hive_archeology.py` & `hive-archeology-bot-0.1.5/hive_archeology.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 """Hive Archaeology tool for voting on timeless content"""
 import time
 import json
 import os
 import argparse
 import operator
 from datetime import datetime
-import dateutil
+from dateutil.parser import parse, _parser  # pylint: disable=import-private-name
 from lighthive.client import Client
 from lighthive.datastructures import Operation
 from lighthive.exceptions import RPCNodeException
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 AUTHORS = {}
 AUTHORS["hive-archology"] = ["pibara", "croupierbot"]
 AUTHORS["lighthive"] = ["emrebeyler", "emrebeyler"]
 
 def make_body(author, benef, curation_rewards):
+    """Construct the proxy comment"""
     ben2prod = {}
     for key, val in AUTHORS.items():
         ben2prod[val[1]] = key
     rval = """This is a [hive-archeology](https://github.com/pibara/hive-archeology) proxy comment meant as a proxy for upvoting good content that is past it's initial pay-out window.
 
 ![image.png](https://files.peakd.com/file/peakd-hive/pibara/EppQ5vutzcx8r5YZ2LiXjW7EnMtgkcam6KpByUfiojAYYXLBmKFTC1jom5Kig1H9Z1w.png)
 
@@ -111,74 +112,82 @@
         self.voter = voter
         self.account = account
         self.wif = wif
         self.tool_creator_share = tool_creator_share
         self.curation_rewards = curation_rewards
         self.printer = printer
 
+    def _comment_is_candidate(self, comment, author):
+        candidate = None
+        # Fetch the last timeout time to check if a payout already occured
+        last_payout = 0
+        try:
+            last_payout =  parse(comment.get("last_payout", "2020-12-31T23:59:59")).timestamp()
+        except _parser.ParserError as exp:
+            self.printer.error(exp)
+            return None
+        except TypeError as exp:
+            self.printer.error(exp)
+            return None
+        if last_payout < 24 * 3600: # no payout yet, this might be a candidate
+            self.printer.info("Candidate comment hasn't been paid out yet")
+            beneficiaries = comment.get("beneficiaries", [])
+            allow_curation_rewards = comment.get("allow_curation_rewards", False)
+            total_ben_cnt = 0
+            total_ben_val = 0
+            # Check if the comment has the post author set as (>=50%) beneficiary)
+            for beneficiary in beneficiaries:
+                if beneficiary.get("account", "") == author:
+                    self.printer.info("- candidate comment has post author as beneficiary")
+                    if (beneficiary.get("weight", 0) > 7999 or
+                            (allow_curation_rewards and beneficiary.get("weight", 0) > 5999)):
+                        self.printer.notice("- candidate has a sufficient reward share going to the post author")
+                    else:
+                        self.printer.notice("- candidate has insufficient share going to post author, no match")
+            # check if all beneficiaries match either the post author or one of the devs
+            valid_beneficiaries = {author}
+            total_ben_cnt = 0
+            total_ben_val = 0
+            for _, value in AUTHORS.items():
+                valid_beneficiaries.add(value[1])
+            all_ok = True
+            for beneficiary in beneficiaries:
+                if beneficiary.get("account", "") not in valid_beneficiaries:
+                    all_ok = False
+                total_ben_val += beneficiary.get("weight", 0)
+                total_ben_cnt += 1
+            if all_ok:
+                self.printer.info("- all beneficiaries are expected beneficiaries")
+                if total_ben_cnt == 1 or total_ben_cnt == len(valid_beneficiaries):
+                    self.printer.info("- valid amount of beneficiaries for comment")
+                    if total_ben_val == 10000:
+                        self.printer.notice("Benneficiary shares add up to 100%, MATCH")
+                        candidate = [comment.get("author", None), comment.get("permlink", None)]
+                else:
+                    self.printer.info("- invalid amount of beneficiaries for comment, no match")
+            else:
+                self.printer.notice("- at least one of the beneficiaries listed is unknown and unexpected, no match")
+        else:
+            self.printer.info("Paid out already, no match")
+        return candidate
+
     def comment(self, author, permlink, weight): # pylint: disable=too-many-locals, too-many-branches, too-many-statements
         """Check is an active proxy comment exists, and if not, create one. Either way, mark for upvote by voter"""
         candidate = None
         self.printer.notice("Looking for candidate reward comment in post comments")
         # Find out if someone else also upvoted this very historic post recently enough to use the proxy comment that user made
         try:
             comments = Client().get_content_replies(author, permlink)
         except RPCNodeException as exp:
             self.printer.error(exp)
             comments = []
         for comment in comments: # pylint: disable = too-many-nested-blocks
             # One candidate is enough
             if candidate is None: # pylint: disable=too-many-statements
-                # Fetch the last timeout time to check if a payout already occured
-                last_payout = 0
-                try:
-                    last_payout =  dateutil.parser.parse(comment.get("last_payout", "2020-12-31T23:59:59")).timestamp()
-                except RPCNodeException as exp:
-                    self.printer.error(exp)
-                    last_payout = time.time()
-                if last_payout < 24 * 3600: # no payout yet, this might be a candidate
-                    self.printer.info("Candidate comment hasn't been paid out yet")
-                    beneficiaries = comment.get("beneficiaries", [])
-                    allow_curation_rewards = comment.get("allow_curation_rewards", False)
-                    total_ben_cnt = 0
-                    total_ben_val = 0
-                    # Check if the comment has the post author set as (>=50%) beneficiary)
-                    for beneficiary in beneficiaries:
-                        if beneficiary.get("account", "") == author:
-                            self.printer.info("- candidate comment has post author as beneficiary")
-                            if (beneficiary.get("weight", 0) > 7999 or
-                                    (allow_curation_rewards and beneficiary.get("weight", 0) > 5999)):
-                                self.printer.notice("- candidate has a sufficient reward share going to the post author")
-                            else:
-                                self.printer.notice("- candidate has insufficient share going to post author, no match")
-                    # check if all beneficiaries match either the post author or one of the devs
-                    valid_beneficiaries = {author}
-                    total_ben_cnt = 0
-                    total_ben_val = 0
-                    for _, value in AUTHORS.items():
-                        valid_beneficiaries.add(value[1])
-                    all_ok = True
-                    for beneficiary in beneficiaries:
-                        if beneficiary.get("account", "") not in valid_beneficiaries:
-                            all_ok = False
-                        total_ben_val += beneficiary.get("weight", 0)
-                        total_ben_cnt += 1
-                    if all_ok:
-                        self.printer.info("- all beneficiaries are expected beneficiaries")
-                        if total_ben_cnt == 1 or total_ben_cnt == len(valid_beneficiaries):
-                            self.printer.info("- valid amount of beneficiaries for comment")
-                            if total_ben_val == 10000:
-                                self.printer.notice("Benneficiary shares add up to 100%, MATCH")
-                                candidate = [comment.get("author", None), comment.get("permlink", None)]
-                        else:
-                            self.printer.info("- invalid amount of beneficiaries for comment, no match")
-                    else:
-                        self.printer.notice("- at least one of the beneficiaries listed is unknown and unexpected, no match")
-                else:
-                    self.printer.info("Paid out already, no match")
+                candidate = self._comment_is_candidate(comment, author)
         if candidate is None or candidate[0] is None or candidate[1] is None:
             # If no candidate was found, we create our own comment.
             self.printer.notice("No candidate comments found, creating a new comment")
             # Calculate the per-tool-author share.
             code_author_share = int(self.tool_creator_share * 100 / len(AUTHORS))
             # Calculate the share for the blog author
             post_author_share = 10000 - len(AUTHORS) * code_author_share
@@ -241,58 +250,67 @@
                 self.voter.vote(candidate[0], candidate[1],weight)
 
 class Archology:
     """The core personal HIVE-Archeology bot"""
     def __init__(self, account, wif, tool_creator_share, curation_rewards, printer, slow): # pylint: disable=too-many-arguments
         self.account = account
         headno = None
-        while headno is None:
+        while headno is None:  # pylint: disable=while-used
             try:
                 headno = Client().get_dynamic_global_properties()["head_block_number"]
             except RPCNodeException as exp:
                 printer.error(exp)
                 time.sleep(5)
+            except KeyError as exp:
+                printer.error(exp)
+                time.sleep(5)
         self.next = headno - 100
         self.prnt = printer
         self.slow = slow
         self.voter = Voter(account, wif, printer)
         self.commenter = Commenter(self.voter, account, wif, tool_creator_share, curation_rewards, printer)
 
     def upto_head(self): # pylint: disable=too-many-branches
         """Process new blocks upto head"""
         # Keep track of time spent in this method call
         start_time = time.time()
         # Get the current head block number for the HIVE chain
         headno = None
-        while headno is None:
+        while headno is None:  # pylint: disable=while-used
             try:
                 headno = Client().get_dynamic_global_properties()["head_block_number"]
             except RPCNodeException as exp:
                 self.prnt.error(exp)
                 time.sleep(5)
+            except KeyError as exp:
+                self.prnt.error(exp)
+                time.sleep(5)
         # Figure out how many blocks we need to process
         blocks_left = headno + 1 - self.next
         # Process blocks in groups of at most 100
-        while blocks_left !=0: # pylint: disable=too-many-nested-blocks
+        while blocks_left > 0: # pylint: disable=too-many-nested-blocks, while-used
             # Figure out if we need to process 100 blocks or less
             if blocks_left > 100:
                 count = 100
                 blocks_left -= 100
             else:
                 count = blocks_left
                 blocks_left = 0
             # Fetch the number of blocks that we need to process this time around
             blocks = None
             self.prnt.info("fetching blocks, count =", count)
-            while blocks is None:
+            while blocks is None:  # pylint: disable=while-used
                 try:
                     blocks = Client()('block_api').get_block_range({"starting_block_num": self.next, "count":count})["blocks"]
                 except RPCNodeException as exp:
                     self.prnt.error(exp)
                     time.sleep(5)
+                except KeyError as exp:
+                    self.prnt.error(exp)
+                    time.sleep(5)
             # Process the blocks one by one
             for block in blocks:
                 if "transactions" in block:
                     for trans in block.get("transactions", []):
                         if "operations" in  trans:
                             # Process all the operations
                             for operation in  trans.get("operations", []):
@@ -323,23 +341,19 @@
             if blocks_left:
                 time.sleep(1)
         # Return the time it took to process up to head.
         return time.time() - start_time
 
     def run(self):
         """Main run function for the bot"""
-        while True:
+        while True:  # pylint: disable=while-used
             # Process all blocks upto head
             duration = self.upto_head()
             # If processing took less than 10 seconds, sleep for a bit
-            if self.slow:
-                sleeptime = 100 - duration
-            else:
-                sleeptime = 10 - duration
-            if sleeptime > 0:
+            if (sleeptime := 100 - duration if self.slow else 10 - duration):
                 self.prnt.info("waiting for :", sleeptime)
                 time.sleep(sleeptime)
             # Do at most one pending vote that is waiting long enough
             self.voter.tick()
 
 class Print:
     """Utility class for simple logging"""
@@ -387,14 +401,16 @@
     parser.add_argument("--wif",
                         help="WIF of the posting key for the user the tool runs under (default to env usage)")
     parser.add_argument("--slow",
                         help="Poll new blocks every 100 seconds instead of every 10 seconds",
                         action="store_true")
     args = parser.parse_args()
     account = args.account
+    if account == ".":
+        account = os.environ.get("HIVE_ARCHEOLOGY_USER", ".")
     wif = args.wif
     if wif is None:
         wif = os.environ.get(account.upper() + "_WIF",os.environ.get("HIVE_ARCHEOLOGY_WIF",None))
     if wif is None:
         wif = input("Posting key WIF for "+ account + ":").rstrip('\r\n')
     tool_creator_share = args.tool_creator_share
     # Creator share can not be set lower than 0% and not higher than 20% .
```

### Comparing `hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/PKG-INFO` & `hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.4
+Version: 0.1.5
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
 Platform: UNKNOWN
```

### Comparing `hive-archeology-bot-0.1.4/setup.py` & `hive-archeology-bot-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    install_requires=["lighthive"],
+    install_requires=["lighthive", "dateutil"],
 )
```

