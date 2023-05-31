# Comparing `tmp/python-nozomi-1.2.0.tar.gz` & `tmp/python-nozomi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-nozomi-1.2.0.tar", last modified: Mon Dec 14 22:14:25 2020, max compression
+gzip compressed data, was "python-nozomi-2.0.0.tar", last modified: Wed May 31 00:37:07 2023, max compression
```

## Comparing `python-nozomi-1.2.0.tar` & `python-nozomi-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-12-14 22:14:25.028644 python-nozomi-1.2.0/
--rw-rw-rw-   0        0        0     2556 2020-12-14 22:14:25.028644 python-nozomi-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1499 2020-12-14 20:09:18.000000 python-nozomi-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2020-12-14 22:14:24.956837 python-nozomi-1.2.0/nozomi/
--rw-rw-rw-   0        0        0       37 2020-12-14 20:09:18.000000 python-nozomi-1.2.0/nozomi/__init__.py
--rw-rw-rw-   0        0        0     5961 2020-12-14 22:13:54.000000 python-nozomi-1.2.0/nozomi/api.py
--rw-rw-rw-   0        0        0     3195 2020-12-14 22:13:55.000000 python-nozomi-1.2.0/nozomi/data.py
--rw-rw-rw-   0        0        0      299 2020-12-14 22:13:55.000000 python-nozomi-1.2.0/nozomi/exceptions.py
--rw-rw-rw-   0        0        0     4621 2020-12-14 22:13:55.000000 python-nozomi-1.2.0/nozomi/helpers.py
-drwxrwxrwx   0        0        0        0 2020-12-14 22:14:25.026649 python-nozomi-1.2.0/python_nozomi.egg-info/
--rw-rw-rw-   0        0        0     2556 2020-12-14 22:14:24.000000 python-nozomi-1.2.0/python_nozomi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2020-12-14 22:14:24.000000 python-nozomi-1.2.0/python_nozomi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-14 22:14:24.000000 python-nozomi-1.2.0/python_nozomi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2020-12-14 22:14:24.000000 python-nozomi-1.2.0/python_nozomi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2020-12-14 22:14:24.000000 python-nozomi-1.2.0/python_nozomi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2020-12-14 22:14:25.039615 python-nozomi-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1005 2020-12-14 22:13:48.000000 python-nozomi-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 00:37:07.852008 python-nozomi-2.0.0/
+-rw-rw-rw-   0        0        0     1084 2023-05-24 20:45:54.000000 python-nozomi-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3509 2023-05-31 00:37:07.852008 python-nozomi-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2581 2023-05-31 00:32:09.000000 python-nozomi-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 00:37:07.820097 python-nozomi-2.0.0/nozomi/
+-rw-rw-rw-   0        0        0       37 2023-05-24 20:45:54.000000 python-nozomi-2.0.0/nozomi/__init__.py
+-rw-rw-rw-   0        0        0     6105 2023-05-31 00:32:09.000000 python-nozomi-2.0.0/nozomi/api.py
+-rw-rw-rw-   0        0        0     2905 2023-05-31 00:02:41.000000 python-nozomi-2.0.0/nozomi/data.py
+-rw-rw-rw-   0        0        0      299 2023-05-24 20:45:54.000000 python-nozomi-2.0.0/nozomi/exceptions.py
+-rw-rw-rw-   0        0        0     5762 2023-05-26 16:44:57.000000 python-nozomi-2.0.0/nozomi/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-31 00:37:07.850012 python-nozomi-2.0.0/python_nozomi.egg-info/
+-rw-rw-rw-   0        0        0     3509 2023-05-31 00:37:07.000000 python-nozomi-2.0.0/python_nozomi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-31 00:37:07.000000 python-nozomi-2.0.0/python_nozomi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 00:37:07.000000 python-nozomi-2.0.0/python_nozomi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-31 00:37:07.000000 python-nozomi-2.0.0/python_nozomi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 00:37:07.000000 python-nozomi-2.0.0/python_nozomi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-31 00:37:07.858988 python-nozomi-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1267 2023-05-31 00:25:28.000000 python-nozomi-2.0.0/setup.py
```

### Comparing `python-nozomi-1.2.0/PKG-INFO` & `python-nozomi-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,109 @@
 Metadata-Version: 2.1
 Name: python-nozomi
-Version: 1.2.0
+Version: 2.0.0
 Summary: Nozomi API for retrieving images, videos, gifs.
 Home-page: https://github.com/Alfa-Q/python-nozomi
+Download-URL: https://github.com/Alfa-Q/python-nozomi/archive/2.0.0.tar.gz
 Author: Alfa_Q
 Author-email: alfakyuu@gmail.com
 License: MIT
-Download-URL: https://github.com/Alfa-Q/python-nozomi/archive/1.1.1.tar.gz
-Description: # python-nozomi
-        [![Build Status](https://travis-ci.com/Alfa-Q/python-nozomi.svg?token=NAcpuTjLC6CrUpWrqz9p&branch=master)](https://travis-ci.com/Alfa-Q/python-nozomi)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/f3bffdff70794c5cb569645b60699e0b)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Alfa-Q/python-nozomi&amp;utm_campaign=Badge_Grade)
-        [![PyPI version](https://badge.fury.io/py/python-nozomi.svg)](https://badge.fury.io/py/python-nozomi)
-        [![Python version](https://img.shields.io/badge/python-%203.7%20%7C%203.8-green)](https://www.python.org/downloads/release/python-360/)
-        
-        nozomi.la API in Python.
-        
-        ## Features
-        -   Retrieving image and video posts
-        -   Downloading posts
-        
-        ## Installation
-        ```
-        $ pip install python-nozomi
-        ```
-        
-        ## Example Usage
-        Retrieve and download all posts containing certain tags
-        ```python
-        from pathlib import Path
-        from nozomi import api
-            
-        # The tags that the posts retrieved must contain
-        positive_tags = ['veigar', 'wallpaper']
-        
-        # Gets all posts with the tags 'veigar', 'wallpaper'
-        for post in api.get_posts(positive_tags):
-            api.download_media(post, Path.cwd())
-        ```
-        
-        Retrieve all posts containing certain tags with blacklisted tags
-        ```python
-        # The blacklisted tags
-        negative_tags = ['chogath']
-        
-        # Gets all posts with the tags 'veigar', 'wallpaper' but no 'chogath' tag.
-        for post in api.get_posts(positive_tags, negative_tags):
-            api.download_media(post, Path.cwd())
-        ```
-        
 Keywords: nozomi,nozomi.la,api,video,image,anime
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# python-nozomi
+
+[![Build Status](https://travis-ci.com/Alfa-Q/python-nozomi.svg?token=NAcpuTjLC6CrUpWrqz9p&branch=master)](https://travis-ci.com/Alfa-Q/python-nozomi)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/20c7f3716811466c9e2d55786885951e)](https://app.codacy.com/gh/Alfa-Q/python-nozomi/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/20c7f3716811466c9e2d55786885951e)](https://app.codacy.com/gh/Alfa-Q/python-nozomi/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![PyPI version](https://badge.fury.io/py/python-nozomi.svg)](https://badge.fury.io/py/python-nozomi)
+[![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-green)](https://www.python.org/downloads/release/python-370/)
+
+nozomi.la API in Python.
+
+## Features
+
+- Retrieving media posts
+- Downloading media
+
+## Installation
+
+```
+$ pip install python-nozomi
+```
+
+## Upgrade
+
+```
+$ pip install python-nozomi --upgrade
+```
+
+## Example Usage
+
+Retrieve and download a single post provided a URL
+
+```python
+from pathlib import Path
+from nozomi import api
+
+url = 'https://nozomi.la/post/26905532.html#veigar'
+
+# Retrieve post metadata using the URL
+post = api.get_post(url)
+
+# Download the post
+api.download_media(post, Path.cwd())
+```
+
+Retrieve and download multiple posts provided a list of URLs
+
+```python
+from pathlib import Path
+from nozomi import api
+
+urls = [
+    'https://nozomi.la/post/26905532.html#veigar',
+    "https://nozomi.la/post/26932594.html#cho'gath",
+    'https://nozomi.la/post/25802243.html#nautilus'
+]
+
+# Retrieve all of the post metadata using the URLs
+posts = api.get_posts(urls)
+
+# Download the posts
+for post in posts:
+    api.download_media(post, Path.cwd())
+```
+
+Retrieve and download all posts containing certain tags
+
+```python
+# The tags that the posts retrieved must contain
+positive_tags = ['veigar', 'wallpaper']
+
+# Gets all posts with the tags 'veigar', 'wallpaper'
+for post in api.get_posts_with_tags(positive_tags):
+    api.download_media(post, Path.cwd())
+```
+
+Retrieve all posts containing certain tags, ignoring blacklisted tags
+
+```python
+# The blacklisted tags
+negative_tags = ['chogath']
+
+# Gets all posts with the tags 'veigar' and 'wallpaper' without the 'chogath' tag.
+for post in api.get_posts_with_tags(positive_tags, negative_tags):
+    api.download_media(post, Path.cwd())
+```
```

### Comparing `python-nozomi-1.2.0/README.md` & `python-nozomi-2.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,85 @@
 # python-nozomi
+
 [![Build Status](https://travis-ci.com/Alfa-Q/python-nozomi.svg?token=NAcpuTjLC6CrUpWrqz9p&branch=master)](https://travis-ci.com/Alfa-Q/python-nozomi)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/f3bffdff70794c5cb569645b60699e0b)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Alfa-Q/python-nozomi&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/20c7f3716811466c9e2d55786885951e)](https://app.codacy.com/gh/Alfa-Q/python-nozomi/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/20c7f3716811466c9e2d55786885951e)](https://app.codacy.com/gh/Alfa-Q/python-nozomi/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 [![PyPI version](https://badge.fury.io/py/python-nozomi.svg)](https://badge.fury.io/py/python-nozomi)
-[![Python version](https://img.shields.io/badge/python-%203.7%20%7C%203.8-green)](https://www.python.org/downloads/release/python-360/)
+[![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-green)](https://www.python.org/downloads/release/python-370/)
 
 nozomi.la API in Python.
 
 ## Features
--   Retrieving image and video posts
--   Downloading posts
+
+- Retrieving media posts
+- Downloading media
 
 ## Installation
+
 ```
 $ pip install python-nozomi
 ```
 
+## Upgrade
+
+```
+$ pip install python-nozomi --upgrade
+```
+
 ## Example Usage
-Retrieve and download all posts containing certain tags
+
+Retrieve and download a single post provided a URL
+
 ```python
 from pathlib import Path
 from nozomi import api
-    
+
+url = 'https://nozomi.la/post/26905532.html#veigar'
+
+# Retrieve post metadata using the URL
+post = api.get_post(url)
+
+# Download the post
+api.download_media(post, Path.cwd())
+```
+
+Retrieve and download multiple posts provided a list of URLs
+
+```python
+from pathlib import Path
+from nozomi import api
+
+urls = [
+    'https://nozomi.la/post/26905532.html#veigar',
+    "https://nozomi.la/post/26932594.html#cho'gath",
+    'https://nozomi.la/post/25802243.html#nautilus'
+]
+
+# Retrieve all of the post metadata using the URLs
+posts = api.get_posts(urls)
+
+# Download the posts
+for post in posts:
+    api.download_media(post, Path.cwd())
+```
+
+Retrieve and download all posts containing certain tags
+
+```python
 # The tags that the posts retrieved must contain
 positive_tags = ['veigar', 'wallpaper']
 
 # Gets all posts with the tags 'veigar', 'wallpaper'
-for post in api.get_posts(positive_tags):
+for post in api.get_posts_with_tags(positive_tags):
     api.download_media(post, Path.cwd())
 ```
 
-Retrieve all posts containing certain tags with blacklisted tags
+Retrieve all posts containing certain tags, ignoring blacklisted tags
+
 ```python
 # The blacklisted tags
 negative_tags = ['chogath']
 
-# Gets all posts with the tags 'veigar', 'wallpaper' but no 'chogath' tag.
-for post in api.get_posts(positive_tags, negative_tags):
+# Gets all posts with the tags 'veigar' and 'wallpaper' without the 'chogath' tag.
+for post in api.get_posts_with_tags(positive_tags, negative_tags):
     api.download_media(post, Path.cwd())
 ```
```

### Comparing `python-nozomi-1.2.0/nozomi/api.py` & `python-nozomi-2.0.0/nozomi/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def get_post(url: str) -> Post:
     """Retrieve a single post.
 
     Args:
         url: The URL of the post to retrieve.
 
     Returns:
-        A post in JSON format if it exists.
+        Post metadata information.
 
     """
     _LOGGER.debug('Retrieving a post from URL "%s"', url)
     try:
         post_id = parse_post_id(url)
         post_url = create_post_filepath(post_id)
         post_data = requests.get(post_url).json()
@@ -37,15 +37,29 @@
     except InvalidUrlFormat:
         raise
     except Exception as ex:
         _LOGGER.exception(ex)
         raise
 
 
-def get_posts(positive_tags: List[str], negative_tags: List[str]=None) -> Iterable[Post]:
+def get_posts(urls: List[str]) -> Iterable[Post]:
+    """Retrieves multiple posts.
+
+    Args:
+        urls: The URLs of the posts to retrieve.
+
+    Yields:
+        Post metadata information.
+ 
+    """
+    for url in urls:
+        yield get_post(url)
+
+
+def get_posts_with_tags(positive_tags: List[str], negative_tags: List[str] = None) -> Iterable[Post]:
     """Retrieve all post data that contains and doesn't contain certain tags.
 
     Args:
         positive_tags: The tags that the posts retrieved must contain.
         negative_tags: Optional, blacklisted tags.
 
     Yields:
@@ -83,44 +97,37 @@
     Returns:
         The names of the images downloaded.
 
     """
     images_downloaded = []
     filepath.mkdir(parents=True, exist_ok=True)
     for media_meta_data in post.imageurls:
-        image_url = media_meta_data.imageurl
-        image_name = image_url.split('/')[-1]
-        image_filepath = filepath.joinpath(image_name)
-        _download_media(image_url, image_filepath)
-        images_downloaded.append(image_name)
+        filename = f'{media_meta_data.dataid}.{media_meta_data.type}'
+        image_filepath = filepath.joinpath(filename)
+        _download_media(media_meta_data.imageurl, image_filepath)
+        images_downloaded.append(filename)
     return images_downloaded
 
 
 def _download_media(image_url: str, filepath: Path):
     """Download an image and save it.
 
     Args:
         image_url: The image URL.
         filepath: The file directory to save the media. The directory will be created if it doesn't
             already exist.
 
     """
     headers = {
-        'Host': 'i.nozomi.la',
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:69.0) Gecko/20100101 Firefox/69.0',
-        'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,/;q=0.8',
-        'Accept-Language': 'en-US,en;q=0.5',
+        'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
+        'Accept-Language': 'en-US,en;q=0.9',
         'Accept-Encoding': 'gzip, deflate, br',
-        'DNT': '1',
-        'Connection': 'keep-alive',
         'Referer': 'https://nozomi.la/',
-        'Upgrade-Insecure-Requests': '1',
-        'TE': 'Trailers',
-        'Pragma': 'no-cache',
-        'Cache-Control': 'no-cache'
+        'Upgrade-Insecure-Requests': '1'
     }
     with requests.get(image_url, stream=True, headers=headers) as r:
         with open(filepath, 'wb') as f:
             shutil.copyfileobj(r.raw, f)
     _LOGGER.debug('Image downloaded %s', filepath)
 
 
@@ -130,15 +137,16 @@
     Args:
         tags: The tags that the posts must contain.
 
     Returns:
         A list of post urls that contain all of the specified tags.
 
     """
-    if len(tags) == 0: return tags
+    if len(tags) == 0:
+        return tags
     _LOGGER.debug('Retrieving all URLs that contain the tags %s', str(tags))
     sanitized_tags = [sanitize_tag(tag) for tag in tags]
     nozomi_urls  = [create_tag_filepath(sanitized_tag) for sanitized_tag in sanitized_tags]
     tag_post_ids = [_get_post_ids(nozomi_url) for nozomi_url in nozomi_urls]
     tag_post_ids = set.intersection(*map(set, tag_post_ids)) # Flatten list of tuples on intersection
     post_urls = [create_post_filepath(post_id) for post_id in tag_post_ids]
     _LOGGER.debug('Got %d post urls containing the tags %s', len(tags), str(tags))
```

### Comparing `python-nozomi-1.2.0/nozomi/data.py` & `python-nozomi-2.0.0/nozomi/data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 """Represents nozomi dataclasses."""
 
 from typing import List, Optional
 from dataclasses import dataclass, field
 
+from nozomi.helpers import create_media_filepath
+
 
 @dataclass(frozen=True)
 class MediaMetaData:
     """Metadata for a media file (i.e. an Image, Video, GIF).
 
     Args:
         is_video (str): Whether the media is a video type.
-        imageurl (str): Url to the media file.
+        type (str): Filetype of the media. This may different from the url type.
+        dataid (str): Hash of the media file.
+        width (int): Width of the media file.
+        height (int): Height of the media file.
 
     """
 
     is_video:   str
-    imageurl:   str
+    type:       str
+    dataid:     str
+    imageurl:   str = field(init=False)
+    width:      int
+    height:     int
 
     def __post_init__(self):
         """Calculate fields after the object is initialized."""
-        new_imageurl = 'https:' + self.imageurl
+        imageurl = create_media_filepath(self)
         # Set the tag without raising a FrozenClass error.
-        object.__setattr__(self, 'imageurl', new_imageurl)
+        object.__setattr__(self, 'imageurl', imageurl)
 
 
 @dataclass(frozen=True)
 class Tag:
     """Tag information.
 
     Args:
@@ -52,38 +61,25 @@
         object.__setattr__(self, 'sanitized_tag', sanitized_tag)
 
 
 @dataclass(frozen=True)
 class Post(MediaMetaData):
     """Post information.
 
-    Some of the fields seem rather redundant. For example, there is the field 'imageurls' but
-    there will only ever be one imageurl.
-
     Args:
-        width (int): Width of the media file.
-        favorites (int): Total number of favorites.
-        source (str): Site name where the media was taken from.
-        date (str): #TODO: Determine if the date is the date that the post was uploaded
-        height (int): Height of the media file.
-        sourceid (int): #TODO: Figure out what this is.
+        date (str): The date that the post was uploaded on.
         postid (int): The unique ID of the post.
-        dataid (str): #TODO: Figure out what this is.
         general (List[Tag]): A list of the general tags that describe the post.
         copyright (List[Tag]): The various series that the media is based on.
         character (List[Tag]): The characters that are featured in the post.
         artist (List[Tag]): The artists that create the media.
         imageurls (List[MediaMetaData]): The media featured in the post.
 
     """
 
-    width:      int
-    source:     str
     date:       str
-    height:     int
     postid:     int
-    dataid:     str
-    general:    List[Tag]           = field(default_factory=list)
-    copyright:  List[Tag]           = field(default_factory=list)
-    character:  List[Tag]           = field(default_factory=list)
-    artist:     List[Tag]           = field(default_factory=list)
+    general:    List[Tag] = field(default_factory=list)
+    copyright:  List[Tag] = field(default_factory=list)
+    character:  List[Tag] = field(default_factory=list)
+    artist:     List[Tag] = field(default_factory=list)
     imageurls:  List[MediaMetaData] = field(default_factory=list)
```

### Comparing `python-nozomi-1.2.0/nozomi/helpers.py` & `python-nozomi-2.0.0/nozomi/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,24 @@
 If this package grows more complex, the functionality can be divided in a more manner. Due to
 the simplicity of the current API, there isn't really a point right now.
 
 """
 
 import re
 import logging
+from typing import ForwardRef
 
 from nozomi.exceptions import InvalidTagFormat, InvalidUrlFormat
 
 
 _LOGGER = logging.getLogger(__name__)
 
+# Prevent circular dependency issues
+MediaMetaData = ForwardRef("MediaMetaData")
+
 
 def sanitize_tag(tag: str) -> str:
     """Remove and replace any invalid characters in the tag.
 
     Args:
         tag: The search tag.
 
@@ -62,14 +66,39 @@
     except AttributeError:
         raise InvalidUrlFormat('The provided URL %s could not be parsed.', url)
     except Exception as ex:
         _LOGGER.exception(ex)
     return post_id
 
 
+def create_media_filepath(media: MediaMetaData) -> str:
+    """Build the path to media on the site.
+
+    Args:
+        media: The media on a post.
+
+    Returns:
+        The URL of the a post's media.
+
+    """
+    if media.is_video:
+        subdomain = 'v'
+        url_type = media.type
+    elif media.type == 'gif':
+        subdomain = 'g'
+        url_type = 'gif'
+    else:
+        subdomain = 'w'
+        url_type = 'webp'
+    path = _calculate_post_filepath(media.dataid)
+    url_fmt = 'https://{subdomain}.nozomi.la/{hashed_path}.{url_type}'
+    url = url_fmt.format(subdomain=subdomain, hashed_path=path, url_type=url_type)
+    return url
+
+
 def create_tag_filepath(sanitized_tag: str) -> str:
     """Build the path to a .nozomi file for a particular tag.
 
     Every search tag/term has an associated .nozomi file stored in the database. Each file contains
     references to data that is related to the tag. This function builds the path to that file.
 
     Args:
@@ -94,32 +123,47 @@
 
 
 def create_post_filepath(post_id: int) -> str:
     """Build the path to a post's JSON file.
 
     The rules for creating the filepath can be found in the site's javascript file. They appear to
     be arbitrary decisions. The JSON file for the post contains a variety of useful data including
-    image data, popularity, tags, etc.
+    image data, tags, etc.
 
     Args:
         post_id: The ID of a post on the website.
 
     Returns:
         The URL of the post's associated JSON file.
 
     """
     _LOGGER.info("Creating tag filepath for post ID %d", post_id)
     post_id = str(post_id)
-    if len(post_id) < 3:
-        path = post_id
-    else:
-        path = re.sub('^.*(..)(.)$', r'\g<2>/\g<1>/' + post_id, post_id)
+    path = _calculate_post_filepath(post_id)
     return f'https://j.nozomi.la/post/{path}.json'
 
 
+def _calculate_post_filepath(id: str) -> str:
+    """Calculate the filepath for data on a post.
+
+    Args:
+        id: Hash of a media file or the post id.
+
+    Returns:
+        The URL path of a post's associated file.
+
+    """
+    _LOGGER.debug("Calculating the filepath of some file for a post '%s'", id)
+    if len(id) < 3:
+        path = id
+    else:
+        path = re.sub('^.*(..)(.)$', r'\g<2>/\g<1>/' + id, id)
+    return path
+
+
 def _validate_tag_sanitized(tag: str) -> None:
     """Validate a search tag is sanitized properly.
 
     Args:
         tag: The search tag.
 
     Raises:
```

### Comparing `python-nozomi-1.2.0/python_nozomi.egg-info/PKG-INFO` & `python-nozomi-2.0.0/python_nozomi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,109 @@
 Metadata-Version: 2.1
 Name: python-nozomi
-Version: 1.2.0
+Version: 2.0.0
 Summary: Nozomi API for retrieving images, videos, gifs.
 Home-page: https://github.com/Alfa-Q/python-nozomi
+Download-URL: https://github.com/Alfa-Q/python-nozomi/archive/2.0.0.tar.gz
 Author: Alfa_Q
 Author-email: alfakyuu@gmail.com
 License: MIT
-Download-URL: https://github.com/Alfa-Q/python-nozomi/archive/1.1.1.tar.gz
-Description: # python-nozomi
-        [![Build Status](https://travis-ci.com/Alfa-Q/python-nozomi.svg?token=NAcpuTjLC6CrUpWrqz9p&branch=master)](https://travis-ci.com/Alfa-Q/python-nozomi)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/f3bffdff70794c5cb569645b60699e0b)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Alfa-Q/python-nozomi&amp;utm_campaign=Badge_Grade)
-        [![PyPI version](https://badge.fury.io/py/python-nozomi.svg)](https://badge.fury.io/py/python-nozomi)
-        [![Python version](https://img.shields.io/badge/python-%203.7%20%7C%203.8-green)](https://www.python.org/downloads/release/python-360/)
-        
-        nozomi.la API in Python.
-        
-        ## Features
-        -   Retrieving image and video posts
-        -   Downloading posts
-        
-        ## Installation
-        ```
-        $ pip install python-nozomi
-        ```
-        
-        ## Example Usage
-        Retrieve and download all posts containing certain tags
-        ```python
-        from pathlib import Path
-        from nozomi import api
-            
-        # The tags that the posts retrieved must contain
-        positive_tags = ['veigar', 'wallpaper']
-        
-        # Gets all posts with the tags 'veigar', 'wallpaper'
-        for post in api.get_posts(positive_tags):
-            api.download_media(post, Path.cwd())
-        ```
-        
-        Retrieve all posts containing certain tags with blacklisted tags
-        ```python
-        # The blacklisted tags
-        negative_tags = ['chogath']
-        
-        # Gets all posts with the tags 'veigar', 'wallpaper' but no 'chogath' tag.
-        for post in api.get_posts(positive_tags, negative_tags):
-            api.download_media(post, Path.cwd())
-        ```
-        
 Keywords: nozomi,nozomi.la,api,video,image,anime
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# python-nozomi
+
+[![Build Status](https://travis-ci.com/Alfa-Q/python-nozomi.svg?token=NAcpuTjLC6CrUpWrqz9p&branch=master)](https://travis-ci.com/Alfa-Q/python-nozomi)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/20c7f3716811466c9e2d55786885951e)](https://app.codacy.com/gh/Alfa-Q/python-nozomi/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/20c7f3716811466c9e2d55786885951e)](https://app.codacy.com/gh/Alfa-Q/python-nozomi/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+[![PyPI version](https://badge.fury.io/py/python-nozomi.svg)](https://badge.fury.io/py/python-nozomi)
+[![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-green)](https://www.python.org/downloads/release/python-370/)
+
+nozomi.la API in Python.
+
+## Features
+
+- Retrieving media posts
+- Downloading media
+
+## Installation
+
+```
+$ pip install python-nozomi
+```
+
+## Upgrade
+
+```
+$ pip install python-nozomi --upgrade
+```
+
+## Example Usage
+
+Retrieve and download a single post provided a URL
+
+```python
+from pathlib import Path
+from nozomi import api
+
+url = 'https://nozomi.la/post/26905532.html#veigar'
+
+# Retrieve post metadata using the URL
+post = api.get_post(url)
+
+# Download the post
+api.download_media(post, Path.cwd())
+```
+
+Retrieve and download multiple posts provided a list of URLs
+
+```python
+from pathlib import Path
+from nozomi import api
+
+urls = [
+    'https://nozomi.la/post/26905532.html#veigar',
+    "https://nozomi.la/post/26932594.html#cho'gath",
+    'https://nozomi.la/post/25802243.html#nautilus'
+]
+
+# Retrieve all of the post metadata using the URLs
+posts = api.get_posts(urls)
+
+# Download the posts
+for post in posts:
+    api.download_media(post, Path.cwd())
+```
+
+Retrieve and download all posts containing certain tags
+
+```python
+# The tags that the posts retrieved must contain
+positive_tags = ['veigar', 'wallpaper']
+
+# Gets all posts with the tags 'veigar', 'wallpaper'
+for post in api.get_posts_with_tags(positive_tags):
+    api.download_media(post, Path.cwd())
+```
+
+Retrieve all posts containing certain tags, ignoring blacklisted tags
+
+```python
+# The blacklisted tags
+negative_tags = ['chogath']
+
+# Gets all posts with the tags 'veigar' and 'wallpaper' without the 'chogath' tag.
+for post in api.get_posts_with_tags(positive_tags, negative_tags):
+    api.download_media(post, Path.cwd())
+```
```

### Comparing `python-nozomi-1.2.0/setup.py` & `python-nozomi-2.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,39 @@
 
 from setuptools import setup
 
 
 setup(
     name='python-nozomi',
     packages=['nozomi'],
-    version='1.2.0',
+    version='2.0.0',
     license='MIT',
     description='Nozomi API for retrieving images, videos, gifs.',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Alfa_Q',
     author_email='alfakyuu@gmail.com',
     url='https://github.com/Alfa-Q/python-nozomi',
-    download_url='https://github.com/Alfa-Q/python-nozomi/archive/1.1.1.tar.gz',
+    download_url='https://github.com/Alfa-Q/python-nozomi/archive/2.0.0.tar.gz',
     keywords=['nozomi', 'nozomi.la', 'api', 'video', 'image', 'anime'],
     install_requires=[
         'requests',
         'dacite',
     ],
+    extras_require={
+        'dev': [
+            'pytest'
+        ]
+    },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
+    python_requires=">=3.7"
 )
```

