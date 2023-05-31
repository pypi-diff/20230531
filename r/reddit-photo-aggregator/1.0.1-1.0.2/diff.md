# Comparing `tmp/reddit_photo_aggregator-1.0.1.tar.gz` & `tmp/reddit_photo_aggregator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_photo_aggregator-1.0.1.tar", last modified: Tue May 30 09:49:18 2023, max compression
+gzip compressed data, was "reddit_photo_aggregator-1.0.2.tar", last modified: Tue May 30 10:14:37 2023, max compression
```

## Comparing `reddit_photo_aggregator-1.0.1.tar` & `reddit_photo_aggregator-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:18.348260 reddit_photo_aggregator-1.0.1/
--rw-rw-rw-   0        0        0      485 2023-05-29 20:52:19.000000 reddit_photo_aggregator-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      727 2023-05-30 09:49:18.348260 reddit_photo_aggregator-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      144 2023-05-29 20:45:14.000000 reddit_photo_aggregator-1.0.1/README.md
--rw-rw-rw-   0        0        0      719 2023-05-30 09:48:58.000000 reddit_photo_aggregator-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 09:49:18.348260 reddit_photo_aggregator-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:18.322254 reddit_photo_aggregator-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:18.334256 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/
--rw-rw-rw-   0        0        0      233 2023-05-30 09:18:23.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/__init__.py
--rw-rw-rw-   0        0        0      135 2023-05-30 09:17:21.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/exceptions.py
--rw-rw-rw-   0        0        0     1280 2023-05-30 09:13:40.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/image.py
--rw-rw-rw-   0        0        0     2061 2023-05-30 09:16:00.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/image_validator.py
--rw-rw-rw-   0        0        0      161 2023-05-30 09:14:23.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/sorting.py
--rw-rw-rw-   0        0        0     2051 2023-05-30 09:24:09.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/subreddit.py
--rw-rw-rw-   0        0        0     1512 2023-05-29 15:21:03.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/user_agent.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:18.346259 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator.egg-info/
--rw-rw-rw-   0        0        0      727 2023-05-30 09:49:18.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-30 09:49:18.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:49:18.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-30 09:49:18.000000 reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 10:14:37.154724 reddit_photo_aggregator-1.0.2/
+-rw-rw-rw-   0        0        0      485 2023-05-29 20:52:19.000000 reddit_photo_aggregator-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      727 2023-05-30 10:14:37.153725 reddit_photo_aggregator-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      144 2023-05-29 20:45:14.000000 reddit_photo_aggregator-1.0.2/README.md
+-rw-rw-rw-   0        0        0      734 2023-05-30 10:14:07.000000 reddit_photo_aggregator-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 10:14:37.154724 reddit_photo_aggregator-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 10:14:37.128718 reddit_photo_aggregator-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 10:14:37.140721 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/
+-rw-rw-rw-   0        0        0      233 2023-05-30 09:18:23.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/__init__.py
+-rw-rw-rw-   0        0        0      135 2023-05-30 09:17:21.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/exceptions.py
+-rw-rw-rw-   0        0        0     1280 2023-05-30 09:13:40.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/image.py
+-rw-rw-rw-   0        0        0     2061 2023-05-30 09:16:00.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/image_validator.py
+-rw-rw-rw-   0        0        0      161 2023-05-30 09:14:23.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/sorting.py
+-rw-rw-rw-   0        0        0     2051 2023-05-30 09:24:09.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/subreddit.py
+-rw-rw-rw-   0        0        0     1512 2023-05-29 15:21:03.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:14:37.152724 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator.egg-info/
+-rw-rw-rw-   0        0        0      727 2023-05-30 10:14:37.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-30 10:14:37.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 10:14:37.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-30 10:14:37.000000 reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator.egg-info/top_level.txt
```

### Comparing `reddit_photo_aggregator-1.0.1/PKG-INFO` & `reddit_photo_aggregator-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_photo_aggregator
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library to scrape subreddits for images
 Author-email: hamolicious <hamolicious@outlook.com>
 Project-URL: Homepage, https://github.com/hamolicious/Reddit-Photo-Aggregator
 Project-URL: Bug Tracker, https://github.com/hamolicious/Reddit-Photo-Aggregator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `reddit_photo_aggregator-1.0.1/pyproject.toml` & `reddit_photo_aggregator-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "reddit_photo_aggregator"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="hamolicious", email="hamolicious@outlook.com" },
 ]
 description = "A library to scrape subreddits for images"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
@@ -18,9 +18,10 @@
 "Bug Tracker" = "https://github.com/hamolicious/Reddit-Photo-Aggregator/issues"
 
 [build-system]
 requires = [
 	"setuptools>=61.0",
 	"beautifulsoup4==4.12.2",
 	"requests==2.31.0",
+	"bs4==0.0.1"
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/image.py` & `reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/image.py`

 * *Files identical despite different names*

### Comparing `reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/image_validator.py` & `reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/image_validator.py`

 * *Files identical despite different names*

### Comparing `reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/subreddit.py` & `reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/subreddit.py`

 * *Files identical despite different names*

### Comparing `reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator/user_agent.py` & `reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator/user_agent.py`

 * *Files identical despite different names*

### Comparing `reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator.egg-info/PKG-INFO` & `reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-photo-aggregator
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library to scrape subreddits for images
 Author-email: hamolicious <hamolicious@outlook.com>
 Project-URL: Homepage, https://github.com/hamolicious/Reddit-Photo-Aggregator
 Project-URL: Bug Tracker, https://github.com/hamolicious/Reddit-Photo-Aggregator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `reddit_photo_aggregator-1.0.1/src/reddit_photo_aggregator.egg-info/SOURCES.txt` & `reddit_photo_aggregator-1.0.2/src/reddit_photo_aggregator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

