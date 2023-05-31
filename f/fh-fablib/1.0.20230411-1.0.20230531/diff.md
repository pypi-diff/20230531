# Comparing `tmp/fh_fablib-1.0.20230411.tar.gz` & `tmp/fh_fablib-1.0.20230531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fh_fablib-1.0.20230411.tar", last modified: Tue Apr 11 12:23:25 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fh_fablib-1.0.20230411.tar` & `fh_fablib-1.0.20230531.tar`

### file list

```diff
@@ -1,25 +1,18 @@
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-11 12:23:25.927419 fh_fablib-1.0.20230411/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/LICENSE
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      198 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/MANIFEST.in
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7689 2023-04-11 12:23:25.927419 fh_fablib-1.0.20230411/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)     7322 2023-04-11 12:23:02.000000 fh_fablib-1.0.20230411/README.rst
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-11 12:23:25.926419 fh_fablib-1.0.20230411/fh_fablib/
--rw-r--r--   0 matthias  (1000) matthias  (1000)    26437 2023-04-11 12:23:02.000000 fh_fablib-1.0.20230411/fh_fablib/__init__.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-11 12:23:25.926419 fh_fablib-1.0.20230411/fh_fablib/dotfiles/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      200 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/.editorconfig
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      201 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/.eslintrc.js
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2013 2023-04-11 12:21:56.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-r--r--   0 matthias  (1000) matthias  (1000)      455 2023-04-11 12:21:56.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/pyproject.toml
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5820 2023-03-07 08:46:55.000000 fh_fablib-1.0.20230411/fh_fablib/dotfiles/webpack.library.js
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     2091 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/fh_fablib/extract_js_gettext_strings.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2023-04-11 12:23:25.926419 fh_fablib-1.0.20230411/fh_fablib.egg-info/
--rw-rw-r--   0 matthias  (1000) matthias  (1000)     7689 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/PKG-INFO
--rw-rw-r--   0 matthias  (1000) matthias  (1000)      538 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/SOURCES.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/dependency_links.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       47 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/entry_points.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2022-05-20 14:16:27.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/not-zip-safe
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       24 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/requires.txt
--rw-rw-r--   0 matthias  (1000) matthias  (1000)       10 2023-04-11 12:23:25.000000 fh_fablib-1.0.20230411/fh_fablib.egg-info/top_level.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)      465 2023-04-11 12:21:56.000000 fh_fablib-1.0.20230411/pyproject.toml
--rw-r--r--   0 matthias  (1000) matthias  (1000)      693 2023-04-11 12:23:25.927419 fh_fablib-1.0.20230411/setup.cfg
--rwxrwxr-x   0 matthias  (1000) matthias  (1000)       62 2022-05-20 14:16:22.000000 fh_fablib-1.0.20230411/setup.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.editorconfig
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    19496 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/CHANGELOG.rst
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/bumpversion.sh
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0    26558 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/__init__.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/extract_js_gettext_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/.editorconfig
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/.eslintrc.js
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/fh_fablib/dotfiles/webpack.library.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/LICENSE
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/README.rst
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/pyproject.toml
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230531/PKG-INFO
```

### Comparing `fh_fablib-1.0.20230411/LICENSE` & `fh_fablib-1.0.20230531/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230411/PKG-INFO` & `fh_fablib-1.0.20230531/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: fh_fablib
-Version: 1.0.20230411
-Summary: fh-fablib
-Home-page: https://github.com/feinheit/fh-fablib/
-Author: Matthias Kestenholz
-Author-email: mk@feinheit.ch
-License: BSD-3-Clause
-Platform: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 =========
 fh-fablib
 =========
 
 Usage
 =====
 
@@ -28,15 +14,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230411")
+       fl.require("1.0.20230531")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +90,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230411")
+    fl.require("1.0.20230531")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230411/README.rst` & `fh_fablib-1.0.20230531/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: fh-fablib
+Version: 1.0.20230531
+Summary: fh-fablib
+Project-URL: Homepage, https://github.com/feinheit/fh-fablib/
+Author-email: Matthias Kestenholz <mk@feinheit.ch>
+License: BSD-3-Clause
+License-File: LICENSE
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.9
+Requires-Dist: fabric>=3
+Requires-Dist: speckenv>=3.3
+Description-Content-Type: text/x-rst
+
 =========
 fh-fablib
 =========
 
 Usage
 =====
 
@@ -14,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230411")
+       fl.require("1.0.20230531")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -90,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230411")
+    fl.require("1.0.20230531")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230411/fh_fablib/__init__.py` & `fh_fablib-1.0.20230531/fh_fablib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa, re-export
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20230411"
+__version__ = "1.0.20230531"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
@@ -343,15 +343,15 @@
     help={"language": "Generate catalogs for a specific language"},
 )
 def mm(ctx, language=None):
     """Update the translation catalogs"""
 
     with open("conf/strings.js", "w", encoding="utf-8") as f:
         f.write("/* eslint-disable */\n")
-        f.write("".join(f"{str}\n" for str in generate_strings()))
+        f.write("".join(f"{string}\n" for string in generate_strings()))
 
     language = f"-l {language}" if language else "-a"
     run_local(
         ctx,
         f"venv/bin/python manage.py makemessages {language} --add-location file"
         " -i venv -i htmlcov -i node_modules -i lib -i build -i dist --no-wrap",
         replace_env=False,
@@ -754,17 +754,19 @@
                 conn,
                 f'source ~/.profile && psql -c "CREATE DATABASE {dbname} WITH'
                 f" OWNER {dbname} TEMPLATE template0 ENCODING 'UTF8'"
                 f'"',
             )
 
         run(conn, f"pg_dump -Ox {source_dsn} | psql {target_dsn}")
+        media_source = f"{source['domain']}/media/"
+        media_target = f"{config.domain}/media/"
         run(
             conn,
-            f"rsync -aH --stats {source['domain']}/media/ {config.domain}/media/",
+            f"rsync -aH --stats --link-dest=`pwd`/{media_source} {media_source} {media_target}",
         )
     progress(f"Success! (A database backup is at {config.domain}/tmp/)")
     progress("You may have to run nine-restart or even deploy once.")
 
 
 @task
 def nine(ctx):
```

### Comparing `fh_fablib-1.0.20230411/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20230531/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,19 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-added-large-files
       - id: check-builtin-literals
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
+      - id: check-toml
+      - id: check-yaml
       - id: detect-private-key
       - id: end-of-file-fixer
+      - id: mixed-line-ending
       - id: trailing-whitespace
       - id: file-contents-sorter
         files: requirements-to-freeze.txt
   - repo: local
     hooks:
       - id: django-check
         name: django check
@@ -26,23 +29,23 @@
       - id: django-upgrade
         args: [--target-version, "4.0"]
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.1
     hooks:
       - id: absolufy-imports
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.261"
+    rev: "v0.0.270"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.38.0
+    rev: v8.41.0
     hooks:
       - id: eslint
         args: [--fix]
         types_or: [css, scss, javascript]
         verbose: true
         additional_dependencies:
           - eslint
@@ -57,12 +60,20 @@
           - "@babel/preset-env"
           - "@babel/preset-react"
           - "@babel/plugin-syntax-class-properties"
           - "@babel/plugin-syntax-decorators"
           - "@babel/plugin-syntax-jsx"
           - jest
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
-        exclude: "^conf/|.*\\.html$"
+        exclude: "^conf/|.*\\.html$|.*\\.json$"
+  - repo: https://github.com/tox-dev/pyproject-fmt
+    rev: 0.11.2
+    hooks:
+      - id: pyproject-fmt
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.13
+    hooks:
+      - id: validate-pyproject
```

### Comparing `fh_fablib-1.0.20230411/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20230531/fh_fablib/dotfiles/webpack.library.js`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230411/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20230531/fh_fablib/extract_js_gettext_strings.py`

 * *Files identical despite different names*

