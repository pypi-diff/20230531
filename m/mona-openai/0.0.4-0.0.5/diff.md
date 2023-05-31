# Comparing `tmp/mona-openai-0.0.4.tar.gz` & `tmp/mona-openai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mona-openai-0.0.4.tar", last modified: Thu May 25 06:03:54 2023, max compression
+gzip compressed data, was "mona-openai-0.0.5.tar", last modified: Wed May 31 08:24:09 2023, max compression
```

## Comparing `mona-openai-0.0.4.tar` & `mona-openai-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.948670 mona-openai-0.0.4/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.4/LICENSE
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-05-25 06:03:54.948351 mona-openai-0.0.4/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     9162 2023-05-25 05:50:33.000000 mona-openai-0.0.4/README.md
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.943688 mona-openai-0.0.4/mona_openai/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.4/mona_openai/__init__.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.945368 mona-openai-0.0.4/mona_openai/analysis/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/analysis/privacy.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/analysis/profanity.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3121 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/analysis/textual.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.946154 mona-openai-0.0.4/mona_openai/endpoints/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     7675 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/endpoints/chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     5091 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/endpoints/completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/endpoints/endpoint_wrapping.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/endpoints/wrapping_getter.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.4/mona_openai/exceptions.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.4/mona_openai/mona_client.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    14956 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/mona_openai.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.947427 mona-openai-0.0.4/mona_openai/util/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      944 2023-05-11 08:33:47.000000 mona-openai-0.0.4/mona_openai/util/async_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.4/mona_openai/util/func_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/util/oop_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/util/openai_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/util/stream_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.4/mona_openai/util/tokens_util.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.4/mona_openai/util/validation_util.py
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.944664 mona-openai-0.0.4/mona_openai.egg-info/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/PKG-INFO
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/SOURCES.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/dependency_links.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/requires.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-25 06:03:54.000000 mona-openai-0.0.4/mona_openai.egg-info/top_level.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-05-25 05:54:16.000000 mona-openai-0.0.4/pyproject.toml
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.4/requirements.txt
--rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-25 06:03:54.948715 mona-openai-0.0.4/setup.cfg
-drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-25 06:03:54.948138 mona-openai-0.0.4/tests/
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    17351 2023-05-25 05:50:33.000000 mona-openai-0.0.4/tests/test_chat_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)    19272 2023-05-25 05:50:33.000000 mona-openai-0.0.4/tests/test_completion.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.4/tests/test_privacy_analyzer.py
--rw-r--r--   0 itaibarsinai   (501) staff       (20)      852 2023-05-25 05:50:33.000000 mona-openai-0.0.4/tests/test_textual_analyzer.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.728045 mona-openai-0.0.5/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    11356 2023-04-04 12:33:03.000000 mona-openai-0.0.5/LICENSE
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-05-31 08:24:09.727876 mona-openai-0.0.5/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9162 2023-05-25 05:50:33.000000 mona-openai-0.0.5/README.md
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.724794 mona-openai-0.0.5/mona_openai/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       77 2023-05-04 03:41:54.000000 mona-openai-0.0.5/mona_openai/__init__.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.725672 mona-openai-0.0.5/mona_openai/analysis/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3613 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/analysis/privacy.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      304 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/analysis/profanity.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3121 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/analysis/textual.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.726194 mona-openai-0.0.5/mona_openai/endpoints/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     7675 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/endpoints/chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     5091 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/endpoints/completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     4792 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/endpoints/endpoint_wrapping.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      792 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/endpoints/wrapping_getter.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      167 2023-04-04 12:33:03.000000 mona-openai-0.0.5/mona_openai/exceptions.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1379 2023-04-04 12:33:03.000000 mona-openai-0.0.5/mona_openai/mona_client.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    16315 2023-05-31 08:23:40.000000 mona-openai-0.0.5/mona_openai/mona_openai.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.727177 mona-openai-0.0.5/mona_openai/util/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      946 2023-05-31 01:28:56.000000 mona-openai-0.0.5/mona_openai/util/async_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      675 2023-05-11 08:33:47.000000 mona-openai-0.0.5/mona_openai/util/func_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1177 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/util/oop_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      364 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/util/openai_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     3788 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/util/stream_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      776 2023-05-25 05:50:33.000000 mona-openai-0.0.5/mona_openai/util/tokens_util.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      971 2023-04-04 12:33:03.000000 mona-openai-0.0.5/mona_openai/util/validation_util.py
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.725322 mona-openai-0.0.5/mona_openai.egg-info/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     9757 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/PKG-INFO
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      925 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)        1 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       51 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/requires.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       12 2023-05-31 08:24:09.000000 mona-openai-0.0.5/mona_openai.egg-info/top_level.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      818 2023-05-31 08:24:02.000000 mona-openai-0.0.5/pyproject.toml
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       50 2023-05-11 08:33:47.000000 mona-openai-0.0.5/requirements.txt
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)       38 2023-05-31 08:24:09.728080 mona-openai-0.0.5/setup.cfg
+drwxr-xr-x   0 itaibarsinai   (501) staff       (20)        0 2023-05-31 08:24:09.727683 mona-openai-0.0.5/tests/
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    17351 2023-05-25 05:50:33.000000 mona-openai-0.0.5/tests/test_chat_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)    20103 2023-05-31 08:23:40.000000 mona-openai-0.0.5/tests/test_completion.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)     1607 2023-05-25 05:50:33.000000 mona-openai-0.0.5/tests/test_privacy_analyzer.py
+-rw-r--r--   0 itaibarsinai   (501) staff       (20)      852 2023-05-25 05:50:33.000000 mona-openai-0.0.5/tests/test_textual_analyzer.py
```

### Comparing `mona-openai-0.0.4/LICENSE` & `mona-openai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/PKG-INFO` & `mona-openai-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mona-openai-0.0.4/README.md` & `mona-openai-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/analysis/privacy.py` & `mona-openai-0.0.5/mona_openai/analysis/privacy.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/analysis/textual.py` & `mona-openai-0.0.5/mona_openai/analysis/textual.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/endpoints/chat_completion.py` & `mona-openai-0.0.5/mona_openai/endpoints/chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/endpoints/completion.py` & `mona-openai-0.0.5/mona_openai/endpoints/completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/endpoints/endpoint_wrapping.py` & `mona-openai-0.0.5/mona_openai/endpoints/endpoint_wrapping.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/endpoints/wrapping_getter.py` & `mona-openai-0.0.5/mona_openai/endpoints/wrapping_getter.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/mona_client.py` & `mona-openai-0.0.5/mona_openai/mona_client.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/mona_openai.py` & `mona-openai-0.0.5/mona_openai/mona_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -344,50 +344,45 @@
     Returns a client class for monitoring OpenAI REST calls not done
     using the OpenAI python client (e.g., for Azure users using their
     endpoints directly). This isn't a wrapper for any http requesting
     library and doesn't call the OpenAI API for you - it's just an easy
     logging client to log requests, responses and exceptions.
     """
 
-    # TODO(itai): Consider creating an async version as well.
-    client, _ = mona_clients_getter(mona_creds)
+    client, async_client = mona_clients_getter(mona_creds)
 
     sampling_ratio = validate_and_get_sampling_ratio(specs)
 
     wrapping_logic = get_endpoint_wrapping(openai_endpoint_name, specs)
 
     class RestClient:
         """
         This will be the returned Mona logging class. We follow
         OpenAI's way of doing things by using a static classe with
         relevant class methods.
         """
 
         @classmethod
-        def log_request(
+        def _inner_log_request(
             cls,
+            mona_export_function,
             request_dict,
             additional_data=None,
             context_id=None,
             export_timestamp=None,
         ):
             """
-            This function should be called with a request data dict,
-            for example, what you would use as "json" when using
-            "requests" to post.
-
-            It returns a response logging function to be used with the
-            response object.
+            Actual logic for logging requests, responses and exceptions.
             """
             start_time = time.time()
 
             inner_response = None
 
             def _inner_mona_export(is_exception):
-                return client.export(
+                return mona_export_function(
                     _get_mona_single_message(
                         api_name=openai_endpoint_name,
                         request_input=request_dict,
                         start_time=start_time,
                         is_exception=is_exception,
                         is_async=False,
                         # TODO(itai): Support stream in REST as well.
@@ -420,16 +415,66 @@
 
             def log_exception():
                 return mona_export(True)
 
             return log_response, log_exception
 
         @classmethod
-        def get_mona_client(cls):
+        def log_request(
+            cls,
+            request_dict,
+            additional_data=None,
+            context_id=None,
+            export_timestamp=None,
+        ):
+            """
+            Sets up mona logging for OpenAI request/response objects.
+
+            This function should be called with a request data dict,
+            for example, what you would use as "json" when using
+            "requests" to post.
+
+            It returns a response logging function to be used with the
+            response object, as well as an exception logging function in case
+            of exceptions.
+
+            Note that this call does not log anything to Mona until one of the
+            returned callbacks is called.
+            """
+            return cls._inner_log_request(
+                client.export,
+                request_dict,
+                additional_data,
+                context_id,
+                export_timestamp,
+            )
+
+        @classmethod
+        def async_log_request(
+            cls,
+            request_dict,
+            additional_data=None,
+            context_id=None,
+            export_timestamp=None,
+        ):
+            """
+            Async version of "log_request". See function's docstring for more
+            details.
+            """
+            return cls._inner_log_request(
+                async_client.export_async,
+                request_dict,
+                additional_data,
+                context_id,
+                export_timestamp,
+            )
+
+        @classmethod
+        def get_mona_clients(cls):
             """
             Returns the two Mona client this class works with to allow
             exporting more data or communicating directly with Mona's
             API.
             """
-            return client
+            return client, async_client
 
     return RestClient
```

### Comparing `mona-openai-0.0.4/mona_openai/util/async_util.py` & `mona-openai-0.0.5/mona_openai/util/async_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from inspect import iscoroutinefunction
 
 
 def run_in_an_event_loop(coroutine):
     """
     A light wrapper around asyncio.run to avoid crushing when trying to run a
     coroutine in an environment where an event loop is already in place and
-    async.run doesn't work.
+    asyncio.run doesn't work.
     """
     try:
         return asyncio.run(coroutine)
     except RuntimeError:
         return asyncio.get_event_loop().run_until_complete(coroutine)
```

### Comparing `mona-openai-0.0.4/mona_openai/util/func_util.py` & `mona-openai-0.0.5/mona_openai/util/func_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/util/oop_util.py` & `mona-openai-0.0.5/mona_openai/util/oop_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/util/stream_util.py` & `mona-openai-0.0.5/mona_openai/util/stream_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/util/tokens_util.py` & `mona-openai-0.0.5/mona_openai/util/tokens_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai/util/validation_util.py` & `mona-openai-0.0.5/mona_openai/util/validation_util.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/mona_openai.egg-info/PKG-INFO` & `mona-openai-0.0.5/mona_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-openai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integration client for monitoring OpenAI usage with Mona
 Author-email: Itai Bar Sinai <itai@monalabs.io>
 Project-URL: Homepage, https://github.com/monalabs/mona-openai
 Project-URL: Bug Tracker, https://github.com/monalabs/mona-openai/issues
 Keywords: OpenAI,LLMs,GPT,Mona,Monitoring,AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mona-openai-0.0.4/mona_openai.egg-info/SOURCES.txt` & `mona-openai-0.0.5/mona_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/pyproject.toml` & `mona-openai-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mona-openai"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Itai Bar Sinai", email="itai@monalabs.io" },
 ]
 description = "Integration client for monitoring OpenAI usage with Mona"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mona-openai-0.0.4/tests/test_chat_completion.py` & `mona-openai-0.0.5/tests/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/tests/test_completion.py` & `mona-openai-0.0.5/tests/test_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -227,14 +227,27 @@
         _DEFAULT_CONTEXT_CLASS,
         mona_clients_getter=get_mock_mona_clients_getter(
             (_get_mona_message(),), ()
         ),
     ).log_request(_DEFAULT_INPUT)[0](_DEFAULT_RESPONSE)
 
 
+def test_rest_async():
+    asyncio.run(
+        get_rest_monitor(
+            Completion.__name__,
+            (),
+            _DEFAULT_CONTEXT_CLASS,
+            mona_clients_getter=get_mock_mona_clients_getter(
+                (), (_get_mona_message(),)
+            ),
+        ).async_log_request(_DEFAULT_INPUT)[0](_DEFAULT_RESPONSE)
+    )
+
+
 def test_rest_exception():
     get_rest_monitor(
         Completion.__name__,
         (),
         _DEFAULT_CONTEXT_CLASS,
         mona_clients_getter=get_mock_mona_clients_getter(
             (
@@ -243,14 +256,32 @@
                 ),
             ),
             (),
         ),
     ).log_request(_DEFAULT_INPUT)[1]()
 
 
+def test_rest_exception_async():
+    asyncio.run(
+        get_rest_monitor(
+            Completion.__name__,
+            (),
+            _DEFAULT_CONTEXT_CLASS,
+            mona_clients_getter=get_mock_mona_clients_getter(
+                (),
+                (
+                    _get_mona_message(
+                        is_exception=True, response=None, analysis=None
+                    ),
+                ),
+            ),
+        ).async_log_request(_DEFAULT_INPUT)[1]()
+    )
+
+
 def test_export_response_text():
     monitor(
         _get_mock_openai_class((_DEFAULT_RESPONSE,), ()),
         (),
         _DEFAULT_CONTEXT_CLASS,
         {"export_response_texts": True},
         mona_clients_getter=get_mock_mona_clients_getter(
```

### Comparing `mona-openai-0.0.4/tests/test_privacy_analyzer.py` & `mona-openai-0.0.5/tests/test_privacy_analyzer.py`

 * *Files identical despite different names*

### Comparing `mona-openai-0.0.4/tests/test_textual_analyzer.py` & `mona-openai-0.0.5/tests/test_textual_analyzer.py`

 * *Files identical despite different names*

