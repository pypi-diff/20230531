# Comparing `tmp/webscapy-1.4.3.tar.gz` & `tmp/webscapy-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscapy-1.4.3.tar", last modified: Tue May 30 01:32:34 2023, max compression
+gzip compressed data, was "webscapy-1.4.4.tar", last modified: Wed May 31 07:22:49 2023, max compression
```

## Comparing `webscapy-1.4.3.tar` & `webscapy-1.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 01:32:34.812758 webscapy-1.4.3/
--rw-rw-rw-   0        0        0     5494 2023-05-30 01:32:34.812758 webscapy-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5199 2023-05-30 01:29:16.000000 webscapy-1.4.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 01:32:34.812758 webscapy-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-05-30 01:32:17.000000 webscapy-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 01:32:34.736556 webscapy-1.4.3/webscapy/
--rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.4.3/webscapy/__init__.py
--rw-rw-rw-   0        0        0     4458 2023-05-30 01:25:00.000000 webscapy-1.4.3/webscapy/webscapy.py
-drwxrwxrwx   0        0        0        0 2023-05-30 01:32:34.805158 webscapy-1.4.3/webscapy.egg-info/
--rw-rw-rw-   0        0        0     5494 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-30 01:32:34.000000 webscapy-1.4.3/webscapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 07:22:49.769841 webscapy-1.4.4/
+-rw-rw-rw-   0        0        0     5648 2023-05-31 07:22:49.766813 webscapy-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5353 2023-05-31 07:21:46.000000 webscapy-1.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:22:49.769841 webscapy-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-05-31 07:22:30.000000 webscapy-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:22:49.686485 webscapy-1.4.4/webscapy/
+-rw-rw-rw-   0        0        0       30 2023-05-28 06:36:42.000000 webscapy-1.4.4/webscapy/__init__.py
+-rw-rw-rw-   0        0        0     5412 2023-05-31 07:15:48.000000 webscapy-1.4.4/webscapy/webscapy.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:22:49.763784 webscapy-1.4.4/webscapy.egg-info/
+-rw-rw-rw-   0        0        0     5648 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-31 07:22:49.000000 webscapy-1.4.4/webscapy.egg-info/top_level.txt
```

### Comparing `webscapy-1.4.3/PKG-INFO` & `webscapy-1.4.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: webscapy
-Version: 1.4.3
-Summary: Selenium built for scraping instead of testing
-Author: Rahul Raj
-Project-URL: Documentation, https://pypi.org/project/webscapy/
-Project-URL: Source, https://pypi.org/project/webscapy/
-Description-Content-Type: text/markdown
-
 # Webscapy: Selenium Configured for Webscraping
 
 ## Introduction
 
 Webscapy is a Python package that extends the capabilities of the Selenium framework, originally designed for web testing, to perform web scraping tasks. It provides a convenient and easy-to-use interface for automating browser interactions, navigating through web pages, and extracting data from websites. By combining the power of Selenium with the flexibility of web scraping, Webscapy enables you to extract structured data from dynamic websites efficiently.
 
 ## Features
@@ -142,15 +133,27 @@
 cookie = {
    "name": "cookie1",
    "value": "value1"
 }
 driver.add_cookie(cookie)
 ```
 
-2. Import cookie from JSON
+2. Get a single cookie
+
+```python
+driver.get_cookie("cookie1")
+```
+
+3. Delete a single cookie
+
+```python
+driver.delete_cookie("cookie1")
+```
+
+4. Import cookie from JSON
 
 ```
 driver.load_cookie_json("cookie.json")
 ```
 
 ## Close the driver
```

### Comparing `webscapy-1.4.3/README.md` & `webscapy-1.4.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: webscapy
+Version: 1.4.4
+Summary: Selenium built for scraping instead of testing
+Author: Rahul Raj
+Project-URL: Documentation, https://pypi.org/project/webscapy/
+Project-URL: Source, https://pypi.org/project/webscapy/
+Description-Content-Type: text/markdown
+
 # Webscapy: Selenium Configured for Webscraping
 
 ## Introduction
 
 Webscapy is a Python package that extends the capabilities of the Selenium framework, originally designed for web testing, to perform web scraping tasks. It provides a convenient and easy-to-use interface for automating browser interactions, navigating through web pages, and extracting data from websites. By combining the power of Selenium with the flexibility of web scraping, Webscapy enables you to extract structured data from dynamic websites efficiently.
 
 ## Features
@@ -133,15 +142,27 @@
 cookie = {
    "name": "cookie1",
    "value": "value1"
 }
 driver.add_cookie(cookie)
 ```
 
-2. Import cookie from JSON
+2. Get a single cookie
+
+```python
+driver.get_cookie("cookie1")
+```
+
+3. Delete a single cookie
+
+```python
+driver.delete_cookie("cookie1")
+```
+
+4. Import cookie from JSON
 
 ```
 driver.load_cookie_json("cookie.json")
 ```
 
 ## Close the driver
```

### Comparing `webscapy-1.4.3/setup.py` & `webscapy-1.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="webscapy",
-    version="1.4.3",
+    version="1.4.4",
     description="Selenium built for scraping instead of testing",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Rahul Raj",
     packages=["webscapy"],
     zip_safe=False,
     project_urls={
```

### Comparing `webscapy-1.4.3/webscapy/webscapy.py` & `webscapy-1.4.4/webscapy/webscapy.py`

 * *Files 18% similar despite different names*

```diff
@@ -113,15 +113,42 @@
         network_data = self.driver.execute_script(network_data_retriever_script)
 
         return network_data
 
     def add_cookie(self, cookie):
         self.driver.add_cookie(cookie)
 
+    def get_cookie(self, name):
+        return self.driver.get_cookie(name)
+    
+    def delete_cookie(self, name):
+        self.driver.delete_cookie(name)
+
+    def cookie_editor_parser(self, cookie):
+        if cookie["sameSite"] == "lax":
+            cookie["sameSite"] = "Lax"
+        if cookie["sameSite"] == "no_restriction":
+            cookie["sameSite"] = "None"
+        if cookie["sameSite"] == "strict":
+            cookie["sameSite"] = "Strict"
+        return cookie
+
+    def is_host_cookie(self, cookie):
+        cookie_name = cookie["name"]
+        if cookie_name.startswith("__Host"):
+            return True
+        return False
+
     def load_cookie_json(self, path):
         file = open(path, "r")
         cookies = json.load(file)
         for cookie in cookies:
+            cookie = self.cookie_editor_parser(cookie)
+            cookie_name = cookie["name"]
+            if self.get_cookie(cookie_name) is not None:
+                self.delete_cookie(cookie_name)
+            if self.is_host_cookie(cookie):
+                del cookie["domain"]
             self.add_cookie(cookie)
 
     def close(self):
         self.driver.close()
```

### Comparing `webscapy-1.4.3/webscapy.egg-info/PKG-INFO` & `webscapy-1.4.4/webscapy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscapy
-Version: 1.4.3
+Version: 1.4.4
 Summary: Selenium built for scraping instead of testing
 Author: Rahul Raj
 Project-URL: Documentation, https://pypi.org/project/webscapy/
 Project-URL: Source, https://pypi.org/project/webscapy/
 Description-Content-Type: text/markdown
 
 # Webscapy: Selenium Configured for Webscraping
@@ -142,15 +142,27 @@
 cookie = {
    "name": "cookie1",
    "value": "value1"
 }
 driver.add_cookie(cookie)
 ```
 
-2. Import cookie from JSON
+2. Get a single cookie
+
+```python
+driver.get_cookie("cookie1")
+```
+
+3. Delete a single cookie
+
+```python
+driver.delete_cookie("cookie1")
+```
+
+4. Import cookie from JSON
 
 ```
 driver.load_cookie_json("cookie.json")
 ```
 
 ## Close the driver
```

