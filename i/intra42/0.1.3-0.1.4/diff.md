# Comparing `tmp/intra42-0.1.3.tar.gz` & `tmp/intra42-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intra42-0.1.3.tar", last modified: Tue May 30 21:01:34 2023, max compression
+gzip compressed data, was "intra42-0.1.4.tar", last modified: Wed May 31 21:42:45 2023, max compression
```

## Comparing `intra42-0.1.3.tar` & `intra42-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 21:01:34.634703 intra42-0.1.3/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-30 21:01:34.634703 intra42-0.1.3/PKG-INFO
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 21:01:34.634703 intra42-0.1.3/intra42.egg-info/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/PKG-INFO
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/SOURCES.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/dependency_links.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/requires.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-30 21:01:34.000000 intra42-0.1.3/intra42.egg-info/top_level.txt
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 21:01:34.634703 intra42-0.1.3/intrascraper/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      304 2023-05-30 21:00:14.000000 intra42-0.1.3/intrascraper/__init__.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5693 2023-05-30 15:15:22.000000 intra42-0.1.3/intrascraper/intrascraper.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-30 21:01:34.634703 intra42-0.1.3/setup.cfg
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-30 21:01:17.000000 intra42-0.1.3/setup.py
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:42:45.317048 intra42-0.1.4/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-31 21:42:45.317048 intra42-0.1.4/PKG-INFO
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:42:45.317048 intra42-0.1.4/intra42.egg-info/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/PKG-INFO
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/SOURCES.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/dependency_links.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/requires.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-31 21:42:45.000000 intra42-0.1.4/intra42.egg-info/top_level.txt
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-31 21:42:45.317048 intra42-0.1.4/intrascraper/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      304 2023-05-30 21:00:14.000000 intra42-0.1.4/intrascraper/__init__.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5553 2023-05-31 21:41:19.000000 intra42-0.1.4/intrascraper/intrascraper.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-31 21:42:45.317048 intra42-0.1.4/setup.cfg
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-31 21:42:33.000000 intra42-0.1.4/setup.py
```

### Comparing `intra42-0.1.3/intrascraper/intrascraper.py` & `intra42-0.1.4/intrascraper/intrascraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 from bs4 import BeautifulSoup, ResultSet
 import urllib.parse
 import urllib
 import typing
 from urllib import parse
 import typing
+import time
 
 KEYCLOAK = "https://profile.intra.42.fr/users/auth/keycloak_student"
 SEND_FORM = "https://auth.42.fr/auth/realms/students-42/login-actions/authenticate"
 
 class Token(typing.TypedDict):
 	cookie:str
 	expires:int
@@ -25,50 +26,47 @@
 
 class SraperError(Exception):
 	pass
 
 class IntraScraper:
 	def __init__(self, creds:Creds = {}):
 		self.token: Token
-		self.creds = creds
 		self.token = {}
 		self.session = requests.session()
 
-	def set_login(self, login:str):
-		self.creds["login"] = login
-
-	def set_password(self, password:str):
-		self.creds["password"] = password
-
-	def get_token(self) -> str:
+	def get_token(self, login:str, password:str) -> Token:
 
 		response = self.session.get(KEYCLOAK)
 		connect_page = response.content
 
 		soup = BeautifulSoup(connect_page, "html.parser")
 		form = soup.find("form", {"id": "kc-form-login"})
 		send_forms_params = {t[0]:t[1] for t in urllib.parse.parse_qsl(form["action"].split('?')[1])}
 
-		data = urllib.parse.urlencode({"username":self.creds['login'], "password":self.creds['password']})
+		data = urllib.parse.urlencode({"username":login, "password":password})
 		x = self.session.post(SEND_FORM,
 			data=data,
 			headers=self.session.headers.update({
 				"Content-Type" : "application/x-www-form-urlencoded",
 				"Content-Length":f"{len(data)}"
 				}),
 			params=send_forms_params)
 
 		cookie = x.cookies.get("_intra_42_session_production")
 		for c in x.cookies:
-			print(c.name, c.name == '_intra_42_session_production', c.expires)
 			if c.name == '_intra_42_session_production':
 				self.token["expires"] = c.expires
 		self.token["cookie"] = cookie
+		return self.token
 
 	def do_request(self, f, *args, **kwargs):
+
+		if self.token["expires"] >= time.time():
+			print("Token seems to be expired...")
+
 		if ("cookies" in kwargs):
 			kwargs["cookies"].update({"_intra_42_session_production":self.token["cookie"]})
 		else:
 			kwargs["cookies"] = {"_intra_42_session_production":self.token["cookie"]}
 		return (f(*args, **kwargs))
 
 SCRAPER = IntraScraper()
@@ -114,15 +112,14 @@
 
 	try:
 		name = soup.find("a", {"href":"#keymodal-365993"}).string.split("'")[1].strip()
 	except:
 		name = None
 
 	tree_p = soup.find("div", {"id":"keymodal-365993"})
-	print(tree_p.prettify())
 	try:
 		tree_values = tree_p.find("table").find_all("tr")[1].find_all("th", {"style":'font-weight: normal;'})
 	except Exception as e:
 		print("Couldn't get tree values :", e)
 		return {"key_name":name, "key_signature":None, "vogsphere":None, "synced":None}
 	try:
 		signature = tree_values[0].string.strip()
```

