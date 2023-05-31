# Comparing `tmp/mdast_cli_core-2022.8.8.tar.gz` & `tmp/mdast_cli_core-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mdast-cli-core/mdast-cli-core/dist/tmpof2chgk3/mdast_cli_core-2022.8.8.tar", last modified: Fri Oct  7 12:04:13 2022, max compression
+gzip compressed data, was "mdast_cli_core-2023.5.1.tar", last modified: Wed May 31 09:56:36 2023, max compression
```

## Comparing `mdast_cli_core-2022.8.8.tar` & `mdast_cli_core-2023.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/
--rw-r--r--   0 runner    (1001) docker     (116)      879 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      511 2022-10-07 12:04:04.000000 mdast_cli_core-2022.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/mdast_cli_core/
--rw-r--r--   0 runner    (1001) docker     (116)       84 2022-10-07 12:04:04.000000 mdast_cli_core-2022.8.8/mdast_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2022-10-07 12:04:04.000000 mdast_cli_core-2022.8.8/mdast_cli_core/api.py
--rw-r--r--   0 runner    (1001) docker     (116)    25115 2022-10-07 12:04:04.000000 mdast_cli_core-2022.8.8/mdast_cli_core/base.py
--rw-r--r--   0 runner    (1001) docker     (116)      574 2022-10-07 12:04:04.000000 mdast_cli_core-2022.8.8/mdast_cli_core/token.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/mdast_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      879 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/mdast_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      313 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/mdast_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/mdast_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/mdast_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/mdast_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-10-07 12:04:13.000000 mdast_cli_core-2022.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      686 2022-10-07 12:04:04.000000 mdast_cli_core-2022.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:36.207982 mdast_cli_core-2023.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 09:56:36.207982 mdast_cli_core-2023.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:36.203982 mdast_cli_core-2023.5.1/mdast_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/mdast_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/mdast_cli_core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/mdast_cli_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/mdast_cli_core/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:36.207982 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 09:56:36.000000 mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:56:36.207982 mdast_cli_core-2023.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-31 09:56:27.000000 mdast_cli_core-2023.5.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mdast_cli_core-2022.8.8/PKG-INFO` & `mdast_cli_core-2023.5.1/mdast_cli_core.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mdast_cli_core
-Version: 2022.8.8
+Name: mdast-cli-core
+Version: 2023.5.1
 Summary: mDast core package
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli-core
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli_core-2022.8.8/mdast_cli_core/api.py` & `mdast_cli_core-2023.5.1/mdast_cli_core/api.py`

 * *Files identical despite different names*

### Comparing `mdast_cli_core-2022.8.8/mdast_cli_core/base.py` & `mdast_cli_core-2023.5.1/mdast_cli_core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,39 @@
                             verify=False)
 
     def get_engines(self):
         return requests.get(f'{self.url}/organizations/{self.current_context["company"]}/engines/',
                             headers=self.headers,
                             verify=False)
 
+    def engine_create(self, name, architecture):
+        data = {
+            "name": name,
+            "architecture": architecture
+        }
+        return requests.post(f'{self.url}/organizations/{self.current_context["company"]}/engines/',
+                             headers=self.headers,
+                             data=json.dumps(data),
+                             verify=False)
+
+    def get_engine(self, engine_id):
+        return requests.get(f'{self.url}/engines/{engine_id}/',
+                            headers=self.headers,
+                            verify=False)
+
+    def engine_management(self, engine_id, action):
+        return requests.get(f'{self.url}/engines/{engine_id}/{action}/',
+                            headers=self.headers,
+                            verify=False)
+
+    def engine_delete(self, engine_id):
+        return requests.delete(f'{self.url}/engines/{engine_id}/',
+                               headers=self.headers,
+                               verify=False)
+
     def get_organizations(self):
         return requests.get(f'{self.url}/organizations/',
                             headers=self.headers,
                             verify=False)
 
     def get_organization(self, organization_id):
         return requests.get(f'{self.url}/organizations/{organization_id}/',
@@ -600,8 +625,18 @@
                             headers=self.headers,
                             verify=False)
         return resp
 
     def get_issue_info(self, issue_id):
         return requests.get(f'{self.url}/dast_issues/{issue_id}/',
                             headers=self.headers,
-                            verify=False)
+                            verify=False)
+
+    def get_localization_issue_data_keys(self):
+        return requests.get(f'{self.url}/localization/issue_data_keys',
+                            headers=self.headers,
+                            verify=False)
+
+    def get_modules(self):
+        return requests.get(f'{self.url}/modules/',
+                            headers=self.headers,
+                            verify=False)
```

### Comparing `mdast_cli_core-2022.8.8/mdast_cli_core/token.py` & `mdast_cli_core-2023.5.1/mdast_cli_core/token.py`

 * *Files identical despite different names*

### Comparing `mdast_cli_core-2022.8.8/mdast_cli_core.egg-info/PKG-INFO` & `mdast_cli_core-2023.5.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mdast-cli-core
-Version: 2022.8.8
+Name: mdast_cli_core
+Version: 2023.5.1
 Summary: mDast core package
 Home-page: https://github.com/Dynamic-Mobile-Security/mdast-cli-core
 Author: Dynamic-Mobile-Security
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
```

### Comparing `mdast_cli_core-2022.8.8/setup.py` & `mdast_cli_core-2023.5.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mdast_cli_core",
-    version='2022.08.8',
+    version='2023.05.01',
     author="Dynamic-Mobile-Security",
     description="mDast core package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dynamic-Mobile-Security/mdast-cli-core",
     packages=find_packages(),
     include_package_data=True,
```

