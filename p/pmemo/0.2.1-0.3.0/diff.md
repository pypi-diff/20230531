# Comparing `tmp/pmemo-0.2.1.tar.gz` & `tmp/pmemo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmemo-0.2.1.tar", max compression
+gzip compressed data, was "pmemo-0.3.0.tar", max compression
```

## Comparing `pmemo-0.2.1.tar` & `pmemo-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-05-27 15:04:11.916826 pmemo-0.2.1/LICENSE
--rw-r--r--   0        0        0     2265 2023-05-27 15:04:11.916826 pmemo-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/__init__.py
--rw-r--r--   0        0        0     4916 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/custom_select.py
--rw-r--r--   0        0        0     3803 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/main.py
--rw-r--r--   0        0        0     5266 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/memo.py
--rw-r--r--   0        0        0     1502 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/openai_completion.py
--rw-r--r--   0        0        0     5352 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/pmemo_editor.py
--rw-r--r--   0        0        0     2415 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/preferences.py
--rw-r--r--   0        0        0      704 2023-05-27 15:04:11.928826 pmemo-0.2.1/pmemo/utils.py
--rw-r--r--   0        0        0      856 2023-05-27 15:04:11.928826 pmemo-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 pmemo-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-31 16:07:23.166156 pmemo-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2709 2023-05-31 16:07:23.166156 pmemo-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 16:07:23.190157 pmemo-0.3.0/pmemo/__init__.py
+-rw-r--r--   0        0        0     4942 2023-05-31 16:07:23.190157 pmemo-0.3.0/pmemo/custom_select.py
+-rw-r--r--   0        0        0     5440 2023-05-31 16:07:23.190157 pmemo-0.3.0/pmemo/main.py
+-rw-r--r--   0        0        0     5266 2023-05-31 16:07:23.190157 pmemo-0.3.0/pmemo/memo.py
+-rw-r--r--   0        0        0     3205 2023-05-31 16:07:23.190157 pmemo-0.3.0/pmemo/openai_completion.py
+-rw-r--r--   0        0        0     9687 2023-05-31 16:07:23.190157 pmemo-0.3.0/pmemo/pmemo_editor.py
+-rw-r--r--   0        0        0     2415 2023-05-31 16:07:23.190157 pmemo-0.3.0/pmemo/preferences.py
+-rw-r--r--   0        0        0      667 2023-05-31 16:07:23.190157 pmemo-0.3.0/pmemo/utils.py
+-rw-r--r--   0        0        0      905 2023-05-31 16:07:23.190157 pmemo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 pmemo-0.3.0/PKG-INFO
```

### Comparing `pmemo-0.2.1/LICENSE` & `pmemo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.1/README.md` & `pmemo-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 ![image](https://github.com/Asugawara/pmemo/actions/workflows/run_test.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/pmemo?color=green)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pmemo)
 ![GitHub](https://img.shields.io/github/license/Asugawara/pmemo)
 
 
-# Pmemo(Prompt/Python memo)
+# Pmemo
 
-**Pmemo** is a command-line memo(notepad) application that allows seamless editing directly in the terminal, without opening in full-screen mode like traditional text editors.<br>
-Additionally, it provides the functionality to query the selected text to OpenAI's ChatGPT by using `ctrl + o` as a shortcut,
-transforming it into a prompt for interactive inquiries.
+**Pmemo** is a command-line memo editor designed for seamless editing directly in the terminal environment. It offers a range of features to enhance your memo-taking experience and leverages the power of OpenAI's ChatGPT.
 
 ![](https://github.com/Asugawara/pmemo/blob/main/pmemo.gif)
 
+# Features
+- Rebind `ctrl-o` to request to **ChatGPT**
+- Rebind `ctrl-t` to quickly access frequently used registered prompts
+- CUI memo application that allows seamless editing directly in the terminal
+- No fullscreen mode, keeping your workflow within the terminal
+- Efficient search functionality for your memos
+- Easily customizable to fit your preferences
+- Execute code blocks written by you or ChatGPT immediately (Python only)
+
 # Installation
 
 ```bash
 $ pip install pmemo
 ```
 
 # Usage
 
 command | description
 -- | --
 `pm` or `pm new` | create new memo
-`pm edit` | edit memo (searching with a specified query, similar to using the `peco`)
+`pm edit` | edit memo
 `pm list` | list all memos
-`pm preview` | preview memo(markdown) on terminal (searching with a specified query, similar to using the `peco`)
+`pm preview` | preview memo(markdown) on terminal
 `pm preference` | please refer to the [Preference section](https://github.com/Asugawara/pmemo#Preference)
+`pm template` | create a new prompt template for completion usingh `ctrl-t`
+`pm template -e` | edit an existing prompt template.
+`pm run` | execute code blocks within your memos.
 
 
 # Preference
 
 name | default | description
 -- | -- | --
 out_dir | `$HOME/.pmemo` | specifies the directory where Pmemo saves memos
@@ -40,13 +50,14 @@
 editor_preference.indentation_spaces | 4 | sets the number of spaces for indentation (tab size)
 openai_preference.api_key | None | The OpenAI API uses API keys for authentication
 openai_preference.model | "gpt-3.5-turbo" | ID of the model to use
 openai_preference.max_tokens | 16 | the maximum number of tokens to generate in the completion
 openai_preference.temperature | 0 | what sampling temperature to use, between 0 and 2
 openai_preference.n | 1 | how many completions to generate for each prompt
 
+Note: To enable ChatGPT functionality, make sure to set your OpenAI API key as an environment variable or preference.
 
 # Versioning
 This repo uses [Semantic Versioning](https://semver.org/).
 
 # License
 **pmemo** is released under the MIT License. See [LICENSE](/LICENSE) for additional details.
```

### Comparing `pmemo-0.2.1/pmemo/custom_select.py` & `pmemo-0.3.0/pmemo/custom_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,19 @@
                 return choices
 
             return wrapper
         return text
 
     def move_cursor_up(self) -> None:
         self.pointed_at -= 1
-        self.pointed_at = max(0, min(self.pointed_at, self.choice_count - 1))
+        self.pointed_at %= self.choice_count if self.choice_count > 0 else 1
 
     def move_cursor_down(self) -> None:
         self.pointed_at += 1
-        self.pointed_at = max(0, min(self.pointed_at, self.choice_count - 1))
+        self.pointed_at %= self.choice_count if self.choice_count > 0 else 1
 
     def get_pointed_at(self) -> AnyFormattedText:
         self.pointed_at = max(0, min(self.pointed_at, self.choice_count - 1))
         return self._fragments[self.pointed_at][1] if self._fragments else None
 
     def get_key_bindings(self) -> KeyBindingsBase:
         bindings = KeyBindings()
@@ -88,15 +88,15 @@
             if self.key_bindings is None
             else merge_key_bindings([bindings, self.key_bindings])
         )
 
 
 @error_handler
 def custom_select(
-    choices: Union[list[str], dict[str, Path]], max_preview_height: int = 10
+    choices: Union[list[str], dict[str, Path]], max_preview_height: int = 10, **kwargs
 ) -> str:
     """Choose one option from a list of choices while searching with a specified query, similar to using the "peco"
     If the execution is interrupted by a "KeyboardInterrupt" (typically triggered by pressing Ctrl+C), the program will be terminated.
 
     Args:
         choices (Union[list[str], dict[str, Path]]): list or dict of choices displayed on the terminal.
 
@@ -140,9 +140,10 @@
     app: Application[AnyFormattedText] = Application(
         layout=Layout(
             HSplit([text_area, VSplit([candidates_display, preview_display])])
         ),
         key_bindings=control.get_key_bindings(),
         style=Style([("item", ""), ("selected", "underline bg:#d980ff #ffffff")]),
         erase_when_done=True,
+        **kwargs,
     )
     return to_plain_text(app.run()).strip()
```

### Comparing `pmemo-0.2.1/pmemo/main.py` & `pmemo-0.3.0/pmemo/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import argparse
 import copy
+import subprocess
 
-from prompt_toolkit import PromptSession
 from rich.console import Console
 from rich.markdown import Markdown
 
 from pmemo.custom_select import custom_select
 from pmemo.memo import Memo
-from pmemo.openai_completion import OpenAiCompletion
+from pmemo.openai_completion import (
+    OpenAiCompletion,
+    PromptTemplateCompleter,
+    register_prompt_template,
+)
 from pmemo.pmemo_editor import PmemoEditor
 from pmemo.preferences import PREFERENCE_FILE_PATH, PmemoPreference
-from pmemo.utils import error_handler, sort_memos_by_mtime
+from pmemo.utils import error_handler, sort_by_mtime
 
 
 @error_handler
-def update_preference(preferences: dict) -> dict:
+def update_preference(editor: PmemoEditor, preferences: dict) -> dict:
     selected = custom_select(list(preferences))
     if isinstance(preferences[selected], dict):
-        update_preference(preferences[selected])
+        update_preference(editor, preferences[selected])
         return preferences
-    session: PromptSession[str] = PromptSession(
-        f"{selected} = {preferences[selected]} -> "
+    new_val = editor.text(
+        f"{selected} = {preferences[selected]} -> ",
+        str(preferences[selected]),
+        multiline=False,
     )
-    preferences[selected] = session.app.run()
+    if new_val:
+        preferences[selected] = new_val
     return preferences
 
 
 def main():
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(dest="cmd")
     parser_new = subparsers.add_parser(
@@ -40,69 +47,106 @@
     parser_list.add_argument("-p", "--prefix", type=str, default="")
     parser_preview = subparsers.add_parser(
         "preview",
         help="preview memo(markdown) on terminal (searching with a specified query, similar to using the `peco`)",
     )
     parser_preferences = subparsers.add_parser("preference", help="set preferences")
     parser_preferences.add_argument("--init", action="store_true")
+    parser_templates = subparsers.add_parser(
+        "template", help="register/edit prompt templates"
+    )
+    parser_templates.add_argument("-e", "--edit", action="store_true")
+    parser_run = subparsers.add_parser("run", help="run codeblock")
     parser.set_defaults(cmd="new")
     args = parser.parse_args()
 
     preferences = (
         PmemoPreference.parse_file(PREFERENCE_FILE_PATH)
         if PREFERENCE_FILE_PATH.exists()
         else PmemoPreference()
     )
 
+    completer = PromptTemplateCompleter(preferences.out_dir)
+
     editor = PmemoEditor(
         **preferences.editor_preference.dict(),
         openai_completion=OpenAiCompletion(**preferences.openai_preference.dict()),
     )
     if args.cmd == "new":
-        content = editor.text("Memo")
+        content = editor.text("Memo", completer=completer)
         memo = Memo(
             preferences.out_dir,
             content,
             title_max_length=preferences.memo_preference.max_title_length,
         )
         memo.save()
 
     elif args.cmd == "edit":
         candidates = {
-            p.name.strip(): p for p in sort_memos_by_mtime(preferences.out_dir)
+            p.name.strip(): p for p in sort_by_mtime(preferences.out_dir, "*/*.md")
         }
         edit_file_name = custom_select(choices=candidates)
         file_path = candidates[edit_file_name]
         memo = Memo.from_file(file_path, preferences.memo_preference.max_title_length)
-        content = editor.text(f"Edit: {file_path.name}", default=memo.content)
+        content = editor.text(
+            f"Edit: {file_path.name}", default=memo.content, completer=completer
+        )
         memo.edit_content(content)
         memo.save()
 
     elif args.cmd == "list":
-        candidates = sort_memos_by_mtime(preferences.out_dir)
+        candidates = sort_by_mtime(preferences.out_dir, "*/*.md")
         candidates = [p.name for p in candidates if p.name.startswith(args.prefix)]
         print("\n".join(candidates))
 
     elif args.cmd == "preview":
         candidates = {
-            p.name.strip(): p for p in sort_memos_by_mtime(preferences.out_dir)
+            p.name.strip(): p for p in sort_by_mtime(preferences.out_dir, "*/*.md")
         }
         edit_file_name = custom_select(choices=candidates)
         file_path = candidates[edit_file_name]
         console = Console()
         memo_content = Markdown(file_path.read_text())
         console.print(memo_content)
 
     elif args.cmd == "preference":
         if args.init:
             new_preferences = PmemoPreference()
         else:
-            new_preferences_dict = update_preference(copy.deepcopy(preferences.dict()))
+            new_preferences_dict = update_preference(
+                editor, copy.deepcopy(preferences.dict())
+            )
             new_preferences = PmemoPreference.parse_obj(new_preferences_dict)
         new_preferences.write()
 
+    elif args.cmd == "template":
+        if args.edit:
+            prompt_title = custom_select(completer.templates)
+            file_path = completer.templates[prompt_title]
+            prompt_text = editor.text(
+                f"Edit: {file_path.name}", default=file_path.read_text()
+            )
+        else:
+            prompt_title = editor.text("Prompt Title:", multiline=False)
+            prompt_text = editor.text("Prompt Text")
+        register_prompt_template(completer.templates_dir, prompt_title, prompt_text)
+
+    elif args.cmd == "run":
+        memo_title_candidates = [
+            p.parent.name.strip() for p in sort_by_mtime(preferences.out_dir, "*/*.py")
+        ]
+        memo_title = custom_select(memo_title_candidates)
+        codeblock_candidates = {
+            p.name.strip(): p
+            for p in sort_by_mtime(preferences.out_dir / memo_title, "*.py")
+        }
+        if not codeblock_candidates:
+            return
+        target_file = custom_select(codeblock_candidates)
+        subprocess.run(["python3", preferences.out_dir / memo_title / target_file])
+
     else:
         raise NotImplementedError
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pmemo-0.2.1/pmemo/memo.py` & `pmemo-0.3.0/pmemo/memo.py`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.1/pmemo/preferences.py` & `pmemo-0.3.0/pmemo/preferences.py`

 * *Files identical despite different names*

### Comparing `pmemo-0.2.1/pmemo/utils.py` & `pmemo-0.3.0/pmemo/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,21 +9,19 @@
             return func(*args, **kwargs)
         except KeyboardInterrupt:
             exit()
 
     return wrapper
 
 
-def sort_memos_by_mtime(memo_dir: Path) -> list:
+def sort_by_mtime(dir: Path, pattern: str) -> list:
     """
-    Sorts memo files in a directory by modification time.
+    Sorts files in a directory by modification time.
 
     Args:
-        memo_dir (Path): The directory path containing memo files.
+        dir (Path): The directory path containing files.
 
     Returns:
-        list: A sorted list of Path objects representing memo files, sorted in descending order based on modification time.
+        list: A sorted list of Path objects representing files, sorted in descending order based on modification time.
 
     """
-    return sorted(
-        memo_dir.glob("*/*.md"), key=lambda p: p.stat().st_mtime, reverse=True
-    )
+    return sorted(dir.glob(pattern), key=lambda p: p.stat().st_mtime, reverse=True)
```

### Comparing `pmemo-0.2.1/pyproject.toml` & `pmemo-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "pmemo"
-version = "0.2.1"
-description = "Pmemo with ChatGPT is a CUI memo app that enables direct terminal editing without full-screen mode. It integrates OpenAI's ChatGPT, allowing interactive inquiries via the ctrl + o shortcut."
+version = "0.3.0"
+description = "Pmemo is a command-line memo editor designed for seamless editing directly in the terminal environment. It offers a range of features to enhance your memo-taking experience and leverages the power of OpenAI's ChatGPT."
 authors = ["Asugawara <asgasw@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pmemo"}]
 
 [tool.poetry.scripts]
 pm = "pmemo.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pygments = "^2.15.1"
 prompt-toolkit = "^3.0.38"
 rich = "^13.3.5"
 pydantic = "^1.10.7"
 openai = "^0.27.7"
+pyperclip = "^1.8.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
```

### Comparing `pmemo-0.2.1/PKG-INFO` & `pmemo-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 Metadata-Version: 2.1
 Name: pmemo
-Version: 0.2.1
-Summary: Pmemo with ChatGPT is a CUI memo app that enables direct terminal editing without full-screen mode. It integrates OpenAI's ChatGPT, allowing interactive inquiries via the ctrl + o shortcut.
+Version: 0.3.0
+Summary: Pmemo is a command-line memo editor designed for seamless editing directly in the terminal environment. It offers a range of features to enhance your memo-taking experience and leverages the power of OpenAI's ChatGPT.
 Author: Asugawara
 Author-email: asgasw@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pygments (>=2.15.1,<3.0.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Description-Content-Type: text/markdown
 
 ![image](https://github.com/Asugawara/pmemo/actions/workflows/run_test.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/pmemo?color=green)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pmemo)
 ![GitHub](https://img.shields.io/github/license/Asugawara/pmemo)
 
 
-# Pmemo(Prompt/Python memo)
+# Pmemo
 
-**Pmemo** is a command-line memo(notepad) application that allows seamless editing directly in the terminal, without opening in full-screen mode like traditional text editors.<br>
-Additionally, it provides the functionality to query the selected text to OpenAI's ChatGPT by using `ctrl + o` as a shortcut,
-transforming it into a prompt for interactive inquiries.
+**Pmemo** is a command-line memo editor designed for seamless editing directly in the terminal environment. It offers a range of features to enhance your memo-taking experience and leverages the power of OpenAI's ChatGPT.
 
 ![](https://github.com/Asugawara/pmemo/blob/main/pmemo.gif)
 
+# Features
+- Rebind `ctrl-o` to request to **ChatGPT**
+- Rebind `ctrl-t` to quickly access frequently used registered prompts
+- CUI memo application that allows seamless editing directly in the terminal
+- No fullscreen mode, keeping your workflow within the terminal
+- Efficient search functionality for your memos
+- Easily customizable to fit your preferences
+- Execute code blocks written by you or ChatGPT immediately (Python only)
+
 # Installation
 
 ```bash
 $ pip install pmemo
 ```
 
 # Usage
 
 command | description
 -- | --
 `pm` or `pm new` | create new memo
-`pm edit` | edit memo (searching with a specified query, similar to using the `peco`)
+`pm edit` | edit memo
 `pm list` | list all memos
-`pm preview` | preview memo(markdown) on terminal (searching with a specified query, similar to using the `peco`)
+`pm preview` | preview memo(markdown) on terminal
 `pm preference` | please refer to the [Preference section](https://github.com/Asugawara/pmemo#Preference)
+`pm template` | create a new prompt template for completion usingh `ctrl-t`
+`pm template -e` | edit an existing prompt template.
+`pm run` | execute code blocks within your memos.
 
 
 # Preference
 
 name | default | description
 -- | -- | --
 out_dir | `$HOME/.pmemo` | specifies the directory where Pmemo saves memos
@@ -58,14 +69,15 @@
 editor_preference.indentation_spaces | 4 | sets the number of spaces for indentation (tab size)
 openai_preference.api_key | None | The OpenAI API uses API keys for authentication
 openai_preference.model | "gpt-3.5-turbo" | ID of the model to use
 openai_preference.max_tokens | 16 | the maximum number of tokens to generate in the completion
 openai_preference.temperature | 0 | what sampling temperature to use, between 0 and 2
 openai_preference.n | 1 | how many completions to generate for each prompt
 
+Note: To enable ChatGPT functionality, make sure to set your OpenAI API key as an environment variable or preference.
 
 # Versioning
 This repo uses [Semantic Versioning](https://semver.org/).
 
 # License
 **pmemo** is released under the MIT License. See [LICENSE](/LICENSE) for additional details.
```

