# Comparing `tmp/thztools-1.0.4.tar.gz` & `tmp/thztools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thztools-1.0.4.tar", last modified: Sat May 27 05:04:30 2023, max compression
+gzip compressed data, was "thztools-1.0.5.tar", last modified: Sat May 27 07:13:51 2023, max compression
```

## Comparing `thztools-1.0.4.tar` & `thztools-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 05:04:30.916012 thztools-1.0.4/
--rw-rw-rw-   0        0        0       26 2023-05-26 04:13:13.000000 thztools-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3001 2023-05-27 05:04:30.913011 thztools-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2579 2023-05-27 05:04:03.000000 thztools-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 05:04:30.920012 thztools-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-05-27 04:59:48.000000 thztools-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:04:30.861009 thztools-1.0.4/thztools/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-1.0.4/thztools/__init__.py
--rw-rw-rw-   0        0        0     2212 2023-05-27 05:03:59.000000 thztools-1.0.4/thztools/ip.py
--rw-rw-rw-   0        0        0     6106 2023-05-27 04:21:41.000000 thztools-1.0.4/thztools/jiami.py
-drwxrwxrwx   0        0        0        0 2023-05-27 05:04:30.903011 thztools-1.0.4/thztools.egg-info/
--rw-rw-rw-   0        0        0     3001 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 05:04:30.000000 thztools-1.0.4/thztools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 07:13:51.822910 thztools-1.0.5/
+-rw-rw-rw-   0        0        0       26 2023-05-26 04:13:13.000000 thztools-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3053 2023-05-27 07:13:51.816910 thztools-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2023-05-27 07:13:00.000000 thztools-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 07:13:51.827911 thztools-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:13:04.000000 thztools-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 07:13:51.743906 thztools-1.0.5/thztools/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 thztools-1.0.5/thztools/__init__.py
+-rw-rw-rw-   0        0        0     2212 2023-05-27 05:03:59.000000 thztools-1.0.5/thztools/ip.py
+-rw-rw-rw-   0        0        0     6138 2023-05-27 07:12:28.000000 thztools-1.0.5/thztools/jiami.py
+drwxrwxrwx   0        0        0        0 2023-05-27 07:13:51.805909 thztools-1.0.5/thztools.egg-info/
+-rw-rw-rw-   0        0        0     3053 2023-05-27 07:13:51.000000 thztools-1.0.5/thztools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-27 07:13:51.000000 thztools-1.0.5/thztools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 07:13:51.000000 thztools-1.0.5/thztools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-27 07:13:51.000000 thztools-1.0.5/thztools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-27 07:13:51.000000 thztools-1.0.5/thztools.egg-info/top_level.txt
```

### Comparing `thztools-1.0.4/PKG-INFO` & `thztools-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thztools
-Version: 1.0.4
+Version: 1.0.5
 Summary: 由天狐宗开发的工具，方便开发时使用
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,17 @@
 >Tianhuzong开发的工具，方便在开发中使用
 1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
 - - -
 >1.0.3版本中，修复了维吉尼亚密码的错误，引入了与ip地址有关的类<kbd>IP</kbd>
 - - -
 >1.0.4版本中，新增了检测ip是否为合法的IPv4
 - - -
+- - -
+>1.0.5中，修复一个命名冲突
+- - -
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install thztools
 ```
 安装完模块之后接下来就是引用了
```

### Comparing `thztools-1.0.4/README.md` & `thztools-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 >Tianhuzong开发的工具，方便在开发中使用
 1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
 - - -
 >1.0.3版本中，修复了维吉尼亚密码的错误，引入了与ip地址有关的类<kbd>IP</kbd>
 - - -
 >1.0.4版本中，新增了检测ip是否为合法的IPv4
 - - -
+- - -
+>1.0.5中，修复一个命名冲突
+- - -
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install thztools
 ```
 安装完模块之后接下来就是引用了
```

### Comparing `thztools-1.0.4/setup.py` & `thztools-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 with open("./README.md",mode='r',encoding='utf-8') as f:
     des = f.read()
 setup(
     name="thztools",      # 包名，用于安装和调用该包
-    version="1.0.4",               # 版本号
+    version="1.0.5",               # 版本号
     author="Sen",
     description="由天狐宗开发的工具，方便开发时使用",
     long_description=des,
     long_description_content_type='text/markdown',
     author_email="tianhuzong@qq.com",
     url="https://github.com/tianhuzong/thztools",
     license="MIT",
```

### Comparing `thztools-1.0.4/thztools/ip.py` & `thztools-1.0.5/thztools/ip.py`

 * *Files identical despite different names*

### Comparing `thztools-1.0.4/thztools/jiami.py` & `thztools-1.0.5/thztools/jiami.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Crypto.Cipher import AES
+from Crypto.Cipher import AES as AESclass
 from Crypto.Random import get_random_bytes
 import rsa
 class KaiSa:
     def jiami(self,plaintext, shift):
         """
         凯撒加密算法
         plaintext: 明文
@@ -104,30 +104,30 @@
         AES加密算法
         plaintext: 明文
         key: 秘钥
         Returns:
             密文,随机数，验证标签，均为bytes类型
         """
         # 用秘钥创建一个AES对象
-        cipher = AES.new(key, AES.MODE_EAX)
+        cipher = AESclass.new(key, AESclass.MODE_EAX)
         # 加密明文
         ciphertext, tag = cipher.encrypt_and_digest(plaintext.encode('utf-8'))
         # 返回加密后的密文和必要的参数
         return ciphertext, cipher.nonce, tag
 
     def jiemi(self,ciphertext, key, nonce, tag):
         """
         AES解密算法
         ciphertext: 密文
         key: 秘钥
         nonce: 加密时生成的随机数
         tag: 加密时生成的验证标签
         """
         # 用密钥和随机数创建一个AES对象
-        cipher = AES.new(key, AES.MODE_EAX, nonce=nonce)
+        cipher = AESclass.new(key, AESclass.MODE_EAX, nonce=nonce)
         try:
             # 解密密文
             plaintext = cipher.decrypt_and_verify(ciphertext, tag)
             return plaintext.decode('utf-8')
         except:
             return None
 class Weijiniya:
```

### Comparing `thztools-1.0.4/thztools.egg-info/PKG-INFO` & `thztools-1.0.5/thztools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thztools
-Version: 1.0.4
+Version: 1.0.5
 Summary: 由天狐宗开发的工具，方便开发时使用
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,17 @@
 >Tianhuzong开发的工具，方便在开发中使用
 1.0.2加入了加密解密内容：<kbd>RSA</kbd>,<kbd>AES</kbd>，<kbd>凯撒加密</kbd>
 - - -
 >1.0.3版本中，修复了维吉尼亚密码的错误，引入了与ip地址有关的类<kbd>IP</kbd>
 - - -
 >1.0.4版本中，新增了检测ip是否为合法的IPv4
 - - -
+- - -
+>1.0.5中，修复一个命名冲突
+- - -
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install thztools
 ```
 安装完模块之后接下来就是引用了
```

