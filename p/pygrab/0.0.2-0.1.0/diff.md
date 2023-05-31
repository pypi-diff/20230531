# Comparing `tmp/pygrab-0.0.2.tar.gz` & `tmp/pygrab-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrab-0.0.2.tar", last modified: Tue May 30 03:21:07 2023, max compression
+gzip compressed data, was "pygrab-0.1.0.tar", last modified: Wed May 31 05:44:58 2023, max compression
```

## Comparing `pygrab-0.0.2.tar` & `pygrab-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 03:21:07.562798 pygrab-0.0.2/
--rw-rw-rw-   0        0        0      183 2023-05-30 03:21:07.561640 pygrab-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-05-30 02:43:17.000000 pygrab-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 03:21:07.552008 pygrab-0.0.2/pygrab/
--rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-0.0.2/pygrab/__init__.py
--rw-rw-rw-   0        0        0     8586 2023-05-30 03:15:50.000000 pygrab-0.0.2/pygrab/pygrab.py
-drwxrwxrwx   0        0        0        0 2023-05-30 03:21:07.558308 pygrab-0.0.2/pygrab.egg-info/
--rw-rw-rw-   0        0        0      183 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 03:21:07.000000 pygrab-0.0.2/pygrab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 03:21:07.563289 pygrab-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      343 2023-05-30 03:20:34.000000 pygrab-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:44:58.110000 pygrab-0.1.0/
+-rw-rw-rw-   0        0        0      183 2023-05-31 05:44:58.098000 pygrab-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-05-31 05:39:15.000000 pygrab-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 05:44:57.992000 pygrab-0.1.0/pygrab/
+-rw-rw-rw-   0        0        0       21 2023-05-30 03:16:15.000000 pygrab-0.1.0/pygrab/__init__.py
+-rw-rw-rw-   0        0        0    10511 2023-05-31 05:32:43.000000 pygrab-0.1.0/pygrab/pygrab.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:44:58.081000 pygrab-0.1.0/pygrab.egg-info/
+-rw-rw-rw-   0        0        0      183 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 05:44:57.000000 pygrab-0.1.0/pygrab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 05:44:58.107000 pygrab-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      338 2023-05-31 05:42:52.000000 pygrab-0.1.0/setup.py
```

### Comparing `pygrab-0.0.2/pygrab/pygrab.py` & `pygrab-0.1.0/pygrab/pygrab.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 # Author: Anish Kanthamneni
 import requests as _requests
-from bs4 import BeautifulSoup as _BeautifulSoup
+from pyppeteer import launch as _launch
 from random import choice as _choice
+import asyncio as _asyncio
 
 class ProxyList():
     PROXY_LIST = []
     
     @classmethod
     def is_empty(cls):
         return cls.PROXY_LIST == []
     
     @classmethod
     def get_random(cls):
+        
+        high_quality = []
+        
+        for ip in cls.PROXY_LIST:
+            if ip[4] == 'Transparent':
+                continue
+            elif int(ip[-1]) < 550:
+                continue
+            high_quality.append(ip)
+        
+        if high_quality != []:
+            x = _choice(high_quality)
+            print (x)
+            print (f'length: {len(cls.PROXY_LIST)}')
+            return x
         return _choice(cls.PROXY_LIST)
     
     @classmethod
     def update_proxies(cls):
         while (cls.PROXY_LIST != []): cls.PROXY_LIST.pop(0)
-        cls.gen_proxies(cls.PROXY_LIST)
+        cls.gen_proxies()
+    
+    @classmethod
+    async def grab_proxies_async(cls):
+        browser = await _launch()
+        page = await browser.newPage()
+        await page.goto('https://proxyscrape.com/free-proxy-list', waitUntil='networkidle0')
+        html = await page.content()    
+        await browser.close()
+        return html
     
     @classmethod
     def gen_proxies(cls):
+        def parse(row):
+            row = row.split('</td><td>')
+            row[-1] = row[4].split('>')[-1].replace('ms', '')
+            row[4] = row[4].split('<')[0]
+            return row
         try:
-            html = _requests.get('https://www.sslproxies.org/').text
-            # html = _requests.get('https://free-proxy-list.net/').text
-
-            # Parses it into the ideal format
-            soup = _BeautifulSoup(html, 'html.parser')
-            table = soup.find('table', {'class': 'table'})
-            rows = table.find_all('tr')
-            for row in rows[1:]:
-                cells = row.find_all('td')
-                ip_address = cells[0].text
-                port = cells[1].text
-                country = cells[3].text
-                https = cells[6].text
-                cls.PROXY_LIST.append([ip_address, port, country, https])
+            raw_html = _asyncio.get_event_loop().run_until_complete(cls.grab_proxies_async())
+            html = raw_html.split('</thead>')[1]
+            html = html.split('<tr><td>')
+            html.pop(0)
+            cls.PROXY_LIST = [parse(i) for i in html]
+            
         except Exception as err:
-            raise Exception(f'{err}\n\nThere seems to have been an error with finding a proxy IP. Please note that free proxies may not be reliable.')
+            raise Exception(f'{err}\n\n{raw_html}\n\nThere seems to have been an error with finding a proxy IP. Please note that free proxies may not be reliable.')
 
     @classmethod
     def set_proxies(cls, lst):
         if len(lst) == 0: 
             cls.PROXY_LIST = []
             return
         
@@ -60,15 +82,15 @@
                     
                 cls.PROXY_LIST.append(lst[i].split(':'))
         raise Exception("Incorrect formatting for setting proxies. Must be [['23.144.56.65', '8080'], ...] or ['23.144.56.65:8080', ...]")
 
 
 
 
-def get(url: str, use_proxy=False, retries=5, encoding='utf-8', *args, **kwargs): 
+def get(url: str, use_proxy=False, retries=5, encoding='utf-8', enable_js=False, *args, **kwargs): 
     """
     Gets the content at the specified URL.
 
     Parameters:
     url (str): The URL to get.
     use_proxy (bool, optional): Whether to use a proxy. Defaults to False.
     retries (int, optional): The number of times to retry the request if it fails. Defaults to 5.
@@ -80,37 +102,43 @@
     requests.Response: The response from the server.
     """
     local_file_starts = ['./', 'C:', '/'] 
     url_file_starts = ['http', 'ftp:', 'mailto:']
     if any([url.startswith(i) for i in local_file_starts]):
         return __local_grab(url, encoding=encoding)
     elif any([url.startswith(i) for i in url_file_starts]):
-        session = _requests.Session()
-        retry = _requests.packages.urllib3.util.retry.Retry(total=retries, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504])
-        adapter = _requests.adapters.HTTPAdapter(max_retries=retry)
-        session.mount('http://', adapter)
-        session.mount('https://', adapter)
-        
-        if use_proxy:
-            if ProxyList.is_empty():
-                ProxyList.gen_proxies()
-            temp_prox = ProxyList.get_random()
-            proxies = {
-                'http': f'http://{temp_prox[0]}:{temp_prox[1]}',
-                'https': f'https://{temp_prox[0]}:{temp_prox[1]}'
-            }
-            try:
-                return session.get(url, *args, **kwargs, proxies=proxies)
-            except Exception as err:
-                raise Exception(f'{err}\n\nThere seems to have been an error with the proxy IP. Please note that free proxies may not be reliable.')
+        if encoding != 'utf-8':
+            raise Exception("'encoding' argument is only relevent to grabbing local files.")
+        
+        if enable_js:
+            return __grab_enable_js(url)
+        else:
+            session = _requests.Session()
+            retry = _requests.packages.urllib3.util.retry.Retry(total=retries, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504])
+            adapter = _requests.adapters.HTTPAdapter(max_retries=retry)
+            session.mount('http://', adapter)
+            session.mount('https://', adapter)
+            
+            if use_proxy:
+                if ProxyList.is_empty():
+                    ProxyList.gen_proxies()
+                temp_prox = ProxyList.get_random()
+                proxies = {
+                    'http': f'http://{temp_prox[0]}:{temp_prox[1]}',
+                    'https': f'https://{temp_prox[0]}:{temp_prox[1]}'
+                }
+                try:
+                    return session.get(url, *args, **kwargs, proxies=proxies)
+                except Exception as err:
+                    raise Exception(f'{err}\n\nThere seems to have been an error with the proxy IP. Please note that free proxies may not be reliable.')
 
-        return session.get(url, *args, **kwargs)
+            return session.get(url, *args, **kwargs)
     raise Exception(f"Invalid url: {url}")
     
-def get_async(urls, use_proxy=False, retries=5, time_rest=0, *args, **kwargs) -> list:
+def get_async(urls, use_proxy=False, retries=5, encoding='utf-8', enable_js=False, time_rest=0, *args, **kwargs) -> list:
     """
     Gets multiple URLs asynchronously.
 
     This function sends HTTP requests to a list of URLs in separate threads, allowing for concurrent HTTP requests.
     The function returns a list of responses from the grabbed URLs.
 
     Args:
@@ -124,33 +152,44 @@
     Returns:
         list: A list of responses from the grabbed URLs.
     """
     # only import if async functionality is needed
     import threading as _threading
     import time
     if type(urls) == str:
-        return [get(urls, use_proxy=use_proxy, retries=retries, *args, **kwargs)]
+        return [get(urls, use_proxy=use_proxy, retries=retries, encoding=encoding, enable_js=enable_js, *args, **kwargs)]
 
     result = []
     threads = []
     for url in urls:
-        threads.append(_threading.Thread(target=__grab_thread_wrapper, args=[url, result, args, kwargs, use_proxy, retries]))
+        threads.append(_threading.Thread(target=__grab_thread_wrapper, args=[url, result, args, kwargs, use_proxy, retries, enable_js]))
         threads[-1].start()
         time.sleep(time_rest)
     
     for thread in threads:
         thread.join()
-    
-    return result    
+        
+    return result
 
 def head(url, **kwargs):
     return _requests.head(url, **kwargs)
 
-def post(url, data=None, json=None, **kwargs):
-    return _requests.post(url, data=data, json=json, **kwargs)
+def post(url:str, data=None, json=None, local_save_type:str=None, encoding:str='utf-8', **kwargs):
+    local_file_starts = ['./', 'C:', '/'] 
+    
+    if any([url.startswith(i) for i in local_file_starts]):
+        if local_save_type is None: local_save_type = 'w'
+        
+        with open(url, local_save_type, encoding=encoding) as f:
+            f.write(data)
+    else:
+        if (local_save_type is not None or encoding != 'utf-8'):
+            raise Exception("Arguments 'local_save_type' and 'encoding' are only relevent for posting to local files.")
+        
+        return _requests.post(url, data=data, json=json, **kwargs)
 
 def put(url, data=None, **kwargs):
     return _requests.put(url, data=data, **kwargs)
 
 def patch(url, data=None, **kwargs):
     return _requests.patch(url, data=data, **kwargs)
 
@@ -186,15 +225,15 @@
 
     Returns:
         None
     """
     ProxyList.update_proxies()
 
 def __local_grab(dir: str, encoding='utf-8'):
-    acceptableRegFiles = ['.txt', '.py', '.js', '.c', '.html', '.css', '.xml', '.md', '.yaml', '.yml']
+    acceptableRegFiles = ['.txt', '.py', '.js', '.c', '.html', '.css', '.xml', '.md', '.yaml', '.yml', '.ipynb']
     acceptableImgFiles = ['.png', '.jpg']
     
     if any([dir.endswith(i) for i in acceptableRegFiles]):
         with open(dir, 'r', encoding=encoding) as f:
             data = f.read()
         return data
     elif dir.endswith('.csv'):
@@ -205,11 +244,21 @@
     if any([dir.endswith(i) for i in acceptableImgFiles]):
         with open(dir, 'rb') as f:
             data = f.read()
         return data
 
     raise Exception(f"File type not supported: {dir}")
 
-def __grab_thread_wrapper(url:str, payload:list, args, kwargs, use_proxy=False, retries=5):
-    res = get(url, use_proxy=use_proxy, retries=retries, *args, **kwargs)
+def __grab_thread_wrapper(url:str, payload:list, args, kwargs, use_proxy=False, retries=5, enable_js=False):
+    res = get(url, use_proxy=use_proxy, retries=retries, enable_js=enable_js, *args, **kwargs)
     payload.append(res)
 
+def __grab_enable_js(url):
+    return _asyncio.get_event_loop().run_until_complete(__grab_enable_js_async(url)) 
+
+async def __grab_enable_js_async(url):
+    browser = await _launch()
+    page = await browser.newPage()
+    await page.goto(url, waitUntil='networkidle0')
+    html = await page.content()    
+    await browser.close()
+    return html
```

