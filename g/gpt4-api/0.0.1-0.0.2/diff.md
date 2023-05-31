# Comparing `tmp/gpt4-api-0.0.1.tar.gz` & `tmp/gpt4-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.0.1.tar", last modified: Tue May 30 06:58:17 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.0.2.tar", last modified: Wed May 31 05:30:30 2023, max compression
```

## Comparing `gpt4-api-0.0.1.tar` & `gpt4-api-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-05-30 06:58:17.000000 gpt4-api-0.0.1/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-05-30 06:58:17.000000 gpt4-api-0.0.1/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-05-30 06:58:17.000000 gpt4-api-0.0.1/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.0.1/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     9610 2023-05-30 06:53:24.000000 gpt4-api-0.0.1/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-05-30 06:58:17.000000 gpt4-api-0.0.1/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-05-30 06:58:16.000000 gpt4-api-0.0.1/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-05-30 06:58:16.000000 gpt4-api-0.0.1/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-05-30 06:58:16.000000 gpt4-api-0.0.1/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-05-30 06:58:16.000000 gpt4-api-0.0.1/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-05-30 06:58:16.000000 gpt4-api-0.0.1/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-05-30 06:58:17.000000 gpt4-api-0.0.1/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.0.1/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.0.2/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     9790 2023-05-31 05:29:54.000000 gpt4-api-0.0.2/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      194 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-05-31 05:30:30.000000 gpt4-api-0.0.2/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.0.2/setup.py
```

### Comparing `gpt4-api-0.0.1/api/gpt.py` & `gpt4-api-0.0.2/api/gpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,16 @@
     @staticmethod
     def __get_active_thread_count():
         return threading.active_count() - 1
 
     def process_task(self, task, ask_content, messages, retries=1, retry=False):
         open_ai_key = self.__get_key()
         if open_ai_key:
+            case_name = task.get("case", None)
+            logging.info("case run: %s" % case_name)
             if len(messages) == 0 and self.system_content:
                 messages.append({"role": "system", "content": self.system_content})
             if not retry:
                 messages.append({"role": "user", "content": ask_content})
             try:
                 start_time = time.time()
                 response = openai.ChatCompletion.create(
@@ -128,35 +130,35 @@
                 )
                 elapsed_time = time.time() - start_time
                 response_str = response['choices'][0]['message']['content']
                 messages.append({"role": response['choices'][0]['message']['role'], "content": response_str})
                 completion_tokens = response['usage']['completion_tokens']
                 prompt_tokens = response['usage']['prompt_tokens']
                 total_tokens = response['usage']['total_tokens']
-                logging.info("request cost time: %s second" % int(elapsed_time))
+                logging.info("request case %s cost time: %s second" % (case_name, int(elapsed_time)))
                 logging.info("prompt tokens: %s" % prompt_tokens)
                 logging.info("completion tokens: %s" % completion_tokens)
                 logging.info("total tokens: %s" % total_tokens)
                 for openaiKey in self.usable_openai_keys:
                     if openaiKey.get("api_key", None) == open_ai_key:
                         openaiKey["token_limit"] += total_tokens
                 logging.info("active threads: %s" % self.__get_active_thread_count())
-                self.call_black(response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens)
+                self.call_black(response_str, messages, elapsed_time, completion_tokens, prompt_tokens, total_tokens, case_name)
             except openai.error.RateLimitError as e:
-                logging.error(f"Retrying: {retries}, OpenAI API request exceeded rate limit: {e} api_key: {open_ai_key}")
+                logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request exceeded rate limit: {e} api_key: {open_ai_key}")
                 self.__release_token(open_ai_key)
                 self.retry_on_error(task, ask_content, messages, retries=retries)
             except openai.error.Timeout as e:
-                logging.error(f"Retrying: {retries}, OpenAI API request timed out: {e} ")
+                logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request timed out: {e} ")
                 self.retry_on_error(task, ask_content, messages, retries=retries)
             except openai.error.APIConnectionError as e:
-                logging.error(f"Retrying: {retries}, OpenAI API request timed out, OpenAI API request failed to connect: {e}")
+                logging.error(f"Retrying: {case_name}/{retries}, OpenAI API request timed out, OpenAI API request failed to connect: {e}")
                 self.retry_on_error(task, ask_content, messages, retries=retries)
             except openai.error.APIError as e:
-                logging.error(f"Retrying: {retries}, OpenAI API returned an API Error: {e}")
+                logging.error(f"Retrying: {case_name}/{retries}, OpenAI API returned an API Error: {e}")
                 self.retry_on_error(task, ask_content, messages, retries=retries)
         else:
             self.task_queue.put(task)
 
     def run_tasks(self, tasks):
         self._run_tasks(tasks=tasks, run_func=self.process_task)
```

### Comparing `gpt4-api-0.0.1/setup.py` & `gpt4-api-0.0.2/setup.py`

 * *Files identical despite different names*

