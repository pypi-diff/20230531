# Comparing `tmp/duckduckgo_search-3.7.0.tar.gz` & `tmp/duckduckgo_search-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.7.0.tar", last modified: Tue May 30 13:50:51 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.7.1.tar", last modified: Wed May 31 06:45:29 2023, max compression
```

## Comparing `duckduckgo_search-3.7.0.tar` & `duckduckgo_search-3.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13701 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    32023 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13701 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32114 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 06:45:29.000000 duckduckgo_search-3.7.1/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:45:29.504399 duckduckgo_search-3.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-31 06:45:12.000000 duckduckgo_search-3.7.1/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.7.0/LICENSE.md` & `duckduckgo_search-3.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.0/PKG-INFO` & `duckduckgo_search-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.7.0
+Version: 3.7.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.7.0/README.md` & `duckduckgo_search-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.0/duckduckgo_search/__init__.py` & `duckduckgo_search-3.7.1/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.0/duckduckgo_search/cli.py` & `duckduckgo_search-3.7.1/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.0/duckduckgo_search/compat.py` & `duckduckgo_search-3.7.1/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.7.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.7.1/duckduckgo_search/duckduckgo_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 
 logger = logging.getLogger(__name__)
 
 REGEX_500_IN_URL = re.compile(r"[0-9]{3}-[0-9]{2}.js")
 REGEX_STRIP_TAGS = re.compile("<.*?>")
 
 USERAGENTS = [
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
-    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
     "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0",
     "Mozilla/5.0 (Macintosh; Intel Mac OS X 13.4; rv:109.0) Gecko/20100101 Firefox/113.0",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13.4; rv:102.0) Gecko/20100101 Firefox/102.0",
     "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.5 Safari/605.1.15",
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.57",
-    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.57",
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/113.0.1774.57",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/113.0.1774.57",
     "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
     "Mozilla/5.0 (Windows NT 10.0; WOW64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
     "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
 ]
 HEADERS = {
     "User-Agent": choice(USERAGENTS),
     "Referer": "https://duckduckgo.com/",
```

### Comparing `duckduckgo_search-3.7.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.7.1/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.7.0
+Version: 3.7.1
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-3.7.0/pyproject.toml` & `duckduckgo_search-3.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.3",
     "lxml>=4.9.2",
-    "httpx[http2,socks]>=0.24.1",
+    "httpx[http2,socks,brotli]>=0.24.1",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
```

### Comparing `duckduckgo_search-3.7.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.7.1/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

