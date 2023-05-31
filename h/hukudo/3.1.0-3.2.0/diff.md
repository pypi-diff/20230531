# Comparing `tmp/hukudo-3.1.0.tar.gz` & `tmp/hukudo-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hukudo-3.1.0.tar", last modified: Mon Mar 13 13:12:06 2023, max compression
+gzip compressed data, was "hukudo-3.2.0.tar", last modified: Wed May 31 11:55:43 2023, max compression
```

## Comparing `hukudo-3.1.0.tar` & `hukudo-3.2.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-03-13 13:12:06.135760 hukudo-3.1.0/
--rw-rw-r--   0 felix     (1337) felix     (1337)     1077 2022-04-05 09:56:29.000000 hukudo-3.1.0/LICENSE
--rw-rw-r--   0 felix     (1337) felix     (1337)     1300 2023-03-13 13:12:06.135760 hukudo-3.1.0/PKG-INFO
--rw-rw-r--   0 felix     (1337) felix     (1337)      890 2022-09-08 11:45:30.000000 hukudo-3.1.0/README.md
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-03-13 13:12:06.131760 hukudo-3.1.0/hukudo/
--rw-rw-r--   0 felix     (1337) felix     (1337)       22 2023-03-13 13:12:05.000000 hukudo-3.1.0/hukudo/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     5305 2023-03-13 12:19:59.000000 hukudo-3.1.0/hukudo/chromedriver.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2235 2022-09-09 10:11:07.000000 hukudo-3.1.0/hukudo/cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)       43 2022-06-07 10:45:57.000000 hukudo-3.1.0/hukudo/exc.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      636 2022-09-08 11:32:36.000000 hukudo-3.1.0/hukudo/filesystem.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-03-13 13:12:06.131760 hukudo-3.1.0/hukudo/gitlab/
--rw-rw-r--   0 felix     (1337) felix     (1337)        0 2022-07-20 19:31:40.000000 hukudo-3.1.0/hukudo/gitlab/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      745 2022-07-20 19:31:40.000000 hukudo-3.1.0/hukudo/gitlab/api.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      723 2022-07-20 19:31:40.000000 hukudo-3.1.0/hukudo/gitlab/cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      430 2022-07-20 19:31:40.000000 hukudo-3.1.0/hukudo/gitlab/jobs.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-03-13 13:12:06.135760 hukudo-3.1.0/hukudo/grafana/
--rw-rw-r--   0 felix     (1337) felix     (1337)       55 2022-03-10 15:35:16.000000 hukudo-3.1.0/hukudo/grafana/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     3618 2022-06-08 15:03:51.000000 hukudo-3.1.0/hukudo/grafana/api.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2564 2022-06-08 15:07:33.000000 hukudo-3.1.0/hukudo/grafana/cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      263 2022-06-07 15:19:07.000000 hukudo-3.1.0/hukudo/grafana/demo.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      141 2022-06-08 10:23:35.000000 hukudo-3.1.0/hukudo/grafana/errors.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      647 2022-06-08 15:07:18.000000 hukudo-3.1.0/hukudo/grafana/models.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     1076 2022-06-08 11:13:22.000000 hukudo-3.1.0/hukudo/log.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-03-13 13:12:06.135760 hukudo-3.1.0/hukudo/pypi/
--rw-rw-r--   0 felix     (1337) felix     (1337)      384 2022-09-09 10:11:07.000000 hukudo-3.1.0/hukudo/pypi/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      187 2022-09-09 10:12:16.000000 hukudo-3.1.0/hukudo/pypi/cli.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-03-13 13:12:06.135760 hukudo-3.1.0/hukudo/xls/
--rw-rw-r--   0 felix     (1337) felix     (1337)        0 2021-11-03 14:53:39.000000 hukudo-3.1.0/hukudo/xls/__init__.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2392 2021-11-03 18:22:13.000000 hukudo-3.1.0/hukudo/xls/edi.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     2417 2021-12-01 09:56:40.000000 hukudo-3.1.0/hukudo/xls/fmt.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     4846 2023-03-13 13:11:33.000000 hukudo-3.1.0/hukudo/xls/sheet.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     1993 2023-03-13 12:43:16.000000 hukudo-3.1.0/hukudo/xls/table.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-03-13 13:12:06.131760 hukudo-3.1.0/hukudo.egg-info/
--rw-rw-r--   0 felix     (1337) felix     (1337)     1300 2023-03-13 13:12:06.000000 hukudo-3.1.0/hukudo.egg-info/PKG-INFO
--rw-rw-r--   0 felix     (1337) felix     (1337)      899 2023-03-13 13:12:06.000000 hukudo-3.1.0/hukudo.egg-info/SOURCES.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)        1 2023-03-13 13:12:06.000000 hukudo-3.1.0/hukudo.egg-info/dependency_links.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)       44 2023-03-13 13:12:06.000000 hukudo-3.1.0/hukudo.egg-info/entry_points.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)      543 2023-03-13 13:12:06.000000 hukudo-3.1.0/hukudo.egg-info/requires.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)        7 2023-03-13 13:12:06.000000 hukudo-3.1.0/hukudo.egg-info/top_level.txt
--rw-rw-r--   0 felix     (1337) felix     (1337)      386 2023-03-13 12:33:26.000000 hukudo-3.1.0/pyproject.toml
--rw-rw-r--   0 felix     (1337) felix     (1337)      753 2023-03-13 13:12:06.135760 hukudo-3.1.0/setup.cfg
--rw-rw-r--   0 felix     (1337) felix     (1337)      348 2023-03-13 12:33:26.000000 hukudo-3.1.0/setup.py
-drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-03-13 13:12:06.135760 hukudo-3.1.0/tests/
--rw-rw-r--   0 felix     (1337) felix     (1337)     2833 2022-06-08 16:07:14.000000 hukudo-3.1.0/tests/test_chromedriver.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      305 2022-06-08 13:34:36.000000 hukudo-3.1.0/tests/test_cli.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      613 2022-07-20 19:31:40.000000 hukudo-3.1.0/tests/test_gitlab.py
--rw-rw-r--   0 felix     (1337) felix     (1337)     5455 2022-10-26 12:58:40.000000 hukudo-3.1.0/tests/test_grafana.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      666 2022-09-08 11:39:19.000000 hukudo-3.1.0/tests/test_keepn.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      144 2022-06-08 15:28:39.000000 hukudo-3.1.0/tests/test_log.py
--rw-rw-r--   0 felix     (1337) felix     (1337)       80 2022-06-08 10:38:01.000000 hukudo-3.1.0/tests/test_pypi.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      436 2021-11-03 14:53:39.000000 hukudo-3.1.0/tests/test_xls.py
--rw-rw-r--   0 felix     (1337) felix     (1337)      240 2023-03-13 12:49:04.000000 hukudo-3.1.0/tests/test_xls_edi.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.190870 hukudo-3.2.0/
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1077 2022-04-05 09:56:29.000000 hukudo-3.2.0/LICENSE
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1246 2023-05-31 11:55:43.190870 hukudo-3.2.0/PKG-INFO
+-rw-rw-r--   0 felix     (1337) felix     (1337)      890 2022-09-08 11:45:30.000000 hukudo-3.2.0/README.md
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.182870 hukudo-3.2.0/hukudo/
+-rw-rw-r--   0 felix     (1337) felix     (1337)       22 2023-05-31 11:55:42.000000 hukudo-3.2.0/hukudo/__init__.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     5305 2023-03-13 12:19:59.000000 hukudo-3.2.0/hukudo/chromedriver.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     2235 2022-09-09 10:11:07.000000 hukudo-3.2.0/hukudo/cli.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)       43 2022-06-07 10:45:57.000000 hukudo-3.2.0/hukudo/exc.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      636 2022-09-08 11:32:36.000000 hukudo-3.2.0/hukudo/filesystem.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.186870 hukudo-3.2.0/hukudo/gitlab/
+-rw-rw-r--   0 felix     (1337) felix     (1337)        0 2022-07-20 19:31:40.000000 hukudo-3.2.0/hukudo/gitlab/__init__.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      745 2022-07-20 19:31:40.000000 hukudo-3.2.0/hukudo/gitlab/api.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      723 2022-07-20 19:31:40.000000 hukudo-3.2.0/hukudo/gitlab/cli.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      430 2022-07-20 19:31:40.000000 hukudo-3.2.0/hukudo/gitlab/jobs.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.186870 hukudo-3.2.0/hukudo/grafana/
+-rw-rw-r--   0 felix     (1337) felix     (1337)       55 2022-03-10 15:35:16.000000 hukudo-3.2.0/hukudo/grafana/__init__.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     3652 2023-05-31 11:31:40.000000 hukudo-3.2.0/hukudo/grafana/api.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     2981 2023-05-31 11:40:08.000000 hukudo-3.2.0/hukudo/grafana/cli.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      263 2022-06-07 15:19:07.000000 hukudo-3.2.0/hukudo/grafana/demo.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      141 2022-06-08 10:23:35.000000 hukudo-3.2.0/hukudo/grafana/errors.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      647 2022-06-08 15:07:18.000000 hukudo-3.2.0/hukudo/grafana/models.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1076 2022-06-08 11:13:22.000000 hukudo-3.2.0/hukudo/log.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.186870 hukudo-3.2.0/hukudo/pypi/
+-rw-rw-r--   0 felix     (1337) felix     (1337)      384 2022-09-09 10:11:07.000000 hukudo-3.2.0/hukudo/pypi/__init__.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      187 2022-09-09 10:12:16.000000 hukudo-3.2.0/hukudo/pypi/cli.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.186870 hukudo-3.2.0/hukudo/xls/
+-rw-rw-r--   0 felix     (1337) felix     (1337)       38 2023-04-13 15:49:31.000000 hukudo-3.2.0/hukudo/xls/__init__.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     2392 2021-11-03 18:22:13.000000 hukudo-3.2.0/hukudo/xls/edi.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     2417 2021-12-01 09:56:40.000000 hukudo-3.2.0/hukudo/xls/fmt.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     4839 2023-04-13 15:56:59.000000 hukudo-3.2.0/hukudo/xls/sheet.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     2029 2023-04-13 15:49:32.000000 hukudo-3.2.0/hukudo/xls/table.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.182870 hukudo-3.2.0/hukudo.egg-info/
+-rw-rw-r--   0 felix     (1337) felix     (1337)     1246 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1337) felix     (1337)      923 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)        1 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)       43 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/entry_points.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)      533 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)        7 2023-05-31 11:55:43.000000 hukudo-3.2.0/hukudo.egg-info/top_level.txt
+-rw-rw-r--   0 felix     (1337) felix     (1337)      386 2023-03-13 12:33:26.000000 hukudo-3.2.0/pyproject.toml
+-rw-rw-r--   0 felix     (1337) felix     (1337)      753 2023-05-31 11:55:43.190870 hukudo-3.2.0/setup.cfg
+-rw-rw-r--   0 felix     (1337) felix     (1337)      348 2023-03-13 12:33:26.000000 hukudo-3.2.0/setup.py
+drwxrwxr-x   0 felix     (1337) felix     (1337)        0 2023-05-31 11:55:43.190870 hukudo-3.2.0/tests/
+-rw-rw-r--   0 felix     (1337) felix     (1337)     2833 2022-06-08 16:07:14.000000 hukudo-3.2.0/tests/test_chromedriver.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      305 2022-06-08 13:34:36.000000 hukudo-3.2.0/tests/test_cli.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      613 2022-07-20 19:31:40.000000 hukudo-3.2.0/tests/test_gitlab.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)     5455 2022-10-26 12:58:40.000000 hukudo-3.2.0/tests/test_grafana.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      666 2022-09-08 11:39:19.000000 hukudo-3.2.0/tests/test_keepn.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      144 2022-06-08 15:28:39.000000 hukudo-3.2.0/tests/test_log.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)       80 2022-06-08 10:38:01.000000 hukudo-3.2.0/tests/test_pypi.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      436 2021-11-03 14:53:39.000000 hukudo-3.2.0/tests/test_xls.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      127 2023-04-13 15:51:20.000000 hukudo-3.2.0/tests/test_xls_edi.py
+-rw-rw-r--   0 felix     (1337) felix     (1337)      717 2023-04-13 16:24:52.000000 hukudo-3.2.0/tests/test_xls_sheet.py
```

### Comparing `hukudo-3.1.0/LICENSE` & `hukudo-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/PKG-INFO` & `hukudo-3.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: hukudo
-Version: 3.1.0
-Summary: UNKNOWN
+Version: 3.2.0
 Home-page: https://gitlab.com/hukudo/lib/
 Author: hukudo GmbH
 Author-email: python@hukudo.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: pypi
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: xls
@@ -58,9 +55,7 @@
 ```
 make
 ```
 
 
 # Development
 See [1-docs/development.md]
-
-
```

### Comparing `hukudo-3.1.0/README.md` & `hukudo-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/chromedriver.py` & `hukudo-3.2.0/hukudo/chromedriver.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/cli.py` & `hukudo-3.2.0/hukudo/cli.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/filesystem.py` & `hukudo-3.2.0/hukudo/filesystem.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/gitlab/api.py` & `hukudo-3.2.0/hukudo/gitlab/api.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/gitlab/cli.py` & `hukudo-3.2.0/hukudo/gitlab/cli.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/grafana/api.py` & `hukudo-3.2.0/hukudo/grafana/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,19 @@
             http2=True,
             verify=verify,
             cert=cert,
         )
         return cls(client)
 
     @classmethod
-    def from_api_key(cls, url, api_key, verify=None, cert=None):
+    def from_api_key(cls, url, api_key, verify=None, cert=None, auth=None):
         client = httpx.Client(
             base_url=url,
             headers=cls.bearer_header(api_key),
+            auth=auth,
             http2=True,
             verify=verify,
             cert=cert,
         )
         return cls(client)
 
     def __init__(self, client: httpx.Client):
```

### Comparing `hukudo-3.1.0/hukudo/grafana/cli.py` & `hukudo-3.2.0/hukudo/grafana/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,32 +19,45 @@
     if config:
         logger.debug('dotenv override', config=config)
         os.environ.update(dotenv.dotenv_values(config))
     # get stuff from env
     try:
         url = os.environ['GRAFANA_URL']
         api_key = os.environ['GRAFANA_API_KEY']
-        root_ca = os.environ.get('GRAFANA_CLIENT_ROOT_CA')
     except KeyError as e:
         raise click.ClickException(f'missing environment variable {e}')
+    root_ca = os.environ.get('GRAFANA_CLIENT_ROOT_CA')
     logger.debug('CA', path=root_ca)
+
     client_cert = None
     try:
+        logger.debug('read config', what='client_cert')
         crt = os.environ['GRAFANA_CLIENT_CRT']
         key = os.environ['GRAFANA_CLIENT_KEY']
         logger.debug('client cert', crt=crt, key=key)
         client_cert = (crt, key)
     except KeyError:
         pass
 
+    basic_auth = None
+    try:
+        logger.debug('read config', what='basic_auth')
+        username = os.environ['GRAFANA_BASIC_AUTH_USERNAME']
+        password = os.environ['GRAFANA_BASIC_AUTH_PASSWORD']
+        logger.debug('basic_auth', username=username)
+        basic_auth = (username, password)
+    except KeyError:
+        pass
+
     ctx.obj = Grafana.from_api_key(
         url=url,
         api_key=api_key,
         verify=root_ca,
         cert=client_cert,
+        auth=basic_auth,
     )
     log = logger.bind(instance=ctx.obj)
     log.debug('instantiated')
 
 
 @grafana.command()
 @click.pass_context
```

### Comparing `hukudo-3.1.0/hukudo/grafana/models.py` & `hukudo-3.2.0/hukudo/grafana/models.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/log.py` & `hukudo-3.2.0/hukudo/log.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/xls/edi.py` & `hukudo-3.2.0/hukudo/xls/edi.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/xls/fmt.py` & `hukudo-3.2.0/hukudo/xls/fmt.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/hukudo/xls/sheet.py` & `hukudo-3.2.0/hukudo/xls/sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             self.ws[value_edi].number_format = self.fmts.get(key, fmt.FMT_GENERAL)
             self.ws[value_edi].alignment = fmt.align_left
             # merge cells
             self.ws.merge_cells(value_edi.get_range_col_offset(merge_cols))
         return start.row_offset(len(d))
 
     def add_table_with_header(
-        self, start: EDISTR, header: str, table: Table, style: str = None, end_col='J', fmts: dict = None
+        self, start: EDISTR, header: str, table: Table, style: str, end_col='J', fmts: dict = None
     ):
         start = EDI(start)
         self.ws[start] = header
         self.style_row(start, style, end_col)
         return self.add_table(start.row_offset(1), table, fmts=fmts)
 
     # noinspection DuplicatedCode
```

### Comparing `hukudo-3.1.0/hukudo/xls/table.py` & `hukudo-3.2.0/hukudo/xls/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from hukudo.xls import TableError
+
 log = logging.getLogger(__name__)
 
 
 class Table:
     def __init__(self, header: list, data: list[list]):
         self.header = header
         self.data = data
@@ -19,15 +21,15 @@
         for d in self.data:
             result.append({k: v for (k, v) in zip(self.header, d)})
         return result
 
     def single_dict(self):
         dicts = self.dicts()
         if len(dicts) != 1:
-            raise Exception('More than one result found. Please fix your query to return exactly one row.')
+            raise TableError('More than one result found. Please fix your query to return exactly one row.')
         return dicts[0]
 
     def change_columns(self, mapping: dict = None, capitalize=True):
         """
         Siehe test case.
         """
         if mapping is None:
```

### Comparing `hukudo-3.1.0/hukudo.egg-info/PKG-INFO` & `hukudo-3.2.0/hukudo.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: hukudo
-Version: 3.1.0
-Summary: UNKNOWN
+Version: 3.2.0
 Home-page: https://gitlab.com/hukudo/lib/
 Author: hukudo GmbH
 Author-email: python@hukudo.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: pypi
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: xls
@@ -58,9 +55,7 @@
 ```
 make
 ```
 
 
 # Development
 See [1-docs/development.md]
-
-
```

### Comparing `hukudo-3.1.0/hukudo.egg-info/SOURCES.txt` & `hukudo-3.2.0/hukudo.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 tests/test_cli.py
 tests/test_gitlab.py
 tests/test_grafana.py
 tests/test_keepn.py
 tests/test_log.py
 tests/test_pypi.py
 tests/test_xls.py
-tests/test_xls_edi.py
+tests/test_xls_edi.py
+tests/test_xls_sheet.py
```

### Comparing `hukudo-3.1.0/hukudo.egg-info/requires.txt` & `hukudo-3.2.0/hukudo.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 pip-tools
 pytest-cov
 pytest-mock
 pytest-xdist
 requests_cache
 twine
 glob2
-pip-tools
 sphinx-reload
 ablog
 linkify-it-py
 myst_parser
 pydata_sphinx_theme
 sphinx
 pypi-simple
```

### Comparing `hukudo-3.1.0/setup.cfg` & `hukudo-3.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hukudo
-version = 3.1.0
+version = 3.2.0
 url = https://gitlab.com/hukudo/lib/
 author = hukudo GmbH
 author_email = python@hukudo.de
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
```

### Comparing `hukudo-3.1.0/tests/test_chromedriver.py` & `hukudo-3.2.0/tests/test_chromedriver.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/tests/test_gitlab.py` & `hukudo-3.2.0/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/tests/test_grafana.py` & `hukudo-3.2.0/tests/test_grafana.py`

 * *Files identical despite different names*

### Comparing `hukudo-3.1.0/tests/test_keepn.py` & `hukudo-3.2.0/tests/test_keepn.py`

 * *Files identical despite different names*

