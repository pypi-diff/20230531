# Comparing `tmp/fresco-3.3.1.tar.gz` & `tmp/fresco-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fresco-3.3.1.tar", last modified: Thu May 18 12:04:33 2023, max compression
+gzip compressed data, was "fresco-3.3.2.tar", last modified: Wed May 31 12:10:01 2023, max compression
```

## Comparing `fresco-3.3.1.tar` & `fresco-3.3.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.167537 fresco-3.3.1/
--rw-r--r--   0 oliver    (1001) wheel        (0)    20745 2023-05-18 12:01:48.000000 fresco-3.3.1/CHANGELOG.rst
--rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-05-18 12:01:48.000000 fresco-3.3.1/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       50 2023-05-18 12:01:48.000000 fresco-3.3.1/MANIFEST.in
--rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-18 12:04:33.167646 fresco-3.3.1/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      822 2023-05-18 12:01:48.000000 fresco-3.3.1/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.159011 fresco-3.3.1/fresco/
--rw-r--r--   0 oliver    (1001) wheel        (0)     3520 2023-05-18 12:04:31.000000 fresco-3.3.1/fresco/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7055 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/cookie.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    26615 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/core.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3232 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/decorators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4410 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4173 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/middleware.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    13362 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/multidict.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    13614 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/options.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    27071 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/request.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3504 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/requestcontext.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    37078 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/response.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10176 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/routeargs.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    58670 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/routing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2513 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/static.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    11081 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/subrequests.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.163318 fresco-3.3.1/fresco/tests/
--rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1871 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/fixtures.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2171 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_cookie.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    34019 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_core.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1480 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_decorators.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      973 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3137 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_middleware.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7565 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_multidict.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10868 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_options.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    16389 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_request.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3115 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_requestcontext.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8934 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_response.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8162 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_routeargs.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    37207 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_routing.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4686 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_static.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7909 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/test_subrequests.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.164807 fresco-3.3.1/fresco/tests/util/
--rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10570 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/form_data.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1117 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_common.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10803 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_http.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1492 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_security.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7643 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_urls.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3038 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/tests/util/test_wsgi.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      106 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/types.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      347 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/typing.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.167353 fresco-3.3.1/fresco/util/
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1609 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/cache.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1258 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/common.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     5484 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/contentencodings.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1383 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/file.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    22175 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/http.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1289 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/io.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      370 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/object.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1058 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/security.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2309 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/textproc.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9195 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/urls.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    12970 2023-05-18 12:01:48.000000 fresco-3.3.1/fresco/util/wsgi.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-18 12:04:33.159850 fresco-3.3.1/fresco.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-18 12:04:32.000000 fresco-3.3.1/fresco.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)     1476 2023-05-18 12:04:32.000000 fresco-3.3.1/fresco.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-05-18 12:04:32.000000 fresco-3.3.1/fresco.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-18 12:04:32.000000 fresco-3.3.1/fresco.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      795 2023-05-18 12:04:33.168250 fresco-3.3.1/setup.cfg
--rw-r--r--   0 oliver    (1001) wheel        (0)      634 2023-05-18 12:01:48.000000 fresco-3.3.1/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-31 12:10:01.544895 fresco-3.3.2/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    20934 2023-05-31 12:07:22.000000 fresco-3.3.2/CHANGELOG.rst
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11358 2023-05-31 12:07:21.000000 fresco-3.3.2/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       50 2023-05-31 12:07:21.000000 fresco-3.3.2/MANIFEST.in
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-31 12:10:01.545008 fresco-3.3.2/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      822 2023-05-31 12:07:21.000000 fresco-3.3.2/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-31 12:10:01.525683 fresco-3.3.2/fresco/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3520 2023-05-31 12:09:58.000000 fresco-3.3.2/fresco/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7055 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/cookie.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    26615 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/core.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3232 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/decorators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4410 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4173 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/middleware.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13362 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/multidict.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    13614 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/options.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    27071 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/request.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3504 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/requestcontext.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    37078 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/response.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10176 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/routeargs.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    58721 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/routing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2513 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/static.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    11081 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/subrequests.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-31 12:10:01.529940 fresco-3.3.2/fresco/tests/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1871 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/fixtures.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2171 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_cookie.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    34019 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_core.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1480 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_decorators.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      973 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3137 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_middleware.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7565 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_multidict.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10868 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_options.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    16389 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_request.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3115 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_requestcontext.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8934 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_response.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8162 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_routeargs.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    37890 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_routing.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4686 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_static.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7909 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/test_subrequests.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-31 12:10:01.531429 fresco-3.3.2/fresco/tests/util/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        0 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/util/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10570 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/util/form_data.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1117 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/util/test_common.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10803 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/util/test_http.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1492 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/util/test_security.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7643 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/util/test_urls.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3038 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/tests/util/test_wsgi.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      106 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/types.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      347 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/typing.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-31 12:10:01.544705 fresco-3.3.2/fresco/util/
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1609 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/cache.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1258 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/common.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     5484 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/contentencodings.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1383 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/file.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    22175 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/http.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1289 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/io.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      370 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/object.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1058 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/security.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2309 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/textproc.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9195 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/urls.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    12970 2023-05-31 12:07:21.000000 fresco-3.3.2/fresco/util/wsgi.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2023-05-31 12:10:01.526517 fresco-3.3.2/fresco.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1575 2023-05-31 12:10:01.000000 fresco-3.3.2/fresco.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1476 2023-05-31 12:10:01.000000 fresco-3.3.2/fresco.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2023-05-31 12:10:01.000000 fresco-3.3.2/fresco.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2023-05-31 12:10:01.000000 fresco-3.3.2/fresco.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      795 2023-05-31 12:10:01.545608 fresco-3.3.2/setup.cfg
+-rw-r--r--   0 oliver    (1001) wheel        (0)      634 2023-05-31 12:07:21.000000 fresco-3.3.2/setup.py
```

### Comparing `fresco-3.3.1/CHANGELOG.rst` & `fresco-3.3.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+3.3.2 (released 2023-05-31)
+---------------------------
+- Bugfix: a fresco app routed through route_wsgi now receives a fresh request
+  and environ dict, isolated from the containing app.
+
 3.3.1 (released 2023-05-18)
 ---------------------------
 
 - The ``route_wsgi`` and ``route_all`` methods now only match at a
   path separator boundary (``'/'``).
 - Bugfix: subrequest now works with views routed via ``RRoute`` (and so expect
   an initial ``request`` argument)
```

### Comparing `fresco-3.3.1/LICENSE.txt` & `fresco-3.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/PKG-INFO` & `fresco-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresco
-Version: 3.3.1
+Version: 3.3.2
 Summary: A Web/WSGI micro-framework
 Home-page: https://ollycope.com/software/fresco/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi web www framework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fresco-3.3.1/README.rst` & `fresco-3.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/__init__.py` & `fresco-3.3.2/fresco/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #     Unless required by applicable law or agreed to in writing, software
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
-__version__ = "3.3.1"
+__version__ = "3.3.2"
 
 DEFAULT_CHARSET = "UTF-8"
 
 __all__ = [
     "Request",
     "currentrequest",
     "context",
```

### Comparing `fresco-3.3.1/fresco/cookie.py` & `fresco-3.3.2/fresco/cookie.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/core.py` & `fresco-3.3.2/fresco/core.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/decorators.py` & `fresco-3.3.2/fresco/decorators.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/exceptions.py` & `fresco-3.3.2/fresco/exceptions.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/middleware.py` & `fresco-3.3.2/fresco/middleware.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/multidict.py` & `fresco-3.3.2/fresco/multidict.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/options.py` & `fresco-3.3.2/fresco/options.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/request.py` & `fresco-3.3.2/fresco/request.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/requestcontext.py` & `fresco-3.3.2/fresco/requestcontext.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/response.py` & `fresco-3.3.2/fresco/response.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/routeargs.py` & `fresco-3.3.2/fresco/routeargs.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/routing.py` & `fresco-3.3.2/fresco/routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1604,14 +1604,15 @@
             shift_script_name = rewrite_script_name and not (
                 path == "/" and ws_SCRIPT_NAME == ""
             )
             if shift_script_name:
                 if ws_path is None:
                     ws_path = path.encode(request.charset).decode("ISO-8859-1")
                 environ = environ.copy()
+                del environ[request.STATE_ENV_KEY]
                 environ["SCRIPT_NAME"] = ws_SCRIPT_NAME + ws_path
                 environ["PATH_INFO"] = environ["PATH_INFO"][len(ws_path) :]
 
             if resolved_wsgi_app is None:
                 if isinstance(wsgiapp, str):
                     if "." in wsgiapp:
                         mod_name, attr_name = wsgiapp.rsplit(".", 1)
```

### Comparing `fresco-3.3.1/fresco/static.py` & `fresco-3.3.2/fresco/static.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/subrequests.py` & `fresco-3.3.2/fresco/subrequests.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/fixtures.py` & `fresco-3.3.2/fresco/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_cookie.py` & `fresco-3.3.2/fresco/tests/test_cookie.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_core.py` & `fresco-3.3.2/fresco/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_decorators.py` & `fresco-3.3.2/fresco/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_exceptions.py` & `fresco-3.3.2/fresco/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_middleware.py` & `fresco-3.3.2/fresco/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_multidict.py` & `fresco-3.3.2/fresco/tests/test_multidict.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_options.py` & `fresco-3.3.2/fresco/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_request.py` & `fresco-3.3.2/fresco/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_requestcontext.py` & `fresco-3.3.2/fresco/tests/test_requestcontext.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_response.py` & `fresco-3.3.2/fresco/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_routeargs.py` & `fresco-3.3.2/fresco/tests/test_routeargs.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_routing.py` & `fresco-3.3.2/fresco/tests/test_routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 #     distributed under the License is distributed on an "AS IS" BASIS,
 #     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #     See the License for the specific language governing permissions and
 #     limitations under the License.
 #
 from copy import copy
 from functools import wraps
-
+from functools import partial
 from unittest.mock import Mock, call
+import typing as t
+
 import pytest
 import tms
 
 from fresco import FrescoApp
 from fresco.core import urlfor
 from fresco.exceptions import NotFound
 from fresco.response import Response
@@ -604,14 +606,30 @@
     def test_it_routes_to_a_wsgi_app_by_dotted_path(self):
         app = FrescoApp()
         app.route_wsgi("/", "fresco.tests.fixtures.wsgi_app")
         with app.requestcontext("/"):
             response = app.view()
         assert list(response.content_iterator) == [b"ok"]
 
+    def test_it_isolates_request_for_wsgi_app(self):
+
+        params: t.Dict[str, t.Any] = {}
+        outerapp = FrescoApp()
+        innerapp = FrescoApp()
+        innerapp.route("/y", GET=Response)
+        outerapp.route_wsgi("/x", innerapp)
+
+        innerapp.process_request(partial(params.__setitem__, 'inner_request'))
+        outerapp.process_request(partial(params.__setitem__, 'outer_request'))
+
+        with outerapp.requestcontext("/x/y"):
+            outerapp.view()
+        assert params["inner_request"] is not params["outer_request"]
+        assert params["inner_request"].environ is not params["outer_request"].environ
+
     def test_fallthrough_can_be_applied_to_collection(self):
         a = Route("/fee", GET=lambda: Response(status=204))
         a = Route("/fie", GET=lambda: Response(status=204))
         b = Route("/foe", GET=lambda: Response(status=204))
         rc = RouteCollection([a, b])
         rc = rc.fallthrough_on(["204"])
         assert all(r.fallthrough_statuses == {204} for r in rc.__routes__)
```

### Comparing `fresco-3.3.1/fresco/tests/test_static.py` & `fresco-3.3.2/fresco/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/test_subrequests.py` & `fresco-3.3.2/fresco/tests/test_subrequests.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/util/form_data.py` & `fresco-3.3.2/fresco/tests/util/form_data.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/util/test_common.py` & `fresco-3.3.2/fresco/tests/util/test_common.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/util/test_http.py` & `fresco-3.3.2/fresco/tests/util/test_http.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/util/test_security.py` & `fresco-3.3.2/fresco/tests/util/test_security.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/util/test_urls.py` & `fresco-3.3.2/fresco/tests/util/test_urls.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/tests/util/test_wsgi.py` & `fresco-3.3.2/fresco/tests/util/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/cache.py` & `fresco-3.3.2/fresco/util/cache.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/common.py` & `fresco-3.3.2/fresco/util/common.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/contentencodings.py` & `fresco-3.3.2/fresco/util/contentencodings.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/file.py` & `fresco-3.3.2/fresco/util/file.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/http.py` & `fresco-3.3.2/fresco/util/http.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/io.py` & `fresco-3.3.2/fresco/util/io.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/security.py` & `fresco-3.3.2/fresco/util/security.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/textproc.py` & `fresco-3.3.2/fresco/util/textproc.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/urls.py` & `fresco-3.3.2/fresco/util/urls.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco/util/wsgi.py` & `fresco-3.3.2/fresco/util/wsgi.py`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/fresco.egg-info/PKG-INFO` & `fresco-3.3.2/fresco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fresco
-Version: 3.3.1
+Version: 3.3.2
 Summary: A Web/WSGI micro-framework
 Home-page: https://ollycope.com/software/fresco/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: wsgi web www framework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fresco-3.3.1/fresco.egg-info/SOURCES.txt` & `fresco-3.3.2/fresco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/setup.cfg` & `fresco-3.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `fresco-3.3.1/setup.py` & `fresco-3.3.2/setup.py`

 * *Files identical despite different names*

