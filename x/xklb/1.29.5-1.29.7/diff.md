# Comparing `tmp/xklb-1.29.5.tar.gz` & `tmp/xklb-1.29.7.tar.gz`

## Comparing `xklb-1.29.5.tar` & `xklb-1.29.7.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.5/.gitattributes
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 xklb-1.29.5/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.5/Windows.md
--rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.5/pdm.lock
--rw-r--r--   0        0        0    19035 2020-02-02 00:00:00.000000 xklb-1.29.5/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.5/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.5/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/__init__.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/books.py
--rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/consts.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/dl_config.py
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/dl_extract.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/gui.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/hn_extract.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/lb.py
--rw-r--r--   0        0        0    24360 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/playback.py
--rw-r--r--   0        0        0    32804 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/player.py
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/praw_extract.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/search.py
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/stats.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/subtitle.py
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/tabs_extract.py
--rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/tube_backend.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/tube_extract.py
--rw-r--r--   0        0        0    54097 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/usage.py
--rw-r--r--   0        0        0    34324 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.5/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.5/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.5/LICENSE
--rw-r--r--   0        0        0    76267 2020-02-02 00:00:00.000000 xklb-1.29.5/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.5/pyproject.toml
--rw-r--r--   0        0        0    79863 2020-02-02 00:00:00.000000 xklb-1.29.5/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.29.7/.gitattributes
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 xklb-1.29.7/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.29.7/Windows.md
+-rw-r--r--   0        0        0   486777 2020-02-02 00:00:00.000000 xklb-1.29.7/pdm.lock
+-rw-r--r--   0        0        0    19042 2020-02-02 00:00:00.000000 xklb-1.29.7/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.29.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.29.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.29.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.29.7/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.29.7/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/__init__.py
+-rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/books.py
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/consts.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/dl_config.py
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/gui.py
+-rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/lb.py
+-rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/playback.py
+-rw-r--r--   0        0        0    33325 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/player.py
+-rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/search.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/subtitle.py
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    23484 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/tube_extract.py
+-rw-r--r--   0        0        0    54188 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/usage.py
+-rw-r--r--   0        0        0    33490 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.29.7/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.29.7/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.29.7/LICENSE
+-rw-r--r--   0        0        0    76377 2020-02-02 00:00:00.000000 xklb-1.29.7/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.29.7/pyproject.toml
+-rw-r--r--   0        0        0    79973 2020-02-02 00:00:00.000000 xklb-1.29.7/PKG-INFO
```

### Comparing `xklb-1.29.5/Windows.md` & `xklb-1.29.7/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/pdm.lock` & `xklb-1.29.7/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/readme.py` & `xklb-1.29.7/readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ("Add reddit media", "redditadd"),
     ("Create / Update a Hacker News database", "hnadd"),
     ("Add tabs", "tabsadd"),
     ("Watch / Listen", "watch"),
     ("Search captions / subtitles", "search"),
     ("Open tabs", "tabs"),
     ("Download media", "download"),
-    ("Show Download Status", "dlstatus"),
+    ("Show Download Status", "download_status"),
     ("Update local media", "fsupdate"),
     ("Update online media", "tubeupdate"),
     ("Update reddit media", "redditupdate"),
     ("Convert pushshift data to reddit.db format", "pushshift"),
     ("List playlists", "playlists"),
     ("Blocklist a channel", "block"),
     ("Show large folders", "bigdirs"),
```

### Comparing `xklb-1.29.5/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.29.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.29.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/.github/workflows/push.yaml` & `xklb-1.29.7/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/sql/transfer.sql` & `xklb-1.29.7/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/av.py` & `xklb-1.29.7/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/books.py` & `xklb-1.29.7/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/consts.py` & `xklb-1.29.7/xklb/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import enum, os, re, secrets, string, sys
+import os, re, secrets, string, sys
 from datetime import datetime, timezone
 from pathlib import Path
 from tempfile import gettempdir
 from types import SimpleNamespace
 from typing import List
 
 
@@ -93,29 +93,21 @@
     view = "view"
     download = "download"
     block = "block"
     stats = "stats"
     search = "search"
 
 
-class Frequency(enum.Enum):
-    Daily = "daily"
-    Weekly = "weekly"
-    Monthly = "monthly"
-    Quarterly = "quarterly"
-    Yearly = "yearly"
-
-
-def reddit_frequency(frequency: Frequency) -> str:
+def reddit_frequency(frequency) -> str:
     mapper = {
-        Frequency.Daily: "day",
-        Frequency.Weekly: "week",
-        Frequency.Monthly: "month",
-        Frequency.Quarterly: "year",
-        Frequency.Yearly: "year",
+        "daily": "day",
+        "weekly": "week",
+        "monthly": "month",
+        "quarterly": "year",
+        "yearly": "year",
     }
 
     return mapper[frequency]
 
 
 TEXTRACT_EXTENSIONS = "csv|tab|tsv|doc|docx|eml|epub|json|htm|html|msg|odt|pdf|pptx|ps|rtf|txt|log|xlsx|xls".split("|")
 SPEECH_RECOGNITION_EXTENSIONS = "mp3|ogg|wav".split("|")
@@ -180,14 +172,31 @@
         extensions.extend(OCR_EXTENSIONS)
     if speech_recognition:
         extensions.extend(SPEECH_RECOGNITION_EXTENSIONS)
 
     return get_files(path, extensions)
 
 
+time_facets = [
+    "watching",
+    "watched",
+    "deleted",
+    "created",
+    "modified",
+]
+
+frequency = [
+    "daily",
+    "weekly",
+    "monthly",
+    "quarterly",
+    "yearly",
+]
+
+
 TUBE_IGNORE_KEYS = (
     "track_id",
     "track_number",
     "repost_count",
     "fragments",
     "thumbnail",
     "thumbnails",
```

### Comparing `xklb-1.29.5/xklb/db.py` & `xklb-1.29.7/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/dl_config.py` & `xklb-1.29.7/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/dl_extract.py` & `xklb-1.29.7/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/fs_extract.py` & `xklb-1.29.7/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/gui.py` & `xklb-1.29.7/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/hn_extract.py` & `xklb-1.29.7/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/lb.py` & `xklb-1.29.7/xklb/lb.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 from xklb.playback import playback_next, playback_now, playback_pause, playback_stop
 from xklb.praw_extract import reddit_add, reddit_update
 from xklb.scripts.bigdirs import bigdirs
 from xklb.scripts.christen import christen
 from xklb.scripts.cluster_sort import cluster_sort
 from xklb.scripts.copy_play_counts import copy_play_counts
 from xklb.scripts.dedupe import dedupe
+from xklb.scripts.download_status import download_status
+from xklb.scripts.history import history
 from xklb.scripts.merge_dbs import merge_dbs
 from xklb.scripts.merge_online_local import merge_online_local
 from xklb.scripts.mining.extract_links import extract_links
 from xklb.scripts.mining.nouns import nouns
 from xklb.scripts.mining.pushshift import pushshift_extract
 from xklb.scripts.mining.reddit_selftext import reddit_selftext
 from xklb.scripts.move_list import move_list
 from xklb.scripts.optimize_db import optimize_db
+from xklb.scripts.playlists import playlists
 from xklb.scripts.redownload import redownload
 from xklb.scripts.relmv import relmv
 from xklb.scripts.scatter import scatter
 from xklb.scripts.streaming_tab_loader import streaming_tab_loader
 from xklb.search import search
-from xklb.stats import dlstatus, playlists
 from xklb.tabs_actions import tabs
 from xklb.tabs_extract import tabs_add
 from xklb.tube_extract import tube_add, tube_update
 from xklb.utils import log
 
 
 def usage() -> str:
@@ -74,17 +76,18 @@
     playback:
       lb now                   Print what is currently playing
       lb next                  Play next file
       lb stop                  Stop all playback
       lb pause                 Pause all playback
 
     statistics:
+      lb history               Show some playback statistics
       lb playlists             List added playlists
-      lb dlstatus              Show download status
-      lb usage                 Print mount usage
+      lb download-status       Show download status
+      lb disk-usage            Print mount usage
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
     mining:
@@ -194,17 +197,19 @@
     subp_block = add_parser(subparsers, "block")
     subp_block.set_defaults(func=dl_block)
     subp_redownload = add_parser(subparsers, "redownload", ["redl"])
     subp_redownload.set_defaults(func=redownload)
 
     subp_playlist = add_parser(subparsers, "playlists", ["pl", "folders"])
     subp_playlist.set_defaults(func=playlists)
-    subp_dlstatus = add_parser(subparsers, "dlstatus", ["ds"])
-    subp_dlstatus.set_defaults(func=dlstatus)
-    subp_usage = add_parser(subparsers, "usage", ["du"])
+    subp_history = add_parser(subparsers, "history", ["hi", "log"])
+    subp_history.set_defaults(func=history)
+    subp_download_status = add_parser(subparsers, "download-status", ["ds", "dlstatus"])
+    subp_download_status.set_defaults(func=download_status)
+    subp_usage = add_parser(subparsers, "disk-usage", ["du", "usage", "mount-stats"])
     subp_usage.set_defaults(func=utils.mount_stats)
 
     subp_playback_now = add_parser(subparsers, "now")
     subp_playback_now.set_defaults(func=playback_now)
     subp_playback_next = add_parser(subparsers, "next")
     subp_playback_next.set_defaults(func=playback_next)
     subp_playback_stop = add_parser(subparsers, "stop")
```

### Comparing `xklb-1.29.5/xklb/play_actions.py` & `xklb-1.29.7/xklb/play_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,60 +478,67 @@
             log.debug("transcode: %s", t.elapsed())
 
     m["now_playing"] = now_playing(m["path"])
 
     return m
 
 
-def play(args, m) -> None:
-    t = utils.Timer()
-    print(m["now_playing"])
-    log.debug("now_playing: %s", t.elapsed())
-
-    args.player = player.parse(args, m)
-    log.debug("player.parse: %s", t.elapsed())
-
-    start_time = time.time()
-    if args.chromecast:
-        try:
-            chromecast_play(args, m)
-        except Exception:
-            if args.ignore_errors:
-                return
-            else:
-                raise
-
-    elif args.interdimensional_cable:
-        player.socket_play(args, m)
-        return
-
-    else:
-        r = player.local_player(args, m)
-        if r.returncode != 0:
-            log.warning("Player exited with code %s", r.returncode)
-            if args.ignore_errors:
-                return
-            else:
-                raise SystemExit(r.returncode)
-
+def save_playhead(args, m, start_time):
     m_columns = args.db["media"].columns_dict
     if "playhead" in m_columns:
         playhead = utils.get_playhead(
             args,
             m["original_path"],
             start_time,
             existing_playhead=m.get("playhead"),
             media_duration=m.get("duration"),
         )
         if playhead:
             player.set_playhead(args, m["original_path"], playhead)
 
-    t.reset()
-    player.post_act(args, m["original_path"])
-    log.debug("player.post_act: %s", t.elapsed())
+
+def play(args, m) -> None:
+    t = utils.Timer()
+    print(m["now_playing"])
+    log.debug("now_playing: %s", t.elapsed())
+
+    args.player = player.parse(args, m)
+    log.debug("player.parse: %s", t.elapsed())
+
+    if args.interdimensional_cable:
+        player.socket_play(args, m)
+        return
+
+    start_time = time.time()
+    try:
+        if args.chromecast:
+            try:
+                chromecast_play(args, m)
+                t.reset()
+                player.post_act(args, m["original_path"])
+                log.debug("player.post_act: %s", t.elapsed())
+            except Exception:
+                if args.ignore_errors:
+                    return
+                else:
+                    raise
+        else:
+            r = player.local_player(args, m)
+            if r.returncode == 0:
+                t.reset()
+                player.post_act(args, m["original_path"])
+                log.debug("player.post_act: %s", t.elapsed())
+            else:
+                log.warning("Player exited with code %s", r.returncode)
+                if args.ignore_errors:
+                    return
+                else:
+                    raise SystemExit(r.returncode)
+    finally:
+        save_playhead(args, m, start_time)
 
 
 def process_playqueue(args) -> None:
     t = utils.Timer()
     query, bindings = construct_query(args)
     log.debug("construct_query: %s", t.elapsed())
```

### Comparing `xklb-1.29.5/xklb/playback.py` & `xklb-1.29.7/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/player.py` & `xklb-1.29.7/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,32 +186,33 @@
 
 
 def set_playhead(args, path: str, playhead: int) -> int:
     with args.db.conn:
         cursor = args.db.conn.execute(
             """UPDATE media
             SET playhead = :playhead
+                , time_played = cast(STRFTIME('%s') as int)
             WHERE path = :path
             """,
             {"playhead": playhead, "path": path},
         )
-        return cursor.rowcount
+    return cursor.rowcount
 
 
 def mark_media_watched(args, files) -> int:
     files = utils.conform(files)
     modified_row_count = 0
     if files:
         df_chunked = utils.chunks(files, consts.SQLITE_PARAM_LIMIT)
         for chunk_paths in df_chunked:
             with args.db.conn:
                 cursor = args.db.conn.execute(
                     """UPDATE media
                     SET play_count = play_count + 1
-                    , time_played = cast(STRFTIME('%s') as int)
+                        , time_played = cast(STRFTIME('%s') as int)
                     WHERE path in ("""
                     + ",".join(["?"] * len(chunk_paths))
                     + ")",
                     (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
@@ -641,23 +642,23 @@
     else:  # tall or square: prefer horizontal split
         return True
 
 
 def modify_display_size_for_taskbar(display):
     try:
         if platform.system() == "Windows":
-            import win32gui
+            import win32gui  # type: ignore
 
             taskbar_window_handle = win32gui.FindWindow("Shell_TrayWnd", None)
             if taskbar_window_handle == 0:
                 taskbar_window_handle = win32gui.FindWindow("Shell_SecondaryTrayWnd", None)
             if taskbar_window_handle == 0:
                 return display
 
-            work_area = win32gui.GetMonitorInfo(taskbar_window_handle)["rcWork"]
+            work_area = win32gui.GetMonitorInfo(taskbar_window_handle)["rcWork"]  # type: ignore
 
             _taskbar_height = display.height - work_area[3]
             display.height = work_area[3] - work_area[1]
             display.width = work_area[2] - work_area[0]
 
         elif platform.system() == "Linux":
             xprop_output = subprocess.check_output("xprop -root _NET_WORKAREA".split()).decode().strip()
@@ -804,35 +805,47 @@
             else:
                 delay = 10  # TODO: idk
             sleep(delay)
 
     return r
 
 
-def historical_usage(args):
-    query = """
+def historical_usage(args, freq="monthly", time_column="time_played", where=""):
+    if freq == "daily":
+        time_format = "%Y-%m-%d"
+    elif freq == "weekly":
+        time_format = "%Y-%W"
+    elif freq == "monthly":
+        time_format = "%Y-%m"
+    elif freq == "yearly":
+        time_format = "%Y"
+    else:
+        raise ValueError(f"Invalid value for 'freq': {freq}")
+
+    query = f"""
     SELECT
-        strftime('%Y-%m-%d', datetime(time_played, 'unixepoch')) AS day
+        strftime('{time_format}', datetime({time_column}, 'unixepoch')) AS time_period
         , SUM(duration) AS duration_sum
         , AVG(duration) AS duration_avg
         , SUM(size) AS size_sum
         , AVG(size) AS size_avg
-    FROM media where time_played>0
-    GROUP BY day
+    FROM media
+    WHERE coalesce(time_period, 0)>0 and {time_column}>0 {where}
+    GROUP BY time_period
     """
     return list(args.db.query(query))
 
 
 def cadence_adjusted_duration(args, duration):
     try:
         historical_daily = statistics.mean((d["duration_sum"] or 0) for d in historical_usage(args))
     except statistics.StatisticsError:
         return duration
 
-    return duration / historical_daily * 86400
+    return duration / historical_daily * 86400 * 30.42
 
 
 def media_printer(args, media) -> None:
     if "b" in args.print:
         media = process_bigdirs(args, media)
 
     if args.verbose >= consts.LOG_DEBUG and args.cols and "*" in args.cols:
```

### Comparing `xklb-1.29.5/xklb/praw_extract.py` & `xklb-1.29.7/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/search.py` & `xklb-1.29.7/xklb/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         nargs="?",
         help="Experimental escape hatch to open a folder glob limited to x number of files",
     )
 
     parser.add_argument("--ignore-errors", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--online-media-only", "--online-only", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--local-media-only", "--local-only", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--only-paths", "--paths", "--files-with-matches", action="store_true", help="Only print paths")
+
     parser.add_argument("--loop", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--override-player", "--player", "-player", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     parser.add_argument("search", nargs="*")
@@ -70,15 +70,15 @@
     captions = utils.list_dict_filter_bool(captions)
     if not captions:
         utils.no_media_found()
 
     tbl = deepcopy(captions)
     utils.col_hhmmss(tbl, "time")
 
-    if args.only_paths:
+    if args.print and "f" in args.print:
         pipe_print("\n".join([d["path"] for d in captions]))
         return
     elif args.json or consts.TERMINAL_SIZE.columns < 80:
         print(json.dumps(tbl, indent=3))
     elif args.csv:
         utils.write_csv_to_stdout(tbl)
     elif args.table:
```

### Comparing `xklb-1.29.5/xklb/stats.py` & `xklb-1.29.7/xklb/scripts/download_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,43 +2,41 @@
 from copy import deepcopy
 from typing import Tuple
 
 from tabulate import tabulate
 
 from xklb import consts, db, dl_extract, play_actions, tube_backend, usage, utils
 from xklb.player import delete_playlists
-from xklb.utils import human_time, log, pipe_print
+from xklb.utils import log
 
 
-def parse_args(prog, usage) -> argparse.Namespace:
+def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog,
-        usage,
+        "library download-status",
+        usage=usage.download_status,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--fields", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--aggregate", "-a", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--json", "-j", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", help=argparse.SUPPRESS)
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--errors", "-errors", "--error", action="store_true", help="Show only rows with errors")
     parser.add_argument("--delete", "--remove", "--erase", "--rm", "-rm", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--print", "-p", default=False, const="p", nargs="?", help=argparse.SUPPRESS)
-    if "dlstatus" in prog:
-        parser.add_argument(
-            "--retry-delay",
-            "-r",
-            default="14 days",
-            help="Must be specified in SQLITE Modifiers format: N hours, days, months, or years",
-        )
+    parser.add_argument(
+        "--retry-delay",
+        "-r",
+        default="14 days",
+        help="Must be specified in SQLITE Modifiers format: N hours, days, months, or years",
+    )
 
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     args = parser.parse_args()
     if args.db:
@@ -93,16 +91,16 @@
 
     tbl = deepcopy(media)
     utils.col_naturaldate(tbl, "avg_time_since_download")
     utils.col_naturalsize(tbl, "size")
     utils.col_duration(tbl, "duration")
     utils.col_duration(tbl, "avg_playlist_duration")
 
-    if args.fields:
-        pipe_print("\n".join([d["path"] for d in media]))
+    if args.print and "f" in args.print:
+        utils.pipe_print("\n".join([d["path"] for d in media]))
         return
     elif args.json or consts.TERMINAL_SIZE.columns < 80:
         print(json.dumps(tbl, indent=3))
     else:
         tbl = utils.col_resize(tbl, "path", 30)
         tbl = utils.col_resize(tbl, "title", 20)
         tbl = utils.col_resize(tbl, "uploader_url")
@@ -110,66 +108,21 @@
         tbl = utils.list_dict_filter_bool(tbl)
 
         print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
     print(f"{len(media)} playlists" if len(media) > 1 else "1 playlist")
     duration = sum(m.get("duration") or 0 for m in media)
     if duration > 0:
-        duration = human_time(duration)
+        duration = utils.human_time(duration)
         if not args.aggregate:
             print("Total duration:", duration)
 
 
-def playlists() -> None:
-    args = parse_args(prog="library playlists", usage=usage.playlists)
-
-    if args.delete:
-        return delete_playlists(args, args.delete)
-
-    pl_columns = args.db["playlists"].columns_dict
-    m_columns = args.db["media"].columns_dict
-    query, bindings = construct_query(args)
-
-    if "playlist_path" in m_columns:
-        query = f"""
-        select
-            coalesce(p.path, "Playlist-less media") path
-            {', p.ie_key' if 'ie_key' in pl_columns else ''}
-            {', p.title' if 'title' in pl_columns else ''}
-            {', p.time_deleted' if 'time_deleted' in pl_columns else ''}
-            {', count(*) FILTER(WHERE play_count>0) play_count' if 'play_count' in m_columns else ''}
-            {', sum(m.duration) duration' if 'duration' in m_columns else ''}
-            {', sum(m.size) size' if 'size' in m_columns else ''}
-            , count(*) count
-        from media m
-        left join ({query}) p on (p.path = m.playlist_path {"and p.ie_key = m.ie_key and m.ie_key != 'Local'" if 'ie_key' in m_columns else ''})
-        group by coalesce(p.path, "Playlist-less media")
-        order by count, p.category nulls last, p.path
-        """
-
-    if args.aggregate:
-        query = f"""
-        select
-            'Aggregate of playlists' path
-            {', count(*) FILTER(WHERE time_deleted>0) deleted_count' if 'time_deleted' in query else ''}
-            {', sum(play_count) play_count' if 'play_count' in query else ''}
-            {', sum(duration) duration' if 'duration' in query else ''}
-            {', avg(duration) avg_playlist_duration' if 'duration' in query else ''}
-            {', sum(size) size' if 'size' in query else ''}
-            , count(*) playlists_count
-            {', sum(count) videos_count' if 'count' in query else ''}
-        from ({query})
-        """
-
-    printer(args, query, bindings)
-    return None
-
-
-def dlstatus() -> None:
-    args = parse_args(prog="library dlstatus", usage=usage.dlstatus)
+def download_status() -> None:
+    args = parse_args()
     play_actions.parse_args_sort(args)
 
     if args.delete:
         return delete_playlists(args, args.delete)
 
     query, bindings = dl_extract.construct_query(args)
```

### Comparing `xklb-1.29.5/xklb/subtitle.py` & `xklb-1.29.7/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/tabs_actions.py` & `xklb-1.29.7/xklb/tabs_actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from pathlib import Path
 from time import sleep
 from typing import Dict, List, Tuple
 
 from xklb import db, usage, utils
 from xklb.consts import SC
 from xklb.player import generic_player, mark_media_watched, override_sort, printer
-from xklb.tabs_extract import Frequency
 from xklb.utils import cmd, flatten, log
 
 
 def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library tabs", formatter_class=argparse.ArgumentDefaultsHelpFormatter, usage=usage.tabs
     )
@@ -132,19 +131,19 @@
 
     cmd(*generic_player(args), media_file, strict=False)
     mark_media_watched(args, [media_file])
 
 
 def frequency_filter(args, media: List[Dict]) -> List[dict]:
     mapper = {
-        Frequency.Daily.value: 1,
-        Frequency.Weekly.value: 7,
-        Frequency.Monthly.value: 30,
-        Frequency.Quarterly.value: 91,
-        Frequency.Yearly.value: 365,
+        "daily": 1,
+        "weekly": 7,
+        "monthly": 30,
+        "quarterly": 91,
+        "yearly": 365,
     }
     counts = args.db.execute("select frequency, count(*) from media group by 1").fetchall()
     filtered_media = []
     for freq, freq_count in counts:
         num_days = mapper.get(freq, 365)
         num_tabs = max(1, freq_count // num_days)
         log.debug(f"freq_count {freq_count} // num_days {num_days} = num_tabs {num_tabs}")
```

### Comparing `xklb-1.29.5/xklb/tabs_extract.py` & `xklb-1.29.7/xklb/tabs_extract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import argparse, sys
 from pathlib import Path
 from typing import List
 
 from xklb import consts, db, player, usage, utils
-from xklb.consts import Frequency
-from xklb.utils import ArgparseEnum, log, sanitize_url
+from xklb.utils import log, sanitize_url
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library tabsadd", usage=usage.tabsadd)
     parser.add_argument(
         "--frequency",
         "--freqency",
         "-f",
-        default=Frequency.Monthly,
-        type=Frequency,
-        action=ArgparseEnum,
-        help=argparse.SUPPRESS,
+        metavar="frequency",
+        choices=consts.frequency,
+        default="monthly",
+        const="monthly",
+        type=str.lower,
+        nargs="?",
+        help=f"One of: %(choices)s (default: %(default)s)",
     )
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
@@ -70,15 +72,15 @@
     from urllib.parse import urlparse
 
     hostname = urlparse(path).hostname or ""
 
     return {
         "path": path,
         "hostname": hostname,
-        "frequency": args.frequency.value,
+        "frequency": args.frequency,
         "category": args.category or "Uncategorized",
         "time_created": consts.APPLICATION_START,
         "time_played": 0,
         "play_count": 0,
         "time_deleted": 0,
     }
```

### Comparing `xklb-1.29.5/xklb/tube_backend.py` & `xklb-1.29.7/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/tube_extract.py` & `xklb-1.29.7/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/usage.py` & `xklb-1.29.7/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     Print list of saved playlists
 
         library playlists dl.db -p a
 
     Print download queue groups
 
-        library dlstatus audio.db
+        library download-status audio.db
         ╒═════════════════════╤════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key     │ duration         │   never_downloaded │   errors │
         ╞═════════════════════╪════════════╪══════════════════╪════════════════════╪══════════╡
         │ 81_New_Music        │ Soundcloud │                  │                 10 │        0 │
         ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
         │ 81_New_Music        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
         │                     │            │ and 20 minutes   │                    │          │
@@ -419,14 +419,20 @@
            34:52 Who will give her a one liter stainless steel boiler for one Lari?
            34:54 Glass boilers cost two
 
     Search and open file
     $ library search fts.db dashi --open
 """
 
+history = """library history [database]
+
+
+
+"""
+
 playlists = """library playlists [database] [--aggregate] [--fields] [--json] [--delete ...]
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
         │ ie_key   │ title              │ path                                                                     │
@@ -450,19 +456,20 @@
         library playlists -p f
         https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n
 
     Remove a playlist/channel and all linked videos:
         library playlists --remove https://vimeo.com/canal180
 
 """
-dlstatus = """library dlstatus [database]
+
+download_status = """library download-status [database]
 
     Print download queue groups
 
-        library dlstatus video.db
+        library download-status video.db
         ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
         ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
         │ 71_Mealtime_Videos  │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
         │                     │             │ minutes          │                    │          │
         ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
         │ 75_MovieQueue       │ Dailymotion │                  │                 53 │        0 │
@@ -484,19 +491,19 @@
         │ Playlist-less media │ Youtube     │ 4 months, 23     │               2686 │        7 │
         │                     │             │ days, 19 hours   │                    │          │
         │                     │             │ and 33 minutes   │                    │          │
         ╘═════════════════════╧═════════════╧══════════════════╧════════════════════╧══════════╛
 
     Simulate --safe flag
 
-        library dlstatus video.db --safe
+        library download-status video.db --safe
 
     Show only download attempts with errors
 
-        library dlstatus video.db --errors
+        library download-status video.db --errors
 """
 
 tabs = """library tabs DATABASE
 
     Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
 
         45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
```

### Comparing `xklb-1.29.5/xklb/utils.py` & `xklb-1.29.7/xklb/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     raise SystemExit(2)
 
 
 def sanitize_url(args, path: str) -> str:
     matches = consts.REGEX_SUBREDDIT.match(path)
     if matches:
         subreddit = conform(matches.groups())[0]
-        frequency = consts.Frequency.Monthly
+        frequency = "monthly"
         if hasattr(args, "frequency"):
             frequency = args.frequency
         return "https://old.reddit.com/r/" + subreddit + "/top/?sort=top&t=" + consts.reddit_frequency(frequency)
 
     if "/m." in path:
         return path.replace("/m.", "/www.")
 
@@ -740,38 +740,14 @@
 
         except ValueError as ex:
             msg = f'Could not parse argument "{values}" as k1=1 k2=2 format {ex}'
             raise argparse.ArgumentError(self, msg) from ex
         setattr(args, self.dest, d)
 
 
-class ArgparseEnum(argparse.Action):
-    def __init__(self, **kwargs) -> None:
-        # Pop off the type value
-        enum_type = kwargs.pop("type", None)
-
-        # Ensure an Enum subclass is provided
-        if enum_type is None:
-            raise ValueError("type must be assigned an Enum when using EnumAction")
-        if not issubclass(enum_type, enum.Enum):
-            raise TypeError("type must be an Enum when using EnumAction")
-
-        # Generate choices from the Enum
-        kwargs.setdefault("choices", tuple(e.value for e in enum_type))
-
-        super().__init__(**kwargs)
-
-        self._enum = enum_type
-
-    def __call__(self, parser, namespace, values, option_string=None):
-        # Convert value back into an Enum
-        value = self._enum(values)
-        setattr(namespace, self.dest, value)
-
-
 def filter_namespace(args, config_opts) -> Optional[Dict]:
     return dict_filter_bool({k: v for k, v in args.__dict__.items() if k in config_opts})
 
 
 def ensure_playlists_exists(args) -> None:
     if "playlists" not in args.db.table_names():
         with args.db.conn:
```

### Comparing `xklb-1.29.5/xklb/scripts/bigdirs.py` & `xklb-1.29.7/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/christen.py` & `xklb-1.29.7/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/cluster_sort.py` & `xklb-1.29.7/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/copy_play_counts.py` & `xklb-1.29.7/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/dedupe.py` & `xklb-1.29.7/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/merge_dbs.py` & `xklb-1.29.7/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/merge_online_local.py` & `xklb-1.29.7/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/move_list.py` & `xklb-1.29.7/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/optimize_db.py` & `xklb-1.29.7/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/redownload.py` & `xklb-1.29.7/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/relmv.py` & `xklb-1.29.7/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/scatter.py` & `xklb-1.29.7/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/streaming_tab_loader.py` & `xklb-1.29.7/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/mining/data.py` & `xklb-1.29.7/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/mining/extract_links.py` & `xklb-1.29.7/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/mining/nouns.py` & `xklb-1.29.7/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/mining/pushshift.py` & `xklb-1.29.7/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.29.7/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/xklb/assets/kotobago.png` & `xklb-1.29.7/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/.gitignore` & `xklb-1.29.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/LICENSE` & `xklb-1.29.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/README.md` & `xklb-1.29.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.005)
+    xk media library subcommands (v1.29.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -183,17 +183,18 @@
     playback:
       lb now                   Print what is currently playing
       lb next                  Play next file
       lb stop                  Stop all playback
       lb pause                 Pause all playback
 
     statistics:
+      lb history               Show some playback statistics
       lb playlists             List added playlists
-      lb dlstatus              Show download status
-      lb usage                 Print mount usage
+      lb download-status       Show download status
+      lb disk-usage            Print mount usage
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
     mining:
@@ -1058,37 +1059,37 @@
 
     Print list of saved playlists
 
         library playlists dl.db -p a
 
     Print download queue groups
 
-        library dlstatus audio.db
+        library download-status audio.db
         ╒═════════════════════╤════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key     │ duration         │   never_downloaded │   errors │
         ╞═════════════════════╪════════════╪══════════════════╪════════════════════╪══════════╡
         │ 81_New_Music        │ Soundcloud │                  │                 10 │        0 │
         ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
         │ 81_New_Music        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
         │                     │            │ and 20 minutes   │                    │          │
         ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
         │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
         ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
 
 
 </details>
 
-<details><summary>Show Download Status (dlstatus)</summary>
+<details><summary>Show Download Status (download_status)</summary>
 
-    $ library dlstatus -h
-    usage: library dlstatus [database]
+    $ library download_status -h
+    usage: library download-status [database]
 
     Print download queue groups
 
-        library dlstatus video.db
+        library download-status video.db
         ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
         ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
         │ 71_Mealtime_Videos  │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
         │                     │             │ minutes          │                    │          │
         ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
         │ 75_MovieQueue       │ Dailymotion │                  │                 53 │        0 │
@@ -1110,19 +1111,19 @@
         │ Playlist-less media │ Youtube     │ 4 months, 23     │               2686 │        7 │
         │                     │             │ days, 19 hours   │                    │          │
         │                     │             │ and 33 minutes   │                    │          │
         ╘═════════════════════╧═════════════╧══════════════════╧════════════════════╧══════════╛
 
     Simulate --safe flag
 
-        library dlstatus video.db --safe
+        library download-status video.db --safe
 
     Show only download attempts with errors
 
-        library dlstatus video.db --errors
+        library download-status video.db --errors
 
 
 </details>
 
 <details><summary>Update local media (fsupdate)</summary>
 
     $ library fsupdate -h
```

### Comparing `xklb-1.29.5/pyproject.toml` & `xklb-1.29.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.29.5/PKG-INFO` & `xklb-1.29.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.29.5
+Version: 1.29.7
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -223,15 +223,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.29.005)
+    xk media library subcommands (v1.29.007)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -267,17 +267,18 @@
     playback:
       lb now                   Print what is currently playing
       lb next                  Play next file
       lb stop                  Stop all playback
       lb pause                 Pause all playback
 
     statistics:
+      lb history               Show some playback statistics
       lb playlists             List added playlists
-      lb dlstatus              Show download status
-      lb usage                 Print mount usage
+      lb download-status       Show download status
+      lb disk-usage            Print mount usage
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
     mining:
@@ -1142,37 +1143,37 @@
 
     Print list of saved playlists
 
         library playlists dl.db -p a
 
     Print download queue groups
 
-        library dlstatus audio.db
+        library download-status audio.db
         ╒═════════════════════╤════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key     │ duration         │   never_downloaded │   errors │
         ╞═════════════════════╪════════════╪══════════════════╪════════════════════╪══════════╡
         │ 81_New_Music        │ Soundcloud │                  │                 10 │        0 │
         ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
         │ 81_New_Music        │ Youtube    │ 10 days, 4 hours │                  1 │     2555 │
         │                     │            │ and 20 minutes   │                    │          │
         ├─────────────────────┼────────────┼──────────────────┼────────────────────┼──────────┤
         │ Playlist-less media │ Youtube    │ 7.68 minutes     │                 99 │        1 │
         ╘═════════════════════╧════════════╧══════════════════╧════════════════════╧══════════╛
 
 
 </details>
 
-<details><summary>Show Download Status (dlstatus)</summary>
+<details><summary>Show Download Status (download_status)</summary>
 
-    $ library dlstatus -h
-    usage: library dlstatus [database]
+    $ library download_status -h
+    usage: library download-status [database]
 
     Print download queue groups
 
-        library dlstatus video.db
+        library download-status video.db
         ╒═════════════════════╤═════════════╤══════════════════╤════════════════════╤══════════╕
         │ category            │ ie_key      │ duration         │   never_downloaded │   errors │
         ╞═════════════════════╪═════════════╪══════════════════╪════════════════════╪══════════╡
         │ 71_Mealtime_Videos  │ Youtube     │ 3 hours and 2.07 │                 76 │        0 │
         │                     │             │ minutes          │                    │          │
         ├─────────────────────┼─────────────┼──────────────────┼────────────────────┼──────────┤
         │ 75_MovieQueue       │ Dailymotion │                  │                 53 │        0 │
@@ -1194,19 +1195,19 @@
         │ Playlist-less media │ Youtube     │ 4 months, 23     │               2686 │        7 │
         │                     │             │ days, 19 hours   │                    │          │
         │                     │             │ and 33 minutes   │                    │          │
         ╘═════════════════════╧═════════════╧══════════════════╧════════════════════╧══════════╛
 
     Simulate --safe flag
 
-        library dlstatus video.db --safe
+        library download-status video.db --safe
 
     Show only download attempts with errors
 
-        library dlstatus video.db --errors
+        library download-status video.db --errors
 
 
 </details>
 
 <details><summary>Update local media (fsupdate)</summary>
 
     $ library fsupdate -h
```

