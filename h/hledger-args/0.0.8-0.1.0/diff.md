# Comparing `tmp/hledger_args-0.0.8.tar.gz` & `tmp/hledger_args-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_args-0.0.8.tar", last modified: Sun May 21 15:20:36 2023, max compression
+gzip compressed data, was "hledger_args-0.1.0.tar", last modified: Wed May 31 00:23:33 2023, max compression
```

## Comparing `hledger_args-0.0.8.tar` & `hledger_args-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.419602 hledger_args-0.0.8/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9956 2023-05-21 15:20:36.418603 hledger_args-0.0.8/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9616 2023-05-21 15:18:13.000000 hledger_args-0.0.8/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.409602 hledger_args-0.0.8/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9616 2023-05-21 15:18:13.000000 hledger_args-0.0.8/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.411602 hledger_args-0.0.8/hledger_args/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.8/hledger_args/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.8/hledger_args/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1822 2023-05-21 15:20:30.000000 hledger_args-0.0.8/hledger_args/base_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2106 2023-05-16 20:53:33.000000 hledger_args-0.0.8/hledger_args/batch_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3766 2023-05-16 20:59:33.000000 hledger_args-0.0.8/hledger_args/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4924 2023-05-21 15:08:55.000000 hledger_args-0.0.8/hledger_args/inter_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-16 19:54:39.000000 hledger_args-0.0.8/hledger_args/options.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1203 2023-05-16 21:00:47.000000 hledger_args-0.0.8/hledger_args/output_result.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.412602 hledger_args-0.0.8/hledger_args.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9956 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      748 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       35 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1167 2023-05-21 15:19:01.000000 hledger_args-0.0.8/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-21 15:20:36.419602 hledger_args-0.0.8/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.412602 hledger_args-0.0.8/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.8/tests/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.408602 hledger_args-0.0.8/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.418603 hledger_args-0.0.8/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-31 00:23:33.557021 hledger_args-0.1.0/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4636 2023-05-31 00:23:33.555021 hledger_args-0.1.0/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4296 2023-05-31 00:22:58.000000 hledger_args-0.1.0/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-31 00:23:33.541021 hledger_args-0.1.0/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4296 2023-05-31 00:22:58.000000 hledger_args-0.1.0/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-31 00:23:33.542021 hledger_args-0.1.0/hledger_args/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.1.0/hledger_args/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.1.0/hledger_args/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1444 2023-05-31 00:22:58.000000 hledger_args-0.1.0/hledger_args/batch_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4552 2023-05-31 00:22:58.000000 hledger_args-0.1.0/hledger_args/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4728 2023-05-31 00:22:58.000000 hledger_args-0.1.0/hledger_args/inter_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2512 2023-05-31 00:22:58.000000 hledger_args-0.1.0/hledger_args/lib.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      718 2023-05-31 00:22:58.000000 hledger_args-0.1.0/hledger_args/options.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-31 00:23:33.543021 hledger_args-0.1.0/hledger_args.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4636 2023-05-31 00:23:33.000000 hledger_args-0.1.0/hledger_args.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      712 2023-05-31 00:23:33.000000 hledger_args-0.1.0/hledger_args.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-31 00:23:33.000000 hledger_args-0.1.0/hledger_args.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-31 00:23:33.000000 hledger_args-0.1.0/hledger_args.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       35 2023-05-31 00:23:33.000000 hledger_args-0.1.0/hledger_args.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-31 00:23:33.000000 hledger_args-0.1.0/hledger_args.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1167 2023-05-31 00:22:58.000000 hledger_args-0.1.0/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-31 00:23:33.557021 hledger_args-0.1.0/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-31 00:23:33.544021 hledger_args-0.1.0/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.1.0/tests/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-31 00:23:33.540021 hledger_args-0.1.0/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-31 00:23:33.555021 hledger_args-0.1.0/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.1.0/venv/bin/rstpep2html.py
```

### Comparing `hledger_args-0.0.8/hledger_args/cli.py` & `hledger_args-0.1.0/hledger_args/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional, Tuple
 
 import rich_click as click
 
-from hledger_args.output_result import output_report
-
-from .batch_args import BatchArgs
-from .inter_args import InteractiveArgs
+from .batch_args import get_batch_reports
+from .inter_args import get_inter_report
+from .lib import create_pdf, get_default_file
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 click.rich_click.USE_MARKDOWN = True
 click.rich_click.SHOW_ARGUMENTS = True
 click.rich_click.GROUP_ARGUMENTS_OPTIONS = True
 click.rich_click.MAX_WIDTH = 80
@@ -27,81 +26,108 @@
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option(
     "-f",
     "--file",
     type=click.STRING,
     required=True,
-    help="Inform the journal file path",
+    default=lambda: get_default_file,
+    multiple=True,
+    help="Pass the journal file path. Can be multiple files",
 )
 @click.option(
     "-i",
     "--interactive",
     is_flag=True,
     required=False,
-    help="Run in interactive mode by answering the prompts. [NAME] and [EXTRA_HLEDGER_OPTIONS] are not used in this mode.",
-)
-@click.option(
-    "-d",
-    "--pdf-dir",
-    type=click.Path(
-        file_okay=False,
-        dir_okay=True,
-    ),
-    required=False,
-    help="Save the report to a folder named according to the current date under the specified directory",
+    help="Run in interactive mode by answering prompts. [NAME] is not used in this mode.",
 )
 @click.option(
     "-o",
     "--pdf-file",
     type=click.Path(file_okay=True, dir_okay=False),
     required=False,
     help="output the report to the specified file in pdf",
 )
-@click.argument("name", type=click.STRING, required=False)
-@click.argument("extra_hledger_options", nargs=-1)
+@click.argument("name", type=click.STRING, required=False, nargs=-1)
 def cli(
-    file: str,
+    file: Tuple[str, ...],
     interactive: bool,
-    name: str,
-    extra_hledger_options: Tuple[str, ...],
-    pdf_dir: Optional[str],
+    name: Tuple[str, str],
     pdf_file: Optional[str],
 ):
     """
-     ---
+    # hledger-args
 
-     **NAME**: Command name to run saved in the journal sub directives. Not available in Interactive mode
+    This package is a replacement for [hledger command file](https://hledger.org/1.29/hledger.html#command-arguments) with additional features.
 
-    **EXTRA_HLEDGER_OPTIONS**: Extra options to send to hledger command. Not available in Interactive mode. The name **"all"** is special and output all the *no interactive* commands.
+    ## Basic Usage
 
-     ---
+    - Save commands directly in the journal file using the custom directive format below.
+    - List available commands with *--file* option without additional name argument
+    - Pass multiple command names to output the reports
+    - Use option *--pdf-file* to save the reports as pdf
+
+    ## Interactive Mode
+
+    Select the report from a menu using the flag *--interactive*.
+
+    Using *placeholders* as below, the user can create a report asking multiple additional information on runtime that read the journal files to provide fuzzy search autocompletion, validation and other conveniences.
+
+    ### Placeholder Command Substitution
+
+     In *Interactive Mode* only, a command can use placeholders by putting them between *curly braces* and additional prompts wil ask for the value and do the proper substitution.
 
-     In basic usage, this package is a replacement for [hledger argument file](https://hledger.org/1.29/hledger.html#command-arguments) using custom directives inside the journal file, instead of referencing to an argument file
+    For example, *{example_placeholder}* will ask for this value and substitute where it is located in the command saved in the journal file.
 
-     **Interactive Mode**: Instead of giving the desired command thru a command-line argument, choose it by selecting from a menu using the flag *--interactive*
+    Some placehoder's name offers additional features
 
-     **Placeholder Command Substitution**: In Interactive Mode, a command can use placeholders by putting them between *curly braces* and additional prompts wil ask for the value and do the proper substitution
+    #### Special Placeholders
 
-     **Special Placeholders**: *{account}, {payee}, {tag}, {tag_name}, {months}, {type}, {cur}* are special placeholders that offers autocomplete with fuzzy search using data from the journal. See the [README](https://github.com/edkedk99/hledger-args) for explanation on each of them
+    - **{account}** : Fuzzy search existing accounts
+    - **{payee}**   : Fuzzy search existing payees
+    - **{cur}**     : Fuzzy search existing commodities
+    - **{tag}**     : Fuzzy search existing tags and values
+    - **{tag_name}**: Search tag name after "_" and fuzzy search existing values for this tag
+    - **{months}**  : Prompt initial and end dates both inclusive. **Diferent from default hledger**
+    - **{type}**    : Select between accounts type
 
-     **Sub directive format**:
+     ## Shell Commands
+
+    Commands name using *{shell_name}* doesn't run hledger by default. It can accept any shell command and receive aditional data from TUI programs with dialog, menus, etc.
+
+    > Placeholder **[file]** subtitute for the path of the first file informed with *--file* option.
+
+    > Can not save to pdf file. Only output to stdout.
+
+     ## Sub directive format
 
      ```text
      #+args [command name]:[hledger options]
      #+args [other command_name]:[other hledger options]
      ```
 
      **Example**:
 
      ```text
      #+args buy_aapl:bal desc:\"Buy AAPL\"
      #+args aapl_cur:bal desc:\"Buy AAPL\" cur:{commodity}
     ```
+
+     ---
+
+     **[NAME]**: Command names to run saved in the journal sub directives. Not available in Interactive mode
+
+     ---
+
     """
 
     if interactive:
-        args = InteractiveArgs((file,))
+        output = get_inter_report(file)
     else:
-        args = BatchArgs((file,), name, extra_hledger_options)
+        output = get_batch_reports(file, name)
 
-    output_report(args, pdf_dir, pdf_file)
+    if pdf_file:
+        create_pdf("", output or "", pdf_file)
+        print(f"Report saved on {pdf_file}")
+    else:
+        click.echo(output)
```

### Comparing `hledger_args-0.0.8/hledger_args/inter_args.py` & `hledger_args-0.1.0/hledger_args/inter_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import subprocess
 from datetime import datetime, timedelta
 from typing import List, Optional, Tuple
 
 import questionary
 from prompt_toolkit.shortcuts import CompleteStyle
 
-from .base_args import BaseArgs
+from .lib import get_files_comm, run_args, run_shell
+from .options import get_namespace_vars
 
 
 def val_date(date: str):
     try:
         datetime.strptime(date, "%Y-%m-%d")
         return True
     except ValueError:
@@ -33,108 +34,110 @@
         match_middle=True,
         style=questionary.Style([("answer", "fg:#f71b07")]),
         complete_style=CompleteStyle.MULTI_COLUMN,
     )
     return question
 
 
-class InteractiveArgs(BaseArgs):
-    def __init__(self, files: Tuple[str, ...]) -> None:
-        super().__init__(files)
-        self.name = self.menu()
-        self.report = self.get_report()
-
-    def ask_placeholder(self, placeholder: str) -> str:
-        if placeholder == "account":
-            choices = self.get_hledger_lines(["accounts"])
-            answer = custom_autocomplete(placeholder, choices).ask()
-        elif placeholder == "tag":
-            tags = self.get_hledger_lines(["tags"])
-            tag = custom_autocomplete(placeholder, choices=tags).ask()
-
-            tag_values = self.get_hledger_lines(["tags", tag, "--values"])
-            value = custom_autocomplete(
-                f"Value for tag {tag}", choices=tag_values
-            ).ask()
-            answer = f'"tag:{tag}={value}"'
-        elif placeholder.startswith("tag_"):
-            tag_name = placeholder.split("_", 1)[1]
-            tag_values = self.get_hledger_lines(["tags", tag_name, "--values"])
-            value = custom_autocomplete(
-                f"Value for tag {tag_name}", choices=tag_values
-            ).ask()
-            answer = f'"tag:{tag_name}={value}"'
-        elif placeholder == "months":
-            initial: str = questionary.text(
-                "Initial", instruction="YYYY-MM-DD", validate=val_date
-            ).ask()
-            final = questionary.text(
-                "Final (inclusive)", instruction="YYYY-MM-DD", validate=val_date
-            ).ask()
-            next_final_date = datetime.strptime(final, "%Y-%m-%d") + timedelta(days=1)
-            next_final = next_final_date.strftime("%Y-%m-%d")
-            answer = f"--begin {initial} --end {next_final}"
-        elif placeholder == "payee":
-            choices = self.get_hledger_lines(["payees"])
-            payee = custom_autocomplete(placeholder, choices).ask()
-            answer = f'"payee:{payee}"'
-        elif placeholder == "cur":
-            choices = self.get_hledger_lines(["commodities"])
-            commodity = custom_autocomplete(placeholder, choices).ask()
-            answer = f'"cur:{commodity}"'
-        elif placeholder == "type":
-            types = dict(
-                Asset="A",
-                Liability="L",
-                Equity="E",
-                Revenue="R",
-                Expense="X",
-                Cash="C",
-                Conversion="V",
-            )
-            choices = list(types.keys())
-            _type = questionary.select("Account Type", choices=choices).ask()
-            type_code = types[_type]
-            answer = f'"type:{type_code}"'
-        else:
-            answer = questionary.text(placeholder).ask()
+def get_hledger_lines(files_comm: List[str], cmds: List[str]):
+    base_comm = ["hledger", *files_comm, *cmds]
+    proc = subprocess.run(base_comm, capture_output=True, check=True)
+    report = proc.stdout.decode("utf8")
+    report_list = [line for line in report.split("\n") if line != ""]
+    return report_list
+
+
+def ask_placeholder(files_comm: List[str], placeholder: str) -> str:
+    if placeholder == "account":
+        choices = get_hledger_lines(files_comm, ["accounts"])
+        answer = custom_autocomplete(placeholder, choices).ask()
+    elif placeholder == "tag":
+        tags = get_hledger_lines(files_comm, ["tags"])
+        tag = custom_autocomplete(placeholder, choices=tags).ask()
+
+        tag_values = get_hledger_lines(files_comm, ["tags", tag, "--values"])
+        value = custom_autocomplete(f"Value for tag {tag}", choices=tag_values).ask()
+        answer = f'"tag:{tag}={value}"'
+    elif placeholder.startswith("tag_"):
+        tag_name = placeholder.split("_", 1)[1]
+        tag_values = get_hledger_lines(files_comm, ["tags", tag_name, "--values"])
+        value = custom_autocomplete(
+            f"Value for tag {tag_name}", choices=tag_values
+        ).ask()
+        answer = f'"tag:{tag_name}={value}"'
+    elif placeholder == "months":
+        initial: str = questionary.text(
+            "Initial", instruction="YYYY-MM-DD", validate=val_date
+        ).ask()
+        final = questionary.text(
+            "Final (inclusive)", instruction="YYYY-MM-DD", validate=val_date
+        ).ask()
+        next_final_date = datetime.strptime(final, "%Y-%m-%d") + timedelta(days=1)
+        next_final = next_final_date.strftime("%Y-%m-%d")
+        answer = f"--begin {initial} --end {next_final}"
+    elif placeholder == "payee":
+        choices = get_hledger_lines(files_comm, ["payees"])
+        payee = custom_autocomplete(placeholder, choices).ask()
+        answer = f'"payee:{payee}"'
+    elif placeholder == "cur":
+        choices = get_hledger_lines(files_comm, ["commodities"])
+        commodity = custom_autocomplete(placeholder, choices).ask()
+        answer = f'"cur:{commodity}"'
+    elif placeholder == "type":
+        types = dict(
+            Asset="A",
+            Liability="L",
+            Equity="E",
+            Revenue="R",
+            Expense="X",
+            Cash="C",
+            Conversion="V",
+        )
+        choices = list(types.keys())
+        _type = questionary.select("Account Type", choices=choices).ask()
+        type_code = types[_type]
+        answer = f'"type:{type_code}"'
+    else:
+        answer = questionary.text(placeholder).ask()
 
+    return answer
+
+
+def substitute(files_comm: List[str], match: re.Match):
+    placeholder: Optional[str] = match.group(1)
+    if placeholder:
+        question_desc = placeholder.replace("{", "").replace("}", "")
+        answer = ask_placeholder(files_comm, question_desc)
         return answer
+    else:
+        return ""
 
-    def substitute(self, match: re.Match):
-        placeholder: Optional[str] = match.group(1)
-        if placeholder:
-            question_desc = placeholder.replace("{", "").replace("}", "")
-            answer = self.ask_placeholder(question_desc)
-            return answer
-        else:
-            return ""
-
-    def replace_options(self, options: str):
-        result = re.sub(r"\{(.*?)\}", self.substitute, options)
-        return result
-
-    def get_hledger_lines(self, cmds: List[str]):
-        base_comm = ["hledger", *self.files_comm, *cmds]
-        proc = subprocess.run(base_comm, capture_output=True, check=True)
-        report = proc.stdout.decode("utf8")
-        report_list = [line for line in report.split("\n") if line != ""]
-        return report_list
-
-    def menu(self):
-        name: str = questionary.select(
-            "Choose report",
-            choices=list(self.names),
-            use_shortcuts=True,
-            use_indicator=False,
-            show_selected=False,
-        ).ask()
-        return name
 
-    def get_report(self):
-        options_str = self.args[self.name]
-        replaced = self.replace_options(options_str)
-
-        if self.name.startswith("shell_"):
-            return self.run_shell(replaced)
-        else:
-            return self.run_args(replaced)
+def replace_options(files_comm: List[str], options: str):
+    result = re.sub(r"\{(.*?)\}", lambda match: substitute(files_comm, match), options)
+    return result
+
+
+def menu(names: List[str]):
+    name: str = questionary.select(
+        "Choose report",
+        choices=names,
+        use_shortcuts=True,
+        use_indicator=False,
+        show_selected=False,
+    ).ask()
+    return name
+
+
+def get_inter_report(files: Tuple[str, ...]):
+    args = get_namespace_vars(files, "args")
+    names = list(args.keys())
+    name = menu(names)
+
+    options_str = args[name]
+    files_comm = get_files_comm(files)
+    replaced = replace_options(files_comm, options_str)
+
+    if name.startswith("shell_"):
+        return run_shell(replaced, files[0])
+    else:
+        return run_args(files, replaced)
```

### Comparing `hledger_args-0.0.8/hledger_args.egg-info/SOURCES.txt` & `hledger_args-0.1.0/hledger_args.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 README.md
 pyproject.toml
 docs/README.md
 hledger_args/__init__.py
 hledger_args/__main__.py
-hledger_args/base_args.py
 hledger_args/batch_args.py
 hledger_args/cli.py
 hledger_args/inter_args.py
+hledger_args/lib.py
 hledger_args/options.py
-hledger_args/output_result.py
 hledger_args.egg-info/PKG-INFO
 hledger_args.egg-info/SOURCES.txt
 hledger_args.egg-info/dependency_links.txt
 hledger_args.egg-info/entry_points.txt
 hledger_args.egg-info/requires.txt
 hledger_args.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `hledger_args-0.0.8/pyproject.toml` & `hledger_args-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_args"
-version = "0.0.8"
+version = "0.1.0"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "questionary",
```

### Comparing `hledger_args-0.0.8/venv/bin/rst2html.py` & `hledger_args-0.1.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2html4.py` & `hledger_args-0.1.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2html5.py` & `hledger_args-0.1.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2latex.py` & `hledger_args-0.1.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2man.py` & `hledger_args-0.1.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2odt.py` & `hledger_args-0.1.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2odt_prepstyles.py` & `hledger_args-0.1.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2pseudoxml.py` & `hledger_args-0.1.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2s5.py` & `hledger_args-0.1.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2xetex.py` & `hledger_args-0.1.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rst2xml.py` & `hledger_args-0.1.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.8/venv/bin/rstpep2html.py` & `hledger_args-0.1.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

