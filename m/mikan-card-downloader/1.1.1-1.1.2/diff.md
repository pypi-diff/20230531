# Comparing `tmp/mikan_card_downloader-1.1.1.tar.gz` & `tmp/mikan_card_downloader-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-1.1.1.tar", max compression
+gzip compressed data, was "mikan_card_downloader-1.1.2.tar", max compression
```

## Comparing `mikan_card_downloader-1.1.1.tar` & `mikan_card_downloader-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.1.1/LICENSE
--rw-r--r--   0        0        0     1041 2023-05-30 17:24:07.287889 mikan_card_downloader-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.1/src/mikan/__init__.py
--rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.1/src/mikan/classes.py
--rw-r--r--   0        0        0     1491 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.1/src/mikan/config.py
--rw-r--r--   0        0        0     3294 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.1/src/mikan/downloader.py
--rw-r--r--   0        0        0     5973 2023-05-30 17:19:50.146741 mikan_card_downloader-1.1.1/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.1.1/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2383 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.1/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.1/src/mikan/py.typed
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1041 2023-05-31 16:51:08.786603 mikan_card_downloader-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.2/src/mikan/__init__.py
+-rw-r--r--   0        0        0     1536 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.2/src/mikan/classes.py
+-rw-r--r--   0        0        0     1491 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.2/src/mikan/config.py
+-rw-r--r--   0        0        0     3294 2023-05-31 10:39:28.598760 mikan_card_downloader-1.1.2/src/mikan/downloader.py
+-rw-r--r--   0        0        0     5673 2023-05-31 10:47:12.451838 mikan_card_downloader-1.1.2/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-1.1.2/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2383 2023-05-05 22:20:27.438705 mikan_card_downloader-1.1.2/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-1.1.2/src/mikan/py.typed
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-1.1.2/PKG-INFO
```

### Comparing `mikan_card_downloader-1.1.1/LICENSE` & `mikan_card_downloader-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.1/pyproject.toml` & `mikan_card_downloader-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "1.1.1"
+version = "1.1.2"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
```

### Comparing `mikan_card_downloader-1.1.1/src/mikan/classes.py` & `mikan_card_downloader-1.1.2/src/mikan/classes.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.1/src/mikan/config.py` & `mikan_card_downloader-1.1.2/src/mikan/config.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.1/src/mikan/downloader.py` & `mikan_card_downloader-1.1.2/src/mikan/downloader.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.1/src/mikan/html_parser.py` & `mikan_card_downloader-1.1.2/src/mikan/html_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             current_page = await self.get_page(current_num)
             if not current_page and self.img_type != SIFCard:
                 break
 
             current_num += 1
 
     async def add_item_to_object_list(self, item: int) -> None:
-        i, obj = await self.item_parser.create_item(
+        obj = await self.item_parser.create_item(
             await self.request_url_data(f"{self.img_type.url_template}{item}")
         )
         self.objs[self.img_type.results_dir][str(item)] = obj
         print(f"Getting item {item}.")
 
 
 class SIFListParser:
@@ -105,17 +105,17 @@
     async def get_num_pages(self, data: aiohttp.ClientResponse) -> int:
         json = await data.json()
         self.items = [json[i : i + 10] for i in range(0, len(json), 10)]  # noqa
         return len(self.items)
 
 
 class SIFCardParser:
-    async def create_item(self, data: aiohttp.ClientResponse) -> tuple[str, list[str]]:
+    async def create_item(self, data: aiohttp.ClientResponse) -> list[str]:
         json = await data.json()
-        return str(json["id"]), [
+        return [
             card for card in [json["card_image"], json["card_idolized_image"]] if card
         ]
 
 
 class ListParser:
     async def get_page(self, data: Any) -> list[int]:
         nums: list[int] = []
@@ -146,35 +146,31 @@
             if match := pattern.search(string):
                 return int(match.group(1))
 
         raise ListParsingException("An error occured while getting number of pages.")
 
 
 class CardParser:
-    async def create_item(self, data: aiohttp.ClientResponse) -> tuple[str, list[str]]:
+    async def create_item(self, data: aiohttp.ClientResponse) -> list[str]:
         page = bs4.BeautifulSoup(await data.text(), features="lxml")
-        pattern = re.compile(r"(\d+)")
 
         if isinstance(top_item := page.find(class_="top-item"), bs4.Tag):
             links = top_item.find_all("a")
             first: str = links[0].get("href")
             second: str = links[1].get("href")
 
-            if match := pattern.search(first.split("/")[-1]):
-                return match.group(1), [first, second]
+            return [first, second]
 
         raise ItemParsingException("An error occured while getting a card.")
 
 
 class StillParser:
-    async def create_item(self, data: aiohttp.ClientResponse) -> tuple[str, list[str]]:
+    async def create_item(self, data: aiohttp.ClientResponse) -> list[str]:
         page = bs4.BeautifulSoup(await data.text(), features="lxml")
-        pattern = re.compile(r"(.+)Still")
 
         if isinstance(top_item := page.find(class_="top-item"), bs4.Tag):
             links = top_item.find_all("a")
             url: str = links[0].get("href")
 
-            if match := pattern.search(url.split("/")[-1]):
-                return match.group(1), [url]
+            return [url]
 
         raise ItemParsingException("An error occured while getting a still.")
```

### Comparing `mikan_card_downloader-1.1.1/src/mikan/json_utils.py` & `mikan_card_downloader-1.1.2/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.1/src/mikan/main.py` & `mikan_card_downloader-1.1.2/src/mikan/main.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-1.1.1/PKG-INFO` & `mikan_card_downloader-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikan-card-downloader
-Version: 1.1.1
+Version: 1.1.2
 Summary: Downloads cards and stills from SIFAS and SIF.
 License: GPLv3
 Author: DemonicSavage
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

