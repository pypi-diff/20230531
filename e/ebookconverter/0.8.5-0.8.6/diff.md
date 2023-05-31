# Comparing `tmp/ebookconverter-0.8.5.tar.gz` & `tmp/ebookconverter-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebookconverter-0.8.5.tar", last modified: Wed Mar  8 17:25:04 2023, max compression
+gzip compressed data, was "ebookconverter-0.8.6.tar", last modified: Wed May 31 20:48:06 2023, max compression
```

## Comparing `ebookconverter-0.8.5.tar` & `ebookconverter-0.8.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-08 17:25:04.615508 ebookconverter-0.8.5/
--rw-r--r--   0 eric       (501) staff       (20)     8945 2023-03-08 16:48:26.000000 ebookconverter-0.8.5/CHANGES
--rw-r--r--   0 eric       (501) staff       (20)    35149 2018-12-20 21:57:45.000000 ebookconverter-0.8.5/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)     2546 2023-03-08 17:25:04.615290 ebookconverter-0.8.5/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1903 2022-11-18 17:54:42.000000 ebookconverter-0.8.5/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-08 17:25:04.609328 ebookconverter-0.8.5/ebookconverter/
--rwxr-xr-x   0 eric       (501) staff       (20)     2954 2021-09-02 06:13:21.000000 ebookconverter-0.8.5/ebookconverter/AutoDelete.py
--rw-r--r--   0 eric       (501) staff       (20)     1602 2021-08-11 20:29:59.000000 ebookconverter-0.8.5/ebookconverter/CSV.py
--rw-r--r--   0 eric       (501) staff       (20)     2626 2021-10-21 15:37:14.000000 ebookconverter-0.8.5/ebookconverter/Candidates.py
--rw-r--r--   0 eric       (501) staff       (20)    22860 2023-02-15 18:47:03.000000 ebookconverter-0.8.5/ebookconverter/EbookConverter.py
--rwxr-xr-x   0 eric       (501) staff       (20)    10752 2023-02-01 17:40:59.000000 ebookconverter-0.8.5/ebookconverter/FileInfo.py
--rw-r--r--   0 eric       (501) staff       (20)     5557 2023-03-06 20:45:09.000000 ebookconverter-0.8.5/ebookconverter/Notifier.py
--rw-r--r--   0 eric       (501) staff       (20)     2070 2022-09-14 19:47:10.000000 ebookconverter-0.8.5/ebookconverter/ReloadWorkflow.py
--rw-r--r--   0 eric       (501) staff       (20)     3444 2022-09-14 20:35:23.000000 ebookconverter-0.8.5/ebookconverter/UpdateFromWorkflow.py
--rw-r--r--   0 eric       (501) staff       (20)       18 2023-03-08 16:48:38.000000 ebookconverter-0.8.5/ebookconverter/Version.py
--rw-r--r--   0 eric       (501) staff       (20)       27 2014-08-23 15:53:05.000000 ebookconverter-0.8.5/ebookconverter/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-08 17:25:04.612039 ebookconverter-0.8.5/ebookconverter/writers/
--rw-r--r--   0 eric       (501) staff       (20)     1707 2021-10-18 22:59:45.000000 ebookconverter-0.8.5/ebookconverter/writers/CoverWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     3193 2022-04-28 19:36:11.000000 ebookconverter-0.8.5/ebookconverter/writers/FacebookWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     1330 2021-09-02 06:13:21.000000 ebookconverter-0.8.5/ebookconverter/writers/QRCodeWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     7222 2023-02-03 19:48:11.000000 ebookconverter-0.8.5/ebookconverter/writers/RDFWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     3024 2019-09-17 19:12:37.000000 ebookconverter-0.8.5/ebookconverter/writers/TwitterWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     1387 2022-09-29 19:43:00.000000 ebookconverter-0.8.5/ebookconverter/writers/UpdateWriter.py
--rw-r--r--   0 eric       (501) staff       (20)       10 2014-02-08 17:56:38.000000 ebookconverter-0.8.5/ebookconverter/writers/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-08 17:25:04.610056 ebookconverter-0.8.5/ebookconverter.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     2546 2023-03-08 17:25:04.000000 ebookconverter-0.8.5/ebookconverter.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1023 2023-03-08 17:25:04.000000 ebookconverter-0.8.5/ebookconverter.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-03-08 17:25:04.000000 ebookconverter-0.8.5/ebookconverter.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)      124 2023-03-08 17:25:04.000000 ebookconverter-0.8.5/ebookconverter.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       15 2023-03-08 17:25:04.000000 ebookconverter-0.8.5/ebookconverter.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-03-08 17:25:04.614797 ebookconverter-0.8.5/scripts/
--rwxr-xr-x   0 eric       (501) staff       (20)      302 2021-09-02 06:13:21.000000 ebookconverter-0.8.5/scripts/autodelete
--rwxr-xr--   0 eric       (501) staff       (20)      209 2022-08-18 12:44:23.000000 ebookconverter-0.8.5/scripts/cron-dopush-social.sh
--rwxr-xr-x   0 eric       (501) staff       (20)     1852 2022-08-18 12:51:16.000000 ebookconverter-0.8.5/scripts/cron-dopush.sh
--rwxr-xr--   0 eric       (501) staff       (20)     1043 2021-08-26 15:02:12.000000 ebookconverter-0.8.5/scripts/cron-jekyll.sh
--rwxr-xr-x   0 eric       (501) staff       (20)      428 2022-08-18 13:04:36.000000 ebookconverter-0.8.5/scripts/cron-rebuild-files.sh
--rwxr-xr-x   0 eric       (501) staff       (20)      244 2021-09-02 06:13:21.000000 ebookconverter-0.8.5/scripts/ebookconverter
--rwxr-xr-x   0 eric       (501) staff       (20)      294 2021-09-02 06:13:21.000000 ebookconverter-0.8.5/scripts/fileinfo
--rwxr-xr-x   0 eric       (501) staff       (20)      228 2021-09-02 06:13:21.000000 ebookconverter-0.8.5/scripts/make_csv
--rwxr-xr-x   0 eric       (501) staff       (20)      287 2022-07-26 15:05:15.000000 ebookconverter-0.8.5/scripts/reload_workflow
--rwxr-xr-x   0 eric       (501) staff       (20)      299 2022-09-14 21:30:51.000000 ebookconverter-0.8.5/scripts/update_from_backup_workflow
--rw-r--r--   0 eric       (501) staff       (20)       38 2023-03-08 17:25:04.615563 ebookconverter-0.8.5/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)     1645 2023-03-08 16:49:03.000000 ebookconverter-0.8.5/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 20:48:06.484730 ebookconverter-0.8.6/
+-rw-r--r--   0 eric       (501) staff       (20)     9062 2023-05-31 20:19:55.000000 ebookconverter-0.8.6/CHANGES
+-rw-r--r--   0 eric       (501) staff       (20)    35149 2018-12-20 21:57:45.000000 ebookconverter-0.8.6/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)     2546 2023-05-31 20:48:06.484542 ebookconverter-0.8.6/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1903 2022-11-18 17:54:42.000000 ebookconverter-0.8.6/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 20:48:06.479824 ebookconverter-0.8.6/ebookconverter/
+-rwxr-xr-x   0 eric       (501) staff       (20)     2954 2021-09-02 06:13:21.000000 ebookconverter-0.8.6/ebookconverter/AutoDelete.py
+-rw-r--r--   0 eric       (501) staff       (20)     1602 2021-08-11 20:29:59.000000 ebookconverter-0.8.6/ebookconverter/CSV.py
+-rw-r--r--   0 eric       (501) staff       (20)     2626 2021-10-21 15:37:14.000000 ebookconverter-0.8.6/ebookconverter/Candidates.py
+-rw-r--r--   0 eric       (501) staff       (20)    22936 2023-05-31 17:18:45.000000 ebookconverter-0.8.6/ebookconverter/EbookConverter.py
+-rwxr-xr-x   0 eric       (501) staff       (20)    10752 2023-02-01 17:40:59.000000 ebookconverter-0.8.6/ebookconverter/FileInfo.py
+-rw-r--r--   0 eric       (501) staff       (20)     5557 2023-03-06 20:45:09.000000 ebookconverter-0.8.6/ebookconverter/Notifier.py
+-rw-r--r--   0 eric       (501) staff       (20)     2070 2022-09-14 19:47:10.000000 ebookconverter-0.8.6/ebookconverter/ReloadWorkflow.py
+-rw-r--r--   0 eric       (501) staff       (20)     3444 2022-09-14 20:35:23.000000 ebookconverter-0.8.6/ebookconverter/UpdateFromWorkflow.py
+-rw-r--r--   0 eric       (501) staff       (20)       18 2023-05-31 20:43:28.000000 ebookconverter-0.8.6/ebookconverter/Version.py
+-rw-r--r--   0 eric       (501) staff       (20)       27 2014-08-23 15:53:05.000000 ebookconverter-0.8.6/ebookconverter/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 20:48:06.482407 ebookconverter-0.8.6/ebookconverter/writers/
+-rw-r--r--   0 eric       (501) staff       (20)     1707 2021-10-18 22:59:45.000000 ebookconverter-0.8.6/ebookconverter/writers/CoverWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     3193 2022-04-28 19:36:11.000000 ebookconverter-0.8.6/ebookconverter/writers/FacebookWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     2863 2023-05-31 20:28:03.000000 ebookconverter-0.8.6/ebookconverter/writers/MastodonWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     1330 2021-09-02 06:13:21.000000 ebookconverter-0.8.6/ebookconverter/writers/QRCodeWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     7222 2023-02-03 19:48:11.000000 ebookconverter-0.8.6/ebookconverter/writers/RDFWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     3024 2019-09-17 19:12:37.000000 ebookconverter-0.8.6/ebookconverter/writers/TwitterWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     1387 2022-09-29 19:43:00.000000 ebookconverter-0.8.6/ebookconverter/writers/UpdateWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)       10 2014-02-08 17:56:38.000000 ebookconverter-0.8.6/ebookconverter/writers/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 20:48:06.480510 ebookconverter-0.8.6/ebookconverter.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     2546 2023-05-31 20:48:06.000000 ebookconverter-0.8.6/ebookconverter.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1064 2023-05-31 20:48:06.000000 ebookconverter-0.8.6/ebookconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-31 20:48:06.000000 ebookconverter-0.8.6/ebookconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)      124 2023-05-31 20:48:06.000000 ebookconverter-0.8.6/ebookconverter.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       15 2023-05-31 20:48:06.000000 ebookconverter-0.8.6/ebookconverter.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-31 20:48:06.484128 ebookconverter-0.8.6/scripts/
+-rwxr-xr-x   0 eric       (501) staff       (20)      302 2021-09-02 06:13:21.000000 ebookconverter-0.8.6/scripts/autodelete
+-rwxr-xr--   0 eric       (501) staff       (20)      226 2023-05-31 17:19:41.000000 ebookconverter-0.8.6/scripts/cron-dopush-social.sh
+-rwxr-xr-x   0 eric       (501) staff       (20)     1852 2022-08-18 12:51:16.000000 ebookconverter-0.8.6/scripts/cron-dopush.sh
+-rwxr-xr--   0 eric       (501) staff       (20)     1043 2021-08-26 15:02:12.000000 ebookconverter-0.8.6/scripts/cron-jekyll.sh
+-rwxr-xr-x   0 eric       (501) staff       (20)      428 2022-08-18 13:04:36.000000 ebookconverter-0.8.6/scripts/cron-rebuild-files.sh
+-rwxr-xr-x   0 eric       (501) staff       (20)      244 2021-09-02 06:13:21.000000 ebookconverter-0.8.6/scripts/ebookconverter
+-rwxr-xr-x   0 eric       (501) staff       (20)      294 2021-09-02 06:13:21.000000 ebookconverter-0.8.6/scripts/fileinfo
+-rwxr-xr-x   0 eric       (501) staff       (20)      228 2021-09-02 06:13:21.000000 ebookconverter-0.8.6/scripts/make_csv
+-rwxr-xr-x   0 eric       (501) staff       (20)      287 2022-07-26 15:05:15.000000 ebookconverter-0.8.6/scripts/reload_workflow
+-rwxr-xr-x   0 eric       (501) staff       (20)      299 2022-09-14 21:30:51.000000 ebookconverter-0.8.6/scripts/update_from_backup_workflow
+-rw-r--r--   0 eric       (501) staff       (20)       38 2023-05-31 20:48:06.484779 ebookconverter-0.8.6/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)     1645 2023-05-31 20:42:55.000000 ebookconverter-0.8.6/setup.py
```

### Comparing `ebookconverter-0.8.5/CHANGES` & `ebookconverter-0.8.6/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-0.8.5 (March 8, 2023
+0.8.6 (May 31, 2023)
+- adds MastodonWriter, to replicate TwitterWriter (posting on @gutenberg_new@mastodon.social)
+
+0.8.5 (March 8, 2023)
 - normalize capitalization of "eBook"
 - only send notification for CRITICAL errors #33
 
 0.8.4 (February 15, 2023)
 - notifications, both success and problem alerts, are now sent only to the whitewasher.
 - notification texts have been cleaned up to be more readable and more friendly
 - refactored  PUBLIC, FILES, FTP into libgutenberg>=0.10.15
```

### Comparing `ebookconverter-0.8.5/LICENSE` & `ebookconverter-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/PKG-INFO` & `ebookconverter-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebookconverter
-Version: 0.8.5
+Version: 0.8.6
 Summary: The Project Gutenberg tool to orchestrate ebook generation.
 Home-page: https://github.com/gutenbergtools/ebookconverter/
 Author: Eric Hellman
 Author-email: eric@hellman.org
 License: GPL v3
 Platform: OS-independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ebookconverter-0.8.5/README.md` & `ebookconverter-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/AutoDelete.py` & `ebookconverter-0.8.6/ebookconverter/AutoDelete.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/CSV.py` & `ebookconverter-0.8.6/ebookconverter/CSV.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/Candidates.py` & `ebookconverter-0.8.6/ebookconverter/Candidates.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/EbookConverter.py` & `ebookconverter-0.8.6/ebookconverter/EbookConverter.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     'cover.medium': ('rst/*', 'html/*', 'txt/*', 'tex/*'),
 
     # only make these if there's a source file registered in the database
     'rdf': ('rst/*', 'html/*', 'txt/*', 'tex/*'),
     'qrcode': ('rst/*', 'html/*', 'txt/*', 'tex/*'),
     'facebook': ('rst/*', 'html/*', 'txt/*', 'tex/*'),
     'twitter': ('rst/*', 'html/*', 'txt/*', 'tex/*'),
+    'mastodon': ('rst/*', 'html/*', 'txt/*', 'tex/*'),
     'update': ('rst/*', 'html/*', 'txt/*', 'tex/*'),
 }
 
 PREFERRED_INPUT_FORMATS['html.noimages']      = PREFERRED_INPUT_FORMATS['html.images']
 PREFERRED_INPUT_FORMATS['epub.noimages']      = PREFERRED_INPUT_FORMATS['epub.images']
 PREFERRED_INPUT_FORMATS['pdf.noimages']       = PREFERRED_INPUT_FORMATS['pdf.images']
 PREFERRED_INPUT_FORMATS['picsdir.noimages']   = PREFERRED_INPUT_FORMATS['picsdir.images']
@@ -117,15 +118,15 @@
     'cover.medium':     'pg{id}.cover.medium.jpg',
     'qrcode':           'pg{id}.qrcode.png',
     'logfile':          'pg{id}.converter.log',      # .converter because of latex log conflicts
 }
 GENERIC_FILENAME = 'pg{id}.generic'
 
 DEPENDENCIES = collections.OrderedDict((
-    ('everything',      ('all', 'kindle.noimages','facebook', 'twitter', 'update')),
+    ('everything',      ('all', 'kindle.noimages','facebook', 'twitter', 'mastodon', 'update')),
     ('all',             ('html', 'epub', 'kindle', 'epub3', 'kf8', 'pdf', 'txt', 'rst',
                          'cover', 'qrcode', 'rdf')),
     ('html',            ('html.images',    'html.noimages')),
     ('epub',            ('epub.images',    'epub.noimages')),
     ('epub3',           ('epub3.images', )),
     ('kindle',          ('kindle.images',)),
     ('kf8',             ('kf8.images', )),
@@ -148,15 +149,15 @@
 txt.utf-8
 html.images html.noimages
 epub.noimages kindle.noimages pdf.noimages
 cover.small cover.medium
 epub.images kindle.images pdf.images
 epub3.images kf8.images
 qrcode rdf
-facebook twitter
+facebook twitter mastodon
 update
 null
 """.split()
 
 MAX_CANDIDATE_SIZE = {'txt': 8, 'epub': 16, 'epub3': 16}
 
 def make_output_filename(type_, ebook = 0):
```

### Comparing `ebookconverter-0.8.5/ebookconverter/FileInfo.py` & `ebookconverter-0.8.6/ebookconverter/FileInfo.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/Notifier.py` & `ebookconverter-0.8.6/ebookconverter/Notifier.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/ReloadWorkflow.py` & `ebookconverter-0.8.6/ebookconverter/ReloadWorkflow.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/UpdateFromWorkflow.py` & `ebookconverter-0.8.6/ebookconverter/UpdateFromWorkflow.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/writers/CoverWriter.py` & `ebookconverter-0.8.6/ebookconverter/writers/CoverWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/writers/FacebookWriter.py` & `ebookconverter-0.8.6/ebookconverter/writers/FacebookWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/writers/QRCodeWriter.py` & `ebookconverter-0.8.6/ebookconverter/writers/QRCodeWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/writers/RDFWriter.py` & `ebookconverter-0.8.6/ebookconverter/writers/RDFWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/writers/TwitterWriter.py` & `ebookconverter-0.8.6/ebookconverter/writers/TwitterWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter/writers/UpdateWriter.py` & `ebookconverter-0.8.6/ebookconverter/writers/UpdateWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/ebookconverter.egg-info/PKG-INFO` & `ebookconverter-0.8.6/ebookconverter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebookconverter
-Version: 0.8.5
+Version: 0.8.6
 Summary: The Project Gutenberg tool to orchestrate ebook generation.
 Home-page: https://github.com/gutenbergtools/ebookconverter/
 Author: Eric Hellman
 Author-email: eric@hellman.org
 License: GPL v3
 Platform: OS-independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ebookconverter-0.8.5/ebookconverter.egg-info/SOURCES.txt` & `ebookconverter-0.8.6/ebookconverter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ebookconverter.egg-info/PKG-INFO
 ebookconverter.egg-info/SOURCES.txt
 ebookconverter.egg-info/dependency_links.txt
 ebookconverter.egg-info/requires.txt
 ebookconverter.egg-info/top_level.txt
 ebookconverter/writers/CoverWriter.py
 ebookconverter/writers/FacebookWriter.py
+ebookconverter/writers/MastodonWriter.py
 ebookconverter/writers/QRCodeWriter.py
 ebookconverter/writers/RDFWriter.py
 ebookconverter/writers/TwitterWriter.py
 ebookconverter/writers/UpdateWriter.py
 ebookconverter/writers/__init__.py
 scripts/autodelete
 scripts/cron-dopush-social.sh
```

### Comparing `ebookconverter-0.8.5/scripts/cron-dopush.sh` & `ebookconverter-0.8.6/scripts/cron-dopush.sh`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/scripts/cron-jekyll.sh` & `ebookconverter-0.8.6/scripts/cron-jekyll.sh`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.8.5/setup.py` & `ebookconverter-0.8.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # ebookconverter distribution
 #
 
 from setuptools import setup
 
-VERSION = '0.8.5'
+VERSION = '0.8.6'
 
 setup (
     name = 'ebookconverter',
     version = VERSION,
 
     packages = [
         'ebookconverter',
```

