# Comparing `tmp/cardboard.py-0.0.1.tar.gz` & `tmp/cardboard.py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardboard.py-0.0.1.tar", last modified: Wed May 31 20:14:46 2023, max compression
+gzip compressed data, was "cardboard.py-0.0.2.tar", last modified: Wed May 31 20:27:24 2023, max compression
```

## Comparing `cardboard.py-0.0.1.tar` & `cardboard.py-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 20:14:46.486199 cardboard.py-0.0.1/
--rw-rw-rw-   0        0        0     2468 2023-05-31 20:14:46.486199 cardboard.py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-05-31 20:14:43.000000 cardboard.py-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 20:14:46.479198 cardboard.py-0.0.1/cardboard/
--rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.1/cardboard/Exceptions.py
--rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.1/cardboard/__init__.py
--rw-rw-rw-   0        0        0    10938 2023-05-31 20:13:17.000000 cardboard.py-0.0.1/cardboard/cardboard.py
--rw-rw-rw-   0        0        0        0 2023-05-31 14:44:45.000000 cardboard.py-0.0.1/cardboard/cardboard_async.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:14:46.485199 cardboard.py-0.0.1/cardboard.py.egg-info/
--rw-rw-rw-   0        0        0     2468 2023-05-31 20:14:46.000000 cardboard.py-0.0.1/cardboard.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-31 20:14:46.000000 cardboard.py-0.0.1/cardboard.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 20:14:46.000000 cardboard.py-0.0.1/cardboard.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-31 20:14:46.000000 cardboard.py-0.0.1/cardboard.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-31 20:14:46.000000 cardboard.py-0.0.1/cardboard.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 20:14:46.486199 cardboard.py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-05-31 20:14:37.000000 cardboard.py-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:27:24.789416 cardboard.py-0.0.2/
+-rw-rw-rw-   0        0        0     3280 2023-05-31 20:27:24.789416 cardboard.py-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2382 2023-05-31 20:26:45.000000 cardboard.py-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 20:27:24.780414 cardboard.py-0.0.2/cardboard/
+-rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.2/cardboard/Exceptions.py
+-rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.2/cardboard/__init__.py
+-rw-rw-rw-   0        0        0    10938 2023-05-31 20:26:53.000000 cardboard.py-0.0.2/cardboard/cardboard.py
+-rw-rw-rw-   0        0        0    10954 2023-05-31 20:27:06.000000 cardboard.py-0.0.2/cardboard/cardboard_async.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:27:24.787414 cardboard.py-0.0.2/cardboard.py.egg-info/
+-rw-rw-rw-   0        0        0     3280 2023-05-31 20:27:24.000000 cardboard.py-0.0.2/cardboard.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-31 20:27:24.000000 cardboard.py-0.0.2/cardboard.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 20:27:24.000000 cardboard.py-0.0.2/cardboard.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-31 20:27:24.000000 cardboard.py-0.0.2/cardboard.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 20:27:24.000000 cardboard.py-0.0.2/cardboard.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 20:27:24.789416 cardboard.py-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-05-31 20:27:21.000000 cardboard.py-0.0.2/setup.py
```

### Comparing `cardboard.py-0.0.1/PKG-INFO` & `cardboard.py-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.1
+Version: 0.0.2
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # cardboard.py
 
 cardboard.py is a Python library for interacting with the cardboard API.
 
-PyPi: https://pypi.org/project/cardboard/
+PyPi: https://pypi.org/project/cardboard.py/
 
 ## Installation
 
 You can install the cardboard.py library using pip:
 
 `pip install cardboard.py`
 
@@ -64,17 +64,43 @@
 - `.refresh_token(refresh_token:str)` (class AuthToken)
     - `.token` (str)
     - `.token_type` (str)
     - `.refresh_token` (str)
     - `.expires_in` (int)
     - `._raw` (dict)
 - `.get_user(token:str)` (class User)
-    - BEING DEVELOPED, NOTHING HERE IS DONE. WILL RAISE AN ERROR.
     - `.name` (str)
     - `.id` (str)
     - `.subdomain` (str)
     - `.aliases` (list(class UserAlias))
-        - ??? (being developed)
-    - ??? (being developed)
+        - `.alias` (str|None)
+        - `.discriminator` (str|None)
+        - `.name` (str)
+        - `.createdAt` (datetime)
+        - `.editedAt` (datetime)
+        - `._raw_createdAt` (str)
+        - `._raw_editedAt` (str)
+        - `.userId` (str)
+        - `.gameId` (int)
+        - `.socialLinkSource` (str|None)
+        - `.socialLinkHandle` (str|None)
+        - `.additionalInfo` (dict)
+        - `.playerInfo` (dict|None)
+        - `._raw` (dict)
+    - `.avatar` (str)
+    - `.banner` (str)
+    - `.status` (class UserStatus)
+        - `.text` (str|None)
+        - `.reaction_id` (int|None)
+        - `._raw` (dict)
+        - `._raw_text` (dict)
+        - `._raw_reaction` (dict)
+    - `.moderationStatus` (str|None)
+    - `.aboutInfo` (class userAbout)
+        - `.bio` (str|None)
+        - `.tagline` (str|None)
+        - `._raw` (dict)
+    - `.userTransientStatus` (str|None)
+    - `._raw` (dict)
 
 # License
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `cardboard.py-0.0.1/cardboard/Exceptions.py` & `cardboard.py-0.0.2/cardboard/Exceptions.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.1/cardboard/cardboard.py` & `cardboard.py-0.0.2/cardboard/cardboard.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.1/cardboard.py.egg-info/PKG-INFO` & `cardboard.py-0.0.2/cardboard.py.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.1
+Version: 0.0.2
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # cardboard.py
 
 cardboard.py is a Python library for interacting with the cardboard API.
 
-PyPi: https://pypi.org/project/cardboard/
+PyPi: https://pypi.org/project/cardboard.py/
 
 ## Installation
 
 You can install the cardboard.py library using pip:
 
 `pip install cardboard.py`
 
@@ -64,17 +64,43 @@
 - `.refresh_token(refresh_token:str)` (class AuthToken)
     - `.token` (str)
     - `.token_type` (str)
     - `.refresh_token` (str)
     - `.expires_in` (int)
     - `._raw` (dict)
 - `.get_user(token:str)` (class User)
-    - BEING DEVELOPED, NOTHING HERE IS DONE. WILL RAISE AN ERROR.
     - `.name` (str)
     - `.id` (str)
     - `.subdomain` (str)
     - `.aliases` (list(class UserAlias))
-        - ??? (being developed)
-    - ??? (being developed)
+        - `.alias` (str|None)
+        - `.discriminator` (str|None)
+        - `.name` (str)
+        - `.createdAt` (datetime)
+        - `.editedAt` (datetime)
+        - `._raw_createdAt` (str)
+        - `._raw_editedAt` (str)
+        - `.userId` (str)
+        - `.gameId` (int)
+        - `.socialLinkSource` (str|None)
+        - `.socialLinkHandle` (str|None)
+        - `.additionalInfo` (dict)
+        - `.playerInfo` (dict|None)
+        - `._raw` (dict)
+    - `.avatar` (str)
+    - `.banner` (str)
+    - `.status` (class UserStatus)
+        - `.text` (str|None)
+        - `.reaction_id` (int|None)
+        - `._raw` (dict)
+        - `._raw_text` (dict)
+        - `._raw_reaction` (dict)
+    - `.moderationStatus` (str|None)
+    - `.aboutInfo` (class userAbout)
+        - `.bio` (str|None)
+        - `.tagline` (str|None)
+        - `._raw` (dict)
+    - `.userTransientStatus` (str|None)
+    - `._raw` (dict)
 
 # License
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `cardboard.py-0.0.1/setup.py` & `cardboard.py-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cardboard.py',
-    version='0.0.1',
+    version='0.0.2',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://cardboard.ink/api/v1/',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cardboard-ink/cardboard.py/',
     packages=find_packages(),
```

