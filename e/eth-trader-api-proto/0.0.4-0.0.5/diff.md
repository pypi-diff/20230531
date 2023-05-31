# Comparing `tmp/eth-trader-api-proto-0.0.4.tar.gz` & `tmp/eth-trader-api-proto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-trader-api-proto-0.0.4.tar", last modified: Wed May 31 18:23:12 2023, max compression
+gzip compressed data, was "eth-trader-api-proto-0.0.5.tar", last modified: Wed May 31 18:30:09 2023, max compression
```

## Comparing `eth-trader-api-proto-0.0.4.tar` & `eth-trader-api-proto-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:23:12.289334 eth-trader-api-proto-0.0.4/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-05-31 18:23:12.289131 eth-trader-api-proto-0.0.4/PKG-INFO
--rw-r--r--   0 atulsrivastava   (501) staff       (20)     1111 2023-05-31 18:00:17.000000 eth-trader-api-proto-0.0.4/README.md
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      357 2023-05-31 18:22:31.000000 eth-trader-api-proto-0.0.4/pyproject.toml
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       38 2023-05-31 18:23:12.289387 eth-trader-api-proto-0.0.4/setup.cfg
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:23:12.286955 eth-trader-api-proto-0.0.4/src/
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:23:12.288016 eth-trader-api-proto-0.0.4/src/eth_trader_api/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       19 2023-05-31 18:21:57.000000 eth-trader-api-proto-0.0.4/src/eth_trader_api/__init__.py
--rw-r--r--   0 atulsrivastava   (501) staff       (20)     4795 2023-05-31 18:21:36.000000 eth-trader-api-proto-0.0.4/src/eth_trader_api/proto.py
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:23:12.288956 eth-trader-api-proto-0.0.4/src/eth_trader_api_proto.egg-info/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-05-31 18:23:12.000000 eth-trader-api-proto-0.0.4/src/eth_trader_api_proto.egg-info/PKG-INFO
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      322 2023-05-31 18:23:12.000000 eth-trader-api-proto-0.0.4/src/eth_trader_api_proto.egg-info/SOURCES.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)        1 2023-05-31 18:23:12.000000 eth-trader-api-proto-0.0.4/src/eth_trader_api_proto.egg-info/dependency_links.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       22 2023-05-31 18:23:12.000000 eth-trader-api-proto-0.0.4/src/eth_trader_api_proto.egg-info/requires.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       15 2023-05-31 18:23:12.000000 eth-trader-api-proto-0.0.4/src/eth_trader_api_proto.egg-info/top_level.txt
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:30:09.301912 eth-trader-api-proto-0.0.5/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-05-31 18:30:09.301751 eth-trader-api-proto-0.0.5/PKG-INFO
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     1111 2023-05-31 18:27:59.000000 eth-trader-api-proto-0.0.5/README.md
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      357 2023-05-31 18:27:49.000000 eth-trader-api-proto-0.0.5/pyproject.toml
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       38 2023-05-31 18:30:09.301958 eth-trader-api-proto-0.0.5/setup.cfg
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:30:09.299864 eth-trader-api-proto-0.0.5/src/
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:30:09.300753 eth-trader-api-proto-0.0.5/src/eth_trader_api/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       20 2023-05-31 18:28:56.000000 eth-trader-api-proto-0.0.5/src/eth_trader_api/__init__.py
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     4795 2023-05-31 18:28:45.000000 eth-trader-api-proto-0.0.5/src/eth_trader_api/proto.py
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-05-31 18:30:09.301574 eth-trader-api-proto-0.0.5/src/eth_trader_api_proto.egg-info/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-05-31 18:30:09.000000 eth-trader-api-proto-0.0.5/src/eth_trader_api_proto.egg-info/PKG-INFO
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      322 2023-05-31 18:30:09.000000 eth-trader-api-proto-0.0.5/src/eth_trader_api_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)        1 2023-05-31 18:30:09.000000 eth-trader-api-proto-0.0.5/src/eth_trader_api_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       22 2023-05-31 18:30:09.000000 eth-trader-api-proto-0.0.5/src/eth_trader_api_proto.egg-info/requires.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       15 2023-05-31 18:30:09.000000 eth-trader-api-proto-0.0.5/src/eth_trader_api_proto.egg-info/top_level.txt
```

### Comparing `eth-trader-api-proto-0.0.4/README.md` & `eth-trader-api-proto-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     cd python
     rm -rf dist/ && python3 -m build 
 ```
 
 you can install package locally before uploading it to the pypi
 
 ```shell
-    pip install dist/eth_trader_api_proto_0.0.3.tar.gz
+    pip install dist/eth-trader-api-proto-0.0.5.tar.gz
 ```
 
     (Don't forget to fix the proto compilation issues before releasing)
     To upload this library officially to pypi, use this command
 
 ```shell
     python3 -m twine upload --repository pypi dist/*
```

### Comparing `eth-trader-api-proto-0.0.4/src/eth_trader_api/proto.py` & `eth-trader-api-proto-0.0.5/src/eth_trader_api/proto.py`

 * *Files identical despite different names*

