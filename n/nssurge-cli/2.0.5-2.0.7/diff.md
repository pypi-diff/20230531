# Comparing `tmp/nssurge_cli-2.0.5.tar.gz` & `tmp/nssurge_cli-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge_cli-2.0.5.tar", max compression
+gzip compressed data, was "nssurge_cli-2.0.7.tar", max compression
```

## Comparing `nssurge_cli-2.0.5.tar` & `nssurge_cli-2.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1100 2023-05-05 05:39:14.369260 nssurge_cli-2.0.5/LICENSE
--rw-r--r--   0        0        0        0 2023-05-05 05:39:14.369608 nssurge_cli-2.0.5/README.md
--rw-r--r--   0        0        0      294 2023-05-31 13:38:44.365756 nssurge_cli-2.0.5/nssurge_cli/__init__.py
--rw-r--r--   0        0        0     2681 2023-05-31 13:27:38.132877 nssurge_cli-2.0.5/nssurge_cli/cap_commands.py
--rw-r--r--   0        0        0     1994 2023-05-31 08:11:06.194486 nssurge_cli-2.0.5/nssurge_cli/cli.py
--rw-r--r--   0        0        0     2778 2023-05-31 13:31:26.294601 nssurge_cli-2.0.5/nssurge_cli/config.py
--rw-r--r--   0        0        0     3128 2023-05-31 12:36:19.669380 nssurge_cli-2.0.5/nssurge_cli/devices_commands.py
--rw-r--r--   0        0        0     1582 2023-05-31 13:27:38.129951 nssurge_cli-2.0.5/nssurge_cli/dns_commands.py
--rw-r--r--   0        0        0     1896 2023-05-31 13:27:38.130199 nssurge_cli-2.0.5/nssurge_cli/global_commands.py
--rw-r--r--   0        0        0     4021 2023-05-31 12:36:19.670386 nssurge_cli-2.0.5/nssurge_cli/group_commands.py
--rw-r--r--   0        0        0     4549 2023-05-31 12:36:19.670738 nssurge_cli-2.0.5/nssurge_cli/misc_commands.py
--rw-r--r--   0        0        0     2183 2023-05-31 12:36:18.550232 nssurge_cli-2.0.5/nssurge_cli/modules_commands.py
--rw-r--r--   0        0        0     1590 2023-05-31 13:27:38.130091 nssurge_cli-2.0.5/nssurge_cli/outbound_commands.py
--rw-r--r--   0        0        0     4962 2023-05-31 12:38:43.487013 nssurge_cli-2.0.5/nssurge_cli/policy_commands.py
--rw-r--r--   0        0        0     3110 2023-05-31 12:36:18.550288 nssurge_cli-2.0.5/nssurge_cli/profiles_commands.py
--rw-r--r--   0        0        0     3014 2023-05-31 12:36:19.669296 nssurge_cli-2.0.5/nssurge_cli/requests_commands.py
--rw-r--r--   0        0        0     1315 2023-05-31 12:36:19.730594 nssurge_cli-2.0.5/nssurge_cli/scripting_commands.py
--rw-r--r--   0        0        0     1974 2023-05-31 12:44:05.388263 nssurge_cli-2.0.5/nssurge_cli/test_commands.py
--rw-r--r--   0        0        0      265 2023-05-05 05:39:14.373640 nssurge_cli-2.0.5/nssurge_cli/types.py
--rw-r--r--   0        0        0     1873 2023-05-31 13:33:35.194828 nssurge_cli-2.0.5/nssurge_cli/utils.py
--rw-r--r--   0        0        0     1062 2023-05-31 13:38:44.365032 nssurge_cli-2.0.5/pyproject.toml
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 nssurge_cli-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-05 05:39:14.369260 nssurge_cli-2.0.7/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-05 05:39:14.369608 nssurge_cli-2.0.7/README.md
+-rw-r--r--   0        0        0      294 2023-05-31 14:14:53.685444 nssurge_cli-2.0.7/nssurge_cli/__init__.py
+-rw-r--r--   0        0        0     2693 2023-05-31 14:11:37.772708 nssurge_cli-2.0.7/nssurge_cli/cap_commands.py
+-rw-r--r--   0        0        0     1994 2023-05-31 08:11:06.194486 nssurge_cli-2.0.7/nssurge_cli/cli.py
+-rw-r--r--   0        0        0     2778 2023-05-31 13:31:26.294601 nssurge_cli-2.0.7/nssurge_cli/config.py
+-rw-r--r--   0        0        0     3328 2023-05-31 14:12:52.578041 nssurge_cli-2.0.7/nssurge_cli/devices_commands.py
+-rw-r--r--   0        0        0     1620 2023-05-31 14:12:52.435392 nssurge_cli-2.0.7/nssurge_cli/dns_commands.py
+-rw-r--r--   0        0        0     1900 2023-05-31 14:12:52.124716 nssurge_cli-2.0.7/nssurge_cli/global_commands.py
+-rw-r--r--   0        0        0     4172 2023-05-31 14:12:52.577967 nssurge_cli-2.0.7/nssurge_cli/group_commands.py
+-rw-r--r--   0        0        0     4558 2023-05-31 14:12:52.645195 nssurge_cli-2.0.7/nssurge_cli/misc_commands.py
+-rw-r--r--   0        0        0     2208 2023-05-31 14:12:52.396396 nssurge_cli-2.0.7/nssurge_cli/modules_commands.py
+-rw-r--r--   0        0        0     1596 2023-05-31 14:12:52.557423 nssurge_cli-2.0.7/nssurge_cli/outbound_commands.py
+-rw-r--r--   0        0        0     4966 2023-05-31 14:12:52.504091 nssurge_cli-2.0.7/nssurge_cli/policy_commands.py
+-rw-r--r--   0        0        0     3166 2023-05-31 14:12:52.462754 nssurge_cli-2.0.7/nssurge_cli/profiles_commands.py
+-rw-r--r--   0        0        0     3064 2023-05-31 14:12:52.647586 nssurge_cli-2.0.7/nssurge_cli/requests_commands.py
+-rw-r--r--   0        0        0     1338 2023-05-31 14:12:52.145411 nssurge_cli-2.0.7/nssurge_cli/scripting_commands.py
+-rw-r--r--   0        0        0     1978 2023-05-31 14:12:51.865239 nssurge_cli-2.0.7/nssurge_cli/test_commands.py
+-rw-r--r--   0        0        0      265 2023-05-05 05:39:14.373640 nssurge_cli-2.0.7/nssurge_cli/types.py
+-rw-r--r--   0        0        0     1877 2023-05-31 14:12:51.902751 nssurge_cli-2.0.7/nssurge_cli/utils.py
+-rw-r--r--   0        0        0     1087 2023-05-31 14:14:53.684489 nssurge_cli-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 nssurge_cli-2.0.7/PKG-INFO
```

### Comparing `nssurge_cli-2.0.5/LICENSE` & `nssurge_cli-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.5/nssurge_cli/cap_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/cap_commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 from nssurge_cli.config import get_config
-from nssurge_cli.types import (OnOffToggleEnum)
-from nssurge_cli.utils import (bool2color, get_cap_state, s2b)
+from nssurge_cli.types import OnOffToggleEnum
+from nssurge_cli.utils import bool2color, get_cap_state, s2b
+
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import Capability
 import typer
 import asyncio
 
 
 app = typer.Typer(name='cap')
 
+
 async def get_set_cap(
     capability: Capability, on_off: OnOffToggleEnum = typer.Argument(None)
 ) -> bool | tuple[bool, bool]:
     """
     Get or set a capability
     """
     async with SurgeAPIClient(*get_config()) as client:
@@ -28,15 +30,18 @@
                 return state_orig
         state_new = await get_cap_state(client, capability)
         return state_orig, state_new
 
 
 # @app.command("cap")
 @app.callback(invoke_without_command=True)
-def cap(capability: Capability = typer.Argument(None), on_off: OnOffToggleEnum = typer.Argument(None)):
+def cap(
+    capability: Capability = typer.Argument(None),
+    on_off: OnOffToggleEnum = typer.Argument(None),
+):
     """
     Get or set a capability.
     """
     if capability is None:
         caps()
         return
     states = asyncio.run(get_set_cap(capability, on_off))
@@ -72,8 +77,7 @@
 def caps():
     """get all caps"""
     states = asyncio.run(get_caps())
     for capability, state in states.items():
         length = 16
         state_colored = typer.style(f"{state}", fg=bool2color(state))
         typer.secho(f"{capability:>{length}}: {state_colored}")
-
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/cli.py` & `nssurge_cli-2.0.7/nssurge_cli/cli.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.5/nssurge_cli/config.py` & `nssurge_cli-2.0.7/nssurge_cli/config.py`

 * *Files identical despite different names*

### Comparing `nssurge_cli-2.0.5/nssurge_cli/devices_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/devices_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,44 +3,51 @@
 from nssurge_cli.config import get_config
 from nssurge_cli.types import ChangeDeviceEnum
 from nssurge_cli.utils import (
     typer_output_dict,
 )
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import (
     ChangeDeviceRequest,
 )
 import typer
 import asyncio
 
 app = typer.Typer(name="devices")
 
 
 async def get_devices():
     async with SurgeAPIClient(*get_config()) as client:
         devices_resp = await client.get_devices()
         return await devices_resp.json()
 
+
 def complete_devices(incomplete: str):
     """
     Complete device names.
     """
     incomplete = incomplete.lower()
-    devices_dict = asyncio.run(get_devices()) # type: ignore
+    devices_dict = asyncio.run(get_devices())  # type: ignore
     devices: list[dict] = devices_dict['devices']
     for device in devices:
-        info = ' | '.join(map(lambda x: str(device.get(x)), ['name', 'displayIPAddress', 'totalBytes']))
-        id: str = device.get('identifier') # type: ignore
+        info = ' | '.join(
+            map(
+                lambda x: str(device.get(x)), ['name', 'displayIPAddress', 'totalBytes']
+            )
+        )
+        id: str = device.get('identifier')  # type: ignore
         if incomplete in id or incomplete in info.lower():
             yield id, info
 
+
 @app.callback(invoke_without_command=True)
-def devices(ctx: typer.Context,
+def devices(
+    ctx: typer.Context,
     output_json: bool = typer.Option(False, "--json", "-j"),
     pretty_print: bool = typer.Option(False, "--pretty", "-p"),
     rich_print: bool = typer.Option(False, "--rich", "-r"),
 ):
     """Manage devices"""
     if ctx.invoked_subcommand is not None:
         return
@@ -51,35 +58,54 @@
 async def get_device_icon(icon_id):
     async with SurgeAPIClient(*get_config()) as client:
         icon_resp = await client.get_device_icon(icon_id)
         return await icon_resp.json()
 
 
 @app.command("icon")
-def icon(icon_id, output_json: bool = typer.Option(False, "--json", "-j"), pretty_print: bool = typer.Option(False, "--pretty", "-p"), rich_print: bool = typer.Option(False, "--rich", "-r")):
+def icon(
+    icon_id,
+    output_json: bool = typer.Option(False, "--json", "-j"),
+    pretty_print: bool = typer.Option(False, "--pretty", "-p"),
+    rich_print: bool = typer.Option(False, "--rich", "-r"),
+):
     icon_resp = asyncio.run(get_device_icon(icon_id))
     typer_output_dict(icon_resp, output_json, pretty_print, rich_print)
-    typer.secho('Warning: the Surge API used is broken on Surge for mac 4.5.0', dim=True, err=True)
+    typer.secho(
+        'Warning: the Surge API used is broken on Surge for mac 4.5.0',
+        dim=True,
+        err=True,
+    )
 
 
 async def change_device(req: ChangeDeviceRequest):
     async with SurgeAPIClient(*get_config()) as client:
         resp = await client.change_device(req)
         return await resp.json()
 
+
 @app.command('set')
-def set_device_command(physical_address: str = typer.Argument(..., autocompletion=complete_devices), field: ChangeDeviceEnum = typer.Argument(...), value: str = typer.Argument(...)):
+def set_device_command(
+    physical_address: str = typer.Argument(..., autocompletion=complete_devices),
+    field: ChangeDeviceEnum = typer.Argument(...),
+    value: str = typer.Argument(...),
+):
     req = ChangeDeviceRequest(
         physicalAddress=physical_address,
     )
     # setattr(req, field.value, value)
     req[field.value] = value
     resp_dict = asyncio.run(change_device(req))
     # typer_output_dict(resp_dict)
     if not resp_dict:
         # success
-        typer.secho(f'Successfully set {field.value} to {value} for {physical_address}', fg=typer.colors.GREEN)
+        typer.secho(
+            f'Successfully set {field.value} to {value} for {physical_address}',
+            fg=typer.colors.GREEN,
+        )
     else:
         # failure
-        typer.secho(f'Failed to set {field.value} to {value} for {physical_address}', fg=typer.colors.RED)
+        typer.secho(
+            f'Failed to set {field.value} to {value} for {physical_address}',
+            fg=typer.colors.RED,
+        )
         typer.secho(f'Error: {resp_dict["error"]}', fg=typer.colors.RED)
-
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/dns_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/dns_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from nssurge_cli.config import get_config
 from nssurge_cli.utils import (
     typer_output_dict,
 )
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 import typer
 import asyncio
 
 app = typer.Typer(name="dns")
 
 
 async def flush_dns():
@@ -28,25 +28,34 @@
 async def get_dns():
     async with SurgeAPIClient(*get_config()) as client:
         dns = await client.get_dns()
         return await dns.json()
 
 
 @app.callback(invoke_without_command=True)
-def get_dns_command(ctx: typer.Context, output_json: bool = typer.Option(False, "--json", "-j"), pretty_print: bool = typer.Option(False, "--pretty", "-p"), rich_print: bool = typer.Option(False, "--rich", "-r")):
+def get_dns_command(
+    ctx: typer.Context,
+    output_json: bool = typer.Option(False, "--json", "-j"),
+    pretty_print: bool = typer.Option(False, "--pretty", "-p"),
+    rich_print: bool = typer.Option(False, "--rich", "-r"),
+):
     """Manage DNS"""
     if ctx.invoked_subcommand is not None:
         return
     dns = asyncio.run(get_dns())
     typer_output_dict(dns, output_json, pretty_print, rich_print)
 
 
 async def test_dns():
     async with SurgeAPIClient(*get_config()) as client:
         resp = await client.test_dns()
         return await resp.json()
 
 
 @app.command("test")
-def test_dns_command(output_json: bool = typer.Option(False, "--json", "-j"), pretty_print: bool = typer.Option(False, "--pretty", "-p"), rich_print: bool = typer.Option(False, "--rich", "-r")):
+def test_dns_command(
+    output_json: bool = typer.Option(False, "--json", "-j"),
+    pretty_print: bool = typer.Option(False, "--pretty", "-p"),
+    rich_print: bool = typer.Option(False, "--rich", "-r"),
+):
     dns = asyncio.run(test_dns())
     typer_output_dict(dns, output_json, pretty_print, rich_print)
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/global_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/global_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 from nssurge_cli.config import get_config
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import Policy
 import typer
 import asyncio
 from typing import Optional
 from typing_extensions import Annotated
 
 from nssurge_cli.policy_commands import complete_policy_and_proxy
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/group_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/group_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 #!/usr/bin/env python3
 from nssurge_cli.config import get_config
 from nssurge_cli.utils import (
     typer_output_dict,
 )
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import (
     Policy,
     PolicyGroup,
 )
 import typer
 import asyncio
-from nssurge_cli.policy_commands import complete_policy, complete_policy_for_policy_group
+from nssurge_cli.policy_commands import (
+    complete_policy,
+    complete_policy_for_policy_group,
+)
 
 app = typer.Typer(name="group")
 
 
 async def get_policy_group(policy_group: PolicyGroup = typer.Argument(None)) -> dict:
     """
     Get all policy groups, or a specific one.
     """
     async with SurgeAPIClient(*get_config()) as client:
         try:
             return await (await client.get_policy_group(policy_group)).json()
         except Exception as e:
             typer.secho(f"Error: {e}", err=True)
-            typer.secho('Using proxy as an arg causes Surge for Mac to crash as of version 4.5.0', err=True, fg='red')
+            typer.secho(
+                'Using proxy as an arg causes Surge for Mac to crash as of version 4.5.0',
+                err=True,
+                fg='red',
+            )
             return {}
 
 
 # @app.command('group')
 # @app.callback(invoke_without_command=True)
 @app.command('policy')
-def policy_group(# ctx: typer.Context,
-    policy_group: PolicyGroup = typer.Argument(..., help="Policy group name", autocompletion=complete_policy),
+def policy_group(  # ctx: typer.Context,
+    policy_group: PolicyGroup = typer.Argument(
+        ..., help="Policy group name", autocompletion=complete_policy
+    ),
     # output_json: bool = typer.Option(False, "--json", "-j"),
     # pretty_print: bool = typer.Option(False, "--pretty", "-p"),
     # rich_print: bool = typer.Option(False, "--rich", "-r"),
 ):
     """
     Get all policy groups, or a specific one.
     """
@@ -79,15 +88,22 @@
     Select a policy group.
     """
     async with SurgeAPIClient(*get_config()) as client:
         return await client.set_policy_group(policy_group, policy)
 
 
 @app.command("select")
-def select_group_command(policy: PolicyGroup = typer.Argument(..., help='Policy group name', autocompletion=complete_policy), policy_selected: Policy = typer.Argument(..., help='Policy name', autocompletion=complete_policy_for_policy_group)):
+def select_group_command(
+    policy: PolicyGroup = typer.Argument(
+        ..., help='Policy group name', autocompletion=complete_policy
+    ),
+    policy_selected: Policy = typer.Argument(
+        ..., help='Policy name', autocompletion=complete_policy_for_policy_group
+    ),
+):
     """
     Select a policy group.
     """
     asyncio.run(select_group(policy, policy_selected))
 
 
 async def test_policy_group(policy_group: PolicyGroup) -> dict:
@@ -97,21 +113,24 @@
     async with SurgeAPIClient(*get_config()) as client:
         resp = await client.test_policy_group(policy_group)
         return await resp.json()
 
 
 @app.command("test")
 def test_policy_group_command(
-    policy_group: PolicyGroup = typer.Argument(..., help="Policy group name", autocompletion=complete_policy),
+    policy_group: PolicyGroup = typer.Argument(
+        ..., help="Policy group name", autocompletion=complete_policy
+    ),
     output_json: bool = typer.Option(False, "--json", "-j"),
     pretty_print: bool = typer.Option(False, "--pretty", "-p"),
     rich_print: bool = typer.Option(False, "--rich", "-r"),
 ):
     """
     Test a policy group.
     """
     test_dict = asyncio.run(test_policy_group(policy_group))
     typer_output_dict(test_dict, output_json, pretty_print, rich_print)
 
+
 @app.callback()
 def group_command_callback():
-    """For policy groups"""
+    """For policy groups"""
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/misc_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/misc_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #!/usr/bin/env python3
 
 from nssurge_cli.config import get_config
 from nssurge_cli.utils import typer_output_dict
+
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import LogLevel
 import typer
 import asyncio
+
 # from nssurge_cli.cli import app
 
+
 async def stop_engine():
     """
     Stop the engine and quit the app
     """
     async with SurgeAPIClient(*get_config()) as client:
         stop_resp = await client.stop_engine()
         stop_dict: dict = await stop_resp.json()
@@ -122,21 +125,23 @@
         log_level_dict: dict = await log_level_resp.json()
         # if 'error' in log_level_dict:
         # if not log_level_dict:
         # 	typer.secho(f'Failed to set log level: {log_level_dict["error"]}', fg=typer.colors.RED)
         # 	raise typer.Exit(1)
         return log_level_dict
 
+
 # doesn't seem to work
 # def complete_loglevel(incomplete: str):
 #     """
 #     Complete log level
 #     """
 #     return [level.value for level in LogLevel if incomplete.lower() in level.value]
 
+
 # @app.command("loglevel")
 def set_log_level_command(log_level: LogLevel = typer.Argument(..., help="Log level")):
     """
     Set log level
     """
     log_level_dict = asyncio.run(set_log_level(log_level))
     typer_output_dict(log_level_dict)
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/modules_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/modules_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 #!/usr/bin/env python3
 
 from nssurge_cli.cap_commands import s2b
 from nssurge_cli.config import get_config
 from nssurge_cli.types import OnOffToggleEnum
-from nssurge_cli.utils import (
-    typer_output_dict,
-    s2b
-)
+from nssurge_cli.utils import typer_output_dict, s2b
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
-from nssurge_api.types import (
-    SetModuleStateRequest,
-    Module
-)
+from nssurge_api.api import SurgeAPIClient
+from nssurge_api.types import SetModuleStateRequest, Module
 import typer
 import asyncio
 
 app = typer.Typer(name="modules")
 
 
 async def get_modules():
     async with SurgeAPIClient(*get_config()) as client:
         modules = await client.get_modules()
         return await modules.json()
 
+
 def complete_module(incomplete: str):
     incomplete = incomplete.lower()
     modules = asyncio.run(get_modules())
     modules_available: list[str] = modules['available']
     modules_enabled: list[str] = modules['enabled']
     for module in modules_available:
         if incomplete in module:
             if module in modules_enabled:
                 yield module, 'enabled'
             else:
                 yield module, 'disabled'
 
 
 @app.callback(invoke_without_command=True)
-def get_modules_command(ctx: typer.Context, output_json: bool = typer.Option(False, "--json", '-j'), pretty_print: bool = typer.Option(False, "--pretty", "-p"), rich_print: bool = typer.Option(False, "--rich", "-r")):
+def get_modules_command(
+    ctx: typer.Context,
+    output_json: bool = typer.Option(False, "--json", '-j'),
+    pretty_print: bool = typer.Option(False, "--pretty", "-p"),
+    rich_print: bool = typer.Option(False, "--rich", "-r"),
+):
     """Manage modules"""
     if ctx.invoked_subcommand is not None:
         return
     modules = asyncio.run(get_modules())
     typer_output_dict(modules, output_json, pretty_print, rich_print)
 
 
 async def set_modules(config: SetModuleStateRequest):
     async with SurgeAPIClient(*get_config()) as client:
         resp = await client.set_modules(config)
         return await resp.json()
 
+
 @app.command('set')
-def set_modules_command(module: Module = typer.Argument(..., help="Module to set", autocompletion=complete_module), state: OnOffToggleEnum = typer.Argument(..., help="State to set")):
+def set_modules_command(
+    module: Module = typer.Argument(
+        ..., help="Module to set", autocompletion=complete_module
+    ),
+    state: OnOffToggleEnum = typer.Argument(..., help="State to set"),
+):
     """Set module state"""
     config: SetModuleStateRequest = {module: s2b(state)}
     set_dict = asyncio.run(set_modules(config))
     if 'error' not in set_dict:
         typer.secho(f"Set module {module} to {state}", fg='green')
     else:
         typer.secho(f"Error: {set_dict['error']}", fg='red')
-
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/outbound_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/outbound_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python3
 from nssurge_cli.config import get_config
+
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import OutboundMode
 import typer
 import asyncio
 
 app = typer.Typer(name="outbound")
 
+
 async def get_set_outbound(
     outbound_mode: OutboundMode = typer.Argument(None),
 ) -> OutboundMode:
     """
     Get or set the outbound mode.
     """
     async with SurgeAPIClient(*get_config()) as client:
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/policy_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/policy_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import typer
 import asyncio
 from typing import Optional
 import typer
 from typing_extensions import Annotated
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import Policy, Policies, Proxies, PolicyGroups
 
 app = typer.Typer(name="policy")
 
 
 @cache
 async def get_policy(
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/profiles_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/profiles_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Iterable
 from nssurge_cli.config import get_config
 from nssurge_cli.utils import (
     typer_output_dict,
 )
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import (
     Profile,
 )
 import typer
 import asyncio
 
 app = typer.Typer(name="profiles")
@@ -20,15 +20,21 @@
 async def get_active_profile(mask_password: bool = True) -> dict:
     async with SurgeAPIClient(*get_config()) as client:
         profile = await client.get_active_profile(mask_password)
         return await profile.json()
 
 
 @app.callback(invoke_without_command=True)
-def active_profile(ctx: typer.Context, mask_password: bool = True, output_json: bool = typer.Option(False, "--json", '-j'), pretty_print: bool = typer.Option(False, "--pretty", "-p"), rich_print: bool = typer.Option(False, "--rich", "-r")):
+def active_profile(
+    ctx: typer.Context,
+    mask_password: bool = True,
+    output_json: bool = typer.Option(False, "--json", '-j'),
+    pretty_print: bool = typer.Option(False, "--pretty", "-p"),
+    rich_print: bool = typer.Option(False, "--rich", "-r"),
+):
     """Get active profile"""
     if ctx.invoked_subcommand is not None:
         return
     profile = asyncio.run(get_active_profile(mask_password))
     typer_output_dict(profile, output_json, pretty_print, rich_print)
 
 
@@ -53,40 +59,46 @@
 
 
 async def list_profiles():
     async with SurgeAPIClient(*get_config()) as client:
         profiles = await client.get_profiles()
         return await profiles.json()
 
+
 def complete_profiles(incomplete: str) -> Iterable[Profile]:
     profiles_dict = asyncio.run(list_profiles())
     profiles: list[Profile] = profiles_dict['profiles']
     # for profile in profiles:
     #     if incomplete.lower() in profile.lower():
     #         yield profile
     return [profile for profile in profiles if incomplete.lower() in profile.lower()]
 
-    
 
 @app.command("list")
-def list_profiles_command(output_json: bool = typer.Option(False, "--json", '-j'), pretty_print: bool = typer.Option(False, "--pretty", "-p"), rich_print: bool = typer.Option(False, "--rich", "-r")):
+def list_profiles_command(
+    output_json: bool = typer.Option(False, "--json", '-j'),
+    pretty_print: bool = typer.Option(False, "--pretty", "-p"),
+    rich_print: bool = typer.Option(False, "--rich", "-r"),
+):
     profiles = asyncio.run(list_profiles())
     typer_output_dict(profiles, output_json, pretty_print, rich_print)
 
 
 async def validate_profile(profile_name: Profile):
     async with SurgeAPIClient(*get_config()) as client:
         resp = await client.validate_profile(profile_name)
         return await resp.json()
 
 
 @app.command("validate")
-def validate_profile_command(profile_name: Profile = typer.Argument(..., help="Profile name", autocompletion=complete_profiles)):
+def validate_profile_command(
+    profile_name: Profile = typer.Argument(
+        ..., help="Profile name", autocompletion=complete_profiles
+    )
+):
     profile = asyncio.run(validate_profile(profile_name))
     if profile['error'] is None:
         typer.secho(f"Profile {profile_name} is valid", fg='green')
     else:
         typer.secho(f"Profile {profile_name} is invalid", fg='red')
         typer.secho(profile['error'], fg='red')
     # typer_output_dict(profile)
-
-
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/requests_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/requests_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 from typing import Iterable
 from nssurge_cli.config import get_config
 from nssurge_cli.utils import typer_output_dict
+
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import RequestsType
 import typer
 import asyncio
 
 app = typer.Typer(name="requests")
 
+
 async def get_requests(requests_type: RequestsType = RequestsType.recent):
     """
     Get requests
     """
     async with SurgeAPIClient(*get_config()) as client:
         req_resp = await client.get_requests(requests_type)
         req_dict: dict = await req_resp.json()
         # if 'error' in req_dict:
         # 	typer.secho(f'Failed to get requests: {req_dict["error"]}', fg=typer.colors.RED)
         # 	raise typer.Exit(1)
         return req_dict
 
+
 def complete_requests_id(incomplete: str) -> Iterable[tuple[str, str]]:
     """
     Complete requests ids.
     """
     incomplete = incomplete.lower()
-    req_dict: dict = asyncio.run(get_requests(requests_type=RequestsType.active)) # type: ignore
+    req_dict: dict = asyncio.run(get_requests(requests_type=RequestsType.active))  # type: ignore
     reqs: list[dict] = req_dict["requests"]
     for req in reqs:
         info = Path(req['processPath']).name
         info += ' | '
-        info += ' | '.join(map(lambda x: req.get(x, ''), ['status', 'policyName', 'rule', 'URL']))
+        info += ' | '.join(
+            map(lambda x: req.get(x, ''), ['status', 'policyName', 'rule', 'URL'])
+        )
         if incomplete in str(req['id']) or incomplete in info.lower():
             yield (str(req['id']), info)
-    
+
 
 # @app.command("requests")
 @app.callback(invoke_without_command=True)
-def requests(ctx: typer.Context,
+def requests(
+    ctx: typer.Context,
     requests_type: RequestsType = typer.Option(RequestsType.recent, '--type', '-t'),
     output_json: bool = typer.Option(False, "--json", "-j"),
     pretty_print: bool = typer.Option(False, "--pretty", "-p"),
     rich_print: bool = typer.Option(False, "--rich", "-r"),
 ):
     """
     Get requests
@@ -67,21 +73,24 @@
         # if not kill_dict:
         # 	typer.secho(f'Failed to kill requests: {kill_dict["error"]}', fg=typer.colors.RED)
         # 	raise typer.Exit(1)
         return kill_dict
 
 
 @app.command("kill")
-def kill_request_command(request_id: int = typer.Argument(..., help="Request ID", autocompletion=complete_requests_id)):
+def kill_request_command(
+    request_id: int = typer.Argument(
+        ..., help="Request ID", autocompletion=complete_requests_id
+    )
+):
     """
     Kill requests
     """
     kill_dict = asyncio.run(kill_request(request_id))
     error = kill_dict.get('error', None)
     if error is None:
         # success
         typer.secho(f'Successfully killed request {request_id}', fg=typer.colors.GREEN)
     else:
         # failed
         typer.secho(f'Failed to kill request {request_id}', fg=typer.colors.RED)
         typer.secho(f'Error: {error}', fg=typer.colors.RED)
-
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/scripting_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/scripting_commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from nssurge_cli.config import get_config
 from nssurge_cli.utils import (
     typer_output_dict,
 )
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import (
     EvalScriptMockRequest,
 )
 import typer
 import asyncio
 
 app = typer.Typer(name="script")
@@ -19,15 +19,20 @@
 async def get_scripts():
     async with SurgeAPIClient(*get_config()) as client:
         scripting_resp = await client.get_scripts()
         return await scripting_resp.json()
 
 
 @app.callback(invoke_without_command=True)
-def scripts(ctx: typer.Context, output_json: bool = typer.Option(False, "--json", '-j'), pretty_print: bool = typer.Option(False, "--pretty", "-p"), rich_print: bool = typer.Option(False, "--rich", "-r")):
+def scripts(
+    ctx: typer.Context,
+    output_json: bool = typer.Option(False, "--json", '-j'),
+    pretty_print: bool = typer.Option(False, "--pretty", "-p"),
+    rich_print: bool = typer.Option(False, "--rich", "-r"),
+):
     """Get all scripts"""
     if ctx.invoked_subcommand is not None:
         return
     scripts_resp = asyncio.run(get_scripts())
     typer_output_dict(scripts_resp, output_json, pretty_print, rich_print)
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/test_commands.py` & `nssurge_cli-2.0.7/nssurge_cli/test_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from nssurge_cli.config import get_config
 from nssurge_cli.utils import typer_output_dict
 
 from typing import Optional
 from typing_extensions import Annotated
 
 # use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import Proxy
 import typer
 import asyncio
 from nssurge_cli.policy_commands import complete_proxies
 
 app = typer.Typer(name="test")
```

### Comparing `nssurge_cli-2.0.5/nssurge_cli/utils.py` & `nssurge_cli-2.0.7/nssurge_cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 import typer
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from aiohttp import ClientResponse
-from nssurge_api import SurgeAPIClient
+from nssurge_api.api import SurgeAPIClient
 from nssurge_api.types import (
     Capability,
 )
 
 from utils_tddschn.utils import strtobool
```

### Comparing `nssurge_cli-2.0.5/pyproject.toml` & `nssurge_cli-2.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nssurge-cli"
-version = "2.0.5"
+version = "2.0.7"
 description = "NSSurge CLI"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/nssurge-cli"
 repository = "https://github.com/tddschn/nssurge-cli"
 classifiers = ["Topic :: Utilities"]
@@ -15,15 +15,15 @@
 nssurge-cli = "nssurge_cli:cli.app"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/nssurge-cli/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.11, <4.0"
-nssurge-api = "0.2.10"
+nssurge-api = "^0.2.14"
 utils-tddschn = "^0.1.5"
 rich = { version = "^12.4.1", extras = ["format"] }
 
 [tool.poetry.dev-dependencies]
 toml = "^0.10.2"
 yapf = "^0.32.0"
 better-exceptions = "^0.3.3"
@@ -31,11 +31,12 @@
 logging-utils-tddschn = "^0.1.8"
 
 [tool.poetry.group.dev.dependencies]
 typer = "^0.9.0"
 pytest = "^7.3.1"
 black = "^23.3.0"
 pyinstrument = "^4.4.0"
+nssurge-api = "^0.2.13"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nssurge_cli-2.0.5/PKG-INFO` & `nssurge_cli-2.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: nssurge-cli
-Version: 2.0.5
+Version: 2.0.7
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
-Requires-Dist: nssurge-api (==0.2.10)
+Requires-Dist: nssurge-api (>=0.2.14,<0.3.0)
 Requires-Dist: rich[format] (>=12.4.1,<13.0.0)
 Requires-Dist: utils-tddschn (>=0.1.5,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/nssurge-cli/issues
 Project-URL: Repository, https://github.com/tddschn/nssurge-cli
 Description-Content-Type: text/markdown
```

