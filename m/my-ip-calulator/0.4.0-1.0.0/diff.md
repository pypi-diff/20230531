# Comparing `tmp/my_ip_calulator-0.4.0.tar.gz` & `tmp/my_ip_calulator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_ip_calulator-0.4.0.tar", max compression
+gzip compressed data, was "my_ip_calulator-1.0.0.tar", max compression
```

## Comparing `my_ip_calulator-0.4.0.tar` & `my_ip_calulator-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-30 23:41:14.070516 my_ip_calulator-0.4.0/LICENSE
--rw-r--r--   0        0        0    31616 2023-05-31 00:34:10.649805 my_ip_calulator-0.4.0/README.md
--rw-r--r--   0        0        0     7769 2023-05-31 20:22:51.763688 my_ip_calulator-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       38 2023-05-30 23:41:14.081683 my_ip_calulator-0.4.0/src/app/__init__.py
--rw-r--r--   0        0        0    18576 2023-05-31 19:33:28.690316 my_ip_calulator-0.4.0/src/app/calc.py
--rw-r--r--   0        0        0    10940 2023-05-31 20:18:29.104011 my_ip_calulator-0.4.0/src/app/cmd.py
--rw-r--r--   0        0        0    32522 1970-01-01 00:00:00.000000 my_ip_calulator-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-31 20:27:54.398428 my_ip_calulator-1.0.0/LICENSE
+-rw-r--r--   0        0        0    31699 2023-05-31 20:27:54.399437 my_ip_calulator-1.0.0/README.md
+-rw-r--r--   0        0        0     7769 2023-05-31 20:27:54.411903 my_ip_calulator-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-05-31 20:27:54.412856 my_ip_calulator-1.0.0/src/app/__init__.py
+-rw-r--r--   0        0        0    18576 2023-05-31 20:27:54.413148 my_ip_calulator-1.0.0/src/app/calc.py
+-rw-r--r--   0        0        0    10940 2023-05-31 20:27:54.413555 my_ip_calulator-1.0.0/src/app/cmd.py
+-rw-r--r--   0        0        0    32605 1970-01-01 00:00:00.000000 my_ip_calulator-1.0.0/PKG-INFO
```

### Comparing `my_ip_calulator-0.4.0/LICENSE` & `my_ip_calulator-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `my_ip_calulator-0.4.0/README.md` & `my_ip_calulator-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ## Demo
 [![asciicast](https://asciinema.org/a/585954.svg)](https://asciinema.org/a/585954)
 
 ## Install
 You can use this tool in many ways:
 
 ### Install from Repository
-With this command:
+With this command, you PC will download the app from https://pypi.org/project/my-ip-calulator/0.4.0/:
 ````
 pip install my-ip-calculator
 ````
 
 [![asciicast](https://asciinema.org/a/585935.svg)](https://asciinema.org/a/585935)
 
 ### Run in Container
```

### Comparing `my_ip_calulator-0.4.0/pyproject.toml` & `my_ip_calulator-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "my-ip-calulator"
-version = "0.4.0"
+version = "1.0.0"
 license = "MIT"
 description = "This is an IPv4 and IPv6 calculator. It can validate IP address, convert then and also do net and subnet calculations."
 authors = ["Bruno Botelho <bruno.botelho.br@gmail.com>"]
 maintainers = ["Bruno Botelho <bruno.botelho.br@gmail.com>"]
 readme = "README.md"
 packages = [{include = "app", from = "src"}]
 repository = "https://github.com/brunobotelhobr/My-IP-Calculator"
```

### Comparing `my_ip_calulator-0.4.0/src/app/calc.py` & `my_ip_calulator-1.0.0/src/app/calc.py`

 * *Files identical despite different names*

### Comparing `my_ip_calulator-0.4.0/src/app/cmd.py` & `my_ip_calulator-1.0.0/src/app/cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 cmd = typer.Typer(no_args_is_help=True)
 
 
 @cmd.command()
 def version() -> str:
     """Show version."""
-    app_version: str = "0.1.0"
+    app_version: str = "1.0.0"
     typer.echo(app_version)
     return app_version
 
 
 @cmd.command()
 def val(
     address: Annotated[str, typer.Argument(..., help="IP address, it supports IPv4 and IPv6")],
```

### Comparing `my_ip_calulator-0.4.0/PKG-INFO` & `my_ip_calulator-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-ip-calulator
-Version: 0.4.0
+Version: 1.0.0
 Summary: This is an IPv4 and IPv6 calculator. It can validate IP address, convert then and also do net and subnet calculations.
 Home-page: https://brunobotelhobr.github.io/My-IP-Calculator
 License: MIT
 Keywords: ip,calculator,ipv4,ipv6,net,subnet,cidr,mask,address,convert,validate
 Author: Bruno Botelho
 Author-email: bruno.botelho.br@gmail.com
 Maintainer: Bruno Botelho
@@ -43,15 +43,15 @@
 ## Demo
 [![asciicast](https://asciinema.org/a/585954.svg)](https://asciinema.org/a/585954)
 
 ## Install
 You can use this tool in many ways:
 
 ### Install from Repository
-With this command:
+With this command, you PC will download the app from https://pypi.org/project/my-ip-calulator/0.4.0/:
 ````
 pip install my-ip-calculator
 ````
 
 [![asciicast](https://asciinema.org/a/585935.svg)](https://asciinema.org/a/585935)
 
 ### Run in Container
```

