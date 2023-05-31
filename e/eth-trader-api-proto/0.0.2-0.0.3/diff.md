# Comparing `tmp/eth_trader_api_proto-0.0.2.tar.gz` & `tmp/eth-trader-api-proto-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth_trader_api_proto-0.0.2.tar", last modified: Wed May 31 17:39:03 2023, max compression
+gzip compressed data, was "eth-trader-api-proto-0.0.3.tar", last modified: Wed May 31 18:01:31 2023, max compression
```

## Comparing `eth_trader_api_proto-0.0.2.tar` & `eth-trader-api-proto-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 17:39:03.218201 eth_trader_api_proto-0.0.2/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-05-31 17:39:03.218024 eth_trader_api_proto-0.0.2/PKG-INFO
--rw-r--r--   0 atulsrivastava   (501) staff       (20)     1025 2023-05-31 17:31:26.000000 eth_trader_api_proto-0.0.2/README.md
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      357 2023-05-31 17:37:43.000000 eth_trader_api_proto-0.0.2/pyproject.toml
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       38 2023-05-31 17:39:03.218258 eth_trader_api_proto-0.0.2/setup.cfg
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 17:39:03.215973 eth_trader_api_proto-0.0.2/src/
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 17:39:03.216873 eth_trader_api_proto-0.0.2/src/eth_trader_api/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 17:38:48.000000 eth_trader_api_proto-0.0.2/src/eth_trader_api/__init__.py
--rw-r--r--   0 atulsrivastava   (501) staff       (20)     4795 2023-05-31 17:38:48.000000 eth_trader_api_proto-0.0.2/src/eth_trader_api/proto.py
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 17:39:03.217805 eth_trader_api_proto-0.0.2/src/eth_trader_api_proto.egg-info/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-05-31 17:39:03.000000 eth_trader_api_proto-0.0.2/src/eth_trader_api_proto.egg-info/PKG-INFO
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      322 2023-05-31 17:39:03.000000 eth_trader_api_proto-0.0.2/src/eth_trader_api_proto.egg-info/SOURCES.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)        1 2023-05-31 17:39:03.000000 eth_trader_api_proto-0.0.2/src/eth_trader_api_proto.egg-info/dependency_links.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       22 2023-05-31 17:39:03.000000 eth_trader_api_proto-0.0.2/src/eth_trader_api_proto.egg-info/requires.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       15 2023-05-31 17:39:03.000000 eth_trader_api_proto-0.0.2/src/eth_trader_api_proto.egg-info/top_level.txt
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:01:31.465148 eth-trader-api-proto-0.0.3/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-05-31 18:01:31.464969 eth-trader-api-proto-0.0.3/PKG-INFO
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     1111 2023-05-31 18:00:17.000000 eth-trader-api-proto-0.0.3/README.md
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      357 2023-05-31 18:00:42.000000 eth-trader-api-proto-0.0.3/pyproject.toml
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       38 2023-05-31 18:01:31.465197 eth-trader-api-proto-0.0.3/setup.cfg
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:01:31.462974 eth-trader-api-proto-0.0.3/src/
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:01:31.463937 eth-trader-api-proto-0.0.3/src/eth_trader_api/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     4843 2023-05-31 17:59:29.000000 eth-trader-api-proto-0.0.3/src/eth_trader_api/__init__.py
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     4795 2023-05-31 17:59:21.000000 eth-trader-api-proto-0.0.3/src/eth_trader_api/proto.py
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:01:31.464772 eth-trader-api-proto-0.0.3/src/eth_trader_api_proto.egg-info/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-05-31 18:01:31.000000 eth-trader-api-proto-0.0.3/src/eth_trader_api_proto.egg-info/PKG-INFO
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      322 2023-05-31 18:01:31.000000 eth-trader-api-proto-0.0.3/src/eth_trader_api_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)        1 2023-05-31 18:01:31.000000 eth-trader-api-proto-0.0.3/src/eth_trader_api_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       22 2023-05-31 18:01:31.000000 eth-trader-api-proto-0.0.3/src/eth_trader_api_proto.egg-info/requires.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       15 2023-05-31 18:01:31.000000 eth-trader-api-proto-0.0.3/src/eth_trader_api_proto.egg-info/top_level.txt
```

### Comparing `eth_trader_api_proto-0.0.2/README.md` & `eth-trader-api-proto-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,20 @@
     cd python
     rm -rf dist/ && python3 -m build 
 ```
 
 you can install package locally before uploading it to the pypi
 
 ```shell
-    pip install dist/eth-trader-api-0.0.2.tar.gz
+    pip install dist/eth_trader_api_proto_0.0.3.tar.gz
 ```
 
     (Don't forget to fix the proto compilation issues before releasing)
+    To upload this library officially to pypi, use this command
+
+```shell
     python3 -m twine upload --repository pypi dist/*
+```   
 
 ## Issues
-
     if you encounter any issues related to the above python3 commands refer to this page for steps to setup your local machine 
     [https://packaging.python.org/en/latest/tutorials/packaging-projects/](https://packaging.python.org/en/latest/tutorials/packaging-projects/)
```

### Comparing `eth_trader_api_proto-0.0.2/src/eth_trader_api/proto.py` & `eth-trader-api-proto-0.0.3/src/eth_trader_api/proto.py`

 * *Files identical despite different names*

