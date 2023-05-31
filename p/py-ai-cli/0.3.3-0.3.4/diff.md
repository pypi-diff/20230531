# Comparing `tmp/py-ai-cli-0.3.3.tar.gz` & `tmp/py-ai-cli-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ai-cli-0.3.3.tar", last modified: Wed Apr 26 05:19:29 2023, max compression
+gzip compressed data, was "py-ai-cli-0.3.4.tar", last modified: Wed May 31 09:09:44 2023, max compression
```

## Comparing `py-ai-cli-0.3.3.tar` & `py-ai-cli-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1729 2023-04-26 05:19:09.935734 py-ai-cli-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0     3155 2023-04-26 05:19:09.935734 py-ai-cli-0.3.3/README.md
--rw-r--r--   0        0        0     3940 2023-04-26 05:19:09.935734 py-ai-cli-0.3.3/README_ja.md
--rw-r--r--   0        0        0     2922 2023-04-26 05:19:09.935734 py-ai-cli-0.3.3/README_zh.md
--rw-r--r--   0        0        0     2021 2023-04-26 05:19:10.279737 py-ai-cli-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      680 2023-04-26 05:19:10.279737 py-ai-cli-0.3.3/src/ai_cli/__init__.py
--rw-r--r--   0        0        0     8231 2023-04-26 05:19:10.279737 py-ai-cli-0.3.3/src/ai_cli/bot/__init__.py
--rw-r--r--   0        0        0      195 2023-04-26 05:19:10.279737 py-ai-cli-0.3.3/src/ai_cli/bot/token.py
--rwxr-xr-x   0        0        0    13577 2023-04-26 05:19:10.283737 py-ai-cli-0.3.3/src/ai_cli/cli.py
--rw-r--r--   0        0        0     4468 2023-04-26 05:19:10.283737 py-ai-cli-0.3.3/src/ai_cli/git.py
--rw-r--r--   0        0        0     2873 2023-04-26 05:19:10.283737 py-ai-cli-0.3.3/src/ai_cli/setting.py
--rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 py-ai-cli-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1830 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1092 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3363 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/README.md
+-rw-r--r--   0        0        0     3940 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/README_ja.md
+-rw-r--r--   0        0        0     2922 2023-05-31 09:09:25.696531 py-ai-cli-0.3.4/README_zh.md
+-rw-r--r--   0        0        0     2021 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      680 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/__init__.py
+-rw-r--r--   0        0        0     8380 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/bot/__init__.py
+-rw-r--r--   0        0        0      195 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/bot/token.py
+-rwxr-xr-x   0        0        0    13721 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/cli.py
+-rw-r--r--   0        0        0     4474 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/git.py
+-rw-r--r--   0        0        0     4400 2023-05-31 09:09:26.040537 py-ai-cli-0.3.4/src/ai_cli/setting.py
+-rw-r--r--   0        0        0     3839 1970-01-01 00:00:00.000000 py-ai-cli-0.3.4/PKG-INFO
```

### Comparing `py-ai-cli-0.3.3/CHANGELOG.md` & `py-ai-cli-0.3.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Release v0.3.4
+---------------------------
+
+- fix: `commit` command error when delete file from git
+
 Release v0.3.2
 ---------------------------
 
 - fix: small bug fix
 
 Release v0.3.0
 ---------------------------
```

### Comparing `py-ai-cli-0.3.3/README.md` & `py-ai-cli-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -127,8 +127,14 @@
 export ALL_PROXY=socks5://x.x.x.x:xxxx
 ```
 
 SOCKS5 proxy requires `pip install pysocks`.
 
 ## Additional Information
 
-Please use `ai --help` to view more commands.
+Please use `ai --help` to view more commands.
+
+## Thanks
+
+![JetBrains Logo (Main) logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)
+
+This project is developed using [JetBrains](https://www.jetbrains.com/) products.
```

### Comparing `py-ai-cli-0.3.3/README_ja.md` & `py-ai-cli-0.3.4/README_ja.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.3/README_zh.md` & `py-ai-cli-0.3.4/README_zh.md`

 * *Files identical despite different names*

### Comparing `py-ai-cli-0.3.3/pyproject.toml` & `py-ai-cli-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     "pysocks>=1.7.1",
     "pyperclip>=1.8.2",
     "EdgeGPT>=0.1.22.1",
     "tiktoken>=0.3.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.3.3"
+version = "0.3.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/yufeikang/ai-cli"
 Documentation = "https://github.com/yufeikang/ai-cli/blob/main/README.md"
```

### Comparing `py-ai-cli-0.3.3/src/ai_cli/__init__.py` & `py-ai-cli-0.3.4/src/ai_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 import logging
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 
 HOME = Path.home()
```

### Comparing `py-ai-cli-0.3.3/src/ai_cli/bot/__init__.py` & `py-ai-cli-0.3.4/src/ai_cli/bot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return "\n".join([repr(h) for h in self.history.values()])
 
 
 class Bot(ABC):
     def __init__(self, setting: Setting):
         self.setting = setting
         self.history = ChatHistoryContainer()
-        self.stream = not setting.no_stream
+        self.stream = not setting.no_stream.get_value()
 
     @abstractmethod
     def _ask(self, question: str, stream=None) -> Union[str, Generator]:
         pass
 
     def should_summarize(self) -> bool:
         return False
@@ -113,16 +113,16 @@
         else:
             return (self.history.add_answer(question_id, a) for a in self._ask(question, stream=stream))
 
 
 class GPTBot(Bot):
     def __init__(self, setting: Setting):
         super().__init__(setting)
-        self.model = setting.model
-        self.max_tokens = setting.max_tokens
+        self.model = setting.model.get_value()
+        self.max_tokens = setting.max_tokens.get_value()
 
     def get_messages(self):
         for h in self.history:
             yield {"role": "user", "content": h.question}
             if h.answer is not None:
                 yield {"role": "assistant", "content": h.answer}
 
@@ -142,16 +142,17 @@
         logger.info(f"Summarize: {content}")
         self.history.reset()
         q_id = self.history.add_question("TLDR")
         self.history.add_answer(q_id, content)
 
     def _ask(self, question: str, stream=None) -> Union[str, Generator]:
         messages = list(self.get_messages())
+        logger.debug(f"Messages: {messages}, model: {self.model}, stream: {stream}")
         try:
-            response = openai.ChatCompletion.create(model=self.setting.model, messages=messages, stream=stream)
+            response = openai.ChatCompletion.create(model=self.model, messages=messages, stream=stream)
             if not stream:
                 yield response.choices[0].message.content
             else:
                 for v in response:
                     if "content" in v.choices[0].delta:
                         yield v.choices[0].delta.content
         except openai.error.RateLimitError:
@@ -161,16 +162,16 @@
 
 
 class BingBot(Bot):
     def __init__(self, setting: Setting):
         super().__init__(setting)
         self.style = ConversationStyle.creative
         self.history.answer_append = False
-        self.bot = Chatbot(cookiePath=setting.bing_cookie)
-        logger.info(f"BingBot init, cookie path: {setting.bing_cookie}")
+        self.bot = Chatbot(cookiePath=setting.bing_cookie.get_value())
+        logger.info(f"BingBot init, cookie path: {setting.bing_cookie.get_value()}")
         self.max_conversation = None
         self.current_conversation = 0
         self.prefix_prompt = None
 
     def update_conversation(self, response: dict):
         throttling = response.get("item").get("throttling")
         if throttling:
@@ -187,15 +188,15 @@
             return True
         return super().should_summarize()
 
     def summarize(self):
         # reset conversation
         summary = list(self._ask("", stream=False))[0]
         logger.info(f"Summarize: {summary}")
-        self.bot = Chatbot(cookiePath=self.setting.bing_cookie)
+        self.bot = Chatbot(cookiePath=self.setting.bing_cookie.get_value())
         self.prefix_prompt = summary
 
     def _get_question(self, question: str) -> str:
         if self.prefix_prompt:
             logger.info("Add prefix prompt")
             question = self.prefix_prompt + "\n" + question
             self.prefix_prompt = None
```

### Comparing `py-ai-cli-0.3.3/src/ai_cli/cli.py` & `py-ai-cli-0.3.4/src/ai_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -207,30 +207,30 @@
     type=str,
     nargs="?",
     help="the extra message to add to the commit message",
 )
 
 args = parser.parse_args()
 
-init_logging(setting.log_level if not args.debug else "DEBUG")
+init_logging(setting.log_level.get_value() if not args.debug else "DEBUG")
 
 logger = logging.getLogger(__name__)
 
 if args.api_key:
     openai.api_key = args.api_key
-elif setting.api_key:
-    openai.api_key = setting.api_key
+elif setting.api_key.get_value():
+    openai.api_key = setting.api_key.get_value()
 elif "OPENAI_API_KEY" in os.environ:
     openai.api_key = os.environ["OPENAI_API_KEY"]
 
 proxy = None
 if args.proxy:
     proxy = args.proxy
-elif setting.proxy:
-    proxy = setting.proxy
+elif setting.proxy.get_value():
+    proxy = setting.proxy.get_value()
 elif "HTTP_PROXY" in os.environ:
     proxy = os.environ["HTTP_PROXY"]
 elif "HTTPS_PROXY" in os.environ:
     proxy = os.environ["HTTPS_PROXY"]
 elif "SOCKS_PROXY" in os.environ:
     proxy = os.environ["SOCKS_PROXY"]
 elif "ALL_PROXY" in os.environ:
@@ -245,37 +245,37 @@
             import socks
         except ImportError:
             print("Please install pysocks: pip install pysocks")
             exit(1)
 
 if args.endpoint:
     openai.api_base = args.endpoint
-elif setting.endpoint:
-    openai.api_base = setting.endpoint
+elif setting.endpoint.get_value():
+    openai.api_base = setting.endpoint.get_value()
 elif "OPENAI_API_BASE" in os.environ:
     openai.api_base = os.environ["OPENAI_API_BASE"]
 
 logger.debug("using endpoint: %s", openai.api_base)
 
 
 def _print(text, render):
     content = text
-    if args.raw or setting.raw:
+    if args.raw or setting.raw.get_value():
         render(content)
         return
     markdown = Markdown(
         content,
         inline_code_lexer="auto",
         inline_code_theme="monokai",
     )
     render(markdown)
 
 
 def _ask(question, stream=False):
-    bot_type = args.bot or setting.bot
+    bot_type = args.bot or setting.bot.get_value()
     bot: Bot = get_bot(setting=setting, bot_type=bot_type)
     return bot.ask(question, stream=stream)
 
 
 def ask(question, stream=False):
     content = ""
     if stream:
@@ -323,15 +323,15 @@
     except Exception as e:
         logger.error("error getting text from file: %s", e)
         return None
 
 
 def get_user_input(prompt="Please enter a question"):
     logger.debug("reading question from stdin")
-    multi_line_input = setting.multi_line_input or args.multi_line_input
+    multi_line_input = setting.multi_line_input.get_value() or args.multi_line_input
     if sys.stdin.isatty():
         if multi_line_input:
             console.print(f"[bold blue]{prompt}:, Ctrl+D end input[/bold blue]")
         else:
             console.print(f"[bold blue]{prompt}:[/bold blue]")
     return "\n".join(sys.stdin.readlines()) if multi_line_input else sys.stdin.readline()
 
@@ -378,15 +378,15 @@
         exit(0)
     for f in diff_files:
         console.print(f"[bold blue]Reviewing file: {f}[/bold blue]")
         diff_context = git.get_file_diff(f, args.target)
         if not diff_context:
             console.print(f"[bold red]No diff found for file: {f}")
             continue
-        text = f"{diff_context} \n\n {setting.review_prompt}"
+        text = f"{diff_context} \n\n {setting.review_prompt.get_value()}"
         ask(text, stream=stream)
         Prompt.ask("[bold blue]Press enter to continue[/bold blue]")
     console.print("[bold green]Done![/bold green]")
 
 
 def set_all_setting():
     for k, v in setting:
@@ -404,15 +404,15 @@
         exit(0)
     diff_files = git.get_change_files("HEAD")
     if not diff_files or len(diff_files) == 0:
         console.print("[bold red]No diff files found")
         exit(0)
     console.print(f"[bold blue]Found {len(diff_files)} files changed[/bold blue]")
     diff = git.get_file_diff(diff_files, "HEAD")
-    message = f"{setting.commit_prompt} \n\n {diff}"
+    message = f"{setting.commit_prompt.get_value()} \n\n {diff}"
     result = ask(message, stream=False).strip()
     if args.message:
         result = result + "\n\n" + args.message
     action = Prompt.ask(
         "[bold blue]Do you want to commit these changes?[/bold blue] [(Yes)y/(No)n/(Edit)e]",
         choices=["y", "n", "e"],
         show_choices=False,
```

### Comparing `py-ai-cli-0.3.3/src/ai_cli/git.py` & `py-ai-cli-0.3.4/src/ai_cli/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         logger.debug("path: {}".format(_path))
         if isinstance(_path, list):
             return [_join_path(p) for p in _path]
         if current != git_root:
             _path = os.path.join(git_root, _path).split(current + "/")[1]
         return _path
 
-    cmd = ["git", "--no-pager", "diff", "--cached", target]
+    cmd = ["git", "--no-pager", "diff", "--cached", "--", target]
     _path = _join_path(path)
     if _path:
         cmd.extend([_path] if isinstance(_path, str) else _path)
     res, output = _run_command(cmd)
     if res != 0:
         logging.error("git command failed, cmd: {}".format(cmd))
         return None
```

### Comparing `py-ai-cli-0.3.3/PKG-INFO` & `py-ai-cli-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ai_cli
-Version: 0.3.3
+Version: 0.3.4
 Summary: This CLI tool allows you to easily chat with chatGPT in the command line. You can chat with it, ask questions, and even translate text. It also
 License: MIT
 Author-email: Yufei Kang <kou.uhi.x@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Documentation, https://github.com/yufeikang/ai-cli/blob/main/README.md
 Project-URL: Repository, https://github.com/yufeikang/ai-cli
 Description-Content-Type: text/markdown
@@ -139,7 +139,14 @@
 ```
 
 SOCKS5 proxy requires `pip install pysocks`.
 
 ## Additional Information
 
 Please use `ai --help` to view more commands.
+
+## Thanks
+
+![JetBrains Logo (Main) logo](https://resources.jetbrains.com/storage/products/company/brand/logos/jb_beam.svg)
+
+This project is developed using [JetBrains](https://www.jetbrains.com/) products.
+
```

