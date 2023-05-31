# Comparing `tmp/ctransformers-0.2.3.tar.gz` & `tmp/ctransformers-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctransformers-0.2.3.tar", last modified: Tue May 30 23:11:24 2023, max compression
+gzip compressed data, was "ctransformers-0.2.4.tar", last modified: Wed May 31 19:04:06 2023, max compression
```

## Comparing `ctransformers-0.2.3.tar` & `ctransformers-0.2.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.464320 ctransformers-0.2.3/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       43 2023-05-08 17:08:45.000000 ctransformers-0.2.3/.gitattributes
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.434320 ctransformers-0.2.3/.github/
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.444320 ctransformers-0.2.3/.github/workflows/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1325 2023-05-29 18:06:10.000000 ctransformers-0.2.3/.github/workflows/build.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      981 2023-05-14 22:40:02.000000 ctransformers-0.2.3/.github/workflows/tests.yml
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13506 2023-05-14 12:42:43.000000 ctransformers-0.2.3/.gitignore
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      211 2023-05-29 14:27:39.000000 ctransformers-0.2.3/.gitmodules
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4266 2023-05-30 20:08:54.000000 ctransformers-0.2.3/CMakeLists.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1078 2023-05-08 17:08:55.000000 ctransformers-0.2.3/LICENSE
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18486 2023-05-30 23:11:24.464320 ctransformers-0.2.3/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13658 2023-05-30 23:09:34.000000 ctransformers-0.2.3/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.444320 ctransformers-0.2.3/ctransformers/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.2.3/ctransformers/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5866 2023-05-19 19:43:30.000000 ctransformers-0.2.3/ctransformers/hub.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2616 2023-05-21 14:15:12.000000 ctransformers-0.2.3/ctransformers/langchain.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1251 2023-05-29 21:19:55.000000 ctransformers-0.2.3/ctransformers/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    15833 2023-05-30 15:15:11.000000 ctransformers-0.2.3/ctransformers/llm.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1146 2023-05-27 21:21:35.000000 ctransformers-0.2.3/ctransformers/utils.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.444320 ctransformers-0.2.3/ctransformers.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18486 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      998 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-30 23:11:23.000000 ctransformers-0.2.3/ctransformers.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-30 23:11:24.000000 ctransformers-0.2.3/ctransformers.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.444320 ctransformers-0.2.3/models/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4905 2023-05-29 15:42:12.000000 ctransformers-0.2.3/models/common.h
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.454320 ctransformers-0.2.3/models/ggml/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    34896 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/ggml-cuda.cu
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      906 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/ggml-cuda.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   506603 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/ggml.c
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    38058 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/ggml.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13668 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/llama-util.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    96303 2023-05-30 14:35:21.000000 ctransformers-0.2.3/models/ggml/llama.cpp
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    14098 2023-05-29 18:16:36.000000 ctransformers-0.2.3/models/ggml/llama.h
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2924 2023-05-30 12:22:12.000000 ctransformers-0.2.3/models/llm.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7218 2023-05-30 12:18:34.000000 ctransformers-0.2.3/models/llm.h
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.464320 ctransformers-0.2.3/models/llms/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21413 2023-05-30 20:22:27.000000 ctransformers-0.2.3/models/llms/dolly.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21973 2023-05-30 20:20:35.000000 ctransformers-0.2.3/models/llms/gpt-neox.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    22306 2023-05-30 20:19:06.000000 ctransformers-0.2.3/models/llms/gpt2.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19234 2023-05-30 20:17:33.000000 ctransformers-0.2.3/models/llms/gptj.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3324 2023-05-30 13:26:40.000000 ctransformers-0.2.3/models/llms/llama.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18424 2023-05-30 20:16:14.000000 ctransformers-0.2.3/models/llms/mpt.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)    24167 2023-05-30 20:13:06.000000 ctransformers-0.2.3/models/llms/starcoder.cc
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      150 2023-05-29 18:34:56.000000 ctransformers-0.2.3/pyproject.toml
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.464320 ctransformers-0.2.3/scripts/
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)      107 2023-05-29 18:06:51.000000 ctransformers-0.2.3/scripts/build.sh
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)     1427 2023-05-30 12:31:41.000000 ctransformers-0.2.3/scripts/docs.py
--rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)      550 2023-05-30 19:39:09.000000 ctransformers-0.2.3/scripts/release.sh
--rwxr--r--   0 ravindra  (1000) ravindra  (1000)      603 2023-05-29 14:52:08.000000 ctransformers-0.2.3/scripts/sync.sh
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-30 23:11:24.464320 ctransformers-0.2.3/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1801 2023-05-30 23:10:19.000000 ctransformers-0.2.3/setup.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-30 23:11:24.464320 ctransformers-0.2.3/tests/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 17:05:29.000000 ctransformers-0.2.3/tests/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      285 2023-05-14 17:57:20.000000 ctransformers-0.2.3/tests/conftest.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1678 2023-05-17 19:46:10.000000 ctransformers-0.2.3/tests/test_llm.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      618 2023-05-27 19:08:53.000000 ctransformers-0.2.3/tests/test_model.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.142619 ctransformers-0.2.4/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       43 2023-05-08 17:08:45.000000 ctransformers-0.2.4/.gitattributes
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.102619 ctransformers-0.2.4/.github/
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.112619 ctransformers-0.2.4/.github/workflows/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1325 2023-05-29 18:06:10.000000 ctransformers-0.2.4/.github/workflows/build.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      981 2023-05-14 22:40:02.000000 ctransformers-0.2.4/.github/workflows/tests.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13506 2023-05-14 12:42:43.000000 ctransformers-0.2.4/.gitignore
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      211 2023-05-29 14:27:39.000000 ctransformers-0.2.4/.gitmodules
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4266 2023-05-30 20:08:54.000000 ctransformers-0.2.4/CMakeLists.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1078 2023-05-08 17:08:55.000000 ctransformers-0.2.4/LICENSE
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18486 2023-05-31 19:04:06.142619 ctransformers-0.2.4/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13658 2023-05-31 14:49:16.000000 ctransformers-0.2.4/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.112619 ctransformers-0.2.4/ctransformers/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       79 2023-05-14 08:13:36.000000 ctransformers-0.2.4/ctransformers/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6243 2023-05-31 15:56:09.000000 ctransformers-0.2.4/ctransformers/hub.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2620 2023-05-31 14:40:49.000000 ctransformers-0.2.4/ctransformers/langchain.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1260 2023-05-31 14:40:56.000000 ctransformers-0.2.4/ctransformers/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    15840 2023-05-31 14:47:17.000000 ctransformers-0.2.4/ctransformers/llm.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1146 2023-05-31 14:33:57.000000 ctransformers-0.2.4/ctransformers/utils.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.122619 ctransformers-0.2.4/ctransformers.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18486 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      998 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-31 19:04:05.000000 ctransformers-0.2.4/ctransformers.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       32 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       14 2023-05-31 19:04:06.000000 ctransformers-0.2.4/ctransformers.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.122619 ctransformers-0.2.4/models/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4905 2023-05-29 15:42:12.000000 ctransformers-0.2.4/models/common.h
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.132619 ctransformers-0.2.4/models/ggml/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    34896 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/ggml-cuda.cu
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      906 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/ggml-cuda.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   506603 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/ggml.c
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    38058 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/ggml.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    13668 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/llama-util.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    96303 2023-05-30 14:35:21.000000 ctransformers-0.2.4/models/ggml/llama.cpp
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    14098 2023-05-29 18:16:36.000000 ctransformers-0.2.4/models/ggml/llama.h
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2924 2023-05-30 12:22:12.000000 ctransformers-0.2.4/models/llm.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7218 2023-05-30 12:18:34.000000 ctransformers-0.2.4/models/llm.h
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.132619 ctransformers-0.2.4/models/llms/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21413 2023-05-30 20:22:27.000000 ctransformers-0.2.4/models/llms/dolly.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    21973 2023-05-30 20:20:35.000000 ctransformers-0.2.4/models/llms/gpt-neox.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    22306 2023-05-30 20:19:06.000000 ctransformers-0.2.4/models/llms/gpt2.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    19234 2023-05-30 20:17:33.000000 ctransformers-0.2.4/models/llms/gptj.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3324 2023-05-30 13:26:40.000000 ctransformers-0.2.4/models/llms/llama.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    18424 2023-05-30 20:16:14.000000 ctransformers-0.2.4/models/llms/mpt.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)    24167 2023-05-30 20:13:06.000000 ctransformers-0.2.4/models/llms/starcoder.cc
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      150 2023-05-29 18:34:56.000000 ctransformers-0.2.4/pyproject.toml
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.142619 ctransformers-0.2.4/scripts/
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)      107 2023-05-29 18:06:51.000000 ctransformers-0.2.4/scripts/build.sh
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)     1432 2023-05-31 14:30:46.000000 ctransformers-0.2.4/scripts/docs.py
+-rwxr-xr-x   0 ravindra  (1000) ravindra  (1000)      550 2023-05-30 19:39:09.000000 ctransformers-0.2.4/scripts/release.sh
+-rwxr--r--   0 ravindra  (1000) ravindra  (1000)      603 2023-05-29 14:52:08.000000 ctransformers-0.2.4/scripts/sync.sh
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-31 19:04:06.142619 ctransformers-0.2.4/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1796 2023-05-31 19:03:06.000000 ctransformers-0.2.4/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-31 19:04:06.142619 ctransformers-0.2.4/tests/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-05-14 17:05:29.000000 ctransformers-0.2.4/tests/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      261 2023-05-31 14:31:30.000000 ctransformers-0.2.4/tests/conftest.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1676 2023-05-31 14:32:37.000000 ctransformers-0.2.4/tests/test_llm.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      566 2023-05-31 14:33:25.000000 ctransformers-0.2.4/tests/test_model.py
```

### Comparing `ctransformers-0.2.3/.github/workflows/build.yml` & `ctransformers-0.2.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/.github/workflows/tests.yml` & `ctransformers-0.2.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/.gitignore` & `ctransformers-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/CMakeLists.txt` & `ctransformers-0.2.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/LICENSE` & `ctransformers-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/PKG-INFO` & `ctransformers-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
```

### Comparing `ctransformers-0.2.3/README.md` & `ctransformers-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/ctransformers/hub.py` & `ctransformers-0.2.4/ctransformers/hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import json
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
-from huggingface_hub import snapshot_download
+from huggingface_hub import HfApi, snapshot_download
 from huggingface_hub.utils import validate_repo_id, HFValidationError
 
 from .llm import Config, LLM
 
 
 def get_path_type(path: str) -> Optional[str]:
     p = Path(path)
     if p.is_file():
-        return 'file'
+        return "file"
     elif p.is_dir():
-        return 'dir'
+        return "dir"
     try:
         validate_repo_id(path)
-        return 'repo'
+        return "repo"
     except HFValidationError:
         pass
 
 
 @dataclass
 class AutoConfig:
     config: Config
     model_type: Optional[str] = None
 
     @classmethod
     def from_pretrained(
         cls,
         model_path_or_repo_id: str,
         **kwargs,
-    ) -> 'AutoConfig':
+    ) -> "AutoConfig":
         path_type = get_path_type(model_path_or_repo_id)
         if not path_type:
-            raise ValueError(
-                f"Model path '{model_path_or_repo_id}' doesn't exist.")
+            raise ValueError(f"Model path '{model_path_or_repo_id}' doesn't exist.")
 
         config = Config()
         auto_config = AutoConfig(config=config)
 
-        if path_type == 'dir':
+        if path_type == "dir":
             cls._update_from_dir(model_path_or_repo_id, auto_config)
-        elif path_type == 'repo':
+        elif path_type == "repo":
             cls._update_from_repo(model_path_or_repo_id, auto_config)
 
         for k, v in kwargs.items():
             if not hasattr(config, k):
                 raise TypeError(
                     f"'{k}' is an invalid keyword argument for from_pretrained()"
                 )
@@ -55,47 +54,46 @@
 
         return auto_config
 
     @classmethod
     def _update_from_repo(
         cls,
         repo_id: str,
-        auto_config: 'AutoConfig',
+        auto_config: "AutoConfig",
     ) -> None:
-        path = snapshot_download(repo_id=repo_id, allow_patterns='config.json')
+        path = snapshot_download(repo_id=repo_id, allow_patterns="config.json")
         cls._update_from_dir(path, auto_config)
 
     @classmethod
-    def _update_from_dir(cls, path: str, auto_config: 'AutoConfig') -> None:
-        path = (Path(path) / 'config.json').resolve()
+    def _update_from_dir(cls, path: str, auto_config: "AutoConfig") -> None:
+        path = (Path(path) / "config.json").resolve()
         if path.is_file():
             cls._update_from_file(path, auto_config)
 
     @classmethod
-    def _update_from_file(cls, path: str, auto_config: 'AutoConfig') -> None:
+    def _update_from_file(cls, path: str, auto_config: "AutoConfig") -> None:
         with open(path) as f:
             config = json.load(f)
 
-        auto_config.model_type = config.get('model_type')
-        params = config.get('task_specific_params', {})
-        params = params.get('text-generation', {})
+        auto_config.model_type = config.get("model_type")
+        params = config.get("task_specific_params", {})
+        params = params.get("text-generation", {})
         for name in [
-                'top_k',
-                'top_p',
-                'temperature',
-                'repetition_penalty',
-                'last_n_tokens',
+            "top_k",
+            "top_p",
+            "temperature",
+            "repetition_penalty",
+            "last_n_tokens",
         ]:
             value = params.get(name)
             if value is not None:
                 setattr(auto_config.config, name, value)
 
 
 class AutoModelForCausalLM:
-
     @classmethod
     def from_pretrained(
         cls,
         model_path_or_repo_id: str,
         *,
         model_type: Optional[str] = None,
         model_file: Optional[str] = None,
@@ -125,64 +123,75 @@
             raise ValueError(
                 "Unable to detect model type. Please specify a model type using:\n\n"
                 "  AutoModelForCausalLM.from_pretrained(..., model_type='...')\n\n"
             )
 
         path_type = get_path_type(model_path_or_repo_id)
         model_path = None
-        if path_type == 'file':
+        if path_type == "file":
             model_path = model_path_or_repo_id
-        elif path_type == 'dir':
-            model_path = cls._find_model_path_from_dir(model_path_or_repo_id,
-                                                       model_file)
-        elif path_type == 'repo':
+        elif path_type == "dir":
+            model_path = cls._find_model_path_from_dir(
+                model_path_or_repo_id, model_file
+            )
+        elif path_type == "repo":
             model_path = cls._find_model_path_from_repo(
-                model_path_or_repo_id, model_file)
+                model_path_or_repo_id, model_file
+            )
 
         return LLM(
             model_path=model_path,
             model_type=model_type,
             config=config.config,
             lib=lib,
         )
 
     @classmethod
     def _find_model_path_from_repo(
         cls,
         repo_id: str,
         filename: Optional[str] = None,
     ) -> str:
-        allow_patterns = filename or '*.bin'
-        path = snapshot_download(repo_id=repo_id,
-                                 allow_patterns=allow_patterns)
+        if not filename:
+            filename = cls._find_model_file_from_repo(repo_id=repo_id)
+        path = snapshot_download(repo_id=repo_id, allow_patterns=filename)
         return cls._find_model_path_from_dir(path, filename=filename)
 
     @classmethod
+    def _find_model_file_from_repo(cls, repo_id: str) -> Optional[str]:
+        api = HfApi()
+        repo_info = api.repo_info(repo_id=repo_id, files_metadata=True)
+        files = [
+            (f.size, f.rfilename)
+            for f in repo_info.siblings
+            if f.rfilename.endswith(".bin")
+        ]
+        if not files:
+            raise ValueError(f"No model file found in repo '{repo_id}'")
+        return min(files)[1]
+
+    @classmethod
     def _find_model_path_from_dir(
         cls,
         path: str,
         filename: Optional[str] = None,
     ) -> str:
         path = Path(path).resolve()
         if filename:
             file = (path / filename).resolve()
             if not file.is_file():
-                raise ValueError(
-                    f"Model file '{filename}' not found in '{path}'")
+                raise ValueError(f"Model file '{filename}' not found in '{path}'")
             return str(file)
 
-        files = [
-            f for f in path.iterdir()
-            if f.is_file() and f.name.endswith('.bin')
-        ]
+        files = [f for f in path.iterdir() if f.is_file() and f.name.endswith(".bin")]
 
         if len(files) == 0:
-            raise ValueError(f"No model files found in '{path}'")
+            raise ValueError(f"No model file found in directory '{path}'")
         elif len(files) > 1:
-            names = '\n'.join([' - ' + f.name for f in files])
+            names = "\n".join([" - " + f.name for f in files])
             raise ValueError(
                 f"Multiple model files found in '{path}':\n\n{names}\n\n"
                 "Please specify a model file using:\n\n"
                 "  AutoModelForCausalLM.from_pretrained(..., model_file='...')\n\n"
             )
 
         return str(files[0].resolve())
```

### Comparing `ctransformers-0.2.3/ctransformers/langchain.py` & `ctransformers-0.2.4/ctransformers/langchain.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 try:
     from langchain.llms.base import LLM
 except ImportError:
     raise ImportError(
-        'To use the ctransformers.langchain module, please install the '
-        '`langchain` python package: `pip install langchain`')
+        "To use the ctransformers.langchain module, please install the "
+        "`langchain` python package: `pip install langchain`"
+    )
 
 from typing import Any, Dict, Optional, Sequence
 
 from pydantic import root_validator
 from langchain.callbacks.manager import CallbackManagerForLLMRun
 
 from ctransformers import AutoModelForCausalLM
 
 
 class CTransformers(LLM):
     """Wrapper around the C Transformers LLM interface.
 
-     To use, you should have the `langchain` python package installed.
+    To use, you should have the `langchain` python package installed.
     """
 
     client: Any  #: :meta private:
 
     model: str
     """The path to a model file or directory or the name of a Hugging Face Hub
     model repo."""
@@ -37,34 +38,34 @@
     lib: Optional[Any] = None
     """The path to a shared library or one of `avx2`, `avx`, `basic`."""
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
         return {
-            'model': self.model,
-            'model_type': self.model_type,
-            'model_file': self.model_file,
-            'config': self.config,
+            "model": self.model,
+            "model_type": self.model_type,
+            "model_file": self.model_file,
+            "config": self.config,
         }
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
-        return 'ctransformers'
+        return "ctransformers"
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate and load model from a local file or remote repo."""
-        config = values['config'] or {}
-        values['client'] = AutoModelForCausalLM.from_pretrained(
-            values['model'],
-            model_type=values['model_type'],
-            model_file=values['model_file'],
-            lib=values['lib'],
+        config = values["config"] or {}
+        values["client"] = AutoModelForCausalLM.from_pretrained(
+            values["model"],
+            model_type=values["model_type"],
+            model_file=values["model_file"],
+            lib=values["lib"],
             **config,
         )
         return values
 
     def _call(
         self,
         prompt: str,
@@ -81,8 +82,8 @@
             The generated text.
         """
         text = []
         for chunk in self.client(prompt, stop=stop, stream=True):
             text.append(chunk)
             if run_manager:
                 run_manager.on_llm_new_token(chunk, verbose=self.verbose)
-        return ''.join(text)
+        return "".join(text)
```

### Comparing `ctransformers-0.2.3/ctransformers/lib.py` & `ctransformers-0.2.4/ctransformers/lib.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from typing import Optional
 import platform
 from pathlib import Path
 
 
 def find_library(path: Optional[str] = None) -> str:
-    lib_directory = Path(__file__).parent.resolve() / 'lib'
+    lib_directory = Path(__file__).parent.resolve() / "lib"
 
     if path:
         subdirs = [d.name for d in lib_directory.iterdir() if d.is_dir()]
         if path not in subdirs:
             return path
 
     system = platform.system()
     if not path:
-        if (lib_directory / 'local').is_dir():
-            path = 'local'
-        elif platform.processor() == 'arm':
+        if (lib_directory / "local").is_dir():
+            path = "local"
+        elif platform.processor() == "arm":
             # Apple silicon doesn't support AVX/AVX2.
-            path = 'basic' if system == 'Darwin' else ''
+            path = "basic" if system == "Darwin" else ""
         else:
-            path = 'avx2'
+            path = "avx2"
 
-    name = 'ctransformers'
-    if system == 'Linux':
-        name = f'lib{name}.so'
-    elif system == 'Windows':
-        name = f'{name}.dll'
-    elif system == 'Darwin':
-        name = f'lib{name}.dylib'
+    name = "ctransformers"
+    if system == "Linux":
+        name = f"lib{name}.so"
+    elif system == "Windows":
+        name = f"{name}.dll"
+    elif system == "Darwin":
+        name = f"lib{name}.dylib"
     else:
-        name = ''
+        name = ""
 
     path = lib_directory / path / name
     if not path.is_file():
         raise OSError(
-            'Precompiled binaries are not available for the current platform. '
-            'Please reinstall from source using:\n\n'
-            '  pip uninstall ctransformers --yes\n'
-            '  pip install ctransformers --no-binary ctransformers\n\n')
+            "Precompiled binaries are not available for the current platform. "
+            "Please reinstall from source using:\n\n"
+            "  pip uninstall ctransformers --yes\n"
+            "  pip install ctransformers --no-binary ctransformers\n\n"
+        )
     return str(path)
```

### Comparing `ctransformers-0.2.3/ctransformers/llm.py` & `ctransformers-0.2.4/ctransformers/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,53 +54,53 @@
 
     # model
     context_length: int = -1
     gpu_layers: int = 0
 
 
 docs = OrderedDict(
-    top_k='The top-k value to use for sampling.',
-    top_p='The top-p value to use for sampling.',
-    temperature='The temperature to use for sampling.',
-    repetition_penalty='The repetition penalty to use for sampling.',
-    last_n_tokens='The number of last tokens to use for repetition penalty.',
-    seed='The seed value to use for sampling tokens.',
-    max_new_tokens='The maximum number of new tokens to generate.',
-    stop='A list of sequences to stop generation when encountered.',
-    stream='Whether to stream the generated text.',
-    reset='Whether to reset the model state before generating text.',
-    batch_size='The batch size to use for evaluating tokens.',
-    threads='The number of threads to use for evaluating tokens.',
-    context_length='The maximum context length to use.',
-    gpu_layers='The number of layers to run on GPU.',
+    top_k="The top-k value to use for sampling.",
+    top_p="The top-p value to use for sampling.",
+    temperature="The temperature to use for sampling.",
+    repetition_penalty="The repetition penalty to use for sampling.",
+    last_n_tokens="The number of last tokens to use for repetition penalty.",
+    seed="The seed value to use for sampling tokens.",
+    max_new_tokens="The maximum number of new tokens to generate.",
+    stop="A list of sequences to stop generation when encountered.",
+    stream="Whether to stream the generated text.",
+    reset="Whether to reset the model state before generating text.",
+    batch_size="The batch size to use for evaluating tokens.",
+    threads="The number of threads to use for evaluating tokens.",
+    context_length="The maximum context length to use.",
+    gpu_layers="The number of layers to run on GPU.",
 )
 
 
 def doc(fn):
     doc = []
     for param in inspect.signature(fn).parameters:
         if param in docs:
             default = getattr(Config, param)
-            doc.append(f'{param}: {docs[param]} Default: `{default}`')
-    doc = ('\n' + ' ' * 12).join(doc)
+            doc.append(f"{param}: {docs[param]} Default: `{default}`")
+    doc = ("\n" + " " * 12).join(doc)
     fn.__doc__ = fn.__doc__.format(params=doc)
     return fn
 
 
 def get(*values):
     for value in values:
         if value is not None:
             return value
 
 
 def load_library(path: Optional[str] = None) -> Any:
     # https://docs.python.org/3.8/whatsnew/3.8.html#bpo-36085-whatsnew
     # https://github.com/abetlen/llama-cpp-python/pull/225
-    if hasattr(os, 'add_dll_directory') and 'CUDA_PATH' in os.environ:
-        os.add_dll_directory(os.path.join(os.environ['CUDA_PATH'], 'bin'))
+    if hasattr(os, "add_dll_directory") and "CUDA_PATH" in os.environ:
+        os.add_dll_directory(os.path.join(os.environ["CUDA_PATH"], "bin"))
 
     path = find_library(path)
     lib = CDLL(path)
 
     lib.ctransformers_llm_create.argtypes = [
         c_char_p,  # model_path
         c_char_p,  # model_type
@@ -164,15 +164,14 @@
     lib.ctransformers_llm_reset.argtypes = [llm_p]
     lib.ctransformers_llm_reset.restype = None
 
     return lib
 
 
 class LLM:
-
     def __init__(
         self,
         model_path: str,
         model_type: str,
         *,
         config: Optional[Config] = None,
         lib: Optional[str] = None,
@@ -200,15 +199,16 @@
             model_path.encode(),
             model_type.encode(),
             config.context_length,
             config.gpu_layers,
         )
         if self._llm is None:
             raise RuntimeError(
-                f"Failed to create LLM '{model_type}' from '{model_path}'.")
+                f"Failed to create LLM '{model_type}' from '{model_path}'."
+            )
 
     @property
     def model_path(self) -> str:
         """The path to the model file."""
         return self._model_path
 
     @property
@@ -220,26 +220,30 @@
     def config(self) -> Config:
         """The config object."""
         return self._config
 
     @property
     def logits(self) -> List[float]:
         """The unnormalized log probabilities."""
-        return Vector(self.ctransformers_llm_logits_data(),
-                      self.ctransformers_llm_logits_size())
+        return Vector(
+            self.ctransformers_llm_logits_data(),
+            self.ctransformers_llm_logits_size(),
+        )
 
     @property
     def embeddings(self) -> List[float]:
         """The input embeddings."""
-        return Vector(self.ctransformers_llm_embeddings_data(),
-                      self.ctransformers_llm_embeddings_size())
+        return Vector(
+            self.ctransformers_llm_embeddings_data(),
+            self.ctransformers_llm_embeddings_size(),
+        )
 
     def __getattr__(self, name: str) -> Callable:
         lib, llm = self._lib, self._llm
-        if name.startswith('ctransformers_llm_') and hasattr(lib, name):
+        if name.startswith("ctransformers_llm_") and hasattr(lib, name):
             return partial(getattr(lib, name), llm)
         raise AttributeError(f"'LLM' object has no attribute '{name}'")
 
     def tokenize(self, text: str) -> List[int]:
         """Converts a text into list of tokens.
 
         Args:
@@ -263,15 +267,15 @@
         """
         if isinstance(tokens, int):
             tokens = [tokens]
         texts = []
         for token in tokens:
             text = self.ctransformers_llm_detokenize(token)
             texts.append(text.decode())
-        return ''.join(texts)
+        return "".join(texts)
 
     def is_eos_token(self, token: int) -> bool:
         """Checks if a token is an end-of-sequence token.
 
         Args:
             token: The token to check.
 
@@ -296,18 +300,22 @@
         """
         config = self.config
         batch_size = get(batch_size, config.batch_size)
         threads = get(threads, config.threads)
 
         n_tokens = len(tokens)
         tokens = (c_int * n_tokens)(*tokens)
-        status = self.ctransformers_llm_batch_eval(tokens, n_tokens,
-                                                   batch_size, threads)
+        status = self.ctransformers_llm_batch_eval(
+            tokens,
+            n_tokens,
+            batch_size,
+            threads,
+        )
         if not status:
-            raise RuntimeError('Failed to evaluate tokens.')
+            raise RuntimeError("Failed to evaluate tokens.")
 
     @doc
     def sample(
         self,
         *,
         top_k: Optional[int] = None,
         top_p: Optional[float] = None,
@@ -414,38 +422,38 @@
         max_new_tokens = get(max_new_tokens, config.max_new_tokens)
         stop = get(stop, config.stop) or []
         if isinstance(stop, str):
             stop = [stop]
 
         tokens = self.tokenize(prompt)
 
-        stop_regex = re.compile('|'.join(map(re.escape, stop)))
+        stop_regex = re.compile("|".join(map(re.escape, stop)))
         count = 0
-        text = ''
+        text = ""
         for token in self.generate(
-                tokens,
-                top_k=top_k,
-                top_p=top_p,
-                temperature=temperature,
-                repetition_penalty=repetition_penalty,
-                last_n_tokens=last_n_tokens,
-                seed=seed,
-                batch_size=batch_size,
-                threads=threads,
-                reset=reset,
+            tokens,
+            top_k=top_k,
+            top_p=top_p,
+            temperature=temperature,
+            repetition_penalty=repetition_penalty,
+            last_n_tokens=last_n_tokens,
+            seed=seed,
+            batch_size=batch_size,
+            threads=threads,
+            reset=reset,
         ):
             text += self.detokenize([token])
 
             # https://github.com/abetlen/llama-cpp-python/blob/1a13d76c487df1c8560132d10bda62d6e2f4fa93/llama_cpp/llama.py#L686-L706
             # Check if one of the stop sequences is part of the text.
             # Note that the stop sequence may not always be at the end of text.
             if stop:
                 match = stop_regex.search(text)
                 if match:
-                    text = text[:match.start()]
+                    text = text[: match.start()]
                     break
 
             # Avoid sending the longest suffix of text which is also a prefix
             # of a stop sequence, as it can form a stop sequence with the text
             # generated later.
             longest = 0
             for s in stop:
@@ -508,15 +516,15 @@
             batch_size=batch_size,
             threads=threads,
             stop=stop,
             reset=reset,
         )
         if stream:
             return text
-        return ''.join(text)
+        return "".join(text)
 
     @doc
     def embed(
         self,
         input: Union[str, Sequence[int]],
         *,
         batch_size: Optional[int] = None,
```

### Comparing `ctransformers-0.2.3/ctransformers/utils.py` & `ctransformers-0.2.4/ctransformers/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         self._data[index] = value
 
     def __len__(self) -> int:
         return self._size
 
     def _validate_index(self, index: int) -> None:
         if not isinstance(index, int):
-            raise TypeError('list index must be integer')
+            raise TypeError("list index must be integer")
         if not 0 <= index < self._size:
-            raise IndexError('list index out of range')
+            raise IndexError("list index out of range")
 
     def __delitem__(self, index: int) -> None:
-        raise NotImplementedError('This operation is not allowed.')
+        raise NotImplementedError("This operation is not allowed.")
 
     def insert(self, index: int, value: Any) -> None:
-        raise NotImplementedError('This operation is not allowed.')
+        raise NotImplementedError("This operation is not allowed.")
```

### Comparing `ctransformers-0.2.3/ctransformers.egg-info/PKG-INFO` & `ctransformers-0.2.4/ctransformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctransformers
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python bindings for the Transformer models implemented in C/C++ using GGML library.
 Home-page: https://github.com/marella/ctransformers
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [C Transformers](https://github.com/marella/ctransformers) [![PyPI](https://img.shields.io/pypi/v/ctransformers)](https://pypi.org/project/ctransformers/) [![tests](https://github.com/marella/ctransformers/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/tests.yml) [![build](https://github.com/marella/ctransformers/actions/workflows/build.yml/badge.svg)](https://github.com/marella/ctransformers/actions/workflows/build.yml)
```

### Comparing `ctransformers-0.2.3/ctransformers.egg-info/SOURCES.txt` & `ctransformers-0.2.4/ctransformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/common.h` & `ctransformers-0.2.4/models/common.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/ggml/ggml-cuda.cu` & `ctransformers-0.2.4/models/ggml/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/ggml/ggml-cuda.h` & `ctransformers-0.2.4/models/ggml/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/ggml/ggml.c` & `ctransformers-0.2.4/models/ggml/ggml.c`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/ggml/ggml.h` & `ctransformers-0.2.4/models/ggml/ggml.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/ggml/llama-util.h` & `ctransformers-0.2.4/models/ggml/llama-util.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/ggml/llama.cpp` & `ctransformers-0.2.4/models/ggml/llama.cpp`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/ggml/llama.h` & `ctransformers-0.2.4/models/ggml/llama.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llm.cc` & `ctransformers-0.2.4/models/llm.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llm.h` & `ctransformers-0.2.4/models/llm.h`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llms/dolly.cc` & `ctransformers-0.2.4/models/llms/dolly.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llms/gpt-neox.cc` & `ctransformers-0.2.4/models/llms/gpt-neox.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llms/gpt2.cc` & `ctransformers-0.2.4/models/llms/gpt2.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llms/gptj.cc` & `ctransformers-0.2.4/models/llms/gptj.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llms/llama.cc` & `ctransformers-0.2.4/models/llms/llama.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llms/mpt.cc` & `ctransformers-0.2.4/models/llms/mpt.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/models/llms/starcoder.cc` & `ctransformers-0.2.4/models/llms/starcoder.cc`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/scripts/docs.py` & `ctransformers-0.2.4/scripts/docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,41 +18,42 @@
 
 ### Config
 
 | Parameter | Type  | Description | Default |
 | :-------- | :---- | :---------- | :------ |
 """
 for param, description in config_docs.items():
-    if param == 'stop':
-        type_ = 'List[str]'
+    if param == "stop":
+        type_ = "List[str]"
     else:
         type_ = get_type_hints(Config)[param].__name__
     default = getattr(Config, param)
-    docs += f'| `{param}` | `{type_}` | {description} | `{default}` |\n'
+    docs += f"| `{param}` | `{type_}` | {description} | `{default}` |\n"
 docs += """
 > **Note:** Currently only LLaMA models support the `context_length` and `gpu_layers` parameters.
 """
 
 # Class Docs
 
 generator = MarkdownGenerator()
 for class_ in (AutoModelForCausalLM, LLM):
     docs += generator.class2md(class_, depth=3)
-docs += '---\n' + generator.func2md(LLM.__call__, clsname='LLM', depth=4)
+docs += "---\n" + generator.func2md(LLM.__call__, clsname="LLM", depth=4)
 
 # Save
 
-README = ROOT / 'README.md'
-MARKER = '<!-- API_DOCS -->'
+README = ROOT / "README.md"
+MARKER = "<!-- API_DOCS -->"
 
 with open(README) as f:
     contents = f.read()
 
 parts = contents.split(MARKER)
 if len(parts) != 3:
     raise RuntimeError(
-        f"README should have exactly 2 '{MARKER}' but has {len(parts) - 1}.")
+        f"README should have exactly 2 '{MARKER}' but has {len(parts) - 1}."
+    )
 parts[1] = docs
 contents = MARKER.join(parts)
 
-with open(README, mode='w') as f:
+with open(README, mode="w") as f:
     f.write(contents)
```

### Comparing `ctransformers-0.2.3/scripts/release.sh` & `ctransformers-0.2.4/scripts/release.sh`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/scripts/sync.sh` & `ctransformers-0.2.4/scripts/sync.sh`

 * *Files identical despite different names*

### Comparing `ctransformers-0.2.3/tests/test_llm.py` & `ctransformers-0.2.4/tests/test_llm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 from ctransformers import LLM, Config
 
 
 class MockLLM(LLM):
-
     def __init__(self):
         self._config = Config()
         self._llm = None
 
     @property
     def config(self):
         return self._config
 
     def tokenize(self, prompt, **kwargs):
-        self.tokens = prompt.split(' ')
+        self.tokens = prompt.split(" ")
         return range(len(self.tokens))
 
     def generate(self, tokens, **kwargs):
         return tokens
 
     def detokenize(self, tokens):
-        return ' ' + self.tokens[tokens[0]]
+        return " " + self.tokens[tokens[0]]
 
 
 class TestLLM:
-
     def test_stop(self):
         llm = MockLLM()
-        prompt = 'foo bar baz lorem ipsum\ndolor'
+        prompt = "foo bar baz lorem ipsum\ndolor"
         expected = [
-            ([], ' foo bar baz lorem ipsum\ndolor'),
-            (['dolor '], ' foo bar baz lorem ipsum\ndolor'),
-            (['ipsum '], ' foo bar baz lorem ipsum\ndolor'),
-            (['doloro'], ' foo bar baz lorem ipsum\ndolor'),
-            (['ipsumo'], ' foo bar baz lorem ipsum\ndolor'),
-            (['dolor'], ' foo bar baz lorem ipsum\n'),
-            (['ipsum'], ' foo bar baz lorem '),
-            (['olor'], ' foo bar baz lorem ipsum\nd'),
-            (['olo'], ' foo bar baz lorem ipsum\nd'),
-            (['psum'], ' foo bar baz lorem i'),
-            (['psu'], ' foo bar baz lorem i'),
-            (['z lor'], ' foo bar ba'),
-            (['rem', 'or'], ' foo bar baz l'),
-            (['foo'], ' '),
-            (['f'], ' '),
-            ([' '], ''),
-            (['\n'], ' foo bar baz lorem ipsum'),
-            (['m\nd'], ' foo bar baz lorem ipsu'),
+            ([], " foo bar baz lorem ipsum\ndolor"),
+            (["dolor "], " foo bar baz lorem ipsum\ndolor"),
+            (["ipsum "], " foo bar baz lorem ipsum\ndolor"),
+            (["doloro"], " foo bar baz lorem ipsum\ndolor"),
+            (["ipsumo"], " foo bar baz lorem ipsum\ndolor"),
+            (["dolor"], " foo bar baz lorem ipsum\n"),
+            (["ipsum"], " foo bar baz lorem "),
+            (["olor"], " foo bar baz lorem ipsum\nd"),
+            (["olo"], " foo bar baz lorem ipsum\nd"),
+            (["psum"], " foo bar baz lorem i"),
+            (["psu"], " foo bar baz lorem i"),
+            (["z lor"], " foo bar ba"),
+            (["rem", "or"], " foo bar baz l"),
+            (["foo"], " "),
+            (["f"], " "),
+            ([" "], ""),
+            (["\n"], " foo bar baz lorem ipsum"),
+            (["m\nd"], " foo bar baz lorem ipsu"),
         ]
         for stop, response in expected:
             assert llm(prompt, stop=stop) == response
             if len(stop) == 1:
                 assert llm(prompt, stop=stop[0]) == response
```

### Comparing `ctransformers-0.2.3/tests/test_model.py` & `ctransformers-0.2.4/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from ctransformers import AutoModelForCausalLM
 
 
 class TestModel:
-
     def test_generate(self, lib):
-        llm = AutoModelForCausalLM.from_pretrained('marella/gpt-2-ggml',
-                                                   lib=lib)
-        response = llm('AI is going to', seed=5, max_new_tokens=3)
-        assert response == ' be a big'
+        llm = AutoModelForCausalLM.from_pretrained("marella/gpt-2-ggml", lib=lib)
+        response = llm("AI is going to", seed=5, max_new_tokens=3)
+        assert response == " be a big"
 
         token = llm.sample()
         logits = llm.logits
         value = logits[token]
         logits[token] -= 1
         assert logits[token] == llm.logits[token] == value - 1
         llm.logits[token] *= 2
```

