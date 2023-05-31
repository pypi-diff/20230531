# Comparing `tmp/llama_hub-0.0.1a1.tar.gz` & `tmp/llama_hub-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_hub-0.0.1a1.tar", max compression
+gzip compressed data, was "llama_hub-0.0.1a2.tar", max compression
```

## Comparing `llama_hub-0.0.1a1.tar` & `llama_hub-0.0.1a2.tar`

### file list

```diff
@@ -1,437 +1,438 @@
--rw-r--r--   0        0        0     1064 2023-04-18 06:55:56.425923 llama_hub-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     5492 2023-05-30 03:31:15.933992 llama_hub-0.0.1a1/README.md
--rw-r--r--   0        0        0      247 2023-03-07 03:10:58.610114 llama_hub-0.0.1a1/llama_hub/README.md
--rw-r--r--   0        0        0       17 2023-03-12 01:04:01.850402 llama_hub-0.0.1a1/llama_hub/__init__.py
--rwxr-xr-x   0        0        0      119 2023-03-07 03:10:58.610243 llama_hub-0.0.1a1/llama_hub/add_loader.sh
--rw-r--r--   0        0        0      826 2023-03-20 16:59:19.504519 llama_hub-0.0.1a1/llama_hub/airtable/README.md
--rw-r--r--   0        0        0       17 2023-03-20 16:59:19.504658 llama_hub-0.0.1a1/llama_hub/airtable/__init__.py
--rw-r--r--   0        0        0      901 2023-04-26 20:58:33.742027 llama_hub-0.0.1a1/llama_hub/airtable/base.py
--rw-r--r--   0        0        0       10 2023-03-20 16:59:19.504974 llama_hub-0.0.1a1/llama_hub/airtable/requirements.txt
--rw-r--r--   0        0        0     1839 2023-04-18 06:14:21.375487 llama_hub-0.0.1a1/llama_hub/apify/actor/README.md
--rw-r--r--   0        0        0       17 2023-04-18 06:14:21.375572 llama_hub-0.0.1a1/llama_hub/apify/actor/__init__.py
--rw-r--r--   0        0        0     2317 2023-04-18 06:14:21.375684 llama_hub-0.0.1a1/llama_hub/apify/actor/base.py
--rw-r--r--   0        0        0       13 2023-04-18 06:14:21.375790 llama_hub-0.0.1a1/llama_hub/apify/actor/requirements.txt
--rw-r--r--   0        0        0     1499 2023-04-18 06:14:21.375933 llama_hub-0.0.1a1/llama_hub/apify/dataset/README.md
--rw-r--r--   0        0        0       17 2023-04-18 06:14:21.375997 llama_hub-0.0.1a1/llama_hub/apify/dataset/__init__.py
--rw-r--r--   0        0        0     1378 2023-04-18 06:14:21.376110 llama_hub-0.0.1a1/llama_hub/apify/dataset/base.py
--rw-r--r--   0        0        0       13 2023-04-18 06:14:21.376197 llama_hub-0.0.1a1/llama_hub/apify/dataset/requirements.txt
--rw-r--r--   0        0        0      778 2023-03-07 03:10:58.610345 llama_hub-0.0.1a1/llama_hub/asana/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.610410 llama_hub-0.0.1a1/llama_hub/asana/__init__.py
--rw-r--r--   0        0        0     1856 2023-03-07 03:10:58.610497 llama_hub-0.0.1a1/llama_hub/asana/base.py
--rw-r--r--   0        0        0        6 2023-03-07 03:10:58.610554 llama_hub-0.0.1a1/llama_hub/asana/requirements.txt
--rw-r--r--   0        0        0     2200 2023-05-21 16:19:51.397555 llama_hub-0.0.1a1/llama_hub/azcognitive_search/README.md
--rw-r--r--   0        0        0       17 2023-04-13 07:27:29.040381 llama_hub-0.0.1a1/llama_hub/azcognitive_search/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-26 20:58:33.742413 llama_hub-0.0.1a1/llama_hub/azcognitive_search/base.py
--rw-r--r--   0        0        0       37 2023-04-13 07:27:29.040559 llama_hub-0.0.1a1/llama_hub/azcognitive_search/requirements.txt
--rw-r--r--   0        0        0     2542 2023-05-23 05:17:27.298258 llama_hub-0.0.1a1/llama_hub/azstorage_blob/README.md
--rw-r--r--   0        0        0       17 2023-05-23 05:17:27.298366 llama_hub-0.0.1a1/llama_hub/azstorage_blob/__init__.py
--rw-r--r--   0        0        0     5228 2023-05-23 05:17:27.298494 llama_hub-0.0.1a1/llama_hub/azstorage_blob/base.py
--rw-r--r--   0        0        0       34 2023-05-23 05:17:27.298588 llama_hub-0.0.1a1/llama_hub/azstorage_blob/requirements.txt
--rw-r--r--   0        0        0     1077 2023-04-02 07:55:11.891017 llama_hub-0.0.1a1/llama_hub/bilibili/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.610712 llama_hub-0.0.1a1/llama_hub/bilibili/__init__.py
--rw-r--r--   0        0        0     2374 2023-03-07 03:10:58.610781 llama_hub-0.0.1a1/llama_hub/bilibili/base.py
--rw-r--r--   0        0        0       21 2023-03-07 03:10:58.610850 llama_hub-0.0.1a1/llama_hub/bilibili/requirements.txt
--rw-r--r--   0        0        0     3373 2023-05-30 03:31:33.609582 llama_hub-0.0.1a1/llama_hub/boarddocs/BoardDocsReader.ipynb
--rw-r--r--   0        0        0     1402 2023-05-21 16:19:51.397709 llama_hub-0.0.1a1/llama_hub/boarddocs/README.md
--rw-r--r--   0        0        0       17 2023-05-21 16:19:51.397756 llama_hub-0.0.1a1/llama_hub/boarddocs/__init__.py
--rw-r--r--   0        0        0     4430 2023-05-21 16:19:51.397817 llama_hub-0.0.1a1/llama_hub/boarddocs/base.py
--rw-r--r--   0        0        0    19752 2023-05-21 16:19:51.397921 llama_hub-0.0.1a1/llama_hub/boarddocs/crawl.ipynb
--rw-r--r--   0        0        0       22 2023-05-21 16:19:51.397973 llama_hub-0.0.1a1/llama_hub/boarddocs/requirements.txt
--rw-r--r--   0        0        0      921 2023-03-26 16:14:37.560097 llama_hub-0.0.1a1/llama_hub/chatgpt_plugin/README.md
--rw-r--r--   0        0        0       16 2023-04-26 20:58:33.742854 llama_hub-0.0.1a1/llama_hub/chatgpt_plugin/__init__.py
--rw-r--r--   0        0        0     2111 2023-04-26 20:58:33.743460 llama_hub-0.0.1a1/llama_hub/chatgpt_plugin/base.py
--rw-r--r--   0        0        0        0 2023-03-26 16:14:37.560691 llama_hub-0.0.1a1/llama_hub/chatgpt_plugin/requirements.txt
--rw-r--r--   0        0        0     1056 2023-03-26 16:14:37.561036 llama_hub-0.0.1a1/llama_hub/chroma/README.md
--rw-r--r--   0        0        0        0 2023-03-07 03:10:58.611052 llama_hub-0.0.1a1/llama_hub/chroma/__init__.py
--rw-r--r--   0        0        0     1918 2023-03-07 03:10:58.611155 llama_hub-0.0.1a1/llama_hub/chroma/base.py
--rw-r--r--   0        0        0        8 2023-03-07 03:10:58.611218 llama_hub-0.0.1a1/llama_hub/chroma/requirements.txt
--rw-r--r--   0        0        0     2288 2023-04-02 07:55:11.891751 llama_hub-0.0.1a1/llama_hub/confluence/README.md
--rw-r--r--   0        0        0       17 2023-03-22 05:54:30.923061 llama_hub-0.0.1a1/llama_hub/confluence/__init__.py
--rw-r--r--   0        0        0    11384 2023-05-21 16:19:51.398881 llama_hub-0.0.1a1/llama_hub/confluence/base.py
--rw-r--r--   0        0        0       80 2023-04-02 07:55:11.892578 llama_hub-0.0.1a1/llama_hub/confluence/requirements.txt
--rw-r--r--   0        0        0     1052 2023-04-13 07:27:29.040875 llama_hub-0.0.1a1/llama_hub/couchdb/README.md
--rw-r--r--   0        0        0       17 2023-04-13 07:27:29.040924 llama_hub-0.0.1a1/llama_hub/couchdb/__init__.py
--rw-r--r--   0        0        0     2564 2023-05-01 23:46:36.351091 llama_hub-0.0.1a1/llama_hub/couchdb/base.py
--rw-r--r--   0        0        0        9 2023-04-13 07:27:29.041113 llama_hub-0.0.1a1/llama_hub/couchdb/requirements.txt
--rw-r--r--   0        0        0      582 2023-03-07 03:10:58.611321 llama_hub-0.0.1a1/llama_hub/dad_jokes/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.611391 llama_hub-0.0.1a1/llama_hub/dad_jokes/__init__.py
--rw-r--r--   0        0        0      715 2023-03-07 03:10:58.611476 llama_hub-0.0.1a1/llama_hub/dad_jokes/base.py
--rw-r--r--   0        0        0     1259 2023-03-07 03:10:58.611612 llama_hub-0.0.1a1/llama_hub/database/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.611691 llama_hub-0.0.1a1/llama_hub/database/__init__.py
--rw-r--r--   0        0        0     3328 2023-04-26 20:58:33.744759 llama_hub-0.0.1a1/llama_hub/database/base.py
--rw-r--r--   0        0        0     1096 2023-04-22 18:27:31.207961 llama_hub-0.0.1a1/llama_hub/deeplake/README.md
--rw-r--r--   0        0        0       18 2023-04-26 20:58:33.745052 llama_hub-0.0.1a1/llama_hub/deeplake/__init__.py
--rw-r--r--   0        0        0     3457 2023-04-19 22:26:43.956932 llama_hub-0.0.1a1/llama_hub/deeplake/base.py
--rw-r--r--   0        0        0        8 2023-04-19 22:26:43.957176 llama_hub-0.0.1a1/llama_hub/deeplake/requirements.txt
--rw-r--r--   0        0        0      851 2023-03-07 03:10:58.611889 llama_hub-0.0.1a1/llama_hub/discord/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.611952 llama_hub-0.0.1a1/llama_hub/discord/__init__.py
--rw-r--r--   0        0        0     4650 2023-03-07 03:10:58.612035 llama_hub-0.0.1a1/llama_hub/discord/base.py
--rw-r--r--   0        0        0       10 2023-03-07 03:10:58.612097 llama_hub-0.0.1a1/llama_hub/discord/requirements.txt
--rw-r--r--   0        0        0     4153 2023-05-21 16:19:51.399011 llama_hub-0.0.1a1/llama_hub/docugami/README.md
--rw-r--r--   0        0        0        4 2023-05-21 16:19:51.399068 llama_hub-0.0.1a1/llama_hub/docugami/__init__.py
--rw-r--r--   0        0        0    12075 2023-05-21 16:19:51.399147 llama_hub-0.0.1a1/llama_hub/docugami/base.py
--rw-r--r--   0        0        0    65833 2023-05-21 16:19:51.399368 llama_hub-0.0.1a1/llama_hub/docugami/docugami.ipynb
--rw-r--r--   0        0        0       20 2023-05-21 16:19:51.399448 llama_hub-0.0.1a1/llama_hub/docugami/requirements.txt
--rw-r--r--   0        0        0     1042 2023-03-07 03:10:58.612196 llama_hub-0.0.1a1/llama_hub/elasticsearch/README.md
--rw-r--r--   0        0        0        0 2023-03-07 03:10:58.612226 llama_hub-0.0.1a1/llama_hub/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2301 2023-04-26 20:58:33.745187 llama_hub-0.0.1a1/llama_hub/elasticsearch/base.py
--rw-r--r--   0        0        0        5 2023-03-07 03:10:58.612374 llama_hub-0.0.1a1/llama_hub/elasticsearch/requirements.txt
--rw-r--r--   0        0        0     1319 2023-03-30 04:12:09.426503 llama_hub-0.0.1a1/llama_hub/faiss/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.612556 llama_hub-0.0.1a1/llama_hub/faiss/__init__.py
--rw-r--r--   0        0        0     2126 2023-03-07 03:10:58.612622 llama_hub-0.0.1a1/llama_hub/faiss/base.py
--rw-r--r--   0        0        0        5 2023-03-07 03:10:58.612674 llama_hub-0.0.1a1/llama_hub/faiss/requirements.txt
--rw-r--r--   0        0        0      585 2023-04-05 21:18:39.573568 llama_hub-0.0.1a1/llama_hub/feedly_rss/README.md
--rw-r--r--   0        0        0        0 2023-04-05 21:18:39.573603 llama_hub-0.0.1a1/llama_hub/feedly_rss/__init__.py
--rw-r--r--   0        0        0     2100 2023-04-26 20:58:33.745595 llama_hub-0.0.1a1/llama_hub/feedly_rss/base.py
--rw-r--r--   0        0        0       13 2023-04-05 21:18:39.573836 llama_hub-0.0.1a1/llama_hub/feedly_rss/requirements.txt
--rw-r--r--   0        0        0     2540 2023-05-21 16:19:51.399588 llama_hub-0.0.1a1/llama_hub/file/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.612849 llama_hub-0.0.1a1/llama_hub/file/__init__.py
--rw-r--r--   0        0        0      858 2023-03-07 03:10:58.612964 llama_hub-0.0.1a1/llama_hub/file/audio/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.613037 llama_hub-0.0.1a1/llama_hub/file/audio/__init__.py
--rw-r--r--   0        0        0     1486 2023-03-07 03:10:58.613118 llama_hub-0.0.1a1/llama_hub/file/audio/base.py
--rw-r--r--   0        0        0       20 2023-03-07 03:10:58.613175 llama_hub-0.0.1a1/llama_hub/file/audio/requirements.txt
--rw-r--r--   0        0        0     1241 2023-04-13 07:27:29.041256 llama_hub-0.0.1a1/llama_hub/file/audio_gladia/README.md
--rw-r--r--   0        0        0       19 2023-04-13 07:27:29.041321 llama_hub-0.0.1a1/llama_hub/file/audio_gladia/__init__.py
--rw-r--r--   0        0        0     3274 2023-04-13 07:27:29.041435 llama_hub-0.0.1a1/llama_hub/file/audio_gladia/base.py
--rw-r--r--   0        0        0       20 2023-04-13 07:27:29.041539 llama_hub-0.0.1a1/llama_hub/file/audio_gladia/requirements.txt
--rw-r--r--   0        0        0     5338 2023-05-21 16:19:51.400302 llama_hub-0.0.1a1/llama_hub/file/base.py
--rw-r--r--   0        0        0     1069 2023-03-07 03:10:58.613366 llama_hub-0.0.1a1/llama_hub/file/cjk_pdf/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.613428 llama_hub-0.0.1a1/llama_hub/file/cjk_pdf/__init__.py
--rw-r--r--   0        0        0     2584 2023-03-07 03:10:58.613499 llama_hub-0.0.1a1/llama_hub/file/cjk_pdf/base.py
--rw-r--r--   0        0        0       12 2023-03-07 03:10:58.613557 llama_hub-0.0.1a1/llama_hub/file/cjk_pdf/requirements.txt
--rw-r--r--   0        0        0      800 2023-05-21 16:19:51.401182 llama_hub-0.0.1a1/llama_hub/file/deepdoctection/README.md
--rw-r--r--   0        0        0        0 2023-05-01 23:46:36.351369 llama_hub-0.0.1a1/llama_hub/file/deepdoctection/__init__.py
--rw-r--r--   0        0        0     1188 2023-05-01 23:46:36.351571 llama_hub-0.0.1a1/llama_hub/file/deepdoctection/base.py
--rw-r--r--   0        0        0       24 2023-05-21 16:19:51.401417 llama_hub-0.0.1a1/llama_hub/file/deepdoctection/requirements.txt
--rw-r--r--   0        0        0      800 2023-03-07 03:10:58.613652 llama_hub-0.0.1a1/llama_hub/file/docx/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.613707 llama_hub-0.0.1a1/llama_hub/file/docx/__init__.py
--rw-r--r--   0        0        0      624 2023-05-21 16:19:51.402041 llama_hub-0.0.1a1/llama_hub/file/docx/base.py
--rw-r--r--   0        0        0        8 2023-03-07 03:10:58.613831 llama_hub-0.0.1a1/llama_hub/file/docx/requirements.txt
--rw-r--r--   0        0        0      724 2023-03-07 03:10:58.613918 llama_hub-0.0.1a1/llama_hub/file/epub/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.613969 llama_hub-0.0.1a1/llama_hub/file/epub/__init__.py
--rw-r--r--   0        0        0     1000 2023-03-07 03:10:58.614035 llama_hub-0.0.1a1/llama_hub/file/epub/base.py
--rw-r--r--   0        0        0       18 2023-03-07 03:10:58.614083 llama_hub-0.0.1a1/llama_hub/file/epub/requirements.txt
--rw-r--r--   0        0        0     1087 2023-04-13 07:27:29.042335 llama_hub-0.0.1a1/llama_hub/file/flat_pdf/README.md
--rw-r--r--   0        0        0       17 2023-04-02 07:55:11.892802 llama_hub-0.0.1a1/llama_hub/file/flat_pdf/__init__.py
--rw-r--r--   0        0        0     2837 2023-05-23 05:17:27.299408 llama_hub-0.0.1a1/llama_hub/file/flat_pdf/base.py
--rw-r--r--   0        0        0       15 2023-04-02 07:55:11.893284 llama_hub-0.0.1a1/llama_hub/file/flat_pdf/requirements.txt
--rw-r--r--   0        0        0     1359 2023-03-07 03:10:58.614185 llama_hub-0.0.1a1/llama_hub/file/image/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.614244 llama_hub-0.0.1a1/llama_hub/file/image/__init__.py
--rw-r--r--   0        0        0     3888 2023-05-21 16:19:51.402151 llama_hub-0.0.1a1/llama_hub/file/image/base.py
--rw-r--r--   0        0        0       63 2023-03-07 03:10:58.614370 llama_hub-0.0.1a1/llama_hub/file/image/requirements.txt
--rw-r--r--   0        0        0      373 2023-04-26 19:51:37.470265 llama_hub-0.0.1a1/llama_hub/file/image_blip/README.md
--rw-r--r--   0        0        0        0 2023-04-26 19:51:37.470295 llama_hub-0.0.1a1/llama_hub/file/image_blip/__init__.py
--rw-r--r--   0        0        0     3223 2023-04-26 20:58:33.746744 llama_hub-0.0.1a1/llama_hub/file/image_blip/base.py
--rw-r--r--   0        0        0       40 2023-04-26 19:51:37.470657 llama_hub-0.0.1a1/llama_hub/file/image_blip/requirements.txt
--rw-r--r--   0        0        0      422 2023-04-26 19:51:37.470792 llama_hub-0.0.1a1/llama_hub/file/image_blip2/README.md
--rw-r--r--   0        0        0        0 2023-04-26 19:51:37.470816 llama_hub-0.0.1a1/llama_hub/file/image_blip2/__init__.py
--rw-r--r--   0        0        0     3325 2023-04-26 20:58:33.747053 llama_hub-0.0.1a1/llama_hub/file/image_blip2/base.py
--rw-r--r--   0        0        0       40 2023-04-26 19:51:37.470995 llama_hub-0.0.1a1/llama_hub/file/image_blip2/requirements.txt
--rw-r--r--   0        0        0      457 2023-04-26 19:51:37.471184 llama_hub-0.0.1a1/llama_hub/file/ipynb/README.md
--rw-r--r--   0        0        0        0 2023-04-26 19:51:37.471215 llama_hub-0.0.1a1/llama_hub/file/ipynb/__init__.py
--rw-r--r--   0        0        0     1296 2023-04-26 20:58:33.747360 llama_hub-0.0.1a1/llama_hub/file/ipynb/base.py
--rw-r--r--   0        0        0        9 2023-04-26 19:51:37.471447 llama_hub-0.0.1a1/llama_hub/file/ipynb/requirements.txt
--rw-r--r--   0        0        0      735 2023-03-20 16:59:19.505917 llama_hub-0.0.1a1/llama_hub/file/json/README.md
--rw-r--r--   0        0        0       16 2023-04-26 20:58:33.747472 llama_hub-0.0.1a1/llama_hub/file/json/__init__.py
--rw-r--r--   0        0        0     2704 2023-04-26 20:58:33.747997 llama_hub-0.0.1a1/llama_hub/file/json/base.py
--rw-r--r--   0        0        0        0 2023-03-07 03:10:58.614625 llama_hub-0.0.1a1/llama_hub/file/json/requirements.txt
--rw-r--r--   0        0        0      744 2023-03-07 03:10:58.614720 llama_hub-0.0.1a1/llama_hub/file/markdown/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.614791 llama_hub-0.0.1a1/llama_hub/file/markdown/__init__.py
--rw-r--r--   0        0        0     3633 2023-05-30 02:38:57.380655 llama_hub-0.0.1a1/llama_hub/file/markdown/base.py
--rw-r--r--   0        0        0      680 2023-03-07 03:10:58.614958 llama_hub-0.0.1a1/llama_hub/file/mbox/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.615013 llama_hub-0.0.1a1/llama_hub/file/mbox/__init__.py
--rw-r--r--   0        0        0     3604 2023-05-30 03:31:37.274479 llama_hub-0.0.1a1/llama_hub/file/mbox/base.py
--rw-r--r--   0        0        0       14 2023-03-07 03:10:58.615139 llama_hub-0.0.1a1/llama_hub/file/mbox/requirements.txt
--rw-r--r--   0        0        0      929 2023-03-15 05:30:00.091626 llama_hub-0.0.1a1/llama_hub/file/paged_csv/README.md
--rw-r--r--   0        0        0        0 2023-03-15 05:30:00.091654 llama_hub-0.0.1a1/llama_hub/file/paged_csv/__init__.py
--rw-r--r--   0        0        0      929 2023-03-15 05:30:00.091771 llama_hub-0.0.1a1/llama_hub/file/paged_csv/base.py
--rw-r--r--   0        0        0      786 2023-03-07 03:10:58.615231 llama_hub-0.0.1a1/llama_hub/file/pandas_csv/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.615288 llama_hub-0.0.1a1/llama_hub/file/pandas_csv/__init__.py
--rw-r--r--   0        0        0     2271 2023-03-07 03:10:58.615340 llama_hub-0.0.1a1/llama_hub/file/pandas_csv/base.py
--rw-r--r--   0        0        0        6 2023-03-07 03:10:58.615393 llama_hub-0.0.1a1/llama_hub/file/pandas_csv/requirements.txt
--rw-r--r--   0        0        0     1334 2023-05-01 23:46:36.353261 llama_hub-0.0.1a1/llama_hub/file/pandas_excel/README.md
--rw-r--r--   0        0        0       17 2023-03-11 23:20:53.304142 llama_hub-0.0.1a1/llama_hub/file/pandas_excel/__init__.py
--rw-r--r--   0        0        0     2219 2023-05-21 16:19:51.402258 llama_hub-0.0.1a1/llama_hub/file/pandas_excel/base.py
--rw-r--r--   0        0        0        6 2023-03-11 23:20:53.304292 llama_hub-0.0.1a1/llama_hub/file/pandas_excel/requirements.txt
--rw-r--r--   0        0        0      790 2023-05-21 16:19:51.402351 llama_hub-0.0.1a1/llama_hub/file/pdf/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.615538 llama_hub-0.0.1a1/llama_hub/file/pdf/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-21 16:19:51.402428 llama_hub-0.0.1a1/llama_hub/file/pdf/base.py
--rw-r--r--   0        0        0        6 2023-05-21 16:19:51.402504 llama_hub-0.0.1a1/llama_hub/file/pdf/requirements.txt
--rw-r--r--   0        0        0     1120 2023-03-07 03:10:58.615758 llama_hub-0.0.1a1/llama_hub/file/pptx/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.615816 llama_hub-0.0.1a1/llama_hub/file/pptx/__init__.py
--rw-r--r--   0        0        0     3447 2023-04-26 20:58:00.478197 llama_hub-0.0.1a1/llama_hub/file/pptx/base.py
--rw-r--r--   0        0        0       49 2023-03-07 03:10:58.615980 llama_hub-0.0.1a1/llama_hub/file/pptx/requirements.txt
--rw-r--r--   0        0        0     1160 2023-05-30 03:31:39.799179 llama_hub-0.0.1a1/llama_hub/file/pymu_pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-21 16:19:51.402658 llama_hub-0.0.1a1/llama_hub/file/pymu_pdf/__init__.py
--rw-r--r--   0        0        0     2415 2023-05-21 16:19:51.402718 llama_hub-0.0.1a1/llama_hub/file/pymu_pdf/base.py
--rw-r--r--   0        0        0        7 2023-05-21 16:19:51.402763 llama_hub-0.0.1a1/llama_hub/file/pymu_pdf/requirements.txt
--rw-r--r--   0        0        0      890 2023-05-21 16:19:51.402877 llama_hub-0.0.1a1/llama_hub/file/rdf/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.616146 llama_hub-0.0.1a1/llama_hub/file/rdf/__init__.py
--rw-r--r--   0        0        0     2203 2023-03-07 03:10:58.616229 llama_hub-0.0.1a1/llama_hub/file/rdf/base.py
--rw-r--r--   0        0        0       13 2023-03-07 03:10:58.616294 llama_hub-0.0.1a1/llama_hub/file/rdf/requirements.txt
--rw-r--r--   0        0        0      792 2023-03-07 03:10:58.616400 llama_hub-0.0.1a1/llama_hub/file/simple_csv/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.616455 llama_hub-0.0.1a1/llama_hub/file/simple_csv/__init__.py
--rw-r--r--   0        0        0     1234 2023-04-26 20:58:33.748463 llama_hub-0.0.1a1/llama_hub/file/simple_csv/base.py
--rw-r--r--   0        0        0     2531 2023-03-07 03:10:58.616610 llama_hub-0.0.1a1/llama_hub/file/unstructured/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.616665 llama_hub-0.0.1a1/llama_hub/file/unstructured/__init__.py
--rw-r--r--   0        0        0     1305 2023-03-07 03:10:58.616725 llama_hub-0.0.1a1/llama_hub/file/unstructured/base.py
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.616783 llama_hub-0.0.1a1/llama_hub/file/unstructured/requirements.txt
--rw-r--r--   0        0        0     3122 2023-05-21 16:19:51.403139 llama_hub-0.0.1a1/llama_hub/github_repo/README.md
--rw-r--r--   0        0        0      153 2023-03-07 03:10:58.616933 llama_hub-0.0.1a1/llama_hub/github_repo/__init__.py
--rw-r--r--   0        0        0    20968 2023-05-30 03:31:41.488977 llama_hub-0.0.1a1/llama_hub/github_repo/base.py
--rw-r--r--   0        0        0    12721 2023-04-26 20:58:33.749411 llama_hub-0.0.1a1/llama_hub/github_repo/github_client.py
--rw-r--r--   0        0        0        5 2023-03-07 03:10:58.617213 llama_hub-0.0.1a1/llama_hub/github_repo/requirements.txt
--rw-r--r--   0        0        0     5736 2023-05-30 03:31:43.771344 llama_hub-0.0.1a1/llama_hub/github_repo/utils.py
--rw-r--r--   0        0        0      948 2023-03-12 07:33:19.338420 llama_hub-0.0.1a1/llama_hub/gmail/README.md
--rw-r--r--   0        0        0       17 2023-03-12 07:33:19.338506 llama_hub-0.0.1a1/llama_hub/gmail/__init__.py
--rw-r--r--   0        0        0     5302 2023-04-26 20:58:33.749867 llama_hub-0.0.1a1/llama_hub/gmail/base.py
--rw-r--r--   0        0        0       81 2023-03-12 07:33:19.338684 llama_hub-0.0.1a1/llama_hub/gmail/requirements.txt
--rw-r--r--   0        0        0     1364 2023-05-21 16:19:51.403395 llama_hub-0.0.1a1/llama_hub/google_calendar/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.617476 llama_hub-0.0.1a1/llama_hub/google_calendar/__init__.py
--rw-r--r--   0        0        0     4755 2023-03-07 03:10:58.617561 llama_hub-0.0.1a1/llama_hub/google_calendar/base.py
--rw-r--r--   0        0        0       66 2023-03-07 03:10:58.617624 llama_hub-0.0.1a1/llama_hub/google_calendar/requirements.txt
--rw-r--r--   0        0        0     2571 2023-05-21 16:19:51.403493 llama_hub-0.0.1a1/llama_hub/google_docs/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.617781 llama_hub-0.0.1a1/llama_hub/google_docs/__init__.py
--rw-r--r--   0        0        0     5019 2023-03-11 23:20:53.304647 llama_hub-0.0.1a1/llama_hub/google_docs/base.py
--rw-r--r--   0        0        0       66 2023-03-07 03:10:58.617940 llama_hub-0.0.1a1/llama_hub/google_docs/requirements.txt
--rw-r--r--   0        0        0     1807 2023-05-21 16:19:51.403584 llama_hub-0.0.1a1/llama_hub/google_drive/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.618115 llama_hub-0.0.1a1/llama_hub/google_drive/__init__.py
--rw-r--r--   0        0        0    13206 2023-05-30 02:38:57.381532 llama_hub-0.0.1a1/llama_hub/google_drive/base.py
--rw-r--r--   0        0        0       76 2023-03-07 03:10:58.618278 llama_hub-0.0.1a1/llama_hub/google_drive/requirements.txt
--rw-r--r--   0        0        0     1150 2023-05-21 16:19:51.404267 llama_hub-0.0.1a1/llama_hub/google_sheets/README.md
--rw-r--r--   0        0        0       17 2023-04-02 07:55:11.894902 llama_hub-0.0.1a1/llama_hub/google_sheets/__init__.py
--rw-r--r--   0        0        0     4989 2023-04-02 07:55:11.896582 llama_hub-0.0.1a1/llama_hub/google_sheets/base.py
--rw-r--r--   0        0        0       66 2023-04-02 07:55:11.896637 llama_hub-0.0.1a1/llama_hub/google_sheets/requirements.txt
--rw-r--r--   0        0        0      809 2023-03-20 16:59:19.506347 llama_hub-0.0.1a1/llama_hub/gpt_repo/README.md
--rw-r--r--   0        0        0       16 2023-04-26 20:58:33.749987 llama_hub-0.0.1a1/llama_hub/gpt_repo/__init__.py
--rw-r--r--   0        0        0     5488 2023-04-26 20:58:33.750276 llama_hub-0.0.1a1/llama_hub/gpt_repo/base.py
--rw-r--r--   0        0        0     1595 2023-05-30 02:38:57.381726 llama_hub-0.0.1a1/llama_hub/graphdb_cypher/README.md
--rw-r--r--   0        0        0       17 2023-05-30 02:38:57.381812 llama_hub-0.0.1a1/llama_hub/graphdb_cypher/__init__.py
--rw-r--r--   0        0        0     1788 2023-05-30 02:38:57.381954 llama_hub-0.0.1a1/llama_hub/graphdb_cypher/base.py
--rw-r--r--   0        0        0        6 2023-05-30 02:38:57.382081 llama_hub-0.0.1a1/llama_hub/graphdb_cypher/requirements.txt
--rw-r--r--   0        0        0     1215 2023-05-23 23:08:11.646060 llama_hub-0.0.1a1/llama_hub/graphql/README.md
--rw-r--r--   0        0        0       17 2023-05-23 23:08:11.646288 llama_hub-0.0.1a1/llama_hub/graphql/__init__.py
--rw-r--r--   0        0        0     2204 2023-05-23 23:08:11.646428 llama_hub-0.0.1a1/llama_hub/graphql/base.py
--rw-r--r--   0        0        0       21 2023-05-23 23:08:11.646585 llama_hub-0.0.1a1/llama_hub/graphql/requirements.txt
--rw-r--r--   0        0        0      969 2023-03-20 16:59:19.506791 llama_hub-0.0.1a1/llama_hub/hatena_blog/README.md
--rw-r--r--   0        0        0       17 2023-03-20 16:59:19.506876 llama_hub-0.0.1a1/llama_hub/hatena_blog/__init__.py
--rw-r--r--   0        0        0     2624 2023-04-26 20:58:33.750625 llama_hub-0.0.1a1/llama_hub/hatena_blog/base.py
--rw-r--r--   0        0        0       28 2023-03-20 16:59:19.507142 llama_hub-0.0.1a1/llama_hub/hatena_blog/requirements.txt
--rw-r--r--   0        0        0      916 2023-04-18 06:14:21.377601 llama_hub-0.0.1a1/llama_hub/hubspot/README.md
--rw-r--r--   0        0        0       17 2023-04-18 06:14:21.377664 llama_hub-0.0.1a1/llama_hub/hubspot/__init__.py
--rw-r--r--   0        0        0     1286 2023-04-26 20:58:33.750942 llama_hub-0.0.1a1/llama_hub/hubspot/base.py
--rw-r--r--   0        0        0       18 2023-04-18 06:14:21.377890 llama_hub-0.0.1a1/llama_hub/hubspot/requirements.txt
--rw-r--r--   0        0        0     1035 2023-04-27 01:18:41.028135 llama_hub-0.0.1a1/llama_hub/huggingface/fs/README.md
--rw-r--r--   0        0        0       18 2023-04-27 01:18:41.028344 llama_hub-0.0.1a1/llama_hub/huggingface/fs/__init__.py
--rw-r--r--   0        0        0     1827 2023-04-27 01:18:41.028519 llama_hub-0.0.1a1/llama_hub/huggingface/fs/base.py
--rw-r--r--   0        0        0       15 2023-04-27 01:18:41.028677 llama_hub-0.0.1a1/llama_hub/huggingface/fs/requirements.txt
--rw-r--r--   0        0        0      797 2023-03-07 03:10:58.618397 llama_hub-0.0.1a1/llama_hub/intercom/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.618466 llama_hub-0.0.1a1/llama_hub/intercom/__init__.py
--rw-r--r--   0        0        0     2416 2023-04-26 20:58:33.751420 llama_hub-0.0.1a1/llama_hub/intercom/base.py
--rw-r--r--   0        0        0       39 2023-03-07 03:10:58.618607 llama_hub-0.0.1a1/llama_hub/intercom/requirements.txt
--rw-r--r--   0        0        0      533 2023-03-30 04:12:09.426623 llama_hub-0.0.1a1/llama_hub/jira/README.md
--rw-r--r--   0        0        0        0 2023-03-30 04:12:09.426649 llama_hub-0.0.1a1/llama_hub/jira/__init__.py
--rw-r--r--   0        0        0     3383 2023-05-21 16:19:51.404374 llama_hub-0.0.1a1/llama_hub/jira/base.py
--rw-r--r--   0        0        0        5 2023-03-30 04:12:09.426840 llama_hub-0.0.1a1/llama_hub/jira/requirements.txt
--rw-r--r--   0        0        0     1362 2023-05-30 02:38:57.382270 llama_hub-0.0.1a1/llama_hub/joplin/README.md
--rw-r--r--   0        0        0        0 2023-05-30 02:38:57.382314 llama_hub-0.0.1a1/llama_hub/joplin/__init__.py
--rw-r--r--   0        0        0     5031 2023-05-30 02:38:57.382491 llama_hub-0.0.1a1/llama_hub/joplin/base.py
--rw-r--r--   0        0        0      698 2023-05-21 16:19:51.404482 llama_hub-0.0.1a1/llama_hub/jsondata/README.md
--rw-r--r--   0        0        0       16 2023-04-26 20:58:33.751933 llama_hub-0.0.1a1/llama_hub/jsondata/__init__.py
--rw-r--r--   0        0        0     1633 2023-04-26 20:58:33.752227 llama_hub-0.0.1a1/llama_hub/jsondata/base.py
--rw-r--r--   0        0        0        0 2023-04-13 07:27:29.043392 llama_hub-0.0.1a1/llama_hub/jsondata/requirements.txt
--rw-r--r--   0        0        0     7206 2023-05-23 23:08:11.646798 llama_hub-0.0.1a1/llama_hub/kaltura/esearch/README.md
--rw-r--r--   0        0        0       17 2023-05-23 23:08:11.646868 llama_hub-0.0.1a1/llama_hub/kaltura/esearch/__init__.py
--rw-r--r--   0        0        0    11968 2023-05-23 23:08:11.647030 llama_hub-0.0.1a1/llama_hub/kaltura/esearch/base.py
--rw-r--r--   0        0        0       24 2023-05-23 23:08:11.647139 llama_hub-0.0.1a1/llama_hub/kaltura/esearch/requirements.txt
--rw-r--r--   0        0        0    11434 2023-05-30 02:38:57.382747 llama_hub-0.0.1a1/llama_hub/library.json
--rw-r--r--   0        0        0     1117 2023-05-21 16:19:51.404867 llama_hub-0.0.1a1/llama_hub/make_com/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.618850 llama_hub-0.0.1a1/llama_hub/make_com/__init__.py
--rw-r--r--   0        0        0     1721 2023-05-21 16:19:51.405457 llama_hub-0.0.1a1/llama_hub/make_com/base.py
--rw-r--r--   0        0        0      810 2023-05-21 16:19:51.405536 llama_hub-0.0.1a1/llama_hub/mangoapps_guides/README.md
--rw-r--r--   0        0        0       17 2023-05-21 16:19:51.405588 llama_hub-0.0.1a1/llama_hub/mangoapps_guides/__init__.py
--rw-r--r--   0        0        0     4752 2023-05-21 16:19:51.405655 llama_hub-0.0.1a1/llama_hub/mangoapps_guides/base.py
--rw-r--r--   0        0        0       39 2023-05-21 16:19:51.405698 llama_hub-0.0.1a1/llama_hub/mangoapps_guides/requirements.txt
--rw-r--r--   0        0        0     2740 2023-05-30 02:38:57.382947 llama_hub-0.0.1a1/llama_hub/maps/README.md
--rw-r--r--   0        0        0       16 2023-05-30 02:38:57.383024 llama_hub-0.0.1a1/llama_hub/maps/__init__.py
--rw-r--r--   0        0        0     4599 2023-05-30 02:38:57.383180 llama_hub-0.0.1a1/llama_hub/maps/base.py
--rw-r--r--   0        0        0       15 2023-05-30 02:38:57.383325 llama_hub-0.0.1a1/llama_hub/maps/requirements.txt
--rw-r--r--   0        0        0      870 2023-03-07 03:10:58.619019 llama_hub-0.0.1a1/llama_hub/memos/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.619069 llama_hub-0.0.1a1/llama_hub/memos/__init__.py
--rw-r--r--   0        0        0     1465 2023-03-07 03:10:58.619127 llama_hub-0.0.1a1/llama_hub/memos/base.py
--rw-r--r--   0        0        0      952 2023-05-21 16:19:51.405772 llama_hub-0.0.1a1/llama_hub/metal/README.md
--rw-r--r--   0        0        0       17 2023-05-21 16:19:51.405816 llama_hub-0.0.1a1/llama_hub/metal/__init__.py
--rw-r--r--   0        0        0     2326 2023-05-21 16:19:51.405867 llama_hub-0.0.1a1/llama_hub/metal/base.py
--rw-r--r--   0        0        0       10 2023-05-21 16:19:51.405913 llama_hub-0.0.1a1/llama_hub/metal/requirements.txt
--rw-r--r--   0        0        0     1174 2023-04-13 07:27:29.043776 llama_hub-0.0.1a1/llama_hub/milvus/README.md
--rw-r--r--   0        0        0       18 2023-04-26 20:58:33.752658 llama_hub-0.0.1a1/llama_hub/milvus/__init__.py
--rw-r--r--   0        0        0     4588 2023-04-13 07:27:29.044087 llama_hub-0.0.1a1/llama_hub/milvus/base.py
--rw-r--r--   0        0        0        8 2023-04-13 07:27:29.044193 llama_hub-0.0.1a1/llama_hub/milvus/requirements.txt
--rw-r--r--   0        0        0      853 2023-05-21 16:19:51.405988 llama_hub-0.0.1a1/llama_hub/mondaydotcom/README.md
--rw-r--r--   0        0        0       17 2023-05-21 16:19:51.406029 llama_hub-0.0.1a1/llama_hub/mondaydotcom/__init__.py
--rw-r--r--   0        0        0     2658 2023-05-21 16:19:51.406081 llama_hub-0.0.1a1/llama_hub/mondaydotcom/base.py
--rw-r--r--   0        0        0        8 2023-05-21 16:19:51.406120 llama_hub-0.0.1a1/llama_hub/mondaydotcom/requirements.txt
--rw-r--r--   0        0        0      973 2023-03-07 03:10:58.619218 llama_hub-0.0.1a1/llama_hub/mongo/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.619281 llama_hub-0.0.1a1/llama_hub/mongo/__init__.py
--rw-r--r--   0        0        0     2260 2023-04-26 19:51:37.473125 llama_hub-0.0.1a1/llama_hub/mongo/base.py
--rw-r--r--   0        0        0        7 2023-03-07 03:10:58.619402 llama_hub-0.0.1a1/llama_hub/mongo/requirements.txt
--rw-r--r--   0        0        0      916 2023-03-07 03:10:58.619494 llama_hub-0.0.1a1/llama_hub/notion/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.619554 llama_hub-0.0.1a1/llama_hub/notion/__init__.py
--rw-r--r--   0        0        0     6102 2023-04-26 20:58:33.752942 llama_hub-0.0.1a1/llama_hub/notion/base.py
--rw-r--r--   0        0        0      688 2023-03-07 03:10:58.619733 llama_hub-0.0.1a1/llama_hub/obsidian/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.619795 llama_hub-0.0.1a1/llama_hub/obsidian/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-21 16:19:51.406223 llama_hub-0.0.1a1/llama_hub/obsidian/base.py
--rw-r--r--   0        0        0     1050 2023-03-26 16:14:37.561367 llama_hub-0.0.1a1/llama_hub/opendal_reader/README.md
--rw-r--r--   0        0        0        0 2023-03-26 16:14:37.561396 llama_hub-0.0.1a1/llama_hub/opendal_reader/__init__.py
--rw-r--r--   0        0        0      980 2023-03-26 16:14:37.561549 llama_hub-0.0.1a1/llama_hub/opendal_reader/azblob/README.md
--rw-r--r--   0        0        0       17 2023-03-26 16:14:37.561614 llama_hub-0.0.1a1/llama_hub/opendal_reader/azblob/__init__.py
--rw-r--r--   0        0        0     2317 2023-05-21 16:19:51.407098 llama_hub-0.0.1a1/llama_hub/opendal_reader/azblob/base.py
--rw-r--r--   0        0        0       16 2023-03-26 16:14:37.561831 llama_hub-0.0.1a1/llama_hub/opendal_reader/azblob/requirements.txt
--rw-r--r--   0        0        0     2789 2023-05-21 16:19:51.407231 llama_hub-0.0.1a1/llama_hub/opendal_reader/base.py
--rw-r--r--   0        0        0      999 2023-03-26 16:14:37.562087 llama_hub-0.0.1a1/llama_hub/opendal_reader/gcs/README.md
--rw-r--r--   0        0        0       17 2023-03-26 16:14:37.562145 llama_hub-0.0.1a1/llama_hub/opendal_reader/gcs/__init__.py
--rw-r--r--   0        0        0     2136 2023-05-21 16:19:51.407356 llama_hub-0.0.1a1/llama_hub/opendal_reader/gcs/base.py
--rw-r--r--   0        0        0       16 2023-03-26 16:14:37.562339 llama_hub-0.0.1a1/llama_hub/opendal_reader/gcs/requirements.txt
--rw-r--r--   0        0        0       16 2023-03-26 16:14:37.562450 llama_hub-0.0.1a1/llama_hub/opendal_reader/requirements.txt
--rw-r--r--   0        0        0     1397 2023-03-26 16:14:37.562649 llama_hub-0.0.1a1/llama_hub/opendal_reader/s3/README.md
--rw-r--r--   0        0        0       17 2023-03-26 16:14:37.562727 llama_hub-0.0.1a1/llama_hub/opendal_reader/s3/__init__.py
--rw-r--r--   0        0        0     2447 2023-05-21 16:19:51.407463 llama_hub-0.0.1a1/llama_hub/opendal_reader/s3/base.py
--rw-r--r--   0        0        0       16 2023-03-26 16:14:37.562957 llama_hub-0.0.1a1/llama_hub/opendal_reader/s3/requirements.txt
--rw-r--r--   0        0        0     2147 2023-05-21 16:19:51.407561 llama_hub-0.0.1a1/llama_hub/outlook_localcalendar/README.md
--rw-r--r--   0        0        0       16 2023-04-18 06:14:21.378313 llama_hub-0.0.1a1/llama_hub/outlook_localcalendar/__init__,py
--rw-r--r--   0        0        0     3838 2023-04-26 20:58:33.753531 llama_hub-0.0.1a1/llama_hub/outlook_localcalendar/base.py
--rw-r--r--   0        0        0        8 2023-04-18 06:14:21.378521 llama_hub-0.0.1a1/llama_hub/outlook_localcalendar/requirements.txt
--rw-r--r--   0        0        0     1801 2023-05-03 17:06:31.638713 llama_hub-0.0.1a1/llama_hub/pandas_ai/README.md
--rw-r--r--   0        0        0       18 2023-05-03 17:06:31.638920 llama_hub-0.0.1a1/llama_hub/pandas_ai/__init__.py
--rw-r--r--   0        0        0     3753 2023-05-03 17:06:31.639050 llama_hub-0.0.1a1/llama_hub/pandas_ai/base.py
--rw-r--r--   0        0        0        8 2023-05-03 17:06:31.639155 llama_hub-0.0.1a1/llama_hub/pandas_ai/requirements.txt
--rw-r--r--   0        0        0     1484 2023-03-11 23:20:53.305569 llama_hub-0.0.1a1/llama_hub/papers/arxiv/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.620068 llama_hub-0.0.1a1/llama_hub/papers/arxiv/__init__.py
--rw-r--r--   0        0        0     6266 2023-04-26 20:58:33.753972 llama_hub-0.0.1a1/llama_hub/papers/arxiv/base.py
--rw-r--r--   0        0        0        5 2023-03-07 03:10:58.620210 llama_hub-0.0.1a1/llama_hub/papers/arxiv/requirements.txt
--rw-r--r--   0        0        0      931 2023-03-07 03:10:58.620306 llama_hub-0.0.1a1/llama_hub/papers/pubmed/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.620365 llama_hub-0.0.1a1/llama_hub/papers/pubmed/__init__.py
--rw-r--r--   0        0        0     6168 2023-04-26 20:58:33.754174 llama_hub-0.0.1a1/llama_hub/papers/pubmed/base.py
--rw-r--r--   0        0        0     1279 2023-03-07 03:10:58.620654 llama_hub-0.0.1a1/llama_hub/pinecone/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.620741 llama_hub-0.0.1a1/llama_hub/pinecone/__init__.py
--rw-r--r--   0        0        0     2587 2023-03-07 03:10:58.620836 llama_hub-0.0.1a1/llama_hub/pinecone/base.py
--rw-r--r--   0        0        0       15 2023-03-07 03:10:58.620904 llama_hub-0.0.1a1/llama_hub/pinecone/requirements.txt
--rw-r--r--   0        0        0     1157 2023-04-22 18:27:31.208258 llama_hub-0.0.1a1/llama_hub/qdrant/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.621099 llama_hub-0.0.1a1/llama_hub/qdrant/__init__.py
--rw-r--r--   0        0        0     6920 2023-05-21 16:19:51.408441 llama_hub-0.0.1a1/llama_hub/qdrant/base.py
--rw-r--r--   0        0        0       13 2023-03-07 03:10:58.621230 llama_hub-0.0.1a1/llama_hub/qdrant/requirements.txt
--rw-r--r--   0        0        0     1551 2023-05-21 16:19:51.408542 llama_hub-0.0.1a1/llama_hub/readwise/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.621416 llama_hub-0.0.1a1/llama_hub/readwise/__init__.py
--rw-r--r--   0        0        0     1800 2023-04-26 20:58:33.754290 llama_hub-0.0.1a1/llama_hub/readwise/base.py
--rw-r--r--   0        0        0     2707 2023-05-21 16:19:51.408645 llama_hub-0.0.1a1/llama_hub/reddit/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.621692 llama_hub-0.0.1a1/llama_hub/reddit/__init__.py
--rw-r--r--   0        0        0     1914 2023-03-07 03:10:58.621768 llama_hub-0.0.1a1/llama_hub/reddit/base.py
--rw-r--r--   0        0        0       81 2023-03-11 23:20:53.306186 llama_hub-0.0.1a1/llama_hub/reddit/requirements.txt
--rw-r--r--   0        0        0     1330 2023-03-07 03:10:58.622034 llama_hub-0.0.1a1/llama_hub/remote/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.622110 llama_hub-0.0.1a1/llama_hub/remote/__init__.py
--rw-r--r--   0        0        0     2971 2023-05-01 23:46:36.353842 llama_hub-0.0.1a1/llama_hub/remote/base.py
--rw-r--r--   0        0        0     1383 2023-03-07 03:10:58.622318 llama_hub-0.0.1a1/llama_hub/remote_depth/README.md
--rw-r--r--   0        0        0        0 2023-03-07 03:10:58.622365 llama_hub-0.0.1a1/llama_hub/remote_depth/__init__.py
--rw-r--r--   0        0        0     3673 2023-04-26 20:58:33.754493 llama_hub-0.0.1a1/llama_hub/remote_depth/base.py
--rw-r--r--   0        0        0       31 2023-03-11 23:20:53.306309 llama_hub-0.0.1a1/llama_hub/remote_depth/requirements.txt
--rw-r--r--   0        0        0     1669 2023-03-07 03:10:58.622654 llama_hub-0.0.1a1/llama_hub/s3/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.622727 llama_hub-0.0.1a1/llama_hub/s3/__init__.py
--rw-r--r--   0        0        0     3795 2023-05-21 16:19:51.408750 llama_hub-0.0.1a1/llama_hub/s3/base.py
--rw-r--r--   0        0        0        5 2023-03-07 03:10:58.622867 llama_hub-0.0.1a1/llama_hub/s3/requirements.txt
--rw-r--r--   0        0        0      821 2023-05-21 16:19:51.408972 llama_hub-0.0.1a1/llama_hub/slack/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.623085 llama_hub-0.0.1a1/llama_hub/slack/__init__.py
--rw-r--r--   0        0        0     7499 2023-05-21 16:19:51.409152 llama_hub-0.0.1a1/llama_hub/slack/base.py
--rw-r--r--   0        0        0        9 2023-03-07 03:10:58.623225 llama_hub-0.0.1a1/llama_hub/slack/requirements.txt
--rw-r--r--   0        0        0      690 2023-05-30 02:38:57.384288 llama_hub-0.0.1a1/llama_hub/snscrape_twitter/README.md
--rw-r--r--   0        0        0       17 2023-05-23 05:17:27.299934 llama_hub-0.0.1a1/llama_hub/snscrape_twitter/__init__.py
--rw-r--r--   0        0        0     1156 2023-05-23 05:17:27.300031 llama_hub-0.0.1a1/llama_hub/snscrape_twitter/base.py
--rw-r--r--   0        0        0       56 2023-05-23 05:17:27.300115 llama_hub-0.0.1a1/llama_hub/snscrape_twitter/requirements.txt
--rw-r--r--   0        0        0     1662 2023-05-21 16:19:51.409299 llama_hub-0.0.1a1/llama_hub/spotify/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.623400 llama_hub-0.0.1a1/llama_hub/spotify/__init__.py
--rw-r--r--   0        0        0     2287 2023-03-07 03:10:58.623470 llama_hub-0.0.1a1/llama_hub/spotify/base.py
--rw-r--r--   0        0        0        7 2023-03-07 03:10:58.623529 llama_hub-0.0.1a1/llama_hub/spotify/requirements.txt
--rw-r--r--   0        0        0      846 2023-04-18 06:14:21.378852 llama_hub-0.0.1a1/llama_hub/stackoverflow/README.md
--rw-r--r--   0        0        0       17 2023-04-18 06:14:21.378915 llama_hub-0.0.1a1/llama_hub/stackoverflow/__init__.py
--rw-r--r--   0        0        0     6263 2023-04-26 20:58:33.755378 llama_hub-0.0.1a1/llama_hub/stackoverflow/base.py
--rw-r--r--   0        0        0       21 2023-04-18 06:14:21.379173 llama_hub-0.0.1a1/llama_hub/stackoverflow/requirements.txt
--rw-r--r--   0        0        0      936 2023-03-11 23:20:53.306574 llama_hub-0.0.1a1/llama_hub/steamship/README.md
--rw-r--r--   0        0        0        0 2023-03-11 23:20:53.306607 llama_hub-0.0.1a1/llama_hub/steamship/__init__.py
--rw-r--r--   0        0        0     3498 2023-03-11 23:20:53.306865 llama_hub-0.0.1a1/llama_hub/steamship/base.py
--rw-r--r--   0        0        0        9 2023-03-11 23:20:53.306992 llama_hub-0.0.1a1/llama_hub/steamship/requirements.txt
--rw-r--r--   0        0        0      726 2023-03-07 03:10:58.623642 llama_hub-0.0.1a1/llama_hub/string_iterable/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.623713 llama_hub-0.0.1a1/llama_hub/string_iterable/__init__.py
--rw-r--r--   0        0        0      969 2023-03-07 03:10:58.623784 llama_hub-0.0.1a1/llama_hub/string_iterable/base.py
--rw-r--r--   0        0        0      676 2023-04-22 18:27:31.208391 llama_hub-0.0.1a1/llama_hub/trello/README.md
--rw-r--r--   0        0        0       17 2023-04-22 18:27:31.208455 llama_hub-0.0.1a1/llama_hub/trello/__init__.py
--rw-r--r--   0        0        0     1429 2023-04-26 20:58:33.755634 llama_hub-0.0.1a1/llama_hub/trello/base.py
--rw-r--r--   0        0        0       10 2023-04-22 18:27:31.208639 llama_hub-0.0.1a1/llama_hub/trello/requirements.txt
--rw-r--r--   0        0        0      924 2023-03-07 03:10:58.623890 llama_hub-0.0.1a1/llama_hub/twitter/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.623957 llama_hub-0.0.1a1/llama_hub/twitter/__init__.py
--rw-r--r--   0        0        0     1777 2023-03-07 03:10:58.624029 llama_hub-0.0.1a1/llama_hub/twitter/base.py
--rw-r--r--   0        0        0        6 2023-03-07 03:10:58.624091 llama_hub-0.0.1a1/llama_hub/twitter/requirements.txt
--rw-r--r--   0        0        0     1162 2023-05-23 05:17:27.300236 llama_hub-0.0.1a1/llama_hub/weather/README.md
--rw-r--r--   0        0        0       16 2023-05-23 05:17:27.300287 llama_hub-0.0.1a1/llama_hub/weather/__init__.py
--rw-r--r--   0        0        0     2779 2023-05-23 05:17:27.300397 llama_hub-0.0.1a1/llama_hub/weather/base.py
--rw-r--r--   0        0        0        5 2023-05-23 05:17:27.300504 llama_hub-0.0.1a1/llama_hub/weather/requirements.txt
--rw-r--r--   0        0        0     1525 2023-03-07 03:10:58.624208 llama_hub-0.0.1a1/llama_hub/weaviate/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.624277 llama_hub-0.0.1a1/llama_hub/weaviate/__init__.py
--rw-r--r--   0        0        0     3697 2023-03-07 03:10:58.624357 llama_hub-0.0.1a1/llama_hub/weaviate/base.py
--rw-r--r--   0        0        0       15 2023-03-07 03:10:58.624421 llama_hub-0.0.1a1/llama_hub/weaviate/requirements.txt
--rw-r--r--   0        0        0      415 2023-05-01 23:46:36.353992 llama_hub-0.0.1a1/llama_hub/web/async_web/README.md
--rw-r--r--   0        0        0        0 2023-05-01 23:46:36.354035 llama_hub-0.0.1a1/llama_hub/web/async_web/__init__.py
--rw-r--r--   0        0        0     2554 2023-05-01 23:46:36.354173 llama_hub-0.0.1a1/llama_hub/web/async_web/base.py
--rw-r--r--   0        0        0       18 2023-05-01 23:46:36.354263 llama_hub-0.0.1a1/llama_hub/web/async_web/requirements.txt
--rw-r--r--   0        0        0     3446 2023-05-21 16:19:51.409418 llama_hub-0.0.1a1/llama_hub/web/beautiful_soup_web/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.624688 llama_hub-0.0.1a1/llama_hub/web/beautiful_soup_web/__init__.py
--rw-r--r--   0        0        0     6747 2023-04-26 20:58:33.755926 llama_hub-0.0.1a1/llama_hub/web/beautiful_soup_web/base.py
--rw-r--r--   0        0        0       31 2023-03-11 23:20:53.307220 llama_hub-0.0.1a1/llama_hub/web/beautiful_soup_web/requirements.txt
--rw-r--r--   0        0        0     3672 2023-05-21 16:19:51.409525 llama_hub-0.0.1a1/llama_hub/web/knowledge_base/README.md
--rw-r--r--   0        0        0        1 2023-03-07 03:10:58.625034 llama_hub-0.0.1a1/llama_hub/web/knowledge_base/__init__.py
--rw-r--r--   0        0        0     5611 2023-03-07 03:10:58.625114 llama_hub-0.0.1a1/llama_hub/web/knowledge_base/base.py
--rw-r--r--   0        0        0       16 2023-03-11 23:20:53.307403 llama_hub-0.0.1a1/llama_hub/web/knowledge_base/requirements.txt
--rw-r--r--   0        0        0     2681 2023-05-21 16:19:51.409776 llama_hub-0.0.1a1/llama_hub/web/readability_web/README.md
--rw-r--r--   0        0        0    83319 2023-04-05 21:18:39.575240 llama_hub-0.0.1a1/llama_hub/web/readability_web/Readability.js
--rw-r--r--   0        0        0       17 2023-03-11 23:20:53.307985 llama_hub-0.0.1a1/llama_hub/web/readability_web/__init__.py
--rw-r--r--   0        0        0     4531 2023-04-26 20:58:33.756303 llama_hub-0.0.1a1/llama_hub/web/readability_web/base.py
--rw-r--r--   0        0        0       18 2023-03-11 23:20:53.308113 llama_hub-0.0.1a1/llama_hub/web/readability_web/requirements.txt
--rw-r--r--   0        0        0      489 2023-05-21 16:19:51.409884 llama_hub-0.0.1a1/llama_hub/web/rss/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.625349 llama_hub-0.0.1a1/llama_hub/web/rss/__init__.py
--rw-r--r--   0        0        0     1986 2023-03-07 03:10:58.625428 llama_hub-0.0.1a1/llama_hub/web/rss/base.py
--rw-r--r--   0        0        0     1994 2023-05-21 16:19:51.409997 llama_hub-0.0.1a1/llama_hub/web/simple_web/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.625609 llama_hub-0.0.1a1/llama_hub/web/simple_web/__init__.py
--rw-r--r--   0        0        0     1257 2023-04-08 00:48:57.092410 llama_hub-0.0.1a1/llama_hub/web/simple_web/base.py
--rw-r--r--   0        0        0        9 2023-03-07 03:10:58.625747 llama_hub-0.0.1a1/llama_hub/web/simple_web/requirements.txt
--rw-r--r--   0        0        0     2009 2023-05-21 16:19:51.410103 llama_hub-0.0.1a1/llama_hub/web/trafilatura_web/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.625922 llama_hub-0.0.1a1/llama_hub/web/trafilatura_web/__init__.py
--rw-r--r--   0        0        0      889 2023-03-07 03:10:58.625999 llama_hub-0.0.1a1/llama_hub/web/trafilatura_web/base.py
--rw-r--r--   0        0        0       16 2023-03-11 23:20:53.308437 llama_hub-0.0.1a1/llama_hub/web/trafilatura_web/requirements.txt
--rw-r--r--   0        0        0     1075 2023-04-02 07:55:11.900591 llama_hub-0.0.1a1/llama_hub/web/unstructured_web/README.md
--rw-r--r--   0        0        0        0 2023-04-02 07:55:11.900624 llama_hub-0.0.1a1/llama_hub/web/unstructured_web/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-21 16:19:51.410332 llama_hub-0.0.1a1/llama_hub/web/unstructured_web/base.py
--rw-r--r--   0        0        0       12 2023-04-02 07:55:11.901235 llama_hub-0.0.1a1/llama_hub/web/unstructured_web/requirements.txt
--rw-r--r--   0        0        0     1315 2023-03-07 03:10:58.626184 llama_hub-0.0.1a1/llama_hub/whatsapp/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.626251 llama_hub-0.0.1a1/llama_hub/whatsapp/__init__.py
--rw-r--r--   0        0        0     1509 2023-03-07 03:10:58.626319 llama_hub-0.0.1a1/llama_hub/whatsapp/base.py
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.626389 llama_hub-0.0.1a1/llama_hub/whatsapp/requirements.txt
--rw-r--r--   0        0        0      895 2023-03-07 03:10:58.626510 llama_hub-0.0.1a1/llama_hub/wikipedia/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.626575 llama_hub-0.0.1a1/llama_hub/wikipedia/__init__.py
--rw-r--r--   0        0        0      818 2023-04-26 20:58:33.756884 llama_hub-0.0.1a1/llama_hub/wikipedia/base.py
--rw-r--r--   0        0        0       14 2023-03-11 23:20:53.308548 llama_hub-0.0.1a1/llama_hub/wikipedia/requirements.txt
--rw-r--r--   0        0        0     1042 2023-03-07 03:10:58.626816 llama_hub-0.0.1a1/llama_hub/wordpress/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.626889 llama_hub-0.0.1a1/llama_hub/wordpress/__init__.py
--rw-r--r--   0        0        0     2546 2023-03-07 03:10:58.626966 llama_hub-0.0.1a1/llama_hub/wordpress/base.py
--rw-r--r--   0        0        0       39 2023-03-07 03:10:58.627031 llama_hub-0.0.1a1/llama_hub/wordpress/requirements.txt
--rw-r--r--   0        0        0      774 2023-03-07 03:10:58.627173 llama_hub-0.0.1a1/llama_hub/youtube_transcript/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.627238 llama_hub-0.0.1a1/llama_hub/youtube_transcript/__init__.py
--rw-r--r--   0        0        0     1687 2023-04-26 20:58:33.757091 llama_hub-0.0.1a1/llama_hub/youtube_transcript/base.py
--rw-r--r--   0        0        0       29 2023-03-11 23:20:53.308735 llama_hub-0.0.1a1/llama_hub/youtube_transcript/requirements.txt
--rw-r--r--   0        0        0      884 2023-03-20 16:59:19.509159 llama_hub-0.0.1a1/llama_hub/zendesk/README.md
--rw-r--r--   0        0        0       17 2023-03-07 03:10:58.627563 llama_hub-0.0.1a1/llama_hub/zendesk/__init__.py
--rw-r--r--   0        0        0     2323 2023-03-20 16:59:19.509383 llama_hub-0.0.1a1/llama_hub/zendesk/base.py
--rw-r--r--   0        0        0       24 2023-03-30 04:12:09.427995 llama_hub-0.0.1a1/llama_hub/zendesk/requirements.txt
--rw-r--r--   0        0        0     1304 2023-04-13 07:27:29.045196 llama_hub-0.0.1a1/llama_hub/zulip/README.md
--rw-r--r--   0        0        0       17 2023-04-13 07:27:29.045245 llama_hub-0.0.1a1/llama_hub/zulip/__init__.py
--rw-r--r--   0        0        0     2432 2023-04-26 20:58:33.757365 llama_hub-0.0.1a1/llama_hub/zulip/base.py
--rw-r--r--   0        0        0        6 2023-04-13 07:27:29.045436 llama_hub-0.0.1a1/llama_hub/zulip/requirements.txt
--rw-r--r--   0        0        0      847 2023-05-30 04:29:19.160461 llama_hub-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     6234 1970-01-01 00:00:00.000000 llama_hub-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-31 00:05:29.625052 llama_hub-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     6505 2023-05-31 00:05:29.641438 llama_hub-0.0.1a2/README.md
+-rw-r--r--   0        0        0      247 2023-05-31 00:05:29.694416 llama_hub-0.0.1a2/llama_hub/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.688747 llama_hub-0.0.1a2/llama_hub/__init__.py
+-rwxr-xr-x   0        0        0      119 2023-05-31 00:05:29.710544 llama_hub-0.0.1a2/llama_hub/add_loader.sh
+-rw-r--r--   0        0        0      826 2023-05-31 00:05:29.698567 llama_hub-0.0.1a2/llama_hub/airtable/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.698464 llama_hub-0.0.1a2/llama_hub/airtable/__init__.py
+-rw-r--r--   0        0        0      901 2023-05-31 00:05:29.698672 llama_hub-0.0.1a2/llama_hub/airtable/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:05:29.698357 llama_hub-0.0.1a2/llama_hub/airtable/requirements.txt
+-rw-r--r--   0        0        0     1839 2023-05-31 00:05:29.718070 llama_hub-0.0.1a2/llama_hub/apify/actor/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.717948 llama_hub-0.0.1a2/llama_hub/apify/actor/__init__.py
+-rw-r--r--   0        0        0     2474 2023-05-31 00:05:29.718248 llama_hub-0.0.1a2/llama_hub/apify/actor/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:05:29.717839 llama_hub-0.0.1a2/llama_hub/apify/actor/requirements.txt
+-rw-r--r--   0        0        0     1499 2023-05-31 00:05:29.717463 llama_hub-0.0.1a2/llama_hub/apify/dataset/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.717305 llama_hub-0.0.1a2/llama_hub/apify/dataset/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-31 00:05:29.717590 llama_hub-0.0.1a2/llama_hub/apify/dataset/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:05:29.717199 llama_hub-0.0.1a2/llama_hub/apify/dataset/requirements.txt
+-rw-r--r--   0        0        0      778 2023-05-31 00:05:29.715654 llama_hub-0.0.1a2/llama_hub/asana/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.715550 llama_hub-0.0.1a2/llama_hub/asana/__init__.py
+-rw-r--r--   0        0        0     1856 2023-05-31 00:05:29.715751 llama_hub-0.0.1a2/llama_hub/asana/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:05:29.715456 llama_hub-0.0.1a2/llama_hub/asana/requirements.txt
+-rw-r--r--   0        0        0     2200 2023-05-31 00:05:29.714038 llama_hub-0.0.1a2/llama_hub/azcognitive_search/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.713921 llama_hub-0.0.1a2/llama_hub/azcognitive_search/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-31 00:05:29.714142 llama_hub-0.0.1a2/llama_hub/azcognitive_search/base.py
+-rw-r--r--   0        0        0       37 2023-05-31 00:05:29.713800 llama_hub-0.0.1a2/llama_hub/azcognitive_search/requirements.txt
+-rw-r--r--   0        0        0     2542 2023-05-31 00:05:29.712822 llama_hub-0.0.1a2/llama_hub/azstorage_blob/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.712714 llama_hub-0.0.1a2/llama_hub/azstorage_blob/__init__.py
+-rw-r--r--   0        0        0     5419 2023-05-31 00:05:29.713031 llama_hub-0.0.1a2/llama_hub/azstorage_blob/base.py
+-rw-r--r--   0        0        0       34 2023-05-31 00:05:29.712602 llama_hub-0.0.1a2/llama_hub/azstorage_blob/requirements.txt
+-rw-r--r--   0        0        0     1077 2023-05-31 00:05:29.677784 llama_hub-0.0.1a2/llama_hub/bilibili/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.677658 llama_hub-0.0.1a2/llama_hub/bilibili/__init__.py
+-rw-r--r--   0        0        0     2374 2023-05-31 00:05:29.677898 llama_hub-0.0.1a2/llama_hub/bilibili/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:05:29.677538 llama_hub-0.0.1a2/llama_hub/bilibili/requirements.txt
+-rw-r--r--   0        0        0     3373 2023-05-31 00:05:29.700339 llama_hub-0.0.1a2/llama_hub/boarddocs/BoardDocsReader.ipynb
+-rw-r--r--   0        0        0     1402 2023-05-31 00:05:29.700132 llama_hub-0.0.1a2/llama_hub/boarddocs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.700034 llama_hub-0.0.1a2/llama_hub/boarddocs/__init__.py
+-rw-r--r--   0        0        0     4430 2023-05-31 00:05:29.700233 llama_hub-0.0.1a2/llama_hub/boarddocs/base.py
+-rw-r--r--   0        0        0    19752 2023-05-31 00:05:29.699833 llama_hub-0.0.1a2/llama_hub/boarddocs/crawl.ipynb
+-rw-r--r--   0        0        0       22 2023-05-31 00:05:29.699930 llama_hub-0.0.1a2/llama_hub/boarddocs/requirements.txt
+-rw-r--r--   0        0        0      921 2023-05-31 00:05:29.711533 llama_hub-0.0.1a2/llama_hub/chatgpt_plugin/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.711414 llama_hub-0.0.1a2/llama_hub/chatgpt_plugin/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-31 00:05:29.711645 llama_hub-0.0.1a2/llama_hub/chatgpt_plugin/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.711273 llama_hub-0.0.1a2/llama_hub/chatgpt_plugin/requirements.txt
+-rw-r--r--   0        0        0     1056 2023-05-31 00:05:29.647988 llama_hub-0.0.1a2/llama_hub/chroma/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.647858 llama_hub-0.0.1a2/llama_hub/chroma/__init__.py
+-rw-r--r--   0        0        0     1918 2023-05-31 00:05:29.648097 llama_hub-0.0.1a2/llama_hub/chroma/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:05:29.647794 llama_hub-0.0.1a2/llama_hub/chroma/requirements.txt
+-rw-r--r--   0        0        0     2288 2023-05-31 00:05:29.704130 llama_hub-0.0.1a2/llama_hub/confluence/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.702816 llama_hub-0.0.1a2/llama_hub/confluence/__init__.py
+-rw-r--r--   0        0        0    11384 2023-05-31 00:05:29.704249 llama_hub-0.0.1a2/llama_hub/confluence/base.py
+-rw-r--r--   0        0        0       80 2023-05-31 00:05:29.702684 llama_hub-0.0.1a2/llama_hub/confluence/requirements.txt
+-rw-r--r--   0        0        0     1052 2023-05-31 00:05:29.650743 llama_hub-0.0.1a2/llama_hub/couchdb/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.650618 llama_hub-0.0.1a2/llama_hub/couchdb/__init__.py
+-rw-r--r--   0        0        0     2564 2023-05-31 00:05:29.650874 llama_hub-0.0.1a2/llama_hub/couchdb/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:05:29.650479 llama_hub-0.0.1a2/llama_hub/couchdb/requirements.txt
+-rw-r--r--   0        0        0      582 2023-05-31 00:05:29.705957 llama_hub-0.0.1a2/llama_hub/dad_jokes/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.705844 llama_hub-0.0.1a2/llama_hub/dad_jokes/__init__.py
+-rw-r--r--   0        0        0      715 2023-05-31 00:05:29.706068 llama_hub-0.0.1a2/llama_hub/dad_jokes/base.py
+-rw-r--r--   0        0        0     1259 2023-05-31 00:05:29.644239 llama_hub-0.0.1a2/llama_hub/database/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.643966 llama_hub-0.0.1a2/llama_hub/database/__init__.py
+-rw-r--r--   0        0        0     3328 2023-05-31 00:05:29.644486 llama_hub-0.0.1a2/llama_hub/database/base.py
+-rw-r--r--   0        0        0     1096 2023-05-31 00:05:29.715137 llama_hub-0.0.1a2/llama_hub/deeplake/README.md
+-rw-r--r--   0        0        0       18 2023-05-31 00:05:29.715021 llama_hub-0.0.1a2/llama_hub/deeplake/__init__.py
+-rw-r--r--   0        0        0     3457 2023-05-31 00:05:29.715240 llama_hub-0.0.1a2/llama_hub/deeplake/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:05:29.714914 llama_hub-0.0.1a2/llama_hub/deeplake/requirements.txt
+-rw-r--r--   0        0        0      851 2023-05-31 00:05:29.649403 llama_hub-0.0.1a2/llama_hub/discord/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.649278 llama_hub-0.0.1a2/llama_hub/discord/__init__.py
+-rw-r--r--   0        0        0     4650 2023-05-31 00:05:29.649529 llama_hub-0.0.1a2/llama_hub/discord/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:05:29.649146 llama_hub-0.0.1a2/llama_hub/discord/requirements.txt
+-rw-r--r--   0        0        0     4153 2023-05-31 00:05:29.648759 llama_hub-0.0.1a2/llama_hub/docugami/README.md
+-rw-r--r--   0        0        0        4 2023-05-31 00:05:29.648621 llama_hub-0.0.1a2/llama_hub/docugami/__init__.py
+-rw-r--r--   0        0        0    12075 2023-05-31 00:05:29.648897 llama_hub-0.0.1a2/llama_hub/docugami/base.py
+-rw-r--r--   0        0        0    65833 2023-05-31 00:05:29.648487 llama_hub-0.0.1a2/llama_hub/docugami/docugami.ipynb
+-rw-r--r--   0        0        0       20 2023-05-31 00:05:29.648324 llama_hub-0.0.1a2/llama_hub/docugami/requirements.txt
+-rw-r--r--   0        0        0     1042 2023-05-31 00:05:29.718737 llama_hub-0.0.1a2/llama_hub/elasticsearch/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.718608 llama_hub-0.0.1a2/llama_hub/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2301 2023-05-31 00:05:29.718868 llama_hub-0.0.1a2/llama_hub/elasticsearch/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:05:29.718535 llama_hub-0.0.1a2/llama_hub/elasticsearch/requirements.txt
+-rw-r--r--   0        0        0     1319 2023-05-31 00:05:29.706511 llama_hub-0.0.1a2/llama_hub/faiss/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.706406 llama_hub-0.0.1a2/llama_hub/faiss/__init__.py
+-rw-r--r--   0        0        0     2126 2023-05-31 00:05:29.706623 llama_hub-0.0.1a2/llama_hub/faiss/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:05:29.706299 llama_hub-0.0.1a2/llama_hub/faiss/requirements.txt
+-rw-r--r--   0        0        0      585 2023-05-31 00:05:29.696224 llama_hub-0.0.1a2/llama_hub/feedly_rss/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.695993 llama_hub-0.0.1a2/llama_hub/feedly_rss/__init__.py
+-rw-r--r--   0        0        0     2100 2023-05-31 00:05:29.696374 llama_hub-0.0.1a2/llama_hub/feedly_rss/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:05:29.695934 llama_hub-0.0.1a2/llama_hub/feedly_rss/requirements.txt
+-rw-r--r--   0        0        0     2829 2023-05-31 00:05:29.667041 llama_hub-0.0.1a2/llama_hub/file/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.663735 llama_hub-0.0.1a2/llama_hub/file/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-31 00:05:29.667496 llama_hub-0.0.1a2/llama_hub/file/audio/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.667386 llama_hub-0.0.1a2/llama_hub/file/audio/__init__.py
+-rw-r--r--   0        0        0     1486 2023-05-31 00:05:29.667607 llama_hub-0.0.1a2/llama_hub/file/audio/base.py
+-rw-r--r--   0        0        0       20 2023-05-31 00:05:29.667268 llama_hub-0.0.1a2/llama_hub/file/audio/requirements.txt
+-rw-r--r--   0        0        0     1241 2023-05-31 00:05:29.659595 llama_hub-0.0.1a2/llama_hub/file/audio_gladia/README.md
+-rw-r--r--   0        0        0       19 2023-05-31 00:05:29.659462 llama_hub-0.0.1a2/llama_hub/file/audio_gladia/__init__.py
+-rw-r--r--   0        0        0     3274 2023-05-31 00:05:29.659727 llama_hub-0.0.1a2/llama_hub/file/audio_gladia/base.py
+-rw-r--r--   0        0        0       20 2023-05-31 00:05:29.659216 llama_hub-0.0.1a2/llama_hub/file/audio_gladia/requirements.txt
+-rw-r--r--   0        0        0     5552 2023-05-31 00:05:29.675373 llama_hub-0.0.1a2/llama_hub/file/base.py
+-rw-r--r--   0        0        0     1069 2023-05-31 00:05:29.670622 llama_hub-0.0.1a2/llama_hub/file/cjk_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.670466 llama_hub-0.0.1a2/llama_hub/file/cjk_pdf/__init__.py
+-rw-r--r--   0        0        0     2584 2023-05-31 00:05:29.670875 llama_hub-0.0.1a2/llama_hub/file/cjk_pdf/base.py
+-rw-r--r--   0        0        0       12 2023-05-31 00:05:29.670297 llama_hub-0.0.1a2/llama_hub/file/cjk_pdf/requirements.txt
+-rw-r--r--   0        0        0      800 2023-05-31 00:05:29.674382 llama_hub-0.0.1a2/llama_hub/file/deepdoctection/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.674239 llama_hub-0.0.1a2/llama_hub/file/deepdoctection/__init__.py
+-rw-r--r--   0        0        0     1188 2023-05-31 00:05:29.674511 llama_hub-0.0.1a2/llama_hub/file/deepdoctection/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:05:29.674169 llama_hub-0.0.1a2/llama_hub/file/deepdoctection/requirements.txt
+-rw-r--r--   0        0        0      800 2023-05-31 00:05:29.675918 llama_hub-0.0.1a2/llama_hub/file/docx/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.675784 llama_hub-0.0.1a2/llama_hub/file/docx/__init__.py
+-rw-r--r--   0        0        0      624 2023-05-31 00:05:29.676075 llama_hub-0.0.1a2/llama_hub/file/docx/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:05:29.675660 llama_hub-0.0.1a2/llama_hub/file/docx/requirements.txt
+-rw-r--r--   0        0        0      724 2023-05-31 00:05:29.676550 llama_hub-0.0.1a2/llama_hub/file/epub/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.676430 llama_hub-0.0.1a2/llama_hub/file/epub/__init__.py
+-rw-r--r--   0        0        0     1000 2023-05-31 00:05:29.676669 llama_hub-0.0.1a2/llama_hub/file/epub/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:05:29.676313 llama_hub-0.0.1a2/llama_hub/file/epub/requirements.txt
+-rw-r--r--   0        0        0     1087 2023-05-31 00:05:29.672484 llama_hub-0.0.1a2/llama_hub/file/flat_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.672331 llama_hub-0.0.1a2/llama_hub/file/flat_pdf/__init__.py
+-rw-r--r--   0        0        0     2837 2023-05-31 00:05:29.672649 llama_hub-0.0.1a2/llama_hub/file/flat_pdf/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:05:29.672175 llama_hub-0.0.1a2/llama_hub/file/flat_pdf/requirements.txt
+-rw-r--r--   0        0        0     1359 2023-05-31 00:05:29.665638 llama_hub-0.0.1a2/llama_hub/file/image/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.665516 llama_hub-0.0.1a2/llama_hub/file/image/__init__.py
+-rw-r--r--   0        0        0     3888 2023-05-31 00:05:29.665764 llama_hub-0.0.1a2/llama_hub/file/image/base.py
+-rw-r--r--   0        0        0       63 2023-05-31 00:05:29.665402 llama_hub-0.0.1a2/llama_hub/file/image/requirements.txt
+-rw-r--r--   0        0        0      373 2023-05-31 00:05:29.666225 llama_hub-0.0.1a2/llama_hub/file/image_blip/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.666092 llama_hub-0.0.1a2/llama_hub/file/image_blip/__init__.py
+-rw-r--r--   0        0        0     3223 2023-05-31 00:05:29.666346 llama_hub-0.0.1a2/llama_hub/file/image_blip/base.py
+-rw-r--r--   0        0        0       40 2023-05-31 00:05:29.666023 llama_hub-0.0.1a2/llama_hub/file/image_blip/requirements.txt
+-rw-r--r--   0        0        0      422 2023-05-31 00:05:29.673234 llama_hub-0.0.1a2/llama_hub/file/image_blip2/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.673064 llama_hub-0.0.1a2/llama_hub/file/image_blip2/__init__.py
+-rw-r--r--   0        0        0     3325 2023-05-31 00:05:29.673379 llama_hub-0.0.1a2/llama_hub/file/image_blip2/base.py
+-rw-r--r--   0        0        0       40 2023-05-31 00:05:29.672979 llama_hub-0.0.1a2/llama_hub/file/image_blip2/requirements.txt
+-rw-r--r--   0        0        0      457 2023-05-31 00:05:29.661565 llama_hub-0.0.1a2/llama_hub/file/ipynb/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.661424 llama_hub-0.0.1a2/llama_hub/file/ipynb/__init__.py
+-rw-r--r--   0        0        0     1296 2023-05-31 00:05:29.661695 llama_hub-0.0.1a2/llama_hub/file/ipynb/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:05:29.661358 llama_hub-0.0.1a2/llama_hub/file/ipynb/requirements.txt
+-rw-r--r--   0        0        0      735 2023-05-31 00:05:29.668058 llama_hub-0.0.1a2/llama_hub/file/json/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.667915 llama_hub-0.0.1a2/llama_hub/file/json/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-31 00:05:29.668240 llama_hub-0.0.1a2/llama_hub/file/json/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.667788 llama_hub-0.0.1a2/llama_hub/file/json/requirements.txt
+-rw-r--r--   0        0        0      744 2023-05-31 00:05:29.660312 llama_hub-0.0.1a2/llama_hub/file/markdown/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.660093 llama_hub-0.0.1a2/llama_hub/file/markdown/__init__.py
+-rw-r--r--   0        0        0     3633 2023-05-31 00:05:29.660493 llama_hub-0.0.1a2/llama_hub/file/markdown/base.py
+-rw-r--r--   0        0        0      680 2023-05-31 00:05:29.666810 llama_hub-0.0.1a2/llama_hub/file/mbox/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.666694 llama_hub-0.0.1a2/llama_hub/file/mbox/__init__.py
+-rw-r--r--   0        0        0     3604 2023-05-31 00:05:29.666927 llama_hub-0.0.1a2/llama_hub/file/mbox/base.py
+-rw-r--r--   0        0        0       14 2023-05-31 00:05:29.666569 llama_hub-0.0.1a2/llama_hub/file/mbox/requirements.txt
+-rw-r--r--   0        0        0      929 2023-05-31 00:05:29.673795 llama_hub-0.0.1a2/llama_hub/file/paged_csv/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.673636 llama_hub-0.0.1a2/llama_hub/file/paged_csv/__init__.py
+-rw-r--r--   0        0        0      929 2023-05-31 00:05:29.673921 llama_hub-0.0.1a2/llama_hub/file/paged_csv/base.py
+-rw-r--r--   0        0        0      786 2023-05-31 00:05:29.658744 llama_hub-0.0.1a2/llama_hub/file/pandas_csv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.658615 llama_hub-0.0.1a2/llama_hub/file/pandas_csv/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-31 00:05:29.658868 llama_hub-0.0.1a2/llama_hub/file/pandas_csv/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:05:29.658490 llama_hub-0.0.1a2/llama_hub/file/pandas_csv/requirements.txt
+-rw-r--r--   0        0        0     1334 2023-05-31 00:05:29.660998 llama_hub-0.0.1a2/llama_hub/file/pandas_excel/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.660873 llama_hub-0.0.1a2/llama_hub/file/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     2219 2023-05-31 00:05:29.661116 llama_hub-0.0.1a2/llama_hub/file/pandas_excel/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:05:29.660743 llama_hub-0.0.1a2/llama_hub/file/pandas_excel/requirements.txt
+-rw-r--r--   0        0        0      790 2023-05-31 00:05:29.663496 llama_hub-0.0.1a2/llama_hub/file/pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.662058 llama_hub-0.0.1a2/llama_hub/file/pdf/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-31 00:05:29.663619 llama_hub-0.0.1a2/llama_hub/file/pdf/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:05:29.661935 llama_hub-0.0.1a2/llama_hub/file/pdf/requirements.txt
+-rw-r--r--   0        0        0     1120 2023-05-31 00:05:29.669006 llama_hub-0.0.1a2/llama_hub/file/pptx/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.668743 llama_hub-0.0.1a2/llama_hub/file/pptx/__init__.py
+-rw-r--r--   0        0        0     3447 2023-05-31 00:05:29.669216 llama_hub-0.0.1a2/llama_hub/file/pptx/base.py
+-rw-r--r--   0        0        0       49 2023-05-31 00:05:29.668567 llama_hub-0.0.1a2/llama_hub/file/pptx/requirements.txt
+-rw-r--r--   0        0        0     1160 2023-05-31 00:05:29.658080 llama_hub-0.0.1a2/llama_hub/file/pymu_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.657959 llama_hub-0.0.1a2/llama_hub/file/pymu_pdf/__init__.py
+-rw-r--r--   0        0        0     2415 2023-05-31 00:05:29.658212 llama_hub-0.0.1a2/llama_hub/file/pymu_pdf/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:05:29.657832 llama_hub-0.0.1a2/llama_hub/file/pymu_pdf/requirements.txt
+-rw-r--r--   0        0        0      890 2023-05-31 00:05:29.675024 llama_hub-0.0.1a2/llama_hub/file/rdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.674903 llama_hub-0.0.1a2/llama_hub/file/rdf/__init__.py
+-rw-r--r--   0        0        0     2203 2023-05-31 00:05:29.675159 llama_hub-0.0.1a2/llama_hub/file/rdf/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:05:29.674747 llama_hub-0.0.1a2/llama_hub/file/rdf/requirements.txt
+-rw-r--r--   0        0        0      792 2023-05-31 00:05:29.669806 llama_hub-0.0.1a2/llama_hub/file/simple_csv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.669633 llama_hub-0.0.1a2/llama_hub/file/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1234 2023-05-31 00:05:29.669969 llama_hub-0.0.1a2/llama_hub/file/simple_csv/base.py
+-rw-r--r--   0        0        0     2531 2023-05-31 00:05:29.671602 llama_hub-0.0.1a2/llama_hub/file/unstructured/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.671449 llama_hub-0.0.1a2/llama_hub/file/unstructured/__init__.py
+-rw-r--r--   0        0        0     1305 2023-05-31 00:05:29.671770 llama_hub-0.0.1a2/llama_hub/file/unstructured/base.py
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.671261 llama_hub-0.0.1a2/llama_hub/file/unstructured/requirements.txt
+-rw-r--r--   0        0        0     3122 2023-05-31 00:05:29.712054 llama_hub-0.0.1a2/llama_hub/github_repo/README.md
+-rw-r--r--   0        0        0      153 2023-05-31 00:05:29.711949 llama_hub-0.0.1a2/llama_hub/github_repo/__init__.py
+-rw-r--r--   0        0        0    20968 2023-05-31 00:05:29.712396 llama_hub-0.0.1a2/llama_hub/github_repo/base.py
+-rw-r--r--   0        0        0    12721 2023-05-31 00:05:29.712279 llama_hub-0.0.1a2/llama_hub/github_repo/github_client.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:05:29.711852 llama_hub-0.0.1a2/llama_hub/github_repo/requirements.txt
+-rw-r--r--   0        0        0     5736 2023-05-31 00:05:29.712163 llama_hub-0.0.1a2/llama_hub/github_repo/utils.py
+-rw-r--r--   0        0        0      948 2023-05-31 00:05:29.719931 llama_hub-0.0.1a2/llama_hub/gmail/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.719834 llama_hub-0.0.1a2/llama_hub/gmail/__init__.py
+-rw-r--r--   0        0        0     5302 2023-05-31 00:05:29.720060 llama_hub-0.0.1a2/llama_hub/gmail/base.py
+-rw-r--r--   0        0        0       81 2023-05-31 00:05:29.719713 llama_hub-0.0.1a2/llama_hub/gmail/requirements.txt
+-rw-r--r--   0        0        0     1364 2023-05-31 00:05:29.645291 llama_hub-0.0.1a2/llama_hub/google_calendar/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.645131 llama_hub-0.0.1a2/llama_hub/google_calendar/__init__.py
+-rw-r--r--   0        0        0     4755 2023-05-31 00:05:29.645435 llama_hub-0.0.1a2/llama_hub/google_calendar/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:05:29.644841 llama_hub-0.0.1a2/llama_hub/google_calendar/requirements.txt
+-rw-r--r--   0        0        0     2571 2023-05-31 00:05:29.691234 llama_hub-0.0.1a2/llama_hub/google_docs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.691110 llama_hub-0.0.1a2/llama_hub/google_docs/__init__.py
+-rw-r--r--   0        0        0     5019 2023-05-31 00:05:29.691373 llama_hub-0.0.1a2/llama_hub/google_docs/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:05:29.690979 llama_hub-0.0.1a2/llama_hub/google_docs/requirements.txt
+-rw-r--r--   0        0        0     1807 2023-05-31 00:05:29.721718 llama_hub-0.0.1a2/llama_hub/google_drive/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.721593 llama_hub-0.0.1a2/llama_hub/google_drive/__init__.py
+-rw-r--r--   0        0        0    13412 2023-05-31 00:05:29.722000 llama_hub-0.0.1a2/llama_hub/google_drive/base.py
+-rw-r--r--   0        0        0       76 2023-05-31 00:05:29.721474 llama_hub-0.0.1a2/llama_hub/google_drive/requirements.txt
+-rw-r--r--   0        0        0     1150 2023-05-31 00:05:29.651924 llama_hub-0.0.1a2/llama_hub/google_sheets/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.651795 llama_hub-0.0.1a2/llama_hub/google_sheets/__init__.py
+-rw-r--r--   0        0        0     4989 2023-05-31 00:05:29.652046 llama_hub-0.0.1a2/llama_hub/google_sheets/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:05:29.651662 llama_hub-0.0.1a2/llama_hub/google_sheets/requirements.txt
+-rw-r--r--   0        0        0      809 2023-05-31 00:05:29.722867 llama_hub-0.0.1a2/llama_hub/gpt_repo/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.722758 llama_hub-0.0.1a2/llama_hub/gpt_repo/__init__.py
+-rw-r--r--   0        0        0     5488 2023-05-31 00:05:29.722969 llama_hub-0.0.1a2/llama_hub/gpt_repo/base.py
+-rw-r--r--   0        0        0     1595 2023-05-31 00:05:29.690039 llama_hub-0.0.1a2/llama_hub/graphdb_cypher/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.689868 llama_hub-0.0.1a2/llama_hub/graphdb_cypher/__init__.py
+-rw-r--r--   0        0        0     1788 2023-05-31 00:05:29.690163 llama_hub-0.0.1a2/llama_hub/graphdb_cypher/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:05:29.689678 llama_hub-0.0.1a2/llama_hub/graphdb_cypher/requirements.txt
+-rw-r--r--   0        0        0     1215 2023-05-31 00:05:29.701659 llama_hub-0.0.1a2/llama_hub/graphql/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.701434 llama_hub-0.0.1a2/llama_hub/graphql/__init__.py
+-rw-r--r--   0        0        0     2204 2023-05-31 00:05:29.701784 llama_hub-0.0.1a2/llama_hub/graphql/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:05:29.701227 llama_hub-0.0.1a2/llama_hub/graphql/requirements.txt
+-rw-r--r--   0        0        0      969 2023-05-31 00:05:29.647475 llama_hub-0.0.1a2/llama_hub/hatena_blog/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.647371 llama_hub-0.0.1a2/llama_hub/hatena_blog/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-31 00:05:29.647589 llama_hub-0.0.1a2/llama_hub/hatena_blog/base.py
+-rw-r--r--   0        0        0       28 2023-05-31 00:05:29.647240 llama_hub-0.0.1a2/llama_hub/hatena_blog/requirements.txt
+-rw-r--r--   0        0        0      916 2023-05-31 00:05:29.694849 llama_hub-0.0.1a2/llama_hub/hubspot/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.694740 llama_hub-0.0.1a2/llama_hub/hubspot/__init__.py
+-rw-r--r--   0        0        0     1286 2023-05-31 00:05:29.694949 llama_hub-0.0.1a2/llama_hub/hubspot/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:05:29.694635 llama_hub-0.0.1a2/llama_hub/hubspot/requirements.txt
+-rw-r--r--   0        0        0     1035 2023-05-31 00:05:29.709934 llama_hub-0.0.1a2/llama_hub/huggingface/fs/README.md
+-rw-r--r--   0        0        0       18 2023-05-31 00:05:29.708976 llama_hub-0.0.1a2/llama_hub/huggingface/fs/__init__.py
+-rw-r--r--   0        0        0     1827 2023-05-31 00:05:29.710033 llama_hub-0.0.1a2/llama_hub/huggingface/fs/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:05:29.708867 llama_hub-0.0.1a2/llama_hub/huggingface/fs/requirements.txt
+-rw-r--r--   0        0        0      797 2023-05-31 00:05:29.685441 llama_hub-0.0.1a2/llama_hub/intercom/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.685333 llama_hub-0.0.1a2/llama_hub/intercom/__init__.py
+-rw-r--r--   0        0        0     2416 2023-05-31 00:05:29.685550 llama_hub-0.0.1a2/llama_hub/intercom/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:05:29.685221 llama_hub-0.0.1a2/llama_hub/intercom/requirements.txt
+-rw-r--r--   0        0        0      533 2023-05-31 00:05:29.699049 llama_hub-0.0.1a2/llama_hub/jira/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.698928 llama_hub-0.0.1a2/llama_hub/jira/__init__.py
+-rw-r--r--   0        0        0     3383 2023-05-31 00:05:29.699155 llama_hub-0.0.1a2/llama_hub/jira/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:05:29.698873 llama_hub-0.0.1a2/llama_hub/jira/requirements.txt
+-rw-r--r--   0        0        0     1362 2023-05-31 00:05:29.678198 llama_hub-0.0.1a2/llama_hub/joplin/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.678064 llama_hub-0.0.1a2/llama_hub/joplin/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-31 00:05:29.678403 llama_hub-0.0.1a2/llama_hub/joplin/base.py
+-rw-r--r--   0        0        0      698 2023-05-31 00:05:29.704842 llama_hub-0.0.1a2/llama_hub/jsondata/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.704678 llama_hub-0.0.1a2/llama_hub/jsondata/__init__.py
+-rw-r--r--   0        0        0     1633 2023-05-31 00:05:29.704963 llama_hub-0.0.1a2/llama_hub/jsondata/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.704480 llama_hub-0.0.1a2/llama_hub/jsondata/requirements.txt
+-rw-r--r--   0        0        0     7206 2023-05-31 00:05:29.695492 llama_hub-0.0.1a2/llama_hub/kaltura/esearch/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.695381 llama_hub-0.0.1a2/llama_hub/kaltura/esearch/__init__.py
+-rw-r--r--   0        0        0    12019 2023-05-31 00:05:29.695601 llama_hub-0.0.1a2/llama_hub/kaltura/esearch/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:05:29.695271 llama_hub-0.0.1a2/llama_hub/kaltura/esearch/requirements.txt
+-rw-r--r--   0        0        0    11434 2023-05-31 00:05:29.699268 llama_hub-0.0.1a2/llama_hub/library.json
+-rw-r--r--   0        0        0     1117 2023-05-31 00:05:29.684129 llama_hub-0.0.1a2/llama_hub/make_com/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.683917 llama_hub-0.0.1a2/llama_hub/make_com/__init__.py
+-rw-r--r--   0        0        0     1721 2023-05-31 00:05:29.684423 llama_hub-0.0.1a2/llama_hub/make_com/base.py
+-rw-r--r--   0        0        0      810 2023-05-31 00:05:29.722428 llama_hub-0.0.1a2/llama_hub/mangoapps_guides/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.722329 llama_hub-0.0.1a2/llama_hub/mangoapps_guides/__init__.py
+-rw-r--r--   0        0        0     4752 2023-05-31 00:05:29.722540 llama_hub-0.0.1a2/llama_hub/mangoapps_guides/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:05:29.722226 llama_hub-0.0.1a2/llama_hub/mangoapps_guides/requirements.txt
+-rw-r--r--   0        0        0     2740 2023-05-31 00:05:29.642842 llama_hub-0.0.1a2/llama_hub/maps/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.642558 llama_hub-0.0.1a2/llama_hub/maps/__init__.py
+-rw-r--r--   0        0        0     4599 2023-05-31 00:05:29.642974 llama_hub-0.0.1a2/llama_hub/maps/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:05:29.642312 llama_hub-0.0.1a2/llama_hub/maps/requirements.txt
+-rw-r--r--   0        0        0      870 2023-05-31 00:05:29.651257 llama_hub-0.0.1a2/llama_hub/memos/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.651123 llama_hub-0.0.1a2/llama_hub/memos/__init__.py
+-rw-r--r--   0        0        0     1465 2023-05-31 00:05:29.651394 llama_hub-0.0.1a2/llama_hub/memos/base.py
+-rw-r--r--   0        0        0      952 2023-05-31 00:05:29.677161 llama_hub-0.0.1a2/llama_hub/metal/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.677047 llama_hub-0.0.1a2/llama_hub/metal/__init__.py
+-rw-r--r--   0        0        0     2326 2023-05-31 00:05:29.677283 llama_hub-0.0.1a2/llama_hub/metal/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:05:29.676920 llama_hub-0.0.1a2/llama_hub/metal/requirements.txt
+-rw-r--r--   0        0        0     1174 2023-05-31 00:05:29.719369 llama_hub-0.0.1a2/llama_hub/milvus/README.md
+-rw-r--r--   0        0        0       18 2023-05-31 00:05:29.719233 llama_hub-0.0.1a2/llama_hub/milvus/__init__.py
+-rw-r--r--   0        0        0     4588 2023-05-31 00:05:29.719474 llama_hub-0.0.1a2/llama_hub/milvus/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:05:29.719106 llama_hub-0.0.1a2/llama_hub/milvus/requirements.txt
+-rw-r--r--   0        0        0      853 2023-05-31 00:05:29.713482 llama_hub-0.0.1a2/llama_hub/mondaydotcom/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.713379 llama_hub-0.0.1a2/llama_hub/mondaydotcom/__init__.py
+-rw-r--r--   0        0        0     2658 2023-05-31 00:05:29.713585 llama_hub-0.0.1a2/llama_hub/mondaydotcom/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:05:29.713276 llama_hub-0.0.1a2/llama_hub/mondaydotcom/requirements.txt
+-rw-r--r--   0        0        0      973 2023-05-31 00:05:29.707580 llama_hub-0.0.1a2/llama_hub/mongo/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.707482 llama_hub-0.0.1a2/llama_hub/mongo/__init__.py
+-rw-r--r--   0        0        0     2260 2023-05-31 00:05:29.707689 llama_hub-0.0.1a2/llama_hub/mongo/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:05:29.707377 llama_hub-0.0.1a2/llama_hub/mongo/requirements.txt
+-rw-r--r--   0        0        0      916 2023-05-31 00:05:29.694140 llama_hub-0.0.1a2/llama_hub/notion/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.693326 llama_hub-0.0.1a2/llama_hub/notion/__init__.py
+-rw-r--r--   0        0        0     6102 2023-05-31 00:05:29.694249 llama_hub-0.0.1a2/llama_hub/notion/base.py
+-rw-r--r--   0        0        0      688 2023-05-31 00:05:29.710327 llama_hub-0.0.1a2/llama_hub/obsidian/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.710227 llama_hub-0.0.1a2/llama_hub/obsidian/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-31 00:05:29.710439 llama_hub-0.0.1a2/llama_hub/obsidian/base.py
+-rw-r--r--   0        0        0     1050 2023-05-31 00:05:29.687587 llama_hub-0.0.1a2/llama_hub/opendal_reader/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.687363 llama_hub-0.0.1a2/llama_hub/opendal_reader/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-31 00:05:29.687000 llama_hub-0.0.1a2/llama_hub/opendal_reader/azblob/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.686883 llama_hub-0.0.1a2/llama_hub/opendal_reader/azblob/__init__.py
+-rw-r--r--   0        0        0     2476 2023-05-31 00:05:29.687255 llama_hub-0.0.1a2/llama_hub/opendal_reader/azblob/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.686761 llama_hub-0.0.1a2/llama_hub/opendal_reader/azblob/requirements.txt
+-rw-r--r--   0        0        0     2979 2023-05-31 00:05:29.687867 llama_hub-0.0.1a2/llama_hub/opendal_reader/base.py
+-rw-r--r--   0        0        0      999 2023-05-31 00:05:29.688387 llama_hub-0.0.1a2/llama_hub/opendal_reader/gcs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.688252 llama_hub-0.0.1a2/llama_hub/opendal_reader/gcs/__init__.py
+-rw-r--r--   0        0        0     2294 2023-05-31 00:05:29.688511 llama_hub-0.0.1a2/llama_hub/opendal_reader/gcs/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.688128 llama_hub-0.0.1a2/llama_hub/opendal_reader/gcs/requirements.txt
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.686502 llama_hub-0.0.1a2/llama_hub/opendal_reader/requirements.txt
+-rw-r--r--   0        0        0     1397 2023-05-31 00:05:29.686159 llama_hub-0.0.1a2/llama_hub/opendal_reader/s3/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.686047 llama_hub-0.0.1a2/llama_hub/opendal_reader/s3/__init__.py
+-rw-r--r--   0        0        0     2605 2023-05-31 00:05:29.686353 llama_hub-0.0.1a2/llama_hub/opendal_reader/s3/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.685924 llama_hub-0.0.1a2/llama_hub/opendal_reader/s3/requirements.txt
+-rw-r--r--   0        0        0     2147 2023-05-31 00:05:29.690509 llama_hub-0.0.1a2/llama_hub/outlook_localcalendar/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.690615 llama_hub-0.0.1a2/llama_hub/outlook_localcalendar/__init__,py
+-rw-r--r--   0        0        0     3838 2023-05-31 00:05:29.690724 llama_hub-0.0.1a2/llama_hub/outlook_localcalendar/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:05:29.690394 llama_hub-0.0.1a2/llama_hub/outlook_localcalendar/requirements.txt
+-rw-r--r--   0        0        0     1801 2023-05-31 00:05:29.652568 llama_hub-0.0.1a2/llama_hub/pandas_ai/README.md
+-rw-r--r--   0        0        0       18 2023-05-31 00:05:29.652436 llama_hub-0.0.1a2/llama_hub/pandas_ai/__init__.py
+-rw-r--r--   0        0        0     3932 2023-05-31 00:05:29.652813 llama_hub-0.0.1a2/llama_hub/pandas_ai/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:05:29.652302 llama_hub-0.0.1a2/llama_hub/pandas_ai/requirements.txt
+-rw-r--r--   0        0        0     1484 2023-05-31 00:05:29.656566 llama_hub-0.0.1a2/llama_hub/papers/arxiv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.656435 llama_hub-0.0.1a2/llama_hub/papers/arxiv/__init__.py
+-rw-r--r--   0        0        0     6441 2023-05-31 00:05:29.656766 llama_hub-0.0.1a2/llama_hub/papers/arxiv/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:05:29.656292 llama_hub-0.0.1a2/llama_hub/papers/arxiv/requirements.txt
+-rw-r--r--   0        0        0      931 2023-05-31 00:05:29.657175 llama_hub-0.0.1a2/llama_hub/papers/pubmed/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.657045 llama_hub-0.0.1a2/llama_hub/papers/pubmed/__init__.py
+-rw-r--r--   0        0        0     6168 2023-05-31 00:05:29.657311 llama_hub-0.0.1a2/llama_hub/papers/pubmed/base.py
+-rw-r--r--   0        0        0     1279 2023-05-31 00:05:29.698043 llama_hub-0.0.1a2/llama_hub/pinecone/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.697776 llama_hub-0.0.1a2/llama_hub/pinecone/__init__.py
+-rw-r--r--   0        0        0     2587 2023-05-31 00:05:29.698144 llama_hub-0.0.1a2/llama_hub/pinecone/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:05:29.697543 llama_hub-0.0.1a2/llama_hub/pinecone/requirements.txt
+-rw-r--r--   0        0        0     1157 2023-05-31 00:05:29.705485 llama_hub-0.0.1a2/llama_hub/qdrant/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.705363 llama_hub-0.0.1a2/llama_hub/qdrant/__init__.py
+-rw-r--r--   0        0        0     6920 2023-05-31 00:05:29.705614 llama_hub-0.0.1a2/llama_hub/qdrant/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:05:29.705228 llama_hub-0.0.1a2/llama_hub/qdrant/requirements.txt
+-rw-r--r--   0        0        0     1551 2023-05-31 00:05:29.643381 llama_hub-0.0.1a2/llama_hub/readwise/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.643239 llama_hub-0.0.1a2/llama_hub/readwise/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-31 00:05:29.643522 llama_hub-0.0.1a2/llama_hub/readwise/base.py
+-rw-r--r--   0        0        0     2707 2023-05-31 00:05:29.702284 llama_hub-0.0.1a2/llama_hub/reddit/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.702185 llama_hub-0.0.1a2/llama_hub/reddit/__init__.py
+-rw-r--r--   0        0        0     1914 2023-05-31 00:05:29.702396 llama_hub-0.0.1a2/llama_hub/reddit/base.py
+-rw-r--r--   0        0        0       81 2023-05-31 00:05:29.702062 llama_hub-0.0.1a2/llama_hub/reddit/requirements.txt
+-rw-r--r--   0        0        0     1330 2023-05-31 00:05:29.723301 llama_hub-0.0.1a2/llama_hub/remote/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.723166 llama_hub-0.0.1a2/llama_hub/remote/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-31 00:05:29.723456 llama_hub-0.0.1a2/llama_hub/remote/base.py
+-rw-r--r--   0        0        0     1383 2023-05-31 00:05:29.653616 llama_hub-0.0.1a2/llama_hub/remote_depth/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.653369 llama_hub-0.0.1a2/llama_hub/remote_depth/__init__.py
+-rw-r--r--   0        0        0     3829 2023-05-31 00:05:29.653746 llama_hub-0.0.1a2/llama_hub/remote_depth/base.py
+-rw-r--r--   0        0        0       31 2023-05-31 00:05:29.653290 llama_hub-0.0.1a2/llama_hub/remote_depth/requirements.txt
+-rw-r--r--   0        0        0     1669 2023-05-31 00:05:29.646762 llama_hub-0.0.1a2/llama_hub/s3/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.646649 llama_hub-0.0.1a2/llama_hub/s3/__init__.py
+-rw-r--r--   0        0        0     3985 2023-05-31 00:05:29.646967 llama_hub-0.0.1a2/llama_hub/s3/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:05:29.646518 llama_hub-0.0.1a2/llama_hub/s3/requirements.txt
+-rw-r--r--   0        0        0      821 2023-05-31 00:05:29.707073 llama_hub-0.0.1a2/llama_hub/slack/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.706963 llama_hub-0.0.1a2/llama_hub/slack/__init__.py
+-rw-r--r--   0        0        0     7499 2023-05-31 00:05:29.707176 llama_hub-0.0.1a2/llama_hub/slack/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:05:29.706850 llama_hub-0.0.1a2/llama_hub/slack/requirements.txt
+-rw-r--r--   0        0        0      690 2023-05-31 00:05:29.692999 llama_hub-0.0.1a2/llama_hub/snscrape_twitter/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.692871 llama_hub-0.0.1a2/llama_hub/snscrape_twitter/__init__.py
+-rw-r--r--   0        0        0     1156 2023-05-31 00:05:29.693108 llama_hub-0.0.1a2/llama_hub/snscrape_twitter/base.py
+-rw-r--r--   0        0        0       56 2023-05-31 00:05:29.692762 llama_hub-0.0.1a2/llama_hub/snscrape_twitter/requirements.txt
+-rw-r--r--   0        0        0     1662 2023-05-31 00:05:29.684880 llama_hub-0.0.1a2/llama_hub/spotify/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.684771 llama_hub-0.0.1a2/llama_hub/spotify/__init__.py
+-rw-r--r--   0        0        0     2287 2023-05-31 00:05:29.684986 llama_hub-0.0.1a2/llama_hub/spotify/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:05:29.684657 llama_hub-0.0.1a2/llama_hub/spotify/requirements.txt
+-rw-r--r--   0        0        0      846 2023-05-31 00:05:29.697063 llama_hub-0.0.1a2/llama_hub/stackoverflow/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.696877 llama_hub-0.0.1a2/llama_hub/stackoverflow/__init__.py
+-rw-r--r--   0        0        0     6263 2023-05-31 00:05:29.697200 llama_hub-0.0.1a2/llama_hub/stackoverflow/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:05:29.696701 llama_hub-0.0.1a2/llama_hub/stackoverflow/requirements.txt
+-rw-r--r--   0        0        0      936 2023-05-31 00:05:29.716782 llama_hub-0.0.1a2/llama_hub/steamship/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.716078 llama_hub-0.0.1a2/llama_hub/steamship/__init__.py
+-rw-r--r--   0        0        0     3498 2023-05-31 00:05:29.716885 llama_hub-0.0.1a2/llama_hub/steamship/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:05:29.715999 llama_hub-0.0.1a2/llama_hub/steamship/requirements.txt
+-rw-r--r--   0        0        0      726 2023-05-31 00:05:29.655159 llama_hub-0.0.1a2/llama_hub/string_iterable/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.654062 llama_hub-0.0.1a2/llama_hub/string_iterable/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-31 00:05:29.655284 llama_hub-0.0.1a2/llama_hub/string_iterable/base.py
+-rw-r--r--   0        0        0      676 2023-05-31 00:05:29.710963 llama_hub-0.0.1a2/llama_hub/trello/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.710857 llama_hub-0.0.1a2/llama_hub/trello/__init__.py
+-rw-r--r--   0        0        0     1429 2023-05-31 00:05:29.711086 llama_hub-0.0.1a2/llama_hub/trello/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:05:29.710743 llama_hub-0.0.1a2/llama_hub/trello/requirements.txt
+-rw-r--r--   0        0        0      924 2023-05-31 00:05:29.646114 llama_hub-0.0.1a2/llama_hub/twitter/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.645903 llama_hub-0.0.1a2/llama_hub/twitter/__init__.py
+-rw-r--r--   0        0        0     1777 2023-05-31 00:05:29.646246 llama_hub-0.0.1a2/llama_hub/twitter/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:05:29.645730 llama_hub-0.0.1a2/llama_hub/twitter/requirements.txt
+-rw-r--r--   0        0        0      637 2023-05-31 00:05:29.699593 llama_hub-0.0.1a2/llama_hub/utils.py
+-rw-r--r--   0        0        0     1162 2023-05-31 00:05:29.708274 llama_hub-0.0.1a2/llama_hub/weather/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.708145 llama_hub-0.0.1a2/llama_hub/weather/__init__.py
+-rw-r--r--   0        0        0     2779 2023-05-31 00:05:29.708401 llama_hub-0.0.1a2/llama_hub/weather/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:05:29.707967 llama_hub-0.0.1a2/llama_hub/weather/requirements.txt
+-rw-r--r--   0        0        0     1525 2023-05-31 00:05:29.714598 llama_hub-0.0.1a2/llama_hub/weaviate/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.714489 llama_hub-0.0.1a2/llama_hub/weaviate/__init__.py
+-rw-r--r--   0        0        0     3697 2023-05-31 00:05:29.714704 llama_hub-0.0.1a2/llama_hub/weaviate/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:05:29.714378 llama_hub-0.0.1a2/llama_hub/weaviate/requirements.txt
+-rw-r--r--   0        0        0      415 2023-05-31 00:05:29.682085 llama_hub-0.0.1a2/llama_hub/web/async_web/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.681937 llama_hub-0.0.1a2/llama_hub/web/async_web/__init__.py
+-rw-r--r--   0        0        0     2554 2023-05-31 00:05:29.682198 llama_hub-0.0.1a2/llama_hub/web/async_web/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:05:29.681867 llama_hub-0.0.1a2/llama_hub/web/async_web/requirements.txt
+-rw-r--r--   0        0        0     3446 2023-05-31 00:05:29.681515 llama_hub-0.0.1a2/llama_hub/web/beautiful_soup_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.681392 llama_hub-0.0.1a2/llama_hub/web/beautiful_soup_web/__init__.py
+-rw-r--r--   0        0        0     6747 2023-05-31 00:05:29.681649 llama_hub-0.0.1a2/llama_hub/web/beautiful_soup_web/base.py
+-rw-r--r--   0        0        0       31 2023-05-31 00:05:29.681254 llama_hub-0.0.1a2/llama_hub/web/beautiful_soup_web/requirements.txt
+-rw-r--r--   0        0        0     3672 2023-05-31 00:05:29.683434 llama_hub-0.0.1a2/llama_hub/web/knowledge_base/README.md
+-rw-r--r--   0        0        0        1 2023-05-31 00:05:29.683314 llama_hub-0.0.1a2/llama_hub/web/knowledge_base/__init__.py
+-rw-r--r--   0        0        0     5611 2023-05-31 00:05:29.683554 llama_hub-0.0.1a2/llama_hub/web/knowledge_base/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.683189 llama_hub-0.0.1a2/llama_hub/web/knowledge_base/requirements.txt
+-rw-r--r--   0        0        0     2681 2023-05-31 00:05:29.682812 llama_hub-0.0.1a2/llama_hub/web/readability_web/README.md
+-rw-r--r--   0        0        0    83319 2023-05-31 00:05:29.682692 llama_hub-0.0.1a2/llama_hub/web/readability_web/Readability.js
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.682552 llama_hub-0.0.1a2/llama_hub/web/readability_web/__init__.py
+-rw-r--r--   0        0        0     4531 2023-05-31 00:05:29.682948 llama_hub-0.0.1a2/llama_hub/web/readability_web/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:05:29.682428 llama_hub-0.0.1a2/llama_hub/web/readability_web/requirements.txt
+-rw-r--r--   0        0        0      489 2023-05-31 00:05:29.680350 llama_hub-0.0.1a2/llama_hub/web/rss/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.680230 llama_hub-0.0.1a2/llama_hub/web/rss/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-31 00:05:29.680459 llama_hub-0.0.1a2/llama_hub/web/rss/base.py
+-rw-r--r--   0        0        0     1994 2023-05-31 00:05:29.679864 llama_hub-0.0.1a2/llama_hub/web/simple_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.679752 llama_hub-0.0.1a2/llama_hub/web/simple_web/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-31 00:05:29.679980 llama_hub-0.0.1a2/llama_hub/web/simple_web/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:05:29.679642 llama_hub-0.0.1a2/llama_hub/web/simple_web/requirements.txt
+-rw-r--r--   0        0        0     2009 2023-05-31 00:05:29.680906 llama_hub-0.0.1a2/llama_hub/web/trafilatura_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.680790 llama_hub-0.0.1a2/llama_hub/web/trafilatura_web/__init__.py
+-rw-r--r--   0        0        0      889 2023-05-31 00:05:29.681020 llama_hub-0.0.1a2/llama_hub/web/trafilatura_web/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:05:29.680682 llama_hub-0.0.1a2/llama_hub/web/trafilatura_web/requirements.txt
+-rw-r--r--   0        0        0     1075 2023-05-31 00:05:29.679263 llama_hub-0.0.1a2/llama_hub/web/unstructured_web/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:05:29.679031 llama_hub-0.0.1a2/llama_hub/web/unstructured_web/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-31 00:05:29.679423 llama_hub-0.0.1a2/llama_hub/web/unstructured_web/base.py
+-rw-r--r--   0        0        0       12 2023-05-31 00:05:29.678963 llama_hub-0.0.1a2/llama_hub/web/unstructured_web/requirements.txt
+-rw-r--r--   0        0        0     1315 2023-05-31 00:05:29.720521 llama_hub-0.0.1a2/llama_hub/whatsapp/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.720421 llama_hub-0.0.1a2/llama_hub/whatsapp/__init__.py
+-rw-r--r--   0        0        0     1509 2023-05-31 00:05:29.720630 llama_hub-0.0.1a2/llama_hub/whatsapp/base.py
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.720296 llama_hub-0.0.1a2/llama_hub/whatsapp/requirements.txt
+-rw-r--r--   0        0        0      895 2023-05-31 00:05:29.650085 llama_hub-0.0.1a2/llama_hub/wikipedia/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.649914 llama_hub-0.0.1a2/llama_hub/wikipedia/__init__.py
+-rw-r--r--   0        0        0      818 2023-05-31 00:05:29.650212 llama_hub-0.0.1a2/llama_hub/wikipedia/base.py
+-rw-r--r--   0        0        0       14 2023-05-31 00:05:29.649788 llama_hub-0.0.1a2/llama_hub/wikipedia/requirements.txt
+-rw-r--r--   0        0        0     1042 2023-05-31 00:05:29.655802 llama_hub-0.0.1a2/llama_hub/wordpress/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.655674 llama_hub-0.0.1a2/llama_hub/wordpress/__init__.py
+-rw-r--r--   0        0        0     2546 2023-05-31 00:05:29.655921 llama_hub-0.0.1a2/llama_hub/wordpress/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:05:29.655539 llama_hub-0.0.1a2/llama_hub/wordpress/requirements.txt
+-rw-r--r--   0        0        0      774 2023-05-31 00:05:29.721124 llama_hub-0.0.1a2/llama_hub/youtube_transcript/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.721000 llama_hub-0.0.1a2/llama_hub/youtube_transcript/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-31 00:05:29.721250 llama_hub-0.0.1a2/llama_hub/youtube_transcript/base.py
+-rw-r--r--   0        0        0       29 2023-05-31 00:05:29.720889 llama_hub-0.0.1a2/llama_hub/youtube_transcript/requirements.txt
+-rw-r--r--   0        0        0      884 2023-05-31 00:05:29.700766 llama_hub-0.0.1a2/llama_hub/zendesk/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.700665 llama_hub-0.0.1a2/llama_hub/zendesk/__init__.py
+-rw-r--r--   0        0        0     2323 2023-05-31 00:05:29.700884 llama_hub-0.0.1a2/llama_hub/zendesk/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:05:29.700545 llama_hub-0.0.1a2/llama_hub/zendesk/requirements.txt
+-rw-r--r--   0        0        0     1304 2023-05-31 00:05:29.689234 llama_hub-0.0.1a2/llama_hub/zulip/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:05:29.689105 llama_hub-0.0.1a2/llama_hub/zulip/__init__.py
+-rw-r--r--   0        0        0     2432 2023-05-31 00:05:29.689342 llama_hub-0.0.1a2/llama_hub/zulip/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:05:29.688981 llama_hub-0.0.1a2/llama_hub/zulip/requirements.txt
+-rw-r--r--   0        0        0      875 2023-05-31 00:05:31.853344 llama_hub-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     7269 1970-01-01 00:00:00.000000 llama_hub-0.0.1a2/PKG-INFO
```

### Comparing `llama_hub-0.0.1a1/LICENSE` & `llama_hub-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/README.md` & `llama_hub-0.0.1a2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,113 @@
 # LlamaHub 🦙
 
-This is a simple library of all the data loaders / readers that have been created by the community. The goal is to make it extremely easy to connect large language models to a large variety of knowledge sources. These are general-purpose utilities that are meant to be used in [LlamaIndex](https://github.com/jerryjliu/gpt_index/tree/main/gpt_index) (e.g. when building a index) and [LangChain](https://github.com/hwchase17/langchain) (e.g. when building different tools an agent can use). For example, there are loaders to parse Google Docs, SQL Databases, PDF files, PowerPoints, Notion, Slack, Obsidian, and many more. Note that because different loaders produce the same types of Documents, you can easily use them together in the same index.
+This is a simple library of all the data loaders / readers that have been created by the community. The goal is to make it extremely easy to connect large language models to a large variety of knowledge sources. These are general-purpose utilities that are meant to be used in [LlamaIndex](https://github.com/jerryjliu/llama_index) (e.g. when building a index) and [LangChain](https://github.com/hwchase17/langchain) (e.g. when building different tools an agent can use). For example, there are loaders to parse Google Docs, SQL Databases, PDF files, PowerPoints, Notion, Slack, Obsidian, and many more. Note that because different loaders produce the same types of Documents, you can easily use them together in the same index.
 
 Check out our website here: https://llamahub.ai/.
 
 ![Website screenshot](https://scrabble-dictionary.s3.us-west-2.amazonaws.com/Screen+Shot+2023-02-11+at+12.45.44+PM.png)
 
-## Usage
+## Usage (Use `llama-hub` as PyPI package)
+These general-purpose loaders are designed to be used as a way to load data into [LlamaIndex](https://github.com/jerryjliu/llama_index) and/or subsequently used in [LangChain](https://github.com/hwchase17/langchain). 
 
-These general-purpose loaders are designed to be used as a way to load data into [LlamaIndex](https://github.com/jerryjliu/gpt_index/tree/main/gpt_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. **You can use them with `download_loader` from LlamaIndex in a single line of code!** For example, see the code snippets below using the Google Docs Loader.
+### Installation
+```
+pip install llama-hub
+```
 
 ### LlamaIndex
 
 ```python
-from llama_index import GPTVectorStoreIndex, download_loader
-
-GoogleDocsReader = download_loader('GoogleDocsReader')
+from llama_index import GPTVectorStoreIndex
+from llama_hub.google_docs.base import GoogleDocsReader
 
 gdoc_ids = ['1wf-y2pd9C878Oh-FmLH7Q_BQkljdm6TQal-c1pUfrec']
 loader = GoogleDocsReader()
 documents = loader.load_data(document_ids=gdoc_ids)
 index = GPTVectorStoreIndex.from_documents(documents)
 index.query('Where did the author go to school?')
 ```
 
 ### LangChain
 
 Note: Make sure you change the description of the `Tool` to match your use-case.
 
 ```python
-from llama_index import GPTVectorStoreIndex, download_loader
+from llama_index import GPTVectorStoreIndex
+from llama_hub.google_docs.base import GoogleDocsReader
 from langchain.llms import OpenAI
 from langchain.chains.question_answering import load_qa_chain
 
 # load documents
-GoogleDocsReader = download_loader('GoogleDocsReader')
 gdoc_ids = ['1wf-y2pd9C878Oh-FmLH7Q_BQkljdm6TQal-c1pUfrec']
 loader = GoogleDocsReader()
 documents = loader.load_data(document_ids=gdoc_ids)
 langchain_documents = [d.to_langchain_format() for d in documents]
 
 # initialize sample QA chain
 llm = OpenAI(temperature=0)
 qa_chain = load_qa_chain(llm)
 question="<query here>"
 answer = qa_chain.run(input_documents=langchain_documents, question=question)
 
 ```
+## Usage (Use `download_loader` from LlamaIndex)
+
+You can also use the loaders with `download_loader` from LlamaIndex in a single line of code.
+
+For example, see the code snippets below using the Google Docs Loader.
+
+```python
+from llama_index import GPTVectorStoreIndex, download_loader
+
+GoogleDocsReader = download_loader('GoogleDocsReader')
+
+gdoc_ids = ['1wf-y2pd9C878Oh-FmLH7Q_BQkljdm6TQal-c1pUfrec']
+loader = GoogleDocsReader()
+documents = loader.load_data(document_ids=gdoc_ids)
+index = GPTVectorStoreIndex.from_documents(documents)
+index.query('Where did the author go to school?')
+
+```
+
 
 ## How to add a loader
 
 Adding a loader simply requires forking this repo and making a Pull Request. The Loader Hub website will update automatically. However, please keep in the mind the following guidelines when making your PR.
 
+### Step 0: Setup virtual environment, install Poetry and dependencies
+
+Create a new Python virtual environment. The command below creates an environment in `.venv`,
+and activates it:
+```bash
+python -m venv .venv
+source .venv/bin/activate
+```
+
+if you are in windows, use the following to activate your virtual environment:
+
+```bash
+.venv\scripts\activate
+```
+
+Install poetry:
+
+```bash
+pip install poetry
+```
+
+Install the required dependencies (this will also install `llama_index`):
+
+```bash
+poetry install
+```
+
+This will create an editable install of `llama-hub` in your venv.
+
+
 ### Step 1: Create a new directory
 
 In `llama_hub`, create a new directory for your new loader. It can be nested within another, but name it something unique because the name of the directory will become the identifier for your loader (e.g. `google_docs`). Inside your new directory, create a `__init__.py` file, which can be empty, a `base.py` file which will contain your loader implementation, and, if needed, a `requirements.txt` file to list the package dependencies of your loader. Those packages will automatically be installed when your loader is used, so no need to worry about that anymore!
 
 If you'd like, you can create the new directory and files by running the following script in the `llama_hub` directory. Just remember to put your dependencies into a `requirements.txt` file.
 
 ```
@@ -78,15 +130,15 @@
 ## Running tests
 
 ```shell
 python3.9 -m venv .venv
 source .venv/bin/activate 
 pip3 install -r test_requirements.txt
 
-python3 -m pytest tests 
+poetry run pytest tests 
 ```
 
 ## FAQ
 
 ### How do I test my loader before it's merged?
 
 There is an argument called `loader_hub_url` in [`download_loader`](https://github.com/jerryjliu/llama_index/blob/main/llama_index/readers/download.py) that defaults to the main branch of this repo. You can set it to your branch or fork to test your new loader.
```

### Comparing `llama_hub-0.0.1a1/llama_hub/airtable/README.md` & `llama_hub-0.0.1a2/llama_hub/airtable/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/airtable/base.py` & `llama_hub-0.0.1a2/llama_hub/airtable/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/apify/actor/README.md` & `llama_hub-0.0.1a2/llama_hub/apify/actor/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/apify/actor/base.py` & `llama_hub-0.0.1a2/llama_hub/apify/actor/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,20 @@
         actor_call = self.apify_client.actor(actor_id).call(
             run_input=run_input,
             build=build,
             memory_mbytes=memory_mbytes,
             timeout_secs=timeout_secs,
         )
 
-        ApifyDataset = download_loader("ApifyDataset")
+        try:
+            from llama_hub.utils import import_loader
+            ApifyDataset = import_loader("ApifyDataset")
+        except ImportError:
+            ApifyDataset = download_loader("ApifyDataset")
+
         reader = ApifyDataset(self.apify_api_token)
         documents = reader.load_data(
             dataset_id=actor_call.get("defaultDatasetId"),
             dataset_mapping_function=dataset_mapping_function,
         )
 
         return documents
```

### Comparing `llama_hub-0.0.1a1/llama_hub/apify/dataset/README.md` & `llama_hub-0.0.1a2/llama_hub/apify/dataset/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/apify/dataset/base.py` & `llama_hub-0.0.1a2/llama_hub/apify/dataset/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/asana/README.md` & `llama_hub-0.0.1a2/llama_hub/asana/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/asana/base.py` & `llama_hub-0.0.1a2/llama_hub/asana/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/azcognitive_search/README.md` & `llama_hub-0.0.1a2/llama_hub/azcognitive_search/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/azcognitive_search/base.py` & `llama_hub-0.0.1a2/llama_hub/azcognitive_search/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/azstorage_blob/README.md` & `llama_hub-0.0.1a2/llama_hub/azstorage_blob/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/azstorage_blob/base.py` & `llama_hub-0.0.1a2/llama_hub/azstorage_blob/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,13 +105,18 @@
                         f"{obj.name} downloaded in {end_time - start_time} seconds."
                     )
             
             total_download_end_time = time.time()
             total_elapsed_time = math.ceil(total_download_end_time - total_download_start_time)
             logger.info(f"Downloading completed in approximately {total_elapsed_time // 60}min {total_elapsed_time % 60}s.")
             logger.info(f"Document creation starting")
-            SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
+
+            try:
+                from llama_hub.utils import import_loader
+                SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
+            except ImportError:
+                SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
             loader = SimpleDirectoryReader(temp_dir, file_extractor=self.file_extractor)
 
             return loader.load_data()
```

### Comparing `llama_hub-0.0.1a1/llama_hub/bilibili/README.md` & `llama_hub-0.0.1a2/llama_hub/bilibili/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/bilibili/base.py` & `llama_hub-0.0.1a2/llama_hub/bilibili/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/boarddocs/BoardDocsReader.ipynb` & `llama_hub-0.0.1a2/llama_hub/boarddocs/BoardDocsReader.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/boarddocs/README.md` & `llama_hub-0.0.1a2/llama_hub/boarddocs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/boarddocs/base.py` & `llama_hub-0.0.1a2/llama_hub/boarddocs/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/boarddocs/crawl.ipynb` & `llama_hub-0.0.1a2/llama_hub/boarddocs/crawl.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/chatgpt_plugin/README.md` & `llama_hub-0.0.1a2/llama_hub/chatgpt_plugin/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/chatgpt_plugin/base.py` & `llama_hub-0.0.1a2/llama_hub/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/chroma/README.md` & `llama_hub-0.0.1a2/llama_hub/chroma/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/chroma/base.py` & `llama_hub-0.0.1a2/llama_hub/chroma/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/confluence/README.md` & `llama_hub-0.0.1a2/llama_hub/confluence/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/confluence/base.py` & `llama_hub-0.0.1a2/llama_hub/confluence/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/couchdb/README.md` & `llama_hub-0.0.1a2/llama_hub/couchdb/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/couchdb/base.py` & `llama_hub-0.0.1a2/llama_hub/couchdb/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/dad_jokes/README.md` & `llama_hub-0.0.1a2/llama_hub/dad_jokes/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/dad_jokes/base.py` & `llama_hub-0.0.1a2/llama_hub/dad_jokes/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/database/README.md` & `llama_hub-0.0.1a2/llama_hub/database/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/database/base.py` & `llama_hub-0.0.1a2/llama_hub/database/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/deeplake/README.md` & `llama_hub-0.0.1a2/llama_hub/deeplake/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/deeplake/base.py` & `llama_hub-0.0.1a2/llama_hub/deeplake/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/discord/README.md` & `llama_hub-0.0.1a2/llama_hub/discord/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/discord/base.py` & `llama_hub-0.0.1a2/llama_hub/discord/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/docugami/README.md` & `llama_hub-0.0.1a2/llama_hub/docugami/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/docugami/base.py` & `llama_hub-0.0.1a2/llama_hub/docugami/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/docugami/docugami.ipynb` & `llama_hub-0.0.1a2/llama_hub/docugami/docugami.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/elasticsearch/README.md` & `llama_hub-0.0.1a2/llama_hub/elasticsearch/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/elasticsearch/base.py` & `llama_hub-0.0.1a2/llama_hub/elasticsearch/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/faiss/README.md` & `llama_hub-0.0.1a2/llama_hub/faiss/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/faiss/base.py` & `llama_hub-0.0.1a2/llama_hub/faiss/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/feedly_rss/README.md` & `llama_hub-0.0.1a2/llama_hub/feedly_rss/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/feedly_rss/base.py` & `llama_hub-0.0.1a2/llama_hub/feedly_rss/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/README.md` & `llama_hub-0.0.1a2/llama_hub/file/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,50 +3,58 @@
 This loader takes in a local directory containing files and extracts `Document`s from each of the files. By default, the loader will utilize the specialized loaders in this library to parse common file extensions (e.g. .pdf, .png, .docx, etc). You can optionally pass in your own custom loaders. Note: if no loader is found for a file extension, and the file extension is not in the list to skip, the file will be read directly.
 
 ## Usage
 
 To use this loader, you simply need to instantiate the `SimpleDirectoryReader` class with a directory, along with other optional settings, such as whether to ignore hidden files. See the code for the complete list.
 
 ```python
-from llama_index import download_loader
+from llama_hub.file.base import SimpleDirectoryReader
 
-SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
+# other way of loading
+# from llama_index import download_loader
+# SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
 
 loader = SimpleDirectoryReader('./data', recursive=True, exclude_hidden=True)
 documents = loader.load_data()
 ```
 
 ## Examples
 
 This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/jerryjliu/gpt_index/tree/main/gpt_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent.
 
 ### LlamaIndex
 
 ```python
-from llama_index import GPTVectorStoreIndex, download_loader
+from llama_hub.file.base import SimpleDirectoryReader
+from llama_index import GPTVectorStoreIndex
 
-SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
+# other way of loading
+# from llama_index import download_loader
+# SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
 
 loader = SimpleDirectoryReader('./data', recursive=True, exclude_hidden=True)
 documents = loader.load_data()
 index = GPTVectorStoreIndex.from_documents(documents)
 index.query('What are these files about?')
 ```
 
 ### LangChain
 
 Note: Make sure you change the description of the `Tool` to match your use-case.
 
 ```python
-from llama_index import GPTVectorStoreIndex, download_loader
+from llama_hub.file.base import SimpleDirectoryReader
+from llama_index import GPTVectorStoreIndex
 from langchain.agents import initialize_agent, Tool
 from langchain.llms import OpenAI
 from langchain.chains.conversation.memory import ConversationBufferMemory
 
-SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
+# other way of loading
+# from llama_index import download_loader
+# SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
 
 loader = SimpleDirectoryReader('./data', recursive=True, exclude_hidden=True)
 documents = loader.load_data()
 index = GPTVectorStoreIndex.from_documents(documents)
 
 tools = [
     Tool(
```

### Comparing `llama_hub-0.0.1a1/llama_hub/file/audio/README.md` & `llama_hub-0.0.1a2/llama_hub/file/audio/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/audio/base.py` & `llama_hub-0.0.1a2/llama_hub/file/audio/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/audio_gladia/README.md` & `llama_hub-0.0.1a2/llama_hub/file/audio_gladia/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/audio_gladia/base.py` & `llama_hub-0.0.1a2/llama_hub/file/audio_gladia/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/base.py` & `llama_hub-0.0.1a2/llama_hub/file/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Simple reader that reads files of different formats from a directory."""
 
 import logging
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
-from llama_index import download_loader
+from llama_index.readers.download import download_loader
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 DEFAULT_FILE_EXTRACTOR: Dict[str, str] = {
     ".pdf": "PDFReader",
     ".docx": "DocxReader",
     ".pptx": "PptxReader",
@@ -129,15 +129,19 @@
             if self.file_metadata is not None:
                 metadata = self.file_metadata(str(input_file))
 
             if input_file.suffix in self.file_extractor:
                 reader = self.file_extractor[input_file.suffix]
 
                 if isinstance(reader, str):
-                    reader = download_loader(reader)()
+                    try:
+                        from llama_hub.utils import import_loader
+                        reader = import_loader(reader)()
+                    except ImportError as e:
+                        reader = download_loader(reader)()
 
                 extracted_documents = reader.load_data(
                     file=input_file, extra_info=metadata
                 )
                 documents.extend(extracted_documents)
             else:
                 data = ""
```

### Comparing `llama_hub-0.0.1a1/llama_hub/file/cjk_pdf/README.md` & `llama_hub-0.0.1a2/llama_hub/file/cjk_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/cjk_pdf/base.py` & `llama_hub-0.0.1a2/llama_hub/file/cjk_pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/deepdoctection/README.md` & `llama_hub-0.0.1a2/llama_hub/file/deepdoctection/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/deepdoctection/base.py` & `llama_hub-0.0.1a2/llama_hub/file/deepdoctection/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/docx/README.md` & `llama_hub-0.0.1a2/llama_hub/file/docx/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/docx/base.py` & `llama_hub-0.0.1a2/llama_hub/file/docx/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/epub/README.md` & `llama_hub-0.0.1a2/llama_hub/file/epub/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/epub/base.py` & `llama_hub-0.0.1a2/llama_hub/file/epub/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/flat_pdf/README.md` & `llama_hub-0.0.1a2/llama_hub/file/flat_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/flat_pdf/base.py` & `llama_hub-0.0.1a2/llama_hub/file/flat_pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/image/README.md` & `llama_hub-0.0.1a2/llama_hub/file/image/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/image/base.py` & `llama_hub-0.0.1a2/llama_hub/file/image/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/image_blip/base.py` & `llama_hub-0.0.1a2/llama_hub/file/image_blip/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/image_blip2/base.py` & `llama_hub-0.0.1a2/llama_hub/file/image_blip2/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/ipynb/base.py` & `llama_hub-0.0.1a2/llama_hub/file/ipynb/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/json/README.md` & `llama_hub-0.0.1a2/llama_hub/file/json/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/json/base.py` & `llama_hub-0.0.1a2/llama_hub/file/json/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/markdown/README.md` & `llama_hub-0.0.1a2/llama_hub/file/markdown/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/markdown/base.py` & `llama_hub-0.0.1a2/llama_hub/file/markdown/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/mbox/README.md` & `llama_hub-0.0.1a2/llama_hub/file/mbox/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/mbox/base.py` & `llama_hub-0.0.1a2/llama_hub/file/mbox/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/paged_csv/README.md` & `llama_hub-0.0.1a2/llama_hub/file/paged_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/paged_csv/base.py` & `llama_hub-0.0.1a2/llama_hub/file/paged_csv/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pandas_csv/README.md` & `llama_hub-0.0.1a2/llama_hub/file/pandas_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pandas_csv/base.py` & `llama_hub-0.0.1a2/llama_hub/file/pandas_csv/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pandas_excel/README.md` & `llama_hub-0.0.1a2/llama_hub/file/pandas_excel/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pandas_excel/base.py` & `llama_hub-0.0.1a2/llama_hub/file/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pdf/README.md` & `llama_hub-0.0.1a2/llama_hub/file/pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pdf/base.py` & `llama_hub-0.0.1a2/llama_hub/file/pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pptx/README.md` & `llama_hub-0.0.1a2/llama_hub/file/pptx/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pptx/base.py` & `llama_hub-0.0.1a2/llama_hub/file/pptx/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pymu_pdf/README.md` & `llama_hub-0.0.1a2/llama_hub/file/pymu_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/pymu_pdf/base.py` & `llama_hub-0.0.1a2/llama_hub/file/pymu_pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/rdf/README.md` & `llama_hub-0.0.1a2/llama_hub/file/rdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/rdf/base.py` & `llama_hub-0.0.1a2/llama_hub/file/rdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/simple_csv/README.md` & `llama_hub-0.0.1a2/llama_hub/file/simple_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/simple_csv/base.py` & `llama_hub-0.0.1a2/llama_hub/file/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/unstructured/README.md` & `llama_hub-0.0.1a2/llama_hub/file/unstructured/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/file/unstructured/base.py` & `llama_hub-0.0.1a2/llama_hub/file/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/github_repo/README.md` & `llama_hub-0.0.1a2/llama_hub/github_repo/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/github_repo/base.py` & `llama_hub-0.0.1a2/llama_hub/github_repo/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/github_repo/github_client.py` & `llama_hub-0.0.1a2/llama_hub/github_repo/github_client.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/github_repo/utils.py` & `llama_hub-0.0.1a2/llama_hub/github_repo/utils.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/gmail/README.md` & `llama_hub-0.0.1a2/llama_hub/gmail/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/gmail/base.py` & `llama_hub-0.0.1a2/llama_hub/gmail/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/google_calendar/README.md` & `llama_hub-0.0.1a2/llama_hub/google_calendar/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/google_calendar/base.py` & `llama_hub-0.0.1a2/llama_hub/google_calendar/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/google_docs/README.md` & `llama_hub-0.0.1a2/llama_hub/google_docs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/google_docs/base.py` & `llama_hub-0.0.1a2/llama_hub/google_docs/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/google_drive/README.md` & `llama_hub-0.0.1a2/llama_hub/google_drive/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/google_drive/base.py` & `llama_hub-0.0.1a2/llama_hub/google_drive/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,19 @@
                     metadata[final_filepath] = {
                         "file id": fileid_meta[0],
                         "author": fileid_meta[1],
                         "file name": fileid_meta[2],
                         "created at": fileid_meta[3],
                         "modified at": fileid_meta[4],
                     }
-                SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
+                try:
+                    from llama_hub.utils import import_loader
+                    SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
+                except ImportError:
+                    SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
                 loader = SimpleDirectoryReader(temp_dir, file_metadata=get_metadata)
                 documents = loader.load_data()
 
             return documents
         except Exception as e:
             logger.error(
                 "An error occurred while loading data from fileids meta: {}".format(e)
```

### Comparing `llama_hub-0.0.1a1/llama_hub/google_sheets/README.md` & `llama_hub-0.0.1a2/llama_hub/google_sheets/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/google_sheets/base.py` & `llama_hub-0.0.1a2/llama_hub/google_sheets/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/gpt_repo/README.md` & `llama_hub-0.0.1a2/llama_hub/gpt_repo/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/gpt_repo/base.py` & `llama_hub-0.0.1a2/llama_hub/gpt_repo/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/graphdb_cypher/README.md` & `llama_hub-0.0.1a2/llama_hub/graphdb_cypher/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/graphdb_cypher/base.py` & `llama_hub-0.0.1a2/llama_hub/graphdb_cypher/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/graphql/README.md` & `llama_hub-0.0.1a2/llama_hub/graphql/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/graphql/base.py` & `llama_hub-0.0.1a2/llama_hub/graphql/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/hatena_blog/README.md` & `llama_hub-0.0.1a2/llama_hub/hatena_blog/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/hatena_blog/base.py` & `llama_hub-0.0.1a2/llama_hub/hatena_blog/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/hubspot/README.md` & `llama_hub-0.0.1a2/llama_hub/hubspot/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/hubspot/base.py` & `llama_hub-0.0.1a2/llama_hub/hubspot/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/huggingface/fs/README.md` & `llama_hub-0.0.1a2/llama_hub/huggingface/fs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/huggingface/fs/base.py` & `llama_hub-0.0.1a2/llama_hub/huggingface/fs/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/intercom/README.md` & `llama_hub-0.0.1a2/llama_hub/intercom/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/intercom/base.py` & `llama_hub-0.0.1a2/llama_hub/intercom/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/jira/README.md` & `llama_hub-0.0.1a2/llama_hub/jira/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/jira/base.py` & `llama_hub-0.0.1a2/llama_hub/jira/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/joplin/README.md` & `llama_hub-0.0.1a2/llama_hub/joplin/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/joplin/base.py` & `llama_hub-0.0.1a2/llama_hub/joplin/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,19 @@
                 If not provided, the JOPLIN_ACCESS_TOKEN environment variable is used. Default is None.
             parse_markdown (bool): Whether to parse the markdown content of the notes using MarkdownReader. Default is True.
             port (int): The port on which Joplin's Web Clipper service is running. Default is 41184.
             host (str): The host on which Joplin's Web Clipper service is running. Default is "localhost".
         """
         self.parse_markdown = parse_markdown
         if parse_markdown:
-            mr = download_loader("MarkdownReader")
+            try:
+                from llama_hub.utils import import_loader
+                mr = import_loader("MarkdownReader")
+            except:
+                mr = download_loader("MarkdownReader")
             self.parser = mr()
 
         access_token = access_token or self._get_token_from_env()
         base_url = f"http://{host}:{port}"
         self._get_note_url = (
             f"{base_url}/notes?token={access_token}"
             f"&fields=id,parent_id,title,body,created_time,updated_time&page={{page}}"
```

### Comparing `llama_hub-0.0.1a1/llama_hub/jsondata/README.md` & `llama_hub-0.0.1a2/llama_hub/jsondata/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/jsondata/base.py` & `llama_hub-0.0.1a2/llama_hub/jsondata/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/kaltura/esearch/README.md` & `llama_hub-0.0.1a2/llama_hub/kaltura/esearch/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/kaltura/esearch/base.py` & `llama_hub-0.0.1a2/llama_hub/kaltura/esearch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,22 +111,22 @@
             for search_result in response.objects:
                 entry = search_result.object
                 items_data = search_result.itemsData
 
                 entry_info = {
                     'entry_id': str(entry.id),
                     'entry_name': str(entry.name),
-                    'entry_description': str(entry.description),
-                    'entry_media_type': int(entry.mediaType.value),
-                    'entry_media_date': int(entry.createdAt),
-                    'entry_ms_duration': int(entry.msDuration),
-                    'entry_last_played_at': int(entry.lastPlayedAt),
-                    'entry_application': str(entry.application),
-                    'entry_tags': str(entry.tags),
-                    'entry_reference_id': str(entry.referenceId)
+                    'entry_description': str(entry.description or ''),
+                    'entry_media_type': int(entry.mediaType.value or 0),
+                    'entry_media_date': int(entry.createdAt or 0),
+                    'entry_ms_duration': int(entry.msDuration or 0),
+                    'entry_last_played_at': int(entry.lastPlayedAt or 0),
+                    'entry_application': str(entry.application or ''),
+                    'entry_tags': str(entry.tags or ''),
+                    'entry_reference_id': str(entry.referenceId or '')
                 }
 
                 if with_captions:
                     caption_search_result = items_data[0].items[0]
                     if hasattr(caption_search_result, 'captionAssetId'):
                         # TODO: change this to fetch captions per language, or as for a specific language code
                         caption_asset_id = caption_search_result.captionAssetId
@@ -141,15 +141,15 @@
                 entry_doc = Document(text=json.dumps(entry_dict), extra_info=entry_info)
                 entries.append(entry_doc)
 
             return entries
 
         except Exception as e:
             if e.code == "INVALID_KS":
-                raise ValueError('Kaltura Auth failed, check your credentials')
+                raise ValueError(f'Kaltura Auth failed, check your credentials: {e}')
             logger.error(f'An error occurred while loading with search params: {e}')
             return []
 
 
     def _get_json_transcript(self, caption_asset_id):
         """Fetch json transcript/captions from a given caption_asset_id
         
@@ -235,8 +235,8 @@
             # Find only entries that has this freeText found in them -
             if free_text is not None:
                 unified_item = KalturaESearchUnifiedItem()
                 unified_item.searchTerm = free_text
                 unified_item.itemType = KalturaESearchItemType.PARTIAL
                 search_params.searchOperator.searchItems.append(unified_item)
         
-        return self._load_from_search_params(search_params, with_captions, max_entries)
+        return self._load_from_search_params(search_params, with_captions, max_entries)
```

### Comparing `llama_hub-0.0.1a1/llama_hub/library.json` & `llama_hub-0.0.1a2/llama_hub/library.json`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/make_com/README.md` & `llama_hub-0.0.1a2/llama_hub/make_com/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/make_com/base.py` & `llama_hub-0.0.1a2/llama_hub/make_com/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/mangoapps_guides/README.md` & `llama_hub-0.0.1a2/llama_hub/mangoapps_guides/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/mangoapps_guides/base.py` & `llama_hub-0.0.1a2/llama_hub/mangoapps_guides/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/maps/README.md` & `llama_hub-0.0.1a2/llama_hub/maps/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/maps/base.py` & `llama_hub-0.0.1a2/llama_hub/maps/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/memos/README.md` & `llama_hub-0.0.1a2/llama_hub/memos/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/memos/base.py` & `llama_hub-0.0.1a2/llama_hub/memos/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/metal/README.md` & `llama_hub-0.0.1a2/llama_hub/metal/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/metal/base.py` & `llama_hub-0.0.1a2/llama_hub/metal/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/milvus/README.md` & `llama_hub-0.0.1a2/llama_hub/milvus/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/milvus/base.py` & `llama_hub-0.0.1a2/llama_hub/milvus/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/mondaydotcom/README.md` & `llama_hub-0.0.1a2/llama_hub/mondaydotcom/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/mondaydotcom/base.py` & `llama_hub-0.0.1a2/llama_hub/mondaydotcom/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/mongo/README.md` & `llama_hub-0.0.1a2/llama_hub/mongo/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/mongo/base.py` & `llama_hub-0.0.1a2/llama_hub/mongo/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/notion/README.md` & `llama_hub-0.0.1a2/llama_hub/notion/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/notion/base.py` & `llama_hub-0.0.1a2/llama_hub/notion/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/obsidian/README.md` & `llama_hub-0.0.1a2/llama_hub/obsidian/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/obsidian/base.py` & `llama_hub-0.0.1a2/llama_hub/obsidian/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/opendal_reader/README.md` & `llama_hub-0.0.1a2/llama_hub/opendal_reader/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/opendal_reader/azblob/README.md` & `llama_hub-0.0.1a2/llama_hub/opendal_reader/azblob/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/opendal_reader/azblob/base.py` & `llama_hub-0.0.1a2/llama_hub/opendal_reader/azblob/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,20 @@
             "account_name": account_name,
             "account_key": account_key,
         }
 
     def load_data(self) -> List[Document]:
         """Load file(s) from OpenDAL."""
 
-        OpendalReader = download_loader("OpendalReader")
+        try:
+            from llama_hub.utils import import_loader
+            OpendalReader = import_loader("OpendalReader")
+        except ImportError:
+            OpendalReader = download_loader("OpendalReader")
+
         loader = OpendalReader(
             scheme="azblob",
             path=self.path,
             file_extractor=self.file_extractor,
             **self.options,
         )
```

### Comparing `llama_hub-0.0.1a1/llama_hub/opendal_reader/base.py` & `llama_hub-0.0.1a2/llama_hub/opendal_reader/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,19 @@
 
         with tempfile.TemporaryDirectory() as temp_dir:
             if not self.path.endswith("/"):
                 asyncio.run(download_file_from_opendal(self.op, temp_dir, self.path))
             else:
                 asyncio.run(download_dir_from_opendal(self.op, temp_dir, self.path))
 
-            SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
+            try:
+                from llama_hub.utils import import_loader
+                SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
+            except ImportError:
+                SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
             loader = SimpleDirectoryReader(temp_dir, file_extractor=self.file_extractor)
 
             return loader.load_data()
 
 
 async def download_file_from_opendal(
     op: Any, temp_dir: str, path: str
```

### Comparing `llama_hub-0.0.1a1/llama_hub/opendal_reader/gcs/README.md` & `llama_hub-0.0.1a2/llama_hub/opendal_reader/gcs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/opendal_reader/gcs/base.py` & `llama_hub-0.0.1a2/llama_hub/opendal_reader/gcs/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,19 @@
             "endpoint": endpoint,
             "credentials": credentials,
         }
 
     def load_data(self) -> List[Document]:
         """Load file(s) from OpenDAL."""
 
-        OpendalReader = download_loader("OpendalReader")
+        try:
+            from llama_hub.utils import import_loader
+            OpendalReader = import_loader("OpendalReader")
+        except ImportError:
+            OpendalReader = download_loader("OpendalReader")
         loader = OpendalReader(
             scheme="gcs",
             path=self.path,
             file_extractor=self.file_extractor,
             **self.options,
         )
```

### Comparing `llama_hub-0.0.1a1/llama_hub/opendal_reader/s3/README.md` & `llama_hub-0.0.1a2/llama_hub/opendal_reader/s3/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/opendal_reader/s3/base.py` & `llama_hub-0.0.1a2/llama_hub/opendal_reader/s3/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,19 @@
             "region": region,
             "bucket": bucket,
         }
 
     def load_data(self) -> List[Document]:
         """Load file(s) from OpenDAL."""
 
-        OpendalReader = download_loader("OpendalReader")
+        try:
+            from llama_hub.utils import import_loader
+            OpendalReader = import_loader("OpendalReader")
+        except ImportError:
+            OpendalReader = download_loader("OpendalReader")
         loader = OpendalReader(
             scheme="s3",
             path=self.path,
             file_extractor=self.file_extractor,
             **self.options,
         )
```

### Comparing `llama_hub-0.0.1a1/llama_hub/outlook_localcalendar/README.md` & `llama_hub-0.0.1a2/llama_hub/outlook_localcalendar/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/outlook_localcalendar/base.py` & `llama_hub-0.0.1a2/llama_hub/outlook_localcalendar/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/pandas_ai/README.md` & `llama_hub-0.0.1a2/llama_hub/pandas_ai/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/pandas_ai/base.py` & `llama_hub-0.0.1a2/llama_hub/pandas_ai/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -90,15 +90,20 @@
             if isinstance(result, (np.generic)):
                 result = pd.Series(result)
             elif isinstance(result, (pd.Series, pd.DataFrame)):
                 pass
             else:
                 raise ValueError("Unexpected type for result: {}".format(type(result)))
             # if not conversational answer, use Pandas CSV Reader
-            PandasCSVReader = download_loader("PandasCSVReader")
+
+            try:
+                from llama_hub.utils import import_loader
+                PandasCSVReader = import_loader("PandasCSVReader")
+            except ImportError:
+                PandasCSVReader = download_loader("PandasCSVReader")
 
             reader = PandasCSVReader(
                 concat_rows=self._concat_rows,
                 col_joiner=self._col_joiner,
                 row_joiner=self._row_joiner,
                 pandas_config=self._pandas_config,
             )
```

### Comparing `llama_hub-0.0.1a1/llama_hub/papers/arxiv/README.md` & `llama_hub-0.0.1a2/llama_hub/papers/arxiv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/papers/arxiv/base.py` & `llama_hub-0.0.1a2/llama_hub/papers/arxiv/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,15 +139,19 @@
             }
             paper.download_pdf(dirpath=papers_dir, filename=filename)
             logging.debug(f"> Downloading {filename}...")
 
         def get_paper_metadata(filename):
             return paper_lookup[filename]
 
-        SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
+        try:
+            from llama_hub.utils import import_loader
+            SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
+        except ImportError: 
+            SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
         arxiv_documents = SimpleDirectoryReader(
             papers_dir, file_metadata=get_paper_metadata
         ).load_data()
         # Include extra documents containing the abstracts
         abstract_documents = []
         for paper in search_results:
             d = f"The following is a summary of the paper: {paper.title}\n\nSummary: {paper.summary}"
```

### Comparing `llama_hub-0.0.1a1/llama_hub/papers/pubmed/README.md` & `llama_hub-0.0.1a2/llama_hub/papers/pubmed/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/papers/pubmed/base.py` & `llama_hub-0.0.1a2/llama_hub/papers/pubmed/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/pinecone/README.md` & `llama_hub-0.0.1a2/llama_hub/pinecone/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/pinecone/base.py` & `llama_hub-0.0.1a2/llama_hub/pinecone/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/qdrant/README.md` & `llama_hub-0.0.1a2/llama_hub/qdrant/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/qdrant/base.py` & `llama_hub-0.0.1a2/llama_hub/qdrant/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/readwise/README.md` & `llama_hub-0.0.1a2/llama_hub/readwise/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/readwise/base.py` & `llama_hub-0.0.1a2/llama_hub/readwise/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/reddit/README.md` & `llama_hub-0.0.1a2/llama_hub/reddit/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/reddit/base.py` & `llama_hub-0.0.1a2/llama_hub/reddit/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/remote/README.md` & `llama_hub-0.0.1a2/llama_hub/remote/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/remote/base.py` & `llama_hub-0.0.1a2/llama_hub/remote/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,19 @@
         result = urlopen(req)
         url_type = result.info().get_content_type()
         documents = []
         if url_type == "text/html" or url_type == "text/plain":
             text = "\n\n".join([str(el.decode("utf-8-sig")) for el in result])
             documents = [Document(text, extra_info=extra_info)]
         elif self._is_youtube_video(url):
-            YoutubeTranscriptReader = download_loader("YoutubeTranscriptReader")
+            try:
+                from llama_hub.utils import import_loader
+                YoutubeTranscriptReader = import_loader("YoutubeTranscriptReader")
+            except ImportError:
+                YoutubeTranscriptReader = download_loader("YoutubeTranscriptReader")
             youtube_reader = YoutubeTranscriptReader()
             # TODO should we have another langauge, like english / french?
             documents = youtube_reader.load_data([url])
         else:
             suffix = Path(urlparse(url).path).suffix
             with tempfile.TemporaryDirectory() as temp_dir:
                 filepath = f"{temp_dir}/temp{suffix}"
```

### Comparing `llama_hub-0.0.1a1/llama_hub/remote_depth/README.md` & `llama_hub-0.0.1a2/llama_hub/remote_depth/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/remote_depth/base.py` & `llama_hub-0.0.1a2/llama_hub/remote_depth/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,19 @@
         self.depth = depth
         self.domain_lock = domain_lock
 
     def load_data(self, url: str) -> List[Document]:
         from tqdm.auto import tqdm
 
         """Parse whatever is at the URL.""" ""
-        RemoteReader = download_loader("RemoteReader")
+        try:
+            from llama_hub.utils import import_loader
+            RemoteReader = import_loader("RemoteReader")
+        except ImportError:
+            RemoteReader = download_loader("RemoteReader")
         remote_reader = RemoteReader(file_extractor=self.file_extractor)
         documents = []
         links = self.get_links(url)
         urls = {-1: [url]}  # -1 is the starting point
         links_visited = []
         for i in range(self.depth + 1):
             urls[i] = []
```

### Comparing `llama_hub-0.0.1a1/llama_hub/s3/README.md` & `llama_hub-0.0.1a2/llama_hub/s3/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/s3/base.py` & `llama_hub-0.0.1a2/llama_hub/s3/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,11 +85,15 @@
                         continue
                     suffix = Path(obj.key).suffix
                     filepath = (
                         f"{temp_dir}/{next(tempfile._get_candidate_names())}{suffix}"
                     )
                     s3_client.download_file(self.bucket, obj.key, filepath)
 
-            SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
+            try:
+                from llama_hub.utils import import_loader
+                SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
+            except ImportError:
+                SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
             loader = SimpleDirectoryReader(temp_dir, file_extractor=self.file_extractor)
 
             return loader.load_data()
```

### Comparing `llama_hub-0.0.1a1/llama_hub/slack/README.md` & `llama_hub-0.0.1a2/llama_hub/slack/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/slack/base.py` & `llama_hub-0.0.1a2/llama_hub/slack/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/snscrape_twitter/README.md` & `llama_hub-0.0.1a2/llama_hub/snscrape_twitter/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/snscrape_twitter/base.py` & `llama_hub-0.0.1a2/llama_hub/snscrape_twitter/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/spotify/README.md` & `llama_hub-0.0.1a2/llama_hub/spotify/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/spotify/base.py` & `llama_hub-0.0.1a2/llama_hub/spotify/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/stackoverflow/README.md` & `llama_hub-0.0.1a2/llama_hub/stackoverflow/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/stackoverflow/base.py` & `llama_hub-0.0.1a2/llama_hub/stackoverflow/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/steamship/README.md` & `llama_hub-0.0.1a2/llama_hub/steamship/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/steamship/base.py` & `llama_hub-0.0.1a2/llama_hub/steamship/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/string_iterable/README.md` & `llama_hub-0.0.1a2/llama_hub/string_iterable/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/string_iterable/base.py` & `llama_hub-0.0.1a2/llama_hub/string_iterable/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/trello/README.md` & `llama_hub-0.0.1a2/llama_hub/trello/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/trello/base.py` & `llama_hub-0.0.1a2/llama_hub/trello/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/twitter/README.md` & `llama_hub-0.0.1a2/llama_hub/twitter/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/twitter/base.py` & `llama_hub-0.0.1a2/llama_hub/twitter/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/weather/README.md` & `llama_hub-0.0.1a2/llama_hub/weather/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/weather/base.py` & `llama_hub-0.0.1a2/llama_hub/weather/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/weaviate/README.md` & `llama_hub-0.0.1a2/llama_hub/weaviate/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/weaviate/base.py` & `llama_hub-0.0.1a2/llama_hub/weaviate/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/async_web/base.py` & `llama_hub-0.0.1a2/llama_hub/web/async_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/beautiful_soup_web/README.md` & `llama_hub-0.0.1a2/llama_hub/web/beautiful_soup_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/beautiful_soup_web/base.py` & `llama_hub-0.0.1a2/llama_hub/web/beautiful_soup_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/knowledge_base/README.md` & `llama_hub-0.0.1a2/llama_hub/web/knowledge_base/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/knowledge_base/base.py` & `llama_hub-0.0.1a2/llama_hub/web/knowledge_base/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/readability_web/README.md` & `llama_hub-0.0.1a2/llama_hub/web/readability_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/readability_web/Readability.js` & `llama_hub-0.0.1a2/llama_hub/web/readability_web/Readability.js`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/readability_web/base.py` & `llama_hub-0.0.1a2/llama_hub/web/readability_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/rss/base.py` & `llama_hub-0.0.1a2/llama_hub/web/rss/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/simple_web/README.md` & `llama_hub-0.0.1a2/llama_hub/web/simple_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/simple_web/base.py` & `llama_hub-0.0.1a2/llama_hub/web/simple_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/trafilatura_web/README.md` & `llama_hub-0.0.1a2/llama_hub/web/trafilatura_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/trafilatura_web/base.py` & `llama_hub-0.0.1a2/llama_hub/web/trafilatura_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/unstructured_web/README.md` & `llama_hub-0.0.1a2/llama_hub/web/unstructured_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/web/unstructured_web/base.py` & `llama_hub-0.0.1a2/llama_hub/web/unstructured_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/whatsapp/README.md` & `llama_hub-0.0.1a2/llama_hub/whatsapp/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/whatsapp/base.py` & `llama_hub-0.0.1a2/llama_hub/whatsapp/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/wikipedia/README.md` & `llama_hub-0.0.1a2/llama_hub/wikipedia/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/wikipedia/base.py` & `llama_hub-0.0.1a2/llama_hub/wikipedia/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/wordpress/README.md` & `llama_hub-0.0.1a2/llama_hub/wordpress/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/wordpress/base.py` & `llama_hub-0.0.1a2/llama_hub/wordpress/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/youtube_transcript/README.md` & `llama_hub-0.0.1a2/llama_hub/youtube_transcript/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/youtube_transcript/base.py` & `llama_hub-0.0.1a2/llama_hub/youtube_transcript/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/zendesk/README.md` & `llama_hub-0.0.1a2/llama_hub/zendesk/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/zendesk/base.py` & `llama_hub-0.0.1a2/llama_hub/zendesk/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/zulip/README.md` & `llama_hub-0.0.1a2/llama_hub/zulip/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/llama_hub/zulip/base.py` & `llama_hub-0.0.1a2/llama_hub/zulip/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.1a1/pyproject.toml` & `llama_hub-0.0.1a2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
-name = "llama-hub"
-version = "0.0.1.alpha1"
+name = "llama_hub"
+version = "0.0.1.alpha2"
 description = "A library of community-driven data loaders for LLMs. Use with LlamaIndex and/or LangChain. "
-authors = ["Jerry Liu"]
+authors = ["Jerry Liu", "Jesse Zhang"]
 # New attributes
 license = "MIT"
 readme = "README.md"
 homepage = "https://llamahub.ai"
 repository = "https://github.com/emptycrown/llama-hub"
 keywords = ["llama-index", "llama-hub", "llama"]
 include = [
@@ -15,14 +15,15 @@
 
 [tool.poetry.dependencies]
 # Updated Python version
 python = ">=3.8.1,<4.0"
 llama-index = ">=0.6.9"
 atlassian-python-api = "*"
 html2text = "*"
+psutil = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 pytest-dotenv = "0.5.2"
 typing-inspect = "0.8.0"
 typing_extensions = "4.5.0"
 types-requests = "2.28.11.8"
```

### Comparing `llama_hub-0.0.1a1/PKG-INFO` & `llama_hub-0.0.1a2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,134 @@
 Metadata-Version: 2.1
 Name: llama-hub
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A library of community-driven data loaders for LLMs. Use with LlamaIndex and/or LangChain. 
 Home-page: https://llamahub.ai
 License: MIT
 Keywords: llama-index,llama-hub,llama
 Author: Jerry Liu
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: atlassian-python-api
 Requires-Dist: html2text
 Requires-Dist: llama-index (>=0.6.9)
+Requires-Dist: psutil
 Project-URL: Repository, https://github.com/emptycrown/llama-hub
 Description-Content-Type: text/markdown
 
 # LlamaHub 🦙
 
-This is a simple library of all the data loaders / readers that have been created by the community. The goal is to make it extremely easy to connect large language models to a large variety of knowledge sources. These are general-purpose utilities that are meant to be used in [LlamaIndex](https://github.com/jerryjliu/gpt_index/tree/main/gpt_index) (e.g. when building a index) and [LangChain](https://github.com/hwchase17/langchain) (e.g. when building different tools an agent can use). For example, there are loaders to parse Google Docs, SQL Databases, PDF files, PowerPoints, Notion, Slack, Obsidian, and many more. Note that because different loaders produce the same types of Documents, you can easily use them together in the same index.
+This is a simple library of all the data loaders / readers that have been created by the community. The goal is to make it extremely easy to connect large language models to a large variety of knowledge sources. These are general-purpose utilities that are meant to be used in [LlamaIndex](https://github.com/jerryjliu/llama_index) (e.g. when building a index) and [LangChain](https://github.com/hwchase17/langchain) (e.g. when building different tools an agent can use). For example, there are loaders to parse Google Docs, SQL Databases, PDF files, PowerPoints, Notion, Slack, Obsidian, and many more. Note that because different loaders produce the same types of Documents, you can easily use them together in the same index.
 
 Check out our website here: https://llamahub.ai/.
 
 ![Website screenshot](https://scrabble-dictionary.s3.us-west-2.amazonaws.com/Screen+Shot+2023-02-11+at+12.45.44+PM.png)
 
-## Usage
+## Usage (Use `llama-hub` as PyPI package)
+These general-purpose loaders are designed to be used as a way to load data into [LlamaIndex](https://github.com/jerryjliu/llama_index) and/or subsequently used in [LangChain](https://github.com/hwchase17/langchain). 
 
-These general-purpose loaders are designed to be used as a way to load data into [LlamaIndex](https://github.com/jerryjliu/gpt_index/tree/main/gpt_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. **You can use them with `download_loader` from LlamaIndex in a single line of code!** For example, see the code snippets below using the Google Docs Loader.
+### Installation
+```
+pip install llama-hub
+```
 
 ### LlamaIndex
 
 ```python
-from llama_index import GPTVectorStoreIndex, download_loader
-
-GoogleDocsReader = download_loader('GoogleDocsReader')
+from llama_index import GPTVectorStoreIndex
+from llama_hub.google_docs.base import GoogleDocsReader
 
 gdoc_ids = ['1wf-y2pd9C878Oh-FmLH7Q_BQkljdm6TQal-c1pUfrec']
 loader = GoogleDocsReader()
 documents = loader.load_data(document_ids=gdoc_ids)
 index = GPTVectorStoreIndex.from_documents(documents)
 index.query('Where did the author go to school?')
 ```
 
 ### LangChain
 
 Note: Make sure you change the description of the `Tool` to match your use-case.
 
 ```python
-from llama_index import GPTVectorStoreIndex, download_loader
+from llama_index import GPTVectorStoreIndex
+from llama_hub.google_docs.base import GoogleDocsReader
 from langchain.llms import OpenAI
 from langchain.chains.question_answering import load_qa_chain
 
 # load documents
-GoogleDocsReader = download_loader('GoogleDocsReader')
 gdoc_ids = ['1wf-y2pd9C878Oh-FmLH7Q_BQkljdm6TQal-c1pUfrec']
 loader = GoogleDocsReader()
 documents = loader.load_data(document_ids=gdoc_ids)
 langchain_documents = [d.to_langchain_format() for d in documents]
 
 # initialize sample QA chain
 llm = OpenAI(temperature=0)
 qa_chain = load_qa_chain(llm)
 question="<query here>"
 answer = qa_chain.run(input_documents=langchain_documents, question=question)
 
 ```
+## Usage (Use `download_loader` from LlamaIndex)
+
+You can also use the loaders with `download_loader` from LlamaIndex in a single line of code.
+
+For example, see the code snippets below using the Google Docs Loader.
+
+```python
+from llama_index import GPTVectorStoreIndex, download_loader
+
+GoogleDocsReader = download_loader('GoogleDocsReader')
+
+gdoc_ids = ['1wf-y2pd9C878Oh-FmLH7Q_BQkljdm6TQal-c1pUfrec']
+loader = GoogleDocsReader()
+documents = loader.load_data(document_ids=gdoc_ids)
+index = GPTVectorStoreIndex.from_documents(documents)
+index.query('Where did the author go to school?')
+
+```
+
 
 ## How to add a loader
 
 Adding a loader simply requires forking this repo and making a Pull Request. The Loader Hub website will update automatically. However, please keep in the mind the following guidelines when making your PR.
 
+### Step 0: Setup virtual environment, install Poetry and dependencies
+
+Create a new Python virtual environment. The command below creates an environment in `.venv`,
+and activates it:
+```bash
+python -m venv .venv
+source .venv/bin/activate
+```
+
+if you are in windows, use the following to activate your virtual environment:
+
+```bash
+.venv\scripts\activate
+```
+
+Install poetry:
+
+```bash
+pip install poetry
+```
+
+Install the required dependencies (this will also install `llama_index`):
+
+```bash
+poetry install
+```
+
+This will create an editable install of `llama-hub` in your venv.
+
+
 ### Step 1: Create a new directory
 
 In `llama_hub`, create a new directory for your new loader. It can be nested within another, but name it something unique because the name of the directory will become the identifier for your loader (e.g. `google_docs`). Inside your new directory, create a `__init__.py` file, which can be empty, a `base.py` file which will contain your loader implementation, and, if needed, a `requirements.txt` file to list the package dependencies of your loader. Those packages will automatically be installed when your loader is used, so no need to worry about that anymore!
 
 If you'd like, you can create the new directory and files by running the following script in the `llama_hub` directory. Just remember to put your dependencies into a `requirements.txt` file.
 
 ```
@@ -98,15 +151,15 @@
 ## Running tests
 
 ```shell
 python3.9 -m venv .venv
 source .venv/bin/activate 
 pip3 install -r test_requirements.txt
 
-python3 -m pytest tests 
+poetry run pytest tests 
 ```
 
 ## FAQ
 
 ### How do I test my loader before it's merged?
 
 There is an argument called `loader_hub_url` in [`download_loader`](https://github.com/jerryjliu/llama_index/blob/main/llama_index/readers/download.py) that defaults to the main branch of this repo. You can set it to your branch or fork to test your new loader.
```

