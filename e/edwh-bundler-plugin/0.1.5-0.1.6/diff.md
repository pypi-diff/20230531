# Comparing `tmp/edwh_bundler_plugin-0.1.5.tar.gz` & `tmp/edwh_bundler_plugin-0.1.6.tar.gz`

## Comparing `edwh_bundler_plugin-0.1.5.tar` & `edwh_bundler_plugin-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/__init__.py
--rw-r--r--   0        0        0    19514 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/bundler_plugin.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/css.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/js.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/shared.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/README.md
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/__init__.py
+-rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/bundler_plugin.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/css.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/js.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/shared.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/README.md
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/PKG-INFO
```

### Comparing `edwh_bundler_plugin-0.1.5/CHANGELOG.md` & `edwh_bundler_plugin-0.1.6/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.6 (2023-05-31)
+
+
 ## v0.1.5 (2023-04-17)
 
 
 ## v0.1.4 (2023-04-17)
 ### Fix
 * **project:** Remove theoretical support for Python versions below 3.10 since that has never worked ([`daa3e39`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/daa3e39abe7627a09c93ccfeb42e164612c14b6c))
```

### Comparing `edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/bundler_plugin.py` & `edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/bundler_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,33 +69,48 @@
         f.close()
 
 
 def cli_or_config(
     value: typing.Any,
     config: dict,
     key: typing.Hashable,
-    bool=True,
+    bool: bool = True,
     default: typing.Any = None,
 ) -> bool | typing.Any:
     """
     Get a setting from either the config yaml or the cli (used to override config)
     cli > config > default
 
     Args:
         value: the value from cli, will override config if anything other than None
         config: the 'config' section of the config yaml
         key: config key to look in (under the 'config' section)
-        bool: should the result alwasy be a boolean? Useful cli arguments such as --cache y,
+        bool: should the result always be a boolean? Useful cli arguments such as --cache y,
                      but should probably be False for named arguments such as --filename ...
         default: if the option can be found in neither the cli arguments or the config file, what should the value be?
     """
     return (truthy(value) if bool else value) if value is not None else config.get(key, default)
 
 
-def _fill_variables(setting: str | dict, variables: dict[re.Pattern, str]) -> str:
+@typing.overload
+def _fill_variables(setting: str, variables: dict[re.Pattern, str]) -> str:
+    """
+    If a string is passed as setting, the $variables in the string are filled.
+    E.g. "$in_app/path/to/css" + {'in_app': 'apps/cmsx'} -> 'apps/cmsx/path/to/css'
+    """
+
+
+@typing.overload
+def _fill_variables(setting: dict, variables: dict[re.Pattern, str]) -> dict[str, str]:
+    """
+    If a dict of settings is passed, all values are filled. Keys are left alone.
+    """
+
+
+def _fill_variables(setting: str | dict, variables: dict[re.Pattern, str]) -> str | dict[str, str]:
     """
     Fill in $variables in a dynamic setting.
     E.g. "$in_app/path/to/css" + {'in_app': 'apps/cmsx'} -> 'apps/cmsx/path/to/css'
     """
     if isinstance(setting, dict):
         # recursive fill nested values:
         return {k: _fill_variables(v, variables) for k, v in setting.items()}
@@ -105,15 +120,18 @@
 
     for reg, repl in variables.items():
         setting = reg.sub(str(repl), setting)
 
     return setting
 
 
-def _regexify_settings(setting_dict: dict) -> dict:
+def _regexify_settings(setting_dict: dict[str, typing.Any]) -> dict[re.Pattern, typing.Any]:
+    """
+    Convert a dict keys from string to a compiled regex pattern (/$string/)
+    """
     return {re.compile(rf"\${key}"): value for key, value in setting_dict.items()}
 
 
 def _handle_files(
     files: list,
     callback: typing.Callable,
     output: str | typing.IO,
@@ -378,24 +396,21 @@
 
 
 def dict_factory(cursor, row):
     return {col[0]: row[idx] for idx, col in enumerate(cursor.description)}
 
 
 def assert_chmod_777(c: Context, filepath: str | list[str]):
-    if isinstance(filepath, str):
-        filepaths = [filepath]
-    else:
-        filepaths = filepath
+    filepaths: list[str] = [filepath] if isinstance(filepath, str) else filepath
 
-    for filepath in filepaths:
-        resp = c.run(f'stat --format "%a  %n" {filepath}', hide=True)
+    for fp in filepaths:
+        resp = c.run(f'stat --format "%a  %n" {fp}', hide=True)
         chmod = resp.stdout.split(" ")[0]
         if chmod != 777:
-            c.sudo(f"chmod 777 {filepath}")
+            c.sudo(f"chmod 777 {fp}")
 
 
 def assert_file_exists(c: Context, db_filepath: str, sql_filepath: str):
     if not os.path.exists(db_filepath):
         # load existing
         c.run(f"sqlite3 {db_filepath} < {sql_filepath}")
 
@@ -442,15 +457,15 @@
 
     sql: invoke.Result = c.run(f"sqlite3 {db_path} .dump", hide=True)
 
     with open(sql_path, "w", encoding="UTF-8") as f:
         f.write(sql.stdout)
 
 
-@task
+@task()
 def update_assets_sql(c):
     # db = setup_db(c)
     _update_assets_sql(c)
 
 
 def insert_version(c: invoke.context.Context, db: sqlite3.Connection, values: dict):
     columns = ", ".join(values.keys())
@@ -523,15 +538,15 @@
         int(groups[0][1].strip(".") or 0),
         int(groups[0][2].strip(".") or 0),
     )
     version = f"{major}.{minor}.{patch}"
     return major, minor, patch, version
 
 
-def file_hash(c: Context, filename: str):
+def calculate_file_hash(c: Context, filename: str):
     return c.run(f"sha1sum {filename}", hide=True).stdout.split(" ")[0]
 
 
 @task()
 def publish(
     c,
     version=None,
@@ -621,49 +636,51 @@
     rmtree(TEMP_OUTPUT_DIR)
 
     # after publish: run `up -s py4web` so the bjoerns are all updated
     c.run("inv up -s py4web")
 
 
 def _should_publish(c: Context, force: bool, output_path: str, previous_hash: str, type: typing.Literal["JS", "CSS"]):
-    hash = file_hash(c, output_path)
-    if hash == previous_hash:
+    file_hash = calculate_file_hash(c, output_path)
+    if file_hash == previous_hash:
         print(f"{type} hash matches previous version.")
         go = confirm("Are you sure you want to release a new version? ", force)
     else:
         go = True
     if not go:
         return False, None, None, None
 
     # if go:
 
     with open(output_path, "r", encoding="UTF-8") as f:
         file_contents = f.read()
 
     filename = output_path.split("/")[-1]
 
-    return True, hash, filename, file_contents
+    return True, file_hash, filename, file_contents
 
 
-@task
-def list(c):
+@task(name="list")
+def list_versions(c):
     db = setup_db(c)
     for row in db.execute(
         "SELECT filetype, version FROM bundle_version ORDER BY major DESC, minor DESC, patch DESC"
     ).fetchall():
         print(row)
 
 
-@task
+@task()
 def reset(c):
     db = setup_db(c)
     if not confirm("Are you sure you want to reset the versions database? "):
         print("Wise.")
         return
 
+    # noinspection SqlWithoutWhere
+    # ^ that's the whole point of 'reset'.
     db.execute("DELETE FROM bundle_version;")
     db.commit()
     _update_assets_sql(c)
 
     assert db.execute("SELECT COUNT(*) as c FROM bundle_version;").fetchone()["c"] == 0
```

### Comparing `edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/css.py` & `edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/css.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/js.py` & `edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/js.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.5/src/edwh_bundler_plugin/shared.py` & `edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,32 +40,31 @@
     """
     Download contents from some url or from cache if possible/desired
 
     Args:
         url (str): online resource location
         cache (bool): use .cdn_cache if possible?
     """
-    if cache:
-        h_url = str(cache_hash(url))
-
-        cache_path = CACHE_DIR / h_url
-        if cache_path.exists():
-            return extract_contents_local(str(cache_path))
-        else:
-            _resp = _extract_contents_cdn(url)
-
-            if not CACHE_DIR.exists():
-                os.mkdir(CACHE_DIR)
-
-            with open(cache_path, "w") as f:
-                f.write(_resp)
-            return _resp
-    else:
+    if not cache:
         return _extract_contents_cdn(url)
 
+    h_url = str(cache_hash(url))
+
+    cache_path = CACHE_DIR / h_url
+    if cache_path.exists():
+        return extract_contents_local(str(cache_path))
+    _resp = _extract_contents_cdn(url)
+
+    if not CACHE_DIR.exists():
+        os.mkdir(CACHE_DIR)
+
+    with open(cache_path, "w") as f:
+        f.write(_resp)
+    return _resp
+
 
 def extract_contents_local(path: str) -> str:
     """
     Read a file from disk
     """
     with open(path) as f:
         return f.read()
```

### Comparing `edwh_bundler_plugin-0.1.5/LICENSE.txt` & `edwh_bundler_plugin-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.5/README.md` & `edwh_bundler_plugin-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.5/pyproject.toml` & `edwh_bundler_plugin-0.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,24 @@
   { name = "Remco Boerma", email = "remco.b@educationwarehouse.nl" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['invoke', 'python-dotenv', 'pysass', 'rjsmin', 'httpx', 'pyyaml']
 
 [project.optional-dependencies]
 dev = [
   "hatch",
-  "python-semantic-release",
+  # "python-semantic-release",
   "black",
 ]
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/edwh-bundler-plugin#readme"
 Issues = "https://github.com/educationwarehouse/edwh-bundler-plugin/issues"
 Source = "https://github.com/educationwarehouse/edwh-bundler-plugin"
@@ -74,15 +75,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.10", "3.11"]
+python = ["3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
```

### Comparing `edwh_bundler_plugin-0.1.5/PKG-INFO` & `edwh_bundler_plugin-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: edwh-bundler-plugin
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python-only static file (js, css) bundler for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-bundler-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-bundler-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-bundler-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: httpx
 Requires-Dist: invoke
 Requires-Dist: pysass
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Requires-Dist: rjsmin
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
-Requires-Dist: python-semantic-release; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # edwh-bundler-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-bundler-plugin.svg)](https://pypi.org/project/edwh-bundler-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-bundler-plugin.svg)](https://pypi.org/project/edwh-bundler-plugin)
```

