# Comparing `tmp/instagpy-0.1.2.tar.gz` & `tmp/instagpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagpy-0.1.2.tar", last modified: Mon May 22 12:25:42 2023, max compression
+gzip compressed data, was "instagpy-0.1.3.tar", last modified: Wed May 31 15:13:13 2023, max compression
```

## Comparing `instagpy-0.1.2.tar` & `instagpy-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 12:25:42.034289 instagpy-0.1.2/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3318 2023-05-22 12:25:42.034289 instagpy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 12:25:42.023415 instagpy-0.1.2/instagpy/
--rw-rw-rw-   0        0        0       32 2023-05-20 05:51:40.000000 instagpy-0.1.2/instagpy/__init__.py
--rw-rw-rw-   0        0        0    20519 2023-05-22 12:17:53.000000 instagpy-0.1.2/instagpy/instagpy.py
--rw-rw-rw-   0        0        0     2019 2023-05-22 09:57:02.000000 instagpy-0.1.2/instagpy/path.py
--rw-rw-rw-   0        0        0     1014 2023-05-19 17:37:45.000000 instagpy-0.1.2/instagpy/request_util.py
--rw-rw-rw-   0        0        0     2512 2023-05-20 05:51:32.000000 instagpy-0.1.2/instagpy/session_util.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 12:05:19.000000 instagpy-0.1.2/instagpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 12:25:42.034289 instagpy-0.1.2/instagpy.egg-info/
--rw-rw-rw-   0        0        0     3318 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 12:25:41.000000 instagpy-0.1.2/instagpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 12:25:42.034289 instagpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1486 2023-05-22 12:25:08.000000 instagpy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:13:13.146643 instagpy-0.1.3/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 instagpy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-05-20 05:58:51.000000 instagpy-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3318 2023-05-31 15:13:13.146643 instagpy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2256 2023-05-22 12:22:05.000000 instagpy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 15:13:13.131008 instagpy-0.1.3/instagpy/
+-rw-rw-rw-   0        0        0       32 2023-05-20 05:51:40.000000 instagpy-0.1.3/instagpy/__init__.py
+-rw-rw-rw-   0        0        0    20509 2023-05-31 15:01:45.000000 instagpy-0.1.3/instagpy/instagpy.py
+-rw-rw-rw-   0        0        0     2019 2023-05-22 09:57:02.000000 instagpy-0.1.3/instagpy/path.py
+-rw-rw-rw-   0        0        0     1092 2023-05-31 15:11:43.000000 instagpy-0.1.3/instagpy/request_util.py
+-rw-rw-rw-   0        0        0     2512 2023-05-20 05:51:32.000000 instagpy-0.1.3/instagpy/session_util.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 12:34:47.000000 instagpy-0.1.3/instagpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:13:13.131008 instagpy-0.1.3/instagpy.egg-info/
+-rw-rw-rw-   0        0        0     3318 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 15:13:12.000000 instagpy-0.1.3/instagpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 15:13:13.146643 instagpy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2023-05-31 15:09:06.000000 instagpy-0.1.3/setup.py
```

### Comparing `instagpy-0.1.2/LICENSE` & `instagpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.2/PKG-INFO` & `instagpy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.2 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.3 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.2/README.md` & `instagpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.2/instagpy/instagpy.py` & `instagpy-0.1.3/instagpy/instagpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,17 @@
             self.session.cookies.update({'sessionid': session_id})
             return
         self.session.cookies = response.cookies
         self.session.headers.update(
             {'x-csrftoken': csrf_token, 'X-Requested-With': "XMLHttpRequest", 'Referer': login_page_url})
 
     def shuffle_session(self):
+        if not self.use_mutiple_account:
+            return
+        self.current_request_number += 1
         if self.current_request_number % self.shuffle_session_after == 0:
             self.shuffle_session_after = random.randint(
                 self.min_requests, self.max_requests)
             if not self.session_ids_container:
                 self.session_ids_container = self.session_ids.copy()
             session_id = self.session_ids_container.pop()
             self.generate_session(session_id=session_id)
@@ -180,15 +183,18 @@
 
         Args:
             username (str): Instagram username.
 
         Returns:
             dict: user info like username,id,bio,follower/following count etc.
         """
-        return make_request(user_profile_endpoint.format(username), session=self.session, max_retries=self.max_retries)
+        response = make_request(user_profile_endpoint.format(
+            username), session=self.session, max_retries=self.max_retries)
+        self.shuffle_session()
+        return response
 
     def get_user_data(self, user_id):
         """Extracts user details. With Contact Info Like email, phone and address.
 
         Args:
             user_id (int): User ID of an Instagram User.
 
@@ -197,17 +203,15 @@
         """
         # returns almost as same data as get_user_info method Except this one returns contact info (email/phone) as well. |LOGIN REQUIRED|
         if not self.logged_in():
             self.login()
         user_id = self.get_user_id(user_id)
         response = make_request(user_data_endpoint.format(
             user_id), session=self.session, max_retries=self.max_retries)
-        if self.use_mutiple_account:
-            self.current_request_number += 1
-            self.shuffle_session()
+        self.shuffle_session()
         return response
 
     def get_user_basic_details(self, username=None, print_formatted=False):
         """Get a brief overview of an Instagram Profile.
 
         Args:
             username (str, optional): Instagram Username. Defaults to None.
@@ -293,17 +297,15 @@
                 user_friends.extend(data)
 
                 print(
                     f"{user['username']} : {len(user_friends)} / {count}", end="\r")
                 if not has_next_page or (max is not None and len(user_friends) >= max):
                     return user_friends
 
-                if self.use_mutiple_account:
-                    self.current_request_number += 1
-                    self.shuffle_session()
+                self.shuffle_session()
 
             except ConnectionError as error:
                 print(error)
                 continue
 
             except Exception as error:
                 print(error)
@@ -376,17 +378,15 @@
                 if from_date:
                     if any(datetime.datetime.fromtimestamp(post['node']['taken_at_timestamp']) <= from_date for post in data['edges']):
                         return user_posts_data
 
                 if not has_next_page or (max is not None and len(user_posts_data) >= max):
                     return user_posts_data
 
-                if self.use_mutiple_account:
-                    self.current_request_number += 1
-                    self.shuffle_session()
+                self.shuffle_session()
 
         except Exception as e:
             print(e)
 
     def get_post_details(self, post_url):
         """Get details of a particular Instagram Post/Media.
 
@@ -396,15 +396,18 @@
         Returns:
             dict: All the details like post_id,datetime,caption,url,location etc.
         """
         post_id = utils.get_post_id(post_url)
         url = graphql_url
         query_params = self.generate_query(
             query=post_details_query, shortcode=post_id, is_graphql=True)
-        return make_request(url, params=query_params, session=self.session, max_retries=self.max_retries)
+        response = make_request(
+            url, params=query_params, session=self.session, max_retries=self.max_retries)
+        self.shuffle_session()
+        return response
 
     def get_media_url(self, response):
         """Extracts High Resolution/Quality Media URL from post details response returned from get_post_details method.
 
         Args:
             response (dict): Response returned from get_post_details method.
 
@@ -436,12 +439,13 @@
         user_id = self.get_user_id(username)
         data = {'referer_type': 'ProfileUsername', 'target_user_id': user_id, 'bk_client_context': {
             'bloks_version': about_user_query, 'style_id': 'instagram'}, 'bloks_versioning_id': about_user_query}
         response = make_request(about_user_url, method='POST', data=data,
                                 session=self.session, max_retries=self.max_retries)
         if print_formatted:
             return utils.format_about_data(response)
+        self.shuffle_session()
         return response
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `instagpy-0.1.2/instagpy/path.py` & `instagpy-0.1.3/instagpy/path.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.2/instagpy/request_util.py` & `instagpy-0.1.3/instagpy/request_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import requests
 import bs4
 
 
-def make_request(url, session=None, method=None, max_retries=None, **kwargs):
+def make_request(url, session=None, method=None, max_retries=None, timeout=None, **kwargs):
     if method is None:
         method = "GET"
     if max_retries is None:
         max_retries = 3
     if session is None:
         session = requests.Session()
+    if timeout is None:
+        timeout = 30
     for retry_count, retry in enumerate(range(max_retries), start=1):
         try:
-            response = session.request(method, url, **kwargs)
+            response = session.request(method, url, timeout=timeout, **kwargs)
             response.raise_for_status()
             soup = bs4.BeautifulSoup(response.content, "lxml")
             if "json" in response.headers["Content-Type"]:
                 return response.json()
             return soup
         except KeyboardInterrupt:
             print("Keyboard Interruption...")
```

### Comparing `instagpy-0.1.2/instagpy/session_util.py` & `instagpy-0.1.3/instagpy/session_util.py`

 * *Files identical despite different names*

### Comparing `instagpy-0.1.2/instagpy/utils.py` & `instagpy-0.1.3/instagpy/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,14 @@
         post_data = urlparse(post_url).path.split('/p/')[-1].split('/')
     post_data = [data for data in post_data if data.strip()]
     post_id = post_data[1] if len(post_data) > 1 else post_data[0]
 
     return post_id
 
 
-if __name__ == '__main__':
-    pass
-
-
 def format_about_data(response, placeholder=None):
     if placeholder is None or not isinstance(placeholder, dict):
         placeholder = {}
     if isinstance(response, list):
         for item in response:
             format_about_data(item, placeholder)
     elif isinstance(response, dict):
@@ -56,7 +52,11 @@
     for key, value in placeholder.items():
         if value is None:
             continue
         if 'bk.action.array.Make' in value and key.endswith('about_this_account_country'):
             placeholder[key] = value.split(
                 'bk.action.array.Make,')[-1].split(")")[0].replace('"', '').strip()
     return placeholder
+
+
+if __name__ == '__main__':
+    pass
```

### Comparing `instagpy-0.1.2/instagpy.egg-info/PKG-INFO` & `instagpy-0.1.3/instagpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc.
 Home-page: https://github.com/iSarabjitDhiman/InstaGPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: instagpy,instagram scraper,instagram email scraper,insta data extraction,instagram api,instagram python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: instagpy Version: 0.1.2 Summary: InstaGPy is an
+Metadata-Version: 2.1 Name: instagpy Version: 0.1.3 Summary: InstaGPy is an
 Instagram Unofficial API to extract data from Instargam Profiles. Scrape data
 from user's profile like username, userid, bio, email, phone, followers/
 followings list, profile media, account_type, etc. Home-page: https://
 github.com/iSarabjitDhiman/InstaGPy Author: Sarabjit Dhiman Author-email:
 hello@sarabjitdhiman.com License: MIT Keywords: instagpy,instagram
 scraper,instagram email scraper,insta data extraction,instagram api,instagram
 python Classifier: Development Status :: 3 - Alpha Classifier: Intended
```

### Comparing `instagpy-0.1.2/setup.py` & `instagpy-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 SHORT_DESCRIPTION = "InstaGPy is an Instagram Unofficial API to extract data from Instargam Profiles. Scrape data from user's profile like username, userid, bio, email, phone, followers/followings list, profile media, account_type, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

