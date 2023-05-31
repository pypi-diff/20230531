# Comparing `tmp/nssurge_cli-2.0.4.tar.gz` & `tmp/nssurge_cli-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge_cli-2.0.4.tar", max compression
+gzip compressed data, was "nssurge_cli-2.0.5.tar", max compression
```

## Comparing `nssurge_cli-2.0.4.tar` & `nssurge_cli-2.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1100 2023-05-05 05:39:14.369260 nssurge_cli-2.0.4/LICENSE
--rw-r--r--   0        0        0        0 2023-05-05 05:39:14.369608 nssurge_cli-2.0.4/README.md
--rw-r--r--   0        0        0      294 2023-05-31 13:28:12.670573 nssurge_cli-2.0.4/nssurge_cli/__init__.py
--rw-r--r--   0        0        0     2681 2023-05-31 13:27:38.132877 nssurge_cli-2.0.4/nssurge_cli/cap_commands.py
--rw-r--r--   0        0        0     1994 2023-05-31 08:11:06.194486 nssurge_cli-2.0.4/nssurge_cli/cli.py
--rw-r--r--   0        0        0     2692 2023-05-05 05:39:14.370556 nssurge_cli-2.0.4/nssurge_cli/config.py
--rw-r--r--   0        0        0     3128 2023-05-31 12:36:19.669380 nssurge_cli-2.0.4/nssurge_cli/devices_commands.py
--rw-r--r--   0        0        0     1582 2023-05-31 13:27:38.129951 nssurge_cli-2.0.4/nssurge_cli/dns_commands.py
--rw-r--r--   0        0        0     1896 2023-05-31 13:27:38.130199 nssurge_cli-2.0.4/nssurge_cli/global_commands.py
--rw-r--r--   0        0        0     4021 2023-05-31 12:36:19.670386 nssurge_cli-2.0.4/nssurge_cli/group_commands.py
--rw-r--r--   0        0        0     4549 2023-05-31 12:36:19.670738 nssurge_cli-2.0.4/nssurge_cli/misc_commands.py
--rw-r--r--   0        0        0     2183 2023-05-31 12:36:18.550232 nssurge_cli-2.0.4/nssurge_cli/modules_commands.py
--rw-r--r--   0        0        0     1590 2023-05-31 13:27:38.130091 nssurge_cli-2.0.4/nssurge_cli/outbound_commands.py
--rw-r--r--   0        0        0     4962 2023-05-31 12:38:43.487013 nssurge_cli-2.0.4/nssurge_cli/policy_commands.py
--rw-r--r--   0        0        0     3110 2023-05-31 12:36:18.550288 nssurge_cli-2.0.4/nssurge_cli/profiles_commands.py
--rw-r--r--   0        0        0     3014 2023-05-31 12:36:19.669296 nssurge_cli-2.0.4/nssurge_cli/requests_commands.py
--rw-r--r--   0        0        0     1315 2023-05-31 12:36:19.730594 nssurge_cli-2.0.4/nssurge_cli/scripting_commands.py
--rw-r--r--   0        0        0     1974 2023-05-31 12:44:05.388263 nssurge_cli-2.0.4/nssurge_cli/test_commands.py
--rw-r--r--   0        0        0      265 2023-05-05 05:39:14.373640 nssurge_cli-2.0.4/nssurge_cli/types.py
--rw-r--r--   0        0        0     1797 2023-05-05 05:39:14.373808 nssurge_cli-2.0.4/nssurge_cli/utils.py
--rw-r--r--   0        0        0     1038 2023-05-31 13:28:12.665760 nssurge_cli-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 nssurge_cli-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-05 05:39:14.369260 nssurge_cli-2.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-05 05:39:14.369608 nssurge_cli-2.0.5/README.md
+-rw-r--r--   0        0        0      294 2023-05-31 13:38:44.365756 nssurge_cli-2.0.5/nssurge_cli/__init__.py
+-rw-r--r--   0        0        0     2681 2023-05-31 13:27:38.132877 nssurge_cli-2.0.5/nssurge_cli/cap_commands.py
+-rw-r--r--   0        0        0     1994 2023-05-31 08:11:06.194486 nssurge_cli-2.0.5/nssurge_cli/cli.py
+-rw-r--r--   0        0        0     2778 2023-05-31 13:31:26.294601 nssurge_cli-2.0.5/nssurge_cli/config.py
+-rw-r--r--   0        0        0     3128 2023-05-31 12:36:19.669380 nssurge_cli-2.0.5/nssurge_cli/devices_commands.py
+-rw-r--r--   0        0        0     1582 2023-05-31 13:27:38.129951 nssurge_cli-2.0.5/nssurge_cli/dns_commands.py
+-rw-r--r--   0        0        0     1896 2023-05-31 13:27:38.130199 nssurge_cli-2.0.5/nssurge_cli/global_commands.py
+-rw-r--r--   0        0        0     4021 2023-05-31 12:36:19.670386 nssurge_cli-2.0.5/nssurge_cli/group_commands.py
+-rw-r--r--   0        0        0     4549 2023-05-31 12:36:19.670738 nssurge_cli-2.0.5/nssurge_cli/misc_commands.py
+-rw-r--r--   0        0        0     2183 2023-05-31 12:36:18.550232 nssurge_cli-2.0.5/nssurge_cli/modules_commands.py
+-rw-r--r--   0        0        0     1590 2023-05-31 13:27:38.130091 nssurge_cli-2.0.5/nssurge_cli/outbound_commands.py
+-rw-r--r--   0        0        0     4962 2023-05-31 12:38:43.487013 nssurge_cli-2.0.5/nssurge_cli/policy_commands.py
+-rw-r--r--   0        0        0     3110 2023-05-31 12:36:18.550288 nssurge_cli-2.0.5/nssurge_cli/profiles_commands.py
+-rw-r--r--   0        0        0     3014 2023-05-31 12:36:19.669296 nssurge_cli-2.0.5/nssurge_cli/requests_commands.py
+-rw-r--r--   0        0        0     1315 2023-05-31 12:36:19.730594 nssurge_cli-2.0.5/nssurge_cli/scripting_commands.py
+-rw-r--r--   0        0        0     1974 2023-05-31 12:44:05.388263 nssurge_cli-2.0.5/nssurge_cli/test_commands.py
+-rw-r--r--   0        0        0      265 2023-05-05 05:39:14.373640 nssurge_cli-2.0.5/nssurge_cli/types.py
+-rw-r--r--   0        0        0     1873 2023-05-31 13:33:35.194828 nssurge_cli-2.0.5/nssurge_cli/utils.py
+-rw-r--r--   0        0        0     1062 2023-05-31 13:38:44.365032 nssurge_cli-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 nssurge_cli-2.0.5/PKG-INFO
```

### Comparing `nssurge_cli-2.0.4/LICENSE` & `nssurge_cli-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/cap_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/cap_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/cli.py` & `nssurge_cli-2.0.5/nssurge_cli/cli.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/config.py` & `nssurge_cli-2.0.5/nssurge_cli/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,34 @@
 
 @app.callback()
 def config_callback():
     """
     Manage configuration
     """
 
+
 @cache
 def read_config(config_path: Path = DEFAULT_CONFIG_PATH) -> dict:
     """
     Read the config file and return a dictionary of the contents.
     """
     import configparser
 
     config = configparser.ConfigParser()
     config.read(config_path)
     return {
-        "SURGE_HTTP_API_ENDPOINT": config.get("DEFAULT", "SURGE_HTTP_API_ENDPOINT", fallback=DEFAULT_SURGE_HTTP_API_ENDPOINT),
+        "SURGE_HTTP_API_ENDPOINT": config.get(
+            "DEFAULT",
+            "SURGE_HTTP_API_ENDPOINT",
+            fallback=DEFAULT_SURGE_HTTP_API_ENDPOINT,
+        ),
         "SURGE_HTTP_API_KEY": config["DEFAULT"]["SURGE_HTTP_API_KEY"],
-        "TRUST_ENV": config.getboolean("DEFAULT", "TRUST_ENV", fallback=DEFAULT_TRUST_ENV),
+        "TRUST_ENV": config.getboolean(
+            "DEFAULT", "TRUST_ENV", fallback=DEFAULT_TRUST_ENV
+        ),
     }
 
 
 @app.command("example")
 def write_example_config(
     write_config: bool = typer.Option(
         False,
@@ -47,15 +54,15 @@
 ):
     """
     Show example config.
     """
     import configparser
 
     config = configparser.ConfigParser()
-    config["DEFAULT"] = {
+    config["DEFAULT"] = {  # type: ignore
         "SURGE_HTTP_API_ENDPOINT": DEFAULT_SURGE_HTTP_API_ENDPOINT,
         "SURGE_HTTP_API_KEY": "",
         "TRUST_ENV": DEFAULT_TRUST_ENV,
     }
     if write_config:
         DEFAULT_CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
         DEFAULT_CONFIG_PATH.touch()
```

### Comparing `nssurge_cli-2.0.4/nssurge_cli/devices_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/devices_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/dns_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/dns_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/global_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/global_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/group_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/group_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/misc_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/misc_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/modules_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/modules_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/outbound_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/outbound_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/policy_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/policy_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/profiles_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/profiles_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/requests_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/requests_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/scripting_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/scripting_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/test_commands.py` & `nssurge_cli-2.0.5/nssurge_cli/test_commands.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.4/nssurge_cli/utils.py` & `nssurge_cli-2.0.5/nssurge_cli/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 import typer
-from aiohttp import ClientResponse
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from aiohttp import ClientResponse
 from nssurge_api import SurgeAPIClient
 from nssurge_api.types import (
     Capability,
 )
 
 from utils_tddschn.utils import strtobool
+
+
 def s2b(s: str) -> bool:
     return bool(strtobool(s))
 
 
-async def parse_cap_get(resp: ClientResponse) -> bool:
+async def parse_cap_get(resp: 'ClientResponse') -> bool:
     if not resp.status == 200:
         raise ValueError(f"Unexpected status code: {resp.status}")
     return (await resp.json())["enabled"]
 
 
 async def get_cap_state(client: SurgeAPIClient, capability: Capability) -> bool:
     get_resp = await client.get_cap(capability)
@@ -64,8 +69,8 @@
             typer.secho("rich module not installed")
     else:
         typer.secho(d)
 
 
 # typer_output_dict_typer_options = (    output_json: bool = typer.Option(False, "--json", "-j"),
 #     pretty_print: bool = typer.Option(False, "--pretty", "-p"),)
-rich_print: bool = (typer.Option(False, "--rich", "-r"),)
+rich_print: bool = (typer.Option(False, "--rich", "-r"),)  # type: ignore
```

### Comparing `nssurge_cli-2.0.4/pyproject.toml` & `nssurge_cli-2.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nssurge-cli"
-version = "2.0.4"
+version = "2.0.5"
 description = "NSSurge CLI"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/nssurge-cli"
 repository = "https://github.com/tddschn/nssurge-cli"
 classifiers = ["Topic :: Utilities"]
@@ -30,11 +30,12 @@
 bump2version = "^1.0.1"
 logging-utils-tddschn = "^0.1.8"
 
 [tool.poetry.group.dev.dependencies]
 typer = "^0.9.0"
 pytest = "^7.3.1"
 black = "^23.3.0"
+pyinstrument = "^4.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nssurge_cli-2.0.4/PKG-INFO` & `nssurge_cli-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nssurge-cli
-Version: 2.0.4
+Version: 2.0.5
 Summary: NSSurge CLI
 Home-page: https://github.com/tddschn/nssurge-cli
 License: MIT
 Keywords: nssurge,cli,surge,typer
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

