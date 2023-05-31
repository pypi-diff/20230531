# Comparing `tmp/drtodo-0.6.4.tar.gz` & `tmp/drtodo-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtodo-0.6.4.tar", max compression
+gzip compressed data, was "drtodo-0.6.5.tar", max compression
```

## Comparing `drtodo-0.6.4.tar` & `drtodo-0.6.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-05-24 00:54:19.171030 drtodo-0.6.4/LICENSE
--rw-r--r--   0        0        0     9777 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/README.md
--rw-r--r--   0        0        0      224 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/__init__.py
--rw-r--r--   0        0        0       46 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/__main__.py
--rw-r--r--   0        0        0    15460 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/main.py
--rw-r--r--   0        0        0     4703 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/man_command.py
--rw-r--r--   0        0        0     4784 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/mdparser.py
--rw-r--r--   0        0        0     1406 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/mistuneplugin.py
--rw-r--r--   0        0        0      618 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/rich_display.py
--rw-r--r--   0        0        0     7061 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/settings.py
--rw-r--r--   0        0        0       11 2023-05-24 00:54:19.171030 drtodo-0.6.4/drtodo/util.py
--rw-r--r--   0        0        0      808 2023-05-24 00:54:33.283104 drtodo-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-31 19:03:43.606591 drtodo-0.6.5/LICENSE
+-rw-r--r--   0        0        0     9777 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/README.md
+-rw-r--r--   0        0        0      224 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/__init__.py
+-rw-r--r--   0        0        0       46 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/__main__.py
+-rw-r--r--   0        0        0    12223 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/main.py
+-rw-r--r--   0        0        0     4977 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/man_command.py
+-rw-r--r--   0        0        0     4784 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/mdparser.py
+-rw-r--r--   0        0        0     1406 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/mistuneplugin.py
+-rw-r--r--   0        0        0      618 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/rich_display.py
+-rw-r--r--   0        0        0     7061 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/settings.py
+-rw-r--r--   0        0        0       11 2023-05-31 19:03:43.610591 drtodo-0.6.5/drtodo/util.py
+-rw-r--r--   0        0        0      808 2023-05-31 19:03:59.298785 drtodo-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    10671 1970-01-01 00:00:00.000000 drtodo-0.6.5/PKG-INFO
```

### Comparing `drtodo-0.6.4/LICENSE` & `drtodo-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.4/drtodo/README.md` & `drtodo-0.6.5/drtodo/README.md`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.4/drtodo/main.py` & `drtodo-0.6.5/drtodo/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import inspect
 import re
 from pathlib import Path
-from typing import Optional, Callable
+from typing import Optional
 
 import rich.markdown
 import typer
+from typer_aliases import Typer
 from git.repo import Repo
 from rich import print
 
 from .man_command import manapp
 from .mdparser import TaskListTraverser, TodoListParser
 from .rich_display import console
 from .settings import constants, globals, settings, Style
 
-app = typer.Typer(
+
+
+app = Typer(
     no_args_is_help=True,
     rich_markup_mode="markdown",
     help=f"**{constants.appname}, MD**: *a straightforward todo list manager for markdown files in git repos.*",
     epilog=f"DrTodo can manage items in a global todo list ({globals.global_todofile_pretty})"
     f" and in a local todo list ({globals.local_todofile_pretty or 'if the current folder is under a git repo'})."
     f" Settings are read from config files and env variables (see *todo man config*).",
     rich_help_panel="Integration")
@@ -274,15 +276,15 @@
               name="man",
               help="Show detailed help and context for settings, file format and heuristics",
               no_args_is_help=True)
 
 
 def _version_callback(value: bool) -> None:
     if value:
-        print(version_string())
+        console().print(f"{version_string()}", highlight=False)
         raise typer.Exit()
 
 
 panel_GLOBAL = "Global Options"
 panel_FILESELECTION = "File Selection Options"
 
 
@@ -297,80 +299,14 @@
                                           rich_help_panel=panel_FILESELECTION),
     version: Optional[bool] = typer.Option(False, "--version", "-V", help="Show version and exit",
                                            callback=_version_callback, is_eager=True, rich_help_panel=panel_GLOBAL),
 ):
     # BUG: this is called even when the command is init, so it prints a warning about the appdir not existing
     ensure_appdir()
 
-
-# this is fairly generic code that can be used to add aliases to any typer app
-# TODO: move this to a separate package and create decorators for it
-# @app.command_alias(name = 'ls') on the command function
-# @typer_aliases(app=app) on the main() function or maybe @app.typer_aliases()
-def typer_aliases(*, app: typer.Typer,
-                  alias_help_formatter: Optional[Callable[[str], str]] = None,
-                  aliases_help_formatter: Optional[Callable[[str, list[str]], str]] = None) -> None:
-    """
-    Initializes typer aliases for all hidden commands and properly sets the help text for them.
-    Parameters:
-        app: the typer app to modify
-        alias_help_formatter: formats a help string for an aliased command like f"Alias of {command name}"
-        aliases_help_formatter: formats a help string for a command with aliases like f"Aliases: {alias1}, {alias2}"
-    """
-
-    def get_command_name(command_info) -> str:
-        # borrowed from Typer.main.get_command_from_info()
-        name = command_info.name or typer.main.get_command_name(command_info.callback.__name__)
-        return name
-
-    def get_command_help(command_info) -> Optional[str]:
-        # borrowed from Typer.main.get_command_from_info()
-        use_help = command_info.help
-        if use_help is None:
-            use_help = inspect.getdoc(command_info.callback)
-        else:
-            use_help = inspect.cleandoc(use_help)
-        return use_help
-
-    def format_alias_help(aliased_name: str) -> str:
-        if app.rich_markup_mode == "markdown":
-            return f"Alias of `{aliased_name}`"
-        elif app.rich_markup_mode == "rich":
-            return f"Alias of [bold]{aliased_name}[/bold]"
-        else:
-            return f"Alias of {aliased_name}"
-
-    def format_aliases_help(base_help: str, aliases: list[str]) -> str:
-        if app.rich_markup_mode == "markdown":
-            return f"{base_help} *[or {', '.join([f'`{alias}`' for alias in aliases])}]*"
-        elif app.rich_markup_mode == "rich":
-            return f"{base_help} [italics][or {', '.join([f'[bold]{alias}[/bold]' for alias in aliases])}][/italics]"
-        else:
-            return f"{base_help} [or {', '.join(aliases)}]"
-
-    alias_help_formatter = alias_help_formatter or format_alias_help
-    aliases_help_formatter = aliases_help_formatter or format_aliases_help
-
-    aliased_commands = set()
-    # for each command that is not hidden, find any hidden command with the same callback
-    for visible_command in [cmd for cmd in app.registered_commands if not cmd.hidden]:
-        for hidden_command in [cmd for cmd in app.registered_commands if cmd.hidden]:
-            if visible_command.callback == hidden_command.callback:
-                if not hidden_command.help:
-                    hidden_command.help = alias_help_formatter(get_command_name(visible_command))
-                setattr(visible_command, 'aliases', getattr(visible_command, 'aliases', []) + [hidden_command])
-                aliased_commands.add(visible_command)
-
-    # adjust help text for aliased commands
-    for cmd in aliased_commands:
-        basehelp = get_command_help(cmd)
-        if basehelp:
-            cmd.help =  aliases_help_formatter(basehelp, [get_command_name(alias) for alias in cmd.aliases])
-
-
 def main(*args, **kwargs):
-    typer_aliases(app=app)
+    # typer_aliases(app=app)
     app(*args, **kwargs)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `drtodo-0.6.4/drtodo/man_command.py` & `drtodo-0.6.5/drtodo/man_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import typer
 import rich
 import rich.markdown
+import typer
+
+from typer_aliases import Typer
+
 from .rich_display import console
 from .settings import constants, get_default_config
 
-
 man_output = None
-manapp = typer.Typer()
+manapp = Typer()
 
 
 def md_mdfiles():
     return f"""
 # Markdown Files
 
 By default, {constants.appname} will look for any lists formatted as GitHub-style task lists in
@@ -132,27 +134,36 @@
 ```toml
 {get_default_config()}
 ```
 """
 
 
 @manapp.command()
+@manapp.command_alias(name="md")
 def mdfiles():
+    """
+    How Markdown files are used to manage todo items.
+    """
     assert man_output
     man_output(md_mdfiles())
 
 
 @manapp.command()
+@manapp.command_alias(name="settings")
 def config():
+    """
+    Where settings are stored and how to configure them.
+    """
     assert man_output
     man_output(md_config())
 
 
 @manapp.command()
 def all():
+    """List all manual pages"""
     assert man_output
     man_output(md_mdfiles() + "\n\n" + md_config())
 
 
 def output_as_raw(mdstring: str):
     console().print(mdstring, markup=False, highlight=False)
```

### Comparing `drtodo-0.6.4/drtodo/mdparser.py` & `drtodo-0.6.5/drtodo/mdparser.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.4/drtodo/mistuneplugin.py` & `drtodo-0.6.5/drtodo/mistuneplugin.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.4/drtodo/rich_display.py` & `drtodo-0.6.5/drtodo/rich_display.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.4/drtodo/settings.py` & `drtodo-0.6.5/drtodo/settings.py`

 * *Files identical despite different names*

### Comparing `drtodo-0.6.4/pyproject.toml` & `drtodo-0.6.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DrTodo"
-version = "0.6.4"
+version = "0.6.5"
 description = "DrTodo, MD: todo list manager using markdown files and git"
 authors = ["exilium <info@exilium.com>"]
 readme = "drtodo/README.md"
 license = "MIT"
 repository = "https://github.com/exilium-com/DrTodo"
 keywords = ["utilities", "todo", "markdown"]
```

### Comparing `drtodo-0.6.4/PKG-INFO` & `drtodo-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drtodo
-Version: 0.6.4
+Version: 0.6.5
 Summary: DrTodo, MD: todo list manager using markdown files and git
 Home-page: https://github.com/exilium-com/DrTodo
 License: MIT
 Keywords: utilities,todo,markdown
 Author: exilium
 Author-email: info@exilium.com
 Requires-Python: >=3.9,<4.0
```

