# Comparing `tmp/uium-0.3.4.tar.gz` & `tmp/uium-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uium-0.3.4.tar", max compression
+gzip compressed data, was "uium-0.3.5.tar", max compression
```

## Comparing `uium-0.3.4.tar` & `uium-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 uium-0.3.4/LICENSE
--rw-r--r--   0        0        0     1478 2023-05-30 16:27:13.926024 uium-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      596 2023-05-30 02:29:40.011464 uium-0.3.4/README.md
--rw-r--r--   0        0        0     1044 2023-05-30 16:21:40.483152 uium-0.3.4/uium/__init__.py
--rw-r--r--   0        0        0     1579 2023-05-30 16:23:02.395487 uium-0.3.4/uium/_auto_electron.py
--rw-r--r--   0        0        0     2991 2023-05-30 16:00:34.308002 uium-0.3.4/uium/_install_driver.py
--rw-r--r--   0        0        0       14 2023-05-30 15:45:01.782811 uium-0.3.4/uium/_mirror.py
--rw-r--r--   0        0        0      137 2023-05-30 16:24:23.007397 uium-0.3.4/uium/_uium.py
--rw-r--r--   0        0        0       14 2023-05-30 15:44:58.897076 uium-0.3.4/uium/_webdriver_manager.py
--rw-r--r--   0        0        0      846 2023-05-30 16:25:33.967458 uium-0.3.4/uium/selenium.py
--rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 uium-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 uium-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1478 2023-05-31 14:31:31.522383 uium-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      596 2023-05-30 02:29:40.011464 uium-0.3.5/README.md
+-rw-r--r--   0        0        0     1044 2023-05-31 14:31:44.340728 uium-0.3.5/uium/__init__.py
+-rw-r--r--   0        0        0     1579 2023-05-30 16:23:02.395487 uium-0.3.5/uium/_auto_electron.py
+-rw-r--r--   0        0        0     3242 2023-05-31 14:22:37.155376 uium-0.3.5/uium/_install_driver.py
+-rw-r--r--   0        0        0       14 2023-05-30 15:45:01.782811 uium-0.3.5/uium/_mirror.py
+-rw-r--r--   0        0        0      137 2023-05-30 16:24:23.007397 uium-0.3.5/uium/_uium.py
+-rw-r--r--   0        0        0       14 2023-05-30 15:44:58.897076 uium-0.3.5/uium/_webdriver_manager.py
+-rw-r--r--   0        0        0      914 2023-05-31 14:23:25.829837 uium-0.3.5/uium/selenium.py
+-rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 uium-0.3.5/PKG-INFO
```

### Comparing `uium-0.3.4/LICENSE` & `uium-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uium-0.3.4/pyproject.toml` & `uium-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uium"
-version = "0.3.4"
+version = "0.3.5"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/uium"
 repository = "https://github.com/MarkHoo/uium"
 classifiers = [
```

### Comparing `uium-0.3.4/README.md` & `uium-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `uium-0.3.4/uium/__init__.py` & `uium-0.3.5/uium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from selenium.webdriver.chrome.service import Service as ChromiumService
 # webdriver manager modules
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 
 __all__ = ["_uium", "Chrome", "ChromeOptions", "webdriver", "Options", "ChromiumService", "ChromeDriverManager", "ChromeType"]
-__version__ = "v0.3.4"
+__version__ = "v0.3.5"
 
 
 """
 TODO:
 - 集成Chrome驱动管理
 - 集成隐藏Chrome指纹防反爬
 - 根据ip来自动选择最近的ChromeDriver镜像点
```

### Comparing `uium-0.3.4/uium/_auto_electron.py` & `uium-0.3.5/uium/_auto_electron.py`

 * *Files identical despite different names*

### Comparing `uium-0.3.4/uium/_install_driver.py` & `uium-0.3.5/uium/_install_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,81 +4,82 @@
 
 import requests
 import zipfile
 from io import BytesIO
 import os
 
 
-# 获取 Chrome 浏览器版本号
-from selenium.webdriver.chrome.service import Service
+if __name__ == '__main__':
+    # 获取 Chrome 浏览器版本号
+    from selenium.webdriver.chrome.service import Service
+
+    command_output = subprocess.run(
+        ['wmic', 'datafile', 'where', 'name="C:\\\\Program Files (x86)\\\\Google\\\\Chrome\\\\Application\\\\chrome.exe"',
+        'get', 'Version', '/value'], capture_output=True)
+    version_string = command_output.stdout.decode().strip()
+
+    chrome_version = re.search(r'(\d+\.\d+\.\d+\.\d+)', version_string).group(1)
+
+    print(f'The current version of Chrome is {chrome_version}')
+
+    # 下载最新版本的 ChromeDriver
+    response = requests.get('https://chromedriver.storage.googleapis.com/LATEST_RELEASE')
+    latest_version = response.text.strip()
+
+    download_url = f'https://chromedriver.storage.googleapis.com/{latest_version}/chromedriver_win32.zip'
+    response = requests.get(download_url)
+
+    if response.status_code == 200:
+        try:
+            with zipfile.ZipFile(BytesIO(response.content)) as zip_file:
+                zip_file.extractall(os.getcwd())
+            print('ChromeDriver has been updated!')
+        except zipfile.BadZipFile:
+            print('The downloaded file is not a valid ZIP file!')
+
+        # 指定 ChromeDriver 可执行文件的路径
+        system_bit = platform.architecture()[0]
+        print(system_bit)
+        # executable_path = os.path.join(os.getcwd(), f'chromedriver_{system_bit}.exe')
+        executable_path = os.path.join(os.getcwd(), f'chromedriver.exe')
+        print(executable_path)
+
+        # ChromeDriver所在文件夹的完整路径
+        # chromedriver_path = r"C:\chromedriver_win32"
+        chromedriver_path = executable_path
+        # 获取当前系统的PATH环境变量
+        path_env = os.environ['PATH']
+        # print(path_env)
+        # 将ChromeDriver路径添加到PATH环境变量中，并用分号分隔
+        os.environ['PATH'] = path_env + ";" + chromedriver_path
+
+        path_env = os.environ['PATH']
+        print(path_env)
+        # print(type(path_env))
+        # s = path_env.split(";")
+        # print(type(s))
+        # for i in s:
+        #     print(i)
+
+        # 检查 ChromeDriver 是否与本地 Chrome 浏览器版本兼容
+        from selenium import webdriver
+
+        options = webdriver.ChromeOptions()
+        options.add_argument('headless')
+        service = Service(executable_path=executable_path)
+        driver = webdriver.Chrome(service=service, options=options)
+
+        local_version = driver.capabilities['browserVersion']
+        if chrome_version.split('.')[0] == local_version.split('.')[0]:
+            print(f'The downloaded ChromeDriver version {latest_version} is compatible with your Chrome browser version.')
+        else:
+            print(
+                f'The downloaded ChromeDriver version {latest_version} may not be compatible with your Chrome browser version. Local version: {local_version}')
 
-command_output = subprocess.run(
-    ['wmic', 'datafile', 'where', 'name="C:\\\\Program Files (x86)\\\\Google\\\\Chrome\\\\Application\\\\chrome.exe"',
-     'get', 'Version', '/value'], capture_output=True)
-version_string = command_output.stdout.decode().strip()
-
-chrome_version = re.search(r'(\d+\.\d+\.\d+\.\d+)', version_string).group(1)
-
-print(f'The current version of Chrome is {chrome_version}')
-
-# 下载最新版本的 ChromeDriver
-response = requests.get('https://chromedriver.storage.googleapis.com/LATEST_RELEASE')
-latest_version = response.text.strip()
-
-download_url = f'https://chromedriver.storage.googleapis.com/{latest_version}/chromedriver_win32.zip'
-response = requests.get(download_url)
-
-if response.status_code == 200:
-    try:
-        with zipfile.ZipFile(BytesIO(response.content)) as zip_file:
-            zip_file.extractall(os.getcwd())
-        print('ChromeDriver has been updated!')
-    except zipfile.BadZipFile:
-        print('The downloaded file is not a valid ZIP file!')
-
-    # 指定 ChromeDriver 可执行文件的路径
-    system_bit = platform.architecture()[0]
-    print(system_bit)
-    # executable_path = os.path.join(os.getcwd(), f'chromedriver_{system_bit}.exe')
-    executable_path = os.path.join(os.getcwd(), f'chromedriver.exe')
-    print(executable_path)
-
-    # ChromeDriver所在文件夹的完整路径
-    # chromedriver_path = r"C:\chromedriver_win32"
-    chromedriver_path = executable_path
-    # 获取当前系统的PATH环境变量
-    path_env = os.environ['PATH']
-    # print(path_env)
-    # 将ChromeDriver路径添加到PATH环境变量中，并用分号分隔
-    os.environ['PATH'] = path_env + ";" + chromedriver_path
-
-    path_env = os.environ['PATH']
-    print(path_env)
-    # print(type(path_env))
-    # s = path_env.split(";")
-    # print(type(s))
-    # for i in s:
-    #     print(i)
-
-    # 检查 ChromeDriver 是否与本地 Chrome 浏览器版本兼容
-    from selenium import webdriver
-
-    options = webdriver.ChromeOptions()
-    options.add_argument('headless')
-    service = Service(executable_path=executable_path)
-    driver = webdriver.Chrome(service=service, options=options)
-
-    local_version = driver.capabilities['browserVersion']
-    if chrome_version.split('.')[0] == local_version.split('.')[0]:
-        print(f'The downloaded ChromeDriver version {latest_version} is compatible with your Chrome browser version.')
-    else:
-        print(
-            f'The downloaded ChromeDriver version {latest_version} may not be compatible with your Chrome browser version. Local version: {local_version}')
-
-    driver.quit()
+        driver.quit()
 
-else:
-    print(f'Failed to download ChromeDriver. Status code: {response.status_code}')
+    else:
+        print(f'Failed to download ChromeDriver. Status code: {response.status_code}')
 
 
 
 __all__ = []
```

### Comparing `uium-0.3.4/uium/selenium.py` & `uium-0.3.5/uium/selenium.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 # webdriver manager modules
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 # utility modules
 from random import randrange
 
 
-def simple_chrome(page=""):
-    options = Options()
-    debugging_port = str(randrange(9222, 9999))
-    options.add_argument('--remote-debugging-port=%s'%debugging_port)
-    service = ChromiumService(ChromeDriverManager().install())
-    browser = webdriver.Chrome(service=service, options=options)
-    browser.get(page)
-    return browser
+if __name__ == '__main__':
+    def simple_chrome(page=""):
+        options = Options()
+        debugging_port = str(randrange(9222, 9999))
+        options.add_argument('--remote-debugging-port=%s'%debugging_port)
+        service = ChromiumService(ChromeDriverManager().install())
+        browser = webdriver.Chrome(service=service, options=options)
+        browser.get(page)
+        return browser
 
 
-browser = simple_chrome("https://sogou.com")
-browser2 = simple_chrome("https://bing.com")
+    browser = simple_chrome("https://sogou.com")
+    browser2 = simple_chrome("https://bing.com")
 
 
 __all__ = ["ChromeType"]
```

### Comparing `uium-0.3.4/PKG-INFO` & `uium-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uium
-Version: 0.3.4
+Version: 0.3.5
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/uium
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

