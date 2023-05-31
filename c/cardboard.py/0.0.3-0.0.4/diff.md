# Comparing `tmp/cardboard.py-0.0.3.tar.gz` & `tmp/cardboard.py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardboard.py-0.0.3.tar", last modified: Wed May 31 21:27:10 2023, max compression
+gzip compressed data, was "cardboard.py-0.0.4.tar", last modified: Wed May 31 21:30:33 2023, max compression
```

## Comparing `cardboard.py-0.0.3.tar` & `cardboard.py-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 21:27:10.703667 cardboard.py-0.0.3/
--rw-rw-rw-   0        0        0     4262 2023-05-31 21:27:10.701516 cardboard.py-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3333 2023-05-31 21:26:13.000000 cardboard.py-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 21:27:10.678458 cardboard.py-0.0.3/cardboard/
--rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.3/cardboard/Exceptions.py
--rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.3/cardboard/__init__.py
--rw-rw-rw-   0        0        0    10938 2023-05-31 20:26:53.000000 cardboard.py-0.0.3/cardboard/cardboard.py
--rw-rw-rw-   0        0        0    10971 2023-05-31 21:26:54.000000 cardboard.py-0.0.3/cardboard/cardboard_async.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:27:10.696818 cardboard.py-0.0.3/cardboard.py.egg-info/
--rw-rw-rw-   0        0        0     4262 2023-05-31 21:27:10.000000 cardboard.py-0.0.3/cardboard.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-31 21:27:10.000000 cardboard.py-0.0.3/cardboard.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 21:27:10.000000 cardboard.py-0.0.3/cardboard.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-31 21:27:10.000000 cardboard.py-0.0.3/cardboard.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-31 21:27:10.000000 cardboard.py-0.0.3/cardboard.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 21:27:10.703667 cardboard.py-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-05-31 21:26:36.000000 cardboard.py-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:30:33.932531 cardboard.py-0.0.4/
+-rw-rw-rw-   0        0        0     4262 2023-05-31 21:30:33.931535 cardboard.py-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3333 2023-05-31 21:26:13.000000 cardboard.py-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 21:30:33.908668 cardboard.py-0.0.4/cardboard/
+-rw-rw-rw-   0        0        0     1142 2023-05-31 14:44:31.000000 cardboard.py-0.0.4/cardboard/Exceptions.py
+-rw-rw-rw-   0        0        0      122 2023-05-31 14:42:16.000000 cardboard.py-0.0.4/cardboard/__init__.py
+-rw-rw-rw-   0        0        0    10934 2023-05-31 21:29:50.000000 cardboard.py-0.0.4/cardboard/cardboard.py
+-rw-rw-rw-   0        0        0    10967 2023-05-31 21:30:09.000000 cardboard.py-0.0.4/cardboard/cardboard_async.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:30:33.927540 cardboard.py-0.0.4/cardboard.py.egg-info/
+-rw-rw-rw-   0        0        0     4262 2023-05-31 21:30:33.000000 cardboard.py-0.0.4/cardboard.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-31 21:30:33.000000 cardboard.py-0.0.4/cardboard.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 21:30:33.000000 cardboard.py-0.0.4/cardboard.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-31 21:30:33.000000 cardboard.py-0.0.4/cardboard.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 21:30:33.000000 cardboard.py-0.0.4/cardboard.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 21:30:33.933541 cardboard.py-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-05-31 21:30:19.000000 cardboard.py-0.0.4/setup.py
```

### Comparing `cardboard.py-0.0.3/PKG-INFO` & `cardboard.py-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.3
+Version: 0.0.4
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardboard.py-0.0.3/README.md` & `cardboard.py-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.3/cardboard/Exceptions.py` & `cardboard.py-0.0.4/cardboard/Exceptions.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.3/cardboard/cardboard.py` & `cardboard.py-0.0.4/cardboard/cardboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
             Returns:
                 bool|list: [True, app_name] if everything is valid, else False.
             """
             resp = requests.post(self._base_url+'/check', headers={'Content-Type': 'application/x-www-form-urlencoded'}, data={'client_id': self.client_id, 'client_secret': self.secret})
             if resp.status_code != 200:
                 return False
-            return [True, resp.json()['app_name']]
+            return [True, resp.json()['name']]
     
         self.__check_verify = lambda: __check_verify(self)
 
         self._valid = self.__check_verify()
         if self._valid is False:
             raise CardboardException("Invalid credentials provided. (Is your ID and Secret correct?)")
         self.app_name = self._valid[1]
```

### Comparing `cardboard.py-0.0.3/cardboard/cardboard_async.py` & `cardboard.py-0.0.4/cardboard/cardboard_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
             Returns:
                 bool|list: [True, app_name] if everything is valid, else False.
             """
             resp = requests.post(self._base_url+'/check', headers={'Content-Type': 'application/x-www-form-urlencoded'}, data={'client_id': self.client_id, 'client_secret': self.secret})
             if resp.status_code != 200:
                 return False
-            return [True, resp.json()['app_name']]
+            return [True, resp.json()['name']]
     
         self.__check_verify = lambda: __check_verify(self)
 
         self._valid = self.__check_verify()
         if self._valid is False:
             raise CardboardException("Invalid credentials provided. (Is your ID and Secret correct?)")
         self.app_name = self._valid[1]
```

### Comparing `cardboard.py-0.0.3/cardboard.py.egg-info/PKG-INFO` & `cardboard.py-0.0.4/cardboard.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.3
+Version: 0.0.4
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardboard.py-0.0.3/setup.py` & `cardboard.py-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cardboard.py',
-    version='0.0.3',
+    version='0.0.4',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://cardboard.ink/api/v1/',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cardboard-ink/cardboard.py/',
     packages=find_packages(),
```

