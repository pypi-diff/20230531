# Comparing `tmp/pymangaj-0.1.5.tar.gz` & `tmp/pymangaj-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymangaj-0.1.5.tar", last modified: Tue May 30 04:13:53 2023, max compression
+gzip compressed data, was "pymangaj-0.1.6.tar", last modified: Wed May 31 00:17:40 2023, max compression
```

## Comparing `pymangaj-0.1.5.tar` & `pymangaj-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 04:13:53.151758 pymangaj-0.1.5/
--rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      808 2023-05-30 04:13:53.150786 pymangaj-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2023-05-30 04:12:15.000000 pymangaj-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 04:13:53.138758 pymangaj-0.1.5/pymangaj/
--rw-rw-rw-   0        0        0       41 2023-05-30 04:12:41.000000 pymangaj-0.1.5/pymangaj/__init__.py
--rw-rw-rw-   0        0        0     5147 2023-05-30 02:30:14.000000 pymangaj-0.1.5/pymangaj/mangalivre.py
--rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.5/pymangaj/muitomanga.py
--rw-rw-rw-   0        0        0      862 2023-05-30 04:12:26.000000 pymangaj-0.1.5/pymangaj/pymangaj.py
-drwxrwxrwx   0        0        0        0 2023-05-30 04:13:53.148793 pymangaj-0.1.5/pymangaj.egg-info/
--rw-rw-rw-   0        0        0      808 2023-05-30 04:13:53.000000 pymangaj-0.1.5/pymangaj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-30 04:13:53.000000 pymangaj-0.1.5/pymangaj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 04:13:53.000000 pymangaj-0.1.5/pymangaj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 04:13:53.000000 pymangaj-0.1.5/pymangaj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 04:13:53.151758 pymangaj-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-05-30 04:04:07.000000 pymangaj-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 00:17:40.478164 pymangaj-0.1.6/
+-rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2061 2023-05-31 00:17:40.478164 pymangaj-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1386 2023-05-30 04:12:15.000000 pymangaj-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 00:17:40.458164 pymangaj-0.1.6/pymangaj/
+-rw-rw-rw-   0        0        0       41 2023-05-30 04:12:41.000000 pymangaj-0.1.6/pymangaj/__init__.py
+-rw-rw-rw-   0        0        0     3324 2023-05-30 23:43:38.000000 pymangaj-0.1.6/pymangaj/mangalivre.py
+-rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.6/pymangaj/muitomanga.py
+-rw-rw-rw-   0        0        0     1051 2023-05-31 00:13:55.000000 pymangaj-0.1.6/pymangaj/pymangaj.py
+drwxrwxrwx   0        0        0        0 2023-05-31 00:17:40.476164 pymangaj-0.1.6/pymangaj.egg-info/
+-rw-rw-rw-   0        0        0     2061 2023-05-31 00:17:40.000000 pymangaj-0.1.6/pymangaj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-31 00:17:40.000000 pymangaj-0.1.6/pymangaj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 00:17:40.000000 pymangaj-0.1.6/pymangaj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 00:17:40.000000 pymangaj-0.1.6/pymangaj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 00:17:40.478164 pymangaj-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-05-31 00:17:24.000000 pymangaj-0.1.6/setup.py
```

### Comparing `pymangaj-0.1.5/LICENSE` & `pymangaj-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.5/README.md` & `pymangaj-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.5/pymangaj/mangalivre.py` & `pymangaj-0.1.6/pymangaj/mangalivre.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,50 @@
 import re
 
 import requests
 
 headers = {
-    'authority': 'mangalivre.net',
-    'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
-    'accept-language': 'en-US,en;q=0.9,pt-BR;q=0.8,pt;q=0.7',
-    'cache-control': 'max-age=0',
+    'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
+    'cache-control': 'max-age=259200',
     'cookie': '_ga=e88959f7-3144-4ae1-af76-cc99b0df6e80; __cf_bm=9SAugMSkcEA8uS.y5FOZY3v.0aNn9ixEZPjsM2iSsP0-1665619463-0-Aa+7SXgc7e2OpVQtzIm4aZ1YSXqEz3CXssnfWO+zBj1yG+g21hUjq8u++ogPiGr0NsHH7kKPUHHmQ8ezanE581oEECXcKvZJjK3vx/FgdoQ/zjLBoyEmVvFfKu+rX16jiw==; cf_use_ob=0',
-    'referer': 'https://mangalivre.net/ler/naruto/online/70908/700-09',
-    'sec-ch-ua': '"Chromium";v="106", "Microsoft Edge";v="106", "Not;A=Brand";v="99"',
+    'authority': 'mangalivre.net',
+    'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;application/json, text/javascript, */*;q=0.9',
     'sec-ch-ua-mobile': '?0',
     'sec-ch-ua-platform': '"Linux"',
     'sec-fetch-dest': 'document',
-    'sec-fetch-mode': 'navigate',
+    'sec-fetch-mode': 'cors',
     'sec-fetch-site': 'same-origin',
+    'Access-Control-Allow-Origin': '*',
+    'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36 Edg/106.0.1370.42',
+    'x-requested-with': 'XMLHttpRequest',
     'sec-fetch-user': '?1',
-    'upgrade-insecure-requests': '1',
-    'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36 Edg/106.0.1370.42'
+    'upgrade-insecure-requests': '1'
 }
 
-headers_2 = {
-        'authority': 'mangalivre.net',
-        'accept': 'application/json, text/javascript, */*; q=0.01',
-        'accept-language': 'en-US,en;q=0.9,pt-BR;q=0.8,pt;q=0.7',
-        'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
-        'cookie': '_ga=e88959f7-3144-4ae1-af76-cc99b0df6e80; __cf_bm=5KDbO1NiKCprQ4ALceOr5UTG7B1n2U4tZ.19Fskp1os-1665617107-0-AYqASKEgB0jSGmmoLUnqambiOQwd4gxR17TEWSoslp2twJ6U1oFj+5PRkZkwGmCyJ+LI61LAFCiQKnu0z9k0XsP3iTmSsVrhSaMLbLFJfS/vjg5l3nqZtNTuNydyN1ceLA==; cf_use_ob=0',
-        'origin': 'https://mangalivre.net',
-        'referer': 'https://mangalivre.net/lista-de-mangas/ordenar-por-numero-de-leituras/todos/desde-o-comeco',
-        'sec-ch-ua': '"Chromium";v="106", "Microsoft Edge";v="106", "Not;A=Brand";v="99"',
-        'sec-ch-ua-mobile': '?0',
-        'sec-ch-ua-platform': '"Linux"',
-        'sec-fetch-dest': 'empty',
-        'sec-fetch-mode': 'cors',
-        'sec-fetch-site': 'same-origin',
-        'Access-Control-Allow-Origin': '*',
-        'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36 Edg/106.0.1370.42',
-        'x-requested-with': 'XMLHttpRequest'
-    }
-
 class MangaLivre:
 
     def __init__(self, manga_name, chapter) -> None:
         self.manga_name = manga_name
         self.chapter = chapter
 
     def search_manga(self, name):
         url = "https://mangalivre.net/lib/search/series.json"
 
         payload = f"search={name}"
      
-        response = requests.post(url, headers=headers_2, data=payload)
+        response = requests.post(url, headers=headers, data=payload)
 
         return response.json().get("series")
 
 
     def get_chapter(self, id_serie, page=1):
         url = f"https://mangalivre.net/series/chapters_list.json?page={page}&id_serie={id_serie}"
     
-        headers = {
-            'sec-ch-ua': '"Chromium";v="106", "Microsoft Edge";v="106", "Not;A=Brand";v="99"',
-            'Accept': 'application/json, text/javascript, */*; q=0.01',
-            'Referer': 'https://mangalivre.net/manga/naruto/1',
-            'X-Requested-With': 'XMLHttpRequest',
-            'sec-ch-ua-mobile': '?0',
-            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36 Edg/106.0.1370.42',
-            'sec-ch-ua-platform': '"Linux"'
-        }
-
         try:
-            response = requests.request("GET", url, headers=headers, data={})
+            response = requests.get(url, headers=headers, data={})
             if response.status_code == 200:
                 for chapter in response.json().get('chapters'):
                     if chapter.get('number') == str(self.chapter):
                         release_scan = list(chapter.get("releases").keys())[0]
                         return chapter.get("releases").get(release_scan).get("id_release"), chapter.get("releases").get(
                             release_scan).get("link")
                 return self.get_chapter(id_serie, page + 1)
```

### Comparing `pymangaj-0.1.5/pymangaj/muitomanga.py` & `pymangaj-0.1.6/pymangaj/muitomanga.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.5/pymangaj/pymangaj.py` & `pymangaj-0.1.6/pymangaj/pymangaj.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 
 
 class pymangaj:
     
     @staticmethod
     # Get mangas by sources
     def search(manga_name, chapter, **sources):
-        result = []
+        pages_result = []
+        if(len(sources) == 0): sources = {'sources':[Sources.MANGA_LIVRE]}
+        if(len(sources['sources']) == 0): raise Exception("Invalid source")
+
         for source in sources['sources']:
             manga_downloader = SourceFactory.get_source(source, manga_name, chapter)
-            pages = manga_downloader.search()
-            result += pages
+            chapter_pages = manga_downloader.search()
+            pages_result += chapter_pages
         
-        return result
+        return pages_result
```

