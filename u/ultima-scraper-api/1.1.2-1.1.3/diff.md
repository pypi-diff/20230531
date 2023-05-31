# Comparing `tmp/ultima_scraper_api-1.1.2.tar.gz` & `tmp/ultima_scraper_api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-1.1.2.tar", max compression
+gzip compressed data, was "ultima_scraper_api-1.1.3.tar", max compression
```

## Comparing `ultima_scraper_api-1.1.2.tar` & `ultima_scraper_api-1.1.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1193 2023-05-22 20:42:52.442027 ultima_scraper_api-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.1.2/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2286 2023-05-13 21:02:27.542962 ultima_scraper_api-1.1.2/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.1.2/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6875 2023-05-10 16:14:24.886974 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     3348 2023-05-22 07:12:01.748229 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     2895 2023-05-09 15:10:07.346536 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    19475 2023-05-22 10:26:50.629643 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0    11481 2023-05-22 10:32:32.883960 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6463 2023-05-13 21:26:45.672240 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0      862 2023-05-14 01:36:53.261674 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/subscription_model.py
--rw-r--r--   0        0        0    27593 2023-05-22 08:33:43.650098 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     2961 2023-05-22 10:30:47.276706 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     2784 2023-05-10 22:02:50.317100 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      191 2023-05-11 21:59:14.648026 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    19161 2023-05-22 10:10:45.530951 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0    11385 2023-05-22 06:26:19.792870 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2971 2023-05-10 21:01:08.286698 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
--rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0     1623 2023-05-13 21:04:18.608237 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
--rw-r--r--   0        0        0    28146 2023-05-22 08:33:34.023692 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     3242 2023-05-22 07:26:53.595528 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2763 2023-05-05 07:56:21.734680 ultima_scraper_api-1.1.2/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.1.2/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.1.2/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.1.2/ultima_scraper_api/classes/prepare_directories.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.2/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-1.1.2/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.2/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.2/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.2/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.1.2/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.1.2/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.1.2/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.1.2/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    11324 2023-05-09 19:08:54.838979 ultima_scraper_api-1.1.2/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.1.2/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.1.2/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     1792 2023-05-13 20:28:21.224283 ultima_scraper_api-1.1.2/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.1.2/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      767 2023-05-12 15:00:15.819155 ultima_scraper_api-1.1.2/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2181 2023-03-27 18:00:12.375116 ultima_scraper_api-1.1.2/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    17628 2023-05-22 20:22:30.307904 ultima_scraper_api-1.1.2/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-1.1.2/ultima_scraper_api/models/__init__.py
--rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-1.1.2/ultima_scraper_api/models/subscription_model.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.1.2/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 ultima_scraper_api-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1193 2023-05-31 21:40:39.725354 ultima_scraper_api-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.1.3/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2286 2023-05-13 21:02:27.542962 ultima_scraper_api-1.1.3/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.1.3/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6875 2023-05-10 16:14:24.886974 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     3348 2023-05-22 07:12:01.748229 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2895 2023-05-09 15:10:07.346536 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    19575 2023-05-28 15:42:17.825968 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0    11479 2023-05-28 15:33:55.688326 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6463 2023-05-31 08:46:59.121721 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     6918 2023-04-09 17:42:13.567826 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0      862 2023-05-14 01:36:53.261674 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/subscription_model.py
+-rw-r--r--   0        0        0    27593 2023-05-22 08:33:43.650098 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     2961 2023-05-22 10:30:47.276706 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2784 2023-05-10 22:02:50.317100 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-11 21:59:14.648026 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    19223 2023-05-31 11:24:17.146008 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0    11391 2023-05-31 18:58:22.644908 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2970 2023-05-31 09:00:33.734398 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
+-rw-r--r--   0        0        0     3375 2023-03-27 00:23:55.042753 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1318 2023-04-09 10:09:44.773447 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0     1623 2023-05-13 21:04:18.608237 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
+-rw-r--r--   0        0        0    28464 2023-05-31 11:29:25.511752 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     3242 2023-05-31 11:23:04.368930 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2763 2023-05-05 07:56:21.734680 ultima_scraper_api-1.1.3/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_directories.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.1.3/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.1.3/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    11343 2023-05-28 15:06:20.263463 ultima_scraper_api-1.1.3/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     1911 2023-05-31 10:43:31.029509 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      767 2023-05-12 15:00:15.819155 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2181 2023-05-31 11:25:12.717213 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    18054 2023-05-31 16:21:52.459421 ultima_scraper_api-1.1.3/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-1.1.3/ultima_scraper_api/models/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-1.1.3/ultima_scraper_api/models/subscription_model.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.1.3/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 ultima_scraper_api-1.1.3/PKG-INFO
```

### Comparing `ultima_scraper_api-1.1.2/pyproject.toml` & `ultima_scraper_api-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "1.1.2"
+version = "1.1.3"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/__init__.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/api_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/api_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         if valid_user:
             return valid_user
         else:
             link = endpoint_links(identifier).users
             response = await self.session_manager.json_request(link)
             if "error" not in response:
                 response["session_manager"] = self.session_manager
-                response = create_user(response, self)
+                response = create_user(response["response"][0], self)
             return response
 
     async def get_lists_users(
         self,
         identifier: int | str,
         check: bool = False,
         limit: int = 100,
@@ -305,24 +305,27 @@
                     new_date = datetime.now() + relativedelta(years=10)
                     new_date = int(new_date.timestamp() * 1000)
                     following.subscribedByData = {}
                     following.subscribedByData["endsAt"] = new_date
         return final_followings
 
     async def get_subscription(
-        self, identifier: int | str = "", custom_list: list[create_user] = []
-    ) -> create_user | None:
+        self, identifier: int | str = "", custom_list: list[SubscriptionModel] = []
+    ) -> SubscriptionModel | None:
         subscriptions = (
             await self.get_subscriptions(refresh=False)
             if not custom_list
             else custom_list
         )
         valid = None
         for subscription in subscriptions:
-            if identifier == subscription.username or identifier == subscription.id:
+            if (
+                identifier == subscription.user.username
+                or identifier == subscription.user.id
+            ):
                 valid = subscription
                 break
         return valid
 
     async def get_subscriptions(
         self,
         refresh: bool = True,
@@ -342,28 +345,28 @@
             if isinstance(user, dict):
                 user = create_user(raw_subscription, self)
                 user.active = False
             subscription_model = SubscriptionModel(raw_subscription, user, self)
             return subscription_model
 
         subscriptions: list[SubscriptionModel] = []
-        if identifiers:
-            found_raw_subscriptions: list[dict[str, Any]] = []
-            for identifier in identifiers:
-                for raw_subscription in raw_subscriptions:
-                    if (
-                        identifier == raw_subscription["id"]
-                        or identifier == raw_subscription["username"]
-                    ):
-                        found_raw_subscriptions.append(raw_subscription)
-                        break
-            raw_subscriptions = found_raw_subscriptions
         with self.get_pool() as pool:
             tasks = pool.starmap(assign_user_to_sub, product(raw_subscriptions))
             subscriptions: list[SubscriptionModel] = await asyncio.gather(*tasks)
+            if identifiers:
+                found_subscriptions: list[SubscriptionModel] = []
+                for identifier in identifiers:
+                    for subscription in subscriptions:
+                        if (
+                            identifier == subscription.user.id
+                            or identifier == subscription.user.username
+                        ):
+                            found_subscriptions.append(subscription)
+                            break
+                subscriptions = found_subscriptions
 
         match sub_type:
             case "all":
                 pass
             case "active":
                 subscriptions = [
                     x for x in subscriptions if x.ends_at > datetime.utcnow()
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     ):
         domain = "https://apiv3.fansly.com"
         api = "/api/v1"
         full_url_path = f"{domain}{api}"
         self.full_url_path = full_url_path
         self.customer = f"{full_url_path}/account?ids={identifier}"
         self.settings = f"{full_url_path}/account/settings"
-        self.users = f"https://onlyfans.com/api2/v2/users/{identifier}"
+        self.users = f"{self.full_url_path}/account?ids={identifier}"
         self.followings = f"{full_url_path}/account/{identifier}/following?before={global_offset}&after=0&limit=100&offset=0"
         self.subscriptions = f"{full_url_path}/subscriptions"
         self.lists = f"https://onlyfans.com/api2/v2/lists?limit={global_limit}&offset={global_offset}"
         self.lists_users = f"https://onlyfans.com/api2/v2/lists/{identifier}/users?limit={global_limit}&offset={global_offset}&query="
         self.list_chats = f"{full_url_path}/messaging/groups?sortOrder=1&flags=0&subscriptionTierId=&search=&limit={global_limit}&offset={global_offset}"
         self.post_by_id = f"https://onlyfans.com/api2/v2/posts/{identifier}"
         self.message_by_id = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit=10&offset=0&firstId={identifier2}&order=desc&skip_users=all&skip_users_dups=1"
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/subscription_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,16 @@
                     ):
                         found_raw_subscriptions.append(raw_subscription)
                         break
             raw_subscriptions = found_raw_subscriptions
         with self.get_pool() as pool:
             tasks = pool.starmap(assign_user_to_sub, product(raw_subscriptions))
             subscriptions: list[SubscriptionModel] = await asyncio.gather(*tasks)
-        return subscriptions
+        self.subscriptions = subscriptions
+        return self.subscriptions
 
     async def get_chats(
         self,
         links: list[str] = [],
         limit: int = 100,
         offset: int = 0,
         depth: int = 1,
@@ -462,15 +463,15 @@
                 final_results.extend(results2)
             if not inside_loop:
                 temp: list[create_message | create_post] = []
                 for final_result in final_results:
                     content = None
                     if final_result["responseType"] == "message":
                         user = await self.get_user(final_result["fromUser"]["id"])
-                        if not user:
+                        if isinstance(user, dict):
                             user = create_user(final_result["fromUser"], self)
                         content = create_message(final_result, user)
                     elif final_result["responseType"] == "post":
                         user = create_user(final_result["author"], self)
                         content = create_post(final_result, user)
                     if content:
                         temp.append(content)
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         self.mass_messages_api = f"https://onlyfans.com/api2/v2/messages/queue/stats?limit=100&offset=0&format=infinite"
         self.stories_api = f"https://onlyfans.com/api2/v2/users/{identifier}/stories?limit=100&offset=0&order=desc"
         self.list_highlights = f"https://onlyfans.com/api2/v2/users/{identifier}/stories/highlights?limit=100&offset=0&order=desc"
         self.highlight = f"https://onlyfans.com/api2/v2/stories/highlights/{identifier}"
         self.list_posts_api = self.list_posts(identifier)
         self.archived_posts = f"https://onlyfans.com/api2/v2/users/{identifier}/posts/archived?limit={global_limit}&offset={global_offset}&order=publish_date_desc"
         self.archived_stories = f"https://onlyfans.com/api2/v2/stories/archive/?limit=100&offset=0&order=publish_date_desc"
-        self.paid_api = f"https://onlyfans.com/api2/v2/posts/paid?{global_limit}&offset={global_offset}"
+        self.paid_api = f"https://onlyfans.com/api2/v2/posts/paid?limit={global_limit}&offset={global_offset}"
         self.pay = f"https://onlyfans.com/api2/v2/payments/pay"
         self.subscribe = f"https://onlyfans.com/api2/v2/users/{identifier}/subscribe"
         self.like = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/like"
         self.favorite = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/favorites/{identifier3}"
         self.transactions = (
             f"https://onlyfans.com/api2/v2/payments/all/transactions?limit=10&offset=0"
         )
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 
 
 class create_message(SiteContent):
     def __init__(self, option: dict[str, Any], user: create_user) -> None:
-
         author = user.get_authed().find_user_by_identifier(option["fromUser"]["id"])
         self.user = user
         SiteContent.__init__(self, option, author)
         self.responseType: Optional[str] = option.get("responseType")
         self.text: str = option.get("text", "")
         self.lockedText: Optional[bool] = option.get("lockedText")
         self.isFree: Optional[bool] = option.get("isFree")
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/only_drm.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/only_drm.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         self.canTrialSend: bool = option.get("canTrialSend")
         self.canAddPhone: bool = option.get("canAddPhone")
         self.phoneLast4: Any = option.get("phoneLast4")
         self.phoneMask: Any = option.get("phoneMask")
         self.hasNewTicketReplies: dict = option.get("hasNewTicketReplies")
         self.hasInternalPayments: bool = option.get("hasInternalPayments")
         self.isCreditsEnabled: bool = option.get("isCreditsEnabled")
-        self.creditBalance: float = option.get("creditBalance")
+        self.creditBalance: float = option.get("creditBalance", 0.0)
         self.isMakePayment: bool = option.get("isMakePayment")
         self.isOtpEnabled: bool = option.get("isOtpEnabled")
         self.email: str = option.get("email")
         self.isEmailChecked: bool = option.get("isEmailChecked")
         self.isLegalApprovedAllowed: bool = option.get("isLegalApprovedAllowed")
         self.isTwitterConnected: bool = option.get("isTwitterConnected")
         self.twitterUsername: Any = option.get("twitterUsername")
@@ -561,34 +561,40 @@
 
     async def get_header(self):
         return self.header
 
     async def is_subscribed(self):
         return not self.subscribedIsExpiredNow
 
-    async def get_paid_contents(self):
+    async def get_paid_contents(self, content_type: str | None = None):
         # REMINDER THAT YOU'LL HAVE TO REFRESH CONTENT
         final_paid_content: list[create_post | message_model.create_message] = []
         authed = self.get_authed()
         for paid_content in authed.paid_content:
+            # Just use response to key function in ContentTypes
             if paid_content.author.id == self.id:
+                if (
+                    content_type is not None
+                    and content_type.lower() != f"{paid_content.responseType}s"
+                ):
+                    continue
                 final_paid_content.append(paid_content)
         return final_paid_content
 
     async def has_socials(self):
         # If error message, this means the user has socials, but we have to subscribe to see them
         result = bool(
             await self.get_session_manager().json_request(
                 endpoint_links(self.id).socials
             )
         )
         return result
 
     async def get_socials(self):
-        result = await self.get_session_manager().json_request(
+        result: list[dict[str, Any]] = await self.get_session_manager().json_request(
             endpoint_links(self.id).socials
         )
         if "error" in result:
             return []
         return result
 
     async def get_spotify(self):
@@ -596,15 +602,15 @@
             result = await self.get_session_manager().json_request(
                 endpoint_links(self.id).spotify
             )
             if "error" in result:
                 return []
             return result
 
-    async def has_socials(self):
+    async def has_spotify(self):
         # If error message, this means the user has socials, but we have to subscribe to see them
         result = bool(
             await self.get_session_manager().json_request(
                 endpoint_links(self.id).spotify
             )
         )
         return result
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/apis/user_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/classes/prepare_directories.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_directories.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-1.1.3/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-1.1.3/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/helpers/main_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     # https://github.com/giampaolo/psutil/blob/master/psutil/_common.py#L176
     sdiskusage = namedtuple("sdiskusage", ["total", "used", "free", "percent"])
 
     # psutil likes to round the disk usage percentage to 1 decimal
     # https://github.com/giampaolo/psutil/blob/master/psutil/_common.py#L365
     def disk_usage(path: str, round_: int = 1):
-
         # check if path exists
         if not os.path.exists(path):
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), path)
 
         # on POSIX systems you can pass either a file or a folder path
         # Windows only allows folder paths
         if not os.path.isdir(path):
@@ -274,23 +273,23 @@
             embed.add_field("username", username)
             message.embeds.append(embed)
             message = orjson.loads(json.dumps(message, default=lambda o: o.__dict__))
             requests.post(webhook_link, json=message)
     if category == "download_webhook":
         subscriptions = await item.get_subscriptions(refresh=False)
         for subscription in subscriptions:
-            if await subscription.if_scraped():
+            if await subscription.user.if_scraped():
                 for webhook_link in webhook_links:
                     message = prepare_webhooks.discord()
                     embed = message.embed()
                     embed.title = f"Downloaded: {subscription.username}"
                     embed.add_field("username", subscription.username)
-                    embed.add_field("post_count", subscription.postsCount)
-                    embed.add_field("link", subscription.get_link())
-                    embed.image.url = subscription.avatar
+                    embed.add_field("post_count", subscription.user.postsCount)
+                    embed.add_field("link", subscription.user.get_link())
+                    embed.image.url = subscription.user.avatar
                     message.embeds.append(embed)
                     message = orjson.loads(
                         json.dumps(message, default=lambda o: o.__dict__)
                     )
                     requests.post(webhook_link, json=message)
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 user_types = ultima_scraper_api.user_types
 
 
 class JobManager:
     def __init__(self) -> None:
         self.jobs: list[CustomJob] = []
         self.queue: asyncio.Queue[Any] = asyncio.Queue()
-        self.worker_task = asyncio.create_task(self.worker())
 
     def create_jobs(
         self, value: str, type_values: list[str], module: Any, module_args: list[Any]
     ):
         local_jobs: list[CustomJob] = []
         for type_value in type_values:
             local_args = copy.copy(module_args)
@@ -38,17 +37,21 @@
         self.jobs.extend(local_jobs)
         return local_jobs
 
     def add_media_type_to_jobs(self, media_type: str | list[str]):
         if isinstance(media_type, str):
             media_type = [media_type]
         [job.add_media_type(mt) for job in self.jobs for mt in media_type]
-
-    async def worker(self):
+    async def process_jobs(self):
+        await asyncio.create_task(self.__worker())
+        await self.queue.join()
+    async def __worker(self):
         while True:
+            if self.queue.qsize() == 0:
+                return
             job = await self.queue.get()
             # We can make jobs work in the background if we make waiting for inputs async
             await job.task
 
             self.queue.task_done()
 
             # print(f'{job.type} has been processed')
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/managers/scrape_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/managers/session_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 from random import randint
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urlparse
 
 import aiohttp
 import python_socks
 import requests
-import ultima_scraper_api
-import ultima_scraper_api.apis.api_helper as api_helper
 from aiohttp import ClientResponse, ClientSession
 from aiohttp.client_exceptions import (
     ClientConnectorError,
     ClientOSError,
     ClientPayloadError,
     ClientResponseError,
     ContentTypeError,
     ServerDisconnectedError,
 )
 from aiohttp_socks import ProxyConnectionError, ProxyConnector, ProxyError, ProxyInfo
 
+import ultima_scraper_api
+import ultima_scraper_api.apis.api_helper as api_helper
+
 if TYPE_CHECKING:
     auth_types = ultima_scraper_api.auth_types
 EXCEPTION_TEMPLATE = (
     ClientPayloadError,
     ContentTypeError,
     ClientOSError,
     ServerDisconnectedError,
@@ -142,15 +143,18 @@
         connector = (
             self.proxy_manager.create_connection(proxy)
             if self.proxies
             else aiohttp.TCPConnector(limit=limit)
         )
         final_cookies = self.get_cookies()
         # Had to remove final_cookies and cookies=final_cookies due to it conflicting with headers
-        timeout = aiohttp.ClientTimeout(total=None)
+        # timeout = aiohttp.ClientTimeout(None)
+        timeout = aiohttp.ClientTimeout(
+            total=None, connect=10, sock_connect=10, sock_read=60
+        )
         client_session = ClientSession(
             connector=connector, cookies=final_cookies, timeout=timeout
         )
         return client_session
 
     def get_proxy(self) -> str:
         proxies = self.proxies
@@ -196,14 +200,16 @@
                             print(proxy_manager.get_current_proxy().host)
 
                         result = await self.active_session.get(url, headers=headers)
                         result.raise_for_status()
                         self.rate_limit_check = False
                         self.is_rate_limited = None
                         break
+                    except EXCEPTION_TEMPLATE as _e:
+                        continue
                     except ClientResponseError as _e:
                         if _e.status == 429:
                             # Still rate limited, wait 5 seconds and retry
                             self.is_rate_limited = True
                             rate_limit_count += 1
                     except Exception as _e:
                         pass
@@ -268,21 +274,28 @@
             except Exception as _e:
                 pass
 
     async def bulk_requests(self, urls: list[str]) -> list[ClientResponse | None]:
         return await asyncio.gather(*[self.request(url) for url in urls])
 
     async def json_request(self, url: str):
-        response = await self.request(url)
-        json_resp: dict[Any, Any] = {}
-        if response.status == 200:
-            json_resp = await response.json()
-        else:
-            json_resp["error"] = {"code": response.status, "message": response.reason}
-        return json_resp
+        while True:
+            response = await self.request(url)
+            json_resp: dict[Any, Any] = {}
+            try:
+                if response.status == 200:
+                    json_resp = await response.json()
+                else:
+                    json_resp["error"] = {
+                        "code": response.status,
+                        "message": response.reason,
+                    }
+                return json_resp
+            except EXCEPTION_TEMPLATE as _e:
+                continue
 
     async def bulk_json_requests(self, urls: list[str]) -> list[dict[Any, Any]]:
         return await asyncio.gather(*[self.json_request(url) for url in urls])
 
     async def json_request_2(
         self,
         link: str,
```

### Comparing `ultima_scraper_api-1.1.2/ultima_scraper_api/models/subscription_model.py` & `ultima_scraper_api-1.1.3/ultima_scraper_api/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.2/PKG-INFO` & `ultima_scraper_api-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

