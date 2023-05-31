# Comparing `tmp/goodmap-0.1.7.tar.gz` & `tmp/goodmap-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodmap-0.1.7.tar", max compression
+gzip compressed data, was "goodmap-0.1.8.tar", max compression
```

## Comparing `goodmap-0.1.7.tar` & `goodmap-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,39 @@
--rw-r--r--   0        0        0     2481 2022-10-27 10:34:26.878696 goodmap-0.1.7/README.md
--rw-r--r--   0        0        0        1 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/__init__.py
--rw-r--r--   0        0        0      560 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/core.py
--rw-r--r--   0        0        0     1403 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/core_api.py
--rw-r--r--   0        0        0      372 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/db/extend.py
--rw-r--r--   0        0        0      279 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/db/google_json_db.py
--rw-r--r--   0        0        0      221 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/db/local_json_db.py
--rw-r--r--   0        0        0      489 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/formatter.py
--rw-r--r--   0        0        0     1181 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/goodmap.py
--rw-r--r--   0        0        0       37 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/static/map.css
--rw-r--r--   0        0        0        0 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/templates/admin.html
--rw-r--r--   0        0        0     3418 2022-10-27 10:34:26.878696 goodmap-0.1.7/goodmap/templates/map.html
--rw-r--r--   0        0        0      573 2022-10-27 10:34:26.878696 goodmap-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 goodmap-0.1.7/setup.py
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 goodmap-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-31 13:00:58.713740 goodmap-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     2763 2023-05-31 13:00:58.713740 goodmap-0.1.8/README.md
+-rw-r--r--   0        0        0        1 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/__init__.py
+-rw-r--r--   0        0        0     2697 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/config.py
+-rw-r--r--   0        0        0      551 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/core.py
+-rw-r--r--   0        0        0     1765 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/core_api.py
+-rw-r--r--   0        0        0      545 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/formatter.py
+-rw-r--r--   0        0        0     1428 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/goodmap.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/__init__.py
+-rw-r--r--   0        0        0     2794 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/blog/blog.py
+-rw-r--r--   0        0        0      498 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/blog/comment_form.py
+-rw-r--r--   0        0        0      354 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/blog/db.py
+-rw-r--r--   0        0        0      476 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/blog/post_formatter.py
+-rw-r--r--   0        0        0      909 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/db/google_json_db.py
+-rw-r--r--   0        0        0     5108 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/db/graph_ql_db.py
+-rw-r--r--   0        0        0     1356 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/db/json_db.py
+-rw-r--r--   0        0        0      732 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/db/json_file_db.py
+-rw-r--r--   0        0        0     3525 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/platzky.py
+-rw-r--r--   0        0        0     1443 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/plugin_loader.py
+-rw-r--r--   0        0        0     1205 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/plugins/redirections/entrypoint.py
+-rw-r--r--   0        0        0      674 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/plugins/sendmail/entrypoint.py
+-rw-r--r--   0        0        0     2615 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/seo/seo.py
+-rw-r--r--   0        0        0     8079 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/static/blog.css
+-rw-r--r--   0        0        0       78 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/404.html
+-rw-r--r--   0        0        0     4165 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/base.html
+-rw-r--r--   0        0        0     1286 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/blog.html
+-rw-r--r--   0        0        0      756 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/body_meta.html
+-rw-r--r--   0        0        0      859 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/feed.xml
+-rw-r--r--   0        0        0     1796 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/head_meta.html
+-rw-r--r--   0        0        0     3900 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/home.html
+-rw-r--r--   0        0        0      647 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/page.html
+-rw-r--r--   0        0        0     1921 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/post.html
+-rw-r--r--   0        0        0      116 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/robots.txt
+-rw-r--r--   0        0        0      578 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/sitemap.xml
+-rw-r--r--   0        0        0      771 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/www_handler.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/templates/admin.html
+-rw-r--r--   0        0        0      214 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/templates/map.html
+-rw-r--r--   0        0        0     1551 2023-05-31 13:00:58.717740 goodmap-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 goodmap-0.1.8/PKG-INFO
```

### Comparing `goodmap-0.1.7/README.md` & `goodmap-0.1.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,77 @@
-![Github Actions](https://github.com/problematy/goodmap/actions/workflows/python-app.yml/badge.svg)
+![Github Actions](https://github.com/problematy/goodmap/actions/workflows/tests.yml/badge.svg?event=push&branch=main)
 [![Coverage Status](https://coveralls.io/repos/github/Problematy/goodmap/badge.png)](https://coveralls.io/github/Problematy/goodmap)
 
 # Good Map
 
 Map engine to serve all the people ;) 
 
+## Setup
+
+Use python 3.10, install poetry: `pip install poetry` and then install dependencies: `poetry install`
+
 ## Running App locally
 
+### TL;DR
+If you don't want to go through all the configuration, e.g. you just simply want to test if everything works,
+you can simply run app with test dataset provided in `tests/e2e_tests` directory:
+
+> poetry run flask --app 'goodmap.goodmap:create_app(config_path="./tests/e2e_tests/e2e_test_config.yml")' run
+
 ### Configuration
 
-Rename config-template.yml to config.yml and change it's contents according to your needs.
+If you want to serve app with your configuration rename config-template.yml to config.yml and change its contents according to your needs.
 Values descriptions you can find inside config-template.yml.
 
-### Backend 
-
-All dependencies are specified in __pyproject.toml__ file. To install them in your onw environment:
-* go to project directory
-* use `poetry install`
-* get into poetry shell `poetry shell`
-* Run `FLASK_ENV=development;FLASK_APP=goodmap.goodmap flask run`
-
-### Frontend (optional)
-In production environment javascript is served as static files, but for ease of development you can run javascript
-server locally:
-* go to frontend directory
-* install all dependencies with `nmp install`
-* run server with `npm run serve`
-* set `development_overwrites` for wanted endpoints, otherwise application will use compiled files.
+Afterwards run it with:
+> poetry run flask --app 'goodmap.goodmap:create_app(config_path="/PATH/TO/YOUR/CONFIG")' --debug run
 
 ## Database
 
 Database consists of three sections:
 
 - `categories` - which informs on what categories data of points is divided
 - `visible_data` - list of categories which will be visible by application users
-- `data` - actual data splitted into `categories`
+- `data` - actual data split into `categories`
 
 
 ### `categories`
 Fully configurable map where key is name of category and value is list of allowed types. E.g.
 * "car_elements": ["mirror", "wheel", "steering wheel"]
 * "color": ["red", "blue", "green"]
 
 ### `data`
 Data consists of two parts:
 * obligatory and constant
   * `name` - name of the object
   * `position` - coordinates of object
 * category dependent - depending on your `categories` setup it varies. See example of config below.
 
-### Examples
+#### `custom data`
+You can define your own, more complex data types as dictionary.
+* obligatory fields in dictionary:
+  * `type` - type of data
+  * `value` - value of data
+* optional fields in dictionary:
+  * `displayValue` - value to display instead of `value`
+
+## Examples
+
 You can find examples of working configuration and database in `tests/e2e_tests` named:
 - `e2e_test_config.yml`
 - `e2e_test_data.json`
 
-## Version History
+# Version History
 
 ### 0.1 - Initial Release - in development
-#### 0.1.5 - in development
+
+#### 0.1.8 - in development
+  * unified frontend
+
+#### 0.1.5
   * better looking frontend
 
 #### 0.1.4 - Makeover
   * frontend for mobile version
 
 #### 0.1.3 - Simplification
   * Simplified and standarized configuration in code
```

### Comparing `goodmap-0.1.7/goodmap/core_api.py` & `goodmap-0.1.8/goodmap/core_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,50 @@
-from flask import Blueprint, request, jsonify
+from flask import Blueprint, jsonify, request
 from flask_babel import gettext
+from flask_restx import Api, Resource
+
+from goodmap.config import LanguagesMapping
+
 from .core import get_queried_data
 from .formatter import prepare_pin
 
 
 def make_tuple_translation(keys_to_translate):
     return [(x, gettext(x)) for x in keys_to_translate]
 
 
-def core_pages(database, languages):
-    core_api = Blueprint('core_api', __name__, url_prefix="/api")
+def core_pages(database, languages: LanguagesMapping) -> Blueprint:
+    core_api_blueprint = Blueprint("api", __name__, url_prefix="/api")
+    core_api = Api(core_api_blueprint, doc="/doc", version="0.1")
 
     @core_api.route("/data")
-    def get_data():
-        all_data = database.get_data()
-        query_params = request.args.to_dict(flat=False)
-        data = all_data["data"]
-        categories = all_data["categories"]
-        visible_data = all_data["visible_data"]
-        queried_data = get_queried_data(data, categories, query_params)
-        formatted_data = map(lambda x: prepare_pin(x, visible_data), queried_data)
-        return jsonify(list(formatted_data))
+    class Data(Resource):
+        def get(self):
+            all_data = database.get_data()
+            query_params = request.args.to_dict(flat=False)
+            data = all_data["data"]
+            categories = all_data["categories"]
+            visible_data = all_data["visible_data"]
+            queried_data = get_queried_data(data, categories, query_params)
+            formatted_data = [prepare_pin(x, visible_data) for x in queried_data]
+            return jsonify(formatted_data)
 
     @core_api.route("/categories")
-    def get_categories():
-        all_data = database.get_data()
-        categories = make_tuple_translation(all_data["categories"].keys())
-        return jsonify(categories)
+    class Categories(Resource):
+        def get(self):
+            all_data = database.get_data()
+            categories = make_tuple_translation(all_data["categories"].keys())
+            return jsonify(categories)
 
     @core_api.route("/languages")
-    def get_languages():
-        return jsonify(languages)
+    class Languages(Resource):
+        def get(self):
+            return jsonify(languages)
 
     @core_api.route("/category/<category_type>")
-    def get_category_types(category_type):
-        all_data = database.get_data()
-        local_data = make_tuple_translation(all_data["categories"][category_type])
-        return jsonify(local_data)
+    class CategoryTypes(Resource):
+        def get(self, category_type):
+            all_data = database.get_data()
+            local_data = make_tuple_translation(all_data["categories"][category_type])
+            return jsonify(local_data)
 
-    return core_api
+    return core_api_blueprint
```

### Comparing `goodmap-0.1.7/PKG-INFO` & `goodmap-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,102 @@
 Metadata-Version: 2.1
 Name: goodmap
-Version: 0.1.7
+Version: 0.1.8
 Summary: Map engine to serve all the people :)
 Author: Krzysztof Kolodzinski
 Author-email: krzysztof.kolodzinski@problematy.pl
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Babel (>=2.10.3,<3.0.0)
-Requires-Dist: Flask (>=2.1.1,<3.0.0)
+Requires-Dist: Flask (>=2.2.2,<3.0.0)
 Requires-Dist: Flask-Babel (>=2.0.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: google-cloud-storage (>=2.3.0,<3.0.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: flask-minify (>=0.41,<0.42)
+Requires-Dist: flask-restx (>=1.0.5,<2.0.0)
+Requires-Dist: flask-wtf (>=1.1.1,<2.0.0)
+Requires-Dist: google-cloud-storage (>=2.7.0,<3.0.0)
+Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
-Requires-Dist: platzky (>=0.1.12,<0.2.0)
-Requires-Dist: pytest (>=7.1.2,<8.0.0)
+Requires-Dist: humanize (>=4.6.0,<5.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
 
-![Github Actions](https://github.com/problematy/goodmap/actions/workflows/python-app.yml/badge.svg)
+![Github Actions](https://github.com/problematy/goodmap/actions/workflows/tests.yml/badge.svg?event=push&branch=main)
 [![Coverage Status](https://coveralls.io/repos/github/Problematy/goodmap/badge.png)](https://coveralls.io/github/Problematy/goodmap)
 
 # Good Map
 
 Map engine to serve all the people ;) 
 
+## Setup
+
+Use python 3.10, install poetry: `pip install poetry` and then install dependencies: `poetry install`
+
 ## Running App locally
 
+### TL;DR
+If you don't want to go through all the configuration, e.g. you just simply want to test if everything works,
+you can simply run app with test dataset provided in `tests/e2e_tests` directory:
+
+> poetry run flask --app 'goodmap.goodmap:create_app(config_path="./tests/e2e_tests/e2e_test_config.yml")' run
+
 ### Configuration
 
-Rename config-template.yml to config.yml and change it's contents according to your needs.
+If you want to serve app with your configuration rename config-template.yml to config.yml and change its contents according to your needs.
 Values descriptions you can find inside config-template.yml.
 
-### Backend 
-
-All dependencies are specified in __pyproject.toml__ file. To install them in your onw environment:
-* go to project directory
-* use `poetry install`
-* get into poetry shell `poetry shell`
-* Run `FLASK_ENV=development;FLASK_APP=goodmap.goodmap flask run`
-
-### Frontend (optional)
-In production environment javascript is served as static files, but for ease of development you can run javascript
-server locally:
-* go to frontend directory
-* install all dependencies with `nmp install`
-* run server with `npm run serve`
-* set `development_overwrites` for wanted endpoints, otherwise application will use compiled files.
+Afterwards run it with:
+> poetry run flask --app 'goodmap.goodmap:create_app(config_path="/PATH/TO/YOUR/CONFIG")' --debug run
 
 ## Database
 
 Database consists of three sections:
 
 - `categories` - which informs on what categories data of points is divided
 - `visible_data` - list of categories which will be visible by application users
-- `data` - actual data splitted into `categories`
+- `data` - actual data split into `categories`
 
 
 ### `categories`
 Fully configurable map where key is name of category and value is list of allowed types. E.g.
 * "car_elements": ["mirror", "wheel", "steering wheel"]
 * "color": ["red", "blue", "green"]
 
 ### `data`
 Data consists of two parts:
 * obligatory and constant
   * `name` - name of the object
   * `position` - coordinates of object
 * category dependent - depending on your `categories` setup it varies. See example of config below.
 
-### Examples
+#### `custom data`
+You can define your own, more complex data types as dictionary.
+* obligatory fields in dictionary:
+  * `type` - type of data
+  * `value` - value of data
+* optional fields in dictionary:
+  * `displayValue` - value to display instead of `value`
+
+## Examples
+
 You can find examples of working configuration and database in `tests/e2e_tests` named:
 - `e2e_test_config.yml`
 - `e2e_test_data.json`
 
-## Version History
+# Version History
 
 ### 0.1 - Initial Release - in development
-#### 0.1.5 - in development
+
+#### 0.1.8 - in development
+  * unified frontend
+
+#### 0.1.5
   * better looking frontend
 
 #### 0.1.4 - Makeover
   * frontend for mobile version
 
 #### 0.1.3 - Simplification
   * Simplified and standarized configuration in code
```

