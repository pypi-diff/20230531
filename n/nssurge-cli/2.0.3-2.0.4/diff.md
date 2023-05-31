# Comparing `tmp/nssurge-cli-2.0.3.tar.gz` & `tmp/nssurge_cli-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge-cli-2.0.3.tar", max compression
+gzip compressed data, was "nssurge_cli-2.0.4.tar", max compression
```

## Comparing `nssurge-cli-2.0.3.tar` & `nssurge_cli-2.0.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1100 2022-05-13 02:00:20.455699 nssurge-cli-2.0.3/LICENSE
--rw-r--r--   0        0        0        0 2022-05-13 01:59:48.629060 nssurge-cli-2.0.3/README.md
--rw-r--r--   0        0        0      294 2022-05-16 01:26:50.311615 nssurge-cli-2.0.3/nssurge_cli/__init__.py
--rw-r--r--   0        0        0     3098 2022-05-16 01:06:05.704090 nssurge-cli-2.0.3/nssurge_cli/cap_commands.py
--rw-r--r--   0        0        0     1889 2022-05-15 05:34:13.699981 nssurge-cli-2.0.3/nssurge_cli/cli.py
--rw-r--r--   0        0        0     2692 2022-05-15 06:00:59.508086 nssurge-cli-2.0.3/nssurge_cli/config.py
--rw-r--r--   0        0        0     3639 2022-05-15 16:20:56.856639 nssurge-cli-2.0.3/nssurge_cli/devices_commands.py
--rw-r--r--   0        0        0     2161 2022-05-15 16:21:21.132188 nssurge-cli-2.0.3/nssurge_cli/dns_commands.py
--rw-r--r--   0        0        0     2269 2022-05-15 11:02:46.234915 nssurge-cli-2.0.3/nssurge_cli/global_commands.py
--rw-r--r--   0        0        0     4561 2022-05-15 10:51:58.212631 nssurge-cli-2.0.3/nssurge_cli/group_commands.py
--rw-r--r--   0        0        0     5035 2022-05-15 16:02:27.241825 nssurge-cli-2.0.3/nssurge_cli/misc_commands.py
--rw-r--r--   0        0        0     2625 2022-05-16 01:17:43.618415 nssurge-cli-2.0.3/nssurge_cli/modules_commands.py
--rw-r--r--   0        0        0     2142 2022-05-15 05:34:13.699818 nssurge-cli-2.0.3/nssurge_cli/outbound_commands.py
--rw-r--r--   0        0        0     5273 2022-05-15 16:21:40.671335 nssurge-cli-2.0.3/nssurge_cli/policy_commands.py
--rw-r--r--   0        0        0     3634 2022-05-15 09:40:28.069576 nssurge-cli-2.0.3/nssurge_cli/profiles_commands.py
--rw-r--r--   0        0        0     3507 2022-05-15 10:00:37.036764 nssurge-cli-2.0.3/nssurge_cli/requests_commands.py
--rw-r--r--   0        0        0     1825 2022-05-15 05:34:13.699763 nssurge-cli-2.0.3/nssurge_cli/scripting_commands.py
--rw-r--r--   0        0        0     2314 2022-05-15 16:19:01.013138 nssurge-cli-2.0.3/nssurge_cli/test_commands.py
--rw-r--r--   0        0        0      265 2022-05-15 03:26:43.089095 nssurge-cli-2.0.3/nssurge_cli/types.py
--rw-r--r--   0        0        0     2035 2022-05-16 01:05:57.586068 nssurge-cli-2.0.3/nssurge_cli/utils.py
--rw-r--r--   0        0        0      974 2022-05-16 01:26:50.311140 nssurge-cli-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      908 2022-05-16 01:26:54.996702 nssurge-cli-2.0.3/setup.py
--rw-r--r--   0        0        0      807 2022-05-16 01:26:54.997028 nssurge-cli-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-05 05:39:14.369260 nssurge_cli-2.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-05 05:39:14.369608 nssurge_cli-2.0.4/README.md
+-rw-r--r--   0        0        0      294 2023-05-31 13:28:12.670573 nssurge_cli-2.0.4/nssurge_cli/__init__.py
+-rw-r--r--   0        0        0     2681 2023-05-31 13:27:38.132877 nssurge_cli-2.0.4/nssurge_cli/cap_commands.py
+-rw-r--r--   0        0        0     1994 2023-05-31 08:11:06.194486 nssurge_cli-2.0.4/nssurge_cli/cli.py
+-rw-r--r--   0        0        0     2692 2023-05-05 05:39:14.370556 nssurge_cli-2.0.4/nssurge_cli/config.py
+-rw-r--r--   0        0        0     3128 2023-05-31 12:36:19.669380 nssurge_cli-2.0.4/nssurge_cli/devices_commands.py
+-rw-r--r--   0        0        0     1582 2023-05-31 13:27:38.129951 nssurge_cli-2.0.4/nssurge_cli/dns_commands.py
+-rw-r--r--   0        0        0     1896 2023-05-31 13:27:38.130199 nssurge_cli-2.0.4/nssurge_cli/global_commands.py
+-rw-r--r--   0        0        0     4021 2023-05-31 12:36:19.670386 nssurge_cli-2.0.4/nssurge_cli/group_commands.py
+-rw-r--r--   0        0        0     4549 2023-05-31 12:36:19.670738 nssurge_cli-2.0.4/nssurge_cli/misc_commands.py
+-rw-r--r--   0        0        0     2183 2023-05-31 12:36:18.550232 nssurge_cli-2.0.4/nssurge_cli/modules_commands.py
+-rw-r--r--   0        0        0     1590 2023-05-31 13:27:38.130091 nssurge_cli-2.0.4/nssurge_cli/outbound_commands.py
+-rw-r--r--   0        0        0     4962 2023-05-31 12:38:43.487013 nssurge_cli-2.0.4/nssurge_cli/policy_commands.py
+-rw-r--r--   0        0        0     3110 2023-05-31 12:36:18.550288 nssurge_cli-2.0.4/nssurge_cli/profiles_commands.py
+-rw-r--r--   0        0        0     3014 2023-05-31 12:36:19.669296 nssurge_cli-2.0.4/nssurge_cli/requests_commands.py
+-rw-r--r--   0        0        0     1315 2023-05-31 12:36:19.730594 nssurge_cli-2.0.4/nssurge_cli/scripting_commands.py
+-rw-r--r--   0        0        0     1974 2023-05-31 12:44:05.388263 nssurge_cli-2.0.4/nssurge_cli/test_commands.py
+-rw-r--r--   0        0        0      265 2023-05-05 05:39:14.373640 nssurge_cli-2.0.4/nssurge_cli/types.py
+-rw-r--r--   0        0        0     1797 2023-05-05 05:39:14.373808 nssurge_cli-2.0.4/nssurge_cli/utils.py
+-rw-r--r--   0        0        0     1038 2023-05-31 13:28:12.665760 nssurge_cli-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 nssurge_cli-2.0.4/PKG-INFO
```

### Comparing `nssurge-cli-2.0.3/LICENSE` & `nssurge_cli-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nssurge-cli-2.0.3/nssurge_cli/config.py` & `nssurge_cli-2.0.4/nssurge_cli/config.py`

 * *Files identical despite different names*

### Comparing `nssurge-cli-2.0.3/nssurge_cli/devices_commands.py` & `nssurge_cli-2.0.4/nssurge_cli/devices_commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,22 @@
 #!/usr/bin/env python3
 
-from typing import Iterable
-from . import __version__, __app_name__, logger
-from .config import read_config, app as config_app, get_config
-from .types import OnOffToggleEnum, ChangeDeviceEnum
-from .utils import (
-    bool2color,
-    parse_cap_get,
-    get_cap_state,
+from nssurge_cli.config import get_config
+from nssurge_cli.types import ChangeDeviceEnum
+from nssurge_cli.utils import (
     typer_output_dict,
-    use_local_nssurge_api_module,
 )
-from utils_tddschn.utils import strtobool
 
 # use_local_nssurge_api_module()
 from nssurge_api import SurgeAPIClient
 from nssurge_api.types import (
-    Capability,
-    LogLevel,
-    OutboundMode,
-    Policy,
-    PolicyGroup,
-    RequestsType,
-    Profile,
-    Enabled,
-    SetModuleStateRequest,
-    EvalScriptMockRequest,
-    EvalCronScriptRequest,
-    Script,
     ChangeDeviceRequest,
-    Policies,
-    Proxy,
 )
 import typer
 import asyncio
-from aiohttp import ClientSession, ClientResponse
 
 app = typer.Typer(name="devices")
 
 
 async def get_devices():
     async with SurgeAPIClient(*get_config()) as client:
         devices_resp = await client.get_devices()
```

### Comparing `nssurge-cli-2.0.3/nssurge_cli/global_commands.py` & `nssurge_cli-2.0.4/nssurge_cli/global_commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #!/usr/bin/env python3
 
-from . import __version__, __app_name__, logger
-from .config import read_config, app as config_app, get_config
-from .types import (OnOffToggleEnum)
-from .utils import (bool2color, parse_cap_get, get_cap_state, typer_output_dict, use_local_nssurge_api_module)
-from utils_tddschn.utils import strtobool
+from nssurge_cli.config import get_config
+
 # use_local_nssurge_api_module()
 from nssurge_api import SurgeAPIClient
-from nssurge_api.types import (Capability, LogLevel, OutboundMode, Policy,
-							   PolicyGroup, RequestsType, Profile, Enabled,
-							   SetModuleStateRequest, EvalScriptMockRequest,
-							   EvalCronScriptRequest, Script,
-							   ChangeDeviceRequest, Policies, Proxy)
+from nssurge_api.types import Policy
 import typer
 import asyncio
-from aiohttp import ClientSession, ClientResponse
-from .policy_commands import complete_policy_and_proxy
+from typing import Optional
+from typing_extensions import Annotated
+
+from nssurge_cli.policy_commands import complete_policy_and_proxy
 
 app = typer.Typer(name="global")
 
-async def get_set_global_policy(policy: Policy | None = None) -> Policy:
+
+async def get_set_global_policy(
+    policy: Annotated[Optional[Policy], typer.Argument()] = None
+) -> Policy:
     """
     Get or set the global policy.
     """
     async with SurgeAPIClient(*get_config()) as client:
         if policy is not None:
             set_resp = await client.set_global_policy(policy)
             set_dict: dict = await set_resp.json()
@@ -39,18 +37,26 @@
         else:
             typer.secho(f"Current global policy: {current_policy}")
         return current_policy
 
 
 # @app.command("global")
 @app.callback(invoke_without_command=True)
-def global_command(ctx: typer.Context, policy: Policy = typer.Argument(None, help="Policy name", autocompletion=complete_policy_and_proxy)):
+def global_command(
+    ctx: typer.Context,
+    policy: Policy = typer.Argument(
+        None, help="Policy name", autocompletion=complete_policy_and_proxy
+    ),
+):
     """
     Get or set the global policy.
     """
     if ctx.invoked_subcommand is not None:
         return
     asyncio.run(get_set_global_policy(policy))
     # typer.secho(f"Warning: the get API is broken on the Surge side")
     # dimmed style
-    typer.secho(f"Warning: the get API is broken on the Surge side, tested on Surge for Mac 4.5.0", dim=True, err=True)
-
+    typer.secho(
+        "Warning: the get API is broken on the Surge side, tested on Surge for Mac 4.5.0",
+        dim=True,
+        err=True,
+    )
```

### Comparing `nssurge-cli-2.0.3/nssurge_cli/group_commands.py` & `nssurge_cli-2.0.4/nssurge_cli/group_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,22 @@
 #!/usr/bin/env python3
-from . import __version__, __app_name__, logger
-from .config import read_config, app as config_app, get_config
-from .types import OnOffToggleEnum
-from .utils import (
-    bool2color,
-    parse_cap_get,
-    get_cap_state,
+from nssurge_cli.config import get_config
+from nssurge_cli.utils import (
     typer_output_dict,
-    use_local_nssurge_api_module,
 )
-from utils_tddschn.utils import strtobool
 
 # use_local_nssurge_api_module()
 from nssurge_api import SurgeAPIClient
 from nssurge_api.types import (
-    Capability,
-    LogLevel,
-    OutboundMode,
     Policy,
     PolicyGroup,
-    RequestsType,
-    Profile,
-    Enabled,
-    SetModuleStateRequest,
-    EvalScriptMockRequest,
-    EvalCronScriptRequest,
-    Script,
-    ChangeDeviceRequest,
-    Policies,
-    Proxy,
 )
 import typer
 import asyncio
-from aiohttp import ClientSession, ClientResponse
-from .policy_commands import complete_policy, complete_proxy, complete_policy_and_proxy, complete_policy_for_policy_group
+from nssurge_cli.policy_commands import complete_policy, complete_policy_for_policy_group
 
 app = typer.Typer(name="group")
 
 
 async def get_policy_group(policy_group: PolicyGroup = typer.Argument(None)) -> dict:
     """
     Get all policy groups, or a specific one.
```

### Comparing `nssurge-cli-2.0.3/nssurge_cli/misc_commands.py` & `nssurge_cli-2.0.4/nssurge_cli/misc_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 #!/usr/bin/env python3
 
-from . import __version__, __app_name__, logger
-from .config import read_config, app as config_app, get_config
-from .types import (OnOffToggleEnum)
-from .utils import (bool2color, parse_cap_get, get_cap_state, typer_output_dict, use_local_nssurge_api_module)
-from utils_tddschn.utils import strtobool
+from nssurge_cli.config import get_config
+from nssurge_cli.utils import typer_output_dict
 # use_local_nssurge_api_module()
 from nssurge_api import SurgeAPIClient
-from nssurge_api.types import (Capability, LogLevel, OutboundMode, Policy,
-							   PolicyGroup, RequestsType, Profile, Enabled,
-							   SetModuleStateRequest, EvalScriptMockRequest,
-							   EvalCronScriptRequest, Script,
-							   ChangeDeviceRequest, Policies, Proxy)
+from nssurge_api.types import LogLevel
 import typer
 import asyncio
-from aiohttp import ClientSession, ClientResponse
-# from .cli import app
+# from nssurge_cli.cli import app
 
 async def stop_engine():
     """
     Stop the engine and quit the app
     """
     async with SurgeAPIClient(*get_config()) as client:
         stop_resp = await client.stop_engine()
```

### Comparing `nssurge-cli-2.0.3/nssurge_cli/modules_commands.py` & `nssurge_cli-2.0.4/nssurge_cli/modules_commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,25 @@
 #!/usr/bin/env python3
 
-from typing import Iterable
 from nssurge_cli.cap_commands import s2b
-from . import __version__, __app_name__, logger
-from .config import read_config, app as config_app, get_config
-from .types import OnOffToggleEnum
-from .utils import (
-    bool2color,
-    parse_cap_get,
-    get_cap_state,
+from nssurge_cli.config import get_config
+from nssurge_cli.types import OnOffToggleEnum
+from nssurge_cli.utils import (
     typer_output_dict,
-    use_local_nssurge_api_module, s2b
+    s2b
 )
 
 # use_local_nssurge_api_module()
 from nssurge_api import SurgeAPIClient
 from nssurge_api.types import (
-    Capability,
-    LogLevel,
-    OutboundMode,
-    Policy,
-    PolicyGroup,
-    RequestsType,
-    Profile,
-    Enabled,
     SetModuleStateRequest,
-    EvalScriptMockRequest,
-    EvalCronScriptRequest,
-    Script,
-    ChangeDeviceRequest,
-    Policies,
-    Proxy, Module
+    Module
 )
 import typer
 import asyncio
-from aiohttp import ClientSession, ClientResponse
 
 app = typer.Typer(name="modules")
 
 
 async def get_modules():
     async with SurgeAPIClient(*get_config()) as client:
         modules = await client.get_modules()
```

### Comparing `nssurge-cli-2.0.3/nssurge_cli/policy_commands.py` & `nssurge_cli-2.0.4/nssurge_cli/policy_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,119 +1,141 @@
 #!/usr/bin/env python3
 
 from functools import cache
 from typing import Iterable
-from . import __version__, __app_name__, logger
-from .config import read_config, app as config_app, get_config
-from .types import (OnOffToggleEnum)
-from .utils import (bool2color, parse_cap_get, get_cap_state, typer_output_dict, use_local_nssurge_api_module)
-from utils_tddschn.utils import strtobool
-# use_local_nssurge_api_module()
-from nssurge_api import SurgeAPIClient
-from nssurge_api.types import (Capability, LogLevel, OutboundMode, Policy,
-							   PolicyGroup, RequestsType, Profile, Enabled,
-							   SetModuleStateRequest, EvalScriptMockRequest,
-							   EvalCronScriptRequest, Script,
-							   ChangeDeviceRequest, Policies, Proxy, Proxies, PolicyGroups)
+from nssurge_cli.config import get_config
+from nssurge_cli.utils import typer_output_dict
+
 import typer
 import asyncio
-from aiohttp import ClientSession, ClientResponse
-# from .completions import complete_policy
+from typing import Optional
+import typer
+from typing_extensions import Annotated
+
+# use_local_nssurge_api_module()
+from nssurge_api import SurgeAPIClient
+from nssurge_api.types import Policy, Policies, Proxies, PolicyGroups
 
 app = typer.Typer(name="policy")
 
+
 @cache
-async def get_policy(policy: Policy | None = None) -> dict:
+async def get_policy(
+    policy: Annotated[Optional[Policy], typer.Argument()] = None
+) -> dict:
     """
     Get all policies.
     """
     async with SurgeAPIClient(*get_config()) as client:
         policy_dict = await (await client.get_policy(policy)).json()
         return policy_dict
 
+
 def complete_policy(incomplete: str) -> Iterable[tuple[str, str]]:
     """
     Complete policy names.
     """
     incomplete = incomplete.lower()
-    policy_dict: Policies = asyncio.run(get_policy()) # type: ignore
+    policy_dict: Policies = asyncio.run(get_policy())  # type: ignore
     # proxies: Proxies = policy_dict["proxies"]
     policy_groups: PolicyGroups = policy_dict["policy-groups"]
-    p2type_mapping = {p: 'policy group' for p in policy_groups if incomplete in p.lower()}
+    p2type_mapping = {
+        p: 'policy group' for p in policy_groups if incomplete in p.lower()
+    }
     # p2type_mapping = {p: 'proxy' for p in proxies if incomplete in p.lower()}
-    
+
     return p2type_mapping.items()
 
+
 def complete_policies(ctx: typer.Context, incomplete: str) -> Iterable[str]:
     """
     Complete policy names.
     """
     incomplete = incomplete.lower()
-    policy_dict: Policies = asyncio.run(get_policy()) # type: ignore
+    policy_dict: Policies = asyncio.run(get_policy())  # type: ignore
     policies_already_supplied = ctx.params.get("policies") or []
     policy_groups: PolicyGroups = policy_dict["policy-groups"]
-    return [p for p in policy_groups if incomplete in p.lower() and p not in policies_already_supplied]
+    return [
+        p
+        for p in policy_groups
+        if incomplete in p.lower() and p not in policies_already_supplied
+    ]
+
 
 def complete_proxies(ctx: typer.Context, incomplete: str) -> Iterable[str]:
     """
     Complete policy names.
     """
     incomplete = incomplete.lower()
-    policy_dict: Policies = asyncio.run(get_policy()) # type: ignore
+    policy_dict: Policies = asyncio.run(get_policy())  # type: ignore
     policies_already_supplied = ctx.params.get("policies") or []
     policy_groups: PolicyGroups = policy_dict["proxies"]
-    return [p for p in policy_groups if incomplete in p.lower() and p not in policies_already_supplied]
+    return [
+        p
+        for p in policy_groups
+        if incomplete in p.lower() and p not in policies_already_supplied
+    ]
+
 
 def complete_proxy(incomplete: str) -> Iterable[tuple[str, str]]:
     """
     Complete policy names.
     """
     incomplete = incomplete.lower()
-    policy_dict: Policies = asyncio.run(get_policy()) # type: ignore
+    policy_dict: Policies = asyncio.run(get_policy())  # type: ignore
     proxies: Proxies = policy_dict["proxies"]
     # policy_groups: PolicyGroups = policy_dict["policy-groups"]
     # p2type_mapping = {p: 'policy group' for p in policy_groups if incomplete in p.lower()}
     p2type_mapping = {p: 'proxy' for p in proxies if incomplete in p.lower()}
-    
+
     return p2type_mapping.items()
 
+
 def complete_policy_and_proxy(incomplete: str) -> Iterable[tuple[str, str]]:
     """
     Complete policy names.
     """
     incomplete = incomplete.lower()
-    policy_dict: Policies = asyncio.run(get_policy()) # type: ignore
+    policy_dict: Policies = asyncio.run(get_policy())  # type: ignore
     proxies: Proxies = policy_dict["proxies"]
     policy_groups: PolicyGroups = policy_dict["policy-groups"]
-    p2type_mapping = {p: 'policy group' for p in policy_groups if incomplete in p.lower()}
+    p2type_mapping = {
+        p: 'policy group' for p in policy_groups if incomplete in p.lower()
+    }
     p2type_mapping.update({p: 'proxy' for p in proxies if incomplete in p.lower()})
-    
+
     return p2type_mapping.items()
 
-def complete_policy_for_policy_group(ctx: typer.Context, incomplete: str) -> Iterable[str]:
+
+def complete_policy_for_policy_group(
+    ctx: typer.Context, incomplete: str
+) -> Iterable[str]:
     """
     Complete policy names.
     """
     policy = ctx.params.get('policy')
 
     # like 'Netflix = select, Proxy, Direct'
     try:
         policy_rule_for_group: str = asyncio.run(get_policy(policy=policy))[policy]
     except:
         typer.secho(f'No policy found for policy group {policy}', fg='red', err=True)
         return []
     policies_str = policy_rule_for_group.split('=')[1].strip()
     import re
+
     policies: list[str] = re.split(r'\s*,\s*', policies_str)
 
     return [p for p in policies if incomplete.lower() in p.lower()]
 
+
 # @app.command("policy")
 @app.callback(invoke_without_command=True)
-def policy(ctx: typer.Context,
+def policy(
+    ctx: typer.Context,
     policy: Policy = typer.Argument(None, autocompletion=complete_policy),
     output_json: bool = typer.Option(False, "--json", "-j"),
     pretty_print: bool = typer.Option(False, "--pretty", "-p"),
     rich_print: bool = typer.Option(False, "--rich", "-r"),
 ):
     """
     Get all policies, or a specific policy
@@ -129,8 +151,7 @@
             typer.secho(
                 f'Failed to get policy {policy}: {policy_dict["error"]}',
                 fg=typer.colors.RED,
             )
             raise typer.Exit(1)
         # return policy_dict
     typer_output_dict(policy_dict, output_json, pretty_print, rich_print)  # type: ignore
-
```

### Comparing `nssurge-cli-2.0.3/nssurge_cli/test_commands.py` & `nssurge_cli-2.0.4/nssurge_cli/test_commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python3
 
-from . import __version__, __app_name__, logger
-from .config import read_config, app as config_app, get_config
-from .types import (OnOffToggleEnum)
-from .utils import (bool2color, parse_cap_get, get_cap_state, typer_output_dict, use_local_nssurge_api_module)
-from utils_tddschn.utils import strtobool
+from nssurge_cli.config import get_config
+from nssurge_cli.utils import typer_output_dict
+
+from typing import Optional
+from typing_extensions import Annotated
+
 # use_local_nssurge_api_module()
 from nssurge_api import SurgeAPIClient
-from nssurge_api.types import (Capability, LogLevel, OutboundMode, Policy,
-							   PolicyGroup, RequestsType, Profile, Enabled,
-							   SetModuleStateRequest, EvalScriptMockRequest,
-							   EvalCronScriptRequest, Script,
-							   ChangeDeviceRequest, Policies, Proxy)
+from nssurge_api.types import Proxy
 import typer
 import asyncio
-from aiohttp import ClientSession, ClientResponse
-from .policy_commands import complete_policies, complete_proxies
+from nssurge_cli.policy_commands import complete_proxies
 
 app = typer.Typer(name="test")
 
-async def test_proxies(policies: list[Proxy], url: str | None = None) -> dict:
+
+async def test_proxies(
+    policies: list[Proxy], url: Annotated[Optional[str], typer.Argument()] = None
+) -> dict:
     """
     Test proxies
     """
     async with SurgeAPIClient(*get_config()) as client:
         test_resp = await client.test_policies(policies, url)
         test_dict: dict = await test_resp.json()
         # if 'error' in test_dict:
@@ -34,15 +33,22 @@
             typer.secho("Please specify at least 1 valid proxy to test")
             raise typer.Exit(1)
         return test_dict
 
 
 # @app.command("test")
 @app.callback(invoke_without_command=True)
-def test_proxies_command(ctx: typer.Context, policies: list[Proxy] = typer.Argument(..., autocompletion=complete_proxies), url: str | None = None, output_json: bool = typer.Option(False, "--json", "-j"), pretty_print: bool = typer.Option(False, "--pretty", "-p"), rich_print: bool = typer.Option(False, "--rich", "-r")):
+def test_proxies_command(
+    ctx: typer.Context,
+    policies: list[Proxy] = typer.Argument(..., autocompletion=complete_proxies),
+    url: Annotated[Optional[str], typer.Argument()] = None,
+    output_json: bool = typer.Option(False, "--json", "-j"),
+    pretty_print: bool = typer.Option(False, "--pretty", "-p"),
+    rich_print: bool = typer.Option(False, "--rich", "-r"),
+):
     """
     Test proxies
     """
     #! bug:
     # options after list of arguments interpreted as argument
     # https://github.com/tiangolo/typer/search?q=options%20after%20list%20of%20arguments%20interpreted%20as%20argument
     # changing the arg to option doesn't help either
```

### Comparing `nssurge-cli-2.0.3/nssurge_cli/utils.py` & `nssurge_cli-2.0.4/nssurge_cli/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,15 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 import typer
-from aiohttp import ClientSession, ClientResponse
+from aiohttp import ClientResponse
 from nssurge_api import SurgeAPIClient
 from nssurge_api.types import (
     Capability,
-    LogLevel,
-    OutboundMode,
-    Policy,
-    PolicyGroup,
-    RequestsType,
-    Profile,
-    Enabled,
-    SetModuleStateRequest,
-    EvalScriptMockRequest,
-    EvalCronScriptRequest,
-    Script,
-    ChangeDeviceRequest,
 )
 
 from utils_tddschn.utils import strtobool
 def s2b(s: str) -> bool:
     return bool(strtobool(s))
```

### Comparing `nssurge-cli-2.0.3/pyproject.toml` & `nssurge_cli-2.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 [tool.poetry]
 name = "nssurge-cli"
-version = "2.0.3"
+version = "2.0.4"
 description = "NSSurge CLI"
 authors = ["Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tddschn/nssurge-cli"
 repository = "https://github.com/tddschn/nssurge-cli"
-classifiers = [
-	"Topic :: Utilities"
-]
+classifiers = ["Topic :: Utilities"]
 keywords = ["nssurge", "cli", "surge", "typer"]
 
 [tool.poetry.scripts]
 nsg = "nssurge_cli:cli.app"
 nssurge-cli = "nssurge_cli:cli.app"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/nssurge-cli/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-typer = "^0.4.1"
+python = ">=3.11, <4.0"
 nssurge-api = "0.2.10"
 utils-tddschn = "^0.1.5"
-rich = {version = "^12.4.1", extras = ["format"]}
+rich = { version = "^12.4.1", extras = ["format"] }
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
 toml = "^0.10.2"
 yapf = "^0.32.0"
 better-exceptions = "^0.3.3"
 bump2version = "^1.0.1"
 logging-utils-tddschn = "^0.1.8"
 
+[tool.poetry.group.dev.dependencies]
+typer = "^0.9.0"
+pytest = "^7.3.1"
+black = "^23.3.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nssurge-cli-2.0.3/PKG-INFO` & `nssurge_cli-2.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: nssurge-cli
-Version: 2.0.3
+Version: 2.0.4
 Summary: NSSurge CLI
 Home-page: https://github.com/tddschn/nssurge-cli
 License: MIT
 Keywords: nssurge,cli,surge,typer
 Author: Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: nssurge-api (==0.2.10)
 Requires-Dist: rich[format] (>=12.4.1,<13.0.0)
-Requires-Dist: typer (>=0.4.1,<0.5.0)
 Requires-Dist: utils-tddschn (>=0.1.5,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/nssurge-cli/issues
 Project-URL: Repository, https://github.com/tddschn/nssurge-cli
 Description-Content-Type: text/markdown
```

