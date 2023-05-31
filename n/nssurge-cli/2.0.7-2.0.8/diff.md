# Comparing `tmp/nssurge_cli-2.0.7.tar.gz` & `tmp/nssurge_cli-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge_cli-2.0.7.tar", max compression
+gzip compressed data, was "nssurge_cli-2.0.8.tar", max compression
```

## Comparing `nssurge_cli-2.0.7.tar` & `nssurge_cli-2.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1100 2023-05-05 05:39:14.369260 nssurge_cli-2.0.7/LICENSE
--rw-r--r--   0        0        0        0 2023-05-05 05:39:14.369608 nssurge_cli-2.0.7/README.md
--rw-r--r--   0        0        0      294 2023-05-31 14:14:53.685444 nssurge_cli-2.0.7/nssurge_cli/__init__.py
--rw-r--r--   0        0        0     2693 2023-05-31 14:11:37.772708 nssurge_cli-2.0.7/nssurge_cli/cap_commands.py
--rw-r--r--   0        0        0     1994 2023-05-31 08:11:06.194486 nssurge_cli-2.0.7/nssurge_cli/cli.py
--rw-r--r--   0        0        0     2778 2023-05-31 13:31:26.294601 nssurge_cli-2.0.7/nssurge_cli/config.py
--rw-r--r--   0        0        0     3328 2023-05-31 14:12:52.578041 nssurge_cli-2.0.7/nssurge_cli/devices_commands.py
--rw-r--r--   0        0        0     1620 2023-05-31 14:12:52.435392 nssurge_cli-2.0.7/nssurge_cli/dns_commands.py
--rw-r--r--   0        0        0     1900 2023-05-31 14:12:52.124716 nssurge_cli-2.0.7/nssurge_cli/global_commands.py
--rw-r--r--   0        0        0     4172 2023-05-31 14:12:52.577967 nssurge_cli-2.0.7/nssurge_cli/group_commands.py
--rw-r--r--   0        0        0     4558 2023-05-31 14:12:52.645195 nssurge_cli-2.0.7/nssurge_cli/misc_commands.py
--rw-r--r--   0        0        0     2208 2023-05-31 14:12:52.396396 nssurge_cli-2.0.7/nssurge_cli/modules_commands.py
--rw-r--r--   0        0        0     1596 2023-05-31 14:12:52.557423 nssurge_cli-2.0.7/nssurge_cli/outbound_commands.py
--rw-r--r--   0        0        0     4966 2023-05-31 14:12:52.504091 nssurge_cli-2.0.7/nssurge_cli/policy_commands.py
--rw-r--r--   0        0        0     3166 2023-05-31 14:12:52.462754 nssurge_cli-2.0.7/nssurge_cli/profiles_commands.py
--rw-r--r--   0        0        0     3064 2023-05-31 14:12:52.647586 nssurge_cli-2.0.7/nssurge_cli/requests_commands.py
--rw-r--r--   0        0        0     1338 2023-05-31 14:12:52.145411 nssurge_cli-2.0.7/nssurge_cli/scripting_commands.py
--rw-r--r--   0        0        0     1978 2023-05-31 14:12:51.865239 nssurge_cli-2.0.7/nssurge_cli/test_commands.py
--rw-r--r--   0        0        0      265 2023-05-05 05:39:14.373640 nssurge_cli-2.0.7/nssurge_cli/types.py
--rw-r--r--   0        0        0     1877 2023-05-31 14:12:51.902751 nssurge_cli-2.0.7/nssurge_cli/utils.py
--rw-r--r--   0        0        0     1087 2023-05-31 14:14:53.684489 nssurge_cli-2.0.7/pyproject.toml
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 nssurge_cli-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-05 05:39:14.369260 nssurge_cli-2.0.8/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-05 05:39:14.369608 nssurge_cli-2.0.8/README.md
+-rw-r--r--   0        0        0      294 2023-05-31 14:17:42.846004 nssurge_cli-2.0.8/nssurge_cli/__init__.py
+-rw-r--r--   0        0        0     2693 2023-05-31 14:11:37.772708 nssurge_cli-2.0.8/nssurge_cli/cap_commands.py
+-rw-r--r--   0        0        0     1994 2023-05-31 08:11:06.194486 nssurge_cli-2.0.8/nssurge_cli/cli.py
+-rw-r--r--   0        0        0     2778 2023-05-31 13:31:26.294601 nssurge_cli-2.0.8/nssurge_cli/config.py
+-rw-r--r--   0        0        0     3328 2023-05-31 14:12:52.578041 nssurge_cli-2.0.8/nssurge_cli/devices_commands.py
+-rw-r--r--   0        0        0     1620 2023-05-31 14:12:52.435392 nssurge_cli-2.0.8/nssurge_cli/dns_commands.py
+-rw-r--r--   0        0        0     1900 2023-05-31 14:12:52.124716 nssurge_cli-2.0.8/nssurge_cli/global_commands.py
+-rw-r--r--   0        0        0     4172 2023-05-31 14:12:52.577967 nssurge_cli-2.0.8/nssurge_cli/group_commands.py
+-rw-r--r--   0        0        0     4558 2023-05-31 14:12:52.645195 nssurge_cli-2.0.8/nssurge_cli/misc_commands.py
+-rw-r--r--   0        0        0     2208 2023-05-31 14:12:52.396396 nssurge_cli-2.0.8/nssurge_cli/modules_commands.py
+-rw-r--r--   0        0        0     1596 2023-05-31 14:12:52.557423 nssurge_cli-2.0.8/nssurge_cli/outbound_commands.py
+-rw-r--r--   0        0        0     4966 2023-05-31 14:12:52.504091 nssurge_cli-2.0.8/nssurge_cli/policy_commands.py
+-rw-r--r--   0        0        0     3166 2023-05-31 14:12:52.462754 nssurge_cli-2.0.8/nssurge_cli/profiles_commands.py
+-rw-r--r--   0        0        0     3064 2023-05-31 14:12:52.647586 nssurge_cli-2.0.8/nssurge_cli/requests_commands.py
+-rw-r--r--   0        0        0     1338 2023-05-31 14:12:52.145411 nssurge_cli-2.0.8/nssurge_cli/scripting_commands.py
+-rw-r--r--   0        0        0     1978 2023-05-31 14:12:51.865239 nssurge_cli-2.0.8/nssurge_cli/test_commands.py
+-rw-r--r--   0        0        0      265 2023-05-05 05:39:14.373640 nssurge_cli-2.0.8/nssurge_cli/types.py
+-rw-r--r--   0        0        0     1877 2023-05-31 14:12:51.902751 nssurge_cli-2.0.8/nssurge_cli/utils.py
+-rw-r--r--   0        0        0     1104 2023-05-31 14:17:42.845532 nssurge_cli-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 nssurge_cli-2.0.8/PKG-INFO
```

### Comparing `nssurge_cli-2.0.7/LICENSE` & `nssurge_cli-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/cap_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/cap_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/cli.py` & `nssurge_cli-2.0.8/nssurge_cli/cli.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/config.py` & `nssurge_cli-2.0.8/nssurge_cli/config.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/devices_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/devices_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/dns_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/dns_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/global_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/global_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/group_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/group_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/misc_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/misc_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/modules_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/modules_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/outbound_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/outbound_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/policy_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/policy_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/profiles_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/profiles_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/requests_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/requests_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/scripting_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/scripting_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/test_commands.py` & `nssurge_cli-2.0.8/nssurge_cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/nssurge_cli/utils.py` & `nssurge_cli-2.0.8/nssurge_cli/utils.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.7/pyproject.toml` & `nssurge_cli-2.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nssurge-cli"
-version = "2.0.7"
+version = "2.0.8"
 description = "NSSurge CLI"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/nssurge-cli"
 repository = "https://github.com/tddschn/nssurge-cli"
 classifiers = ["Topic :: Utilities"]
@@ -18,14 +18,15 @@
 "Bug Tracker" = "https://github.com/tddschn/nssurge-cli/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.11, <4.0"
 nssurge-api = "^0.2.14"
 utils-tddschn = "^0.1.5"
 rich = { version = "^12.4.1", extras = ["format"] }
+typer = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 toml = "^0.10.2"
 yapf = "^0.32.0"
 better-exceptions = "^0.3.3"
 bump2version = "^1.0.1"
 logging-utils-tddschn = "^0.1.8"
```

### Comparing `nssurge_cli-2.0.7/PKG-INFO` & `nssurge_cli-2.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nssurge-cli
-Version: 2.0.7
+Version: 2.0.8
 Summary: NSSurge CLI
 Home-page: https://github.com/tddschn/nssurge-cli
 License: MIT
 Keywords: nssurge,cli,surge,typer
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: nssurge-api (>=0.2.14,<0.3.0)
 Requires-Dist: rich[format] (>=12.4.1,<13.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: utils-tddschn (>=0.1.5,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/nssurge-cli/issues
 Project-URL: Repository, https://github.com/tddschn/nssurge-cli
 Description-Content-Type: text/markdown
```

