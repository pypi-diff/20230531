# Comparing `tmp/configzen-0.2.1.tar.gz` & `tmp/configzen-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.1.tar", max compression
+gzip compressed data, was "configzen-0.2.2.tar", max compression
```

## Comparing `configzen-0.2.1.tar` & `configzen-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.1/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.1/configzen/__main__.py
--rw-r--r--   0        0        0    60674 2023-05-30 13:51:47.402579 configzen-0.2.1/configzen/config.py
--rw-r--r--   0        0        0     2553 2023-05-30 00:29:12.193684 configzen-0.2.1/configzen/errors.py
--rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.2.1/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.1/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.2.1/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.1/LICENSE
--rw-r--r--   0        0        0     1154 2023-05-30 13:52:50.177583 configzen-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7326 2023-05-30 00:29:12.142683 configzen-0.2.1/README.md
--rw-r--r--   0        0        0     7851 1970-01-01 00:00:00.000000 configzen-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.2/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.2/configzen/__main__.py
+-rw-r--r--   0        0        0    60641 2023-05-31 04:04:21.671560 configzen-0.2.2/configzen/config.py
+-rw-r--r--   0        0        0     2460 2023-05-31 03:37:38.318229 configzen-0.2.2/configzen/errors.py
+-rw-r--r--   0        0        0    20820 2023-05-30 00:45:02.555346 configzen-0.2.2/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.2/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.2.2/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1154 2023-05-31 04:06:30.940657 configzen-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.2/README.md
+-rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.2/PKG-INFO
```

### Comparing `configzen-0.2.1/configzen/__main__.py` & `configzen-0.2.2/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.1/configzen/config.py` & `configzen-0.2.2/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         return functools.partial(with_pre_serialize, func)
 
     pre_serialize.register(cls, func)
 
     if not hasattr(cls, "__get_validators__"):
 
         def validator_gen() -> (
-            collections.abc.Generator[collections.abc.Callable[[Any], Any], None, None]
+            collections.abc.Iterator[collections.abc.Callable[[Any], Any]]
         ):
             yield lambda value: post_deserialize.dispatch(cls)(cls, value)
 
         cls.__get_validators__ = validator_gen  # type: ignore[attr-defined]
 
     return cls
 
@@ -542,17 +542,17 @@
         self.ac_parser = ac_parser
 
         if isinstance(resource, (str, os.PathLike)) and not (
             isinstance(resource, str)
             and urllib.parse.urlparse(str(resource)).scheme in _URL_SCHEMES
         ):
             raw_path = os.fspath(resource)
-            if raw_path.startswith("."):
-                self.relative = True
             resource = pathlib.Path(raw_path)
+            if raw_path.startswith(".") and len(resource.parts) > 1:
+                self.relative = True
 
         self.resource = resource
         self.create_if_missing = create_if_missing
         self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
         self.default_kwargs = kwargs.pop(
             "default_kwargs", self.predefined_default_kwargs.copy()
         )
@@ -1089,15 +1089,15 @@
         if isinstance(other, list):
             return self.list_route == other
         return NotImplemented
 
     def __str__(self) -> str:
         return self.compose()
 
-    def __iter__(self) -> collections.abc.Generator[str, None, None]:
+    def __iter__(self) -> collections.abc.Iterator[str]:
         yield from self.list_route
 
 
 def at(
     mapping: Any,
     route: SupportsRoute,
     converter_func: collections.abc.Callable[[Any], dict[str, Any]] = _vars,
@@ -1404,15 +1404,15 @@
         The initial configuration state.
 
     """
 
     initial_state: dict[str, Any]
 
     @abc.abstractmethod
-    def trace_route(self) -> collections.abc.Generator[str, None, None]:
+    def trace_route(self) -> collections.abc.Iterator[str]:
         """Trace the route to where the configuration subcontext points to."""
 
     @property
     def route(self) -> Route:
         """The route to where the configuration subcontext points to."""
         return Route(list(self.trace_route()))
 
@@ -1487,15 +1487,15 @@
     ) -> None:
         self._manager = manager
         self._owner = None
         self._initial_state = {}
 
         self.owner = owner
 
-    def trace_route(self) -> collections.abc.Generator[str, None, None]:
+    def trace_route(self) -> collections.abc.Iterator[str]:
         yield from ()
 
     @property
     def manager(self) -> ConfigManager[ConfigModelT]:
         return self._manager
 
     @property
@@ -1545,15 +1545,15 @@
         self._parent = parent
         self._part = part
 
     @property
     def manager(self) -> ConfigManager[ConfigModelT]:
         return self._parent.manager
 
-    def trace_route(self) -> collections.abc.Generator[str, None, None]:
+    def trace_route(self) -> collections.abc.Iterator[str]:
         yield from self._parent.trace_route()
         yield self._part
 
     @property
     def at(self) -> ConfigAt[ConfigModelT]:
         if self.owner is None:
             msg = "Cannot get section pointed to by an unbound context"
@@ -1706,15 +1706,15 @@
         ctx = contextvars.copy_context()
         _exporting.reset(tok)
         return ctx.run(self.dict, **kwargs)
 
     @no_type_check
     def _iter(
         self, **kwargs: Any
-    ) -> collections.abc.Generator[tuple[str, Any], None, None]:
+    ) -> collections.abc.Iterator[tuple[str, Any]]:
         if kwargs.get("to_dict", False) and _exporting.get():
             state = {}
             for key, value in super()._iter(**kwargs):
                 state[key] = value
             metadata = getattr(self, EXPORT, None)
             if metadata:
                 context = get_context(self)
@@ -1825,14 +1825,15 @@
         state.pop(TOKEN, None)
         return type(self)(**copy.deepcopy(state))
 
     @classmethod
     def load(
         cls: type[ConfigModelT],
         resource: ConfigManager[ConfigModelT] | RawResourceT | None = None,
+        *,
         create_if_missing: bool | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file.
         To reload the configuration, use the `reload()` method.
 
@@ -1938,15 +1939,15 @@
         return context.manager.write(blob, **kwargs)
 
     @classmethod
     async def load_async(
         cls: type[ConfigModelT],
         resource: ConfigManager[ConfigModelT] | RawResourceT | None,
         *,
-        create_if_missing: bool = False,
+        create_if_missing: bool | None = None,
         **kwargs: Any,
     ) -> ConfigModelT:
         """
         Load the configuration file asynchronously.
         To reload the configuration, use the `reload()` method.
 
         Parameters
```

### Comparing `configzen-0.2.1/configzen/errors.py` & `configzen-0.2.2/configzen/errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-"""This module contains all the custom errors raised by _configzen_."""
-
-from __future__ import annotations
-
-import contextlib
-from collections.abc import Generator
-from typing import TYPE_CHECKING, Any
-
-import anyconfig
-
-if TYPE_CHECKING:
-    from configzen.config import ConfigManager
-    from configzen.typedefs import ConfigModelT
-
-
-class ConfigError(Exception):
-    """An error occurred while loading a configuration."""
-
-
-class IncorrectConfigError(ConfigError):
-    """An error occurred while loading a configuration."""
-
-
-class InternalConfigError(ConfigError):
-    """Error to raise before reraising as an underlying error."""
-
-    def __init__(self, msg: str, extra: Any = None) -> None:
-        super().__init__(msg)
-        self.extra = extra
-
-
-class ArgumentSyntaxError(ConfigError):
-    """An error occurred while parsing arguments."""
-
-
-@contextlib.contextmanager
-def pretty_syntax_error(source: str) -> Generator[None, None, None]:
-    """Raise a SyntaxError with a message and a source."""
-    try:
-        yield
-    except InternalConfigError as exc:
-        char_no = exc.extra
-        charlist = ["~"] * len(source)
-        charlist[char_no] = "^"
-        indicator = "".join(charlist)
-        msg = "\n".join(map(str, (exc, repr(source), indicator)))
-        raise ArgumentSyntaxError(msg) from None
-
-
-class UnspecifiedParserError(ConfigError, anyconfig.UnknownFileTypeError):
-    """Could not determine the parser to use."""
-
-
-class ConfigAccessError(ConfigError, LookupError):
-    """An error occurred while accessing configuration part."""
-
-    def __init__(self, config: ConfigModelT, route: str | list[str]) -> None:
-        if not isinstance(route, str):
-            route = ".".join(route)
-        self.route = route
-        super().__init__(
-            f"could not get {type(config).__name__}.{route}",
-        )
-
-
-class ConfigProcessorError(ConfigError):
-    """An error occurred while preprocessing/exporting a configuration."""
-
-
-class ResourceLookupError(ConfigError, LookupError):
-    """An error occurred while looking up a resource."""
-
-    def __init__(
-        self, resource: ConfigManager[ConfigModelT] | None, route: list[str]
-    ) -> None:
-        resource_name = resource.resource if resource else "the provided resource"
-        super().__init__(f"{route} not found in {resource_name}")
-
-
-class ConfigPreprocessingError(ConfigProcessorError, ValueError):
-    """An error occurred while preprocessing a configuration value."""
+"""This module contains all the custom errors raised by _configzen_."""
+
+from __future__ import annotations
+
+import contextlib
+import collections.abc
+from typing import TYPE_CHECKING, Any
+
+import anyconfig
+
+if TYPE_CHECKING:
+    from configzen.config import ConfigManager
+    from configzen.typedefs import ConfigModelT
+
+
+class ConfigError(Exception):
+    """An error occurred while loading a configuration."""
+
+
+class IncorrectConfigError(ConfigError):
+    """An error occurred while loading a configuration."""
+
+
+class InternalConfigError(ConfigError):
+    """Error to raise before reraising as an underlying error."""
+
+    def __init__(self, msg: str, extra: Any = None) -> None:
+        super().__init__(msg)
+        self.extra = extra
+
+
+class ArgumentSyntaxError(ConfigError):
+    """An error occurred while parsing arguments."""
+
+
+@contextlib.contextmanager
+def pretty_syntax_error(source: str) -> collections.abc.Iterator[None]:
+    """Raise a SyntaxError with a message and a source."""
+    try:
+        yield
+    except InternalConfigError as exc:
+        char_no = exc.extra
+        charlist = ["~"] * len(source)
+        charlist[char_no] = "^"
+        indicator = "".join(charlist)
+        msg = "\n".join(map(str, (exc, repr(source), indicator)))
+        raise ArgumentSyntaxError(msg) from None
+
+
+class UnspecifiedParserError(ConfigError, anyconfig.UnknownFileTypeError):
+    """Could not determine the parser to use."""
+
+
+class ConfigAccessError(ConfigError, LookupError):
+    """An error occurred while accessing configuration part."""
+
+    def __init__(self, config: ConfigModelT, route: str | list[str]) -> None:
+        if not isinstance(route, str):
+            route = ".".join(route)
+        self.route = route
+        super().__init__(
+            f"could not get {type(config).__name__}.{route}",
+        )
+
+
+class ConfigProcessorError(ConfigError):
+    """An error occurred while preprocessing/exporting a configuration."""
+
+
+class ResourceLookupError(ConfigError, LookupError):
+    """An error occurred while looking up a resource."""
+
+    def __init__(
+        self, resource: ConfigManager[ConfigModelT] | None, route: list[str]
+    ) -> None:
+        resource_name = resource.resource if resource else "the provided resource"
+        super().__init__(f"{route} not found in {resource_name}")
+
+
+class ConfigPreprocessingError(ConfigProcessorError, ValueError):
+    """An error occurred while preprocessing a configuration value."""
```

### Comparing `configzen-0.2.1/configzen/processor.py` & `configzen-0.2.2/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.1/configzen/typedefs.py` & `configzen-0.2.2/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.1/LICENSE` & `configzen-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.1/pyproject.toml` & `configzen-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.1"
+version = "0.2.2"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.2.1/README.md` & `configzen-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-# configzen
-_configzen_ – managing configuration files easily.
-Currently under development, not ready for production use.
-
-⭐ Contributions welcome! ⭐
-
-## What is this?
-For a more precise and also philosophic explanation, see the wiki article [configzen – explanation without code](https://github.com/bswck/configzen/wiki/configzen-%E2%80%93-explanation-without-code).
-
-_configzen_ combines the power of [pydantic](https://pydantic-docs.helpmanual.io/) 
-and [anyconfig](https://github.com/ssato/python-anyconfig) to provide the most simplistic
-way on Earth of managing configuration files in your Python projects.
-
-Thanks to this, instead of manually using 
-`pyyaml` for YAML configuration files, `configparser` for INI files, `json` for JSON files, etc. 
-you can create a data model of your configuration and let _configzen_ do the rest and provide you 
-with some extra features on top of that, such as both synchronous and asynchronous, 
-preferably full or partial reloading and saving of your structured configuration.
-
-_configzen_ will help you to organize your configuration files and make them easy to use 
-and maintain. One of the core features of _configzen_ is that it allows you to import 
-configuration files inside other configuration files, which is especially useful when you
-have a lot of configuration files, and you want to avoid repeating yourself.
-
-
-## Features
-
-### Managing content
-Let's see how it looks like in practice. Let's say you have a YAML configuration file like this:
-```yaml
-# database.yaml
-host: 127.0.0.1
-port: 5432
-user: postgres
-```
-You can create a data model for it like this:
-
-```python
-# config.py
-from ipaddress import IPv4Address, IPv6Address
-from configzen import ConfigModel, ConfigMeta, ConfigField
-
-
-class DatabaseConfig(ConfigModel):
-    host: IPv4Address | IPv6Address
-    port: int
-    user: str
-    password: str = ConfigField(exclude=True)
-    
-    class Config(ConfigMeta):
-        resource = "database.yaml"
-        env_prefix = "DB_"
-
-
-db_config = DatabaseConfig.load()
-```
-
-As simple as that!
-This way, you can load your configuration from a file as well as from the environment variables
-`DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with 
-the option `exclude=True`, it will not be included in the configuration's exported data: that
-guarantees that your password won't leak into `database.yaml` on save – but you may still pass it 
-through an environment variable (here – the mentioned `DB_PASSWORD`).
-
-[pydantic](https://docs.pydantic.dev/latest/) will take care of parsing and validating the loaded data.
-
-You can now use the `db_config` object to access the configuration values:
-
-```python
->>> db_config.host
-IPv4Address('127.0.0.1')
-```
-
-modify them, if the pydantic model allows it:
-
-```python
->>> db_config.host = "0.0.0.0"
->>> db_config.host
-IPv4Address('0.0.0.0')
-```
-
-as well as reload particular values, without touching the rest of the configuration:
-
-```python
->>> db_config.at("port").reload()
-5432
->>> db_config
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
->>> db_config.at("host").reload()
-IPv4Address('127.0.0.1')
->>> db_config
-DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
-```
-
-or reload the whole configuration:
-
-```python
->>> db_config.port = 1234
->>> db_config.reload()
-DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
-```
-
-or save a particular value, without touching the rest of the configuration:
-
-```python
->>> db_config.host = "0.0.0.0"
->>> db_config.port = 443
->>> db_config
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=443, user='postgres', password='password')
->>> db_config.at("host").save()
-40
->>> db_config.reload()
-DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
-```
-
-or save the whole configuration:
-
-```python
->>> db_config.save()
-39
-```
-
-### Preprocessing directives
-_configzen_ allows you to use built-in preprocessing directives in your configuration files,
-offering features such as importing other configuration files in order to extend 
-your base configuration without writing any code. You might think of it as something
-that is analogous to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
-but for configuration files, broadened to any configuration file format and with some extra features planned.
-
-Thanks to this, you can write your configuration in a modular way, and avoid repeating yourself.
-
-Let's say you have a base configuration file like this (`base.json`):
-
-```json
-{
-  "i18n": {
-    "language": "en",
-    "timezone": "UTC"
-  },
-  "app": {
-    "debug": true
-  }
-}
-```
-
-To extend this configuration, you can create another configuration file like this,
-overriding desired sections as needed:
-
-```yaml
-# production.yaml
-^extend: base.json
-
-+app:
-  debug: false
-```
-
-Using `+` in front of a key will update the section already defined at that key,
-instead of replacing it.
-
-Notice how configuration file formats don't matter in _configzen_: you can 
-extend JSON configurations in YAML, but that might be as well any other format
-among [JSON](https://en.wikipedia.org/wiki/JSON), [INI](https://en.wikipedia.org/wiki/INI_file),
-[XML](https://en.wikipedia.org/wiki/XML), [.properties](https://en.wikipedia.org/wiki/.properties),
-shellvars (
-see [Augeas docs on shellvars](https://augeas.net/docs/references/1.4.0/lenses/files/shellvars-aug.html)),
-[YAML](https://yaml.org), [TOML](https://en.wikipedia.org/wiki/TOML),
-[Amazon Ion](https://en.wikipedia.org/wiki/Ion_(serialization_format)),
-[BSON](https://en.wikipedia.org/wiki/BSON), [CBOR](https://en.wikipedia.org/wiki/CBOR),
-[ConfigObj](https://configobj.readthedocs.io/en/latest/configobj.html#introduction) or
-[MessagePack](https://en.wikipedia.org/wiki/MessagePack).
-
-The above example is equivalent to as if you used:
-
-```yaml
-# production.yaml
-i18n:
-  language: en
-  timezone: UTC
-app:
-  debug: false
-```
-
-With the difference that the primary example, while saving the configuration,
-will preserve the relation to the base configuration file, so that you can reload
-the configuration, and it will be updated with the changes made in the base configuration file.
-
-
-## Setup
-For using _configzen_ in your project, you need to install it first:
-
-```bash
-pip install configzen
-```
-
-For development, you can clone the repository and install its dependencies with [poetry](https://python-poetry.org/):
-```bash
-poetry install --with dev
-```
-
-## License
-[MIT License](https://choosealicense.com/licenses/mit/)
-
-## Contributing
-Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose) 
-or [submit a pull request](https://github.com/bswck/configzen/compare).
-
-## Credits
-* [@Lunarmagpie](https://github.com/Lunarmagpie) for _crucial_ design tips and ideas.
- 
-## Author
-* [bswck](https://github.com/bswck) (contact: bswck.dev@gmail.com or via [Discord](https://discord.com/) `bswck#8238`)
+# configzen
+_configzen_ – managing configuration files easily.
+Currently under development, not ready for production use.
+
+⭐ Contributions welcome! ⭐
+
+## What is this?
+For a more precise and also philosophic explanation, see the wiki article [configzen – explanation without code](https://github.com/bswck/configzen/wiki/configzen-%E2%80%93-explanation-without-code).
+
+_configzen_ combines the power of [pydantic](https://pydantic-docs.helpmanual.io/) 
+and [anyconfig](https://github.com/ssato/python-anyconfig) to provide the most simplistic
+way on Earth of managing configuration files in your Python projects.
+
+Thanks to this, instead of manually using 
+`pyyaml` for YAML configuration files, `configparser` for INI files, `json` for JSON files, etc. 
+you can create a data model of your configuration and let _configzen_ do the rest and provide you 
+with some extra features on top of that, such as both synchronous and asynchronous, 
+preferably full or partial reloading and saving of your structured configuration.
+
+_configzen_ will help you to organize your configuration files and make them easy to use 
+and maintain. One of the core features of _configzen_ is that it allows you to import 
+configuration files inside other configuration files, which is especially useful when you
+have a lot of configuration files, and you want to avoid repeating yourself.
+
+
+## Features
+
+### Managing content
+Let's see how it looks like in practice. Let's say you have a YAML configuration file like this:
+```yaml
+# database.yaml
+host: 127.0.0.1
+port: 5432
+user: postgres
+```
+You can create a data model for it like this:
+
+```python
+# config.py
+from ipaddress import IPv4Address, IPv6Address
+from configzen import ConfigModel, ConfigMeta, ConfigField
+
+
+class DatabaseConfig(ConfigModel):
+    host: IPv4Address | IPv6Address
+    port: int
+    user: str
+    password: str = ConfigField(exclude=True)
+    
+    class Config(ConfigMeta):
+        resource = "database.yaml"
+        env_prefix = "DB_"
+
+
+db_config = DatabaseConfig.load()
+```
+
+As simple as that!
+This way, you can load your configuration from a file as well as from the environment variables
+`DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with 
+the option `exclude=True`, it will not be included in the configuration's exported data: that
+guarantees that your password won't leak into `database.yaml` on save – but you may still pass it 
+through an environment variable (here – the mentioned `DB_PASSWORD`). Secret files are also supported though.
+
+[pydantic](https://docs.pydantic.dev/latest/) will take care of parsing and validating the loaded data.
+
+You can now use the `db_config` object to access the configuration values:
+
+```python
+>>> db_config.host
+IPv4Address('127.0.0.1')
+```
+
+modify them, if the pydantic model allows it:
+
+```python
+>>> db_config.host = "0.0.0.0"
+>>> db_config.host
+IPv4Address('0.0.0.0')
+```
+
+as well as reload particular values, without touching the rest of the configuration:
+
+```python
+>>> db_config.at("port").reload()
+5432
+>>> db_config
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
+>>> db_config.at("host").reload()
+IPv4Address('127.0.0.1')
+>>> db_config
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
+```
+
+or reload the whole configuration:
+
+```python
+>>> db_config.port = 1234
+>>> db_config.reload()
+DatabaseConfig(host=IPv4Address('127.0.0.1'), port=5432, user='postgres', password='password')
+```
+
+or save a particular value, without touching the rest of the configuration:
+
+```python
+>>> db_config.host = "0.0.0.0"
+>>> db_config.port = 443
+>>> db_config
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=443, user='postgres', password='password')
+>>> db_config.at("host").save()
+40
+>>> db_config.reload()
+DatabaseConfig(host=IPv4Address('0.0.0.0'), port=5432, user='postgres', password='password')
+```
+
+or save the whole configuration:
+
+```python
+>>> db_config.save()
+39
+```
+
+### Preprocessing directives
+_configzen_ allows you to use built-in preprocessing directives in your configuration files,
+offering features such as importing other configuration files in order to extend 
+your base configuration without writing any code. You might think of it as something
+that is analogous to [Azure DevOps YAML templates](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops),
+but for configuration files, broadened to any configuration file format and with some extra features planned.
+
+Thanks to this, you can write your configuration in a modular way, and avoid repeating yourself.
+
+Let's say you have a base configuration file like this (`base.json`):
+
+```json
+{
+  "i18n": {
+    "language": "en",
+    "timezone": "UTC"
+  },
+  "app": {
+    "debug": true
+  }
+}
+```
+
+To extend this configuration, you can create another configuration file like this,
+overriding desired sections as needed:
+
+```yaml
+# production.yaml
+^extend: base.json
+
++app:
+  debug: false
+```
+
+Using `+` in front of a key will update the section already defined at that key,
+instead of replacing it.
+
+Notice how configuration file formats don't matter in _configzen_: you can 
+extend JSON configurations in YAML, but that might be as well any other format
+among [JSON](https://en.wikipedia.org/wiki/JSON), [INI](https://en.wikipedia.org/wiki/INI_file),
+[XML](https://en.wikipedia.org/wiki/XML), [.properties](https://en.wikipedia.org/wiki/.properties),
+shellvars (
+see [Augeas docs on shellvars](https://augeas.net/docs/references/1.4.0/lenses/files/shellvars-aug.html)),
+[YAML](https://yaml.org), [TOML](https://en.wikipedia.org/wiki/TOML),
+[Amazon Ion](https://en.wikipedia.org/wiki/Ion_(serialization_format)),
+[BSON](https://en.wikipedia.org/wiki/BSON), [CBOR](https://en.wikipedia.org/wiki/CBOR),
+[ConfigObj](https://configobj.readthedocs.io/en/latest/configobj.html#introduction) or
+[MessagePack](https://en.wikipedia.org/wiki/MessagePack).
+
+The above example is equivalent to as if you used:
+
+```yaml
+# production.yaml
+i18n:
+  language: en
+  timezone: UTC
+app:
+  debug: false
+```
+
+With the difference that the primary example, while saving the configuration,
+will preserve the relation to the base configuration file, so that you can reload
+the configuration, and it will be updated with the changes made in the base configuration file.
+
+
+## Setup
+For using _configzen_ in your project, you need to install it first:
+
+```bash
+pip install configzen
+```
+
+For development, you can clone the repository and install its dependencies with [poetry](https://python-poetry.org/):
+```bash
+poetry install --with dev
+```
+
+## License
+[MIT License](https://choosealicense.com/licenses/mit/)
+
+## Contributing
+Contributions are welcome! Feel free to [open an issue](https://github.com/bswck/configzen/issues/new/choose) 
+or [submit a pull request](https://github.com/bswck/configzen/compare).
+
+## Credits
+* [@Lunarmagpie](https://github.com/Lunarmagpie) for _crucial_ design tips and ideas.
+ 
+## Author
+* [bswck](https://github.com/bswck) (contact: bswck.dev@gmail.com or via [Discord](https://discord.com/) `bswck#8238`)
```

### Comparing `configzen-0.2.1/PKG-INFO` & `configzen-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.1
+Version: 0.2.2
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -75,15 +75,15 @@
 ```
 
 As simple as that!
 This way, you can load your configuration from a file as well as from the environment variables
 `DB_HOST`, `DB_PORT`, `DB_USER` and `DB_PASSWORD`. Since `password` is a field created with 
 the option `exclude=True`, it will not be included in the configuration's exported data: that
 guarantees that your password won't leak into `database.yaml` on save – but you may still pass it 
-through an environment variable (here – the mentioned `DB_PASSWORD`).
+through an environment variable (here – the mentioned `DB_PASSWORD`). Secret files are also supported though.
 
 [pydantic](https://docs.pydantic.dev/latest/) will take care of parsing and validating the loaded data.
 
 You can now use the `db_config` object to access the configuration values:
 
 ```python
 >>> db_config.host
```

