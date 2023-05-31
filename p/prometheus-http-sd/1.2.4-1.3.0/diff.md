# Comparing `tmp/prometheus_http_sd-1.2.4.tar.gz` & `tmp/prometheus_http_sd-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_http_sd-1.2.4.tar", max compression
+gzip compressed data, was "prometheus_http_sd-1.3.0.tar", max compression
```

## Comparing `prometheus_http_sd-1.2.4.tar` & `prometheus_http_sd-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-05-29 01:19:14.063772 prometheus_http_sd-1.2.4/LICENSE
--rw-r--r--   0        0        0    11097 2023-05-29 01:19:14.063772 prometheus_http_sd-1.2.4/README.md
--rw-r--r--   0        0        0        0 2023-05-29 01:19:14.067772 prometheus_http_sd-1.2.4/prometheus_http_sd/__init__.py
--rw-r--r--   0        0        0     3774 2023-05-29 01:19:14.067772 prometheus_http_sd-1.2.4/prometheus_http_sd/app.py
--rw-r--r--   0        0        0     2398 2023-05-29 01:19:14.067772 prometheus_http_sd-1.2.4/prometheus_http_sd/cli.py
--rw-r--r--   0        0        0      110 2023-05-29 01:19:14.067772 prometheus_http_sd-1.2.4/prometheus_http_sd/config.py
--rw-r--r--   0        0        0       45 2023-05-29 01:19:14.067772 prometheus_http_sd-1.2.4/prometheus_http_sd/const.py
--rw-r--r--   0        0        0     7352 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/prometheus_http_sd/decorator.py
--rw-r--r--   0        0        0        0 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/prometheus_http_sd/exceptions.py
--rw-r--r--   0        0        0     1165 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/prometheus_http_sd/mem_perf.py
--rw-r--r--   0        0        0     5019 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/prometheus_http_sd/sd.py
--rw-r--r--   0        0        0      147 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/prometheus_http_sd/targets.py
--rw-r--r--   0        0        0     1148 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/prometheus_http_sd/templates/admin.html
--rw-r--r--   0        0        0     2118 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/prometheus_http_sd/validate.py
--rw-r--r--   0        0        0       18 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/prometheus_http_sd/version.py
--rw-r--r--   0        0        0      648 2023-05-29 01:19:14.071772 prometheus_http_sd-1.2.4/pyproject.toml
--rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 prometheus_http_sd-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 03:52:46.087086 prometheus_http_sd-1.3.0/LICENSE
+-rw-r--r--   0        0        0    11097 2023-05-31 03:52:46.087086 prometheus_http_sd-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/__init__.py
+-rw-r--r--   0        0        0     3774 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/app.py
+-rw-r--r--   0        0        0     2398 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/cli.py
+-rw-r--r--   0        0        0      110 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/config.py
+-rw-r--r--   0        0        0       45 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/const.py
+-rw-r--r--   0        0        0     7349 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/decorator.py
+-rw-r--r--   0        0        0        0 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/exceptions.py
+-rw-r--r--   0        0        0     1165 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/mem_perf.py
+-rw-r--r--   0        0        0     5019 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/sd.py
+-rw-r--r--   0        0        0      147 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/targets.py
+-rw-r--r--   0        0        0     1148 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/templates/admin.html
+-rw-r--r--   0        0        0     2118 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/validate.py
+-rw-r--r--   0        0        0       18 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/version.py
+-rw-r--r--   0        0        0      648 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 prometheus_http_sd-1.3.0/PKG-INFO
```

### Comparing `prometheus_http_sd-1.2.4/LICENSE` & `prometheus_http_sd-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.4/README.md` & `prometheus_http_sd-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.4/prometheus_http_sd/app.py` & `prometheus_http_sd-1.3.0/prometheus_http_sd/app.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.4/prometheus_http_sd/cli.py` & `prometheus_http_sd-1.3.0/prometheus_http_sd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.4/prometheus_http_sd/decorator.py` & `prometheus_http_sd-1.3.0/prometheus_http_sd/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 
 
 class WrapTargetException(Exception):
     """Raised when user's function raises an exception."""
 
     def __init__(self, message, exception_type="Exception", traceback=[]):
-        traceback = "\n".join(traceback)
+        traceback = "".join(traceback)
         super().__init__(
             self,
             f"""this is a cached exception,
 type: {exception_type}, message: {message}, traceback: {traceback}""",
         )
 
 
@@ -160,15 +160,15 @@
                 try:
                     cache["response"] = function(*arg, **kwargs)
                     cache["expired_timestamp"] = time.time() + self.cache_time
                 except Exception as e:
                     cache["error"] = {
                         "message": str(e),
                         "error_type": type(e).__name__,
-                        "traceback": traceback.extract_tb(e.__traceback__),
+                        "traceback": traceback.format_tb(e.__traceback__),
                     }
                     cache["expired_timestamp"] = 0
                 with self.heap_lock:
                     heapq.heappush(
                         self.heap,
                         (
                             cache["expired_timestamp"],
```

### Comparing `prometheus_http_sd-1.2.4/prometheus_http_sd/mem_perf.py` & `prometheus_http_sd-1.3.0/prometheus_http_sd/mem_perf.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.4/prometheus_http_sd/sd.py` & `prometheus_http_sd-1.3.0/prometheus_http_sd/sd.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.4/prometheus_http_sd/templates/admin.html` & `prometheus_http_sd-1.3.0/prometheus_http_sd/templates/admin.html`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.4/prometheus_http_sd/validate.py` & `prometheus_http_sd-1.3.0/prometheus_http_sd/validate.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.4/pyproject.toml` & `prometheus_http_sd-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-http-sd"
-version = "1.2.4"
+version = "1.3.0"
 description = "Prometheus HTTP SD framework."
 authors = ["laixintao <laixintaoo@gmail.com>"]
 readme = 'README.md'
 homepage = "https://python-poetry.org://github.com/laixintao/prometheus-http-sd"
 
 
 [tool.poetry.dependencies]
@@ -15,15 +15,15 @@
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 
 [build-system]
-requires = ["poetry-core>=1.2.4"]
+requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry.scripts]
 prometheus-http-sd = 'prometheus_http_sd.cli:main'
```

### Comparing `prometheus_http_sd-1.2.4/PKG-INFO` & `prometheus_http_sd-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-http-sd
-Version: 1.2.4
+Version: 1.3.0
 Summary: Prometheus HTTP SD framework.
 Home-page: https://python-poetry.org://github.com/laixintao/prometheus-http-sd
 Author: laixintao
 Author-email: laixintaoo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

