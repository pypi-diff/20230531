# Comparing `tmp/sankaku-1.0.1.tar.gz` & `tmp/sankaku-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sankaku-1.0.1.tar", last modified: Wed May 17 15:20:07 2023, max compression
+gzip compressed data, was "sankaku-1.0.2.tar", last modified: Wed May 31 04:28:53 2023, max compression
```

## Comparing `sankaku-1.0.1.tar` & `sankaku-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.866396 sankaku-1.0.1/
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1064 2023-05-15 12:04:32.000000 sankaku-1.0.1/LICENSE
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2948 2023-05-17 15:20:07.866396 sankaku-1.0.1/PKG-INFO
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2388 2023-05-17 15:02:34.000000 sankaku-1.0.1/README.md
--rw-r--r--   0 moldus    (1000) moldus    (1000)       81 2023-05-15 15:32:11.000000 sankaku-1.0.1/pyproject.toml
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.863396 sankaku-1.0.1/sankaku/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      120 2023-05-10 14:37:51.000000 sankaku-1.0.1/sankaku/__init__.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.864396 sankaku-1.0.1/sankaku/clients/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      351 2023-05-16 19:34:35.000000 sankaku-1.0.1/sankaku/clients/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1222 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/clients/abc.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)    15150 2023-05-17 14:47:16.000000 sankaku-1.0.1/sankaku/clients/clients.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1998 2023-05-15 10:39:52.000000 sankaku-1.0.1/sankaku/clients/http_client.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1285 2023-05-15 10:30:11.000000 sankaku-1.0.1/sankaku/constants.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1748 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/errors.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.865396 sankaku-1.0.1/sankaku/models/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      104 2023-05-14 06:27:00.000000 sankaku-1.0.1/sankaku/models/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1900 2023-05-15 09:27:13.000000 sankaku-1.0.1/sankaku/models/books.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      367 2023-05-15 09:37:39.000000 sankaku-1.0.1/sankaku/models/http.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      263 2023-05-15 09:37:39.000000 sankaku-1.0.1/sankaku/models/pages.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3466 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/models/posts.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3975 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/models/tags.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2131 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/models/users.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.866396 sankaku-1.0.1/sankaku/paginators/
--rw-r--r--   0 moldus    (1000) moldus    (1000)       26 2023-05-13 09:01:36.000000 sankaku-1.0.1/sankaku/paginators/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      857 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/paginators/abc.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)    10342 2023-05-15 10:29:22.000000 sankaku-1.0.1/sankaku/paginators/paginators.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      265 2023-05-15 10:29:01.000000 sankaku-1.0.1/sankaku/typedefs.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1986 2023-05-15 09:54:46.000000 sankaku-1.0.1/sankaku/types.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1905 2023-05-17 14:50:40.000000 sankaku-1.0.1/sankaku/utils.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-17 15:20:07.863396 sankaku-1.0.1/sankaku.egg-info/
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2948 2023-05-17 15:20:06.000000 sankaku-1.0.1/sankaku.egg-info/PKG-INFO
--rw-r--r--   0 moldus    (1000) moldus    (1000)      676 2023-05-17 15:20:07.000000 sankaku-1.0.1/sankaku.egg-info/SOURCES.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)        1 2023-05-17 15:20:07.000000 sankaku-1.0.1/sankaku.egg-info/dependency_links.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)       24 2023-05-17 15:20:07.000000 sankaku-1.0.1/sankaku.egg-info/requires.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)        8 2023-05-17 15:20:07.000000 sankaku-1.0.1/sankaku.egg-info/top_level.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)       38 2023-05-17 15:20:07.866396 sankaku-1.0.1/setup.cfg
--rw-r--r--   0 moldus    (1000) moldus    (1000)      847 2023-05-17 15:14:00.000000 sankaku-1.0.1/setup.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.115640 sankaku-1.0.2/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1064 2023-05-15 12:04:32.000000 sankaku-1.0.2/LICENSE
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       90 2023-05-31 03:19:49.000000 sankaku-1.0.2/MANIFEST.in
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3250 2023-05-31 04:28:53.115640 sankaku-1.0.2/PKG-INFO
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2447 2023-05-31 03:56:32.000000 sankaku-1.0.2/README.md
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       81 2023-05-15 15:32:11.000000 sankaku-1.0.2/pyproject.toml
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       13 2023-05-31 03:19:49.000000 sankaku-1.0.2/requirements-socks.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      126 2023-05-31 03:19:49.000000 sankaku-1.0.2/requirements-test.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       79 2023-05-31 03:19:49.000000 sankaku-1.0.2/requirements.txt
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.112640 sankaku-1.0.2/sankaku/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      120 2023-05-29 15:50:51.000000 sankaku-1.0.2/sankaku/__init__.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.113641 sankaku-1.0.2/sankaku/clients/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      351 2023-05-16 19:34:35.000000 sankaku-1.0.2/sankaku/clients/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1228 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/clients/abc.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)    15472 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/clients/clients.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3258 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/clients/http_client.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1325 2023-05-31 03:19:49.000000 sankaku-1.0.2/sankaku/constants.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1748 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/errors.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.114641 sankaku-1.0.2/sankaku/models/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      104 2023-05-14 06:27:00.000000 sankaku-1.0.2/sankaku/models/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1906 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/books.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      367 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/http.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      268 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/pages.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3464 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/posts.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     4250 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/tags.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2137 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/models/users.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.115640 sankaku-1.0.2/sankaku/paginators/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       26 2023-05-13 09:01:36.000000 sankaku-1.0.2/sankaku/paginators/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      829 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/paginators/abc.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)    10560 2023-05-31 04:05:29.000000 sankaku-1.0.2/sankaku/paginators/paginators.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      380 2023-05-31 04:05:29.000000 sankaku-1.0.2/sankaku/typedefs.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1986 2023-05-31 04:15:17.000000 sankaku-1.0.2/sankaku/types.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2049 2023-05-31 04:17:38.000000 sankaku-1.0.2/sankaku/utils.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-05-31 04:28:53.113641 sankaku-1.0.2/sankaku.egg-info/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3250 2023-05-31 04:28:52.000000 sankaku-1.0.2/sankaku.egg-info/PKG-INFO
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      750 2023-05-31 04:28:53.000000 sankaku-1.0.2/sankaku.egg-info/SOURCES.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)        1 2023-05-31 04:28:52.000000 sankaku-1.0.2/sankaku.egg-info/dependency_links.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      241 2023-05-31 04:28:52.000000 sankaku-1.0.2/sankaku.egg-info/requires.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)        8 2023-05-31 04:28:52.000000 sankaku-1.0.2/sankaku.egg-info/top_level.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       38 2023-05-31 04:28:53.115640 sankaku-1.0.2/setup.cfg
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1631 2023-05-31 04:26:03.000000 sankaku-1.0.2/setup.py
```

### Comparing `sankaku-1.0.1/LICENSE` & `sankaku-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.1/PKG-INFO` & `sankaku-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: sankaku
-Version: 1.0.1
+Version: 1.0.2
 Summary: Asynchronous API wrapper for Sankaku Complex.
 Home-page: https://github.com/zerex290/sankaku
 Author: zerex290
 Author-email: zerex290@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/zerex290/sankaku/issues
 Keywords: sankaku,sankakucomplex,api
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: socks
+Provides-Extra: test
 License-File: LICENSE
 
 <h1 align="center">
   <a href="https://github.com/zerex290/sankaku">
     <img src="https://raw.githubusercontent.com/zerex290/sankaku/main/docs/icon.png" alt="Sankaku Complex"
     width="150" height="150"/>
   </a>
@@ -45,18 +51,20 @@
 
 Source code: https://github.com/zerex290/sankaku
 
 ---
 
 ## Requirements
 
-- Python 3.11+
+- Python 3.7+
 - aiohttp
 - pydantic
 - loguru
+- aiohttp-retry
+- typing_extensions; python_version < '3.9'
 
 ## Installation
 
 To install sankaku via pip write following line of code in your terminal:
 
 ```commandline
 pip install sankaku
```

#### html2text {}

```diff
@@ -1,38 +1,42 @@
-Metadata-Version: 2.1 Name: sankaku Version: 1.0.1 Summary: Asynchronous API
+Metadata-Version: 2.1 Name: sankaku Version: 1.0.2 Summary: Asynchronous API
 wrapper for Sankaku Complex. Home-page: https://github.com/zerex290/sankaku
 Author: zerex290 Author-email: zerex290@gmail.com License: MIT Project-URL:
 Issue Tracker, https://github.com/zerex290/sankaku/issues Keywords:
-sankaku,sankakucomplex,api Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
-markdown License-File: LICENSE
+sankaku,sankakucomplex,api Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+socks Provides-Extra: test License-File: LICENSE
                                [Sankaku_Complex]
                                     sankaku
                             For real men of culture
 ## About Asynchronous API wrapper for [Sankaku Complex](https://
 beta.sankakucomplex.com) with *type-hinting*, pydantic *data validation* and an
 optional *logging support* with loguru. ### Features: - Type-hints -
 Deserialization of raw json data thanks to pydantic models - Enumerations for
 API request parameters to provide better user experience > For instance, you
 can type `types.TagType.ARTIST` instead of `types[]=1` --- Documentation:
 https://zerex290.github.io/sankaku API Reference: https://zerex290.github.io/
 sankaku/api Source code: https://github.com/zerex290/sankaku --- ##
-Requirements - Python 3.11+ - aiohttp - pydantic - loguru ## Installation To
-install sankaku via pip write following line of code in your terminal:
-```commandline pip install sankaku ``` To install the sankaku via Docker, you
-can follow these steps: ###### Step 1: Install Docker Ensure that Docker is
-installed on your machine. If Docker is not already installed, you can download
-and install it from the official [Docker website](https://www.docker.com/get-
-started). ###### Step 2: Use docker to install sankaku Open a command prompt.
-Navigate to the directory where you want to install Sankaku. Type the following
-command: ```commandline git clone https://github.com/zerex290/sankaku.git cd
-sankaku docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash
-``` ## Usage example It's very simple to use and doesn't require to always keep
-opened browser page with documentation because all methods are self-
-explanatory: ```py import asyncio from sankaku import SankakuClient async def
-main(): client = SankakuClient() post = await client.get_post(25742064) print
-(f"Rating: {post.rating} | Created: {post.created_at}") # "Rating:
-Rating.QUESTIONABLE | Created: 2021-08-01 23:18:52+03:00" await client.login
-(access_token="token") # Or you can authorize by credentials: # await
-client.login(login="nickname or email", password="password") async for book in
-client.get_recently_read_books(): ... asyncio.run(main()) ```
+Requirements - Python 3.7+ - aiohttp - pydantic - loguru - aiohttp-retry -
+typing_extensions; python_version < '3.9' ## Installation To install sankaku
+via pip write following line of code in your terminal: ```commandline pip
+install sankaku ``` To install the sankaku via Docker, you can follow these
+steps: ###### Step 1: Install Docker Ensure that Docker is installed on your
+machine. If Docker is not already installed, you can download and install it
+from the official [Docker website](https://www.docker.com/get-started). ######
+Step 2: Use docker to install sankaku Open a command prompt. Navigate to the
+directory where you want to install Sankaku. Type the following command:
+```commandline git clone https://github.com/zerex290/sankaku.git cd sankaku
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash ``` ##
+Usage example It's very simple to use and doesn't require to always keep opened
+browser page with documentation because all methods are self-explanatory: ```py
+import asyncio from sankaku import SankakuClient async def main(): client =
+SankakuClient() post = await client.get_post(25742064) print(f"Rating:
+{post.rating} | Created: {post.created_at}") # "Rating: Rating.QUESTIONABLE |
+Created: 2021-08-01 23:18:52+03:00" await client.login(access_token="token") #
+Or you can authorize by credentials: # await client.login(login="nickname or
+email", password="password") async for book in client.get_recently_read_books
+(): ... asyncio.run(main()) ```
```

### Comparing `sankaku-1.0.1/README.md` & `sankaku-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 
 Source code: https://github.com/zerex290/sankaku
 
 ---
 
 ## Requirements
 
-- Python 3.11+
+- Python 3.7+
 - aiohttp
 - pydantic
 - loguru
+- aiohttp-retry
+- typing_extensions; python_version < '3.9'
 
 ## Installation
 
 To install sankaku via pip write following line of code in your terminal:
 
 ```commandline
 pip install sankaku
```

#### html2text {}

```diff
@@ -5,26 +5,27 @@
 beta.sankakucomplex.com) with *type-hinting*, pydantic *data validation* and an
 optional *logging support* with loguru. ### Features: - Type-hints -
 Deserialization of raw json data thanks to pydantic models - Enumerations for
 API request parameters to provide better user experience > For instance, you
 can type `types.TagType.ARTIST` instead of `types[]=1` --- Documentation:
 https://zerex290.github.io/sankaku API Reference: https://zerex290.github.io/
 sankaku/api Source code: https://github.com/zerex290/sankaku --- ##
-Requirements - Python 3.11+ - aiohttp - pydantic - loguru ## Installation To
-install sankaku via pip write following line of code in your terminal:
-```commandline pip install sankaku ``` To install the sankaku via Docker, you
-can follow these steps: ###### Step 1: Install Docker Ensure that Docker is
-installed on your machine. If Docker is not already installed, you can download
-and install it from the official [Docker website](https://www.docker.com/get-
-started). ###### Step 2: Use docker to install sankaku Open a command prompt.
-Navigate to the directory where you want to install Sankaku. Type the following
-command: ```commandline git clone https://github.com/zerex290/sankaku.git cd
-sankaku docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash
-``` ## Usage example It's very simple to use and doesn't require to always keep
-opened browser page with documentation because all methods are self-
-explanatory: ```py import asyncio from sankaku import SankakuClient async def
-main(): client = SankakuClient() post = await client.get_post(25742064) print
-(f"Rating: {post.rating} | Created: {post.created_at}") # "Rating:
-Rating.QUESTIONABLE | Created: 2021-08-01 23:18:52+03:00" await client.login
-(access_token="token") # Or you can authorize by credentials: # await
-client.login(login="nickname or email", password="password") async for book in
-client.get_recently_read_books(): ... asyncio.run(main()) ```
+Requirements - Python 3.7+ - aiohttp - pydantic - loguru - aiohttp-retry -
+typing_extensions; python_version < '3.9' ## Installation To install sankaku
+via pip write following line of code in your terminal: ```commandline pip
+install sankaku ``` To install the sankaku via Docker, you can follow these
+steps: ###### Step 1: Install Docker Ensure that Docker is installed on your
+machine. If Docker is not already installed, you can download and install it
+from the official [Docker website](https://www.docker.com/get-started). ######
+Step 2: Use docker to install sankaku Open a command prompt. Navigate to the
+directory where you want to install Sankaku. Type the following command:
+```commandline git clone https://github.com/zerex290/sankaku.git cd sankaku
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash ``` ##
+Usage example It's very simple to use and doesn't require to always keep opened
+browser page with documentation because all methods are self-explanatory: ```py
+import asyncio from sankaku import SankakuClient async def main(): client =
+SankakuClient() post = await client.get_post(25742064) print(f"Rating:
+{post.rating} | Created: {post.created_at}") # "Rating: Rating.QUESTIONABLE |
+Created: 2021-08-01 23:18:52+03:00" await client.login(access_token="token") #
+Or you can authorize by credentials: # await client.login(login="nickname or
+email", password="password") async for book in client.get_recently_read_books
+(): ... asyncio.run(main()) ```
```

### Comparing `sankaku-1.0.1/sankaku/clients/abc.py` & `sankaku-1.0.2/sankaku/clients/abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from abc import ABC, abstractmethod
-from typing import Optional, Self
+from typing import Optional
 
 from sankaku.models.http import ClientResponse
 
 
 __all__ = ["ABCHttpClient", "ABCClient"]
 
 
 class ABCHttpClient(ABC):
     """Abstract client for handling http requests."""
     @abstractmethod
     def __init__(self, *args, **kwargs) -> None:
         pass
 
-    async def __aenter__(self) -> Self:
+    async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         await self.close()
 
     @abstractmethod
     def __del__(self) -> None:
@@ -36,14 +36,14 @@
     """Abstract Sankaku client."""
     @abstractmethod
     def __init__(self, *args, **kwargs) -> None:
         pass
 
     @abstractmethod
     async def login(
-        self,
-        *,
-        access_token: Optional[str] = None,
-        login: Optional[str] = None,
-        password: Optional[str] = None
+            self,
+            *,
+            access_token: Optional[str] = None,
+            login: Optional[str] = None,
+            password: Optional[str] = None
     ) -> None:
         """Login into sankakucomplex.com via access token or credentials."""
```

### Comparing `sankaku-1.0.1/sankaku/clients/clients.py` & `sankaku-1.0.2/sankaku/clients/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import json
-from typing import Optional, Literal, Annotated
-from collections.abc import AsyncIterator
 from datetime import datetime
+from typing import Optional, Union, List, AsyncIterator
+
+try:
+    from typing import Literal, Annotated
+except (ModuleNotFoundError, ImportError):
+    from typing_extensions import Literal, Annotated  # type: ignore[assignment]
 
 from loguru import logger
 
-from .abc import ABCClient
-from .http_client import HttpClient
-from sankaku.typedefs import ValueRange
-from sankaku.utils import from_locals
 from sankaku import models as mdl, constants as const, types, errors
 from sankaku.paginators import *
+from sankaku.utils import from_locals
+from sankaku.typedefs import ValueRange
+from .abc import ABCClient
+from .http_client import HttpClient
 
 
 __all__ = [
     "PostClient",
     "AIClient",
     "TagClient",
     "BookClient",
@@ -65,70 +69,69 @@
             raise errors.SankakuServerError(
                 response.status, "Failed to get user profile", **response.json
             )
 
         return mdl.ExtendedUser(**response.json["user"])
 
     async def login(
-        self,
-        *,
-        access_token: Optional[str] = None,
-        login: Optional[str] = None,
-        password: Optional[str] = None
+            self,
+            *,
+            access_token: Optional[str] = None,
+            login: Optional[str] = None,
+            password: Optional[str] = None
     ) -> None:
         """Login into sankakucomplex.com via access token or credentials.
         In case when all arguments are specified, preference will be given
         to authorization by credentials.
 
         Args:
             access_token: User access token
             login: User email or nickname
             password: User password
         """
-        match (access_token, login, password):
-            case [str(), str(), str()] | [_, str(), str()]:
-                await self._login_via_credentials(login, password)  # type: ignore[arg-type]
-            case [str(), _, _]:
-                await self._login_via_access_token(access_token)  # type: ignore[arg-type]
-            case _:
-                raise errors.SankakuError(
-                    "The given data is not enough "
-                    "or invalid (perhaps of the wrong type)."
-                )
+        if login and password:
+            await self._login_via_credentials(login, password)  # type: ignore[arg-type]
+        elif access_token and not login and not password:
+            await self._login_via_access_token(access_token)  # type: ignore[arg-type]
+        else:
+            raise errors.SankakuError(
+                "The given data is not enough "
+                "or invalid (perhaps of the wrong type)."
+            )
 
         self._http_client.headers.update(
             authorization=f"{self._token_type} {self._access_token}"
         )
         logger.info(f"Successfully logged in as {self._profile.name}.")  # type: ignore[union-attr]
 
     @property
     def profile(self) -> Optional[mdl.ExtendedUser]:
         return self._profile
 
 
 class PostClient(BaseClient):
     """Client for post browsing."""
     async def browse_posts(
-        self,
-        order: Optional[types.PostOrder] = None,
-        date: Optional[list[datetime]] = None,
-        rating: Optional[types.Rating] = None,
-        threshold: Optional[Annotated[int, ValueRange(1, 100)]] = None,
-        hide_posts_in_books: Optional[Literal["in-larger-tags", "always"]] = None,
-        file_size: Optional[types.FileSize] = None,
-        file_type: Optional[types.FileType] = None,
-        video_duration: Optional[list[int]] = None,
-        recommended_for: Optional[str] = None,
-        favorited_by: Optional[str] = None,
-        tags: Optional[list[str]] = None,
-        added_by: Optional[list[str]] = None,
-        voted: Optional[str] = None,
-        *,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
+            self,
+            order: Optional[types.PostOrder] = None,
+            date: Optional[List[datetime]] = None,
+            rating: Optional[types.Rating] = None,
+            threshold: Optional[Annotated[int, ValueRange(1, 100)]] = None,
+            hide_posts_in_books: Optional[Literal["in-larger-tags", "always"]] = None,
+            file_size: Optional[types.FileSize] = None,
+            file_type: Optional[types.FileType] = None,
+            video_duration: Optional[List[int]] = None,
+            recommended_for: Optional[str] = None,
+            favorited_by: Optional[str] = None,
+            tags: Optional[List[str]] = None,
+            added_by: Optional[List[str]] = None,
+            voted: Optional[str] = None,
+            *,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
 
     ) -> AsyncIterator[mdl.Post]:
         """Get posts from post pages.
 
         Args:
             order: Post order rule
             date: Date or range of dates
@@ -143,15 +146,15 @@
             tags: Tags available for search
             added_by: Posts uploaded by specified users
             voted: Posts voted by specified user
             page_number: Page number from which to start iteration
             limit: Maximum amount of posts per page
         """
         async for page in PostPaginator(
-            self._http_client, const.POST_URL, **from_locals(locals())
+                self._http_client, const.POST_URL, **from_locals(locals())
         ):
             for post in page.items:
                 yield post
 
     async def get_favorited_posts(self) -> AsyncIterator[mdl.Post]:
         """Shorthand way to get favorited posts of currently logged-in user."""
         if self._profile is None:
@@ -183,17 +186,17 @@
         tag = f"recommended_for_post:{post_id}"
         async for post in self.browse_posts(tags=[tag]):
             yield post
 
     async def get_post_comments(self, post_id: int) -> AsyncIterator[mdl.Comment]:
         """Get comments of the specific post by its ID."""
         async for page in Paginator(
-            self._http_client,
-            const.COMMENT_URL.format(post_id=post_id),
-            mdl.Comment
+                self._http_client,
+                const.COMMENT_URL.format(post_id=post_id),
+                mdl.Comment
         ):
             for comment in page.items:
                 yield comment
 
     async def get_post(self, post_id: int) -> mdl.Post:
         """Get specific post by its ID."""
         response = await self._http_client.get(f"{const.POST_URL}/{post_id}")
@@ -206,28 +209,28 @@
     async def create_post(self):  # TODO: TBA
         raise NotImplementedError
 
 
 class AIClient(BaseClient):
     """Client for working with Sankaku built-in AI."""
     async def browse_ai_posts(
-        self,
-        *,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
+            self,
+            *,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
     ) -> AsyncIterator[mdl.AIPost]:
         """Get AI created posts from AI dedicated post pages.
 
         Args:
             page_number: Page number from which to start iteration
             limit: Maximum amount of posts per page
         """
         async for page in Paginator(
-            self._http_client, const.AI_POST_URL,
-            mdl.AIPost, **from_locals(locals())
+                self._http_client, const.AI_POST_URL,
+                mdl.AIPost, **from_locals(locals())
         ):
             for post in page.items:
                 yield post
 
     async def get_ai_post(self, post_id: int) -> mdl.AIPost:
         """Get specific AI post by its ID."""
         response = await self._http_client.get(f"{const.AI_POST_URL}/{post_id}")
@@ -240,24 +243,24 @@
     async def create_ai_post(self):  # TODO: TBA
         raise NotImplementedError
 
 
 class TagClient(BaseClient):
     """Client for tag browsing."""
     async def browse_tags(
-        self,
-        tag_type: Optional[types.TagType] = None,  # TODO: ability to specify multiple tags
-        order: Optional[types.TagOrder] = None,
-        rating: Optional[types.Rating] = None,
-        max_post_count: Optional[int] = None,
-        sort_parameter: Optional[types.SortParameter] = None,
-        sort_direction: Optional[types.SortDirection] = None,
-        *,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
+            self,
+            tag_type: Optional[types.TagType] = None,  # TODO: ability to specify multiple tags
+            order: Optional[types.TagOrder] = None,
+            rating: Optional[types.Rating] = None,
+            max_post_count: Optional[int] = None,
+            sort_parameter: Optional[types.SortParameter] = None,
+            sort_direction: Optional[types.SortDirection] = None,
+            *,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
 
     ) -> AsyncIterator[mdl.PageTag]:
         """Get tags from tag pages.
 
         Args:
             tag_type: Tag type filter
             order: Tag order rule
@@ -265,20 +268,20 @@
             max_post_count: Upper threshold for number of posts with tags found
             sort_parameter: Tag sorting parameter
             sort_direction: Tag sorting direction
             page_number: Page number from which to start iteration
             limit: Maximum amount of tags per page
         """
         async for page in TagPaginator(
-            self._http_client, const.TAG_URL, **from_locals(locals())
+                self._http_client, const.TAG_URL, **from_locals(locals())
         ):
             for tag in page.items:
                 yield tag
 
-    async def get_tag(self, name_or_id: str | int) -> mdl.WikiTag:
+    async def get_tag(self, name_or_id: Union[str, int]) -> mdl.WikiTag:
         """Get specific tag by its name or ID."""
         ref = "/name" if isinstance(name_or_id, str) else "/id"
         url = f"{const.TAG_WIKI_URL}{ref}/{name_or_id}"
 
         response = await self._http_client.get(url)
 
         if not response.ok:
@@ -286,25 +289,25 @@
 
         return mdl.WikiTag(wiki=response.json["wiki"], **response.json["tag"])
 
 
 class BookClient(BaseClient):
     """Client for book (pool) browsing."""
     async def browse_books(
-        self,
-        order: Optional[types.BookOrder] = None,
-        rating: Optional[types.Rating] = None,
-        recommended_for: Optional[str] = None,
-        favorited_by: Optional[str] = None,
-        tags: Optional[list[str]] = None,
-        added_by: Optional[list[str]] = None,
-        voted: Optional[str] = None,
-        *,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
+            self,
+            order: Optional[types.BookOrder] = None,
+            rating: Optional[types.Rating] = None,
+            recommended_for: Optional[str] = None,
+            favorited_by: Optional[str] = None,
+            tags: Optional[List[str]] = None,
+            added_by: Optional[List[str]] = None,
+            voted: Optional[str] = None,
+            *,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
     ) -> AsyncIterator[mdl.PageBook]:
         """Get books from book (pool) pages.
 
         Args:
             order: Book order rule
             rating: Books rating
             recommended_for: Books recommended for specified user
@@ -312,15 +315,15 @@
             tags: Tags available for search
             added_by: Books uploaded by specified users
             voted: Books voted by specified user
             page_number: Page number from which to start iteration
             limit: Maximum amount of books per page
         """
         async for page in BookPaginator(
-            self._http_client, const.BOOK_URL, **from_locals(locals())
+                self._http_client, const.BOOK_URL, **from_locals(locals())
         ):
             for book in page.items:
                 yield book
 
     async def get_favorited_books(self) -> AsyncIterator[mdl.PageBook]:
         """Shorthand way to get favorited books for the currently logged-in user."""
         if self._profile is None:
@@ -344,15 +347,15 @@
 
         async for book in self.browse_books(tags=[f"read:@{self._profile.id}@"]):
             yield book
 
     async def get_related_books(self, post_id: int) -> AsyncIterator[mdl.PageBook]:
         """Get books related to specific post by its ID."""
         async for page in BookPaginator(
-            self._http_client, const.RELATED_BOOK_URL.format(post_id=post_id)
+                self._http_client, const.RELATED_BOOK_URL.format(post_id=post_id)
         ):
             for book in page.items:
                 yield book
 
     async def get_book(self, book_id: int) -> mdl.Book:
         """Get specific book by its ID."""
         response = await self._http_client.get(f"{const.BOOK_URL}/{book_id}")
@@ -362,36 +365,36 @@
 
         return mdl.Book(**response.json)
 
 
 class UserClient(BaseClient):
     """Client for browsing users."""
     async def browse_users(
-        self,
-        order: Optional[types.UserOrder] = None,
-        level: Optional[types.UserLevel] = None,
-        *,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
+            self,
+            order: Optional[types.UserOrder] = None,
+            level: Optional[types.UserLevel] = None,
+            *,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None
     ) -> AsyncIterator[mdl.User]:
         """Get user profiles from user pages.
 
         Args:
             order: User order rule
             level: User level type
             page_number: Page number from which to start iteration
             limit: Maximum amount of users per page
         """
         async for page in UserPaginator(
-            self._http_client, const.USER_URL, **from_locals(locals())
+                self._http_client, const.USER_URL, **from_locals(locals())
         ):
             for user in page.items:
                 yield user
 
-    async def get_user(self, name_or_id: str | int) -> mdl.User:
+    async def get_user(self, name_or_id: Union[str, int]) -> mdl.User:
         """Get specific user by its name or ID."""
         ref = "/name" if isinstance(name_or_id, str) else ""
         url = f"{const.USER_URL}{ref}/{name_or_id}"
 
         response = await self._http_client.get(url)
 
         if not response.ok:
```

### Comparing `sankaku-1.0.1/sankaku/constants.py` & `sankaku-1.0.2/sankaku/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Necessary constants such as hardcoded headers, API urls and endpoints,
 default values of parameters etc.
 """
+from typing import Dict
 
-HEADERS: dict[str, str] = {
+HEADERS: Dict[str, str] = {
     "user-agent": (
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 "
         "(KHTML, like Gecko) Chrome/94.0.4606.85 YaBrowser/21.11.0.1996 "
         "Yowser/2.5 Safari/537.36"
     ),
     "content-type": "application/json; charset=utf-8",
     "x-requested-with": "com.android.browser",
     "accept-encoding": "gzip, deflate, br",
     "host": "capi-v2.sankakucomplex.com"
 }
 
-
 BASE_URL = "https://login.sankakucomplex.com"
 API_URL = "https://capi-v2.sankakucomplex.com"
 
 LOGIN_URL = f"{BASE_URL}/auth/token"
 POST_URL = f"{API_URL}/posts"
 AI_POST_URL = f"{API_URL}/ai_posts"
 TAG_URL = f"{API_URL}/tags"
@@ -27,19 +27,20 @@
 USER_URL = f"{API_URL}/users"
 PROFILE_URL = f"{USER_URL}/me"
 
 # Not fully completed urls for usage with str.format()
 COMMENT_URL = f"{POST_URL}/{{post_id}}/comments"
 RELATED_BOOK_URL = f"{API_URL}/post/{{post_id}}/pools"
 
-
 BASE_RPS = 3
 BASE_RPM = 180
 BASE_PAGE_NUMBER = 1
 BASE_PAGE_LIMIT = 40
 
+BASE_RETRIES = 3
+
 PAGE_ALLOWED_ERRORS = [
     "snackbar__anonymous-recommendations-limit-reached",
     "snackbar__account_offset-forbidden"
 ]
 
 DEFAULT_TOKEN_TYPE = "Bearer"
```

### Comparing `sankaku-1.0.1/sankaku/errors.py` & `sankaku-1.0.2/sankaku/errors.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.1/sankaku/models/books.py` & `sankaku-1.0.2/sankaku/models/books.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
-from typing import Optional
 from datetime import datetime
+from typing import Optional, List
 
 from pydantic import BaseModel
 
 from sankaku import types
-from .users import Author
-from .tags import PostTag
 from .posts import Post
+from .tags import PostTag
+from .users import Author
 
 
 __all__ = ["PageBook", "Book"]
 
 
 class BookState(BaseModel):
     current_page: int
@@ -46,21 +46,21 @@
     parent_id: Optional[int]
     has_children: Optional[bool]
     is_rating_locked: bool
     fav_count: int
     vote_count: int
     total_score: int
     comment_count: Optional[int]
-    tags: list[PostTag]
-    post_tags: list[PostTag]
-    artist_tags: list[PostTag]
-    genre_tags: list[PostTag]
+    tags: List[PostTag]
+    post_tags: List[PostTag]
+    artist_tags: List[PostTag]
+    genre_tags: List[PostTag]
     is_favorited: bool
     user_vote: Optional[int]
-    posts: list[Post]
+    posts: List[Post]
     file_url: Optional[str]
     sample_url: Optional[str]
     preview_url: Optional[str]
     cover_post: Optional[Post]
     reading: Optional[BookState]
     is_premium: bool
     is_pending: bool
@@ -72,10 +72,10 @@
     cover_post_id: Optional[int]
     name: Optional[str]
     parent_pool: Optional[PageBook]
 
 
 class Book(PageBook):
     """Model that describes specific book."""
-    child_pools: Optional[list[PageBook]]
+    child_pools: Optional[List[PageBook]]
     flagged_by_user: bool
     prem_post_count: int
```

### Comparing `sankaku-1.0.1/sankaku/models/posts.py` & `sankaku-1.0.2/sankaku/models/posts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from typing import Optional
 from datetime import datetime
+from typing import Optional, List
 
 from pydantic import BaseModel, Field, validator
 
 from sankaku import types
 from sankaku.utils import convert_ts_to_datetime
 from .tags import PostTag
 from .users import Author
@@ -36,28 +36,27 @@
     preview_url: Optional[str]
     width: int
     height: int
     file_size: int
     extension: Optional[str] = Field(alias="file_type")
     generation_directives: Optional[GenerationDirectives]
     md5: str
-    tags: list[PostTag]
+    tags: List[PostTag]
 
     @property
     def file_type(self) -> Optional[types.FileType]:
         """Get type of the file."""
-        match self.extension:
-            case "png" | "jpeg" | "webp":
-                return types.FileType.IMAGE
-            case "webm" | "mp4":
-                return types.FileType.VIDEO
-            case "gif":
-                return types.FileType.GIF
-            case _:
-                return None
+        if self.extension in ('png', 'jpeg', 'webp'):
+            return types.FileType.IMAGE
+        elif self.extension in ('webm', 'mp4'):
+            return types.FileType.VIDEO
+        elif self.extension in ('gif',):
+            return types.FileType.GIF
+        else:
+            return None
 
     # Validators
     _normalize_datetime = (
         validator("created_at", pre=True, allow_reuse=True)
         (convert_ts_to_datetime)
     )
 
@@ -71,15 +70,15 @@
     id: int
     created_at: datetime
     post_id: int
     author: Author
     body: str
     score: int
     parent_id: Optional[int]
-    children: list[Comment]
+    children: List[Comment]
     deleted: bool
     deleted_by: dict  # Seen only empty dictionaries so IDK real type
     updated_at: Optional[datetime]
     can_reply: bool
     reason: None  # Seen only None values so IDK real type
```

### Comparing `sankaku-1.0.1/sankaku/models/tags.py` & `sankaku-1.0.2/sankaku/models/tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Optional
 from datetime import datetime
+from typing import Optional, List
 
 from pydantic import BaseModel, Field, validator
 
 from sankaku import types
 from sankaku.utils import convert_ts_to_datetime
 from .users import Author
 
@@ -30,72 +30,82 @@
     tag_name: str = Field(alias="tagName")
     total_post_count: int
     total_pool_count: int
 
 
 class PostTag(BaseTag, TagMixin):
     """Model that describes tags related to posts."""
-    locale: str
+    locale: Optional[str]
     version: Optional[int]
 
 
 class NestedTag(BaseTag):
     """Model that describes tags with specific relation to certain tag on tag page."""
     post_count: int = Field(alias="postCount")
-    cached_related: Optional[list[int]] = Field(alias="cachedRelated")
+    cached_related: Optional[List[int]] = Field(alias="cachedRelated")
     cached_related_expires_on: datetime = Field(alias="cachedRelatedExpiresOn")
     type: types.TagType = Field(alias="tagType")
     name_en: str = Field(alias="nameEn")
     name_ja: Optional[str] = Field(alias="nameJa")
     popularity_all: Optional[float] = Field(alias="scTagPopularityAll")
     quality_all: Optional[float] = Field(alias="scTagQualityAll")
     popularity_ero: Optional[float] = Field(alias="scTagPopularityEro")
     popularity_safe: Optional[float] = Field(alias="scTagPopularitySafe")
     quality_ero: Optional[float] = Field(alias="scTagQualityEro")
     quality_safe: Optional[float] = Field(alias="scTagQualitySafe")
-    parent_tags: Optional[list[int]] = Field(alias="parentTags")
-    child_tags: Optional[list[int]] = Field(alias="childTags")
+    parent_tags: Optional[List[int]] = Field(alias="parentTags")
+    child_tags: Optional[List[int]] = Field(alias="childTags")
     pool_count: int = Field(alias="poolCount")
     premium_post_count: int = Field(alias="premPostCount")
     non_premium_post_count: int = Field(alias="nonPremPostCount")
     premium_pool_count: int = Field(alias="premPoolCount")
     non_premium_pool_count: int = Field(alias="nonPremPoolCount")
     series_count: int = Field(alias="seriesCount")
     premium_series_count: int = Field(alias="premSeriesCount")
     non_premium_series_count: int = Field(alias="nonPremSeriesCount")
     is_trained: bool = Field(alias="isTrained")
     child: int
     parent: int
     version: Optional[int]
 
     @validator("cached_related", "parent_tags", "child_tags", pre=True)
-    def flatten(cls, v) -> Optional[list[int]]:  # noqa
+    def flatten(cls, v) -> Optional[List[int]]:  # noqa
         """Flatten nested lists into one."""
         if not v:
             return None
         tag_ids = v.split(",") if "," in v else v.split()
         try:
             return [int(tag_id) for tag_id in tag_ids]
         except ValueError:
             return None
 
 
-class Translations(BaseModel):
-    """Model that describes tag translations if they are present."""
-    root_id: int = Field(alias="rootId")
+class BaseTranslations(BaseModel):
+    """Model that contain minimum information about tag translations."""
     lang: str
     translation: str
 
 
+class PageTagTranslations(BaseTranslations):
+    """Model that describes page tag translations."""
+    root_id: int = Field(alias="rootId")
+
+
+class WikiTagTranslations(BaseTranslations):
+    """Model that describes wiki tag translations."""
+    status: int
+    opacity: float
+
+
 class PageTag(PostTag):
     """Model that describes tags on tag page."""
-    translations: list[Translations]
-    related_tags: list[NestedTag]
-    child_tags: list[NestedTag]
-    parent_tags: list[NestedTag]
+    translations: List[PageTagTranslations]
+    related_tags: List[NestedTag]
+    child_tags: List[NestedTag]
+    parent_tags: List[NestedTag]
 
 
 class Wiki(BaseModel):
     """Model that describes wiki information for specific tag."""
     id: int
     title: str
     body: str
@@ -110,14 +120,14 @@
         validator("created_at", "updated_at", pre=True, allow_reuse=True)
         (convert_ts_to_datetime)
     )
 
 
 class WikiTag(BaseTag, TagMixin):
     """Model that describes tag on wiki page."""
-    related_tags: list[PostTag]
-    child_tags: list[PostTag]
-    parent_tags: list[PostTag]
-    alias_tags: list[PostTag]
-    implied_tags: list[PostTag]
-    translations: list[Translations]
+    related_tags: List[PostTag]
+    child_tags: List[PostTag]
+    parent_tags: List[PostTag]
+    alias_tags: List[PostTag]
+    implied_tags: List[PostTag]
+    translations: List[WikiTagTranslations]
     wiki: Wiki
```

### Comparing `sankaku-1.0.1/sankaku/models/users.py` & `sankaku-1.0.2/sankaku/models/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Optional
+from typing import Optional, List
 
 from pydantic import BaseModel, Field, validator
 
 from sankaku import types
 
 
 __all__ = ["Author", "User", "ExtendedUser"]
@@ -51,29 +51,29 @@
     favorite_count: Optional[int] = None
     post_favorite_count: Optional[int]
     pool_favorite_count: Optional[int]
     vote_count: Optional[int] = None
     post_vote_count: Optional[int] = None
     pool_vote_count: Optional[int] = None
     recommended_posts_for_user: Optional[int] = None
-    subscriptions: list[str] = []
+    subscriptions: List[str] = []
 
 
 class ExtendedUser(User):
     """Profile of the currently logged-in user."""
     email: str
     hide_ads: bool
     subscription_level: int
     filter_content: bool
     receive_dmails: bool
     email_verification_status: str
     is_verified: bool
     verifications_count: int
     blacklist_is_hidden: bool
-    blacklisted_tags: list[str]
-    blacklisted: list[str]
+    blacklisted_tags: List[str]
+    blacklisted: List[str]
     mfa_method: int
 
     @validator("blacklisted_tags", pre=True)
-    def flatten_blacklisted_tags(cls, v) -> list[str]:  # noqa
+    def flatten_blacklisted_tags(cls, v) -> List[str]:  # noqa
         """Flatten nested lists into one."""
         return [tag[0] for tag in v]
```

### Comparing `sankaku-1.0.1/sankaku/paginators/abc.py` & `sankaku-1.0.2/sankaku/paginators/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from abc import ABC, abstractmethod
-from collections.abc import AsyncIterator
-from typing import Generic, TypeVar
+from typing import Generic, TypeVar, AsyncIterator
 
 from sankaku import errors, models as mdl
 
 
 __all__ = ["ABCPaginator"]
 
-
 _T = TypeVar("_T")
 
 
 class ABCPaginator(ABC, Generic[_T]):
     """Abstract paginator class."""
     @abstractmethod
     def __init__(self, *args, **kwargs) -> None:
```

### Comparing `sankaku-1.0.1/sankaku/paginators/paginators.py` & `sankaku-1.0.2/sankaku/paginators/paginators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,108 @@
-from typing import Optional, Literal, Annotated, TypeVar
 from datetime import datetime
+from typing import Optional, TypeVar, List, Dict, Type
+
+try:
+    from typing import Literal, Annotated
+except (ModuleNotFoundError, ImportError):
+    from typing_extensions import Literal, Annotated  # type: ignore[assignment]
 
-from .abc import ABCPaginator
-from sankaku.typedefs import ValueRange
-from sankaku.utils import ratelimit
 from sankaku import models as mdl, constants as const, types, errors
 from sankaku.clients import HttpClient
+from sankaku.utils import ratelimit
+from sankaku.typedefs import ValueRange
+from .abc import ABCPaginator
 
 
 __all__ = [
     "Paginator",
     "PostPaginator",
     "TagPaginator",
     "BookPaginator",
     "UserPaginator"
 ]
 
-
 _T = TypeVar("_T")
 
 
 class Paginator(ABCPaginator[_T]):
     """Basic paginator for iteration without any special parameters."""
     def __init__(
-        self,
-        http_client: HttpClient,
-        url: str,
-        model: type[_T],
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
-        params: Optional[dict[str, str]] = None
+            self,
+            http_client: HttpClient,
+            url: str,
+            model: Type[_T],
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
+            params: Optional[Dict[str, str]] = None
     ) -> None:
         self.http_client = http_client
         self.url = url
         self.model = model
         self.page_number = page_number or const.BASE_PAGE_NUMBER
         self.limit = limit or const.BASE_PAGE_LIMIT
-        self.params: dict[str, str] = params or {}
+        self.params: Dict[str, str] = params or {}
 
         self.complete_params()
 
     @ratelimit(rps=const.BASE_RPS)
     async def next_page(self) -> mdl.Page[_T]:  # type: ignore[override]
         """Get paginator next page."""
         response = await self.http_client.get(self.url, params=self.params)
-        match response.json:
-            case [] | {"data": []}:
-                raise errors.PaginatorLastPage(response.status, page=self.page_number)
-            case {"code": code} if code in const.PAGE_ALLOWED_ERRORS:
-                raise errors.PaginatorLastPage(response.status, page=self.page_number)
-            case {"code": _, "errorId": _}:
-                raise errors.SankakuServerError(response.status, **response.json)
-            case {"data": list() as data} if data:
-                response.json = data
+        json_ = response.json
+        if "code" in json_ and json_["code"] in const.PAGE_ALLOWED_ERRORS:
+            raise errors.PaginatorLastPage(response.status, page=self.page_number)
+        elif "code" in json_:
+            raise errors.SankakuServerError(response.status, **response.json)
+        elif json_ == [] or (isinstance(json_, dict) and not json_["data"]):
+            raise errors.PaginatorLastPage(response.status, page=self.page_number)
+        elif "data" in json_:
+            response.json = json_["data"]
 
         self.page_number += 1
         self.params["page"] = str(self.page_number)
         return self._construct_page(response.json)
 
     def complete_params(self) -> None:
         """Complete params passed to paginator for further use."""
         self.params["lang"] = "en"
         if self.page_number is not None:
             self.params["page"] = str(self.page_number)
         if self.limit is not None:
             self.params["limit"] = str(self.limit)
 
-    def _construct_page(self, data: list[dict]) -> mdl.Page[_T]:
+    def _construct_page(self, data: List[dict]) -> mdl.Page[_T]:
         """Construct and return page model."""
         items = [self.model(**d) for d in data]
         return mdl.Page[_T](number=self.page_number - 1, items=items)
 
 
 class PostPaginator(Paginator[mdl.Post]):
     """Paginator used for iteration through post pages."""
     def __init__(
-        self,
-        http_client: HttpClient,
-        url: str,
-        model: type[mdl.Post] = mdl.Post,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
-        params: Optional[dict[str, str]] = None,
-        order: Optional[types.PostOrder] = None,
-        date: Optional[list[datetime]] = None,
-        rating: Optional[types.Rating] = None,
-        threshold: Optional[Annotated[int, ValueRange(1, 100)]] = None,
-        hide_posts_in_books: Optional[Literal["in-larger-tags", "always"]] = None,
-        file_size: Optional[types.FileSize] = None,
-        file_type: Optional[types.FileType] = None,
-        video_duration: Optional[list[int]] = None,
-        recommended_for: Optional[str] = None,
-        favorited_by: Optional[str] = None,
-        tags: Optional[list[str]] = None,
-        added_by: Optional[list[str]] = None,
-        voted: Optional[str] = None
+            self,
+            http_client: HttpClient,
+            url: str,
+            model: Type[mdl.Post] = mdl.Post,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
+            params: Optional[Dict[str, str]] = None,
+            order: Optional[types.PostOrder] = None,
+            date: Optional[List[datetime]] = None,
+            rating: Optional[types.Rating] = None,
+            threshold: Optional[Annotated[int, ValueRange(1, 100)]] = None,
+            hide_posts_in_books: Optional[Literal["in-larger-tags", "always"]] = None,
+            file_size: Optional[types.FileSize] = None,
+            file_type: Optional[types.FileType] = None,
+            video_duration: Optional[List[int]] = None,
+            recommended_for: Optional[str] = None,
+            favorited_by: Optional[str] = None,
+            tags: Optional[List[str]] = None,
+            added_by: Optional[List[str]] = None,
+            voted: Optional[str] = None
     ) -> None:
         self.order = order
         self.date = date
         self.rating = rating
         self.threshold = threshold
         self.hide_posts_in_books = hide_posts_in_books
         self.file_size = file_size
@@ -112,60 +116,59 @@
         super().__init__(http_client, url, model, page_number, limit, params)
 
     def complete_params(self) -> None:
         super().complete_params()
         if self.tags is None:
             self.tags = []
 
-        for items in self.__dict__.items():
-            match items:
-                case [_, None]:
-                    continue
-                case ["order" | "rating" | "file_type" as k, v] if v is not types.FileType.IMAGE:  # noqa
-                    self.tags.append(f"{k}:{v.value}")
-                case ["threshold" | "recommended_for" | "voted" as k, v]:
-                    self.tags.append(f"{k}:{v}")
-                case ["file_size", _]:
-                    self.tags.append(self.file_size.value)  # type: ignore[union-attr]
-                case ["date", _]:
-                    date = "..".join(d.strftime("%Y-%m-%dT%H:%M") for d in self.date)  # type: ignore[union-attr]
-                    self.tags.append(f"date:{date}")
-                case ["video_duration", _] if self.file_type is not types.FileType.VIDEO:  # noqa
-                    raise errors.VideoDurationError
-                case ["video_duration", _]:
-                    duration = "..".join(str(sec) for sec in self.video_duration)  # type: ignore[union-attr]
-                    self.tags.append(f"duration:{duration}")
-                case ["favorited_by", _]:
-                    self.tags.append(f"fav:{self.favorited_by}")
-                case ["added_by", _]:
-                    for user in self.added_by:  # type: ignore[union-attr]
-                        self.tags.append(f"user:{user}")
+        for k, v in self.__dict__.items():
+            if v is None:
+                continue
+            elif k in {"order", "rating", "file_type"} and v is not types.FileType.IMAGE:  # noqa
+                self.tags.append(f"{k}:{v.value}")
+            elif k in {"threshold", "recommended_for", "voted"}:
+                self.tags.append(f"{k}:{v}")
+            elif k == "file_size":
+                self.tags.append(self.file_size.value)  # type: ignore[union-attr]
+            elif k == "date":
+                date = "..".join(d.strftime("%Y-%m-%dT%H:%M") for d in self.date)  # type: ignore[union-attr]
+                self.tags.append(f"date:{date}")
+            elif k == "video_duration" and self.file_type is not types.FileType.VIDEO:  # noqa
+                raise errors.VideoDurationError
+            elif k == "video_duration":
+                duration = "..".join(str(sec) for sec in self.video_duration)  # type: ignore[union-attr]
+                self.tags.append(f"duration:{duration}")
+            elif k == "favorited_by":
+                self.tags.append(f"fav:{self.favorited_by}")
+            elif k == "added_by":
+                for user in self.added_by:  # type: ignore[union-attr]
+                    self.tags.append(f"user:{user}")
 
         if self.hide_posts_in_books is not None:
             self.params["hide_posts_in_books"] = self.hide_posts_in_books
         if self.tags:
             self.params["tags"] = " ".join(self.tags)
 
 
 class TagPaginator(Paginator[mdl.PageTag]):
     """Paginator used for iteration through tag pages."""
     def __init__(
-        self,
-        http_client: HttpClient,
-        url: str,
-        model: type[mdl.PageTag] = mdl.PageTag,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
-        params: Optional[dict[str, str]] = None,
-        tag_type: Optional[types.TagType] = None,
-        order: Optional[types.TagOrder] = None,
-        rating: Optional[types.Rating] = None,
-        max_post_count: Optional[int] = None,
-        sort_parameter: Optional[types.SortParameter] = None,
-        sort_direction: Optional[types.SortDirection] = None
+            self,
+            http_client: HttpClient,
+            url: str,
+            model: Type[mdl.PageTag] = mdl.PageTag,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
+            params: Optional[Dict[str, str]] = None,
+            tag_type: Optional[types.TagType] = None,
+            order: Optional[types.TagOrder] = None,
+            rating: Optional[types.Rating] = None,
+            max_post_count: Optional[int] = None,
+            sort_parameter: Optional[types.SortParameter] = None,
+            sort_direction: Optional[types.SortDirection] = None
     ) -> None:
         self.tag_type = tag_type
         self.order = order
         self.rating = rating
         self.max_post_count = max_post_count
         self.sort_parameter = sort_parameter
         self.sort_direction = sort_direction or types.SortDirection.DESC
@@ -187,28 +190,28 @@
                 sortDirection=self.sort_direction.value
             )
 
 
 class BookPaginator(Paginator[mdl.PageBook]):
     """Paginator used for iteration through book pages."""
     def __init__(
-        self,
-        http_client: HttpClient,
-        url: str,
-        model: type[mdl.PageBook] = mdl.PageBook,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
-        params: Optional[dict[str, str]] = None,
-        order: Optional[types.BookOrder] = None,
-        rating: Optional[types.Rating] = None,
-        recommended_for: Optional[str] = None,
-        favorited_by: Optional[str] = None,
-        tags: Optional[list[str]] = None,
-        added_by: Optional[list[str]] = None,
-        voted: Optional[str] = None
+            self,
+            http_client: HttpClient,
+            url: str,
+            model: Type[mdl.PageBook] = mdl.PageBook,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
+            params: Optional[Dict[str, str]] = None,
+            order: Optional[types.BookOrder] = None,
+            rating: Optional[types.Rating] = None,
+            recommended_for: Optional[str] = None,
+            favorited_by: Optional[str] = None,
+            tags: Optional[List[str]] = None,
+            added_by: Optional[List[str]] = None,
+            voted: Optional[str] = None
     ) -> None:
         self.order = order
         self.rating = rating
         self.recommended_for = recommended_for
         self.favorited_by = favorited_by
         self.tags = tags
         self.added_by = added_by
@@ -216,44 +219,43 @@
         super().__init__(http_client, url, model, page_number, limit, params)
 
     def complete_params(self) -> None:
         super().complete_params()
         if self.tags is None:
             self.tags = []
 
-        for items in self.__dict__.items():
-            match items:
-                case [_, None]:
-                    continue
-                case ["order" | "rating" as k, v]:  # noqa
-                    self.tags.append(f"{k}:{v.value}")
-                case ["recommended_for" | "voted" as k, v]:
-                    self.tags.append(f"{k}:{v}")
-                case ["favorited_by", _]:
-                    self.tags.append(f"fav:{self.favorited_by}")
-                case ["added_by", _]:
-                    for user in self.added_by:  # type: ignore[union-attr]
-                        self.tags.append(f"user:{user}")
+        for k, v in self.__dict__.items():
+            if v is None:
+                continue
+            elif k in {"order", "rating"}:
+                self.tags.append(f"{k}:{v.value}")
+            elif k in {"recommended_for", "voted"}:
+                self.tags.append(f"{k}:{v}")
+            elif k == "favorited_by":
+                self.tags.append(f"fav:{self.favorited_by}")
+            elif k == "added_by":
+                for user in self.added_by:  # type: ignore[union-attr]
+                    self.tags.append(f"user:{user}")
 
         if self.tags:
             self.params["tags"] = " ".join(self.tags)
 
 
 class UserPaginator(Paginator[mdl.User]):
     """Paginator used for iteration through user pages."""
     def __init__(
-        self,
-        http_client: HttpClient,
-        url: str,
-        model: type[mdl.User] = mdl.User,
-        page_number: Optional[int] = None,
-        limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
-        params: Optional[dict[str, str]] = None,
-        order: Optional[types.UserOrder] = None,
-        level: Optional[types.UserLevel] = None
+            self,
+            http_client: HttpClient,
+            url: str,
+            model: Type[mdl.User] = mdl.User,
+            page_number: Optional[int] = None,
+            limit: Optional[Annotated[int, ValueRange(1, 100)]] = None,
+            params: Optional[Dict[str, str]] = None,
+            order: Optional[types.UserOrder] = None,
+            level: Optional[types.UserLevel] = None
     ) -> None:
         self.order = order
         self.level = level
         super().__init__(http_client, url, model, page_number, limit, params)
 
     def complete_params(self) -> None:
         super().complete_params()
```

### Comparing `sankaku-1.0.1/sankaku/types.py` & `sankaku-1.0.2/sankaku/types.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.1/sankaku/utils.py` & `sankaku-1.0.2/sankaku/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Miscellaneous support functions that are used at different places."""
 
 import asyncio
 from datetime import datetime
 from functools import wraps
-from typing import TypeVar, ParamSpec, Optional, Any
-from collections.abc import Callable, Awaitable
+from typing import TypeVar, Optional, Any, Dict, Tuple, Callable, Awaitable
 
+try:
+    from typing import ParamSpec
+except (ModuleNotFoundError, ImportError):
+    from typing_extensions import ParamSpec  # type: ignore[assignment]
 
 from sankaku.errors import RateLimitError
 from sankaku.typedefs import Timestamp
 
 
 __all__ = ["ratelimit", "convert_ts_to_datetime", "from_locals"]
 
-
 _T = TypeVar("_T")
 _P = ParamSpec("_P")
 
 
 def ratelimit(
-    *,
-    rps: Optional[int] = None,
-    rpm: Optional[int] = None
+        *,
+        rps: Optional[int] = None,
+        rpm: Optional[int] = None
 ) -> Callable[[Callable[_P, Awaitable[_T]]], Callable[_P, Awaitable[_T]]]:
     """Limit the number of requests.
 
     Args:
         rps: Request per second
         rpm: Requests per minute
     """
@@ -37,29 +39,30 @@
     sleep_time: float = (1 / rps) if rps else (60 / rpm)  # type: ignore[operator]
 
     def wrapper(func: Callable[_P, Awaitable[_T]]) -> Callable[_P, Awaitable[_T]]:
         @wraps(func)
         async def inner(*args: _P.args, **kwargs: _P.kwargs) -> _T:
             await asyncio.sleep(sleep_time)
             return await func(*args, **kwargs)  # noqa
+
         return inner
 
     return wrapper
 
 
 def convert_ts_to_datetime(ts: Timestamp) -> Optional[datetime]:
     """Convert timestamp in datetime dict into datetime class."""
     if ts.get("s") is None:
         return None
     return datetime.utcfromtimestamp(ts["s"]).astimezone()  # type: ignore[arg-type]
 
 
 def from_locals(
-    loc: dict[str, Any], exclude: tuple[str, ...] = ("self",)
-) -> dict[str, Any]:
+        loc: Dict[str, Any], exclude: Tuple[str, ...] = ("self",)
+) -> Dict[str, Any]:
     """Get arguments of calling function from its locals to pass them to paginator.
 
     Args:
         loc: locals of calling function
         exclude: arguments to be excluded
     """
     return {k: v for k, v in loc.copy().items() if k not in exclude}
```

### Comparing `sankaku-1.0.1/sankaku.egg-info/PKG-INFO` & `sankaku-1.0.2/sankaku.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 Metadata-Version: 2.1
 Name: sankaku
-Version: 1.0.1
+Version: 1.0.2
 Summary: Asynchronous API wrapper for Sankaku Complex.
 Home-page: https://github.com/zerex290/sankaku
 Author: zerex290
 Author-email: zerex290@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/zerex290/sankaku/issues
 Keywords: sankaku,sankakucomplex,api
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: socks
+Provides-Extra: test
 License-File: LICENSE
 
 <h1 align="center">
   <a href="https://github.com/zerex290/sankaku">
     <img src="https://raw.githubusercontent.com/zerex290/sankaku/main/docs/icon.png" alt="Sankaku Complex"
     width="150" height="150"/>
   </a>
@@ -45,18 +51,20 @@
 
 Source code: https://github.com/zerex290/sankaku
 
 ---
 
 ## Requirements
 
-- Python 3.11+
+- Python 3.7+
 - aiohttp
 - pydantic
 - loguru
+- aiohttp-retry
+- typing_extensions; python_version < '3.9'
 
 ## Installation
 
 To install sankaku via pip write following line of code in your terminal:
 
 ```commandline
 pip install sankaku
```

#### html2text {}

```diff
@@ -1,38 +1,42 @@
-Metadata-Version: 2.1 Name: sankaku Version: 1.0.1 Summary: Asynchronous API
+Metadata-Version: 2.1 Name: sankaku Version: 1.0.2 Summary: Asynchronous API
 wrapper for Sankaku Complex. Home-page: https://github.com/zerex290/sankaku
 Author: zerex290 Author-email: zerex290@gmail.com License: MIT Project-URL:
 Issue Tracker, https://github.com/zerex290/sankaku/issues Keywords:
-sankaku,sankakucomplex,api Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
-markdown License-File: LICENSE
+sankaku,sankakucomplex,api Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+socks Provides-Extra: test License-File: LICENSE
                                [Sankaku_Complex]
                                     sankaku
                             For real men of culture
 ## About Asynchronous API wrapper for [Sankaku Complex](https://
 beta.sankakucomplex.com) with *type-hinting*, pydantic *data validation* and an
 optional *logging support* with loguru. ### Features: - Type-hints -
 Deserialization of raw json data thanks to pydantic models - Enumerations for
 API request parameters to provide better user experience > For instance, you
 can type `types.TagType.ARTIST` instead of `types[]=1` --- Documentation:
 https://zerex290.github.io/sankaku API Reference: https://zerex290.github.io/
 sankaku/api Source code: https://github.com/zerex290/sankaku --- ##
-Requirements - Python 3.11+ - aiohttp - pydantic - loguru ## Installation To
-install sankaku via pip write following line of code in your terminal:
-```commandline pip install sankaku ``` To install the sankaku via Docker, you
-can follow these steps: ###### Step 1: Install Docker Ensure that Docker is
-installed on your machine. If Docker is not already installed, you can download
-and install it from the official [Docker website](https://www.docker.com/get-
-started). ###### Step 2: Use docker to install sankaku Open a command prompt.
-Navigate to the directory where you want to install Sankaku. Type the following
-command: ```commandline git clone https://github.com/zerex290/sankaku.git cd
-sankaku docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash
-``` ## Usage example It's very simple to use and doesn't require to always keep
-opened browser page with documentation because all methods are self-
-explanatory: ```py import asyncio from sankaku import SankakuClient async def
-main(): client = SankakuClient() post = await client.get_post(25742064) print
-(f"Rating: {post.rating} | Created: {post.created_at}") # "Rating:
-Rating.QUESTIONABLE | Created: 2021-08-01 23:18:52+03:00" await client.login
-(access_token="token") # Or you can authorize by credentials: # await
-client.login(login="nickname or email", password="password") async for book in
-client.get_recently_read_books(): ... asyncio.run(main()) ```
+Requirements - Python 3.7+ - aiohttp - pydantic - loguru - aiohttp-retry -
+typing_extensions; python_version < '3.9' ## Installation To install sankaku
+via pip write following line of code in your terminal: ```commandline pip
+install sankaku ``` To install the sankaku via Docker, you can follow these
+steps: ###### Step 1: Install Docker Ensure that Docker is installed on your
+machine. If Docker is not already installed, you can download and install it
+from the official [Docker website](https://www.docker.com/get-started). ######
+Step 2: Use docker to install sankaku Open a command prompt. Navigate to the
+directory where you want to install Sankaku. Type the following command:
+```commandline git clone https://github.com/zerex290/sankaku.git cd sankaku
+docker run -it --name sankaku -w /opt -v$(pwd):/opt python:3.11 bash ``` ##
+Usage example It's very simple to use and doesn't require to always keep opened
+browser page with documentation because all methods are self-explanatory: ```py
+import asyncio from sankaku import SankakuClient async def main(): client =
+SankakuClient() post = await client.get_post(25742064) print(f"Rating:
+{post.rating} | Created: {post.created_at}") # "Rating: Rating.QUESTIONABLE |
+Created: 2021-08-01 23:18:52+03:00" await client.login(access_token="token") #
+Or you can authorize by credentials: # await client.login(login="nickname or
+email", password="password") async for book in client.get_recently_read_books
+(): ... asyncio.run(main()) ```
```

