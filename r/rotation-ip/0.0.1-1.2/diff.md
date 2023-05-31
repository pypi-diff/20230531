# Comparing `tmp/rotation_ip-0.0.1.tar.gz` & `tmp/rotation-ip-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotation_ip-0.0.1.tar", last modified: Tue Dec  6 18:24:16 2022, max compression
+gzip compressed data, was "rotation-ip-1.2.tar", last modified: Wed May 31 19:46:28 2023, max compression
```

## Comparing `rotation_ip-0.0.1.tar` & `rotation-ip-1.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxr-x   0 anish     (1000) anish     (1000)        0 2022-12-06 18:24:16.983687 rotation_ip-0.0.1/
--rw-rw-r--   0 anish     (1000) anish     (1000)     1062 2022-12-04 16:16:22.000000 rotation_ip-0.0.1/LICENSE
--rw-rw-r--   0 anish     (1000) anish     (1000)      652 2022-12-06 18:24:16.983687 rotation_ip-0.0.1/PKG-INFO
--rw-rw-r--   0 anish     (1000) anish     (1000)      138 2022-12-06 11:19:07.000000 rotation_ip-0.0.1/README.md
--rw-rw-r--   0 anish     (1000) anish     (1000)      651 2022-12-06 18:23:21.000000 rotation_ip-0.0.1/pyproject.toml
--rw-rw-r--   0 anish     (1000) anish     (1000)       38 2022-12-06 18:24:16.983687 rotation_ip-0.0.1/setup.cfg
-drwxrwxr-x   0 anish     (1000) anish     (1000)        0 2022-12-06 18:24:16.979687 rotation_ip-0.0.1/src/
-drwxrwxr-x   0 anish     (1000) anish     (1000)        0 2022-12-06 18:24:16.983687 rotation_ip-0.0.1/src/roation_ip/
--rw-rw-r--   0 anish     (1000) anish     (1000)       30 2022-12-06 14:12:27.000000 rotation_ip-0.0.1/src/roation_ip/__init__.py
--rw-rw-r--   0 anish     (1000) anish     (1000)     2799 2022-12-04 16:16:22.000000 rotation_ip-0.0.1/src/roation_ip/rotation_ip.py
-drwxrwxr-x   0 anish     (1000) anish     (1000)        0 2022-12-06 18:24:16.983687 rotation_ip-0.0.1/src/rotation_ip.egg-info/
--rw-rw-r--   0 anish     (1000) anish     (1000)      652 2022-12-06 18:24:16.000000 rotation_ip-0.0.1/src/rotation_ip.egg-info/PKG-INFO
--rw-rw-r--   0 anish     (1000) anish     (1000)      283 2022-12-06 18:24:16.000000 rotation_ip-0.0.1/src/rotation_ip.egg-info/SOURCES.txt
--rw-rw-r--   0 anish     (1000) anish     (1000)        1 2022-12-06 18:24:16.000000 rotation_ip-0.0.1/src/rotation_ip.egg-info/dependency_links.txt
--rw-rw-r--   0 anish     (1000) anish     (1000)       29 2022-12-06 18:24:16.000000 rotation_ip-0.0.1/src/rotation_ip.egg-info/requires.txt
--rw-rw-r--   0 anish     (1000) anish     (1000)       11 2022-12-06 18:24:16.000000 rotation_ip-0.0.1/src/rotation_ip.egg-info/top_level.txt
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 19:46:28.093338 rotation-ip-1.2/
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 19:46:28.089668 rotation-ip-1.2/.github/
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 19:46:28.090859 rotation-ip-1.2/.github/workflows/
+-rw-r--r--   0 anish      (501) staff       (20)     1359 2023-05-31 19:37:36.000000 rotation-ip-1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 anish      (501) staff       (20)     1062 2023-05-31 19:35:29.000000 rotation-ip-1.2/LICENSE
+-rw-r--r--   0 anish      (501) staff       (20)     1164 2023-05-31 19:46:28.093101 rotation-ip-1.2/PKG-INFO
+-rw-r--r--   0 anish      (501) staff       (20)      655 2023-05-31 19:35:29.000000 rotation-ip-1.2/README.md
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 19:46:28.091233 rotation-ip-1.2/ip_rotator/
+-rw-r--r--   0 anish      (501) staff       (20)       29 2023-05-31 19:35:29.000000 rotation-ip-1.2/ip_rotator/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)     2860 2023-05-31 19:35:29.000000 rotation-ip-1.2/ip_rotator/ip_rotator.py
+-rw-r--r--   0 anish      (501) staff       (20)      698 2023-05-31 19:46:15.000000 rotation-ip-1.2/pyproject.toml
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 19:46:28.092320 rotation-ip-1.2/rotation_ip.egg-info/
+-rw-r--r--   0 anish      (501) staff       (20)     1164 2023-05-31 19:46:28.000000 rotation-ip-1.2/rotation_ip.egg-info/PKG-INFO
+-rw-r--r--   0 anish      (501) staff       (20)      329 2023-05-31 19:46:28.000000 rotation-ip-1.2/rotation_ip.egg-info/SOURCES.txt
+-rw-r--r--   0 anish      (501) staff       (20)        1 2023-05-31 19:46:28.000000 rotation-ip-1.2/rotation_ip.egg-info/dependency_links.txt
+-rw-r--r--   0 anish      (501) staff       (20)       29 2023-05-31 19:46:28.000000 rotation-ip-1.2/rotation_ip.egg-info/requires.txt
+-rw-r--r--   0 anish      (501) staff       (20)       11 2023-05-31 19:46:28.000000 rotation-ip-1.2/rotation_ip.egg-info/top_level.txt
+-rw-r--r--   0 anish      (501) staff       (20)       38 2023-05-31 19:46:28.093398 rotation-ip-1.2/setup.cfg
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-05-31 19:46:28.092739 rotation-ip-1.2/tests/
+-rw-r--r--   0 anish      (501) staff       (20)        0 2023-05-31 19:35:29.000000 rotation-ip-1.2/tests/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)     3193 2023-05-31 19:35:29.000000 rotation-ip-1.2/tests/ip_rotator.py
```

### Comparing `rotation_ip-0.0.1/LICENSE` & `rotation-ip-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rotation_ip-0.0.1/src/roation_ip/rotation_ip.py` & `rotation-ip-1.2/ip_rotator/ip_rotator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests
+import requests , time
 from bs4 import BeautifulSoup
 
 class Proxy:
     
     def __init__(self,https=False):
         '''
         Set https = True if you wish to use an HTTPS website. \n
@@ -19,39 +19,37 @@
         self.setProxy()
         
         
     def updateIpList(self):
         '''
         This Method Pulls All Free Proxy Server From The Website https://free-proxy-list.net/.
         '''
+        self.timeOfUpdate = time.time()
+        self.id = 0
         proxyList = requests.get('https://free-proxy-list.net/')
         soup = BeautifulSoup(proxyList.text,'lxml')
         self.listOfIp = soup.find('tbody').findAll('tr')
     
     def setProxy(self):  
         '''
         This Method Gathers All Available Free Proxy Servers And Establishes A Connection With Them.        
         '''
-        self.id = 0
         self.updateIpList()
         self.session = requests.Session()
-        self.nextIp()
+        self.changeIp()
         # return session
         
-    def nextIp(self):
+    def changeIp(self):
         '''
         This Method Finds The Next Proxy Server That Is Available And Connects To It.
         '''
         while True:
-            try:
-                data = self.listOfIp[self.id].findAll('td')
-            except:
+            if 350 <= int(time.time() - self.timeOfUpdate):                  # update list every 5 min 
                 self.updateIpList()
-                self.id = 0
-                continue
+            data = self.listOfIp[self.id].findAll('td')
             self.currentIp = data[0].text
             proxyPort = data[1].text
             country = data[3].text
             is_https = data[6].text
             if self.https and is_https == 'no':
                 self.id+=1
                 continue
```

