# Comparing `tmp/my_ip_calulator-0.1.0.tar.gz` & `tmp/my_ip_calulator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_ip_calulator-0.1.0.tar", max compression
+gzip compressed data, was "my_ip_calulator-0.4.0.tar", max compression
```

## Comparing `my_ip_calulator-0.1.0.tar` & `my_ip_calulator-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       72 2023-05-19 20:33:56.000000 my_ip_calulator-0.1.0/LICENSE.md
--rw-r--r--   0        0        0    31615 2023-05-19 20:40:02.338894 my_ip_calulator-0.1.0/README.md
--rw-r--r--   0        0        0     7763 2023-05-19 20:43:23.451739 my_ip_calulator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       38 2023-05-19 20:33:56.000000 my_ip_calulator-0.1.0/src/app/__init__.py
--rw-r--r--   0        0        0    18576 2023-05-19 20:36:52.004295 my_ip_calulator-0.1.0/src/app/calc.py
--rw-r--r--   0        0        0    11103 2023-05-19 20:43:38.870454 my_ip_calulator-0.1.0/src/app/cmd.py
--rw-r--r--   0        0        0    32521 1970-01-01 00:00:00.000000 my_ip_calulator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 23:41:14.070516 my_ip_calulator-0.4.0/LICENSE
+-rw-r--r--   0        0        0    31616 2023-05-31 00:34:10.649805 my_ip_calulator-0.4.0/README.md
+-rw-r--r--   0        0        0     7769 2023-05-31 20:22:51.763688 my_ip_calulator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-05-30 23:41:14.081683 my_ip_calulator-0.4.0/src/app/__init__.py
+-rw-r--r--   0        0        0    18576 2023-05-31 19:33:28.690316 my_ip_calulator-0.4.0/src/app/calc.py
+-rw-r--r--   0        0        0    10940 2023-05-31 20:18:29.104011 my_ip_calulator-0.4.0/src/app/cmd.py
+-rw-r--r--   0        0        0    32522 1970-01-01 00:00:00.000000 my_ip_calulator-0.4.0/PKG-INFO
```

### Comparing `my_ip_calulator-0.1.0/README.md` & `my_ip_calulator-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 ┏━━━━━━━━━┳━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━┓
 ┃ Item    ┃ Value ┃ Message         ┃ Status     ┃
 ┡━━━━━━━━━╇━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━┩
 │ address │ A     │ Invalid address │ ⛔ Invalid │
 └─────────┴───────┴─────────────────┴────────────┘
 `````
 
-### Netork (Net)
+### Network (Net)
 Usage: `my-ip-calculator net [OPTIONS] ADDRESS [MASK]`
 Calculate the network address from an IP address and a subnet mask, output the address in the desired format.
 if a mask isn't provided:
 
 - For IPv4 it will provide a mask based on the adress class: A, B,C,D and E
 - For IPv6 a standart /64 will be provided.
```

### Comparing `my_ip_calulator-0.1.0/pyproject.toml` & `my_ip_calulator-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "my-ip-calulator"
-version = "0.1.0"
+version = "0.4.0"
 license = "MIT"
 description = "This is an IPv4 and IPv6 calculator. It can validate IP address, convert then and also do net and subnet calculations."
 authors = ["Bruno Botelho <bruno.botelho.br@gmail.com>"]
 maintainers = ["Bruno Botelho <bruno.botelho.br@gmail.com>"]
 readme = "README.md"
 packages = [{include = "app", from = "src"}]
 repository = "https://github.com/brunobotelhobr/My-IP-Calculator"
@@ -38,15 +38,15 @@
 taskipy = "^1.10.4"
 ipython = "^8.13.2"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.6"
 mkdocs = "^1.4.2"
 mkdocs-material-extensions = "^1.1.1"
-pymdown-extensions = "^9.11"
+pymdown-extensions = ">=9.11,<11.0"
 mkdocstrings = {version = "^0.21.2", extras = ["python"]}
 mike = "^1.1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -112,15 +112,15 @@
 docs_branch = "documentation"
 package_dir = { var = "src/app", recursive = true }
 package_name = "my-ip-calulator"
 package_version = "0.0.1"
 docker_context = "brunobotelhobr"
 
 [tool.taskipy.tasks]
-pre-commit = { cmd = "task format && task lint && task tests", help = "Run all pre-commit tasks" }
+pre-commit = { cmd = "task format && task lint && task test", help = "Run all pre-commit tasks" }
 pre-release = { cmd = "task pre-commit && task bom && task req &&  task sec", help = "Run all pre-release tasks" }
 ----------- = "----------------------------------------"
 info = { cmd = "poetry env info && poetry check && poetry show", help = "Show project info" }
 meta = { cmd = "python scripts/update-project-properties.py", help = "Update project properties" }
 upgrade = { cmd = "poetry self update && poetry update && task bom && task req", help = "Upgrade all dependencies" }
 sec = { cmd = "trivy fs --exit-code 1 --scanners vuln,config,secret . && bandit -c pyproject.toml -r src && horusec start -D -p ./src", help = "Run all security checks" }
 format = { cmd = "echo 'Running IsSort' && isort --settings-path pyproject.toml src && isort --settings-path pyproject.toml tests && echo 'Running Black' && black --config ./pyproject.toml src && black --config ./pyproject.toml tests  && echo 'Running Autoflake' && autoflake --recursive src && autoflake --recursive tests", help = "Run all formaters" }
```

### Comparing `my_ip_calulator-0.1.0/src/app/calc.py` & `my_ip_calulator-0.4.0/src/app/calc.py`

 * *Files identical despite different names*

### Comparing `my_ip_calulator-0.1.0/src/app/cmd.py` & `my_ip_calulator-0.4.0/src/app/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,28 +73,28 @@
     ).convert()
     # Print the address
     Printer().address(address=address, version=address_version)
     return True
 
 
 @cmd.command()
-def net(  # type: ignore
+def net(
     address: Annotated[str, typer.Argument(..., help="IP address, it supports IPv4 and IPv6.")],
     output: Annotated[
         Optional[OutputOptions],
         typer.Option(
             "-o",
             "--output",
             help="Output format for the network address details of an IP address, it supports bin, hex, dec.",
             case_sensitive=False,
             show_choices=True,
         ),
     ] = None,
     mask: Annotated[
-        str | None, typer.Argument(help="IP address mask, if not provided an auto generated one will be assigned.")
+        Optional[str], typer.Argument(help="IP address mask, if not provided an auto generated one will be assigned.")
     ] = None,
 ) -> bool:
     """Calculate the network address from an IP address and a subnet mask, output the address in the desired format."""
     # Identify the address type
     address_version: int = discover_version(address=address)
     # Return False if the address is invalid
     if address_version not in [4, 6]:
@@ -167,15 +167,15 @@
 
 @cmd.command()
 def subnet(  # type: ignore
     address: Annotated[str, typer.Argument(..., help="IP address, it supports IPv4 and IPv6.")],
     mask: Annotated[str, typer.Argument(help="IP address mask.")],
     parts: Annotated[int, typer.Argument(help="Split the netork into this parts.")],
     output: Annotated[
-        str | None,
+        Optional[str],
         typer.Option(
             "-o",
             "--output",
             help="Output format for the network address details of an IP address, it supports bin, hex, dec.",
             case_sensitive=False,
             show_choices=True,
         ),
@@ -215,32 +215,26 @@
     if address_version == 6:
         try:
             mask = Validator(address=mask, version=address_version).expand_v6()
         except ValueError:
             Printer().error(name="mask", value=mask, message="Invalid mask")
             return False
     # Validate the mask
-    try:
-        Validator(address=mask, version=address_version).validate()
-    except ValueError:
+    if Validator(address=mask, version=address_version).validate() is False:
         Printer().error(name="mask", value=mask, message="Invalid mask")
         return False
     # Validate the split
     # Validate if the parts are base 2
     if parts < 0:
         Printer().error(name="parts", value=str(parts), message="The parts must be greater than 1")
         return False
     if not log2(parts).is_integer():
         Printer().error(name="parts", value=str(parts), message="The parts must be base 2")
         return False
-    try:
-        mask = str(MaskCompress(mask=mask, version=address_version).compress())
-    except ValueError:
-        Printer().error(name="mask", value=mask, message="Invalid mask")
-        return False
+    mask = str(MaskCompress(mask=mask, version=address_version).compress())
     if address_version == 4:
         if int(mask) + parts > 32:
             Printer().error(name="parts", value=str(parts), message="The parts are too big for the mask")
             return False
     if address_version == 6:
         if int(mask) + parts > 128:
             Printer().error(name="parts", value=str(parts), message="The parts are too big for the mask")
```

### Comparing `my_ip_calulator-0.1.0/PKG-INFO` & `my_ip_calulator-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-ip-calulator
-Version: 0.1.0
+Version: 0.4.0
 Summary: This is an IPv4 and IPv6 calculator. It can validate IP address, convert then and also do net and subnet calculations.
 Home-page: https://brunobotelhobr.github.io/My-IP-Calculator
 License: MIT
 Keywords: ip,calculator,ipv4,ipv6,net,subnet,cidr,mask,address,convert,validate
 Author: Bruno Botelho
 Author-email: bruno.botelho.br@gmail.com
 Maintainer: Bruno Botelho
@@ -174,15 +174,15 @@
 ┏━━━━━━━━━┳━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━┓
 ┃ Item    ┃ Value ┃ Message         ┃ Status     ┃
 ┡━━━━━━━━━╇━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━┩
 │ address │ A     │ Invalid address │ ⛔ Invalid │
 └─────────┴───────┴─────────────────┴────────────┘
 `````
 
-### Netork (Net)
+### Network (Net)
 Usage: `my-ip-calculator net [OPTIONS] ADDRESS [MASK]`
 Calculate the network address from an IP address and a subnet mask, output the address in the desired format.
 if a mask isn't provided:
 
 - For IPv4 it will provide a mask based on the adress class: A, B,C,D and E
 - For IPv6 a standart /64 will be provided.
```

