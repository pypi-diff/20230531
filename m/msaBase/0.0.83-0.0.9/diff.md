# Comparing `tmp/msaBase-0.0.83.tar.gz` & `tmp/msaBase-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msaBase-0.0.83.tar", last modified: Wed May 31 09:47:37 2023, max compression
+gzip compressed data, was "msaBase-0.0.9.tar", last modified: Thu Nov 24 17:12:13 2022, max compression
```

## Comparing `msaBase-0.0.83.tar` & `msaBase-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-31 09:47:37.756284 msaBase-0.0.83/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1094 2023-03-26 10:37:44.000000 msaBase-0.0.83/LICENCE
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       58 2023-03-26 10:37:44.000000 msaBase-0.0.83/MANIFEST.in
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     4135 2023-05-31 09:47:37.756284 msaBase-0.0.83/PKG-INFO
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2689 2023-03-26 10:37:44.000000 msaBase-0.0.83/README.md
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-31 09:47:37.756284 msaBase-0.0.83/msaBase/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      472 2023-05-29 11:30:49.000000 msaBase-0.0.83/msaBase/__init__.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     8182 2023-05-31 07:36:42.000000 msaBase-0.0.83/msaBase/config.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    38074 2023-05-31 08:54:39.000000 msaBase-0.0.83/msaBase/configurate.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2116 2023-04-21 08:06:10.000000 msaBase-0.0.83/msaBase/errorhandling.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2476 2023-05-29 12:22:21.000000 msaBase-0.0.83/msaBase/healthcheck.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2930 2023-05-31 08:30:19.000000 msaBase-0.0.83/msaBase/helpers.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     3720 2023-04-21 08:06:10.000000 msaBase-0.0.83/msaBase/logger.py
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-31 09:47:37.756284 msaBase-0.0.83/msaBase/models/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      211 2023-04-21 08:06:10.000000 msaBase-0.0.83/msaBase/models/__init__.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      948 2023-04-04 06:43:14.000000 msaBase-0.0.83/msaBase/models/functionality.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1414 2023-03-26 10:37:44.000000 msaBase-0.0.83/msaBase/models/middlewares.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      381 2023-03-26 10:37:44.000000 msaBase-0.0.83/msaBase/models/settings.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    14964 2023-05-01 07:24:39.000000 msaBase-0.0.83/msaBase/models/sysinfo.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     4785 2023-05-11 16:54:40.000000 msaBase-0.0.83/msaBase/profiler.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)    14841 2023-05-11 16:54:40.000000 msaBase-0.0.83/msaBase/sysinfo.py
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-31 09:47:37.756284 msaBase-0.0.83/msaBase/utils/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        0 2023-03-26 10:37:44.000000 msaBase-0.0.83/msaBase/utils/__init__.py
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      338 2023-05-31 07:36:42.000000 msaBase-0.0.83/msaBase/utils/constants.py
-drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-05-31 09:47:37.756284 msaBase-0.0.83/msaBase.egg-info/
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     4135 2023-05-31 09:47:37.000000 msaBase-0.0.83/msaBase.egg-info/PKG-INFO
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      615 2023-05-31 09:47:37.000000 msaBase-0.0.83/msaBase.egg-info/SOURCES.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        1 2023-05-31 09:47:37.000000 msaBase-0.0.83/msaBase.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      808 2023-05-31 09:47:37.000000 msaBase-0.0.83/msaBase.egg-info/requires.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        8 2023-05-31 09:47:37.000000 msaBase-0.0.83/msaBase.egg-info/top_level.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        1 2023-03-31 07:37:42.000000 msaBase-0.0.83/msaBase.egg-info/zip-safe
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     3878 2023-05-29 14:36:05.000000 msaBase-0.0.83/requirements.txt
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       38 2023-05-31 09:47:37.756284 msaBase-0.0.83/setup.cfg
--rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2312 2023-04-21 08:06:10.000000 msaBase-0.0.83/setup.py
+drwxrwxr-x   0 cornhub   (1000) cornhub   (1000)        0 2022-11-24 17:12:13.607689 msaBase-0.0.9/
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     1094 2022-11-22 10:10:58.000000 msaBase-0.0.9/LICENCE
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)       58 2022-11-22 10:10:58.000000 msaBase-0.0.9/MANIFEST.in
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     4154 2022-11-24 17:12:13.607689 msaBase-0.0.9/PKG-INFO
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     2689 2022-11-22 10:10:58.000000 msaBase-0.0.9/README.md
+drwxrwxr-x   0 cornhub   (1000) cornhub   (1000)        0 2022-11-24 17:12:13.607689 msaBase-0.0.9/msaBase/
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)      477 2022-11-24 16:54:20.000000 msaBase-0.0.9/msaBase/__init__.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     6982 2022-11-24 15:50:02.000000 msaBase-0.0.9/msaBase/config.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)    31229 2022-11-24 16:53:20.000000 msaBase-0.0.9/msaBase/configurate.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     2128 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/errorhandling.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     2171 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/healthcheck.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)      676 2022-11-24 17:03:51.000000 msaBase-0.0.9/msaBase/helpers.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     3656 2022-11-24 15:49:31.000000 msaBase-0.0.9/msaBase/logger.py
+drwxrwxr-x   0 cornhub   (1000) cornhub   (1000)        0 2022-11-24 17:12:13.607689 msaBase-0.0.9/msaBase/models/
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)      217 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/models/__init__.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)      951 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/models/functionality.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     1182 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/models/middlewares.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)      380 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/models/settings.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)    10963 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/models/sysinfo.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     3869 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/profiler.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     1265 2022-11-24 15:50:02.000000 msaBase-0.0.9/msaBase/router.py
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)    14384 2022-11-22 10:10:58.000000 msaBase-0.0.9/msaBase/sysinfo.py
+drwxrwxr-x   0 cornhub   (1000) cornhub   (1000)        0 2022-11-24 17:12:13.607689 msaBase-0.0.9/msaBase.egg-info/
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     4154 2022-11-24 17:12:13.000000 msaBase-0.0.9/msaBase.egg-info/PKG-INFO
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)      580 2022-11-24 17:12:13.000000 msaBase-0.0.9/msaBase.egg-info/SOURCES.txt
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)        1 2022-11-24 17:12:13.000000 msaBase-0.0.9/msaBase.egg-info/dependency_links.txt
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)      912 2022-11-24 17:12:13.000000 msaBase-0.0.9/msaBase.egg-info/requires.txt
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)        8 2022-11-24 17:12:13.000000 msaBase-0.0.9/msaBase.egg-info/top_level.txt
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)        1 2022-11-24 17:06:05.000000 msaBase-0.0.9/msaBase.egg-info/zip-safe
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     4343 2022-11-24 17:11:51.000000 msaBase-0.0.9/requirements.txt
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)       38 2022-11-24 17:12:13.607689 msaBase-0.0.9/setup.cfg
+-rw-rw-r--   0 cornhub   (1000) cornhub   (1000)     2319 2022-11-22 10:10:58.000000 msaBase-0.0.9/setup.py
```

### Comparing `msaBase-0.0.83/LICENCE` & `msaBase-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.83/PKG-INFO` & `msaBase-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: msaBase
-Version: 0.0.83
+Version: 0.0.9
 Summary: msaBase - General package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo, Healtcheck, Error Handling etc.
 Home-page: https://github.com/u2d-ai/msaBase
-Download-URL: http://pypi.python.org/pypi/msaBase
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
+Download-URL: http://pypi.python.org/pypi/msaBase
 Project-URL: Documentation, http://msaBase.u2d.ai/
 Project-URL: Source, https://github.com/u2d-ai/msaBase
 Project-URL: Tracker, https://github.com/u2d-ai/msaBase/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -92,7 +93,9 @@
 Build:  
 
     python setup.py sdist
 
 Publish to pypi:
 
     twine upload dist/*
+
+
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: msaBase Version: 0.0.83 Summary: msaBase - General
+Metadata-Version: 2.1 Name: msaBase Version: 0.0.9 Summary: msaBase - General
 package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo,
 Healtcheck, Error Handling etc. Home-page: https://github.com/u2d-ai/msaBase
-Download-URL: http://pypi.python.org/pypi/msaBase Author: Stefan Welcker
-Author-email: stefan@u2d.ai License: MIT Project-URL: Documentation, http://
+Author: Stefan Welcker Author-email: stefan@u2d.ai License: MIT Download-URL:
+http://pypi.python.org/pypi/msaBase Project-URL: Documentation, http://
 msaBase.u2d.ai/ Project-URL: Source, https://github.com/u2d-ai/msaBase Project-
-URL: Tracker, https://github.com/u2d-ai/msaBase/issues Classifier: Development
-Status :: 4 - Beta Classifier: Framework :: FastAPI Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Database Classifier: Topic ::
-Database :: Front-Ends Classifier: Topic :: Documentation Classifier: Topic ::
-Internet :: WWW/HTTP :: WSGI :: Server Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Description-Content-Type: text/markdown License-File: LICENCE
+URL: Tracker, https://github.com/u2d-ai/msaBase/issues Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta Classifier: Framework :: FastAPI
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: MacOS :: MacOS X Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+:: Linux Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Database
+Classifier: Topic :: Database :: Front-Ends Classifier: Topic :: Documentation
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server Classifier: Topic
+:: Software Development :: Libraries Classifier: Topic :: Software Development
+:: Libraries :: Python Modules Description-Content-Type: text/markdown License-
+File: LICENCE
  > msaBase- General Package for Microservices based on FastAPI like Profiler,
              Scheduler, Sysinfo, Healtcheck, Error Handling etc.
                    Optimized for use with FastAPI/Pydantic.
                  [Package_version] [Supported_Python_versions]
 ------ **Documentation**: Documentation_(https://msaBase.u2d.ai/) ------ ##
 Features - **MSABaseExceptionHandler**: Central exception handler which sends
 formatted exception to logger - **Filehandler utilities**: Classes for
```

### Comparing `msaBase-0.0.83/README.md` & `msaBase-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.83/msaBase/config.py` & `msaBase-0.0.9/msaBase/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 import json
 import os
-from typing import Any, Dict, List, Optional, Union
+from functools import lru_cache
+from typing import List, Optional
 
 from msaDocModels.health import MSAHealthDefinition
 from pydantic import BaseModel
 
-from msaBase.helpers import _prioritize_envs_in_settings
 from msaBase.logger import logger
 from msaBase.models.settings import MSAAppSettings
-from msaBase.utils.constants import HTTPCEPTION_EXCLUDE_STATUS_CODES
 
 
 class MSAServiceStatus(BaseModel):
     """
     **MSAServiceStatus** Pydantic Response Class
     """
 
@@ -35,183 +34,138 @@
     initializer, or by setting the corresponding environment variable.
 
     Attribute `xxx_yyy` corresponds to environment variable `API_XXX_YYY`. So, for example, to override
     `openapi_prefix`, you would set the environment variable `API_OPENAPI_PREFIX`.
 
     Note that assignments to variables are also validated, ensuring that even if you make runtime-modifications
     to the config, they should have the correct types.
-
-    Attributes:
-        name: Service Name, also used as Title.
-        description: Description of the Service.
-        version: Version of the Service.
-        host: Host/IP which the service runs on.
-        port: Port which the service binds to.
-        dapr_http_port: Port http which  used dapr app.
-        dapr_grpc_port: Port grpc which used dapr app.
-        tags: Optional Metadata: Use this to carry some variables through the service instance.
-        allow_origins: CORSMiddleware. List of allowed origins (as strings) or all of them with the wildcard "*".
-        allow_credentials: CORSMiddleware. Allow (False) Credentials (Authorization headers, Cookies, etc).
-        allow_methods: CORSMiddleware. Specific HTTP methods (POST, PUT) or all of them with the wildcard "*".
-        allow_headers: CORSMiddleware. List[str]. Specific HTTP headers or all of them with the wildcard "*".
-        healthdefinition: Healthdefinition Instance.
-        uvloop: Use UVLoop instead of asyncio loop.
-        sysrouter: Enable the System Routes defined by router.system module (/sysinfo, /sysgpuinfo, /syserror, ...).
-        servicerouter: Enable the Service Routes defined by the MSAApp
-        (/scheduler, /status, /defintion, /settings, /schema, /info, ...).
-        starception: Enable Starception Middleware.
-        validationception: Enable Validation Exception Handler.
-        httpception: Enable the HTTP Exception Handler, which provides HTML Error Pages instead of JSONResponse.
-        httpception_exclude: List of HTTP Exception Codes which are excluded and just
-        forwarded by the HTTP Exception Handler.
-        cors: Enable CORS Middleware.
-        httpsredirect: Enable HTTPS Redirect Middleware.
-        gzip: Enable GZIP Middleware.
-        session: Enable Session Middleware.
-        csrf: Enable CSRF Forms Protection Middleware.
-        msgpack: Enable Messagepack Negotiation Middleware.
-        instrument: Enable Prometheus Instrumentation for the instance.
-        signal_middleware: Enable MSASignal Middleware.
-        task_middleware: Enable MSATask Middleware.
-        context: Enable Context Middleware.
-        profiler: Enable Profiler Middleware.
-        profiler_output_type: Set the Profiler Output Type, should be html or text,
-        html is needed if you want to use the profiler on the Admin Site.
-        profiler_single_calls: Enable to Track each Request by the Profiler.
-        profiler_url: Set the URL to reach the profiler result html, /profiler.
-        timing: Enables Timing Middleware, reports timing data at the granularity of individual endpoint calls.
-        limiter: Enables Rate Limiter (slowapi).
-        background_scheduler: Enables Background Scheduler.
-        asyncio_scheduler: Enables Asyncio Scheduler.
-        abstract_fs: Enables internal Abstract Filesystem.
-        abstract_fs_url: Set's Filesystem URL.
-        json_db_url: Set's DB URL, for nonlocal JSON DB.
-        contact: Contacts of the service owner.
-        progress_topic: Topic to which services send their progress.
     """
 
     name: str = "msaBase Service"
-    description: str = ""
+    """Service Name, also used as Title."""
     version: str = "0.0.0"
-    host: str = "0.0.0.0"
+    """Version of the Service."""
+    host: str = "127.0.0.1"
+    """Host/IP which the service runs on."""
     port: int = 8000
+    """Port which the service binds to."""
     dapr_http_port: int = 6000
-    dapr_grpc_port: int = 50001
     tags: List[str] = []
+    """Optional Metadata: Use this to carry some variables through the service instance."""
     allow_origins: List[str] = ["*"]
+    """CORSMiddleware. List[str]. List of allowed origins (as strings) or all of them with the wildcard ``*`` ."""
     allow_credentials: bool = False
+    """CORSMiddleware. Bool. Allow (False) Credentials (Authorization headers, Cookies, etc)."""
     allow_methods: List[str] = ["*"]
+    """CORSMiddleware. List[str]. Specific HTTP methods (POST, PUT) or all of them with the wildcard ``*`` ."""
     allow_headers: List[str] = ["*"]
+    """CORSMiddleware. List[str]. Specific HTTP headers or all of them with the wildcard ``*`` ."""
     healthdefinition: MSAHealthDefinition = MSAHealthDefinition()
+    """Healthdefinition Instance."""
     uvloop: bool = True
+    """Use UVLoop instead of asyncio loop."""
     sysrouter: bool = True
+    """Enable the System Routes defined by router.system module (/sysinfo, /sysgpuinfo, /syserror, ...)."""
     servicerouter: bool = True
+    """Enable the Service Routes defined by the MSAApp (/scheduler, /status, /defintion, /settings, /schema, /info, ...)."""
     starception: bool = True
+    """Enable Starception Middleware."""
     validationception: bool = True
+    """Enable Validation Exception Handler."""
     httpception: bool = True
-    httpception_exclude: List[int] = HTTPCEPTION_EXCLUDE_STATUS_CODES
+    """Enable the HTTP Exception Handler, which provides HTML Error Pages instead of JSONResponse."""
+    httpception_exclude: List[int] = [
+        307,
+    ]
+    """List of HTTP Exception Codes which are excluded and just forwarded by the HTTP Exception Handler."""
     cors: bool = True
+    """Enable CORS Middleware."""
     httpsredirect: bool = False
+    """Enable HTTPS Redirect Middleware."""
     gzip: bool = False
+    """Enable GZIP Middleware."""
     session: bool = False
+    """Enable Session Middleware."""
     csrf: bool = False
+    """Enable CSRF Forms Protection Middleware."""
     msgpack: bool = False
+    """Enable Messagepack Negotiation Middleware."""
     instrument: bool = True
+    """Enable Prometheus Instrumentation for the instance."""
     signal_middleware: bool = False
+    """Enable MSASignal Middleware."""
     task_middleware: bool = False
+    """Enable MSATask Middleware."""
+    graphql: bool = False
+    """Enable initiation of Strawberry GraphQLRouter (/graphql)."""
     context: bool = False
+    """Enable Context Middleware."""
     profiler: bool = False
-    profiler_output_type: str = "html"
+    """Enable Profiler Middleware."""
+    profiler_output_type: str = "html"  # text or html
+    """Set the Profiler Output Type, should be html or text, html is needed if you want to use the profiler on the Admin Site."""
     profiler_single_calls: bool = False
+    """Enable to Track each Request by the Profiler."""
     profiler_url: str = "/profiler"
+    """Set the URL to reach the profiler result html, /profiler."""
     timing: bool = False
+    """Enables Timing Middleware, reports timing data at the granularity of individual endpoint calls."""
     limiter: bool = False
-    background_scheduler: bool = False
-    asyncio_scheduler: bool = False
+    """Enables Rate Limiter (slowapi)."""
+    background_scheduler: bool = True
+    "Enables Background Scheduler."
+    asyncio_scheduler: bool = True
+    "Enables Asyncio Scheduler."
     abstract_fs: bool = False
+    """Enables internal Abstract Filesystem."""
     abstract_fs_url: str = "."
+    """Set's Filesystem URL"""
+    tiny_json_db: bool = False
+    """Enables internal NoSQl/TinyDB DB."""
+    json_db_memory_only: bool = False
+    """JSON DB only in memory, don't store to file/db url"""
+    tiny_json_db_url: str = "./msa_base.json"
+    """Set's DB URL, compatibility with async and BaseModel/SQLAlchemy is required."""
     json_db_url: str = ""
-    sql_db_url: str = ""
-    contact: Dict[str, Union[str, Any]] = {
-        "name": "Marcus Rostalski",
-        "url": "https://www.sparkasse-bremen.de/",
-        "email": "marcus.rostalski@sparkasse-bremen.de",
-    }
-    progress_topic: str = "progress"
-
-    def save_config(self) -> None:
-        """
-        Saves config to a JSON file
-        """
+    """Set's DB URL, for nonlocal JSON DB"""
+    sqlite_db: bool = False
+    """Enables internal Asynchron SQLite DB."""
+    sqlite_db_debug: bool = False
+    """Enables internal DB Debug output."""
+    sqlite_db_crud: bool = False
+    """Enables CRUD API creation of the provided BaseModels."""
+    sqlite_db_meta_drop: bool = False
+    """If True, all existing Data and Schemas in internal DB get's deleted at Startup."""
+    sqlite_db_meta_create: bool = False
+    """Enables internal DB Metadata creation from defined BaseModels at Startup."""
+    sqlite_db_url: str = "sqlite+aiosqlite:///msa_base.sqlite_db?check_same_thread=True"
+    """Set's DB URL, compatibility with async and BaseModel/SQLAlchemy is required."""
+
+    def saveConfig(self):
         sa = self.copy(deep=True)
         with open("config.json", "w") as fp:
             json.dump(sa.dict(), fp, sort_keys=True, indent=4)
 
     @staticmethod
-    def load_config():
-        """
-        Loads config from JSON file.
-
-        Returns:
-            MSAServiceDefinition config model
-        """
-        settings: MSAServiceDefinition = MSAServiceDefinition()
+    def loadConfig():
+        ret: MSAServiceDefinition = MSAServiceDefinition()
         if os.path.exists("config.json"):
             with open("config.json", "rb") as fp:
-                json_config: dict = json.load(fp)
-                retrieved_envs = _prioritize_envs_in_settings(
-                    settings.Config.env_prefix
-                )
-                merged_config_payload = {**json_config, **retrieved_envs}
-                ret = MSAServiceDefinition.parse_obj(merged_config_payload)
+                intext = json.load(fp)
+                ret = MSAServiceDefinition.parse_obj(intext)
             logger.info("Loaded config file")
         else:
-            settings.save_config()
-            ret = MSAServiceDefinition.parse_obj(settings)
+            ret.saveConfig()
         return ret
 
 
+_msa_config: MSAServiceDefinition = MSAServiceDefinition.loadConfig()
+
+
+@lru_cache()
 def get_msa_app_settings() -> MSAServiceDefinition:
     """
-    Returns a cached instance of the MSAServiceDefinition object.
-
+    This function returns a cached instance of the MSAServiceDefinition object.
     Note:
         Caching is used to prevent re-reading the environment every time the API settings are used in an endpoint.
     """
-    return MSAServiceDefinition.load_config()
-
-
-class ConfigDTO(BaseModel):
-    """
-    DTO that contains needed attributes to be processed.
-
-    Attributes:
-        one_time: Flag indicating whether the configuration is applied only to one request.
-        config: Service config.
-    """
-
-    one_time: bool = False
-    config: MSAServiceDefinition
-
-
-class ConfigInput(BaseModel):
-    """
-    Pydantic model to receive service configs from pub/sub.
-
-    Attributes:
-        data: Service config.
-    """
-
-    data: ConfigDTO
-
-
-class ConfigDataDTO(BaseModel):
-    """
-    DTO that represents result of service work.
-
-    Attributes:
-        service_name: Service name to distinguish.
-        config_dto: Service config.
-    """
-
-    service_name: str
-    config_dto: ConfigDTO
+    return _msa_config
```

### Comparing `msaBase-0.0.83/msaBase/configurate.py` & `msaBase-0.0.9/msaBase/configurate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,393 +1,291 @@
 # -*- coding: utf-8 -*-
 """Main Service Module for MSAApp.
 
 Initialize with a MSAServiceDefintion Instance to control the features and functions of the MSAApp.
 
 """
-import json
 import os
+from asyncio import Task
 from datetime import datetime
-from functools import wraps
-from typing import Any, Dict, List, Optional, Type, Union
-
-import aiohttp
-import sentry_sdk
-from apscheduler.schedulers.asyncio import AsyncIOScheduler
-from apscheduler.schedulers.background import BackgroundScheduler
+from typing import List, Optional, Type, Union
 from dapr.clients import DaprClient
-from dapr.ext.fastapi import DaprApp
+
 from fastapi import FastAPI, HTTPException
 from fastapi.encoders import jsonable_encoder
 from fastapi.exception_handlers import http_exception_handler
 from fastapi.exceptions import RequestValidationError
 from fastapi.responses import ORJSONResponse
-from fs.base import FS
 from loguru import logger as logger_gruru
-from msaBase.config import ConfigDTO, ConfigInput, MSAServiceDefinition, MSAServiceStatus, get_msa_app_settings
-from msaBase.errorhandling import getMSABaseExceptionHandler
-from msaBase.healthcheck import MSAHealthCheck
-from msaBase.logger import init_logging
-from msaBase.models.functionality import FunctionalityTypes
-from msaBase.models.middlewares import MiddlewareTypes
-from msaBase.models.sysinfo import MSASystemGPUInfo, MSASystemInfo
-from msaBase.sysinfo import get_sysgpuinfo, get_sysinfo
-from msaBase.utils.constants import PUBSUB_NAME, REGISTRY_TOPIC, SERVICE_TOPIC
 from msaDocModels.health import MSAHealthDefinition, MSAHealthMessage
-from msaDocModels.openapi import MSAOpenAPIInfo
-from msaDocModels.scheduler import MSASchedulerStatus, MSASchedulerTaskDetail, MSASchedulerTaskStatus
+from msaDocModels.scheduler import (
+    MSASchedulerStatus,
+    MSASchedulerTaskDetail,
+    MSASchedulerTaskStatus,
+)
 from msaDocModels.sdu import SDUVersion
-from msaFilesystem.msafs import MSAFilesystem
-from pyinstrument import Profiler
-from slowapi import Limiter
+from msaDocModels.openapi import MSAOpenAPIInfo
+from sqlmodel import SQLModel
 from starlette import status
 from starlette.exceptions import HTTPException as StarletteHTTPException
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, JSONResponse, Response
 from starlette_context import plugins
 
+from msaBase.config import MSAServiceDefinition, MSAServiceStatus
+from msaBase.errorhandling import getMSABaseExceptionHandler
+from msaBase.logger import init_logging
+from msaBase.models.functionality import FunctionalityTypes
+from msaBase.models.middlewares import MiddlewareTypes
+from msaBase.models.sysinfo import MSASystemInfo
+from msaBase.sysinfo import get_sysinfo
+
 
-def get_secret_key() -> str:
+def getSecretKey() -> str:
     """
     Get Secret Key for Token creation from OS Environment Variable **SECRET_KEY_TOKEN**
 
     Returns:
         key: The SECRET_KEY_TOKEN.
 
     """
     key: str = os.getenv(
         "SECRET_KEY_TOKEN",
         "u2dmsaservicex_#M8A{1o3Bd?<ipwt^K},Z)OE<Fkj-X9IILWq|Cf`Y:HFI~&2L%Ion3}+p{T%",
     )
     return key
 
 
-def get_secret_key_sessions() -> str:
+def getSecretKeySessions() -> str:
     """
     Get Secret Key for Session Middleware from OS Environment Variable **SECRET_KEY_SESSIONS**
 
     Returns:
         key: The SECRET_KEY_SESSIONS.
 
     """
     key: str = os.getenv(
         "SECRET_KEY_SESSIONS",
         "u2dmsaserviceeP)zg5<g@4WJ0W8'?ad!T9UBvW1z2k|y~|Pgtewv=H?GY_Q]t~-~UUe'pJ0V[>!<)",
     )
     return key
 
 
-def get_secret_key_csrf() -> str:
+def getSecretKeyCSRF() -> str:
     """
     Get Secret Key for CSRF Middleware from OS Environment Variable **SECRET_KEY_CSRF**
 
     Returns:
         key: The SECRET_KEY_CSRF.
 
     """
     key: str = os.getenv(
         "SECRET_KEY_CSRF",
         "u2dmsaservicee_rJM'onkEV1trD=I7dci$flB)aSNW+raL4j]Ww=n~_BRg35*3~(E.>rx`1aTw:s",
     )
     return key
 
 
-async def load_config(url: str) -> None:
-    """
-    Get config.
-
-    Parameters:
-
-        url: request URL.
-    """
-    try:
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as resp:
-                if resp.status == 200:
-                    config = MSAServiceDefinition.parse_obj(await resp.json())
-                    new_config = get_msa_app_settings()
-                    if new_config.dict(exclude={"version"}) == config.dict(exclude={"version"}):
-                        return
-
-                    with open("config.json", "w") as json_file:
-                        json.dump(config.dict(), json_file, sort_keys=True, indent=4)
-
-                    logger_gruru.info("New config saved to config.json")
-                else:
-                    logger_gruru.info("Config not found")
-    except BaseException as ex:
-        logger_gruru.error(ex)
-
-
 class MSAApp(FastAPI):
     """Creates an application msaBase instance.
 
     Note:
         As with FastApi the MSAApp provides two events:
-        ``startup``: A list of callables to run on application startup. Startup handler callables do not take
-        any arguments, and may be be either standard functions, or async functions.
-        ``shutdown``: A list of callables to run on application shutdown. Shutdown handler callables do not
-        take any arguments, and may be be either standard functions, or async functions.
+        ``startup``: A list of callables to run on application startup. Startup handler callables do not take any arguments, and may be be either standard functions, or async functions.
+        ``shutdown``: A list of callables to run on application shutdown. Shutdown handler callables do not take any arguments, and may be be either standard functions, or async functions.
         Those are also used internally, which are triggered before the external events.
 
         Do not include the `self` parameter in the ``Args`` section.
 
     Args:
         settings: MSAServiceDefinition (Must be provided), instance of a service definition with all settings
-        sql_models: List of SQLModel Default None, provide list of your SQLModel Classes and the instance can create
-        CRUD API and if site is enabled also UI for CRUD auto_mount_site: Default True,
-        if site is enabled in settings and this is true, mounts the site in internal startup event.
+        sql_models: List of SQLModel Default None, provide list of your SQLModel Classes and the instance can create CRUD API and if site is enabled also UI for CRUD
+        auto_mount_site: Default True, if site is enabled in settings and this is true, mounts the site in internal startup event.
 
     Attributes:
         logger: loguru logger instance
         auto_mount_site: bool auto_mount_site
         settings: MSAServiceDefinition settings instance.
         healthdefinition: MSAHealthDefinition settings.healthdefinition
         limiter: Limiter = None
+        db_engine: AsyncEngine = Db Engine instance
+        sql_models: List[SQLModel] = sql_models
+        sql_cruds: List[MSASQLModelCrud] = []
+        scheduler: MSAScheduler = None
+        scheduler_task: The Task instance that runs the Scheduler in the Background
         ROOTPATH: str os.path.join(os.path.dirname(__file__))
 
     """
 
     def __init__(
-            self,
-            settings: MSAServiceDefinition,
-            auto_mount_site: Optional[bool] = True,
-            title: Optional[str] = None,
-            description: Optional[str] = None,
-            host: Optional[str] = None,
-            version: Optional[str] = None,
-            openapi_url: Optional[str] = None,
-            redoc_url: Optional[str] = None,
-            openapi_tags: Optional[List[Dict[str, Any]]] = None,
-            terms_of_service: Optional[str] = None,
-            contact: Optional[Dict[str, Union[str, Any]]] = None,
-            license_info: Optional[Dict[str, Union[str, Any]]] = None,
-            *args,
-            **kwargs,
+        self,
+        settings: MSAServiceDefinition,
+        sql_models: List[SQLModel] = None,
+        auto_mount_site: bool = True,
+        title: str = "FastAPI",
+        description: str = "",
+        version: str = "0.1.0",
+        openapi_url: Optional[str] = "/openapi.json",
+        *args,
+        **kwargs,
     ) -> None:
         # call super class __init__
         super().__init__(*args, **settings.fastapi_kwargs)
-        self.profiler = None
-        self.settings = settings
 
-        self.previous_settings = None
-        self.one_time_config = False
         self.logger = logger_gruru
         self.fastApi = FastAPI
-        self.daprApp = DaprApp(self)
-        self.title = title if title else self.settings.title
-        self.description = description if description else self.settings.description
-        self.host = host if host else self.settings.host
-
-        self.version = version if version else self.settings.version
-        self.openapi_url = openapi_url if openapi_url else self.settings.openapi_url
-        self.redoc_url = redoc_url if redoc_url else self.settings.redoc_url
+        self.title = title
+        self.description = description
+        self.version = version
+        self.openapi_url = openapi_url
         self.auto_mount_site: bool = auto_mount_site
-        self.SDUVersion = SDUVersion(version=self.settings.version, creation_date=datetime.utcnow().isoformat())
-        self.license_info = license_info
-        self.contact = contact if contact else self.settings.contact
-        self.terms_of_service = terms_of_service
-        self.openapi_tags = openapi_tags
+        self.settings = settings
+        self.SDUVersion = SDUVersion(
+            version=self.settings.version, creation_date=datetime.utcnow().isoformat()
+        )
         self.healthdefinition: MSAHealthDefinition = self.settings.healthdefinition
-        self.limiter: Optional[Limiter] = None
-        self.background_scheduler: Optional[BackgroundScheduler] = None
-        self.asyncio_scheduler: Optional[AsyncIOScheduler] = None
+        self.limiter: "Limiter" = None
+        self.sqlite_db_engine: "AsyncEngine" = None
+        self.json_db_engine: "TinyDB" = None
+        self.sql_models: List[SQLModel] = sql_models
+        self.sql_cruds: List["MSASQLModelCrud"] = []
+        self.background_scheduler: "BackgroundScheduler" = None
+        self.asyncio_scheduler: "AsyncIOScheduler" = None
         self.site = None
+        self._scheduler_task: Task = None
         self.ROOTPATH = os.path.join(os.path.dirname(__file__))
-        self.abstract_fs: Optional[MSAFilesystem] = None
-        self.fs: Optional[FS] = None
-        self.healthcheck: Optional[MSAHealthCheck] = None
+        self.abstract_fs: "MSAFilesystem" = None
+        self.fs: "FS" = None
+        self.healthcheck: "health.MSAHealthCheck" = None
         self.logger.info_pub = self.logger_info
 
         init_logging()
         self.add_middlewares()
         self.add_functionality()
+        self.logger.info("Events - Add Internal Handlers")
         self.add_event_handler("shutdown", self.shutdown_event)
         self.add_event_handler("startup", self.startup_event)
-        self.create_dapr_endpoint()
-
-    def create_dapr_endpoint(self):
-        """
-        Subscribes service to pubsub topic through which new configs will be received.
-        """
-
-        @self.daprApp.subscribe(pubsub=PUBSUB_NAME, topic=SERVICE_TOPIC)
-        async def read_config(received_config: ConfigInput) -> None:
-            """
-            Receives new config and updates current settings with received data.
-
-            Parameters:
-                received_config: Data to update current config with.
-            """
-            try:
-                self.logger.info(f"Received config from svcRegistry. Data: {received_config.data}")
-                if received_config.data.config.name == self.settings.name:
-                    reload_needed = self.update_settings(received_config.data.config, received_config.data.one_time)
-                    if reload_needed:
-                        self.logger.info("New config needs reload.")
-                        with open("config.json", "w") as json_file:
-                            json.dump(received_config.data.dict(), json_file)
-
-                        self.logger.info("New config saved to config.json")
-
-            except Exception as ex:
-                self.logger.info(ex)
-
-    @staticmethod
-    def uses_temporary_config(function):
-        """
-        Makes an endpoint use one-time config whenever it is present.
-
-        Parameters:
-            function: an endpoint to wrap
-        """
-
-        @wraps(function)
-        def decorator(self, *args, **kwargs):
-            result = function(self, *args, **kwargs)
-            if self.one_time_config:
-                self.logger.info("One-time config used. Loading previous config...")
-                self.update_settings(self.previous_settings)
-
-                self.previous_settings = None
-                self.one_time_config = False
-            return result
-
-        return decorator
 
-    def model_block(self, func):
-        """
-        Block ML model while data in process.
-
-        Parameters:
-            func: an endpoint to wrap
-        """
-        @wraps(func)
-        def decorator(*args, **kwargs):
-            if not self.state.blocker.check_ml_model_availability():
-                raise HTTPException(
-                    status_code=status.HTTP_408_REQUEST_TIMEOUT,
-                    detail="The ML model is busy processing data and is not available at the moment. Please try later."
-                )
-            try:
-                self.state.blocker.set_ml_model_unavailable()
-                return func(*args, **kwargs)
-            except Exception as ex:
-                raise ex
-            finally:
-                self.state.blocker.set_ml_model_available()
-        return decorator
-
-    def logger_info(self, message: str, service_name: str = "", topic_name: str = "") -> None:
-        """
-        Sends message to pubsub topic.
-
-        Parameters:
-            message: JSON message to send.
-            topic_name: name of pubsub topic that needs this message.
-            service_name: the name of the service from which the call was made
-        """
+    def logger_info(self, message: str, topic_name: str = ""):
         if topic_name:
             with DaprClient() as client:
                 client.publish_event(
-                    pubsub_name=PUBSUB_NAME,
+                    pubsub_name="spk_pub_sub",
                     topic_name=topic_name,
-                    data=f"[{service_name}]: " + message if service_name else message,
+                    data=message,
                     data_content_type="application/json",
                 )
         self.logger.info(message)
 
     async def extend_startup_event(self) -> None:
         """You can extend the main shutdown"""
 
     async def startup_event(self) -> None:
         """Internal Startup Event Handler"""
         self.logger.info("msaBase Internal Startup MSAUIEvent")
         await self.extend_startup_event()
 
+        if self.settings.sqlite_db:
+            async with self.sqlite_db_engine.begin() as conn:
+                if self.settings.sqlite_db_meta_drop:
+                    self.logger.info(
+                        "SQLite DB - Drop Meta All: " + self.settings.sqlite_db_url
+                    )
+                    await conn.run_sync(SQLModel.metadata.drop_all)
+                if self.settings.sqlite_db_meta_create:
+                    self.logger.info(
+                        "SQLite DB - Create Meta All: " + self.settings.sqlite_db_url
+                    )
+                    await conn.run_sync(SQLModel.metadata.create_all)
+            await self.sqlite_db_engine.dispose()
+
     async def extend_shutdown_event(self) -> None:
         """You can extend the main shutdown"""
 
     async def shutdown_event(self) -> None:
         """Internal Shutdown event handler"""
         self.logger.info("msaBase Internal Shutdown MSAUIEvent")
         await self.extend_shutdown_event()
 
-        self.stop_scheduler(self.background_scheduler, "Background")
-        self.stop_scheduler(self.asyncio_scheduler, "Asyncio")
+        if self.settings.background_scheduler:
+            self.logger.info("Stop Background Scheduler")
+            self.background_scheduler.shutdown()
+
+        if self.settings.asyncio_scheduler:
+            self.logger.info("Stop Asyncio Scheduler")
+            self.asyncio_scheduler.shutdown()
 
         if self.healthcheck:
             self.logger.info("Stopping Healthcheck Thread")
-            self.healthcheck.stop()
+            await self.healthcheck.stop()
             self.healthcheck = None
 
         if self.settings.abstract_fs:
             try:
                 self.logger.info("Closing Abstract Filesystem")
                 self.fs.close()
             except Exception as ex:
-                getMSABaseExceptionHandler().handle(ex, "Error: Closing Abstract Filesystem failed:")
+                getMSABaseExceptionHandler().handle(
+                    ex, "Error: Closing Abstract Filesystem failed:"
+                )
 
-    def stop_scheduler(self, scheduler: Union[None, AsyncIOScheduler, BackgroundScheduler], name: str) -> None:
-        if scheduler:
-            self.logger.info(f"Stop {name} Scheduler")
-            if scheduler.get_jobs():
-                scheduler.shutdown()
-            if isinstance(scheduler, AsyncIOScheduler):
-                self.asyncio_scheduler = None
-            else:
-                self.background_scheduler = None
+        if self.settings.tiny_json_db:
+            self.logger.info("JSON DB - Close: " + self.settings.sqlite_db_url)
+            self.json_db_engine.close()
+
+        if self.settings.sqlite_db:
+            self.logger.info(
+                "SQLite DB - Dispose Connections: " + self.settings.sqlite_db_url
+            )
+            await self.sqlite_db_engine.dispose()
 
-    async def get_system_info(self) -> MSASystemGPUInfo:
-        """Get System Nvidia GPU's Info
-        Returns:
-            sys_info: MSASystemGPUInfo Pydantic Model
+    async def init_graphql(self, strawberry_schema) -> None:
         """
-        sys_info = get_sysinfo(f"{self.settings.name} {self.settings.version}")
-        return sys_info
-
-    async def get_system_gpu_info(self) -> MSASystemGPUInfo:
-        """Get System Nvidia GPU's Info
-        Returns:
-            sys_gpu_info: MSASystemGPUInfo Pydantic Model
+        Internal helper function to initialize the graphql router
         """
-        sys_gpu_info = get_sysgpuinfo(f"{self.settings.name} {self.settings.version}")
-        return sys_gpu_info
+        if self.settings.graphql:
+            from strawberry.fastapi import GraphQLRouter
+
+            self.graphql_schema = strawberry_schema
+            self.graphql_app = GraphQLRouter(self.graphql_schema, graphiql=True)
+            self.include_router(self.graphql_app, prefix="/graphql", tags=["graphql"])
 
     async def get_healthcheck(self, request: Request) -> ORJSONResponse:
         """
         Get Healthcheck Status
         """
+        self.logger.info("Called - get_healthcheck :" + str(request.url))
         msg: MSAHealthMessage = MSAHealthMessage()
         if not self.healthcheck:
             msg.message = "Healthcheck is disabled!"
-            health_status = status.HTTP_409_CONFLICT
         else:
             msg.healthy = self.healthcheck.is_healthy
             msg.message = await self.healthcheck.get_health()
-            health_status = await self.healthcheck.get_status()
             if len(self.healthcheck.error) > 0:
                 msg.error = self.healthcheck.error
 
-        return ORJSONResponse(content=jsonable_encoder(msg), status_code=health_status)
+        return ORJSONResponse(content=jsonable_encoder(msg))
 
     async def get_scheduler_status(self, request: Request) -> MSASchedulerStatus:
         """
         Get Service Scheduler Status, with the registered Task's
 
         Args:
             request: The input http request object
 
         Returns:
             sst: MSASchedulerStatus Pydantic Response Model
 
         """
         self.logger.info("Called - get_scheduler_status :" + str(request.url))
         sst: MSASchedulerStatus = MSASchedulerStatus()
-        if not self.settings.background_scheduler or not self.settings.asyncio_scheduler:
+        if (
+            not self.settings.background_scheduler
+            or not self.settings.asyncio_scheduler
+        ):
             sst.name = self.settings.name
             sst.message = "Schedulers is disabled!"
 
         else:
             sst.name = self.settings.name
             for task in self.background_scheduler.get_jobs():
                 nt: MSASchedulerTaskStatus = MSASchedulerTaskStatus()
@@ -424,14 +322,28 @@
         else:
             sst.name = self.settings.name
             sst.healthy = await self.healthcheck.get_health()
             sst.message = "Healthcheck is enabled!"
 
         return sst
 
+    def get_services_definition(self, request: Request) -> MSAServiceDefinition:
+        """
+        Get Service Definition Info
+
+        Args:
+            request: The input http request object
+
+        Returns:
+            settings: MSAServiceDefinition Pydantic Response Model
+
+        """
+        self.logger.info("Called - get_services_definition :" + str(request.url))
+        return self.settings
+
     def get_services_settings(self, request: Request) -> ORJSONResponse:
         """
         Get Service OpenAPI Schema
 
         Args:
             request: The input http request object
 
@@ -455,19 +367,21 @@
             }
         )
 
     def get_services_openapi_schema(self, request: Request) -> ORJSONResponse:
         """
         Get Service OpenAPI Schema
 
-        Parameters:
+        Args:
             request: The input http request object
 
         Returns:
-            ORJSONResponse openapi schema
+            openapi: ORJSONResponse openapi schema
+
+
         """
         self.logger.info("Called - get_services_openapi_schema :" + str(request.url))
 
         def try_get_json():
             try:
 
                 return jsonable_encoder(self.openapi())
@@ -477,43 +391,42 @@
 
         return ORJSONResponse(
             {
                 self.settings.name: try_get_json(),
             }
         )
 
-    async def msa_exception_handler(self, request: Request, exc: HTTPException) -> Response:
+    async def msa_exception_handler(
+        self, request: Request, exc: HTTPException
+    ) -> Response:
         """
-        Handles all HTTPExceptions if enabled with HTML
-        Response or forward error if the code is in the exclude settings list.
+        Handles all HTTPExceptions if enabled with HTML Response or forward error if the code is in the exclude settings list.
 
-        Parameters:
+        Args:
             request: The input http request object
             exc : The HTTPException instance
 
         Returns:
-            HTTPResponse: response with status code corresponding to the handled exception.
+            HTTPException
+
         """
         error_content = {
             "request": request.__dict__,
             "detail": exc.detail,
             "status": exc.status_code,
             "definitions": jsonable_encoder(self.settings),
         }
-        if exc.status_code not in self.settings.httpception_exclude:
-            sentry_sdk.capture_exception(exc)
         self.logger.error("msa_exception_handler - " + str(error_content))
         return await http_exception_handler(request, exc)
 
     def get_sduversion(self) -> SDUVersion:
-        """
-        Get SDUVersion
-
+        """Get SDUVersion
         Returns:
             sdu_version: Pydantic Version Info Model.
+
         """
         return self.SDUVersion
 
     def get_services_openapi_info(self, request: Request) -> MSAOpenAPIInfo:
         """
         Get Service OpenAPI Info
 
@@ -533,48 +446,26 @@
             oai.url = self.openapi_url
             oai.tags = self.openapi_tags
         except Exception as e:
             oai.tags = ["error:400 error" + e.__str__()]
 
         return oai
 
-    def get_profiler(self, request: Request) -> HTMLResponse:
-        """
-        Get Profiler
-
-        Parameters:
-            request: The input http request object
-
-        Returns:
-            HTMLResponse: response with html code of profiler
-        """
-        self.profiler.start()
-        self.profiler.stop()
-        html = self.profiler.output_html()
-        service_name = f"Profiler for {self.settings.name} {self.settings.version} was disabled"
-        html_code = html.replace("pyinstrument", service_name).replace("Pyinstrument", service_name)
-        return HTMLResponse(html_code)
-
-    async def validation_exception_handler(self, request: Request, exc: RequestValidationError) -> JSONResponse:
-        """
-        Handles validation error exception and returns exception info as a JSON.
-
-        Parameters:
-            request: Request that raised the exception
-            exc: exception to handle
-        Returns:
-            response: JSONResponse that represents the exception
-        """
+    async def validation_exception_handler(
+        self, request: Request, exc: RequestValidationError
+    ) -> JSONResponse:
         self.logger.error("validation_exception_handler - " + str(exc.errors()))
         return JSONResponse(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             content=jsonable_encoder({"detail": exc.errors(), "body": exc.body}),
         )
 
-    async def msa_exception_handler_disabled(self, request: Request, exc: HTTPException) -> JSONResponse:
+    async def msa_exception_handler_disabled(
+        self, request: Request, exc: HTTPException
+    ) -> JSONResponse:
         """
         Handles all HTTPExceptions if Disabled with JSON Response.
 
         Args:
             request: The input http request object
 
         Returns:
@@ -621,75 +512,35 @@
                 if status_middleware:
                     self.choose_functionality_configurator(functionality)()
                 else:
                     self.logger.info(f"Excluded {functionality.readable_name}")
             except Exception as ex:
                 getMSABaseExceptionHandler().handle(ex)
 
-    def update_settings(self, new_config: MSAServiceDefinition, one_time=False) -> bool:
-        """
-        Updates app configuration.
-
-        Parameters:
-            new_config: MSAServiceDefinition. Config received from svcRegistry.
-            one_time: a flag for using the config only one time.
-        Returns:
-            bool. True if app reload is needed, False otherwise.
-        """
-        if one_time:
-            self.previous_settings = self.settings
-
-        for middleware in MiddlewareTypes:
-            current_middleware = getattr(self.settings, middleware.name, None)
-
-            new_middleware = getattr(new_config, middleware.name, None)
-
-            if (current_middleware is not None and new_middleware is not None) and (
-                    current_middleware != new_middleware
-            ):
-                return True
-
-        for functionality in FunctionalityTypes:
-            current_functionality = getattr(self.settings, functionality.name, None)
-
-            new_functionality = getattr(new_config, functionality.name, None)
-            reload_needed = functionality.need_restart
-
-            if (current_functionality is not None and new_functionality is not None) and (
-                    current_functionality != new_functionality
-            ):
-
-                if reload_needed:
-                    return True
-
-                setattr(self.settings, functionality.name, new_functionality)
-                self.choose_functionality_configurator(functionality)()
-
-        return False
-
     def unknown_middleware(self) -> None:
         """
         Unknown Middleware, doing nothing
         """
         self.logger.info("Unknown Middleware")
 
     def unknown_functionality(self) -> None:
         """
         Unknown Functionality, doing  nothing
         """
         self.logger.info("Unknown Functionality")
 
     def choose_middleware_configurator(
-            self, middleware: Union[MiddlewareTypes, FunctionalityTypes]
+        self, middleware: Union[MiddlewareTypes, FunctionalityTypes]
     ) -> Type[unknown_middleware]:
         """
         Get the configurator by type of Middleware
 
         Returns:
             func: The configurator.
+
         """
         configurator_mappings = {
             MiddlewareTypes.profiler: self.configure_profiler_middleware,
             MiddlewareTypes.validationception: self.configure_validation_handler,
             MiddlewareTypes.httpception: self.configure_httpexception_handler,
             MiddlewareTypes.starception: self.configure_starception_middleware,
             MiddlewareTypes.cors: self.configure_cors_middleware,
@@ -700,32 +551,63 @@
             MiddlewareTypes.msgpack: self.configure_msgpack_middleware,
             MiddlewareTypes.context: self.configure_context_middleware,
             MiddlewareTypes.timing: self.configure_timing_middleware,
             MiddlewareTypes.limiter: self.configure_limiter_handler,
         }
         return configurator_mappings.get(middleware, self.unknown_middleware)
 
-    def choose_functionality_configurator(self, middleware: FunctionalityTypes) -> Type[unknown_functionality]:
+    def choose_functionality_configurator(
+        self, middleware: FunctionalityTypes
+    ) -> Type[unknown_functionality]:
         """
         Get the configurator by type of Functionality
 
         Returns:
             func: The configurator.
+
         """
         configurator_mappings = {
             FunctionalityTypes.uvloop: self.configure_event_loop,
+            FunctionalityTypes.json_db: self.configure_json_db,
+            FunctionalityTypes.sqlite_db: self.configure_sqlite_db,
+            FunctionalityTypes.graphql: self.configure_graphql,
             FunctionalityTypes.healthdefinition: self.configure_healthdefinition,
+            FunctionalityTypes.sysrouter: self.configure_sysrouter,
             FunctionalityTypes.servicerouter: self.configure_servicerouter,
             FunctionalityTypes.instrument: self.configure_prometheus_instrument,
             FunctionalityTypes.background_scheduler: self.configure_background_scheduler,
             FunctionalityTypes.asyncio_scheduler: self.configure_asyncio_scheduler,
             FunctionalityTypes.abstract_fs: self.configure_abstract_fs,
         }
         return configurator_mappings.get(middleware, self.unknown_middleware)
 
+    def configure_json_db(self) -> None:
+        """Create JSON DB"""
+        self.logger.info("JSON DB - Init: " + self.settings.sqlite_db_url)
+        from tinydb import TinyDB
+        from tinydb.storages import MemoryStorage
+
+        if self.settings.json_db_memory_only:
+            self.json_db_engine = TinyDB(
+                self.settings.tiny_json_db_url, storage=MemoryStorage
+            )
+        else:
+            self.json_db_engine = TinyDB(
+                self.settings.tiny_json_db_url, storage=TinyDB.default_storage_class
+            )
+
+    def configure_graphql(self) -> None:
+        """Init Graphql"""
+        self.logger.info("Init Graphql")
+        from strawberry import schema
+        from strawberry.fastapi import GraphQLRouter
+
+        self.graphql_app: GraphQLRouter = None
+        self.graphql_schema: schema = None
+
     def configure_starception_middleware(self) -> None:
         """Add Middleware Starception"""
         self.logger.info("Add Middleware Starception")
         from starception import StarceptionMiddleware
 
         self.add_middleware(StarceptionMiddleware)
 
@@ -735,39 +617,42 @@
         if self.settings.background_scheduler or self.settings.asyncio_scheduler:
             self.add_api_route(
                 "/scheduler",
                 self.get_scheduler_status,
                 tags=["service"],
                 response_model=MSASchedulerStatus,
             )
-        self.add_api_route("/", self.get_sduversion, tags=["service"], response_model=SDUVersion)
-        self.add_api_route("/sysinfo", self.get_system_info, tags=["service"], response_model=MSASystemInfo)
-        self.add_api_route(
-            "/sysgpuinfo",
-            self.get_system_gpu_info,
-            tags=["service"],
-            response_model=MSASystemGPUInfo,
-        )
-        self.add_api_route("/settings", self.get_services_settings, tags=["service"])
         self.add_api_route(
             "/status",
             self.get_services_status,
             tags=["service"],
             response_model=MSAServiceStatus,
         )
-        self.add_api_route("/schema", self.get_services_openapi_schema, tags=["openapi"])
+        self.add_api_route(
+            "/definition",
+            self.get_services_definition,
+            tags=["service"],
+            response_model=MSAServiceDefinition,
+        )
+        self.add_api_route(
+            "/sys_info", get_sysinfo, tags=["service"], response_model=MSASystemInfo
+        )
+        self.add_api_route(
+            "/", self.get_sduversion, tags=["service"], response_model=SDUVersion
+        )
+        self.add_api_route("/settings", self.get_services_settings, tags=["service"])
+        self.add_api_route(
+            "/schema", self.get_services_openapi_schema, tags=["openapi"]
+        )
         self.add_api_route(
             "/info",
             self.get_services_openapi_info,
             tags=["openapi"],
             response_model=MSAOpenAPIInfo,
         )
-        if not self.settings.profiler:
-            self.profiler = Profiler()
-            self.add_api_route(self.settings.profiler_url, self.get_profiler, tags=["service"], response_model=MSAOpenAPIInfo)
 
     def configure_limiter_handler(self) -> None:
         """Add Limiter Handler"""
         self.logger.info("Add Limiter Handler")
         from slowapi import Limiter, _rate_limit_exceeded_handler
         from slowapi.errors import RateLimitExceeded
         from slowapi.util import get_remote_address
@@ -788,57 +673,91 @@
             msa_app=self,
         )
 
     def configure_httpexception_handler(self) -> None:
         """Add Handler HTTPException"""
         self.logger.info("Add Handler HTTPException")
         exception_handler = (
-            self.msa_exception_handler if self.settings.httpception else self.msa_exception_handler_disabled
+            self.msa_exception_handler
+            if self.settings.httpception
+            else self.msa_exception_handler_disabled
         )
         self.add_exception_handler(StarletteHTTPException, exception_handler)
 
     def configure_validation_handler(self) -> None:
         """Add Handler ValidationError"""
         self.logger.info("Add Handler ValidationError")
-        self.add_exception_handler(RequestValidationError, self.validation_exception_handler)
+        self.add_exception_handler(
+            RequestValidationError, self.validation_exception_handler
+        )
+
+    def configure_sqlite_db(self) -> None:
+        """Create sqlite db connection and create crud in db by sql_model in Settings"""
+        from sqlalchemy.ext.asyncio import create_async_engine
+        from sqlalchemy.ext.declarative import declarative_base
+        from sqlalchemy.orm import DeclarativeMeta
+
+        self.logger.info("SQLite DB - Init: " + self.settings.sqlite_db_url)
+        self.Base: DeclarativeMeta = declarative_base()
+        self.sqlite_db_engine = create_async_engine(
+            self.settings.sqlite_db_url,
+            echo=self.settings.sqlite_db_debug,
+            future=True,
+        )
+        if self.settings.sqlite_db_crud and self.sql_models:
+            self.configure_db_crud()
+
+    def configure_db_crud(self) -> None:
+        """Register all Models and the crud for them"""
+        if self.settings.sqlite_db_crud and self.sql_models:
+            self.logger.info(
+                "SQLite DB - Register/CRUD SQL Models: " + str(self.sql_models)
+            )
+            from msaCRUD import MSASQLModelCrud
+
+            for model in self.sql_models:
+                new_crud: MSASQLModelCrud = MSASQLModelCrud(
+                    model=model, engine=self.sqlite_db_engine
+                ).register_crud()
+                if self.settings.sqlite_db_crud:
+                    self.include_router(new_crud.router)
+                self.sql_cruds.append(new_crud)
 
     def configure_healthdefinition(self) -> None:
-        """Configure health definition and start healthcheck thread."""
         self.logger.info("Init Healthcheck")
         from msaBase.healthcheck import MSAHealthCheck
 
-        if self.settings.healthdefinition.enabled:
-            self.healthcheck = MSAHealthCheck(
-                healthdefinition=self.healthdefinition,
-                host=self.settings.host,
-                port=self.settings.port,
-            )
-            self.logger.info("Start Healthcheck Thread")
-            self.healthcheck.start()
+        self.healthcheck = MSAHealthCheck(
+            healthdefinition=self.healthdefinition,
+            host=self.settings.host,
+            port=self.settings.port,
+        )
+        self.logger.info("Start Healthcheck Thread")
+        self.healthcheck.start()
         self.add_api_route(
             self.healthdefinition.path,
             self.get_healthcheck,
             response_model=MSAHealthMessage,
             tags=["service"],
         )
 
+    def configure_sysrouter(self) -> None:
+        """Enable Sysrouter"""
+        self.logger.info("Include Sysrouter")
+        from msaBase.router import sys_router
+
+        self.include_router(sys_router)
+
     def configure_abstract_fs(self) -> None:
         """Enable Abstract Filesystem"""
         self.logger.info("Enable Abstract Filesystem")
         from msaFilesystem.msafs import MSAFilesystem
 
-        if self.settings.abstract_fs:
-            try:
-                self.logger.info("Closing Abstract Filesystem")
-                self.fs.close()
-            except Exception as ex:
-                getMSABaseExceptionHandler().handle(ex, "Error: Closing Abstract Filesystem failed:")
-        else:
-            self.abstract_fs = MSAFilesystem(fs_url=self.settings.abstract_fs_url)
-            self.fs = self.abstract_fs.fs
+        self.abstract_fs = MSAFilesystem(fs_url=self.settings.abstract_fs_url)
+        self.fs = self.abstract_fs.fs
 
     def configure_msgpack_middleware(self) -> None:
         """Add Middleware MSGPack"""
         self.logger.info("Add Middleware MSGPack")
         from msgpack_asgi import MessagePackMiddleware
 
         self.add_middleware(MessagePackMiddleware)
@@ -866,52 +785,48 @@
         )
 
     def configure_csrf_middleware(self) -> None:
         """Add Middleware CSRF"""
         self.logger.info("Add Middleware CSRF")
         from starlette_wtf import CSRFProtectMiddleware
 
-        self.add_middleware(CSRFProtectMiddleware, csrf_secret=get_secret_key_csrf())
+        self.add_middleware(CSRFProtectMiddleware, csrf_secret=getSecretKeyCSRF())
 
     def configure_session_middleware(self) -> None:
         """Add Middleware Session"""
         self.logger.info("Add Middleware Session")
         from starlette.middleware.sessions import SessionMiddleware
 
-        self.add_middleware(SessionMiddleware, secret_key=get_secret_key_sessions())
+        self.add_middleware(SessionMiddleware, secret_key=getSecretKeySessions())
 
     def configure_background_scheduler(self) -> None:
         """Add Background Scheduler"""
         self.logger.info("Add Background Scheduler")
         from apscheduler.schedulers.background import BackgroundScheduler
 
-        if self.settings.background_scheduler and not self.background_scheduler:
-            self.background_scheduler = BackgroundScheduler()
-        elif not self.settings.background_scheduler:
-            self.stop_scheduler(self.background_scheduler, "Asyncio")
+        self.background_scheduler = BackgroundScheduler()
+        self.background_scheduler.start()
 
     def configure_asyncio_scheduler(self) -> None:
         """Add Asyncio Scheduler"""
         self.logger.info("Add Asyncio Scheduler")
         from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
-        if self.settings.asyncio_scheduler and not self.asyncio_scheduler:
-            self.asyncio_scheduler = AsyncIOScheduler()
-        elif not self.settings.asyncio_scheduler:
-            self.stop_scheduler(self.asyncio_scheduler, "Asyncio")
+        self.asyncio_scheduler = AsyncIOScheduler()
+        self.asyncio_scheduler.start()
 
     def configure_event_loop(self) -> None:
         """Enable UVLoop"""
         self.logger.info("Enable UVLoop")
         import uvloop
 
         uvloop.install()
 
     def configure_cors_middleware(self) -> None:
-        """Add Middleware CORS"""
+        """ "Add Middleware CORS"""
         self.logger.info("Add Middleware CORS")
         from starlette.middleware.cors import CORSMiddleware
 
         self.add_middleware(
             CORSMiddleware,
             allow_origins=self.settings.allow_origins,
             allow_credentials=self.settings.allow_credentials,
@@ -920,95 +835,24 @@
         )
 
     def configure_timing_middleware(self) -> None:
         """Add Middleware Timing"""
         self.logger.info("Add Middleware Timing")
         from fastapi_utils.timing import add_timing_middleware
 
-        add_timing_middleware(self, record=self.logger.info, prefix="app", exclude="untimed")
+        add_timing_middleware(
+            self, record=self.logger.info, prefix="app", exclude="untimed"
+        )
 
     def configure_gzip_middleware(self) -> None:
         """Add Middleware GZip"""
         self.logger.info("Add Middleware GZip")
         from starlette.middleware.gzip import GZipMiddleware
 
         self.add_middleware(GZipMiddleware)
 
     def configure_httpsredirect_middleware(self) -> None:
         """Add Middleware HTTPSRedirectMiddleware"""
         from starlette.middleware.httpsredirect import HTTPSRedirectMiddleware
 
         self.logger.info("Add Middleware HTTPSRedirect")
         self.add_middleware(HTTPSRedirectMiddleware)
-
-    def send_config(self) -> None:
-        """
-        Sends current config to pubsub registry topic.
-        """
-        try:
-            self.logger.info("Start send config to pubsub")
-            with open("config.json") as json_file:
-                config = MSAServiceDefinition.parse_obj(json.load(json_file))
-                data = ConfigDTO(config=config, one_time=False)
-            self.logger_info(data.json(), topic_name=REGISTRY_TOPIC)
-            self.logger.info(f"Sent config to pubsub, {data}")
-        except Exception as ex:
-            self.logger.error(f"An error occurred while trying to send config to svcRegistry. Exception: {ex}")
-
-    def info_pub_logger(self, message: str) -> None:
-        """Sending progress to the topic
-
-        Parameters:
-
-            message: message with status
-        """
-        if self.settings.debug:
-            self.logger.info(message)
-        else:
-            self.logger.info_pub(
-                message,
-                topic_name=self.settings.progress_topic,
-                service_name=self.settings.name,
-            )
-
-    def init_sentry(self, sentry_dsn: str) -> None:
-        """Sending progress to the topic
-
-        Parameters:
-
-            sentry_dsn: dsn to sentry project
-        """
-        if not self.settings.debug:
-            sentry_sdk.init(
-                dsn=sentry_dsn,
-                traces_sample_rate=1.0,
-            )
-
-
-class AvailabilityML:
-    def __init__(self, app: MSAApp):
-        self.in_process = False
-        self._app = app
-
-    def set_ml_model_unavailable(self) -> None:
-        """
-        Blocks the endpoint while data is being processed.
-        """
-        self.in_process = True
-        self._app.info_pub_logger("The model is processing the data and is not available.")
-
-    def set_ml_model_available(self) -> None:
-        """
-        Unblocks the endpoint.
-        """
-        self.in_process = False
-        self._app.info_pub_logger("The model has finished to process the data and is available.")
-
-    def check_ml_model_availability(self) -> bool:
-        """
-        Return True if service
-
-        Returns:
-
-            False if model is not available
-        """
-        return False if self.in_process else True
```

### Comparing `msaBase-0.0.83/msaBase/errorhandling.py` & `msaBase-0.0.9/msaBase/errorhandling.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         ex_type, ex_value, ex_traceback = sys.exc_info()
 
         # Extract unformatter stack traces as tuples
         trace_back = traceback.extract_tb(ex_traceback)
 
         # Format stacktrace
         self.stack_trace = [
-            "File : %s , Line : %d, Func.Name : %s, Message : %s" % (trace[0], trace[1], trace[2], trace[3])
+            "File : %s , Line : %d, Func.Name : %s, Message : %s"
+            % (trace[0], trace[1], trace[2], trace[3])
             for trace in trace_back
         ]
 
         logger.error("Exception: %s " % ex.__str__(), args)
         logger.error("Exception type : %s " % ex_type.__name__)
         logger.error("Exception message : %s" % ex_value)
         logger.error("Stack trace : %s" % self.stack_trace)
```

### Comparing `msaBase-0.0.83/msaBase/healthcheck.py` & `msaBase-0.0.9/msaBase/healthcheck.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,68 @@
 # -*- coding: utf-8 -*-
 
-from threading import Timer
+import time
+from threading import Thread
 
 import httpx
 from msaDocModels.health import MSAHealthDefinition
-from starlette import status
 
 
-class MSAHealthCheck:
+class MSAHealthCheck(Thread):
     def __init__(self, healthdefinition: MSAHealthDefinition, host: str, port: int):
         """MSAHealthCheckObject, provides a thread to give a healthcheck.
 
-        Parameters:
+        Args:
             healthdefinition: The MSAHealthDefinition instance
             host: IP/URl to call the healtcheck endpoint
             port: Port of the healtcheck endpoint server listener/endpoint
         """
         super().__init__()
         self.url = "http://{}:{}/".format(host, port)
+        self.interval = healthdefinition.interval
         self._is_running = True
         self.healthy: str = "No Healthcheck executed yet:400"
         self.is_healthy: bool = False
         self.error: str = ""
-        self.status = status.HTTP_200_OK
-        self.timer = Timer(healthdefinition.interval, self.run)
 
     async def get_health(self) -> str:
-        """
-        Get the last health check result
+        """Get the last health check result
 
-        Returns:
-            string "positiv: status_code" or "negative: status_code"
-        """
-        return self.healthy
-
-    async def get_status(self) -> str:
-        """
-        Get the status code of check result
+        The string is "positiv: status_code" or "negative: status_code"
 
-        Returns:
-            status code
         """
-        return self.status
-
-    def start(self):
-        self.timer.start()
+        return self.healthy
 
     def run(self):
-        """
-        Run the Healthcheck Thread
+        """Run the Healthcheck Thread
 
         Sleeps by the interval provided by the MSAHealthDefinition.
 
         Uses httpx to call the healthcheck endpoint which is http://{}:{}/".format(host, port)
 
         Any 200 <= response.status_code < 300 is healthy, rest is not healthy
         """
-        try:
-            self.error = ""
-            resp = httpx.get(url=self.url, timeout=3.0)
-            if status.HTTP_200_OK <= resp.status_code < status.HTTP_300_MULTIPLE_CHOICES:
-                self.is_healthy = True
-                self.status = status.HTTP_200_OK
-            else:
+        while self._is_running:
+            try:
+                self.error = ""
+                resp = httpx.get(url=self.url, timeout=3.0)
+                status_code = resp.status_code
+                if 200 <= status_code < 300:
+                    self.is_healthy = True
+                else:
+                    self.is_healthy = False
+            except Exception as e:
+                status_code = 400
                 self.is_healthy = False
-                self.status = status.HTTP_503_SERVICE_UNAVAILABLE
-        except Exception as e:
-            self.status = status.HTTP_503_SERVICE_UNAVAILABLE
-            self.is_healthy = False
-            self.error = e.__str__()
-
-        self.healthy = (
-            "positiv:" + str(self.status) if (200 <= self.status < 300) else "negativ:" + str(self.status)
-        )
+                self.error = e.__str__()
+
+            self.healthy = (
+                "positiv:" + str(status_code)
+                if (200 <= status_code < 300)
+                else "negativ:" + str(status_code)
+            )
+
+            time.sleep(self.interval)
 
-    def stop(self):
+    async def stop(self):
         """Stops the Healthcheck Thread."""
-        self.timer.cancel()
+        self._is_running = False
```

### Comparing `msaBase-0.0.83/msaBase/logger.py` & `msaBase-0.0.9/msaBase/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,55 +10,52 @@
 class InterceptHandler(logging.Handler):
     """
     Default handler from examples in loguru documentaion.
     See https://loguru.readthedocs.io/en/stable/overview.html#entirely-compatible-with-standard-logging
     """
 
     def emit(self, record: logging.LogRecord):
-        """
-        Gets corresponding Loguru level if it exists, finds caller.
-
-        Parameters:
-            record: log record
-        """
         # Get corresponding Loguru level if it exists
         try:
             level = logger.level(record.levelname).name
         except ValueError:
             level = record.levelno
 
         # Find caller from where originated the logged message
         frame, depth = logging.currentframe(), 2
         while frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
 
-        logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
+        logger.opt(depth=depth, exception=record.exc_info).log(
+            level, record.getMessage()
+        )
 
 
 def format_record(record: dict) -> str:
     """
     Custom format for loguru loggers.
     Uses pformat for log any data like request/response body during debug.
     Works with logging if loguru handler it.
 
     Example:
         ```python
-        payload = [{"users":[{"name": "Nick", "age": 87, "is_active": True},
-        {"name": "Alex", "age": 27, "is_active": True}], "count": 2}]
+        payload = [{"users":[{"name": "Nick", "age": 87, "is_active": True}, {"name": "Alex", "age": 27, "is_active": True}], "count": 2}]
         logger.bind(payload=).debug("users payload")
         [   {   'count': 2,
                 'users': [   {'age': 87, 'is_active': True, 'name': 'Nick'},
                              {'age': 27, 'is_active': True, 'name': 'Alex'}]}]
         ```
     """
 
     format_string = LOGURU_FORMAT
     if record["extra"].get("payload") is not None:
-        record["extra"]["payload"] = pformat(record["extra"]["payload"], indent=4, compact=True, width=88)
+        record["extra"]["payload"] = pformat(
+            record["extra"]["payload"], indent=4, compact=True, width=88
+        )
         format_string += "\n<level>{extra[payload]}</level>"
 
     format_string += "{exception}\n"
     return format_string
 
 
 def init_logging():
@@ -86,23 +83,29 @@
     # to redirect their output to the default uvicorn logger
     # works with uvicorn==0.11.6
     # print("Logger", [name for name in logging.root.manager.loggerDict])
 
     for handler in logging.root.handlers[:]:
         logging.root.removeHandler(handler)
 
-    loggers = (logging.getLogger(name) for name in logging.root.manager.loggerDict if name.startswith("uvicorn."))
+    loggers = (
+        logging.getLogger(name)
+        for name in logging.root.manager.loggerDict
+        if name.startswith("uvicorn.")
+    )
 
     # change handler for default uvicorn logger
     intercept_handler = InterceptHandler()
 
     for uvicorn_logger in loggers:
         try:
             uvicorn_logger.handlers = [intercept_handler]
         except:
             pass
     # logging.getLogger().handlers = [intercept_handler]
     logging.getLogger("uvicorn").handlers = []
     logging.getLogger("rocketry").handlers = []
 
     # set logs output, level and format
-    logger.configure(handlers=[{"sink": sys.stdout, "level": logging.INFO, "format": format_record}])
+    logger.configure(
+        handlers=[{"sink": sys.stdout, "level": logging.INFO, "format": format_record}]
+    )
```

### Comparing `msaBase-0.0.83/msaBase/profiler.py` & `msaBase-0.0.9/msaBase/profiler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,56 @@
 # -*- coding: utf-8 -*-
 import codecs
+import time
 from typing import Dict, Optional
 
-from msaBase.configurate import MSAApp
 from pyinstrument import Profiler
-from starlette.responses import HTMLResponse
+from starlette.routing import Router
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
 
 
 class MSAProfilerMiddleware:
     """PyInstrument Profiler as Middleware
 
     Used to create an HTML from the Profiler result if enabled in the MSAServiceDefinition instance.
 
-    Parameters:
-        msa_app: Instance of the MSAApp
-        profiler_interval: 0.0001
-        profiler_output_type: "text" or "html" should be html if Admin Site Profiler Page should be used.
-        track_each_request: True, Tracks each single request and profiles it immediatly, if off then profiler
-        creates result during shutdown event.
+    Args:
+        msa_app: Optional[Router] = None, Instance of the MSAApp
+        profiler_interval: float = 0.0001,
+        profiler_output_type: str = "html", ``text`` or ``html``should be html if Admin Site Profiler Page should be used.
+        track_each_request: bool = True, Tracks each single request and profiles it immediatly, if off then profiler creates result while shutdwon event.
         **profiler_kwargs: other pyinstrument args like 'html_file_name'
     """
 
     def __init__(
         self,
         app: ASGIApp,
         *,
-        msa_app: Optional[MSAApp] = None,
+        msa_app: Optional[Router] = None,
         profiler_interval: float = 0.0001,
         profiler_output_type: str = "html",
         track_each_request: bool = True,
-        **profiler_kwargs: Dict,
+        **profiler_kwargs: Dict
     ):
         self.app = app
         """Linked/Mounted MSAApp Instance"""
         self._profiler = Profiler(interval=profiler_interval)
+
         self._server_app = msa_app
         self._output_type = profiler_output_type
         self._profiler_kwargs: dict = profiler_kwargs
         self._handler_init_done: bool = False
         self._htmlfile_init_done: bool = False
         self._track_each_request: bool = track_each_request
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        """
-        Register an event handler for profiler stop
-
-        Parameters:
-            scope: event scope
-            receive: receive callable
-            send: send callable
-        """
+        """register an event handler for profiler stop"""
         if self._server_app is not None and not self._handler_init_done:
             self._handler_init_done = True
             self._server_app.add_event_handler("shutdown", self.get_profiler_result)
-            if self._server_app.settings.profiler:
-                self._server_app.add_api_route("/profiler", self.get_profiler, tags=["service"])
 
         if scope["type"] != "http":
             await self.app(scope, receive, send)
             return
         if not self._profiler.is_running:
             self._profiler.start()
 
@@ -74,51 +65,32 @@
 
         try:
             await self.app(scope, receive, wrapped_send)
         finally:
             if scope["type"] == "http":
                 if self._profiler.is_running:
                     self._profiler.stop()
+                    end = time.perf_counter()
                     if self._output_type == "html" and not self._htmlfile_init_done:
                         await self.get_profiler_result()
                     elif self._track_each_request:
                         await self.get_profiler_result()
 
-    async def get_profiler_result(self, html_file: str = "profiler.html", replace_title: str = "msaBase-Profiler"):
-        """
-        Produces the profiler result in the defined output type format, "text" or "html"
-
-        Parameters:
-            html_file: path to html file
-            replace_title: title to replace "pyinstrument" with.
-        """
+    async def get_profiler_result(
+        self, html_file: str = "profiler.html", replace_title: str = "msaBase-Profiler"
+    ):
+        """Produces the profiler result in the defined output type format, ``text`` or ``html``"""
         if self._output_type == "text":
             print(self._profiler.output_text(**self._profiler_kwargs))
         elif self._output_type == "html":
             html_name = self._profiler_kwargs.get("html_file_name")
             if html_name is None:
                 html_name = html_file
             html_code = self._profiler.output_html(
                 **self._profiler_kwargs
             )  # HTMLRenderer().render(session=self._profiler.last_session)
             if replace_title:
-                html_code = html_code.replace("pyinstrument", replace_title).replace("Pyinstrument", replace_title)
+                html_code = html_code.replace("pyinstrument", replace_title).replace(
+                    "Pyinstrument", replace_title
+                )
             with codecs.open(html_name, "w", "utf-8") as f:
                 f.write(html_code)
-            return html_code
-
-    async def get_profiler(self) -> HTMLResponse:
-        """
-        Produces the profiler result and return in the html
-
-        Returns:
-            HTMLResponse: response with html code of profiler
-        """
-
-        if self._profiler.is_running:
-            self._profiler.stop()
-        html_code = await self.get_profiler_result(
-            replace_title=f"{self._server_app.settings.name} {self._server_app.settings.version}"
-        )
-        if not self._profiler.is_running:
-            self._profiler.start()
-        return HTMLResponse(html_code)
```

### Comparing `msaBase-0.0.83/msaBase/sysinfo.py` & `msaBase-0.0.9/msaBase/sysinfo.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import datetime
 import decimal
 import os
 import re
 import socket
 import uuid
 from subprocess import getoutput
-from typing import Dict, List, Tuple
+from typing import Dict, List
 
 import GPUtil
 import psutil
+
 from msaBase.errorhandling import getMSABaseExceptionHandler
 from msaBase.models.sysinfo import (
     MSACPUFrequency,
     MSACPUStats,
     MSACPUTimes,
     MSADiskIO,
     MSAGPUInfo,
@@ -31,44 +32,41 @@
     MSASystemInfo,
     MSATemperature,
     MSATemperatures,
 )
 
 
 def get_hostname() -> str:
-    """
-    Get current host name.
+    """Get socket.gethostname()
 
     Returns:
-        hostname string
+        hostname: str
     """
     hostname: str = socket.gethostname()
     return hostname
 
 
 def get_list_partitions() -> List:
-    """
-    Get mounted partitions as a list.
+    """Get psutil.disk_partitions()
 
     Returns:
-        List of mounted partitions.
+        partitions_list: List = []
     """
     partitions_list = []
     partitions = psutil.disk_partitions()
     partitions_list = [partition[1] for partition in partitions]
 
     return partitions_list
 
 
 def get_gpus() -> List[MSAGPUInfo]:
-    """
-    Get GPU information.
+    """Get GPUtil.getGPUs()
 
     Returns:
-        List of GPUs
+        list_gpus: List[MSAGPUInfo] = []
     """
     gpus = GPUtil.getGPUs()
     list_gpus: List[MSAGPUInfo] = []
     for gpu in gpus:
         ng: MSAGPUInfo = MSAGPUInfo()
         # get the GPU id
         ng.id = gpu.id
@@ -86,19 +84,18 @@
         ng.temperature = f"{gpu.temperature} °C"
         ng.uuid = gpu.uuid
         list_gpus.append(ng)
     return list_gpus
 
 
 def get_partition_usage(partitions) -> Dict:
-    """
-    Get disc usage statistics for given partitions.
+    """Get psutil.disk_usage(partition)
 
     Returns:
-        Dictionary containing partition usage statistics info
+        ret: Dict = {"partition": list, "total": list, "used": list, "free": list, "percent": list}
     """
     lstotal = []
     lsused = []
     lsfree = []
     lspercent = []
     lspartition: List = [partition for partition in partitions]
 
@@ -118,36 +115,34 @@
         "free": lsfree,
         "percent": lspercent,
     }
     return ret
 
 
 def get_map_disk_usage() -> Dict:
-    """
-    Get reformatted disk usage info
+    """Get get_partition_usage(get_list_partitions())
 
     Returns:
-        Dictionary containing reformatted disk usage statistics info
+        rdict: Dict
     """
     MapUsage: Dict = get_partition_usage(get_list_partitions())
     disk = MapUsage["partition"]
     total = MapUsage["total"]
     used = MapUsage["used"]
     free = MapUsage["free"]
     percent = MapUsage["percent"]
     rdict = dict(zip(disk, zip(total, used, free, percent)))
     return rdict
 
 
 def get_memory_usage() -> MSAMemoryUsage:
-    """
-    Get virtual memory usage
+    """Get psutil.virtual_memory()
 
     Returns:
-        Pydantic model containing memory usage information
+        mu: MSAMemoryUsage
     """
     mu: MSAMemoryUsage = MSAMemoryUsage()
     memory = psutil.virtual_memory()
 
     mu.total = memory.total / 1024 / 1024
     mu.available = memory.available / 1024 / 1024
     mu.used = memory.used / 1024 / 1024
@@ -157,31 +152,29 @@
     mu.cached = memory.cached / 1024 / 1024
     mu.active = memory.active / 1024 / 1024
     mu.inactive = memory.inactive / 1024 / 1024
     return mu
 
 
 def get_cpu_freq() -> MSACPUFrequency:
-    """
-    Get CPU frequency information
+    """Get psutil.cpu_freq()
 
     Returns:
-        Pydantic model containing CPU frequency information
+        cpf: MSACPUFrequency
     """
     cpf: MSACPUFrequency = MSACPUFrequency()
     cpf.current, cpf.min, cpf.max = psutil.cpu_freq()
     return cpf
 
 
 def get_cpu_times() -> MSACPUTimes:
-    """
-    Get CPU timings information
+    """Get psutil.cpu_times()
 
     Returns:
-        Pydantic model containing CPU timings information
+        cti: MSACPUTimes
     """
     cti: MSACPUTimes = MSACPUTimes()
     (
         cti.user,
         cti.nice,
         cti.system,
         cti.idle,
@@ -192,36 +185,34 @@
         cti.guest,
         cti.guest_nice,
     ) = psutil.cpu_times()
     return cti
 
 
 def get_cpu_stats() -> MSACPUStats:
-    """
-    Get CPU statistics
+    """Get psutil.cpu_times()
 
     Returns:
-        Pydantic model containing CPU statistics
+        cst: MSACPUStats
     """
     cst: MSACPUStats = MSACPUStats()
     (
         cst.ctx_switches,
         cst.interrupts,
         cst.soft_interrupts,
         cst.syscalls,
     ) = psutil.cpu_stats()
     return cst
 
 
 def get_disk_io() -> MSADiskIO:
-    """
-    Get disk input/output information.
+    """Get psutil.disk_io_counters()
 
     Returns:
-        Pydantic model containing disk input/output information
+        dio: MSADiskIO
     """
     dio: MSADiskIO = MSADiskIO()
     (
         dio.read_count,
         dio.write_count,
         dio.read_bytes,
         dio.write_bytes,
@@ -231,19 +222,18 @@
         dio.write_merged_count,
         dio.busy_time,
     ) = psutil.disk_io_counters()
     return dio
 
 
 def get_network_io() -> MSANetworkIO:
-    """
-    Get network input/output information.
+    """Get psutil.net_io_counters()
 
     Returns:
-        Pydantic model containing network input/output information
+        nio: MSANetworkIO
     """
     nio: MSANetworkIO = MSANetworkIO()
     (
         nio.bytes_sent,
         nio.bytes_recv,
         nio.packets_sent,
         nio.packets_recv,
@@ -252,19 +242,18 @@
         nio.dropin,
         nio.dropout,
     ) = psutil.net_io_counters()
     return nio
 
 
 def get_network_adapters() -> List[MSANetworkAdapters]:
-    """
-    Get the addresses associated to each NIC (network interface card)
+    """Get psutil.net_if_addrs()
 
     Returns:
-        List of Network Adapters List models
+        ret: List[MSANetworkAdapters] = []
     """
     ret: List[MSANetworkAdapters] = []
     la: Dict = psutil.net_if_addrs()
 
     for key, val in la.items():
         na: MSANetworkAdapters = MSANetworkAdapters()
         na.name = key
@@ -277,19 +266,18 @@
             la_entry.ptp = entry[4]
             na.adapters.append(la_entry)
         ret.append(na)
     return ret
 
 
 def get_temperatures() -> List[MSATemperatures]:
-    """
-    Get hardware temperatures.
+    """Get psutil.sensors_temperatures()
 
     Returns:
-        List of models containing temperature information.
+        ret: List[MSATemperatures] = []
     """
     ret: List[MSATemperatures] = []
     ta: Dict = psutil.sensors_temperatures()
     for key, val in ta.items():
         tp: MSATemperatures = MSATemperatures()
         tp.device = key
         for entry in val:
@@ -300,19 +288,18 @@
             tp_entry.critical = entry[3]
             tp.temps.append(tp_entry)
         ret.append(tp)
     return ret
 
 
 def get_network_stats() -> List[MSANetworkStats]:
-    """
-    Get information about each NIC (network interface card)
+    """Get psutil.net_if_stats()
 
     Returns:
-        List of models containing network statistics information.
+        ret: List[MSANetworkStats] = []
     """
     ret: List[MSANetworkStats] = []
     net_stats: Dict = psutil.net_if_stats()
     for key, entry in net_stats.items():
         ns: MSANetworkStats = MSANetworkStats()
         ns.name = key
         ns_entry: MSANetworkStat = MSANetworkStat()
@@ -322,19 +309,18 @@
         ns_entry.mtu = entry[3]
         ns.adapters.append(ns_entry)
         ret.append(ns)
     return ret
 
 
 def get_network_connections() -> List[MSANetworkConnection]:
-    """
-    Get system-wide socket connections as a list
+    """Get psutil.net_connections()
 
     Returns:
-        List of models containing network connections information.
+        rlist: List[MSANetworkConnection] = []
     """
     rlist: List[MSANetworkConnection] = []
     inlist = psutil.net_connections()
     for xi, entry in enumerate(inlist):
         nc: MSANetworkConnection = MSANetworkConnection()
         nc.index = xi
         nc.file_descriptor = entry[0]
@@ -347,98 +333,100 @@
         nc.status = entry[5]
         nc.pid = entry[6]
         rlist.append(nc)
     return rlist
 
 
 def get_swap() -> MSASwap:
-    """
-    Get system swap memory statistics.
+    """Get psutil.swap_memory()
 
     Returns:
-        Pydantic model containing system swap memory information
+        sw: MSASwap
     """
     swap = psutil.swap_memory()
     sw: MSASwap = MSASwap()
     sw.total = swap.total / 1024 / 1024
     sw.used = swap.used / 1024 / 1024
     sw.free = swap.free / 1024 / 1024
     sw.percent = swap.percent
     return sw
 
 
 def get_load_average() -> List[float]:
-    """
-    Returns the CPU load average in tuple[1min, 5min, 15min].
+    """Returns the CPU load average in tuple[1min, 5min, 15min].
 
     Returns:
         1min: total usage
         5min: largest process usage
         15min: name of the largest process
 
     """
     return [x / psutil.cpu_count() * 100 for x in psutil.getloadavg()]
 
 
-def get_cpu_usage(user: str = None, ignore_self: bool = False) -> Tuple[int, int, str]:
-    """
-    Returns the total CPU usage for all available cores.
+def get_cpu_usage(user: str = None, ignore_self: bool = False) -> tuple[int, int, str]:
+    """Returns the total CPU usage for all available cores.
 
-    Parameters:
+    Args:
         user: If given, returns only the total CPU usage of all processes for the given user.
         ignore_self: If ``True`` the process that runs this script will be ignored.
 
     Returns:
         total: total usage
         largest_process: largest process usage
         largest_process_name: name of the largest process
+
     """
     pid = os.getpid()
     cmd = "ps aux"
     output = getoutput(cmd)
     total: int = 0
     largest_process = 0
-    largest_process_name = ""
+    largest_process_name = None
     for row in output.split("\n")[1:]:
         erow: List = row.split()
         if erow[1] == str(pid) and ignore_self:
             continue
         if user is None or user == erow[0]:
             cpu = decimal.Decimal(erow[2])
             if cpu > total:
                 largest_process = cpu
                 largest_process_name = " ".join(erow[10 : len(erow)])
             total += decimal.Decimal(erow[2])
     return total, largest_process, largest_process_name
 
 
-def get_sysinfo(version: str) -> MSASystemInfo:
-    """
-    Get system information.
-
+def get_sysinfo() -> MSASystemInfo:
+    """Get MSASystemInfo
     Returns:
-        Pydantic System Info Model.
+        system_info: Pydantic System Info Model.
+
     """
     system_info: MSASystemInfo = MSASystemInfo()
     try:
-        system_info.Version = version
         system_info.OS_Name = os.uname().sysname
         system_info.Node_Name = os.uname().nodename
         system_info.Host_Name = get_hostname()
         system_info.OS_Release = os.uname().release
         system_info.OS_Version = os.uname().version
         system_info.HW_Identifier = os.uname().machine
         system_info.CPU_Physical = psutil.cpu_count(logical=False)
         system_info.CPU_Logical = os.cpu_count()
-        system_info.Memory_Physical = str(round(psutil.virtual_memory().total / 1024000000.0, 2)) + " GB"
-        system_info.Memory_Available = str(round(psutil.virtual_memory().available / 1024000000.0, 2)) + " GB"
-        system_info.System_Boot = datetime.datetime.fromtimestamp(psutil.boot_time()).strftime("%Y-%m-%d %H:%M:%S")
-        system_info.Service_Start = datetime.datetime.fromtimestamp(psutil.Process().create_time()).strftime(
-            "%Y-%m-%d %H:%M:%S"
+        system_info.Memory_Physical = (
+            str(round(psutil.virtual_memory().total / 1024000000.0, 2)) + " GB"
         )
+        system_info.Memory_Available = (
+            str(round(psutil.virtual_memory().available / 1024000000.0, 2)) + " GB"
+        )
+        system_info.System_Boot = datetime.datetime.fromtimestamp(
+            psutil.boot_time()
+        ).strftime("%Y-%m-%d %H:%M:%S")
+        system_info.Service_Start = datetime.datetime.fromtimestamp(
+            psutil.Process().create_time()
+        ).strftime("%Y-%m-%d %H:%M:%S")
         system_info.Runtime_Exe = psutil.Process().exe()
         system_info.Runtime_Cmd = psutil.Process().cmdline()
         system_info.PID = psutil.Process().pid
         system_info.CPU_Current = psutil.Process().cpu_num()
         system_info.Disk_IO = get_disk_io()
         system_info.Network_IO = get_network_io()
         system_info.CPU_Times = get_cpu_times()
@@ -463,43 +451,48 @@
 
     except Exception as e:
         getMSABaseExceptionHandler().handle(e, "Error: Get System Information:")
 
     return system_info
 
 
-def get_sysgpuinfo(version: str) -> MSASystemGPUInfo:
-    """
-    Get GPU information
-
+def get_sysgpuinfo() -> MSASystemGPUInfo:
+    """Get MSASystemGPUInfo
     Returns:
-        Pydantic model containing GPU information
+        system_gpu_info: Pydantic System GPU Info Model.
     """
     system_gpu_info: MSASystemGPUInfo = MSASystemGPUInfo()
     try:
-        system_gpu_info.Version = version
         system_gpu_info.OS_Name = os.uname().sysname
         system_gpu_info.Node_Name = os.uname().nodename
         system_gpu_info.Host_Name = get_hostname()
         system_gpu_info.OS_Release = os.uname().release
         system_gpu_info.OS_Version = os.uname().version
         system_gpu_info.HW_Identifier = os.uname().machine
         system_gpu_info.CPU_Physical = psutil.cpu_count(logical=False)
         system_gpu_info.CPU_Logical = os.cpu_count()
-        system_gpu_info.Memory_Physical = str(round(psutil.virtual_memory().total / 1024000000.0, 2)) + " GB"
-        system_gpu_info.Memory_Available = str(round(psutil.virtual_memory().available / 1024000000.0, 2)) + " GB"
-        system_gpu_info.System_Boot = datetime.datetime.fromtimestamp(psutil.boot_time()).strftime("%Y-%m-%d %H:%M:%S")
-        system_gpu_info.Service_Start = datetime.datetime.fromtimestamp(psutil.Process().create_time()).strftime(
-            "%Y-%m-%d %H:%M:%S"
+        system_gpu_info.Memory_Physical = (
+            str(round(psutil.virtual_memory().total / 1024000000.0, 2)) + " GB"
+        )
+        system_gpu_info.Memory_Available = (
+            str(round(psutil.virtual_memory().available / 1024000000.0, 2)) + " GB"
         )
+        system_gpu_info.System_Boot = datetime.datetime.fromtimestamp(
+            psutil.boot_time()
+        ).strftime("%Y-%m-%d %H:%M:%S")
+        system_gpu_info.Service_Start = datetime.datetime.fromtimestamp(
+            psutil.Process().create_time()
+        ).strftime("%Y-%m-%d %H:%M:%S")
         system_gpu_info.Runtime_Exe = psutil.Process().exe()
         system_gpu_info.Runtime_Cmd = psutil.Process().cmdline()
         system_gpu_info.Runtime_Status = psutil.Process().status()
         system_gpu_info.PID = psutil.Process().pid
         system_gpu_info.GPUs = get_gpus()
         system_gpu_info.IP_Address = socket.gethostbyname(socket.gethostname())
-        system_gpu_info.MAC_Address = ":".join(re.findall("..", "%012x" % uuid.getnode()))
+        system_gpu_info.MAC_Address = ":".join(
+            re.findall("..", "%012x" % uuid.getnode())
+        )
 
     except Exception as e:
         getMSABaseExceptionHandler().handle(e, "Error: Get System GPU Information:")
 
     return system_gpu_info
```

### Comparing `msaBase-0.0.83/msaBase.egg-info/PKG-INFO` & `msaBase-0.0.9/msaBase.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: msaBase
-Version: 0.0.83
+Version: 0.0.9
 Summary: msaBase - General package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo, Healtcheck, Error Handling etc.
 Home-page: https://github.com/u2d-ai/msaBase
-Download-URL: http://pypi.python.org/pypi/msaBase
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
+Download-URL: http://pypi.python.org/pypi/msaBase
 Project-URL: Documentation, http://msaBase.u2d.ai/
 Project-URL: Source, https://github.com/u2d-ai/msaBase
 Project-URL: Tracker, https://github.com/u2d-ai/msaBase/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -92,7 +93,9 @@
 Build:  
 
     python setup.py sdist
 
 Publish to pypi:
 
     twine upload dist/*
+
+
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: msaBase Version: 0.0.83 Summary: msaBase - General
+Metadata-Version: 2.1 Name: msaBase Version: 0.0.9 Summary: msaBase - General
 package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo,
 Healtcheck, Error Handling etc. Home-page: https://github.com/u2d-ai/msaBase
-Download-URL: http://pypi.python.org/pypi/msaBase Author: Stefan Welcker
-Author-email: stefan@u2d.ai License: MIT Project-URL: Documentation, http://
+Author: Stefan Welcker Author-email: stefan@u2d.ai License: MIT Download-URL:
+http://pypi.python.org/pypi/msaBase Project-URL: Documentation, http://
 msaBase.u2d.ai/ Project-URL: Source, https://github.com/u2d-ai/msaBase Project-
-URL: Tracker, https://github.com/u2d-ai/msaBase/issues Classifier: Development
-Status :: 4 - Beta Classifier: Framework :: FastAPI Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Database Classifier: Topic ::
-Database :: Front-Ends Classifier: Topic :: Documentation Classifier: Topic ::
-Internet :: WWW/HTTP :: WSGI :: Server Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Description-Content-Type: text/markdown License-File: LICENCE
+URL: Tracker, https://github.com/u2d-ai/msaBase/issues Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta Classifier: Framework :: FastAPI
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: MacOS :: MacOS X Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+:: Linux Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Database
+Classifier: Topic :: Database :: Front-Ends Classifier: Topic :: Documentation
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server Classifier: Topic
+:: Software Development :: Libraries Classifier: Topic :: Software Development
+:: Libraries :: Python Modules Description-Content-Type: text/markdown License-
+File: LICENCE
  > msaBase- General Package for Microservices based on FastAPI like Profiler,
              Scheduler, Sysinfo, Healtcheck, Error Handling etc.
                    Optimized for use with FastAPI/Pydantic.
                  [Package_version] [Supported_Python_versions]
 ------ **Documentation**: Documentation_(https://msaBase.u2d.ai/) ------ ##
 Features - **MSABaseExceptionHandler**: Central exception handler which sends
 formatted exception to logger - **Filehandler utilities**: Classes for
```

### Comparing `msaBase-0.0.83/msaBase.egg-info/SOURCES.txt` & `msaBase-0.0.9/msaBase.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 msaBase/config.py
 msaBase/configurate.py
 msaBase/errorhandling.py
 msaBase/healthcheck.py
 msaBase/helpers.py
 msaBase/logger.py
 msaBase/profiler.py
+msaBase/router.py
 msaBase/sysinfo.py
 msaBase.egg-info/PKG-INFO
 msaBase.egg-info/SOURCES.txt
 msaBase.egg-info/dependency_links.txt
 msaBase.egg-info/requires.txt
 msaBase.egg-info/top_level.txt
 msaBase.egg-info/zip-safe
 msaBase/models/__init__.py
 msaBase/models/functionality.py
 msaBase/models/middlewares.py
 msaBase/models/settings.py
-msaBase/models/sysinfo.py
-msaBase/utils/__init__.py
-msaBase/utils/constants.py
+msaBase/models/sysinfo.py
```

### Comparing `msaBase-0.0.83/requirements.txt` & `msaBase-0.0.9/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 # MSA Dependencies
-msaFileSystem==0.0.3 # Agnostic Abstract Filesystem API which allows to use S3, GCS, Azure Datalake, your local FS, Youtube etc Optimized for use with FastAPI/Pydantic.
-msaDocModels==0.0.78 # MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and AI results for processed documents
+msaCRUD>=0.0.1 # SQLModel/SQLAlchemy/FastAPI - DB Object CRUD/API Automation
+msaFileSystem>=0.0.1 # Agnostic Abstract Filesystem API which allows to use S3, GCS, Azure Datalake, your local FS, Youtube etc Optimized for use with FastAPI/Pydantic.
+msaDocModels>=0.0.8 # MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and AI results for processed documents
 
 # FastAPI related Dependencies
-fastapi[all]==0.86.0 # FastAPI framework, high performance, easy to learn, fast to code, ready for production
-fastapi_utils==0.2.1 # Reusable utilities for FastAPI, Repeated Tasks, APIModel, APISettings
-pydantic[email,dotenv]==1.9.2 # Data validation and settings management using python type hints
-pyinstrument==4.4.0 # pyinstrument to check service performance.
+fastapi[all]>=0.85.0 # FastAPI framework, high performance, easy to learn, fast to code, ready for production
+fastapi_utils>=0.2.1 # Reusable utilities for FastAPI, Repeated Tasks, APIModel, APISettings
+pydantic[email,dotenv]~=1.9.2 # Data validation and settings management using python type hints
+pyinstrument>=4.3.0 # pyinstrument to check service performance.
 
 
+# GraphQL related Dependencies
+strawberry-graphql>=0.130.4 #A library for creating GraphQL APIs
+strawberry-graphql[fastapi]>=0.130.4 # Strawberry provides support for FastAPI with a custom APIRouter called GraphQLRouter.
+
 # General Dependencies
-autoflake==2.0.1 # Removes unused imports and unused variables
-black==22.6.0 # Code formatter
-pyproject-flake8==6.0.0 # configure flake8
-flake8==6.0.0 # modular source code checker: pep8 pyflakes and co
-colorama==0.4.6 # Makes ANSI escape character sequence
-isort==5.12.0 # library to sort Python imports.
-sentry-sdk==1.24.0 # library to automatic reporting of errors and exceptions.
-loguru==0.6.0 # Python logging made (stupidly) simple
-lxml==4.9.2 # Powerful and Pythonic XML processing library combining libxml2/libxslt with the ElementTree API.
-mypy==1.0.0 # Optional static typing for Python
-setuptools==67.6.1 # Easily download, build, install, upgrade, and uninstall Python packages
-prometheus_fastapi_instrumentator==5.9.1 # Instrument your FastAPI with Prometheus metrics
-Jinja2==3.1.2 # A very fast and expressive template engine.
-orjson==3.8.3 # Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy
-pyinstrument==4.4.0 # pyinstrument to check service performance.
-msgpack-asgi==1.1.0 # Drop-in MessagePack support for ASGI applications and frameworks
-slowapi==0.1.7 # A rate limiting extension for Starlette and Fastapi
-addict==2.4.0 # A dictionary whose items can be set using both attribute and item syntax.
-pymongo==4.3.3 # A Python distribution containing tools for working with MongoDB
+autoflake>=1.6.1 # Removes unused imports and unused variables
+black>=22.8.0 # Code formatter
+pyproject-flake8>=5.0.4 # configure flake8
+flake8>=5.0.4 # modular source code checker: pep8 pyflakes and co
+isort>=5.10.1 # library to sort Python imports.
+loguru>=0.6.0 # Python logging made (stupidly) simple
+lxml>=4.9.1 # Powerful and Pythonic XML processing library combining libxml2/libxslt with the ElementTree API.
+mypy>=0.971 # Optional static typing for Python
+setuptools>=65.2.0 # Easily download, build, install, upgrade, and uninstall Python packages
+prometheus_fastapi_instrumentator>=5.9.1 # Instrument your FastAPI with Prometheus metrics
+Jinja2>=3.1.2 # A very fast and expressive template engine.
+orjson>=3.8.0 # Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy
+pyinstrument>=4.3.0 # pyinstrument to check service performance.
+msgpack-asgi>=1.1.0 # Drop-in MessagePack support for ASGI applications and frameworks
+slowapi>=0.1.6 # A rate limiting extension for Starlette and Fastapi
+addict>=2.4.0 # A dictionary whose items can be set using both attribute and item syntax.
 
 # Dapr Dependencies
-dapr==1.9.0 # Dapr is a portable, serverless, event-driven runtime that makes it easy for developers to build resilient, stateless and stateful microservices that run on the cloud and edge
-dapr-ext-grpc==1.9.0 # gRPC extension for Dapr.
-dapr-ext-fastapi==1.9.0 # Dapr is a portable, serverless, event-driven runtime
+dapr~=1.7.0 # Dapr is a portable, serverless, event-driven runtime that makes it easy for developers to build resilient, stateless and stateful microservices that run on the cloud and edge
+dapr-ext-grpc~=1.7.0 # gRPC extension for Dapr.
+dapr-ext-fastapi~=1.7.0 # Dapr is a portable, serverless, event-driven runtime
 
 # File Management related libs
-aiofiles==23.1.0 # handling local disk files in asyncio applications
-fs==2.4.16 # Python's filesystem abstraction layer
+aiofiles>=22.1.0 # handling local disk files in asyncio applications
+fs>=2.4.16 # Python's filesystem abstraction layer
 
 # Starlette related Dependencies
-starlette==0.20.4 # Starlette is a lightweight ASGI framework/toolkit, which is ideal for building async web services in Python.
-starlette-context==0.3.5 # Access context in Starlette
-starception==0.4.1 # Beautiful debugging page for Starlette apps.
-Starlette-WTF==0.4.3 # Simple integration of Starlette and WTForms.
+starlette~=0.20.4 # Starlette is a lightweight ASGI framework/toolkit, which is ideal for building async web services in Python.
+starlette-context~=0.3.4 # Access context in Starlette
+starception~=0.4.0 # Beautiful debugging page for Starlette apps.
+Starlette-WTF~=0.4.3 # Simple integration of Starlette and WTForms.
+
+# SQL/No-SQL/DB related Dependencies
+aiosqlite>=0.17.0 # asyncio bridge to the standard sqlite3 module
+aioredis>=2.0.1 # asyncio (PEP 3156) Redis support
+sqlmodel>=0.0.8 # SQLModel, SQL databases in Python, designed for simplicity, compatibility, and robustness.
+sqlalchemy[asyncio]>=1.4.41 # Database Abstraction Library
+sqlalchemy_database>=0.0.7 # SQLAlchemy-Database provides shortcut functions to common database operations for SQLAlchemy ORM
+tinydb>=4.7.0 # TinyDB is a tiny, document oriented database
 
 # Other Dependencies
-httpx==0.23.3 # The next generation HTTP client.
-aiohttp==3.8.4 # The next generation HTTP client.
-hjson==3.1.0 # Hjson, a user interface for JSON.
+httpx~=0.23.0 # The next generation HTTP client.
+aiohttp>=3.8.3 # The next generation HTTP client.
+hjson~=3.1.0 # Hjson, a user interface for JSON.
 
 # Uvicorn related Dependencies
-uvicorn==0.18.3 # The lightning-fast ASGI server.
-uvloop==0.17.0 # Fast implementation of asyncio event loop on top of libuv
+uvicorn~=0.18.3 # The lightning-fast ASGI server.
+uvloop~=0.17.0 # Fast implementation of asyncio event loop on top of libuv
 
 # Sysinfo related libs
-gputil==1.4.0 # Python module for getting the GPU status from NVIDA GPUs using nvidia-smi.
-psutil==5.9.4 # Cross-platform lib for process and system monitoring in Python.
+gputil>=1.4.0 # Python module for getting the GPU status from NVIDA GPUs using nvidia-smi.
+psutil>=5.9.2 # Cross-platform lib for process and system monitoring in Python.
 
 # Scheduler
-apscheduler==3.10.0 # APScheduler is a Python library that lets you schedule your Python code to be executed later, either just once or periodically
+apscheduler>=3.9.1 # APScheduler is a Python library that lets you schedule your Python code to be executed later, either just once or periodically
 
 # Testing
-pytest==7.2.0 # Framework makes it easy to write small tests, yet scales to support complex functional testing for applications and libraries.
-pytest-asyncio==0.20.2 # Library for testing asyncio code with pytest.
-pytest-mock==3.10.0 # Library for mock data with pytest.
+pytest>=7.2.0 # Framework makes it easy to write small tests, yet scales to support complex functional testing for applications and libraries.
```

### Comparing `msaBase-0.0.83/setup.py` & `msaBase-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 import pathlib
 
 from pkg_resources import parse_requirements
 from setuptools import find_packages, setup
 
 with pathlib.Path("requirements.txt").open() as requirements_txt:
-    REQUIREMETS = [str(requirement) for requirement in parse_requirements(requirements_txt)]
+    REQUIREMETS = [
+        str(requirement) for requirement in parse_requirements(requirements_txt)
+    ]
 
 
 # Parse version number from pyglet/__init__.py:
 with open("msaBase/__init__.py") as f:
     info = {}
     for line in f:
         if line.startswith("version"):
@@ -24,16 +26,15 @@
     url="https://github.com/u2d-ai/msaBase",
     download_url="http://pypi.python.org/pypi/msaBase",
     project_urls={
         "Documentation": "http://msaBase.u2d.ai/",
         "Source": "https://github.com/u2d-ai/msaBase",
         "Tracker": "https://github.com/u2d-ai/msaBase/issues",
     },
-    description="msaBase - General package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo, "
-    "Healtcheck, Error Handling etc.",
+    description="msaBase - General package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo, Healtcheck, Error Handling etc.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: FastAPI",
         "Intended Audience :: Developers",
```

