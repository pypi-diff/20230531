# Comparing `tmp/timona-0.0.3.tar.gz` & `tmp/timona-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timona-0.0.3.tar", max compression
+gzip compressed data, was "timona-0.0.4.tar", max compression
```

## Comparing `timona-0.0.3.tar` & `timona-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.3/LICENSE
--rw-r--r--   0        0        0       46 2023-05-26 12:19:29.287039 timona-0.0.3/README.md
--rw-r--r--   0        0        0      542 2023-05-29 08:13:17.409564 timona-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.3/timona/__init__.py
--rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.3/timona/__main__.py
--rw-r--r--   0        0        0       38 2023-05-29 08:13:17.413564 timona-0.0.3/timona/__version__.py
--rw-r--r--   0        0        0     1177 2023-05-28 07:24:27.978336 timona-0.0.3/timona/config.py
--rw-r--r--   0        0        0     2715 2023-05-26 12:19:29.311040 timona-0.0.3/timona/helm.py
--rw-r--r--   0        0        0     2766 2023-05-26 13:16:03.924441 timona-0.0.3/timona/main.py
--rw-r--r--   0        0        0     4946 2023-05-29 07:37:05.204532 timona-0.0.3/timona/releases.py
--rw-r--r--   0        0        0     1408 2023-05-29 07:40:45.722364 timona-0.0.3/timona/template.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 timona-0.0.3/setup.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 timona-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 12:17:14.109740 timona-0.0.4/LICENSE
+-rw-r--r--   0        0        0      104 2023-05-30 12:02:34.562872 timona-0.0.4/README.md
+-rw-r--r--   0        0        0      542 2023-05-31 06:58:01.033207 timona-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 13:27:02.242952 timona-0.0.4/timona/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-26 12:53:23.927626 timona-0.0.4/timona/__main__.py
+-rw-r--r--   0        0        0       38 2023-05-31 06:58:01.033207 timona-0.0.4/timona/__version__.py
+-rw-r--r--   0        0        0     1228 2023-05-30 14:40:01.114338 timona-0.0.4/timona/config.py
+-rw-r--r--   0        0        0     2715 2023-05-30 12:27:04.454612 timona-0.0.4/timona/helm.py
+-rw-r--r--   0        0        0     2771 2023-05-30 14:15:58.083494 timona-0.0.4/timona/main.py
+-rw-r--r--   0        0        0     5236 2023-05-30 14:50:19.327125 timona-0.0.4/timona/releases.py
+-rw-r--r--   0        0        0     2463 2023-05-30 14:56:57.258194 timona-0.0.4/timona/template/__init__.py
+-rw-r--r--   0        0        0      201 2023-05-30 14:57:24.210402 timona-0.0.4/timona/template/module_jinja2.py
+-rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 timona-0.0.4/setup.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 timona-0.0.4/PKG-INFO
```

### Comparing `timona-0.0.3/LICENSE` & `timona-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `timona-0.0.3/pyproject.toml` & `timona-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timona"
-version = "0.0.3"
+version = "0.0.4"
 description = "Tool to automate Helm deployments"
 authors = ["mihaiush <mihaiush@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/mihaiush/timona"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `timona-0.0.3/timona/config.py` & `timona-0.0.4/timona/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 
 def load_config_file(c):
     _data = []
 
     def _load_config(c):
         if c.startswith('http://') or c.startswith('https://'):
-            r = requests.get(c)
+            r = requests.get(c, timeout=(0.5, 5))
+            r.raise_for_status()
             cfg = r.text
         else:
             with open(c) as f:
                 cfg = f.read()
         for ln in cfg.split('\n'):
             ln = ln.rstrip()
             if ln.startswith('#+'):
```

### Comparing `timona-0.0.3/timona/helm.py` & `timona-0.0.4/timona/helm.py`

 * *Files identical despite different names*

### Comparing `timona-0.0.3/timona/main.py` & `timona-0.0.4/timona/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             usage()
         R = sys.argv[2]
 
     CONFIG = load_config()
 
     TMP = '{}/.timona'.format(CONFIG['config']['tmp'])
     os.makedirs(TMP, exist_ok=True)
-    T = Template(CONFIG['config']['template'])
+    T = Template(CONFIG['config']['template'], TMP)
     H = Helm(CONFIG['config']['helm'], T, TMP)
 
     if CMD == 'version':
         print('timona: {}'.format(version))
         print('template: {}'.format(T.version))
         print('helm: {}'.format(H.version))
         print('helm: diff: {}'.format(H.version_diff))
```

### Comparing `timona-0.0.3/timona/releases.py` & `timona-0.0.4/timona/releases.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,14 +89,23 @@
                 for matrix in data['matrix']:
                     flat_matrix = flatten_matrix(matrix)
                     for release_matrix in flat_matrix:
                         out.append({**release_template, **release_matrix})
             else:
                 out.append(release_template)
 
+        # Remove empty vars
+        for release in out:
+            to_del = []
+            for var_name, var_value in release.items():
+                if not var_value:
+                    to_del.append(var_name)
+            for var_name in to_del:
+                del(release[var_name])
+
         # Solve vars, each release in a thread
         _releases = []
         threads = []
         for release in out:
             x = {
                 't': None,    # thread
                 'r': {        # solved vars release
```

### Comparing `timona-0.0.3/setup.py` & `timona-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['timona']
+['timona', 'timona.template']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['deepmerge', 'jinja2', 'pyyaml', 'requests']
 
 entry_points = \
 {'console_scripts': ['timona = timona.main:main']}
 
 setup_kwargs = {
     'name': 'timona',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Tool to automate Helm deployments',
-    'long_description': '# timona\n\nA tool to automate Helm deployments\n',
+    'long_description': '# timona\n\nA tool to automate Helm deployments.\n\nFor usage see https://github.com/mihaiush/timona/wiki .\n',
     'author': 'mihaiush',
     'author_email': 'mihaiush@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mihaiush/timona',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `timona-0.0.3/PKG-INFO` & `timona-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timona
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to automate Helm deployments
 Home-page: https://github.com/mihaiush/timona
 Author: mihaiush
 Author-email: mihaiush@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -16,9 +16,11 @@
 Requires-Dist: jinja2
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # timona
 
-A tool to automate Helm deployments
+A tool to automate Helm deployments.
+
+For usage see https://github.com/mihaiush/timona/wiki .
```

