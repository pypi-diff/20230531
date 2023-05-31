# Comparing `tmp/intra42-0.1.4.tar.gz` & `tmp/intra42-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intra42-0.1.4.tar", last modified: Wed May 31 21:42:45 2023, max compression
+gzip compressed data, was "intra42-0.1.5.tar", last modified: Wed May 31 21:50:45 2023, max compression
```

## Comparing `intra42-0.1.4.tar` & `intra42-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:42:45.317048 intra42-0.1.4/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-31 21:42:45.317048 intra42-0.1.4/PKG-INFO
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:42:45.317048 intra42-0.1.4/intra42.egg-info/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/PKG-INFO
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/SOURCES.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/dependency_links.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/requires.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/top_level.txt
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:42:45.317048 intra42-0.1.4/intrascraper/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      304 2023-05-30 21:00:14.000000 intra42-0.1.4/intrascraper/__init__.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5553 2023-05-31 21:41:19.000000 intra42-0.1.4/intrascraper/intrascraper.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-31 21:42:45.317048 intra42-0.1.4/setup.cfg
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-31 21:42:33.000000 intra42-0.1.4/setup.py
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:50:45.541592 intra42-0.1.5/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-31 21:50:45.541592 intra42-0.1.5/PKG-INFO
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:50:45.541592 intra42-0.1.5/intra42.egg-info/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-31 21:50:45.000000 intra42-0.1.5/intra42.egg-info/PKG-INFO
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-31 21:50:45.000000 intra42-0.1.5/intra42.egg-info/SOURCES.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-31 21:50:45.000000 intra42-0.1.5/intra42.egg-info/dependency_links.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-31 21:50:45.000000 intra42-0.1.5/intra42.egg-info/requires.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-31 21:50:45.000000 intra42-0.1.5/intra42.egg-info/top_level.txt
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:50:45.541592 intra42-0.1.5/intrascraper/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      304 2023-05-30 21:00:14.000000 intra42-0.1.5/intrascraper/__init__.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5631 2023-05-31 21:49:25.000000 intra42-0.1.5/intrascraper/intrascraper.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-31 21:50:45.541592 intra42-0.1.5/setup.cfg
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-31 21:50:29.000000 intra42-0.1.5/setup.py
```

### Comparing `intra42-0.1.4/intrascraper/intrascraper.py` & `intra42-0.1.5/intrascraper/intrascraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from bs4 import BeautifulSoup, ResultSet
 import urllib.parse
 import urllib
 import typing
 from urllib import parse
 import typing
 import time
+from typing import Callable, TypeVar
+
+T = TypeVar('T')
 
 KEYCLOAK = "https://profile.intra.42.fr/users/auth/keycloak_student"
 SEND_FORM = "https://auth.42.fr/auth/realms/students-42/login-actions/authenticate"
 
 class Token(typing.TypedDict):
 	cookie:str
 	expires:int
@@ -54,17 +57,17 @@
 		cookie = x.cookies.get("_intra_42_session_production")
 		for c in x.cookies:
 			if c.name == '_intra_42_session_production':
 				self.token["expires"] = c.expires
 		self.token["cookie"] = cookie
 		return self.token
 
-	def do_request(self, f, *args, **kwargs):
+	def do_request(self, f: Callable[..., T], *args, **kwargs) -> T:
 
-		if self.token["expires"] >= time.time():
+		if time.time() >= self.token["expires"]:
 			print("Token seems to be expired...")
 
 		if ("cookies" in kwargs):
 			kwargs["cookies"].update({"_intra_42_session_production":self.token["cookie"]})
 		else:
 			kwargs["cookies"] = {"_intra_42_session_production":self.token["cookie"]}
 		return (f(*args, **kwargs))
```

