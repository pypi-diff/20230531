# Comparing `tmp/courlan-0.9.2.tar.gz` & `tmp/courlan-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "courlan-0.9.2.tar", last modified: Tue May  2 16:57:44 2023, max compression
+gzip compressed data, was "courlan-0.9.3.tar", last modified: Wed May 31 14:36:19 2023, max compression
```

## Comparing `courlan-0.9.2.tar` & `courlan-0.9.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1131 2020-08-31 17:20:52.000000 courlan-0.9.2/CONTRIBUTING.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2801 2023-05-02 16:57:40.000000 courlan-0.9.2/HISTORY.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    35141 2020-08-31 17:20:52.000000 courlan-0.9.2/LICENSE
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      160 2022-07-18 17:01:18.000000 courlan-0.9.2/MANIFEST.in
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    17701 2023-05-02 16:57:44.378929 courlan-0.9.2/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16025 2023-04-24 16:04:57.000000 courlan-0.9.2/README.rst
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/courlan/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      629 2023-05-02 16:57:40.000000 courlan-0.9.2/courlan/__init__.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     6212 2023-05-02 14:30:24.000000 courlan-0.9.2/courlan/clean.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3691 2022-07-27 15:47:45.000000 courlan-0.9.2/courlan/cli.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8447 2023-03-07 11:31:10.000000 courlan-0.9.2/courlan/core.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7320 2023-05-02 14:30:24.000000 courlan-0.9.2/courlan/filters.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7223 2023-03-07 12:06:22.000000 courlan-0.9.2/courlan/langinfo.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1665 2023-05-02 14:30:24.000000 courlan-0.9.2/courlan/network.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2022-07-18 15:53:08.000000 courlan-0.9.2/courlan/py.typed
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1786 2022-07-07 18:06:58.000000 courlan-0.9.2/courlan/settings.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16213 2023-05-02 14:30:24.000000 courlan-0.9.2/courlan/urlstore.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5794 2023-03-03 12:29:51.000000 courlan-0.9.2/courlan/urlutils.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/courlan.egg-info/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    17701 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      605 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/SOURCES.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/dependency_links.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       46 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/entry_points.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-03-07 12:17:45.000000 courlan-0.9.2/courlan.egg-info/not-zip-safe
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      128 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/requires.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        8 2023-05-02 16:57:44.000000 courlan-0.9.2/courlan.egg-info/top_level.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   151953 2020-08-31 17:20:52.000000 courlan-0.9.2/courlan_harns-march.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-12-07 18:31:00.000000 courlan-0.9.2/pytest.ini
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2023-05-02 16:57:44.378929 courlan-0.9.2/setup.cfg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3921 2023-05-02 14:30:24.000000 courlan-0.9.2/setup.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/tests/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2020-08-31 17:20:52.000000 courlan-0.9.2/tests/__init__.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-02 16:57:44.378929 courlan-0.9.2/tests/data/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      324 2021-12-07 18:52:06.000000 courlan-0.9.2/tests/data/input.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    34725 2023-05-02 14:30:24.000000 courlan-0.9.2/tests/unit_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    13036 2023-05-02 14:30:24.000000 courlan-0.9.2/tests/urlstore_tests.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-31 14:36:19.958463 courlan-0.9.3/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1131 2020-08-31 17:20:52.000000 courlan-0.9.3/CONTRIBUTING.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3159 2023-05-31 14:35:28.000000 courlan-0.9.3/HISTORY.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    35141 2020-08-31 17:20:52.000000 courlan-0.9.3/LICENSE
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      160 2022-07-18 17:01:18.000000 courlan-0.9.3/MANIFEST.in
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    18146 2023-05-31 14:36:19.958463 courlan-0.9.3/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16470 2023-05-31 14:35:28.000000 courlan-0.9.3/README.rst
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-31 14:36:19.954463 courlan-0.9.3/courlan/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      629 2023-05-31 14:35:28.000000 courlan-0.9.3/courlan/__init__.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     6201 2023-05-26 15:52:59.000000 courlan-0.9.3/courlan/clean.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5241 2023-05-31 14:35:28.000000 courlan-0.9.3/courlan/cli.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8313 2023-05-30 11:10:44.000000 courlan-0.9.3/courlan/core.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7340 2023-05-16 14:47:00.000000 courlan-0.9.3/courlan/filters.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7223 2023-03-07 12:06:22.000000 courlan-0.9.3/courlan/langinfo.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      360 2023-05-17 11:43:25.000000 courlan-0.9.3/courlan/meta.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1665 2023-05-15 09:53:28.000000 courlan-0.9.3/courlan/network.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2022-07-18 15:53:08.000000 courlan-0.9.3/courlan/py.typed
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1786 2022-07-07 18:06:58.000000 courlan-0.9.3/courlan/settings.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16449 2023-05-31 14:35:28.000000 courlan-0.9.3/courlan/urlstore.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     6037 2023-05-17 11:43:25.000000 courlan-0.9.3/courlan/urlutils.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-31 14:36:19.958463 courlan-0.9.3/courlan.egg-info/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    18146 2023-05-31 14:36:19.000000 courlan-0.9.3/courlan.egg-info/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      621 2023-05-31 14:36:19.000000 courlan-0.9.3/courlan.egg-info/SOURCES.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-05-31 14:36:19.000000 courlan-0.9.3/courlan.egg-info/dependency_links.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       46 2023-05-31 14:36:19.000000 courlan-0.9.3/courlan.egg-info/entry_points.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-05-31 14:36:19.000000 courlan-0.9.3/courlan.egg-info/not-zip-safe
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      128 2023-05-31 14:36:19.000000 courlan-0.9.3/courlan.egg-info/requires.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        8 2023-05-31 14:36:19.000000 courlan-0.9.3/courlan.egg-info/top_level.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   151953 2020-08-31 17:20:52.000000 courlan-0.9.3/courlan_harns-march.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-12-07 18:31:00.000000 courlan-0.9.3/pytest.ini
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2023-05-31 14:36:19.958463 courlan-0.9.3/setup.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3921 2023-05-15 09:53:28.000000 courlan-0.9.3/setup.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-31 14:36:19.958463 courlan-0.9.3/tests/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2020-08-31 17:20:52.000000 courlan-0.9.3/tests/__init__.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2023-05-31 14:36:19.958463 courlan-0.9.3/tests/data/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      324 2021-12-07 18:52:06.000000 courlan-0.9.3/tests/data/input.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    36941 2023-05-31 14:30:47.000000 courlan-0.9.3/tests/unit_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    13166 2023-05-31 14:35:28.000000 courlan-0.9.3/tests/urlstore_tests.py
```

### Comparing `courlan-0.9.2/CONTRIBUTING.md` & `courlan-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `courlan-0.9.2/HISTORY.md` & `courlan-0.9.3/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 ## History / Changelog
 
+### 0.9.3
+
+- more efficient URL parsing (#33)
+- refined link extraction and link filters (#30, #36)
+- more efficient normalization (#32)
+- more efficient sampling strategy (#31, #35)
+- added meta function to clear LRU caches (#34)
+- added parallel option in command-line interface (#37, #39)
+- added ``get_unvisited_domains()`` method to ``UrlStore`` (#40)
+
 
 ### 0.9.2
 
 - add blogspot archives to type filter
 - maintenance: upgrade ``urllib3`` and review code
```

### Comparing `courlan-0.9.2/LICENSE` & `courlan-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `courlan-0.9.2/PKG-INFO` & `courlan-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: courlan
-Version: 0.9.2
+Version: 0.9.3
 Summary: Clean, filter and sample URLs to optimize data collection – includes spam, content type and language filters.
 Home-page: https://github.com/adbar/courlan
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: GPLv3+
 Project-URL: Blog, https://adrien.barbaresi.eu/blog/
 Project-URL: Tracker, https://github.com/adbar/courlan/issues
@@ -278,14 +278,26 @@
     >>> from courlan import validate_url
     >>> validate_url('http://1234')
     (False, None)
     >>> validate_url('http://www.example.org/')
     (True, ParseResult(scheme='http', netloc='www.example.org', path='/', params='', query='', fragment=''))
 
 
+Troubleshooting
+~~~~~~~~~~~~~~~
+
+Courlan uses an internal cache to speed up URL parsing. It can be reset as follows:
+
+.. code-block:: python
+
+    >>> from courlan.meta import clear_caches
+    >>> clear_caches()
+
+
+
 UrlStore class
 ~~~~~~~~~~~~~~
 
 The ``UrlStore`` class allow for storing and retrieving domain-classified URLs, where a URL like ``https://example.org/path/testpage`` is stored as the path ``/path/testpage`` within the domain ``https://example.org``. It features the following methods:
 
 - URL management
    - ``add_urls(urls=[], appendleft=None, visited=False)``: Add a list of URLs to the (possibly) existing one. Optional: append certain URLs to the left, specify if the URLs have already been visited.
@@ -297,14 +309,15 @@
    - ``total_url_number()``: Find number of all URLs in store.
    - ``is_known(url)``: Check if the given URL has already been stored.
    - ``has_been_visited(url)``: Check if the given URL has already been visited.
    - ``filter_unknown_urls(urls)``: Take a list of URLs and return the currently unknown ones.
    - ``filter_unvisited_urls(urls)``: Take a list of URLs and return the currently unvisited ones.
    - ``find_known_urls(domain)``: Get all already known URLs for the given domain (ex. "https://example.org").
    - ``find_unvisited_urls(domain)``: Get all unvisited URLs for the given domain.
+   - ``get_unvisited_domains()``: Return all domains which have not been all visited.
    - ``reset()``: Re-initialize the URL store.
 - Crawling and downloads
    - ``get_url(domain)``: Retrieve a single URL and consider it to be visited (with corresponding timestamp).
    - ``get_rules(domain)``: Return the stored crawling rules for the given website.
    - ``get_crawl_delay()``: Return the delay as extracted from robots.txt, or a given default.
    - ``get_download_urls(timelimit=10)``: Get a list of immediately downloadable URLs according to the given time limit per domain.
    - ``establish_download_schedule(max_urls=100, time_limit=10)``: Get up to the specified number of URLs along with a suitable backoff schedule (in seconds).
@@ -343,14 +356,16 @@
   -i INPUTFILE, --inputfile INPUTFILE
                         name of input file (required)
   -o OUTPUTFILE, --outputfile OUTPUTFILE
                         name of output file (required)
   -d DISCARDEDFILE, --discardedfile DISCARDEDFILE
                         name of file to store discarded URLs (optional)
   -v, --verbose         increase output verbosity
+  -p PARALLEL, --parallel PARALLEL
+                        number of parallel processes (not used for sampling)
 
 Filtering:
   Configure URL filters
 
   --strict              perform more restrictive tests
   -l LANGUAGE, --language LANGUAGE
                         use language filter (ISO 639-1 code)
@@ -369,15 +384,15 @@
 
 
 License
 -------
 
 *coURLan* is distributed under the `GNU General Public License v3.0 <https://github.com/adbar/courlan/blob/master/LICENSE>`_. If you wish to redistribute this library but feel bounded by the license conditions please try interacting `at arms length <https://www.gnu.org/licenses/gpl-faq.html#GPLInProprietarySystem>`_, `multi-licensing <https://en.wikipedia.org/wiki/Multi-licensing>`_ with `compatible licenses <https://en.wikipedia.org/wiki/GNU_General_Public_License#Compatibility_and_multi-licensing>`_, or `contacting me <https://github.com/adbar/courlan#author>`_.
 
-See also `GPL and free software licensing: What's in it for business? <https://www.techrepublic.com/blog/cio-insights/gpl-and-free-software-licensing-whats-in-it-for-business/>`_
+See also `GPL and free software licensing: What's in it for business? <https://web.archive.org/web/20230127221311/https://www.techrepublic.com/article/gpl-and-free-software-licensing-whats-in-it-for-business/>`_
 
 
 
 Settings
 --------
 
 ``courlan`` is optimized for English and German but its generic approach is also usable in other contexts.
```

### Comparing `courlan-0.9.2/README.rst` & `courlan-0.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,26 @@
     >>> from courlan import validate_url
     >>> validate_url('http://1234')
     (False, None)
     >>> validate_url('http://www.example.org/')
     (True, ParseResult(scheme='http', netloc='www.example.org', path='/', params='', query='', fragment=''))
 
 
+Troubleshooting
+~~~~~~~~~~~~~~~
+
+Courlan uses an internal cache to speed up URL parsing. It can be reset as follows:
+
+.. code-block:: python
+
+    >>> from courlan.meta import clear_caches
+    >>> clear_caches()
+
+
+
 UrlStore class
 ~~~~~~~~~~~~~~
 
 The ``UrlStore`` class allow for storing and retrieving domain-classified URLs, where a URL like ``https://example.org/path/testpage`` is stored as the path ``/path/testpage`` within the domain ``https://example.org``. It features the following methods:
 
 - URL management
    - ``add_urls(urls=[], appendleft=None, visited=False)``: Add a list of URLs to the (possibly) existing one. Optional: append certain URLs to the left, specify if the URLs have already been visited.
@@ -260,14 +272,15 @@
    - ``total_url_number()``: Find number of all URLs in store.
    - ``is_known(url)``: Check if the given URL has already been stored.
    - ``has_been_visited(url)``: Check if the given URL has already been visited.
    - ``filter_unknown_urls(urls)``: Take a list of URLs and return the currently unknown ones.
    - ``filter_unvisited_urls(urls)``: Take a list of URLs and return the currently unvisited ones.
    - ``find_known_urls(domain)``: Get all already known URLs for the given domain (ex. "https://example.org").
    - ``find_unvisited_urls(domain)``: Get all unvisited URLs for the given domain.
+   - ``get_unvisited_domains()``: Return all domains which have not been all visited.
    - ``reset()``: Re-initialize the URL store.
 - Crawling and downloads
    - ``get_url(domain)``: Retrieve a single URL and consider it to be visited (with corresponding timestamp).
    - ``get_rules(domain)``: Return the stored crawling rules for the given website.
    - ``get_crawl_delay()``: Return the delay as extracted from robots.txt, or a given default.
    - ``get_download_urls(timelimit=10)``: Get a list of immediately downloadable URLs according to the given time limit per domain.
    - ``establish_download_schedule(max_urls=100, time_limit=10)``: Get up to the specified number of URLs along with a suitable backoff schedule (in seconds).
@@ -306,14 +319,16 @@
   -i INPUTFILE, --inputfile INPUTFILE
                         name of input file (required)
   -o OUTPUTFILE, --outputfile OUTPUTFILE
                         name of output file (required)
   -d DISCARDEDFILE, --discardedfile DISCARDEDFILE
                         name of file to store discarded URLs (optional)
   -v, --verbose         increase output verbosity
+  -p PARALLEL, --parallel PARALLEL
+                        number of parallel processes (not used for sampling)
 
 Filtering:
   Configure URL filters
 
   --strict              perform more restrictive tests
   -l LANGUAGE, --language LANGUAGE
                         use language filter (ISO 639-1 code)
@@ -332,15 +347,15 @@
 
 
 License
 -------
 
 *coURLan* is distributed under the `GNU General Public License v3.0 <https://github.com/adbar/courlan/blob/master/LICENSE>`_. If you wish to redistribute this library but feel bounded by the license conditions please try interacting `at arms length <https://www.gnu.org/licenses/gpl-faq.html#GPLInProprietarySystem>`_, `multi-licensing <https://en.wikipedia.org/wiki/Multi-licensing>`_ with `compatible licenses <https://en.wikipedia.org/wiki/GNU_General_Public_License#Compatibility_and_multi-licensing>`_, or `contacting me <https://github.com/adbar/courlan#author>`_.
 
-See also `GPL and free software licensing: What's in it for business? <https://www.techrepublic.com/blog/cio-insights/gpl-and-free-software-licensing-whats-in-it-for-business/>`_
+See also `GPL and free software licensing: What's in it for business? <https://web.archive.org/web/20230127221311/https://www.techrepublic.com/article/gpl-and-free-software-licensing-whats-in-it-for-business/>`_
 
 
 
 Settings
 --------
 
 ``courlan`` is optimized for English and German but its generic approach is also usable in other contexts.
```

### Comparing `courlan-0.9.2/courlan/__init__.py` & `courlan-0.9.3/courlan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # meta
 __title__ = "courlan"
 __author__ = "Adrien Barbaresi"
 __license__ = "GNU GPL v3+"
 __copyright__ = "Copyright 2020-2023, Adrien Barbaresi"
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 
 # imports
 from .clean import clean_url, normalize_url, scrub_url
 from .core import check_url, extract_links, sample_urls
 from .filters import is_navigation_page, is_not_crawlable, lang_filter, validate_url
 from .urlstore import UrlStore
```

### Comparing `courlan-0.9.2/courlan/clean.py` & `courlan-0.9.3/courlan/clean.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## This file is available from https://github.com/adbar/courlan
 ## under GNU GPL v3 license
 
 import logging
 import re
 
 from typing import Optional, Union
-from urllib.parse import parse_qs, urlencode, ParseResult
+from urllib.parse import parse_qs, urlencode, urlunsplit, ParseResult
 
 from .filters import validate_url
 from .settings import ALLOWED_PARAMS, CONTROL_PARAMS, TARGET_LANG_DE, TARGET_LANG_EN
 from .urlutils import _parse
 
 
 LOGGER = logging.getLogger(__name__)
@@ -27,15 +27,15 @@
 NETLOC_RE = re.compile(r"(?<=\w):(?:80|443)")
 
 # path
 PATH1 = re.compile(r"/+")
 PATH2 = re.compile(r"^(?:/\.\.(?![^/]))+")
 
 # scrub
-LINK_TAG = re.compile(r"</?a>")
+REMAINING_MARKUP = re.compile(r"</?[a-z]{,4}?>|{.+?}")
 TRAILING_AMP = re.compile(r"/\&$")
 TRAILING_PARTS = re.compile(r'(.*?)[<>"\'\s]')
 
 
 def clean_url(url: str, language: Optional[str] = None) -> Optional[str]:
     """Helper function: chained scrubbing and normalization"""
     try:
@@ -56,15 +56,15 @@
     # clean the input string
     url = url.replace("[ \t]+", "")
     # <![CDATA[http://www.urbanlife.de/item/260-bmw-i8-hybrid-revolution-unter-den-sportwagen.html]]>
     if url.startswith("<![CDATA["):
         url = url.replace("<![CDATA[", "")  # url = re.sub(r'^<!\[CDATA\[', '', url)
         url = url.replace("]]>", "")  # url = re.sub(r'\]\]>$', '', url)
     # markup rests
-    url = LINK_TAG.sub("", url)
+    url = REMAINING_MARKUP.sub("", url)
     # & and &amp;
     if "&amp;" in url:
         url = url.replace("&amp;", "&")
     url = TRAILING_AMP.sub("", url)
     # if '"' in link:
     #    link = link.split('"')[0]
     # double/faulty URLs
@@ -78,18 +78,18 @@
         else:
             match = MIDDLE_URL.match(url)
             if match and validate_url(match[1])[0] is True:
                 url = match[1]
                 LOGGER.debug("taking url: %s", url)
     # too long and garbled URLs e.g. due to quotes URLs
     # https://github.com/cocrawler/cocrawler/blob/main/cocrawler/urls.py
-    if len(url) > 500:  # arbitrary choice
-        match = TRAILING_PARTS.match(url)
-        if match:
-            url = match[1]
+    # if len(url) > 500:  # arbitrary choice
+    match = TRAILING_PARTS.match(url)
+    if match:
+        url = match[1]
     if len(url) > 500:
         LOGGER.debug("invalid-looking link %s of length %d", url[:50] + "…", len(url))
 
     # trailing slashes in URLs without path or in embedded URLs
     if url.count("/") == 3 or url.count("://") > 1:
         url = url.rstrip("/")
     # lower
@@ -150,31 +150,27 @@
 def normalize_url(
     parsed_url: Union[ParseResult, str],
     strict: bool = False,
     language: Optional[str] = None,
 ) -> str:
     """Takes a URL string or a parsed URL and returns a (basically) normalized URL string"""
     parsed_url = _parse(parsed_url)
+    # lowercase + remove fragments + normalize punycode
+    scheme = parsed_url.scheme.lower()
     # port
     if parsed_url.port and parsed_url.port in (80, 443):
         netloc = NETLOC_RE.sub("", parsed_url.netloc)
     else:
         netloc = parsed_url.netloc
     # lowercase + remove fragments + normalize punycode
     netloc = decode_punycode(netloc.lower())
     # path: https://github.com/saintamh/alcazar/blob/master/alcazar/utils/urls.py
-    newpath = PATH1.sub("/", parsed_url.path)
-    # Leading /../'s in the path are removed
-    newpath = PATH2.sub("", newpath)
+    # leading /../'s in the path are removed
+    newpath = PATH2.sub("", PATH1.sub("/", parsed_url.path))
+    # strip unwanted query elements
+    newquery = clean_query(parsed_url, strict, language) or ""
+    if newquery and newpath == "":
+        newpath = "/"
     # fragment
     newfragment = "" if strict else parsed_url.fragment
-    # lowercase + remove fragments + normalize punycode
-    parsed_url = parsed_url._replace(
-        scheme=parsed_url.scheme.lower(),
-        netloc=netloc,
-        path=newpath,
-        fragment=newfragment,
-        # strip unwanted query elements
-        query=clean_query(parsed_url, strict, language),
-    )
     # rebuild
-    return parsed_url.geturl()
+    return urlunsplit([scheme, netloc, newpath, newquery, newfragment])
```

### Comparing `courlan-0.9.2/courlan/cli.py` & `courlan-0.9.3/courlan/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 ## This file is available from https://github.com/adbar/courlan
 ## under GNU GPL v3 license
 
 import argparse
 import sys
 
-from typing import Any, List
+from concurrent.futures import ProcessPoolExecutor, as_completed
+from itertools import islice
+from typing import Any, Iterator, List, Optional, Tuple
 
 from .core import check_url, sample_urls
 
 
 def parse_args(args: Any) -> Any:
     """Define parser for command-line arguments"""
     argsparser = argparse.ArgumentParser(
@@ -38,14 +40,21 @@
         "--discardedfile",
         help="name of file to store discarded URLs (optional)",
         type=str,
     )
     group1.add_argument(
         "-v", "--verbose", help="increase output verbosity", action="store_true"
     )
+    group1.add_argument(
+        "-p",
+        "--parallel",
+        help="number of parallel processes (not used for sampling)",
+        type=int,
+        default=4,
+    )
     group2 = argsparser.add_argument_group("Filtering", "Configure URL filters")
     group2.add_argument(
         "--strict", help="perform more restrictive tests", action="store_true"
     )
     group2.add_argument(
         "-l", "--language", help="use language filter (ISO 639-1 code)", type=str
     )
@@ -64,33 +73,74 @@
     )  # default=10000
     group3.add_argument(
         "--exclude-min", help="exclude domains with less than n URLs", type=int
     )
     return argsparser.parse_args()
 
 
+def _cli_check_urls(
+    urls: List[str],
+    strict: bool = False,
+    with_redirects: bool = False,
+    language: Optional[str] = None,
+    with_nav: bool = False,
+) -> List[Tuple[bool, str]]:
+    "Internal function to be used with CLI multiprocessing."
+    results = []
+    for url in urls:
+        result = check_url(
+            url,
+            strict=strict,
+            with_redirects=with_redirects,
+            language=language,
+            with_nav=with_nav,
+        )
+        if result is not None:
+            results.append((True, result[0]))
+        else:
+            results.append((False, url))
+    return results
+
+
+def _get_line_batches(filename: str, size: int = 1000) -> Iterator[List[str]]:
+    "Iterate over a file and returns series of line batches."
+    with open(filename, "r", encoding="utf-8", errors="ignore") as inputfh:
+        while True:
+            line_batch = list(islice(inputfh, size))
+            if not line_batch:
+                break
+            yield line_batch
+
+
 def process_args(args: Any) -> None:
     """Start processing according to the arguments"""
     if not args.sample:
-        with open(
-            args.inputfile, "r", encoding="utf-8", errors="ignore"
-        ) as inputfh, open(args.outputfile, "w", encoding="utf-8") as outputfh:
-            for line in inputfh:
-                result = check_url(
-                    line,
+        with ProcessPoolExecutor(max_workers=args.parallel) as executor, open(
+            args.outputfile, "w", encoding="utf-8"
+        ) as outputfh:
+            futures = (
+                executor.submit(
+                    _cli_check_urls,
+                    batch,
                     strict=args.strict,
                     with_redirects=args.redirects,
                     language=args.language,
                 )
-                if result is not None:
-                    outputfh.write(result[0] + "\n")
-                # proceed with discarded URLs. to be rewritten
-                elif args.discardedfile is not None:
-                    with open(args.discardedfile, "a", encoding="utf-8") as discardfh:
-                        discardfh.write(line)
+                for batch in _get_line_batches(args.inputfile)
+            )
+            for future in as_completed(futures):
+                for valid, url in future.result():
+                    if valid:
+                        outputfh.write(url + "\n")
+                    # proceed with discarded URLs. to be rewritten
+                    elif args.discardedfile is not None:
+                        with open(
+                            args.discardedfile, "a", encoding="utf-8"
+                        ) as discardfh:
+                            discardfh.write(url)
     else:
         urllist: List[str] = []
         with open(args.inputfile, "r", encoding="utf-8", errors="ignore") as inputfh:
             urllist.extend(line.strip() for line in inputfh)
         with open(args.outputfile, "w", encoding="utf-8") as outputfh:
             for url in sample_urls(
                 urllist,
```

### Comparing `courlan-0.9.2/courlan/core.py` & `courlan-0.9.3/courlan/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -128,47 +128,45 @@
 ) -> List[str]:
     """Sample a list of URLs by domain name, optionally using constraints on their number"""
     # logging
     if verbose:
         LOGGER.setLevel(logging.DEBUG)
     else:
         LOGGER.setLevel(logging.ERROR)
-    # deduplicate
-    input_urls = list(dict.fromkeys(input_urls))
-    # validate
-    input_urls = [
-        u
-        for u in input_urls
-        if check_url(u, strict=strict, with_redirects=False) is not None
-    ]
     # store
     output_urls = []
-    urlstore = UrlStore(compressed=False, language=None, strict=strict)
-    urlstore.add_urls(input_urls)
+    use_compression = len(input_urls) > 10**6
+    urlstore = UrlStore(
+        compressed=use_compression, language=None, strict=strict, verbose=verbose
+    )
+    urlstore.add_urls(sorted(input_urls))
     # iterate
     for domain in urlstore.urldict:  # key=cmp_to_key(locale.strcoll)
-        urlpaths = [p.urlpath for p in urlstore._load_urls(domain)]
+        urlpaths = [
+            p.urlpath
+            for p in urlstore._load_urls(domain)
+            if p.urlpath not in ("/", None)
+        ]
         # too few or too many URLs
         if (
-            exclude_min is not None
+            not urlpaths
+            or exclude_min is not None
             and len(urlpaths) < exclude_min
             or exclude_max is not None
             and len(urlpaths) > exclude_max
         ):
-            LOGGER.info("discarded (size): %s\t\turls: %s", domain, len(urlpaths))
-            continue
-        # copy all URLs
-        if len(urlpaths) <= samplesize:
-            output_urls.extend([domain + p for p in urlpaths])
-            LOGGER.info("%s\t\turls: %s", domain, len(urlpaths))
+            LOGGER.warning("discarded (size): %s\t\turls: %s", domain, len(urlpaths))
             continue
         # sample
-        mysample = sorted(sample(urlpaths, k=samplesize))
+        if len(urlpaths) > samplesize:
+            mysample = sorted(sample(urlpaths, k=samplesize))
+        else:
+            mysample = urlpaths
         output_urls.extend([domain + p for p in mysample])
-        LOGGER.info(
+        LOGGER.debug(
             "%s\t\turls: %s\tprop.: %s",
             domain,
             len(mysample),
             len(mysample) / len(urlpaths),
         )
     # return gathered URLs
     return output_urls
@@ -201,23 +199,22 @@
     Returns:
         A set containing filtered HTTP links checked for sanity and consistency.
 
     Raises:
         Nothing.
     """
     candidates, validlinks = set(), set()  # type: Set[str], Set[str]
-    if pagecontent is None or not pagecontent:
+    if not pagecontent:
         return validlinks
     # define host reference
-    if reference is None:
-        reference = base_url
+    reference = reference or base_url
     # extract links
-    for match in FIND_LINKS_REGEX.finditer(pagecontent):
-        # filters
-        link = match[0]
+    for link in (m[0] for m in FIND_LINKS_REGEX.finditer(pagecontent)):
+        if "rel" in link and "nofollow" in link:
+            continue
         # https://en.wikipedia.org/wiki/Hreflang
         if no_filter is False and language is not None and "hreflang" in link:
             langmatch = HREFLANG_REGEX.search(link)
             if langmatch and (
                 langmatch[1].startswith(language) or langmatch[1] == "x-default"
             ):
                 linkmatch = LINK_REGEX.search(link)
```

### Comparing `courlan-0.9.2/courlan/filters.py` & `courlan-0.9.3/courlan/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,45 +17,51 @@
 from .langinfo import COUNTRY_CODES, LANGUAGE_CODES
 
 
 LOGGER = logging.getLogger(__name__)
 
 # content filters
 SITE_STRUCTURE = re.compile(
-    r"/(?:page|seite|user|search|gallery|gall?erie|labels|archives|uploads|modules|attachment)/|/(?:tags?|schlagwort|category|cat|kategorie|kat|auth?or)/[^/]+/?$|/[0-9]+/[0-9]+/$|/[0-9]{4}/$|_archive\.html$",
+    # wordpress
+    r"/(?:paged?|seite|search|suche|gall?er[a-z]{1,2}|labels|archives|uploads|modules|attachment|wp-admin|wp-content|wp-includes|wp-json|wp-themes|oembed)/|"
+    # wordpress + short URL
+    r"[/_-](?:tags?|schlagwort|[ck]ategor[a-z]{1,2}|[ck]at|auth?or|user)/[^/]+/?$|"
+    # mixed/blogspot
+    r"[^0-9]/[0-9]+/[0-9]+/$|[^0-9]/[0-9]{4}/$|"
+    # blogspot
+    r"_archive\.html$",
     re.IGNORECASE,
 )
 FILE_TYPE = re.compile(
-    r"\.(atom|json|css|xml|js|jpg|jpeg|png|gif|tiff|pdf|ogg|mp3|m4a|aac|avi|mp4|mov|webm|flv|ico|pls|zip|tar|gz|iso|swf)\b",
+    r"\.(atom|json|css|xml|js|jpg|jpeg|png|gif|tiff|pdf|ogg|mp3|m4a|aac|avi|mp4|mov|webm|flv|ico|pls|zip|tar|gz|iso|swf)\b|"
+    r"[/-](img|jpg|png)(\b|_)",
     re.IGNORECASE,
 )  # (?=[&?])
-UNDESIRABLE = re.compile(
-    r"\b(?:add?s?|banner|doubleclick|livestream|tradedoubler)\b|/oembed\b"
-)
 ADULT_AND_VIDEOS = re.compile(
-    r"\b(?:live|videos?|adult|amateur|arsch|cams?|cash|fick|gangbang|incest|porn|sexyeroti[ck]|sexcam|swinger|xxx|bild\-?kontakte)\b",
+    r"[/_-](?:bild\-?kontakte|fick|gangbang|incest|live-?chat|live-?cams?|porno?|sexyeroti[ck]|sexcam|swinger|xxx)\b",
     re.IGNORECASE,
-)  # ass|orgasm ?
+)
 
 # language filter
 PATH_LANG_FILTER = re.compile(
     r"(?:https?://[^/]+/)([a-z]{2})([_-][a-z]{2,3})?(?:/)", re.IGNORECASE
 )
 ALL_PATH_LANGS = re.compile(r"(?:/)([a-z]{2})([_-][a-z]{2})?(?:/)", re.IGNORECASE)
 HOST_LANG_FILTER = re.compile(
     r"https?://([a-z]{2})\.(?:[^.]{4,})\.(?:[^.]+)(?:\.[^.]+)?/", re.IGNORECASE
 )
 
 # navigation/crawls
 NAVIGATION_FILTER = re.compile(
-    r"/(archives|auth?or|[ck]at|category|kategorie|page|schlagwort|seite|tags?|topics?|user)/|\?p=[0-9]+",
+    r"[/_-](archives|auth?or|[ck]at|category|kategorie|paged?|schlagwort|seite|tags?|topics?|user)/|\?p=[0-9]+",
     re.IGNORECASE,
 )
 NOTCRAWLABLE = re.compile(
-    r"/(login|impressum|imprint)(\.[a-z]{3,4})?/?$|/login\?|/(javascript:|mailto:|tel\.?:|whatsapp:)",
+    r"/([ck]onta[ck]t|datenschutzerkl.{1,2}rung|login|impressum|imprint)(\.[a-z]{3,4})?/?$|/login\?|"
+    r"/(javascript:|mailto:|tel\.?:|whatsapp:)",
     re.IGNORECASE,
 )
 # |/(www\.)?(facebook\.com|google\.com|instagram\.com|twitter\.com)/
 INDEX_PAGE_FILTER = re.compile(
     r".{0,5}/(default|home|index)(\.[a-z]{3,5})?/?$", re.IGNORECASE
 )
 
@@ -174,21 +180,18 @@
 def type_filter(url: str, strict: bool = False, with_nav: bool = False) -> bool:
     """Make sure the target URL is from a suitable type (HTML page with primarily text).
     Strict: Try to filter out other document types, spam, video and adult websites."""
     try:
         # feeds
         if url.endswith(("/feed", "/rss")):
             raise ValueError
-        # wordpress website structure
+        # website structure
         if SITE_STRUCTURE.search(url) and (not with_nav or not is_navigation_page(url)):
             raise ValueError
-        # not suitable: ads, adult and embedded content
-        if UNDESIRABLE.search(url):
-            raise ValueError
-        # type hidden in parameters + video content
+        # type (also hidden in parameters), videos, adult content
         if strict and (FILE_TYPE.search(url) or ADULT_AND_VIDEOS.search(url)):
             raise ValueError
     except ValueError:
         return False
     # default
     return True
```

### Comparing `courlan-0.9.2/courlan/langinfo.py` & `courlan-0.9.3/courlan/langinfo.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.2/courlan/network.py` & `courlan-0.9.3/courlan/network.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.2/courlan/settings.py` & `courlan-0.9.3/courlan/settings.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.2/courlan/urlstore.py` & `courlan-0.9.3/courlan/urlstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Tuple,
     Union,
 )
 
 from urllib.robotparser import RobotFileParser
 
 from .filters import lang_filter, validate_url
+from .meta import clear_caches
 from .urlutils import get_host_and_path, is_known_link
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class DomainEntry:
@@ -85,22 +86,23 @@
             signal.signal(signal.SIGINT, dump_unvisited_urls)
             signal.signal(signal.SIGTERM, dump_unvisited_urls)
 
     def reset(self) -> None:
         "Re-initialize the URL store."
         with self._lock:
             self.urldict = defaultdict(DomainEntry)
+            clear_caches()
             num = gc.collect()
             LOGGER.debug("UrlStore reset, %s objects in GC", num)
 
     def _buffer_urls(
         self, data: List[str], visited: bool = False
     ) -> DefaultDict[str, Deque[UrlPathTuple]]:
         inputdict: DefaultDict[str, Deque[UrlPathTuple]] = defaultdict(deque)
-        for url in list(dict.fromkeys(data)):
+        for url in dict.fromkeys(data):
             # segment URL and add to domain dictionary
             try:
                 # validate
                 validation_result, parsed_url = validate_url(url)
                 if validation_result is False:
                     LOGGER.debug("Invalid URL: %s", url)
                     raise ValueError
@@ -229,24 +231,30 @@
         """Get all already known URLs for the given domain (ex. "https://example.org")."""
         return [domain + u.urlpath for u in self._load_urls(domain)]
 
     def filter_unknown_urls(self, urls: List[str]) -> List[str]:
         "Take a list of URLs and return the currently unknown ones."
         return self._search_urls(urls, switch=1)
 
+    # DOMAINS / HOSTNAMES
+
     def get_known_domains(self) -> List[str]:
         "Return all known domains as a list."
         return list(self.urldict)
 
     def is_exhausted_domain(self, domain: str) -> bool:
         "Tell if all known URLs for the website have been visited."
         if domain in self.urldict:
             return self.urldict[domain].all_visited
         raise KeyError("website not in store")
 
+    def get_unvisited_domains(self) -> List[str]:
+        "Return all domains which have not been all visited."
+        return [d for d in self.urldict if not self.urldict[d].all_visited]
+
     # URL-BASED QUERIES
 
     def has_been_visited(self, url: str) -> bool:
         "Check if the given URL has already been visited.."
         hostinfo, urlpath = get_host_and_path(url)
         known_urlpaths = {u.urlpath: u.visited for u in self._load_urls(hostinfo)}
         # defaults to None, thus False
@@ -258,15 +266,15 @@
 
     def filter_unvisited_urls(self, urls: List[str]) -> List[Union[Any, str]]:
         "Take a list of URLs and return the currently unvisited ones."
         return self._search_urls(urls, switch=2)
 
     def unvisited_websites_number(self) -> int:
         "Return the number of websites for which there are still URLs to visit."
-        return len([d for d in self.urldict if not self.urldict[d].all_visited])
+        return len(self.get_unvisited_domains())
 
     # DOWNLOADS
 
     def get_url(self, domain: str, as_visited: bool = True) -> Optional[str]:
         "Retrieve a single URL and consider it to be visited (with corresponding timestamp)."
         # not fully used
         if not self.urldict[domain].all_visited:
```

### Comparing `courlan-0.9.2/courlan/urlutils.py` & `courlan-0.9.3/courlan/urlutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Functions related to URL manipulation and extraction of URL parts.
 """
 
 import re
 
 from functools import lru_cache
 from typing import Any, List, Optional, Set, Tuple, Union
-from urllib.parse import urlparse, ParseResult
+from urllib.parse import urlparse, urlunsplit, ParseResult
 
 from tld import get_tld
 
 
 DOMAIN_REGEX = re.compile(
     r"(?:http|ftp)s?://"  # protocols
     r"(?:[^/?#]{,63}\.)?"  # subdomain, www, etc.
@@ -18,14 +18,16 @@
     r"[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}|"  # IPv4
     r"[0-9a-f:]{16,})"  # IPv6
     r"(?:/|$)"  # slash or end of string
 )
 NO_EXTENSION_REGEX = re.compile(r"(^[^.]+)")
 STRIP_DOMAIN_REGEX = re.compile(r"^.+?:.*?@|(?<=[^0-9]):[0-9]+")
 CLEAN_FLD_REGEX = re.compile(r"^www[0-9]*\.")
+INNER_SLASH_REGEX = re.compile(r"(.+/)+")
+FEED_WHITELIST_REGEX = re.compile(r"(feedburner|feedproxy)", re.I)
 
 
 @lru_cache(maxsize=1024)
 def get_tldinfo(
     url: str, fast: bool = False
 ) -> Union[Tuple[None, None], Tuple[str, str]]:
     """Cached function to extract top-level domain info"""
@@ -76,23 +78,29 @@
     return parsed_url
 
 
 def get_base_url(url: Any) -> str:
     """Strip URL of some of its parts to get base URL.
     Accepts strings and urllib.parse ParseResult objects."""
     parsed_url = _parse(url)
-    return parsed_url._replace(path="", params="", query="", fragment="").geturl()
+    if parsed_url.scheme:
+        scheme = parsed_url.scheme + "://"
+    else:
+        scheme = ""
+    return scheme + parsed_url.netloc
 
 
 def get_host_and_path(url: Any) -> Tuple[str, str]:
     """Decompose URL in two parts: protocol + host/domain and path.
     Accepts strings and urllib.parse ParseResult objects."""
     parsed_url = _parse(url)
     hostname = get_base_url(parsed_url)
-    pathval = parsed_url._replace(scheme="", netloc="").geturl()
+    pathval = urlunsplit(
+        ["", "", parsed_url.path, parsed_url.query, parsed_url.fragment]
+    )
     # correction for root/homepage
     if pathval == "":
         pathval = "/"
     if not hostname or not pathval:
         raise ValueError(f"incomplete URL: {url}")
     return hostname, pathval
 
@@ -109,36 +117,32 @@
     if url.startswith("//"):
         return "https:" + url if baseurl.startswith("https") else "http:" + url
     if url.startswith("/"):
         # imperfect path handling
         return baseurl + url
     if url.startswith("."):
         # don't try to correct these URLs
-        return baseurl + "/" + re.sub(r"(.+/)+", "", url)
-    if not url.startswith("http") and not url.startswith("{"):
+        return baseurl + "/" + INNER_SLASH_REGEX.sub("", url)
+    if not url.startswith(("http", "{")):
         return baseurl + "/" + url
     # todo: handle here
     # if url.startswith('{'):
     return url
 
 
-def filter_urls(linklist: List[str], urlfilter: Optional[str]) -> List[str]:
+def filter_urls(link_list: List[str], urlfilter: Optional[str]) -> List[str]:
     "Return a list of links corresponding to the given substring pattern."
     if urlfilter is None:
-        return sorted(set(linklist))
+        return sorted(set(link_list))
     # filter links
-    newlist = [l for l in linklist if urlfilter in l]
+    filtered_list = [l for l in link_list if urlfilter in l]
     # feedburner option: filter and wildcards for feeds
-    if not newlist:
-        newlist = [
-            l
-            for l in linklist
-            if urlfilter in l or "feedburner" in l or "feedproxy" in l
-        ]
-    return sorted(set(newlist))
+    if not filtered_list:
+        filtered_list = [l for l in link_list if FEED_WHITELIST_REGEX.search(l)]
+    return sorted(set(filtered_list))
 
 
 def is_external(url: str, reference: str, ignore_suffix: bool = True) -> bool:
     """Determine if a link leads to another host, takes a reference URL and
     a URL as input, returns a boolean"""
     stripped_ref, ref = get_tldinfo(reference, fast=True)
     stripped_domain, domain = get_tldinfo(url, fast=True)
@@ -146,24 +150,29 @@
     if ignore_suffix:
         return stripped_domain != stripped_ref
     return domain != ref
 
 
 def is_known_link(link: str, known_links: Set[str]) -> bool:
     "Compare the link and its possible variants to the existing URL base."
-    # easy check
+    # check exact link
     if link in known_links:
         return True
-    # trailing slash
-    test1 = link.rstrip("/")
-    test2 = test1 + "/"
-    if test1 in known_links or test2 in known_links:
+
+    # check link and variants with trailing slashes
+    test_links = [link.rstrip("/"), link.rstrip("/") + "/"]
+    if any(test_link in known_links for test_link in test_links):
         return True
-    # http/https + trailing slash
+
+    # check link and variants with modified protocol
     if link.startswith("http"):
         if link.startswith("https"):
             testlink = link[:4] + link[5:]
         else:
             testlink = "".join([link[:4], "s", link[4:]])
-        test1, test2 = testlink.rstrip("/"), testlink.rstrip("/") + "/"
-        return testlink in known_links or test1 in known_links or test2 in known_links
+        if any(
+            test in known_links
+            for test in [testlink, testlink.rstrip("/"), testlink.rstrip("/") + "/"]
+        ):
+            return True
+
     return False
```

### Comparing `courlan-0.9.2/courlan.egg-info/PKG-INFO` & `courlan-0.9.3/courlan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: courlan
-Version: 0.9.2
+Version: 0.9.3
 Summary: Clean, filter and sample URLs to optimize data collection – includes spam, content type and language filters.
 Home-page: https://github.com/adbar/courlan
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: GPLv3+
 Project-URL: Blog, https://adrien.barbaresi.eu/blog/
 Project-URL: Tracker, https://github.com/adbar/courlan/issues
@@ -278,14 +278,26 @@
     >>> from courlan import validate_url
     >>> validate_url('http://1234')
     (False, None)
     >>> validate_url('http://www.example.org/')
     (True, ParseResult(scheme='http', netloc='www.example.org', path='/', params='', query='', fragment=''))
 
 
+Troubleshooting
+~~~~~~~~~~~~~~~
+
+Courlan uses an internal cache to speed up URL parsing. It can be reset as follows:
+
+.. code-block:: python
+
+    >>> from courlan.meta import clear_caches
+    >>> clear_caches()
+
+
+
 UrlStore class
 ~~~~~~~~~~~~~~
 
 The ``UrlStore`` class allow for storing and retrieving domain-classified URLs, where a URL like ``https://example.org/path/testpage`` is stored as the path ``/path/testpage`` within the domain ``https://example.org``. It features the following methods:
 
 - URL management
    - ``add_urls(urls=[], appendleft=None, visited=False)``: Add a list of URLs to the (possibly) existing one. Optional: append certain URLs to the left, specify if the URLs have already been visited.
@@ -297,14 +309,15 @@
    - ``total_url_number()``: Find number of all URLs in store.
    - ``is_known(url)``: Check if the given URL has already been stored.
    - ``has_been_visited(url)``: Check if the given URL has already been visited.
    - ``filter_unknown_urls(urls)``: Take a list of URLs and return the currently unknown ones.
    - ``filter_unvisited_urls(urls)``: Take a list of URLs and return the currently unvisited ones.
    - ``find_known_urls(domain)``: Get all already known URLs for the given domain (ex. "https://example.org").
    - ``find_unvisited_urls(domain)``: Get all unvisited URLs for the given domain.
+   - ``get_unvisited_domains()``: Return all domains which have not been all visited.
    - ``reset()``: Re-initialize the URL store.
 - Crawling and downloads
    - ``get_url(domain)``: Retrieve a single URL and consider it to be visited (with corresponding timestamp).
    - ``get_rules(domain)``: Return the stored crawling rules for the given website.
    - ``get_crawl_delay()``: Return the delay as extracted from robots.txt, or a given default.
    - ``get_download_urls(timelimit=10)``: Get a list of immediately downloadable URLs according to the given time limit per domain.
    - ``establish_download_schedule(max_urls=100, time_limit=10)``: Get up to the specified number of URLs along with a suitable backoff schedule (in seconds).
@@ -343,14 +356,16 @@
   -i INPUTFILE, --inputfile INPUTFILE
                         name of input file (required)
   -o OUTPUTFILE, --outputfile OUTPUTFILE
                         name of output file (required)
   -d DISCARDEDFILE, --discardedfile DISCARDEDFILE
                         name of file to store discarded URLs (optional)
   -v, --verbose         increase output verbosity
+  -p PARALLEL, --parallel PARALLEL
+                        number of parallel processes (not used for sampling)
 
 Filtering:
   Configure URL filters
 
   --strict              perform more restrictive tests
   -l LANGUAGE, --language LANGUAGE
                         use language filter (ISO 639-1 code)
@@ -369,15 +384,15 @@
 
 
 License
 -------
 
 *coURLan* is distributed under the `GNU General Public License v3.0 <https://github.com/adbar/courlan/blob/master/LICENSE>`_. If you wish to redistribute this library but feel bounded by the license conditions please try interacting `at arms length <https://www.gnu.org/licenses/gpl-faq.html#GPLInProprietarySystem>`_, `multi-licensing <https://en.wikipedia.org/wiki/Multi-licensing>`_ with `compatible licenses <https://en.wikipedia.org/wiki/GNU_General_Public_License#Compatibility_and_multi-licensing>`_, or `contacting me <https://github.com/adbar/courlan#author>`_.
 
-See also `GPL and free software licensing: What's in it for business? <https://www.techrepublic.com/blog/cio-insights/gpl-and-free-software-licensing-whats-in-it-for-business/>`_
+See also `GPL and free software licensing: What's in it for business? <https://web.archive.org/web/20230127221311/https://www.techrepublic.com/article/gpl-and-free-software-licensing-whats-in-it-for-business/>`_
 
 
 
 Settings
 --------
 
 ``courlan`` is optimized for English and German but its generic approach is also usable in other contexts.
```

### Comparing `courlan-0.9.2/courlan.egg-info/SOURCES.txt` & `courlan-0.9.3/courlan.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 setup.py
 courlan/__init__.py
 courlan/clean.py
 courlan/cli.py
 courlan/core.py
 courlan/filters.py
 courlan/langinfo.py
+courlan/meta.py
 courlan/network.py
 courlan/py.typed
 courlan/settings.py
 courlan/urlstore.py
 courlan/urlutils.py
 courlan.egg-info/PKG-INFO
 courlan.egg-info/SOURCES.txt
```

### Comparing `courlan-0.9.2/courlan_harns-march.jpg` & `courlan-0.9.3/courlan_harns-march.jpg`

 * *Files identical despite different names*

### Comparing `courlan-0.9.2/setup.py` & `courlan-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `courlan-0.9.2/tests/unit_tests.py` & `courlan-0.9.3/tests/unit_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import subprocess
 import sys
 import tempfile
 
 from contextlib import redirect_stdout
 from unittest.mock import patch
-from urllib.parse import ParseResult
+from urllib.parse import ParseResult, urlsplit
 
 import pytest
 
 from courlan import cli
 from courlan import (
     clean_url,
     normalize_url,
@@ -35,15 +35,16 @@
     get_host_and_path,
     get_hostinfo,
     is_navigation_page,
     is_not_crawlable,
     lang_filter,
 )
 from courlan.filters import extension_filter, path_filter, type_filter
-from courlan.urlutils import _parse, is_known_link
+from courlan.meta import clear_caches
+from courlan.urlutils import _parse, get_tldinfo, is_known_link
 
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 RESOURCES_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), "data")
 
 
 def test_baseurls():
@@ -99,14 +100,19 @@
     )
 
 
 def test_scrub():
     # clean: scrub + normalize
     assert clean_url(5) is None
     assert clean_url("ø\xaa") == "øª"
+    assert clean_url("https://example.org/?p=100") == "https://example.org/?p=100"
+    assert (
+        clean_url("https://example.org:443/file.html?p=100&abc=1#frag")
+        == "https://example.org/file.html?abc=1&p=100#frag"
+    )
     # scrub
     assert scrub_url("  https://www.dwds.de") == "https://www.dwds.de"
     assert scrub_url("<![CDATA[https://www.dwds.de]]>") == "https://www.dwds.de"
     assert (
         scrub_url("https://www.dwds.de/test?param=test&amp;other=test")
         == "https://www.dwds.de/test?param=test&other=test"
     )
@@ -135,19 +141,21 @@
     )
     # end of URL
     assert scrub_url("https://www.test.com/&") == "https://www.test.com"
     # white space
     assert scrub_url("\x19https://www.test.com/\x06") == "https://www.test.com"
     # markup
     assert scrub_url("https://www.test.com/</a>") == "https://www.test.com"
+    assert scrub_url("https://www.test.com/1</div>") == "https://www.test.com/1"
+    assert scrub_url("https://www.test.com/{user_name}") == "https://www.test.com"
     # garbled URLs e.g. due to quotes
     assert (
         scrub_url('https://www.test.com/"' + "<p></p>" * 100) == "https://www.test.com"
     )
-    assert scrub_url('https://www.test.com/"' * 50) != "https://www.test.com"
+    assert scrub_url('https://www.test.com/"' * 50) == "https://www.test.com"
     # simply too long, left untouched
     my_url = "https://www.test.com/" + "abcdefg" * 100
     assert scrub_url(my_url) == my_url
 
 
 def test_extension_filter():
     validation_test, parsed_url = validate_url("http://www.example.org/test.js")
@@ -177,46 +185,51 @@
     validation_test, parsed_url = validate_url("http://www.example.org/test.php5")
     assert extension_filter(parsed_url.path) is True
     validation_test, parsed_url = validate_url("http://www.example.org/test.php6")
     assert extension_filter(parsed_url.path) is True
 
 
 def test_spam_filter():
-    assert type_filter("http://www.example.org/cams/test.html", strict=False) is True
-    assert type_filter("http://www.example.org/cams/test.html", strict=True) is False
+    assert (
+        type_filter("http://www.example.org/livecams/test.html", strict=False) is True
+    )
+    assert (
+        type_filter("http://www.example.org/livecams/test.html", strict=True) is False
+    )
     assert type_filter("http://www.example.org/test.html") is True
 
 
 def test_type_filter():
     assert type_filter("http://www.example.org/feed") is False
     # straight category
     assert type_filter("http://www.example.org/category/123") is False
+    assert type_filter("http://www.example.org/product-category/123") is False
     # post simply filed under a category
     assert type_filter("http://www.example.org/category/tropes/time-travel") is True
     assert (
         type_filter("http://www.example.org/test.xml?param=test", strict=True) is False
     )
     assert type_filter("http://www.example.org/test.asp") is True
-    assert type_filter("http://ads.example.org/") is False
     # -video- vs. /video/
-    assert type_filter("http://my-videos.com/") is True
-    assert type_filter("http://my-videos.com/", strict=True) is False
-    assert type_filter("http://example.com/video/1", strict=True) is False
-    assert type_filter("http://example.com/new-video-release") is True
-    assert type_filter("http://example.com/new-video-release", strict=True) is False
+    assert type_filter("http://my-livechat.com/") is True
+    assert type_filter("http://my-livechat.com/", strict=True) is False
+    assert type_filter("http://example.com/livechat/1", strict=True) is False
+    assert type_filter("http://example.com/new-sexcam") is True
+    assert type_filter("http://example.com/new-sexcam", strict=True) is False
     # tags
     assert type_filter("https://de.thecitizen.de/tag/anonymity/") is False
     assert type_filter("https://de.thecitizen.de/tags/anonymity/") is False
     # author
     assert type_filter("http://www.example.org/author/abcde") is False
     assert type_filter("http://www.example.org/autor/abcde/") is False
     # archives
     assert type_filter("http://www.example.org/2011/11/") is False
     assert type_filter("http://www.example.org/2011/") is False
     assert type_filter("http://www.example.org/2011_archive.html") is False
+    assert type_filter("http://www.example.org/2020/02/06/1859/") is True
     # misc
     assert (
         type_filter("http://www.bmbwk.gv.at/forschung/fps/gsk/befragung.xml?style=text")
         is True
     )
     assert (
         type_filter(
@@ -225,25 +238,35 @@
         is False
     )
     # nav
     assert type_filter("http://www.example.org/tag/abcde/", with_nav=False) is False
     assert type_filter("http://www.example.org/tag/abcde/", with_nav=True) is True
     assert type_filter("http://www.example.org/page/10/", with_nav=False) is False
     assert type_filter("http://www.example.org/page/10/", with_nav=True) is True
+    # img
+    assert type_filter("http://www.example.org/logo_800_web-jpg/", strict=True) is False
+    assert (
+        type_filter("http://www.example.org/img_2020-03-03_25/", strict=True) is False
+    )
 
 
 def test_path_filter():
     assert (
         check_url(
             "http://www.case-modder.de/index.php?sec=artikel&id=68&page=1", strict=True
         )
         is not None
     )
+    assert path_filter("/index.php", "") is False
     assert check_url("http://www.case-modder.de/index.php", strict=True) is None
+    assert path_filter("/default/", "") is False
     assert check_url("http://www.case-modder.de/default/", strict=True) is None
+    assert path_filter("/contact/", "") is False
+    assert path_filter("/Datenschutzerklaerung", "") is False
+    # assert path_filter("/", "") is False
 
 
 def test_lang_filter():
     assert (
         lang_filter(
             "https://www.20min.ch/fr/story/des-millions-pour-produire-de-l-energie-renouvelable-467974085377",
             None,
@@ -410,14 +433,18 @@
         == "http://test.net/foo.html"
     )
     assert (
         normalize_url("http://www.example.org:80/test.html")
         == "http://www.example.org/test.html"
     )
     assert (
+        normalize_url("http://www.example.org:80?p=123")
+        == "http://www.example.org/?p=123"
+    )
+    assert (
         normalize_url("https://hanxiao.io//404.html") == "https://hanxiao.io/404.html"
     )
     # punycode
     assert normalize_url("http://xn--Mnchen-3ya.de") == "http://münchen.de"
     assert normalize_url("http://Mnchen-3ya.de") == "http://mnchen-3ya.de"
     assert normalize_url("http://xn--München.de") == "http://xn--münchen.de"
 
@@ -474,20 +501,20 @@
         "https://httpbun.org",
         "httpbun.org",
     )
     # assert check_url('https://www.httpbin.org/status/302', with_redirects=True) == ('https://www.httpbin.org/status/302', 'httpbin.org')
     assert check_url("https://www.httpbin.org/status/404", with_redirects=True) is None
     assert check_url("https://www.ht.or", with_redirects=True) is None
     # recheck type and spam filters
-    assert check_url("http://example.org/code/oembed/") is None
-    assert check_url("http://cams.com/", strict=False) == (
-        "http://cams.com",
-        "cams.com",
+    assert check_url("http://example.org/wp-json/oembed/") is None
+    assert check_url("http://livecams.com/", strict=False) == (
+        "http://livecams.com",
+        "livecams.com",
     )
-    assert check_url("http://cams.com/", strict=True) is None
+    assert check_url("http://livecams.com/", strict=True) is None
     assert check_url("https://denkiterm.wordpress.com/impressum/", strict=True) is None
     assert (
         check_url(
             "http://www.fischfutter-index.de/improvit-trocken-frostfutter-fur-fast-alle-fische/",
             strict=True,
         )
         is not None
@@ -676,14 +703,17 @@
 def test_extraction():
     """test link comparison in HTML"""
     assert len(extract_links(None, "https://test.com/", False)) == 0
     assert len(extract_links("", "https://test.com/", False)) == 0
     # link known under another form
     pagecontent = '<html><a href="https://test.org/example"/><a href="https://test.org/example/&"/></html>'
     assert len(extract_links(pagecontent, "https://test.org", False)) == 1
+    # nofollow
+    pagecontent = '<html><a href="https://test.com/example" rel="nofollow ugc"/></html>'
+    assert len(extract_links(pagecontent, "https://test.com/", False)) == 0
     # language
     pagecontent = '<html><a href="https://test.com/example" hreflang="de-DE"/></html>'
     assert len(extract_links(pagecontent, "https://test.com/", False)) == 1
     assert len(extract_links(pagecontent, "https://test.com/", True)) == 0
     assert (
         len(extract_links(pagecontent, "https://test.com/", False, language="de")) == 1
     )
@@ -780,22 +810,22 @@
         '<html><a href="{privacy}" target="_privacy">{privacy-link}</a></html>'
     )
     assert (
         len(extract_links(pagecontent, "https://test.com/", external_bool=False)) == 0
     )
     assert len(extract_links(pagecontent, "https://test.com/", external_bool=True)) == 0
     # links without quotes
-    pagecontent = "<html><a href=/contact>Link</a></html>"
+    pagecontent = "<html><a href=/link>Link</a></html>"
     assert extract_links(pagecontent, "https://test.com/", external_bool=False) == {
-        "https://test.com/contact"
+        "https://test.com/link"
     }
     assert extract_links(pagecontent, "https://test.com/", external_bool=True) == set()
-    pagecontent = "<html><a href=/contact attribute=value>Link</a></html>"
+    pagecontent = "<html><a href=/link attribute=value>Link</a></html>"
     assert extract_links(pagecontent, "https://test.com/", external_bool=False) == {
-        "https://test.com/contact"
+        "https://test.com/link"
     }
     # external links with extension (here ".com")
     pagecontent = '<html><body><a href="https://knoema.com/o/data-engineer-india"/><a href="https://knoema.recruitee.com/"/></body></html>'
     assert extract_links(pagecontent, "https://knoema.com/", external_bool=False) == {
         "https://knoema.com/o/data-engineer-india"
     }
     assert extract_links(pagecontent, "https://knoema.com/", external_bool=True) == {
@@ -822,38 +852,47 @@
         "-d",
         "discardedfile.txt",
         "--outputfile",
         "output.txt",
         "-v",
         "--language",
         "en",
+        "--parallel",
+        "2",
     ]
     with patch.object(sys, "argv", testargs):
         args = cli.parse_args(testargs)
     assert args.inputfile == "input.txt"
     assert args.discardedfile == "discardedfile.txt"
     assert args.outputfile == "output.txt"
     assert args.verbose is True
     assert args.language == "en"
+    assert args.parallel == 2
     assert os.system("courlan --help") == 0  # exit status
 
+    # _cli_check_urls
+    assert cli._cli_check_urls(["123", "https://example.org"]) == [
+        (False, "123"),
+        (True, "https://example.org"),
+    ]
+
     # testfile
     inputfile = os.path.join(RESOURCES_DIR, "input.txt")
     os_handle, temp_outputfile = tempfile.mkstemp(suffix=".txt", text=True)
     env = os.environ.copy()
     # Force encoding to utf-8 for Windows (seem to be a problem only in GitHub Actions)
     if os.name == "nt":
         env["PYTHONIOENCODING"] = "utf-8"
         courlan_bin = os.path.join(sys.prefix, "Scripts", "courlan")
     else:
         courlan_bin = "courlan"
     # test for Windows and the rest
     assert (
         subprocess.run(
-            [courlan_bin, "-i", inputfile, "-o", temp_outputfile], env=env
+            [courlan_bin, "-i", inputfile, "-o", temp_outputfile, "-p", "1"], env=env
         ).returncode
         == 0
     )
 
     # tests without Windows
     if os.name != "nt":
         # dry runs (writes to /tmp/)
@@ -864,14 +903,16 @@
             "-d",
             "/tmp/tralala1.txt",
             "-o",
             temp_outputfile,
             "--language",
             "en",
             "--strict",
+            "-p",
+            "1",
         ]
         f = io.StringIO()
         with patch.object(sys, "argv", testargs):
             args = cli.parse_args(testargs)
         with redirect_stdout(f):
             cli.process_args(args)
         assert len(f.getvalue()) == 0
@@ -887,14 +928,15 @@
     except PermissionError:
         print("couldn't delete temp file")
 
 
 def test_sample():
     """test URL sampling"""
     assert not list(sample_urls(["http://test.org/test1", "http://test.org/test2"], 0))
+    assert not list(sample_urls(["http://test.org/", "http://test.org"], 10))
 
     # assert len(sample_urls(['http://test.org/test1', 'http://test.org/test2'], 1)) == 1
     mylist = [
         "http://t.o/t1",
         "http://test.org/test1",
         "http://test.org/test2",
         "http://test2.org/test2",
@@ -932,7 +974,24 @@
     assert (
         normalize_url(
             "http://test.net/foo.html?utm_source=twitter&post=abc&page=2#fragment",
             strict=True,
         )
         == "http://test.net/foo.html?page=2&post=abc"
     )
+
+
+def test_meta():
+    "Test package meta functions."
+    url = "https://example.net/123/abc"
+    _ = get_tldinfo(url)
+    _ = _parse(url)
+    assert get_tldinfo.cache_info().currsize > 0
+    try:
+        urlsplit_lrucache = True
+        assert urlsplit.cache_info().currsize > 0
+    except AttributeError:  # newer Python versions only
+        urlsplit_lrucache = False
+    clear_caches()
+    assert get_tldinfo.cache_info().currsize == 0
+    if urlsplit_lrucache:
+        assert urlsplit.cache_info().currsize == 0
```

### Comparing `courlan-0.9.2/tests/urlstore_tests.py` & `courlan-0.9.3/tests/urlstore_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import pickle
 import signal
 import sys
 import uuid
 
 from datetime import datetime
+from time import sleep
 
 import pytest
 
 from courlan import UrlStore
 
 
 def test_urlstore():
@@ -164,25 +165,26 @@
 
     # get_url
     assert my_urls.urldict[example_domain].timestamp is None
     assert my_urls.urldict[example_domain].count == 0
 
     url1 = my_urls.get_url(example_domain)
     timestamp = my_urls.urldict[example_domain].timestamp
+    sleep(0.1)
     url2 = my_urls.get_url(example_domain)
     assert url1 != url2 and url1 == "https://www.example.org/1/10/"
     assert my_urls.urldict[example_domain].count == 2
     assert timestamp != my_urls.urldict[example_domain].timestamp
     assert url2 not in set(my_urls.find_unvisited_urls(example_domain))
     assert my_urls.get_all_counts() == [2, 0, 0]
 
     # as_visited=False
     timestamp = my_urls.urldict[example_domain].timestamp
     url3 = my_urls.get_url(example_domain, as_visited=False)
-    assert url3 != url1 and url3 != url2
+    assert url3 not in (url1, url2)
     assert my_urls.urldict[example_domain].count == 2
     assert timestamp == my_urls.urldict[example_domain].timestamp
     assert url3 in set(my_urls.find_unvisited_urls(example_domain))
 
     url_tuples = my_urls._load_urls(example_domain)
     # positions
     assert url1.endswith(url_tuples[0].urlpath) and url2.endswith(url_tuples[1].urlpath)
@@ -220,15 +222,15 @@
     assert (
         url_tuples[0].visited is True
         and url_tuples[1].visited is True
         and url_tuples[2].visited is False
     )
     assert my_urls.has_been_visited("http://tovisit.com/page") is True
     assert my_urls.urldict["http://tovisit.com"].all_visited is True
-    assert my_urls.filter_unvisited_urls(["http://tovisit.com/page"]) == []
+    assert not my_urls.filter_unvisited_urls(["http://tovisit.com/page"])
     assert my_urls.filter_unvisited_urls(["http://tovisit.com/otherpage"]) == [
         "http://tovisit.com/otherpage"
     ]
     assert my_urls.has_been_visited("https://www.other.org/1") is False
     assert my_urls.has_been_visited(url1) is True
     assert my_urls.has_been_visited(f"{example_domain}/this") is False
     assert my_urls.has_been_visited(f"{example_domain}/999") is False
@@ -239,15 +241,18 @@
     ]
     assert (
         len(my_urls.find_known_urls(example_domain))
         == len(my_urls._load_urls(example_domain))
         == 10011
     )
     assert len(my_urls.find_unvisited_urls(example_domain)) == 10009
-    assert my_urls.unvisited_websites_number() == 4
+    assert (
+        my_urls.unvisited_websites_number() == len(my_urls.get_unvisited_domains()) == 4
+    )
+    assert my_urls.total_url_number() == 20013
 
     # get download URLs
     downloadable_urls = my_urls.get_download_urls(timelimit=0)
     assert (
         len(downloadable_urls) == 2
         and downloadable_urls[0] == "https://www.example.org/1"
     )
@@ -256,19 +261,19 @@
     ).total_seconds() < 0.25
     assert my_urls.urldict["https://www.example.org"].count == 3
     assert my_urls.urldict["https://test.org"].count == 1
     downloadable_urls = my_urls.get_download_urls()  # limit=10
     assert len(downloadable_urls) == 0
     other_store = UrlStore()
     downloadable_urls = other_store.get_download_urls()
-    assert downloadable_urls == [] and other_store.done is True
+    assert not downloadable_urls and other_store.done is True
 
     # schedule
     schedule = other_store.establish_download_schedule()
-    assert schedule == []
+    assert not schedule
     # store exhaustion
     other_store = UrlStore()
     other_store.add_urls(
         ["http://domain.fi/page1", "http://domain.fi/page2", "http://domain.no/0"]
     )
     schedule = other_store.establish_download_schedule()
     assert len(schedule) == 3
```

