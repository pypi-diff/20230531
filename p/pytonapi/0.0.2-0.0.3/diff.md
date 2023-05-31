# Comparing `tmp/pytonapi-0.0.2.tar.gz` & `tmp/pytonapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonapi-0.0.2.tar", last modified: Fri May 26 18:06:01 2023, max compression
+gzip compressed data, was "pytonapi-0.0.3.tar", last modified: Wed May 31 20:44:56 2023, max compression
```

## Comparing `pytonapi-0.0.2.tar` & `pytonapi-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-26 18:06:01.139994 pytonapi-0.0.2/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2023-05-26 17:22:12.000000 pytonapi-0.0.2/LICENSE
--rw-rw-r--   0 ness      (1000) ness      (1000)     6262 2023-05-26 18:06:01.139994 pytonapi-0.0.2/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     5860 2023-05-26 17:22:12.000000 pytonapi-0.0.2/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-26 18:06:01.135995 pytonapi-0.0.2/pytonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)       65 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/__init__.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-26 18:06:01.135995 pytonapi-0.0.2/pytonapi/async_tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1376 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1646 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-26 18:06:01.139994 pytonapi-0.0.2/pytonapi/async_tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3410 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2236 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      890 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      501 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2660 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      587 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/async_tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1030 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/exceptions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-26 18:06:01.139994 pytonapi-0.0.2/pytonapi/schema/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1713 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/schema/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      460 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/schema/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1660 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/schema/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      349 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/schema/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      318 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/schema/domains.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      969 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/schema/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      983 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/schema/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2968 2023-05-26 18:04:03.000000 pytonapi-0.0.2/pytonapi/schema/traces.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-26 18:06:01.139994 pytonapi-0.0.2/pytonapi/tonapi/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1357 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1618 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/client.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-26 18:06:01.139994 pytonapi-0.0.2/pytonapi/tonapi/methods/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/methods/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     3316 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/methods/accounts.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2166 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/methods/blockchain.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      850 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/methods/dns.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      473 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/methods/jettons.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2578 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/methods/nft.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      559 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/tonapi/methods/traces.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2220 2023-05-26 17:22:12.000000 pytonapi-0.0.2/pytonapi/utils.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-26 18:06:01.135995 pytonapi-0.0.2/pytonapi.egg-info/
--rw-rw-r--   0 ness      (1000) ness      (1000)     6262 2023-05-26 18:06:01.000000 pytonapi-0.0.2/pytonapi.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     1103 2023-05-26 18:06:01.000000 pytonapi-0.0.2/pytonapi.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2023-05-26 18:06:01.000000 pytonapi-0.0.2/pytonapi.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       64 2023-05-26 18:06:01.000000 pytonapi-0.0.2/pytonapi.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        9 2023-05-26 18:06:01.000000 pytonapi-0.0.2/pytonapi.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-05-26 18:06:01.139994 pytonapi-0.0.2/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)      768 2023-05-26 18:05:47.000000 pytonapi-0.0.2/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.896121 pytonapi-0.0.3/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1060 2023-05-26 17:22:12.000000 pytonapi-0.0.3/LICENSE
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6262 2023-05-31 20:44:56.896121 pytonapi-0.0.3/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     5860 2023-05-31 20:44:28.000000 pytonapi-0.0.3/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)       65 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/__init__.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/async_tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1376 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1646 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/async_tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3410 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2236 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      890 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      501 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2660 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      587 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/async_tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1030 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/exceptions.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/schema/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1713 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      460 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1660 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      349 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      318 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/domains.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      969 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      983 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/schema/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2968 2023-05-26 18:04:03.000000 pytonapi-0.0.3/pytonapi/schema/traces.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi/tonapi/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1357 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1618 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/client.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.896121 pytonapi-0.0.3/pytonapi/tonapi/methods/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     3316 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/accounts.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2166 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/blockchain.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      850 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/dns.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      473 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/jettons.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2578 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/nft.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      559 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/tonapi/methods/traces.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2220 2023-05-26 17:22:12.000000 pytonapi-0.0.3/pytonapi/utils.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2023-05-31 20:44:56.892120 pytonapi-0.0.3/pytonapi.egg-info/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6262 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1103 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       64 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        9 2023-05-31 20:44:56.000000 pytonapi-0.0.3/pytonapi.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2023-05-31 20:44:56.896121 pytonapi-0.0.3/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)      768 2023-05-31 20:44:51.000000 pytonapi-0.0.3/setup.py
```

### Comparing `pytonapi-0.0.2/LICENSE` & `pytonapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/PKG-INFO` & `pytonapi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/nessshon/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -125,15 +125,15 @@
 
         # print transaction value (amount)
         print(nano_to_amount(transaction.in_msg.value))
         # output: 1.0
 
         # print transaction text comment
         if transaction.in_msg.decoded_op_name == "text_comment":
-            print(transaction.in_msg.decoded_body["text"])
+            print(transaction.in_msg.decoded_body["Text"])
             # output: Hello, World!
 
 
 if __name__ == '__main__':
     main()
 ```
```

### Comparing `pytonapi-0.0.2/README.md` & `pytonapi-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         # print transaction value (amount)
         print(nano_to_amount(transaction.in_msg.value))
         # output: 1.0
 
         # print transaction text comment
         if transaction.in_msg.decoded_op_name == "text_comment":
-            print(transaction.in_msg.decoded_body["text"])
+            print(transaction.in_msg.decoded_body["Text"])
             # output: Hello, World!
 
 
 if __name__ == '__main__':
     main()
 ```
```

### Comparing `pytonapi-0.0.2/pytonapi/async_tonapi/__init__.py` & `pytonapi-0.0.3/pytonapi/async_tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/async_tonapi/client.py` & `pytonapi-0.0.3/pytonapi/async_tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/async_tonapi/methods/accounts.py` & `pytonapi-0.0.3/pytonapi/async_tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/async_tonapi/methods/blockchain.py` & `pytonapi-0.0.3/pytonapi/async_tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/async_tonapi/methods/dns.py` & `pytonapi-0.0.3/pytonapi/async_tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/async_tonapi/methods/nft.py` & `pytonapi-0.0.3/pytonapi/async_tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/async_tonapi/methods/traces.py` & `pytonapi-0.0.3/pytonapi/async_tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/exceptions.py` & `pytonapi-0.0.3/pytonapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/schema/__init__.py` & `pytonapi-0.0.3/pytonapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/schema/blockchain.py` & `pytonapi-0.0.3/pytonapi/schema/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/schema/jettons.py` & `pytonapi-0.0.3/pytonapi/schema/jettons.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/schema/nft.py` & `pytonapi-0.0.3/pytonapi/schema/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/schema/traces.py` & `pytonapi-0.0.3/pytonapi/schema/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/tonapi/__init__.py` & `pytonapi-0.0.3/pytonapi/tonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/tonapi/client.py` & `pytonapi-0.0.3/pytonapi/tonapi/client.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/tonapi/methods/accounts.py` & `pytonapi-0.0.3/pytonapi/tonapi/methods/accounts.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/tonapi/methods/blockchain.py` & `pytonapi-0.0.3/pytonapi/tonapi/methods/blockchain.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/tonapi/methods/dns.py` & `pytonapi-0.0.3/pytonapi/tonapi/methods/dns.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/tonapi/methods/nft.py` & `pytonapi-0.0.3/pytonapi/tonapi/methods/nft.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/tonapi/methods/traces.py` & `pytonapi-0.0.3/pytonapi/tonapi/methods/traces.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi/utils.py` & `pytonapi-0.0.3/pytonapi/utils.py`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/pytonapi.egg-info/PKG-INFO` & `pytonapi-0.0.3/pytonapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provide access to indexed TON blockchain.
 Home-page: https://github.com/nessshon/pytonapi/
 Author: nessshon
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -125,15 +125,15 @@
 
         # print transaction value (amount)
         print(nano_to_amount(transaction.in_msg.value))
         # output: 1.0
 
         # print transaction text comment
         if transaction.in_msg.decoded_op_name == "text_comment":
-            print(transaction.in_msg.decoded_body["text"])
+            print(transaction.in_msg.decoded_body["Text"])
             # output: Hello, World!
 
 
 if __name__ == '__main__':
     main()
 ```
```

### Comparing `pytonapi-0.0.2/pytonapi.egg-info/SOURCES.txt` & `pytonapi-0.0.3/pytonapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytonapi-0.0.2/setup.py` & `pytonapi-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytonapi",
-    version="0.0.2",
+    version="0.0.3",
     author="nessshon",
     description="Provide access to indexed TON blockchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nessshon/pytonapi/",
     packages=setuptools.find_packages(exclude="pytonapi"),
     python_requires='>=3.10',
```

