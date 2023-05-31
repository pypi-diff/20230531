# Comparing `tmp/ngscrape-1.2.0.tar.gz` & `tmp/ngscrape-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-1.2.0.tar", last modified: Wed May 31 00:32:32 2023, max compression
+gzip compressed data, was "ngscrape-1.2.1.tar", last modified: Wed May 31 00:39:59 2023, max compression
```

## Comparing `ngscrape-1.2.0.tar` & `ngscrape-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 00:32:32.205721 ngscrape-1.2.0/
--rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.2.0/LICENSE
--rw-rw-rw-   0        0        0    42296 2023-05-31 00:32:32.203727 ngscrape-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-05-31 00:32:09.000000 ngscrape-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1259 2023-05-28 19:51:04.000000 ngscrape-1.2.0/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-31 00:32:32.205721 ngscrape-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 00:32:32.166724 ngscrape-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 00:32:32.174723 ngscrape-1.2.0/src/ngscrape/
--rw-rw-rw-   0        0        0     7940 2023-05-31 00:31:45.000000 ngscrape-1.2.0/src/ngscrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 00:32:32.199717 ngscrape-1.2.0/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    42296 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 00:39:59.562269 ngscrape-1.2.1/
+-rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0    43961 2023-05-31 00:39:59.561262 ngscrape-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-05-31 00:36:52.000000 ngscrape-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2924 2023-05-31 00:39:25.000000 ngscrape-1.2.1/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 00:39:59.563262 ngscrape-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 00:39:59.528265 ngscrape-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 00:39:59.534277 ngscrape-1.2.1/src/ngscrape/
+-rw-rw-rw-   0        0        0     7907 2023-05-31 00:38:10.000000 ngscrape-1.2.1/src/ngscrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 00:39:59.559283 ngscrape-1.2.1/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    43961 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-1.2.0/LICENSE` & `ngscrape-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-1.2.0/PKG-INFO` & `ngscrape-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.2.0
+Version: 1.2.1
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,18 +683,41 @@
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
 - `scrape_game_by_url(url: str, download: str, filename: str) -> None`
     - Scrape a flash game by url.
     - Parameters:
-        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file.
     - Example parameters:
-        - url = 'https://www.newgrounds.com/portal/view/59593'
-        - download = 'testdir'
-        - filename = 'game.swf'
+        - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - `download = 'testdir'`
+        - `filename = 'game.swf'`
     - Example output with debug mode:
-        - NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
-        - NGScrape: Found flash game link https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499
+        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+        - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
         - NGScrape: Downloaded swf file to testdir/game.swf
+- `scrape_desc_by_url(self, url: str) -> str`
+    - Scrape a flash game's description by url. Returns the description of the game.
+    - Parameters:
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+    - Example parameters:
+        - `url = 'https://www.newgrounds.com/portal/view/59593'`
+    - Example output with debug mode:`
+        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+        - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
+- `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
+    - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
+    - Parameters:
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - download (str): The directory to download the file to.
+        - filename (str): The name of the downloaded file. The file extention will be automatically determined.
+    - Example parameters:
+        - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - `download = 'testdir'`
+        - `filename = 'card'`
+    - Example output with debug mode:
+        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+        - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
+        - NGScrape: Downloaded `swf` file to `testdir/card.png`
```

### Comparing `ngscrape-1.2.0/pyproject.toml` & `ngscrape-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "1.2.0"
+version = "1.2.1"
 description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
```

### Comparing `ngscrape-1.2.0/src/ngscrape/__init__.py` & `ngscrape-1.2.1/src/ngscrape/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         if self.debug:
             print('NGScrape: Downloaded swf file to ' + download + '/' + filename)
             
     def scrape_card_by_url(self, url: str, download: str, filename: str) -> str:
         '''
         Scrape a flash game's card by url. The file extention will be automatically determined.
         Returns the name of the card file.
+        
         Parameters:
             url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
             download (str): The directory to download the file to.
             filename (str): The name of the downloaded file. The file extention will be automatically determined.
         Example parameters:
             url = 'https://www.newgrounds.com/portal/view/59593'
             download = 'testdir'
@@ -113,16 +114,17 @@
                 _imageFiletype = i
         open(download + '/' + filename + _imageFiletype, 'wb').write(requests.get(_gameLink, allow_redirects = True).content)
         if self.debug:
             print('NGScrape: Downloaded swf file to ' + download + '/' + filename + _imageFiletype)
         return filename + _imageFiletype
     def scrape_desc_by_url(self, url: str) -> str:
         '''
-        Scrape a flash game's description by url. The file extention will be automatically determined.
+        Scrape a flash game's description by url.
         Returns the description of the game.
+        
         Parameters:
             url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
         Example parameters:
             url = 'https://www.newgrounds.com/portal/view/59593'
         Example output with debug mode:
             NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
             NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
```

### Comparing `ngscrape-1.2.0/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-1.2.1/src/ngscrape.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.2.0
+Version: 1.2.1
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,18 +683,41 @@
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
 - `scrape_game_by_url(url: str, download: str, filename: str) -> None`
     - Scrape a flash game by url.
     - Parameters:
-        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is https://www.newgrounds.com/portal/view/59593.
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file.
     - Example parameters:
-        - url = 'https://www.newgrounds.com/portal/view/59593'
-        - download = 'testdir'
-        - filename = 'game.swf'
+        - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - `download = 'testdir'`
+        - `filename = 'game.swf'`
     - Example output with debug mode:
-        - NGScrape: Made request to https://www.newgrounds.com/portal/view/59593 and got status code 200
-        - NGScrape: Found flash game link https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499
+        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+        - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
         - NGScrape: Downloaded swf file to testdir/game.swf
+- `scrape_desc_by_url(self, url: str) -> str`
+    - Scrape a flash game's description by url. Returns the description of the game.
+    - Parameters:
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+    - Example parameters:
+        - `url = 'https://www.newgrounds.com/portal/view/59593'`
+    - Example output with debug mode:`
+        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+        - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
+- `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
+    - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
+    - Parameters:
+        - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
+        - download (str): The directory to download the file to.
+        - filename (str): The name of the downloaded file. The file extention will be automatically determined.
+    - Example parameters:
+        - `url = 'https://www.newgrounds.com/portal/view/59593'`
+        - `download = 'testdir'`
+        - `filename = 'card'`
+    - Example output with debug mode:
+        - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
+        - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
+        - NGScrape: Downloaded `swf` file to `testdir/card.png`
```

