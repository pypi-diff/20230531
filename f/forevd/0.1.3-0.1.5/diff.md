# Comparing `tmp/forevd-0.1.3.tar.gz` & `tmp/forevd-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.1.3.tar", max compression
+gzip compressed data, was "forevd-0.1.5.tar", max compression
```

## Comparing `forevd-0.1.3.tar` & `forevd-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-12 13:44:29.592854 forevd-0.1.3/LICENSE
--rw-r--r--   0        0        0      832 2023-05-12 13:44:29.592854 forevd-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-12 13:44:29.592854 forevd-0.1.3/forevd/__init__.py
--rw-r--r--   0        0        0     4390 2023-05-12 13:44:29.592854 forevd-0.1.3/forevd/__main__.py
--rw-r--r--   0        0        0     1498 2023-05-12 13:44:29.592854 forevd-0.1.3/forevd/apache/__init__.py
--rw-r--r--   0        0        0     3429 2023-05-12 13:44:29.592854 forevd-0.1.3/forevd/apache/httpd.conf
--rw-r--r--   0        0        0        0 2023-05-12 13:44:29.592854 forevd-0.1.3/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 13:44:29.592854 forevd-0.1.3/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-05-12 13:44:29.592854 forevd-0.1.3/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      844 2023-05-12 13:44:29.592854 forevd-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 forevd-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 18:58:46.623227 forevd-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4019 2023-05-31 18:58:46.623227 forevd-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/__init__.py
+-rw-r--r--   0        0        0     4760 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/__main__.py
+-rw-r--r--   0        0        0     1543 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     4500 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0      216 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/app.py
+-rw-r--r--   0        0        0        0 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-31 18:58:46.627226 forevd-0.1.5/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      884 2023-05-31 18:58:46.627226 forevd-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 forevd-0.1.5/PKG-INFO
```

### Comparing `forevd-0.1.3/LICENSE` & `forevd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.1.3/forevd/__main__.py` & `forevd-0.1.5/forevd/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,24 @@
     cli.init_logging("forevd.resources.logging", "cli.conf")
 
     if debug:
         logging.getLogger().setLevel(logging.DEBUG)
         logging.getLogger("forevd").setLevel(logging.DEBUG)
 
 
-def _nomalize_locations(locations: list, backend: str, location: str, mtls: bool):
+def _nomalize_locations(
+    locations: dict, backend: str, location: str, mtls: bool, http_methods: list
+):
     if not locations:
         locations = {}
 
     loc_struct = locations.get(location, {})
     loc_struct["backend"] = backend
     loc_struct["mtls"] = mtls
+    loc_struct["http_methods"] = http_methods
 
     locations[location] = loc_struct
 
     return locations
 
 
 @click.command()
@@ -94,34 +97,44 @@
     "--err-log",
     help="Location of the error log",
     type=click.Path(),
     default=_DEFAULT_ERRLOG,
     show_default=True,
 )
 @click.option(
+    "--http-methods",
+    help="Restrict HTTP method calls for the supplied list ",
+    type=cli.StrList,
+)
+@click.option(
+    "--ldap",
+    help="Provide the LDAP config in a JSON or YAML string or file",
+    type=cli.FromJsonOrYaml(),
+)
+@click.option(
     "--listen",
-    help="The ip/hostname and port to listen on",
+    help="The IP/hostname and port to listen on",
     type=str,
     default=_DEFAULT_LISTEN,
     show_default=True,
 )
 @click.option(
     "--location",
     help="Provide a json string or file with location details",
     type=str,
 )
 @click.option(
     "--locations",
-    help="Provide a json string or file with location details",
+    help="Provide the Location config in a JSON or YAML string or file",
     type=cli.FromJsonOrYaml(),
 )
 @click.option("--mtls", help="Enable mutual TLS", type=click.Choice(["optional", "require"]))
 @click.option(
     "--oidc",
-    help="Provide the OIDC config in a json string; e.g. `provider_metada_url`",
+    help="Provide the OIDC config in a JSON or YAML string or file",
     type=cli.FromJsonOrYaml(),
 )
 @click.option(
     "--server-name",
     help="Define the server name, else it uses $HOSTNAME",
     type=str,
     show_default=True,
@@ -143,38 +156,39 @@
     ca_cert,
     cert,
     cert_key,
     cmd,
     debug,
     err_log,
     do_exec,
+    http_methods,
+    ldap,
     listen,
     location,
     locations,
     mtls,
     oidc,
     server_name,
     var_dir,
 ):
-    """forevd is a forward/reverse proxy, primarily used as a sidecar for REST or any HTTP/s
-    applications.
-    """
+    """forevd is a forward/reverse proxy, primarily used as a sidecar for REST or any HTTP/s apps."""
     _setup_logging(debug)
 
     if not backend and location and not locations:
         raise click.UsageError("You must supply a --backend and --location or --locations")
 
     config = {
         "err_log": err_log,
         "access_log": access_log,
         "ca_cert": ca_cert,
         "cert": cert,
         "cert_key": cert_key,
         "debug": debug,
-        "locations": _nomalize_locations(locations, backend, location, mtls),
+        "ldap": ldap,
+        "locations": _nomalize_locations(locations, backend, location, mtls, http_methods),
         "listen": listen,
         "oidc": oidc,
         "server_name": server_name,
     }
     _LOGGER.debug(f"config: {config}")
 
     mod = importlib.import_module(f"forevd.{backend_type}")
```

### Comparing `forevd-0.1.3/forevd/apache/__init__.py` & `forevd-0.1.5/forevd/apache/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 def run(var_dir: str, config: dict, do_exec: bool, cmd: str = None):
     """Execute Apache given the config."""
 
     jinja_env = jinja2.Environment(
         loader=jinja2.PackageLoader("forevd", "apache"), autoescape=jinja2.select_autoescape()
     )
+    jinja_env.add_extension("jinja2.ext.do")
 
     template = jinja_env.get_template("httpd.conf")
 
     apache_config = template.render(**config)
     _LOGGER.debug(f"apache_config: {apache_config}")
 
     config_file = os.path.join(var_dir, "httpd.conf")
```

### Comparing `forevd-0.1.3/pyproject.toml` & `forevd-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "forevd"
-version = "0.1.3"
+version = "0.1.5"
 description = "Forward and reverse proxy using nginx or apache"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Jinja2 = "^3.1.2"
 requests = "^2.28.1"
-firestone-lib = "^0.1.5"
+firestone-lib = "^0.1.8"
+fastapi = "^0.95.2"
+uvicorn = "^0.22.0"
 
 [tool.poetry.group.build.dependencies]
 black = "^22.10.0"
 pytest = "^7.2.0"
 pylint = "^2.15.5"
 pytest-mock = "^3.10.0"
 mock = "^4.0.3"
```

