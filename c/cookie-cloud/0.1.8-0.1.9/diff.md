# Comparing `tmp/cookie_cloud-0.1.8-py2.py3-none-any.whl.zip` & `tmp/cookie_cloud-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17015 bytes, number of entries: 9
+Zip file size: 17068 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-20 09:21 cookie_cloud/__init__.py
 -rw-r--r--  2.0 unx     7543 b- defN 22-Sep-27 00:14 cookie_cloud/generate.py
--rw-r--r--  2.0 unx     1949 b- defN 22-Dec-31 13:59 cookie_cloud/util.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Dec-31 14:02 cookie_cloud-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1200 b- defN 22-Dec-31 14:02 cookie_cloud-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Dec-31 14:02 cookie_cloud-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 22-Dec-31 14:02 cookie_cloud-0.1.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 22-Dec-31 14:02 cookie_cloud-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      749 b- defN 22-Dec-31 14:02 cookie_cloud-0.1.8.dist-info/RECORD
-9 files, 46772 bytes uncompressed, 15715 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     2116 b- defN 23-Jan-04 06:39 cookie_cloud/util.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jan-04 06:41 cookie_cloud-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1200 b- defN 23-Jan-04 06:41 cookie_cloud-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jan-04 06:41 cookie_cloud-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jan-04 06:41 cookie_cloud-0.1.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Jan-04 06:41 cookie_cloud-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      749 b- defN 23-Jan-04 06:41 cookie_cloud-0.1.9.dist-info/RECORD
+9 files, 46939 bytes uncompressed, 15768 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: cookie_cloud/generate.py
 Comment: 
 
 Filename: cookie_cloud/util.py
 Comment: 
 
-Filename: cookie_cloud-0.1.8.dist-info/LICENSE
+Filename: cookie_cloud-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: cookie_cloud-0.1.8.dist-info/METADATA
+Filename: cookie_cloud-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: cookie_cloud-0.1.8.dist-info/WHEEL
+Filename: cookie_cloud-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: cookie_cloud-0.1.8.dist-info/entry_points.txt
+Filename: cookie_cloud-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: cookie_cloud-0.1.8.dist-info/top_level.txt
+Filename: cookie_cloud-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: cookie_cloud-0.1.8.dist-info/RECORD
+Filename: cookie_cloud-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cookie_cloud/util.py

```diff
@@ -10,15 +10,15 @@
 
 conf_path = ".cookie_cloud.json"
 if not os.path.isfile(conf_path):
     conf_path = os.path.join(HOME, ".cookie_cloud.json")
 
 
 COOKIES_PATH = os.path.join(TMP_DIR, "cookies.json")
-conf = json.load(open(conf_path))
+conf = json.load(open(conf_path)) if os.path.isfile(conf_path) else {}
 
 
 headers = {
     "Accept": "application/vnd.github.v3+json",
     "Authorization": "token " + conf["github_token"],
 }
 
@@ -50,16 +50,20 @@
     )
     data = git_get(url)
     if not data:
         return
     return data[-1]["url"]
 
 
-def get_cookie(site, update=False, raw=False):
+def get_cookie(site, update=False, raw=False, user=None, repo=None):
+    global conf
     cookies = {}
+    if user and repo:
+        conf["github_user"] = user
+        conf["github_repo"] = repo
     if os.path.isfile(COOKIES_PATH) and not update:
         cookies_str = open(COOKIES_PATH).read()
         cookies = json.loads(cookies_str) if cookies_str else {}
     if cookies.get(site):
         return cookies[site]
     data = get_comment_body(get_issue_url(site))
     cookie = data
```

## Comparing `cookie_cloud-0.1.8.dist-info/LICENSE` & `cookie_cloud-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cookie_cloud-0.1.8.dist-info/METADATA` & `cookie_cloud-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookie-cloud
-Version: 0.1.8
+Version: 0.1.9
 Summary: Get cookie through Tampermonkey, use cookie anywhere.
 Home-page: https://github.com/twfb/cookie_cloud
 Author: twfb
 Author-email: twfb@hotmail.com
 Maintainer: twfb
 Maintainer-email: twfb@hotmail.com
 License: BSD License
```

