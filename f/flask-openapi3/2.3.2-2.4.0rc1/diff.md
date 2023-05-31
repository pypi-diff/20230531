# Comparing `tmp/flask-openapi3-2.3.2.tar.gz` & `tmp/flask-openapi3-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-openapi3-2.3.2.tar", last modified: Mon Apr  3 02:25:04 2023, max compression
+gzip compressed data, was "flask-openapi3-2.4.0rc1.tar", last modified: Wed May 31 09:01:07 2023, max compression
```

## Comparing `flask-openapi3-2.3.2.tar` & `flask-openapi3-2.4.0rc1.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/api_blueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/api_view_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/async_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/custom_ui_templates_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/enum_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/header_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/image_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/init_oauth_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/just_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/nested_apiblueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/orjson_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/pydantic_custom_root_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/response_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/rest_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/servers_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/upload_file_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3/models/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.688719 flask-openapi3-2.3.2/flask_openapi3/templates/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3/templates/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/css/swagger-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/apidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/rapidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/redoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/swagger.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/rapidoc-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/redoc.standalone.js
--rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-05-31 09:00:57.000000 flask-openapi3-2.4.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/api_blueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/api_view_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/async_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/custom_ui_templates_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/enum_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/header_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/image_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/init_oauth_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/just_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/nested_apiblueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/openapi_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/orjson_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/pydantic_custom_root_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/response_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/rest_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/servers_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/examples/upload_file_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.884657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/swagger-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.892657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/apidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/rapidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/redoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/swagger.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.892657 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/rapidoc-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/redoc.standalone.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/flask_openapi3/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:01:07.888656 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 09:01:07.000000 flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:01:07.896657 flask-openapi3-2.4.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-31 09:00:58.000000 flask-openapi3-2.4.0rc1/setup.py
```

### Comparing `flask-openapi3-2.3.2/CHANGELOG.md` & `flask-openapi3-2.4.0rc1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,59 @@
+## v2.4.0 2023-??-??
+
+- [#72](https://github.com/luolingchun/flask-openapi3/pull/72) security_schemes(SecurityScheme) supports a json format.
+- [#68](https://github.com/luolingchun/flask-openapi3/pull/68) feat: Add operation_id_callback. Thanks, @BoyanYK.
+- Add DeprecationWarning to APIKey, HTTPBase, OAuth2, OpenIdConnect, HTTPBearer that will be deprecated in v3.0.
+
+
 ## v2.3.2 2023-04-03
 
 - [#61](https://github.com/luolingchun/flask-openapi3/issues/61) Fix headers with pydantic alias
 
 ## v2.3.1 2023-02-13
 
 - remove * in install_requires for setuptools 67+
 
 ## v2.3.0 2023-02-12
 
-- Support custom UI templates (#55)
+- Support for custom UI templates (#55)
 - endpoint index rename to openapi
-- fix missing enum in components schemas
+- fix missing enum in component schemas
 
 ## v2.2.2 2023-01-01
 
 - Fix async
 - Fix duplicate tags
 
 ## v2.2.1 2022-11-23
 
 - Add dependent files
 
 ## v2.2.0 2022-11-14
 
 - support APIView
 - Add mypy
-- Support python 3.11
+- Support for python 3.11
 - Upgrade Swagger UI 4.15.5
 - Upgrade Redoc UI 2.0.0
 
 ## v2.1.1 2022-10-12
 
-- [#41](https://github.com/luolingchun/flask-openapi3/issues/41) Set the `requestBody required` default value to True. Thanks @Colin-b
+- [#41](https://github.com/luolingchun/flask-openapi3/issues/41) Set the `requestBody required` default value to True. Thanks, @Colin-b
 - Fix multi decorator for api
-- [#42](https://github.com/luolingchun/flask-openapi3/issues/42) Fix required header is not found when `_` in header field. Thanks @elirud
+- [#42](https://github.com/luolingchun/flask-openapi3/issues/42) Fix required header is not found when `_` in header field. Thanks, @elirud
 
 ## v2.1.0 2022-09-04
 
-- [#36](https://github.com/luolingchun/flask-openapi3/issues/36) Add extra_form for operation. Thanks @Colin-b
-- [#36](https://github.com/luolingchun/flask-openapi3/issues/36) Add extra_body for operation. Thanks @Colin-b
+- [#36](https://github.com/luolingchun/flask-openapi3/issues/36) Add extra_form for operation. Thanks, @Colin-b
+- [#36](https://github.com/luolingchun/flask-openapi3/issues/36) Add extra_body for operation. Thanks, @Colin-b
 - Add external_docs for operation
 - Add servers for operation
-- Support parse extra field in parameters
-- [#35](https://github.com/luolingchun/flask-openapi3/issues/35) Fixed extra_responses can now be used to set every field in Response. Thanks @Colin-b
+- Support to parse extra field in parameters
+- [#35](https://github.com/luolingchun/flask-openapi3/issues/35) Fixed extra_responses can now be used to set every field in Response. Thanks, @Colin-b
 - Upgrade Swagger UI 4.14.0
 - Upgrade Redoc UI 2.0.0-rc.76
 - Upgrade RapiDoc UI 9.3.3
 
 
 ### Breaking Changes
 
@@ -55,20 +62,20 @@
 
 ## v2.0.1 2022-08-07
 
 - [#32](https://github.com/luolingchun/flask-openapi3/issues/32) Fix: parse_rule is deprecated in werkzeug>=2.2.0.
 
 ## v2.0.0 2022-06-26
 
-- [#26](https://github.com/luolingchun/flask-openapi3/issues/26) Fixed: Body throws exception when receiving str instead of dict. Thanks @nor3th
-- [#23](https://github.com/luolingchun/flask-openapi3/pull/23) Fixed externalDocs support. Thanks @dvaerum
-- [#28](https://github.com/luolingchun/flask-openapi3/pull/28) Fixed to enable `__root__` property when validation responses. Thanks @dvaerum
-- [#17](https://github.com/luolingchun/flask-openapi3/issues/17) Support for Nested APIBlueprint enhancement. Thanks @dvaerum
-- [#29](https://github.com/luolingchun/flask-openapi3/pull/29) Support disable warnings. Thanks @dvaerum
-- Support for empty response body. Thanks @dvaerum
+- [#26](https://github.com/luolingchun/flask-openapi3/issues/26) Fixed: Body throws exception when receiving str instead of dict. Thanks, @nor3th
+- [#23](https://github.com/luolingchun/flask-openapi3/pull/23) Fixed externalDocs support. Thanks, @dvaerum
+- [#28](https://github.com/luolingchun/flask-openapi3/pull/28) Fixed to enable `__root__` property when validation responses. Thanks, @dvaerum
+- [#17](https://github.com/luolingchun/flask-openapi3/issues/17) Support for Nested APIBlueprint enhancement. Thanks, @dvaerum
+- [#29](https://github.com/luolingchun/flask-openapi3/pull/29) Support disable warnings. Thanks, @dvaerum
+- Support for empty response body. Thanks, @dvaerum
 - Support reload authorizations in Swagger UI
 - Add `flask openapi` command
 - Add options in view functions
 - Upgrade flask to v2.x
 
 ### Breaking Changes
 
@@ -78,54 +85,54 @@
 ## v1.1.4 2022-05-05
 
 - fix: Trailing slash in APIBlueprint
 
 ## v1.1.3 2022-05-01
 
 - fix: Find globalns for the unwrapped func
-- [#19](https://github.com/luolingchun/flask-openapi3/issues/19) fix: Trailing slash in APIBlueprint. Thanks @ev-agelos
+- [#19](https://github.com/luolingchun/flask-openapi3/issues/19) fix: Trailing slash in APIBlueprint. Thanks, @ev-agelos
 - add description for UnprocessableEntity
 - remove printouts in `__init__.py`
 
 ## v1.1.2 2022-04-01
 
-- [#16](https://github.com/luolingchun/flask-openapi3/issues/16) Fix fileStorage list is not supported. Thanks @tekrei
+- [#16](https://github.com/luolingchun/flask-openapi3/issues/16) Fix fileStorage list is not supported. Thanks, @tekrei
 
 ## v1.1.0 2022-03-13
 
-- [#13](https://github.com/luolingchun/flask-openapi3/issues/13) drop support for flask 1.0.x. Thanks @danmur
-- [#15](https://github.com/luolingchun/flask-openapi3/pull/15) Fix to enable BaseModel with `__root__` property. Thanks @tarcisiojr
-- [#14](https://github.com/luolingchun/flask-openapi3/pull/14) Custom parameters: doc_prefix, api_doc_url, swagger_url, redoc_url, rapidoc_url. Thanks @barryrobison
+- [#13](https://github.com/luolingchun/flask-openapi3/issues/13) drop support for flask 1.0.x. Thanks, @danmur
+- [#15](https://github.com/luolingchun/flask-openapi3/pull/15) Fix to enable BaseModel with `__root__` property. Thanks, @tarcisiojr
+- [#14](https://github.com/luolingchun/flask-openapi3/pull/14) Custom parameters: doc_prefix, api_doc_url, swagger_url, redoc_url, rapidoc_url. Thanks, @barryrobison
 - Upgrade swagger UI v4.6.2
 - Upgrade Redoc v2.0.0-rc.63
 - Upgrade RapiDoc v9.2.0
 
 ## v1.0.1 2022-02-12
 
 - add operation_id for OpenAPI Specification
 
 ## v1.0.0 2022-01-11
 
-- [#10](https://github.com/luolingchun/flask-openapi3/issues/10) Fix: header's title case. Thanks @rrr34
-- [#9](https://github.com/luolingchun/flask-openapi3/issues/9) Support for extra responses. Thanks @blynn99
-- [#12](https://github.com/luolingchun/flask-openapi3/pull/12) Support for path operation field deprecated. Thanks @blynn99
+- [#10](https://github.com/luolingchun/flask-openapi3/issues/10) Fix: header's title case. Thanks, @rrr34
+- [#9](https://github.com/luolingchun/flask-openapi3/issues/9) Support for extra responses. Thanks, @blynn99
+- [#12](https://github.com/luolingchun/flask-openapi3/pull/12) Support for path operation field deprecated. Thanks, @blynn99
 - Add keyword parameters `summary` and `description`
 - Add servers for OpenAPI
 - Upgrade swagger UI v4.1.3
 - Upgrade Redoc v2.0.0-rc.59
 - Add rapidoc
 
 ### Breaking Changes
 
 - Renamed `securitySchemes` to `security_schemes`
 - Renamed `docExpansion` to `doc_expansion`
 
 ## v0.9.9 2021-12-09
 
-- fix: default value in query and form model
+- fix: default value in a query and form model
 - fix: empty form and body
 - support `from __future__ import annotations`
 - drop python36
 
 ## v0.9.8 2021-11-12
 
 - add Configuration `docExpansion`
@@ -144,25 +151,24 @@
 
 - remove `validate_resp` and add `VALIDATE_RESPONSE`
 
 ## v0.9.4 2021-07-03
 
 - OpenAPI add responses and APIBlueprint add abp_responses
 - fix: validate response error when responses is empty dict
-- [#3](https://github.com/luolingchun/flask-openapi3/issues/3) endpoint and APIBlueprint add `doc_ui`. Thanks
-  @DerManoMann
-- [#4](https://github.com/luolingchun/flask-openapi3/issues/4) fix: response description. Thanks @DerManoMann
-- [#5](https://github.com/luolingchun/flask-openapi3/issues/5) add custom parameter `oauth_config`. Thanks @DerManoMann
-- [#6](https://github.com/luolingchun/flask-openapi3/issues/6) support validation Flask Response. Thanks @DerManoMann
+- [#3](https://github.com/luolingchun/flask-openapi3/issues/3) endpoint and APIBlueprint add `doc_ui`. Thanks, @DerManoMann
+- [#4](https://github.com/luolingchun/flask-openapi3/issues/4) fix: response description. Thanks, @DerManoMann
+- [#5](https://github.com/luolingchun/flask-openapi3/issues/5) add custom parameter `oauth_config`. Thanks, @DerManoMann
+- [#6](https://github.com/luolingchun/flask-openapi3/issues/6) support validation Flask Response. Thanks, @DerManoMann
 - [#7](https://github.com/luolingchun/flask-openapi3/issues/7) fix: response validation does not work when uses
-  http.HTTPStatus enums as status_code. Thanks @DerManoMann
+  http.HTTPStatus enums as status_code. Thanks, @DerManoMann
 
 ## v0.9.3 2021-06-08
 
-- APIBlueprint add abp_tags and abp_security
+- APIBlueprint adds abp_tags and abp_security
 - fix: tags de-duplication
 - fix: operation summary and description
 
 ## v0.9.2 2021-05-17
 
 - fix: _do_decorator
 - add doc_ui args. support close swagger UI and redoc
```

### Comparing `flask-openapi3-2.3.2/CONTRIBUTING.md` & `flask-openapi3-2.4.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/LICENSE.rst` & `flask-openapi3-2.4.0rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/PKG-INFO` & `flask-openapi3-2.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.3.2
+Version: 2.4.0rc1
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,15 +55,15 @@
 **Flask OpenAPI3** is a web API framework based on **Flask**. It uses **Pydantic** to verify data and automatic
 generation of interaction documentation: **Swagger**, **ReDoc** and **RapiDoc**.
 
 The key features are:
 
 - **Easy to code:** Easy to use and easy to learn
 
-- **Standard document specification:** Based on [OpenAPI Specification](https://github.com/OAI/OpenAPI-Specification)
+- **Standard document specification:** Based on [OpenAPI Specification](https://spec.openapis.org/oas/v3.0.3)
 
 - **Interactive OpenAPI documentation:** [Swagger](https://github.com/swagger-api/swagger-ui), [Redoc](https://github.com/Redocly/redoc) and [RapiDoc](https://github.com/rapi-doc/RapiDoc)
   
 - **Data validation:** Fast data verification based on [Pydantic](https://github.com/pydantic/pydantic)
 
 - **Authorization:** Support to reload authorizations in Swagger UI
 
@@ -111,15 +111,15 @@
 # or manually
 pip install pyyaml asgiref python-dotenv email-validator
 ```
 </details>
 
 ## A Simple Example
 
-Here's a simple example, further go to the [Example](https://luolingchun.github.io/flask-openapi3/en/Example/).
+Here's a simple example, further go to the [Example](https://luolingchun.github.io/flask-openapi3/latest/Example/).
 
 ```python
 from pydantic import BaseModel
 
 from flask_openapi3 import Info, Tag
 from flask_openapi3 import OpenAPI
```

### Comparing `flask-openapi3-2.3.2/README.md` & `flask-openapi3-2.4.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 **Flask OpenAPI3** is a web API framework based on **Flask**. It uses **Pydantic** to verify data and automatic
 generation of interaction documentation: **Swagger**, **ReDoc** and **RapiDoc**.
 
 The key features are:
 
 - **Easy to code:** Easy to use and easy to learn
 
-- **Standard document specification:** Based on [OpenAPI Specification](https://github.com/OAI/OpenAPI-Specification)
+- **Standard document specification:** Based on [OpenAPI Specification](https://spec.openapis.org/oas/v3.0.3)
 
 - **Interactive OpenAPI documentation:** [Swagger](https://github.com/swagger-api/swagger-ui), [Redoc](https://github.com/Redocly/redoc) and [RapiDoc](https://github.com/rapi-doc/RapiDoc)
   
 - **Data validation:** Fast data verification based on [Pydantic](https://github.com/pydantic/pydantic)
 
 - **Authorization:** Support to reload authorizations in Swagger UI
 
@@ -81,15 +81,15 @@
 # or manually
 pip install pyyaml asgiref python-dotenv email-validator
 ```
 </details>
 
 ## A Simple Example
 
-Here's a simple example, further go to the [Example](https://luolingchun.github.io/flask-openapi3/en/Example/).
+Here's a simple example, further go to the [Example](https://luolingchun.github.io/flask-openapi3/latest/Example/).
 
 ```python
 from pydantic import BaseModel
 
 from flask_openapi3 import Info, Tag
 from flask_openapi3 import OpenAPI
```

### Comparing `flask-openapi3-2.3.2/examples/api_blueprint_demo.py` & `flask-openapi3-2.4.0rc1/examples/api_blueprint_demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 # @Time    : 2021/6/6 14:05
 
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
 from flask_openapi3 import APIBlueprint, OpenAPI
-from flask_openapi3 import HTTPBearer
 from flask_openapi3 import Tag, Info
 
 info = Info(title='book API', version='1.0.0')
-security_schemes = {"jwt": HTTPBearer(bearerFormat="JWT")}
+
+jwt = {
+    "type": "http",
+    "scheme": "bearer",
+    "bearerFormat": "JWT"
+}
+security_schemes = {"jwt": jwt}
 
 app = OpenAPI(__name__, info=info, security_schemes=security_schemes)
 
 tag = Tag(name='book', description="Some Book")
 security = [{"jwt": []}]
```

### Comparing `flask-openapi3-2.3.2/examples/api_view_demo.py` & `flask-openapi3-2.4.0rc1/examples/api_view_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 # @Author  : llc
 # @Time    : 2022/10/18 9:00
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
 from flask_openapi3 import APIView
-from flask_openapi3 import OpenAPI, Tag, Info, HTTPBearer
+from flask_openapi3 import OpenAPI, Tag, Info
 
-jwt = HTTPBearer()
+jwt = {
+    "type": "http",
+    "scheme": "bearer",
+    "bearerFormat": "JWT"
+}
 security_schemes = {"jwt": jwt}
 info = Info(title='book API', version='1.0.0')
 app = OpenAPI(__name__, info=info, security_schemes=security_schemes)
 
 security = [{"jwt": []}]
 
 api_view = APIView(url_prefix="/api/v1", view_tags=[Tag(name="book")], view_security=security)
@@ -38,15 +42,15 @@
     @api_view.doc(summary="get book list")
     def get(self, query: BookQuery):
         print(self.a)
         return query.json()
 
     @api_view.doc(summary="create book")
     def post(self, body: BookBody):
-        """description for create book"""
+        """description for a created book"""
         return body.json()
 
 
 @api_view.route("/book/<id>")
 class BookAPIView:
     @api_view.doc(summary="get book")
     def get(self, path: BookPath):
```

### Comparing `flask-openapi3-2.3.2/examples/async_demo.py` & `flask-openapi3-2.4.0rc1/examples/async_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     @api_view.doc(summary="get book list")
     async def get(self, query: BookQuery):
         return query.json()
 
     @api_view.doc(summary="create book")
     async def post(self, body: BookBody):
-        """description for create book"""
+        """description for a created book"""
         return body.json()
 
 
 app.register_api_view(api_view)
 
 if __name__ == '__main__':
     app.run(debug=True)
```

### Comparing `flask-openapi3-2.3.2/examples/custom_ui_templates_demo.py` & `flask-openapi3-2.4.0rc1/examples/custom_ui_templates_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     age: int
     author: str
 
 
 @app.get('/book', tags=[book_tag])
 def get_book(query: BookQuery):
     """get books
-    get all books
+    to get all books
     """
     return {
         "code": 0,
         "message": "ok",
         "data": [
             {"bid": 1, "age": query.age, "author": query.author},
             {"bid": 2, "age": query.age, "author": query.author}
```

### Comparing `flask-openapi3-2.3.2/examples/enum_demo.py` & `flask-openapi3-2.4.0rc1/examples/enum_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/examples/header_demo.py` & `flask-openapi3-2.4.0rc1/examples/header_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/examples/init_oauth_demo.py` & `flask-openapi3-2.4.0rc1/examples/init_oauth_demo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2021/6/21 11:23
-from flask_openapi3 import OpenAPI, OAuthConfig
 from flask_openapi3 import Info
-from flask_openapi3 import OAuth2, OAuthFlows, OAuthFlowImplicit
+from flask_openapi3 import OpenAPI, OAuthConfig
 
 info = Info(title='oauth API', version='1.0.0')
 
 oauth_config = OAuthConfig(
     clientId="xxx",
     clientSecret="xxx"
 )
 
-oauth2 = OAuth2(flows=OAuthFlows(
-    implicit=OAuthFlowImplicit(
-        authorizationUrl="https://example.com/api/oauth/dialog",
-        scopes={
-            "write:pets": "modify pets in your account",
-            "read:pets": "read your pets"
+oauth2 = {
+    "type": "oauth2",
+    "flows": {
+        "implicit": {
+            "authorizationUrl": "https://example.com/api/oauth/dialog",
+            "scopes": {
+                "write:pets": "modify pets in your account",
+                "read:pets": "read your pets"
+            }
         }
-    )))
+    }
+}
 security_schemes = {"oauth2": oauth2}
 
 app = OpenAPI(__name__, info=info, oauth_config=oauth_config, security_schemes=security_schemes)
 
 security = [
     {"oauth2": ["write:pets", "read:pets"]}
 ]
```

### Comparing `flask-openapi3-2.3.2/examples/nested_apiblueprint_demo.py` & `flask-openapi3-2.4.0rc1/examples/nested_apiblueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/examples/orjson_demo.py` & `flask-openapi3-2.4.0rc1/examples/orjson_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/examples/pydantic_custom_root_types.py` & `flask-openapi3-2.4.0rc1/examples/pydantic_custom_root_types.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/examples/response_demo.py` & `flask-openapi3-2.4.0rc1/examples/response_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/examples/rest_demo.py` & `flask-openapi3-2.4.0rc1/examples/rest_demo.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,31 +2,50 @@
 # @Author  : llc
 # @Time    : 2021/4/28 11:24
 from http import HTTPStatus
 from typing import Optional, List
 
 from pydantic import BaseModel, Field
 
+from flask_openapi3 import ExternalDocumentation, ExtraRequestBody, Example
 from flask_openapi3 import Info, Tag, Server
 from flask_openapi3 import OpenAPI
-from flask_openapi3 import ExternalDocumentation, ExtraRequestBody, Example
-from flask_openapi3 import HTTPBearer, OAuth2, OAuthFlows, OAuthFlowImplicit, APIKey, HTTPBase
 
 info = Info(title='book API', version='1.0.0')
-basic = HTTPBase()
-jwt = HTTPBearer()
-api_key = APIKey(name='api key')
-oauth2 = OAuth2(flows=OAuthFlows(
-    implicit=OAuthFlowImplicit(
-        authorizationUrl="https://example.com/api/oauth/dialog",
-        scopes={
-            "write:pets": "modify pets in your account",
-            "read:pets": "read your pets"
+
+# Basic Authentication Sample
+basic = {
+    "type": "http",
+    "scheme": "basic"
+}
+# JWT Bearer Sample
+jwt = {
+    "type": "http",
+    "scheme": "bearer",
+    "bearerFormat": "JWT"
+}
+# API Key Sample
+api_key = {
+    "type": "apiKey",
+    "name": "api_key",
+    "in": "header"
+}
+# Implicit OAuth2 Sample
+oauth2 = {
+    "type": "oauth2",
+    "flows": {
+        "implicit": {
+            "authorizationUrl": "https://example.com/api/oauth/dialog",
+            "scopes": {
+                "write:pets": "modify pets in your account",
+                "read:pets": "read your pets"
+            }
         }
-    )))
+    }
+}
 security_schemes = {"jwt": jwt, "api_key": api_key, "oauth2": oauth2, "basic": basic}
 
 
 class NotFoundResponse(BaseModel):
     code: int = Field(-1, description="Status Code")
     message: str = Field("Resource not found!", description="Exception Information")
 
@@ -79,28 +98,28 @@
 
     responses={"200": BookResponse},
     extra_responses={"200": {"content": {"text/csv": {"schema": {"type": "string"}}}}},
     security=security,
     servers=[Server(url="https://www.openapis.org/", description="openapi")]
 )
 def get_book(path: BookPath):
-    """Get book
-    Get some book by id, like:
+    """Get a book
+    to Get some book by id, like:
     http://localhost:5000/book/3
     """
     if path.bid == 4:
         return NotFoundResponse().dict(), 404
     return {"code": 0, "message": "ok", "data": {"bid": path.bid, "age": 3, "author": 'no'}}
 
 
 # set doc_ui False disable openapi UI
 @app.get('/book', doc_ui=True, deprecated=True)
 def get_books(query: BookQuery):
     """get books
-    get all books
+    to get all books
     """
     print(query)
     return {
         "code": 0,
         "message": "ok",
         "data": [
             {"bid": 1, "age": query.age, "author": 'a1'},
```

### Comparing `flask-openapi3-2.3.2/examples/servers_demo.py` & `flask-openapi3-2.4.0rc1/examples/servers_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     age: int
     author: str
 
 
 @app.get('/book', tags=[book_tag])
 def get_book(query: BookQuery):
     """get books
-    get all books
+    to get all books
     """
     return {
         "code": 0,
         "message": "ok",
         "data": [
             {"bid": 1, "age": query.age, "author": query.author},
             {"bid": 2, "age": query.age, "author": query.author}
```

### Comparing `flask-openapi3-2.3.2/examples/simple_demo.py` & `flask-openapi3-2.4.0rc1/examples/simple_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/examples/upload_file_demo.py` & `flask-openapi3-2.4.0rc1/examples/upload_file_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/__init__.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/blueprint.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/blueprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,39 +23,44 @@
             name: str,
             import_name: str,
             *,
             abp_tags: Optional[List[Tag]] = None,
             abp_security: Optional[List[Dict[str, List[str]]]] = None,
             abp_responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             doc_ui: bool = True,
+            operation_id_callback: Callable = get_operation_id_for_path,
             **kwargs: Any
     ) -> None:
         """
         Based on Flask Blueprint
 
         Arguments:
             name: The name of the blueprint. It Will be prepared to each endpoint name.
             import_name: The name of the blueprint package, usually
                          ``__name__``. This helps locate the ``root_path`` for the blueprint.
             abp_tags: APIBlueprint tags for every api
             abp_security: APIBlueprint security for every api
             abp_responses: APIBlueprint response model
             doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
+            operation_id_callback: Callback function for custom operation_id generation.
+                Receives name (str), path (str) and method (str) parameters.
+                Defaults to `get_operation_id_for_path` from utils
             **kwargs: Flask Blueprint kwargs
         """
         super(APIBlueprint, self).__init__(name, import_name, **kwargs)
         self.paths: Dict = dict()
         self.components_schemas: Dict = dict()
         self.tags: List[Tag] = []
         self.tag_names: List[str] = []
 
         self.abp_tags = abp_tags or []
         self.abp_security = abp_security or []
         self.abp_responses = abp_responses or {}
         self.doc_ui = doc_ui
+        self.operation_id_callback: Callable = operation_id_callback
 
     def register_api(self, api: "APIBlueprint") -> None:
         """Register a nested APIBlueprint"""
         if api is self:
             raise ValueError("Cannot register a api blueprint on itself")
 
         for tag in api.tags:
@@ -88,48 +93,59 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, Dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             method: str = HTTPMethod.GET
     ) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
         """
         Collect openapi specification information
-        :param rule: flask route
-        :param func: flask view_func
-        :param tags: api tag
-        :param responses: response model
-        :param extra_responses: extra response dict
-        :param security: security name
-        :param doc_ui: adds openapi document UI(swagger and redoc). defaults to True.
-        :param deprecated: mark as deprecated support. default to not True.
-        :param operation_id: unique string used to identify the operation.
-        :param method: api method
-        :return:
+        Arguments:
+            rule: Flask route
+            func: Flask view_func
+            tags: Adds metadata to a single tag.
+            summary: A short summary of what the operation does.
+            description: A verbose explanation of the operation behavior.
+            external_docs: Additional external documentation for this operation.
+            operation_id: Unique string used to identify the operation.
+            extra_form: Extra information describing the request body(application/form).
+            extra_body: Extra information describing the request body(application/json).
+            responses: response's model must be pydantic BaseModel.
+            extra_responses: Extra information for responses.
+            deprecated: Declares this operation to be deprecated.
+            security: A declaration of which security mechanisms can be used for this operation.
+            servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
         if self.doc_ui is True and doc_ui is True:
             if responses is None:
                 responses = {}
             if extra_responses is None:
                 extra_responses = {}
             # global response combine api responses
             combine_responses = deepcopy(self.abp_responses)
             combine_responses.update(**responses)
             # create operation
-            operation = get_operation(func, summary=summary, description=description)
+            operation = get_operation(
+                func,
+                summary=summary,
+                description=description,
+                openapi_extensions=openapi_extensions
+            )
             # set external docs
             operation.externalDocs = external_docs
             # Unique string used to identify the operation.
-            if operation_id:
-                operation.operationId = operation_id
-            else:
-                operation.operationId = get_operation_id_for_path(name=func.__name__, path=rule, method=method)
+            operation.operationId = operation_id or self.operation_id_callback(
+                name=func.__name__, path=rule, method=method
+            )
             # only set `deprecated` if True otherwise leave it as None
             operation.deprecated = deprecated
             # add security
             if security is None:
                 security = []
             operation.security = security + self.abp_security or None
             # add servers
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3/commands.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/commands.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/http.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/http.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/markdown.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/markdown.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/__init__.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/common.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/common.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/component.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/component.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,13 +14,13 @@
     """https://spec.openapis.org/oas/v3.0.3#components-object"""
     schemas: Optional[Dict[str, Union[Schema, Reference]]] = None
     responses: Optional[Dict[str, Union[Response, Reference]]] = None
     parameters: Optional[Dict[str, Union[Parameter, Reference]]] = None
     examples: Optional[Dict[str, Union[Example, Reference]]] = None
     requestBodies: Optional[Dict[str, Union[RequestBody, Reference]]] = None
     headers: Optional[Dict[str, Union[Header, Reference]]] = None
-    securitySchemes: Optional[Dict[str, Union[SecurityScheme, Reference]]] = None
+    securitySchemes: Optional[Dict[str, Union[SecurityScheme, Dict[str, Any]]]] = None
     links: Optional[Dict[str, Union[Link, Reference]]] = None
     callbacks: Optional[Dict[str, Union[Dict[str, PathItem], Reference, Any]]] = None
 
     class Config:
         extra = "allow"
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/file.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/file.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/info.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/info.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/oauth.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/oauth.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/path.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     class Config:
         extra = "allow"
 
 
 class RequestBody(BaseModel):
     description: Optional[str] = None
     content: Dict[str, MediaType]
-    required: Optional[bool] = None
+    required: Optional[bool] = True
 
     class Config:
         extra = "allow"
 
 
 class Response(BaseModel):
     description: Optional[str]
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/server.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/server.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/models/validation_error.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/openapi.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/openapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from flask import Flask, Blueprint, render_template_string
 from pydantic import BaseModel
 
 from .blueprint import APIBlueprint
 from .commands import openapi_command
 from .http import HTTPMethod
 from .models import Info, APISpec, Tag, Components, Server
-from .models.common import Reference, ExternalDocumentation, ExtraRequestBody
+from .models.common import ExternalDocumentation, ExtraRequestBody
 from .models.oauth import OAuthConfig
 from .models.security import SecurityScheme
 from .scaffold import APIScaffold
 from .templates import openapi_html_string, redoc_html_string, rapidoc_html_string, swagger_html_string
 from .utils import get_operation, get_responses, parse_and_store_tags, parse_parameters, parse_method, \
     get_operation_id_for_path
 from .view import APIView
@@ -26,27 +26,29 @@
 
 class OpenAPI(APIScaffold, Flask):
     def __init__(
             self,
             import_name: str,
             *,
             info: Optional[Info] = None,
-            security_schemes: Optional[Dict[str, Union[SecurityScheme, Reference]]] = None,
+            security_schemes: Optional[Dict[str, Union[SecurityScheme, Dict[str, Any]]]] = None,
             oauth_config: Optional[OAuthConfig] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             doc_ui: bool = True,
             doc_expansion: str = "list",
             doc_prefix: str = "/openapi",
             api_doc_url: str = "/openapi.json",
             swagger_url: str = "/swagger",
             redoc_url: str = "/redoc",
             rapidoc_url: str = "/rapidoc",
             ui_templates: Optional[Dict[str, str]] = None,
             servers: Optional[List[Server]] = None,
             external_docs: Optional[ExternalDocumentation] = None,
+            operation_id_callback: Callable = get_operation_id_for_path,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             **kwargs: Any
     ) -> None:
         """
         Based on Flask. Provide REST api, swagger-ui and redoc.
 
         Arguments:
             import_name: Just flask import_name
@@ -66,14 +68,19 @@
             swagger_url: The Swagger UI documentation. Defaults to `/swagger`.
             redoc_url: The Redoc UI documentation. Defaults to `/redoc`.
             rapidoc_url: The RapiDoc UI documentation. Defaults to `/rapidoc`.
             ui_templates: Custom UI templates, which are used to overwrite or add UI documents.
             servers: An array of Server Objects, which provide connectivity information to a target server.
             external_docs: Allows referencing an external resource for extended documentation.
                            See: https://spec.openapis.org/oas/v3.0.3#external-documentation-object
+            operation_id_callback: Callback function for custom operation_id generation.
+                          Receives name (str), path (str) and method (str) parameters.
+                          Default to `get_operation_id_for_path` from utils
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+                                See https://spec.openapis.org/oas/v3.0.3#specification-extensions
             **kwargs: Flask kwargs
         """
         super(OpenAPI, self).__init__(import_name, **kwargs)
         self.openapi_version = "3.0.3"
         self.info = info or Info(title="OpenAPI", version="1.0.0")
         self.security_schemes = security_schemes
         self.responses = responses or {}
@@ -88,14 +95,16 @@
         self.redoc_url = redoc_url
         self.rapidoc_url = rapidoc_url
         self.oauth_config = oauth_config
         self.doc_expansion = doc_expansion
         self.ui_templates = ui_templates or dict()
         self.severs = servers
         self.external_docs = external_docs
+        self.operation_id_callback: Callable = operation_id_callback
+        self.openapi_extensions = openapi_extensions or dict()
         if doc_ui:
             self._init_doc()
         # add openapi command
         self.cli.add_command(openapi_command)
 
     def _init_doc(self) -> None:
         """
@@ -161,35 +170,47 @@
             externalDocs=self.external_docs
         )
         spec.tags = self.tags or None
         spec.paths = self.paths
         self.components.schemas = self.components_schemas
         self.components.securitySchemes = self.security_schemes
         spec.components = self.components
-        return json.loads(spec.json(by_alias=True, exclude_none=True))
+
+        spec_json = json.loads(spec.json(by_alias=True, exclude_none=True))
+        spec_json.update(**self.openapi_extensions)
+
+        return spec_json
 
     def register_api(self, api: APIBlueprint) -> None:
         """Register APIBlueprint"""
         for tag in api.tags:
             if tag.name not in self.tag_names:
                 self.tags.append(tag)
                 self.tag_names.append(tag.name)
         self.paths.update(**api.paths)
         self.components_schemas.update(**api.components_schemas)
         self.register_blueprint(api)
 
-    def register_api_view(self, api_view: APIView) -> None:
-        """Register APIView"""
+    def register_api_view(self, api_view: APIView, view_kwargs: Optional[Dict[Any, Any]] = None) -> None:
+        """
+        Register APIView
+
+        Arguments:
+            api_view: APIView
+            view_kwargs: extra view kwargs
+        """
+        if view_kwargs is None:
+            view_kwargs = {}
         for tag in api_view.tags:
             if tag.name not in self.tag_names:
                 self.tags.append(tag)
                 self.tag_names.append(tag.name)
         self.paths.update(**api_view.paths)
         self.components_schemas.update(**api_view.components_schemas)
-        api_view.register(self)
+        api_view.register(self, view_kwargs=view_kwargs)
 
     def _do_decorator(
             self,
             rule: str,
             func: Callable,
             *,
             tags: Optional[List[Tag]] = None,
@@ -200,48 +221,59 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, Dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             method: str = HTTPMethod.GET
     ) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
         """
         Collect openapi specification information
-        :param rule: Flask route
-        :param func: Flask view_func
-        :param tags: API tag
-        :param responses: Response model
-        :param extra_responses: Extra response dict
-        :param security: Security name
-        :param deprecated: Mark as deprecated support. Default to not True.
-        :param doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
-        :param operation_id: Unique string used to identify the operation.
-        :param method: API method
-        :return:
+        Arguments:
+            rule: Flask route
+            func: Flask view_func
+            tags: Adds metadata to a single tag.
+            summary: A short summary of what the operation does.
+            description: A verbose explanation of the operation behavior.
+            external_docs: Additional external documentation for this operation.
+            operation_id: Unique string used to identify the operation.
+            extra_form: Extra information describing the request body(application/form).
+            extra_body: Extra information describing the request body(application/json).
+            responses: response's model must be pydantic BaseModel.
+            extra_responses: Extra information for responses.
+            deprecated: Declares this operation to be deprecated.
+            security: A declaration of which security mechanisms can be used for this operation.
+            servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
         if doc_ui is True:
             if responses is None:
                 responses = {}
             if extra_responses is None:
                 extra_responses = {}
             # global response combine api responses
             combine_responses = deepcopy(self.responses)
             combine_responses.update(**responses)
             # create operation
-            operation = get_operation(func, summary=summary, description=description)
+            operation = get_operation(
+                func,
+                summary=summary,
+                description=description,
+                openapi_extensions=openapi_extensions
+            )
             # set external docs
             operation.externalDocs = external_docs
             # Unique string used to identify the operation.
-            if operation_id:
-                operation.operationId = operation_id
-            else:
-                operation.operationId = get_operation_id_for_path(name=func.__name__, path=rule, method=method)
+            operation.operationId = operation_id or self.operation_id_callback(
+                name=func.__name__, path=rule, method=method
+            )
             # only set `deprecated` if True otherwise leave it as None
             operation.deprecated = deprecated
             # add security
             operation.security = security
             # add servers
             operation.servers = servers
             # store tags
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3/request.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/request.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/scaffold.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/scaffold.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,24 +46,35 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             method: str = HTTPMethod.GET
     ) -> Tuple[Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel], Type[BaseModel]]:
         raise NotImplementedError
 
     def register_api(self, api) -> None:
         raise NotImplementedError
 
     @staticmethod
-    def create_view_func(func, header, cookie, path, query, form, body, view_class=None):
+    def create_view_func(
+            func,
+            header,
+            cookie,
+            path,
+            query,
+            form,
+            body,
+            view_class=None,
+            view_kwargs=None
+    ):
         is_coroutine_function = iscoroutinefunction(func)
         if is_coroutine_function:
             @wraps(func)
             async def view_func(**kwargs) -> Response:
                 result = _do_request(
                     header=header,
                     cookie=cookie,
@@ -74,15 +85,21 @@
                     **kwargs
                 )
                 if isinstance(result, Response):
                     # 422
                     return result
                 # handle async request
                 if view_class:
-                    response = await func(view_class, **result)
+                    signature = inspect.signature(view_class.__init__)
+                    parameters = signature.parameters
+                    if parameters.get("view_kwargs"):
+                        view_object = view_class(view_kwargs=view_kwargs)
+                    else:
+                        view_object = view_class()
+                    response = await func(view_object, **result)
                 else:
                     response = await func(**result)
                 return response
         else:
             @wraps(func)
             def view_func(**kwargs) -> Response:
                 result = _do_request(
@@ -95,15 +112,21 @@
                     **kwargs
                 )
                 if isinstance(result, Response):
                     # 422
                     return result
                 # handle request
                 if view_class:
-                    response = func(view_class, **result)
+                    signature = inspect.signature(view_class.__init__)
+                    parameters = signature.parameters
+                    if parameters.get("view_kwargs"):
+                        view_object = view_class(view_kwargs=view_kwargs)
+                    else:
+                        view_object = view_class()
+                    response = func(view_object, **result)
                 else:
                     response = func(**result)
                 return response
 
         if not hasattr(func, "view"):
             func.view = view_func
 
@@ -121,14 +144,15 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
         Decorator for rest api, like: app.route(methods=["GET"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
@@ -142,14 +166,15 @@
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
             responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
@@ -162,14 +187,15 @@
                     extra_form=extra_form,
                     extra_body=extra_body,
                     responses=responses,
                     extra_responses=extra_responses,
                     deprecated=deprecated,
                     security=security,
                     servers=servers,
+                    openapi_extensions=openapi_extensions,
                     doc_ui=doc_ui,
                     method=HTTPMethod.GET
                 )
 
             view_func = self.create_view_func(func, header, cookie, path, query, form, body)
             options.update({"methods": [HTTPMethod.GET]})
             self.add_url_rule(rule, view_func=view_func, **options)
@@ -190,14 +216,15 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
         Decorator for rest api, like: app.route(methods=["POST"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
@@ -211,14 +238,15 @@
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
             responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Declares this operation to be shown.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
@@ -231,14 +259,15 @@
                     extra_form=extra_form,
                     extra_body=extra_body,
                     responses=responses,
                     extra_responses=extra_responses,
                     deprecated=deprecated,
                     security=security,
                     servers=servers,
+                    openapi_extensions=openapi_extensions,
                     doc_ui=doc_ui,
                     method=HTTPMethod.POST
                 )
 
             view_func = self.create_view_func(func, header, cookie, path, query, form, body)
             options.update({"methods": [HTTPMethod.POST]})
             self.add_url_rule(rule, view_func=view_func, **options)
@@ -259,14 +288,15 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
         Decorator for rest api, like: app.route(methods=["PUT"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
@@ -280,14 +310,15 @@
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
             responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Declares this operation to be shown.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
@@ -300,14 +331,15 @@
                     extra_form=extra_form,
                     extra_body=extra_body,
                     responses=responses,
                     extra_responses=extra_responses,
                     deprecated=deprecated,
                     security=security,
                     servers=servers,
+                    openapi_extensions=openapi_extensions,
                     doc_ui=doc_ui,
                     method=HTTPMethod.PUT
                 )
 
             view_func = self.create_view_func(func, header, cookie, path, query, form, body)
             options.update({"methods": [HTTPMethod.PUT]})
             self.add_url_rule(rule, view_func=view_func, **options)
@@ -328,14 +360,15 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
         Decorator for rest api, like: app.route(methods=["DELETE"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
@@ -349,14 +382,15 @@
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
             responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Declares this operation to be shown.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
@@ -369,14 +403,15 @@
                     extra_form=extra_form,
                     extra_body=extra_body,
                     responses=responses,
                     extra_responses=extra_responses,
                     deprecated=deprecated,
                     security=security,
                     servers=servers,
+                    openapi_extensions=openapi_extensions,
                     doc_ui=doc_ui,
                     method=HTTPMethod.DELETE
                 )
 
             view_func = self.create_view_func(func, header, cookie, path, query, form, body)
             options.update({"methods": [HTTPMethod.DELETE]})
             self.add_url_rule(rule, view_func=view_func, **options)
@@ -397,14 +432,15 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True,
             **options: Any
     ) -> Callable:
         """
         Decorator for rest api, like: app.route(methods=["PATCH"])
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
@@ -418,14 +454,15 @@
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
             responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
             doc_ui: Declares this operation to be shown.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
@@ -438,14 +475,15 @@
                     extra_form=extra_form,
                     extra_body=extra_body,
                     responses=responses,
                     extra_responses=extra_responses,
                     deprecated=deprecated,
                     security=security,
                     servers=servers,
+                    openapi_extensions=openapi_extensions,
                     doc_ui=doc_ui,
                     method=HTTPMethod.PATCH
                 )
 
             view_func = self.create_view_func(func, header, cookie, path, query, form, body)
             options.update({"methods": [HTTPMethod.PATCH]})
             self.add_url_rule(rule, view_func=view_func, **options)
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/__init__.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,18 +147,20 @@
                 SwaggerUIBundle.presets.apis,
                 SwaggerUIStandalonePreset
             ],
             plugins: [
                 SwaggerUIBundle.plugins.DownloadUrl
             ],
             layout: "StandaloneLayout",
-            docExpansion: "{{ doc_expansion }}"
+            docExpansion: "{{ doc_expansion }}",
+            showExtensions: true,
+            showCommonExtensions: true
         })
         // End Swagger UI call region
-        const oauthConfig = JSON.parse("{{ oauth_config|tojson }}");
+        const oauthConfig = JSON.parse(`{{ oauth_config|tojson }}`);
         if (oauthConfig != null) {
             window.ui.initOAuth({
                 clientId: oauthConfig.clientId,
                 clientSecret: oauthConfig.clientSecret,
                 realm: oauthConfig.realm,
                 appName: oauthConfig.appName,
                 scopeSeparator: oauthConfig.scopeSeparator,
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/css/swagger-ui.css` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/css/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/images/apidoc.svg` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/apidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/images/rapidoc.svg` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/rapidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/images/redoc.svg` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/redoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/images/swagger.svg` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/images/swagger.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/js/rapidoc-min.js` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/rapidoc-min.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/js/redoc.standalone.js` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/js/swagger-ui-bundle.js` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js` & `flask-openapi3-2.4.0rc1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.2/flask_openapi3/utils.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 # -*- coding: utf-8 -*-
 # @Author  : llc
 # @Time    : 2021/5/1 21:34
 
 import inspect
 import re
-from typing import get_type_hints, Dict, Type, Callable, List, Tuple, Optional
+from typing import get_type_hints, Dict, Type, Callable, List, Tuple, Optional, Any
 
 from pydantic import BaseModel
 
 from .http import HTTP_STATUS, HTTPMethod
 from .models import OPENAPI3_REF_TEMPLATE, OPENAPI3_REF_PREFIX, Tag
 from .models.common import Schema, MediaType, Encoding, ExtraRequestBody
 from .models.path import Operation, RequestBody, PathItem, Response
 from .models.path import ParameterInType, Parameter
 from .models.validation_error import UnprocessableEntity
 
 
-def get_operation(func: Callable, *, summary: Optional[str] = None, description: Optional[str] = None) -> Operation:
+def get_operation(
+        func: Callable, *,
+        summary: Optional[str] = None,
+        description: Optional[str] = None,
+        openapi_extensions: Optional[Dict[str, Any]] = None,
+) -> Operation:
     """Return an Operation object with summary and description."""
     doc = inspect.getdoc(func) or ""
     doc = doc.strip()
     lines = doc.split("\n")
     doc_summary = lines[0] or None
     if summary is None:
         doc_description = lines[0] if len(lines) == 0 else "</br>".join(lines[1:]) or None
     else:
         doc_description = "</br>".join(lines) or None
-    operation = Operation(
+
+    operation_dict = dict(
         summary=summary or doc_summary,
         description=description or doc_description
     )
+    # update openapi_extensions
+    openapi_extensions = openapi_extensions or {}
+    operation_dict.update(**openapi_extensions)
+
+    operation = Operation(**operation_dict)
 
     return operation
 
 
 def get_operation_id_for_path(*, name: str, path: str, method: str) -> str:
     operation_id = name + path
     operation_id = re.sub(r"\W", "_", operation_id)
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3/view.py` & `flask-openapi3-2.4.0rc1/flask_openapi3/view.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,31 +23,36 @@
 class APIView:
     def __init__(
             self,
             url_prefix: Optional[str] = None,
             view_tags: Optional[List[Tag]] = None,
             view_security: Optional[List[Dict[str, List[str]]]] = None,
             view_responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
-            doc_ui: bool = True
+            doc_ui: bool = True,
+            operation_id_callback: Callable = get_operation_id_for_path,
     ):
         """
         Create a class-based view
 
         Arguments:
             url_prefix: A path to prepend to all the APIView's urls
             view_tags: APIView tags for every api
             view_security: APIView security for every api
             view_responses: APIView response models
             doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
+            operation_id_callback: Callback function for custom operation_id generation.
+                Receives name (str), path (str) and method (str) parameters.
+                Defaults to `get_operation_id_for_path` from utils
         """
         self.url_prefix = url_prefix
         self.view_tags = view_tags or []
         self.view_security = view_security or []
         self.view_responses = view_responses or {}
         self.doc_ui = doc_ui
+        self.operation_id_callback: Callable = operation_id_callback
 
         self.views: Dict = dict()
         self.paths: Dict = dict()
         self.components_schemas: Dict = dict()
         self.tags: List[Tag] = []
         self.tag_names: List[str] = []
 
@@ -74,15 +79,15 @@
                     continue
                 if not getattr(cls_method, "operation", None):
                     continue
                 # parse method
                 parse_method(uri, method, self.paths, cls_method.operation)
                 # update operation_id
                 if not cls_method.operation.operationId:
-                    cls_method.operation.operationId = get_operation_id_for_path(
+                    cls_method.operation.operationId = self.operation_id_callback(
                         name=cls_method.__qualname__,
                         path=rule,
                         method=method
                     )
             # /pet/{petId} --> /pet/<petId>
             _rule = uri.replace("{", "<").replace("}", ">")
             self.views[_rule] = (cls, methods)
@@ -102,14 +107,15 @@
             extra_form: Optional[ExtraRequestBody] = None,
             extra_body: Optional[ExtraRequestBody] = None,
             responses: Optional[Dict[str, Optional[Type[BaseModel]]]] = None,
             extra_responses: Optional[Dict[str, dict]] = None,
             deprecated: Optional[bool] = None,
             security: Optional[List[Dict[str, List[Any]]]] = None,
             servers: Optional[List[Server]] = None,
+            openapi_extensions: Optional[Dict[str, Any]] = None,
             doc_ui: bool = True
     ) -> Callable:
         """
         Decorator for view method.
         More information goto https://spec.openapis.org/oas/v3.0.3#operation-object
 
         Arguments:
@@ -121,15 +127,16 @@
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
             responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
-            doc_ui: Declares this operation to be shown.
+            openapi_extensions: Allows extensions to the OpenAPI Schema.
+            doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
 
         if responses is None:
             responses = {}
         if extra_responses is None:
             extra_responses = {}
         if security is None:
@@ -139,15 +146,20 @@
         def decorator(func):
             if self.doc_ui is False or doc_ui is False:
                 return
             # global response combine api responses
             combine_responses = deepcopy(self.view_responses)
             combine_responses.update(**responses)
             # create operation
-            operation = get_operation(func, summary=summary, description=description)
+            operation = get_operation(
+                func,
+                summary=summary,
+                description=description,
+                openapi_extensions=openapi_extensions
+            )
             # set external docs
             operation.externalDocs = external_docs
             # Unique string used to identify the operation.
             operation.operationId = operation_id
             # only set `deprecated` if True otherwise leave it as None
             operation.deprecated = deprecated
             # add security
@@ -168,18 +180,30 @@
             get_responses(combine_responses, extra_responses, self.components_schemas, operation)
             func.operation = operation
 
             return func
 
         return decorator
 
-    def register(self, app: "OpenAPI"):
+    def register(self, app: "OpenAPI", view_kwargs: Optional[Dict[Any, Any]] = None):
+        if view_kwargs is None:
+            view_kwargs = {}
         for rule, (cls, methods) in self.views.items():
             for method in methods:
                 func = getattr(cls, method.lower())
                 header, cookie, path, query, form, body = parse_parameters(func, doc_ui=False)
-                view_func = app.create_view_func(func, header, cookie, path, query, form, body, view_class=cls)
+                view_func = app.create_view_func(
+                    func,
+                    header,
+                    cookie,
+                    path,
+                    query,
+                    form,
+                    body,
+                    view_class=cls,
+                    view_kwargs=view_kwargs
+                )
                 options = {
                     "endpoint": cls.__name__ + "." + method.lower(),
                     "methods": [method.upper()]
                 }
                 app.add_url_rule(rule, view_func=view_func, **options)
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3.egg-info/PKG-INFO` & `flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.3.2
+Version: 2.4.0rc1
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,15 +55,15 @@
 **Flask OpenAPI3** is a web API framework based on **Flask**. It uses **Pydantic** to verify data and automatic
 generation of interaction documentation: **Swagger**, **ReDoc** and **RapiDoc**.
 
 The key features are:
 
 - **Easy to code:** Easy to use and easy to learn
 
-- **Standard document specification:** Based on [OpenAPI Specification](https://github.com/OAI/OpenAPI-Specification)
+- **Standard document specification:** Based on [OpenAPI Specification](https://spec.openapis.org/oas/v3.0.3)
 
 - **Interactive OpenAPI documentation:** [Swagger](https://github.com/swagger-api/swagger-ui), [Redoc](https://github.com/Redocly/redoc) and [RapiDoc](https://github.com/rapi-doc/RapiDoc)
   
 - **Data validation:** Fast data verification based on [Pydantic](https://github.com/pydantic/pydantic)
 
 - **Authorization:** Support to reload authorizations in Swagger UI
 
@@ -111,15 +111,15 @@
 # or manually
 pip install pyyaml asgiref python-dotenv email-validator
 ```
 </details>
 
 ## A Simple Example
 
-Here's a simple example, further go to the [Example](https://luolingchun.github.io/flask-openapi3/en/Example/).
+Here's a simple example, further go to the [Example](https://luolingchun.github.io/flask-openapi3/latest/Example/).
 
 ```python
 from pydantic import BaseModel
 
 from flask_openapi3 import Info, Tag
 from flask_openapi3 import OpenAPI
```

### Comparing `flask-openapi3-2.3.2/flask_openapi3.egg-info/SOURCES.txt` & `flask-openapi3-2.4.0rc1/flask_openapi3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 examples/custom_ui_templates_demo.py
 examples/enum_demo.py
 examples/header_demo.py
 examples/image_demo.py
 examples/init_oauth_demo.py
 examples/just_flask.py
 examples/nested_apiblueprint_demo.py
+examples/openapi_extensions.py
 examples/orjson_demo.py
 examples/pydantic_custom_root_types.py
 examples/response_demo.py
 examples/rest_demo.py
 examples/servers_demo.py
 examples/simple_demo.py
 examples/upload_file_demo.py
```

### Comparing `flask-openapi3-2.3.2/setup.py` & `flask-openapi3-2.4.0rc1/setup.py`

 * *Files identical despite different names*

