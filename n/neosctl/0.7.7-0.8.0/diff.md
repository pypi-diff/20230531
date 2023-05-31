# Comparing `tmp/neosctl-0.7.7.tar.gz` & `tmp/neosctl-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.7.7.tar", max compression
+gzip compressed data, was "neosctl-0.8.0.tar", max compression
```

## Comparing `neosctl-0.7.7.tar` & `neosctl-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-05-23 14:44:03.004880 neosctl-0.7.7/README.md
--rw-r--r--   0        0        0       22 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/__init__.py
--rw-r--r--   0        0        0     4476 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/auth.py
--rw-r--r--   0        0        0     4677 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/constant.py
--rw-r--r--   0        0        0     4420 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-05-23 14:44:03.004880 neosctl-0.7.7/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/__init__.py
--rw-r--r--   0        0        0      249 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0      723 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/consume.py
--rw-r--r--   0        0        0     4989 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/kafka.py
--rw-r--r--   0        0        0     2809 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0    15074 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/metadata.py
--rw-r--r--   0        0        0     8593 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/product.py
--rw-r--r--   0        0        0     3985 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     5884 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0    12365 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/source.py
--rw-r--r--   0        0        0    13015 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0       55 2023-05-23 14:44:03.005880 neosctl-0.7.7/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     3762 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3080 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      141 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     8408 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0     8127 2023-05-23 14:44:03.006880 neosctl-0.7.7/neosctl/util.py
--rw-r--r--   0        0        0     3013 2023-05-23 14:44:03.006880 neosctl-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-05-31 10:11:42.836576 neosctl-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/constant.py
+-rw-r--r--   0        0        0     4420 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-05-31 10:11:42.836576 neosctl-0.8.0/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    11574 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     4974 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     3842 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3331 2023-05-31 10:11:42.837576 neosctl-0.8.0/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1157 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     3749 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3067 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      141 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     8408 2023-05-31 10:11:42.838576 neosctl-0.8.0/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    12308 2023-05-31 10:11:42.839577 neosctl-0.8.0/neosctl/util.py
+-rw-r--r--   0        0        0     3013 2023-05-31 10:11:42.839577 neosctl-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.0/PKG-INFO
```

### Comparing `neosctl-0.7.7/README.md` & `neosctl-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.7.7
+# Core CLI v0.8.0
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.7.7/neosctl/auth.py` & `neosctl-0.8.0/neosctl/profile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,172 +1,139 @@
-import sys
+import re
 import typing
 
-if sys.version_info < (3, 10):
-    from typing_extensions import ParamSpec
-else:
-    from typing import ParamSpec
-
-
 import click
-import httpx
 import typer
 
 from neosctl import schema, util
-from neosctl.util import (
-    check_profile_exists,
-    constant,
-    exit_with_output,
-    get_user_profile,
-    is_success_response,
-    process_response,
-    read_config_dotfile,
-    upsert_config,
-)
+from neosctl.util import exit_with_output, get_user_profile_section, prettify_json, remove_config, upsert_config
 
 app = typer.Typer()
 
 
-def _auth_url(iam_api_url: str) -> str:
-    return "{}".format(iam_api_url.rstrip("/"))
-
-
-def _check_refresh_token_exists(ctx: click.Context) -> bool:
-    if not ctx.obj.profile.refresh_token:  # nosec: B105
-        raise exit_with_output(
-            msg=f"You need to login. Run neosctl -p {ctx.obj.profile_name} auth login",
-            exit_code=1,
-        )
-
-    return True
+r = re.compile(r"http[s]?:\/\/.*")
 
 
-def _refresh_token(ctx: click.Context) -> httpx.Response:
-    check_profile_exists(ctx)
-    _check_refresh_token_exists(ctx)
-
-    r = util.post(
-        ctx,
-        f"{_auth_url(ctx.obj.get_iam_api_url())}/refresh",
-        json={"refresh_token": ctx.obj.profile.refresh_token},
-    )
+def _validate_url(value: str) -> str:
+    """Validate a given url is a valid url with schema."""
+    m = r.match(value)
+    if m is None:
+        msg = f"Invalid url, must match pattern: `{r}`."
+        raise click.UsageError(msg)
+    return value
 
-    if not is_success_response(r):
-        process_response(r)
-
-    upsert_config(ctx, _update_profile(ctx, schema.Auth(**r.json())))
-
-    return r
-
-
-P = ParamSpec("P")
 
+@app.command()
+def init(
+    ctx: typer.Context,
+    *,
+    hostname: typing.Optional[str] = typer.Option(None, "--host", "-h", callback=util.sanitize),
+    gateway_api_url: typing.Optional[str] = typer.Option(None, "--gateway-api-url", "-g", callback=util.sanitize),
+    registry_api_url: typing.Optional[str] = typer.Option(None, "--registry-api-url", "-r", callback=util.sanitize),
+    iam_api_url: typing.Optional[str] = typer.Option(None, "--iam-api-url", "-i", callback=util.sanitize),
+    storage_api_url: typing.Optional[str] = typer.Option(None, "--storage-api-url", "-s", callback=util.sanitize),
+    username: typing.Optional[str] = typer.Option(None, "--username", "-u", callback=util.sanitize),
+    ignore_tls: bool = typer.Option(
+        False,
+        "--ignore-tls",
+        help="Ignore TLS errors (useful in local/development environments",
+    ),
+    non_interactive: bool = typer.Option(
+        False,
+        "--non-interactive",
+        help="Don't ask for input, generate api values based on hostname.",
+    ),
+) -> None:
+    """Initialise a profile.
 
-def ensure_login(method: typing.Callable[P, httpx.Response]) -> typing.Callable[P, httpx.Response]:
-    """Capture authentication errors and retry requests.
+    Create a profile that can be reused in later commands to define which
+    services to interact with, and which user to interact as.
 
-    On request failure check if the response is a 401, and attempt to refresh the access_token.
-    Retry the request with refreshed token, on subsequent failure, return.
+    Call `init` on an existing profile will update the existing profile.
     """
+    typer.echo(f"Initialising [{ctx.obj.profile_name}] profile.")
+    default_host = f"{hostname}/api/{{}}" if hostname else ""
 
-    def check_access_token(*args: P.args, **kwargs: P.kwargs) -> httpx.Response:
-        ctx = args[0]
-        if not isinstance(ctx, click.Context):
-            # Developer reminder
-            msg = "First argument should be click.Context instance"
-            raise TypeError(msg)
-
-        r = method(*args, **kwargs)
-
-        check_profile_exists(ctx)
-
-        # Try to refresh token
-        # Confirm it is a token invalid 401, registry not configured mistriggers this flow.
-        if r.status_code == constant.UNAUTHORISED_CODE:
-            data = r.json()
-            if "code" in data and data["code"].startswith("A0"):
-                _refresh_token(ctx)
-
-                # Refresh the context
-                c = read_config_dotfile()
-                ctx.obj.config = c
-                ctx.obj.profile = get_user_profile(c, ctx.obj.profile_name)
-
-                r = method(*args, **kwargs)
-
-        return r  # noqa: RET504
-
-    return check_access_token
-
-
-def _update_profile(
-    ctx: click.Context,
-    auth: schema.Auth = schema.Auth(),
-) -> schema.Profile:
-    return schema.Profile(
-        gateway_api_url=ctx.obj.gateway_api_url,
-        registry_api_url=ctx.obj.registry_api_url,
-        iam_api_url=ctx.obj.iam_api_url,
-        storage_api_url=ctx.obj.storage_api_url,
-        user=ctx.obj.profile.user,
-        access_token=auth.access_token,
-        refresh_token=auth.refresh_token,
-        ignore_tls=ctx.obj.profile.ignore_tls,
-    )
-
-
-@app.command()
-def login(
-    ctx: typer.Context,
-    password: typing.Optional[str] = typer.Option(None, "--password", "-p", callback=util.sanitize),
-) -> None:
-    """Login to neos."""
-    check_profile_exists(ctx)
+    if non_interactive and not (hostname and username):
+        raise exit_with_output(
+            msg="\nError: --hostname/-h and --username/-u required for non-interactive mode.",
+            exit_code=1,
+        )
 
-    if password is None:
-        password = typer.prompt(
-            "[{profile}] Enter password for user ({user})".format(
-                profile=ctx.obj.profile_name,
-                user=ctx.obj.profile.user,
-            ),
-            hide_input=True,
+    if non_interactive:
+        gateway_api_url = gateway_api_url or f"{hostname}/api/gateway"
+        storage_api_url = storage_api_url or f"{hostname}/api/storage"
+        iam_api_url = iam_api_url or f"{hostname}/api/iam"
+        registry_api_url = registry_api_url or f"{hostname}/api/registry"
+
+    urls = {
+        "gateway_api_url": gateway_api_url,
+        "registry_api_url": registry_api_url,
+        "iam_api_url": iam_api_url,
+        "storage_api_url": storage_api_url,
+    }
+    for key, default, prompt in [
+        ("gateway", ctx.obj.get_gateway_api_url(), "Gateway API url"),
+        ("registry", ctx.obj.get_registry_api_url(), "Registry API url"),
+        ("iam", ctx.obj.get_iam_api_url(), "IAM API url"),
+        ("storage", ctx.obj.get_storage_api_url(), "Storage API url"),
+    ]:
+        url_key = f"{key}_api_url"
+        url = urls[url_key]
+        if url is None:
+            urls[url_key] = typer.prompt(
+                prompt,
+                default=default or default_host.format(key),
+                value_proc=_validate_url,
+            )
+        else:
+            _validate_url(url)
+
+    if username is None:
+        kwargs = {}
+        if ctx.obj.profile:
+            kwargs["default"] = ctx.obj.profile.user
+        username_input: str = typer.prompt(
+            "Username",
+            **kwargs,
         )
+        username = username_input
 
-    r = util.post(
-        ctx,
-        f"{_auth_url(ctx.obj.get_iam_api_url())}/login",
-        json={"user": ctx.obj.profile.user, "password": password},
+    profile = schema.Profile(  # nosec: B106
+        user=username,
+        access_token="",
+        refresh_token="",
+        ignore_tls=ignore_tls,
+        **urls,
     )
 
-    if not is_success_response(r):
-        process_response(r)
+    upsert_config(ctx, profile)
 
-    upsert_config(ctx, _update_profile(ctx, schema.Auth(**r.json())))
 
-    raise exit_with_output(
-        msg="Login success",
-        exit_code=0,
-    )
+@app.command()
+def delete(
+    ctx: typer.Context,
+) -> None:
+    """Delete a profile."""
+    typer.confirm(f"Remove [{ctx.obj.profile_name}] profile", abort=True)
+    remove_config(ctx)
 
 
 @app.command()
-def logout(ctx: typer.Context) -> None:
-    """Logout from neos."""
-    check_profile_exists(ctx)
-
-    _check_refresh_token_exists(ctx)
-
-    r = util.post(
-        ctx,
-        f"{_auth_url(ctx.obj.get_iam_api_url())}/logout",
-        json={"refresh_token": ctx.obj.profile.refresh_token},
+def view(
+    ctx: typer.Context,
+) -> None:
+    """View configuration for a profile."""
+    profile = get_user_profile_section(ctx.obj.config, ctx.obj.profile_name)
+    raise exit_with_output(
+        msg=prettify_json({k: v for k, v in profile.items()}),
     )
 
-    if not is_success_response(r):
-        process_response(r)
-
-    upsert_config(ctx, _update_profile(ctx, schema.Auth()))
 
+@app.command(name="list")
+def list_profiles(
+    ctx: typer.Context,
+) -> None:
+    """List available profiles."""
     raise exit_with_output(
-        msg="Logout success",
-        exit_code=0,
+        msg=prettify_json(sorted(ctx.obj.config.sections())),
     )
```

### Comparing `neosctl-0.7.7/neosctl/cli.py` & `neosctl-0.8.0/neosctl/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     auth,
     constant,
     profile,
     schema,
     services,
     util,
 )
-from neosctl.util import get_user_profile, read_config_dotfile
+from neosctl.util import get_user_profile, read_config_dotfile, user_profile_callback
 
 
 def _generate_common_schema(
     gateway_api_url: str,
     registry_api_url: str,
     iam_api_url: str,
     storage_api_url: str,
@@ -107,34 +107,29 @@
         config=config,
         profile=user_profile,
     )
 
     ctx.obj = common_schema
 
 
-def _common(
-    ctx: typer.Context,
-) -> None:
-    """Inject required user_profile into context."""
-    user_profile = get_user_profile(ctx.obj.config, ctx.obj.profile_name)
-    ctx.obj.profile = user_profile
-
-
 app = typer.Typer(name="neosctl", callback=_callback)
 app.add_typer(profile.app, name="profile", help="Manage profiles.")
-app.add_typer(auth.app, name="auth", callback=_common, help="Manage authentication status.")
+app.add_typer(auth.app, name="auth", callback=user_profile_callback, help="Manage authentication status.")
+app.add_typer(services.iam.app, name="iam", callback=user_profile_callback, help="Manage access policies.")
+app.add_typer(
+    services.storage.app,
+    name="storage",
+    callback=user_profile_callback,
+    help="Interact with Storage (as a service).",
+)
+app.add_typer(
+    services.gateway.app,
+    name="gateway",
+    callback=user_profile_callback,
+    help="Interact with Gateway service.",
+)
 app.add_typer(
-    services.gateway.consume.app,
-    name="consume",
-    callback=_common,
-    help="Consume published data products.",
+    services.registry.app,
+    name="registry",
+    callback=user_profile_callback,
+    help="Manage cores and search data products.",
 )
-app.add_typer(services.iam.app, name="iam", callback=_common, help="Manage access policies.")
-app.add_typer(services.storage.app, name="storage", callback=_common, help="Interact with Storage (as a service).")
-app.add_typer(services.gateway.metadata.app, name="metadata", callback=_common, help="Manage and browse metadata.")
-app.add_typer(services.gateway.product.app, name="product", callback=_common, help="Manage data products.")
-app.add_typer(services.gateway.source.app, name="source", help="Manage sources.")
-app.add_typer(services.registry.app, name="registry", callback=_common, help="Manage cores and search data products.")
-app.add_typer(services.gateway.spark.app, name="spark", callback=_common, help="Manage data product spark jobs.")
-app.add_typer(services.gateway.secret.app, name="secret", callback=_common, help="Manage secrets.")
-app.add_typer(services.gateway.kafka.app, name="kafka", callback=_common, help="Manage data product kafka streaming.")
-app.add_typer(services.gateway.link.app, name="link", callback=_common, help="Manage links.")
```

### Comparing `neosctl-0.7.7/neosctl/schema.py` & `neosctl-0.8.0/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.7/neosctl/services/gateway/link.py` & `neosctl-0.8.0/neosctl/services/registry/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,116 @@
 import httpx
 import typer
 
 from neosctl import util
-from neosctl.auth import ensure_login
+from neosctl.services.registry.schema import RegisterCore, RemoveCore
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
-def _link_url(ctx: typer.Context) -> str:
-    return "{}/link".format(ctx.obj.gateway_api_url.rstrip("/"))
+def _core_url(registry_api_url: str) -> str:
+    return "{}/core".format(registry_api_url.rstrip("/"))
 
 
-@app.command(name="list")
-def list_links(
+def _data_product_url(registry_api_url: str, postfix: str = "") -> str:
+    return "{}/data_product{}".format(registry_api_url.rstrip("/"), postfix)
+
+
+@app.command(name="register-core")
+def register_core(
     ctx: typer.Context,
+    partition: str = typer.Argument(..., help="Core partition", callback=util.sanitize),
+    name: str = typer.Argument(..., help="Core name", callback=util.sanitize),
 ) -> None:
-    """List all links."""
+    """Register a core.
 
-    @ensure_login
-    def _request(ctx: typer.Context) -> httpx.Response:
-        return util.get(
+    Register a core to receive an identifier and access key for use in deployment.
+    """
+
+    @util.ensure_login
+    def _request(ctx: typer.Context, rc: RegisterCore) -> httpx.Response:
+        return util.post(
             ctx,
-            url=_link_url(ctx),
+            _core_url(ctx.obj.get_registry_api_url()),
+            json=rc.dict(exclude_none=True),
         )
 
-    r = _request(ctx)
+    rc = RegisterCore(partition=partition, name=name)
+
+    r = _request(ctx, rc)
     process_response(r)
 
 
-@app.command()
-def link_product_product(
+@app.command(name="list-cores")
+def list_cores(
     ctx: typer.Context,
-    parent: str = typer.Argument(..., help="Parent data product identifier", callback=util.sanitize),
-    child: str = typer.Argument(..., help="Child data product identifier", callback=util.sanitize),
 ) -> None:
-    """Link data products."""
+    """List existing registered cores."""
 
-    @ensure_login
+    @util.ensure_login
     def _request(ctx: typer.Context) -> httpx.Response:
-        return util.post(
+        return util.get(
             ctx,
-            url=f"{_link_url(ctx)}/product/{parent}/product/{child}",
+            _core_url(ctx.obj.get_registry_api_url()),
         )
 
     r = _request(ctx)
     process_response(r)
 
 
-@app.command()
-def unlink_product_product(
+@app.command(name="remove-core")
+def remove_core(
     ctx: typer.Context,
-    parent: str = typer.Argument(..., help="Parent data product identifier", callback=util.sanitize),
-    child: str = typer.Argument(..., help="Child data product identifier", callback=util.sanitize),
+    urn: str = typer.Argument(..., help="Core urn", callback=util.sanitize),
 ) -> None:
-    """Unlink data products."""
+    """Remove a registered core."""
 
-    @ensure_login
-    def _request(ctx: typer.Context) -> httpx.Response:
+    @util.ensure_login
+    def _request(ctx: typer.Context, rc: RemoveCore) -> httpx.Response:
         return util.delete(
             ctx,
-            url=f"{_link_url(ctx)}/product/{parent}/product/{child}",
+            url=_core_url(ctx.obj.get_registry_api_url()),
+            json=rc.dict(exclude_none=True),
         )
 
-    r = _request(ctx)
+    rc = RemoveCore(urn=urn)
+
+    r = _request(ctx, rc)
     process_response(r)
 
 
-@app.command()
-def link_source_product(
+@app.command(name="search")
+def search_products(
     ctx: typer.Context,
-    parent: str = typer.Argument(..., help="Parent source identifier", callback=util.sanitize),
-    child: str = typer.Argument(..., help="Child data product identifier", callback=util.sanitize),
+    search_term: str = typer.Argument(..., callback=util.sanitize),
 ) -> None:
-    """Link source and data product."""
+    """Search published data products across cores."""
 
-    @ensure_login
-    def _request(ctx: typer.Context) -> httpx.Response:
-        return util.post(
+    @util.ensure_login
+    def _request(ctx: typer.Context, search_term: str) -> httpx.Response:
+        return util.get(
             ctx,
-            url=f"{_link_url(ctx)}/source/{parent}/product/{child}",
+            _data_product_url(ctx.obj.get_registry_api_url(), "/search"),
+            params={"search_term": search_term},
         )
 
-    r = _request(ctx)
+    r = _request(ctx, search_term)
     process_response(r)
 
 
-@app.command()
-def unlink_source_product(
+@app.command(name="get-product")
+def get_product(
     ctx: typer.Context,
-    parent: str = typer.Argument(..., help="Parent source identifier", callback=util.sanitize),
-    child: str = typer.Argument(..., help="Child data product identifier", callback=util.sanitize),
+    urn: str = typer.Argument(..., callback=util.sanitize),
 ) -> None:
-    """Unlink source and data product."""
+    """Get data product details."""
 
-    @ensure_login
-    def _request(ctx: typer.Context) -> httpx.Response:
-        return util.delete(
+    @util.ensure_login
+    def _request(ctx: typer.Context, urn: str) -> httpx.Response:
+        return util.get(
             ctx,
-            url=f"{_link_url(ctx)}/source/{parent}/product/{child}",
+            _data_product_url(ctx.obj.get_registry_api_url(), f"/urn/{urn}"),
         )
 
-    r = _request(ctx)
+    r = _request(ctx, urn)
     process_response(r)
```

### Comparing `neosctl-0.7.7/neosctl/services/iam/iam.py` & `neosctl-0.8.0/neosctl/services/iam/iam.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing
 
 import httpx
 import typer
 
 from neosctl import util
-from neosctl.auth import ensure_login
 from neosctl.services.iam import schema
 from neosctl.util import process_response
 
 app = typer.Typer()
 
 
 def _iam_url(iam_api_url: str, postfix: str = "") -> str:
@@ -20,15 +19,15 @@
     ctx: typer.Context,
     page: int = typer.Option(1, help="Page number."),
     page_size: int = typer.Option(10, help="Page size number."),
     resource: typing.Optional[str] = typer.Option(None, help="Resource nrn.", callback=util.sanitize),
 ) -> None:
     """List existing policies."""
 
-    @ensure_login
+    @util.ensure_login
     def _request(ctx: typer.Context) -> httpx.Response:
         params: typing.Dict[str, typing.Union[int, str]] = {"page": page, "page_size": page_size}
         if resource:
             params["resource"] = resource
 
         return util.get(
             ctx,
@@ -43,15 +42,15 @@
 @app.command(name="create")
 def create_from_json(
     ctx: typer.Context,
     filepath: str = typer.Argument(..., help="Filepath of the user policy json payload", callback=util.sanitize),
 ) -> None:
     """Create an IAM policy."""
 
-    @ensure_login
+    @util.ensure_login
     def _request(ctx: typer.Context, user_policy: schema.UserPolicy) -> httpx.Response:
         return util.post(
             ctx,
             "{iam_url}".format(iam_url=_iam_url(ctx.obj.get_iam_api_url(), "policy/user")),
             json=user_policy.dict(),
         )
 
@@ -68,15 +67,15 @@
 def update_from_json(
     ctx: typer.Context,
     principal: str = typer.Argument(..., help="Principal uuid", callback=util.sanitize),
     filepath: str = typer.Argument(..., help="Filepath of the user policy json payload", callback=util.sanitize),
 ) -> None:
     """Update an existing IAM policy."""
 
-    @ensure_login
+    @util.ensure_login
     def _request(ctx: typer.Context, user_policy: schema.UserPolicy) -> httpx.Response:
         return util.put(
             ctx,
             "{iam_url}".format(iam_url=_iam_url(ctx.obj.get_iam_api_url(), "policy/user")),
             params={"user_nrn": principal},
             json=user_policy.dict(),
         )
@@ -93,15 +92,15 @@
 @app.command()
 def delete(
     ctx: typer.Context,
     user_nrn: str = typer.Argument(..., callback=util.sanitize),
 ) -> None:
     """Delete an existing IAM policy."""
 
-    @ensure_login
+    @util.ensure_login
     def _request(ctx: typer.Context) -> httpx.Response:
         return util.delete(
             ctx,
             "{iam_url}".format(iam_url=_iam_url(ctx.obj.get_iam_api_url(), "policy/user")),
             params={"user_nrn": user_nrn},
         )
 
@@ -112,15 +111,15 @@
 @app.command()
 def get(
     ctx: typer.Context,
     user_nrn: str = typer.Argument(..., callback=util.sanitize),
 ) -> None:
     """Get an existing IAM policy."""
 
-    @ensure_login
+    @util.ensure_login
     def _request(ctx: typer.Context) -> httpx.Response:
         return util.get(
             ctx,
             "{iam_url}".format(iam_url=_iam_url(ctx.obj.get_iam_api_url(), "policy/user")),
             params={"user_nrn": user_nrn},
         )
```

### Comparing `neosctl-0.7.7/neosctl/services/iam/schema.py` & `neosctl-0.8.0/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.7/neosctl/services/storage/storage.py` & `neosctl-0.8.0/neosctl/services/storage/storage.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.7.7/pyproject.toml` & `neosctl-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.7.7"
+version = "0.8.0"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.7.7/PKG-INFO` & `neosctl-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.7.7
+Version: 0.8.0
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.7.7
+# Core CLI v0.8.0
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

