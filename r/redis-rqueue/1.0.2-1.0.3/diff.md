# Comparing `tmp/redis-rqueue-1.0.2.tar.gz` & `tmp/redis-rqueue-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-rqueue-1.0.2.tar", last modified: Fri May 26 17:39:22 2023, max compression
+gzip compressed data, was "redis-rqueue-1.0.3.tar", last modified: Wed May 31 20:59:47 2023, max compression
```

## Comparing `redis-rqueue-1.0.2.tar` & `redis-rqueue-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-26 17:39:22.891910 redis-rqueue-1.0.2/
--rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-26 17:39:22.891735 redis-rqueue-1.0.2/PKG-INFO
--rw-r--r--   0 vitor      (501) staff       (20)       15 2023-05-26 17:37:27.000000 redis-rqueue-1.0.2/README.md
--rw-r--r--   0 vitor      (501) staff       (20)      263 2023-05-26 17:38:11.000000 redis-rqueue-1.0.2/pyproject.toml
--rw-r--r--   0 vitor      (501) staff       (20)       12 2023-05-26 17:38:02.000000 redis-rqueue-1.0.2/requirements.txt
--rw-r--r--   0 vitor      (501) staff       (20)       38 2023-05-26 17:39:22.891954 redis-rqueue-1.0.2/setup.cfg
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-26 17:39:22.889653 redis-rqueue-1.0.2/src/
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-26 17:39:22.890816 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/
--rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/PKG-INFO
--rw-r--r--   0 vitor      (501) staff       (20)      292 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/SOURCES.txt
--rw-r--r--   0 vitor      (501) staff       (20)        1 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/dependency_links.txt
--rw-r--r--   0 vitor      (501) staff       (20)       13 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/requires.txt
--rw-r--r--   0 vitor      (501) staff       (20)        7 2023-05-26 17:39:22.000000 redis-rqueue-1.0.2/src/redis_rqueue.egg-info/top_level.txt
-drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-26 17:39:22.891206 redis-rqueue-1.0.2/src/rqueue/
--rw-r--r--   0 vitor      (501) staff       (20)       67 2023-05-26 17:37:27.000000 redis-rqueue-1.0.2/src/rqueue/__init__.py
--rw-r--r--   0 vitor      (501) staff       (20)     3490 2023-05-26 17:37:27.000000 redis-rqueue-1.0.2/src/rqueue/queue_executor.py
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-31 20:59:47.719422 redis-rqueue-1.0.3/
+-rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-31 20:59:47.719276 redis-rqueue-1.0.3/PKG-INFO
+-rw-r--r--   0 vitor      (501) staff       (20)       15 2023-05-31 20:20:24.000000 redis-rqueue-1.0.3/README.md
+-rw-r--r--   0 vitor      (501) staff       (20)      263 2023-05-31 20:59:22.000000 redis-rqueue-1.0.3/pyproject.toml
+-rw-r--r--   0 vitor      (501) staff       (20)       12 2023-05-31 20:20:24.000000 redis-rqueue-1.0.3/requirements.txt
+-rw-r--r--   0 vitor      (501) staff       (20)       38 2023-05-31 20:59:47.719462 redis-rqueue-1.0.3/setup.cfg
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-31 20:59:47.717206 redis-rqueue-1.0.3/src/
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-31 20:59:47.718482 redis-rqueue-1.0.3/src/redis_rqueue.egg-info/
+-rw-r--r--   0 vitor      (501) staff       (20)       79 2023-05-31 20:59:47.000000 redis-rqueue-1.0.3/src/redis_rqueue.egg-info/PKG-INFO
+-rw-r--r--   0 vitor      (501) staff       (20)      292 2023-05-31 20:59:47.000000 redis-rqueue-1.0.3/src/redis_rqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 vitor      (501) staff       (20)        1 2023-05-31 20:59:47.000000 redis-rqueue-1.0.3/src/redis_rqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 vitor      (501) staff       (20)       13 2023-05-31 20:59:47.000000 redis-rqueue-1.0.3/src/redis_rqueue.egg-info/requires.txt
+-rw-r--r--   0 vitor      (501) staff       (20)        7 2023-05-31 20:59:47.000000 redis-rqueue-1.0.3/src/redis_rqueue.egg-info/top_level.txt
+drwxr-xr-x   0 vitor      (501) staff       (20)        0 2023-05-31 20:59:47.718949 redis-rqueue-1.0.3/src/rqueue/
+-rw-r--r--   0 vitor      (501) staff       (20)       67 2023-05-31 20:20:24.000000 redis-rqueue-1.0.3/src/rqueue/__init__.py
+-rw-r--r--   0 vitor      (501) staff       (20)     3706 2023-05-31 20:57:24.000000 redis-rqueue-1.0.3/src/rqueue/queue_executor.py
```

### Comparing `redis-rqueue-1.0.2/src/rqueue/queue_executor.py` & `redis-rqueue-1.0.3/src/rqueue/queue_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,26 +20,28 @@
         user_function: Callable[[str], None],
         function_timeout: int,
         queue: str,
         doing_queue: str,
         success_queue: str,
         error_queue: str,
         maximum_attempts: int,
-        sleep_time: int
+        sleep_time: int,
+        execute_on_error: Callable[[str], None] = None
     ) -> None:
 
         self.redis_client = redis_client
         self.user_function = user_function
         self.function_timeout = function_timeout
         self.queue = queue
         self.doing_queue = doing_queue
         self.success_queue = success_queue
         self.error_queue = error_queue
         self.maximum_attempts = maximum_attempts
         self.sleep_time = sleep_time
+        self.execute_on_error = execute_on_error
 
         self.redis_client.connection_pool.connection_kwargs['decode_responses'] = True
         self.redis_client.ping()
 
         self.attempt = 1
         self.current_queue = queue
 
@@ -58,14 +60,16 @@
                     self.redis_client.lrem(self.doing_queue, 0, parameter)
                     self.redis_client.rpush(self.success_queue, parameter)
                     logging.info(
                         f'User function successfully executed with parameter "{parameter}" (attempt {self.attempt}).')
                 except Exception as e:
                     self.redis_client.lrem(self.doing_queue, 0, parameter)
                     if self.attempt >= self.maximum_attempts:
+                        if self.execute_on_error:
+                            self.execute_on_error(parameter)
                         self.redis_client.rpush(self.error_queue, parameter)
                     else:
                         self.redis_client.rpush(
                             f'{self.queue}:attempt:{self.attempt + 1}', parameter)
                     logging.error(
                         f'Failed to execute user function with parameter "{parameter}" (attempt {self.attempt}). {e}')
                 finally:
```

