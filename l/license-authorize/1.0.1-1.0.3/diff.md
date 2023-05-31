# Comparing `tmp/license_authorize-1.0.1.tar.gz` & `tmp/license_authorize-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\license_authorize-1.0.1.tar", last modified: Fri May 19 11:19:01 2023, max compression
+gzip compressed data, was "dist\license_authorize-1.0.3.tar", last modified: Wed May 31 07:25:03 2023, max compression
```

## Comparing `license_authorize-1.0.1.tar` & `license_authorize-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 11:19:01.665431 license_authorize-1.0.1/
--rw-rw-rw-   0        0        0     1394 2023-05-19 11:19:01.663432 license_authorize-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-05-19 09:47:18.000000 license_authorize-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 11:19:01.656432 license_authorize-1.0.1/license_authorize/
--rw-rw-rw-   0        0        0      226 2023-05-19 06:53:07.000000 license_authorize-1.0.1/license_authorize/__init__.py
--rw-rw-rw-   0        0        0     3103 2023-05-19 10:27:37.000000 license_authorize-1.0.1/license_authorize/_core.py
--rw-rw-rw-   0        0        0      877 2023-05-19 10:12:48.000000 license_authorize-1.0.1/license_authorize/decode.py
-drwxrwxrwx   0        0        0        0 2023-05-19 11:19:01.662432 license_authorize-1.0.1/license_authorize.egg-info/
--rw-rw-rw-   0        0        0     1394 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-19 11:19:01.000000 license_authorize-1.0.1/license_authorize.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 11:19:01.665431 license_authorize-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2175 2023-05-19 11:18:58.000000 license_authorize-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:25:03.342274 license_authorize-1.0.3/
+-rw-rw-rw-   0        0        0     1405 2023-05-31 07:25:03.341274 license_authorize-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-05-19 09:47:18.000000 license_authorize-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 07:25:03.332274 license_authorize-1.0.3/license_authorize/
+-rw-rw-rw-   0        0        0      226 2023-05-19 06:53:07.000000 license_authorize-1.0.3/license_authorize/__init__.py
+-rw-rw-rw-   0        0        0     3381 2023-05-31 07:14:43.000000 license_authorize-1.0.3/license_authorize/_core.py
+-rw-rw-rw-   0        0        0      877 2023-05-19 10:12:48.000000 license_authorize-1.0.3/license_authorize/decode.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:25:03.339274 license_authorize-1.0.3/license_authorize.egg-info/
+-rw-rw-rw-   0        0        0     1405 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-31 07:25:03.000000 license_authorize-1.0.3/license_authorize.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:25:03.342274 license_authorize-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2236 2023-05-31 07:22:35.000000 license_authorize-1.0.3/setup.py
```

### Comparing `license_authorize-1.0.1/PKG-INFO` & `license_authorize-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: license_authorize
-Version: 1.0.1
-Summary: A tools for license authorize
+Version: 1.0.3
+Summary: A tools for license authorize in windows
 Home-page: https://github.com/gisfanmachel/licenseAuthorize
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this program is for lincense authorize
         
         ### it use cpuid and servertime and clienttime to verify the request with the premaked lic file
```

### Comparing `license_authorize-1.0.1/license_authorize/_core.py` & `license_authorize-1.0.3/license_authorize/_core.py`

 * *Files 27% similar despite different names*

```diff
@@ -40,27 +40,35 @@
                 break
             line = f.readline()
         f.close()
         private_key = "-----BEGIN RSA PRIVATE KEY-----\n" + private_key + "\n-----END RSA PRIVATE KEY-----"
         return text_encrypted_base64, private_key
 
     def verify_cpuId(self, license_cpu_id):
+        # sys.platform.startswith（"win"）
         sysstr = platform.system()
         server_cpu_id = None
         if sysstr == "Windows":
             cmd = "wmic cpu get ProcessorId"
-            with os.popen(cmd, "r") as p:
-                r = p.read()
-            print(r.replace("\n", ""))
-            server_cpu_id = r.replace("\n", "").replace(" ", "").lstrip("ProcessorId").strip()
-            print(server_cpu_id)
+            output = os.popen(cmd, "r")
+            info = output.readlines()
+            # 读取第3行
+            rowindex = 0
+            for line in info:
+                print(line.replace("\n", "").replace(" ", ""))
+                if rowindex == 2:
+                    server_cpu_id = line.replace("\n", "").replace(" ", "")
+                    print(server_cpu_id)
+                    break
+                rowindex += 1
         elif sysstr == "Linux":
             cmd = "dmidecode -t processor | grep 'ID'"
             output = os.popen(cmd, "r")
             info = output.readlines()
+            # 读取第一行
             for line in info:
                 print(line.replace("\n", "").replace(" ", ""))
                 server_cpu_id = line.replace("\n", "").replace(" ", "").split(":")[1]
                 print(server_cpu_id)
                 break
         if server_cpu_id is not None and server_cpu_id.upper() == license_cpu_id:
             return True
@@ -69,15 +77,15 @@
 
     def check_validity(self, client_time, lic_path):
         text_encrypted_base64, private_key = self.__read_lic_file(lic_path)
         text_decrypted = decryption(text_encrypted_base64, private_key.encode('utf-8'))
         license_cpuid = text_decrypted.split(",")[0]
         license_time = text_decrypted.split(",")[1]
         license_time_obj = datetime.datetime.strptime(license_time, "%Y-%m-%d %H:%M:%S")
-        license_time = int(time.mktime(license_time_obj.timetuple())*1000)
+        license_time = int(time.mktime(license_time_obj.timetuple()) * 1000)
         server_time = int(time.time() * 1000)
         if license_time >= client_time and license_time >= server_time and self.verify_cpuId(license_cpuid):
             return True
         else:
             return False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `license_authorize-1.0.1/license_authorize/decode.py` & `license_authorize-1.0.3/license_authorize/decode.py`

 * *Files identical despite different names*

### Comparing `license_authorize-1.0.1/license_authorize.egg-info/PKG-INFO` & `license_authorize-1.0.3/license_authorize.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: license-authorize
-Version: 1.0.1
-Summary: A tools for license authorize
+Version: 1.0.3
+Summary: A tools for license authorize in windows
 Home-page: https://github.com/gisfanmachel/licenseAuthorize
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this program is for lincense authorize
         
         ### it use cpuid and servertime and clienttime to verify the request with the premaked lic file
```

### Comparing `license_authorize-1.0.1/setup.py` & `license_authorize-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
+    # name="license_authorize",  # Required 项目名称
     name="license_authorize",  # Required 项目名称
-    version="1.0.1",  # Required 发布版本号
-    description="A tools for license authorize",  # Optional 项目简单描述
+    version="1.0.3",  # Required 发布版本号
+    description="A tools for license authorize in windows",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/licenseAuthorize",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
 
@@ -44,18 +45,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
 
     keywords="license,authorize, setuptools, development",  # Optional 搜索关键字
 
-
     packages=find_packages(),  # Required
 
     python_requires=">=3.7, <4",  # python 版本要求
 
     install_requires=["pycryptodome"],  # Optional 第三方依赖库
 
-
-
-
 )
```

