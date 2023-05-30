# Comparing `tmp/git_llm-0.1.0.tar.gz` & `tmp/git_llm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_llm-0.1.0.tar", max compression
+gzip compressed data, was "git_llm-0.1.2.tar", max compression
```

## Comparing `git_llm-0.1.0.tar` & `git_llm-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-30 20:33:24.939500 git_llm-0.1.0/LICENSE
--rw-r--r--   0        0        0     2054 2023-05-30 20:33:24.939500 git_llm-0.1.0/README.md
--rw-r--r--   0        0        0      840 2023-05-30 20:33:24.939500 git_llm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 20:33:24.939500 git_llm-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     1718 2023-05-30 20:33:24.939500 git_llm-0.1.0/src/cli.py
--rw-r--r--   0        0        0      745 2023-05-30 20:33:24.939500 git_llm-0.1.0/src/gitutils.py
--rw-r--r--   0        0        0     2511 2023-05-30 20:33:24.939500 git_llm-0.1.0/src/llm.py
--rw-r--r--   0        0        0      408 2023-05-30 20:33:24.939500 git_llm-0.1.0/src/prompt.py
--rw-r--r--   0        0        0      820 2023-05-30 20:33:24.939500 git_llm-0.1.0/src/utils.py
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 git_llm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 22:27:54.731972 git_llm-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2221 2023-05-30 22:27:54.731972 git_llm-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/__init__.py
+-rw-r--r--   0        0        0     2433 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/cli.py
+-rw-r--r--   0        0        0     2497 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/llm.py
+-rw-r--r--   0        0        0      852 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/prompt.py
+-rw-r--r--   0        0        0        0 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/utils/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/utils/git.py
+-rw-r--r--   0        0        0      819 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/utils/helpers.py
+-rw-r--r--   0        0        0      848 2023-05-30 22:27:54.735972 git_llm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 git_llm-0.1.2/PKG-INFO
```

### Comparing `git_llm-0.1.0/LICENSE` & `git_llm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `git_llm-0.1.0/README.md` & `git_llm-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 ## git-llm
 
-The project integrates Git with a llm (OpenAI, LlamaCpp, and GPT-4-All) to extend the capabilities of git.
+The project integrates Git with a llm (OpenAI, LlamaCpp, and GPT-4-All) to extend the capabilities of git. It supports
+offline processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or
+you can use OpenAI if privacy is not a concern for you. It is only recommended for educational purposes and not for
+production use.
 
-## Description
-
-git-llm is a tool that allows you to generate changelog entries, and other things using OpenAI, LlamaCpp, and GPT-4-All.
-It supports
-offline processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third
-parties, or you can use OpenAI if privacy is not a concern for you. It is only recommended for educational purposes and
-not for production use.
-
-## Installation
+### Installation
 
 To install `git-llm`, you need to have Python 3.9 and an OpenAI API
-key [api-keys](https://platform.openai.com/account/api-keys).
-Additionally, if you want to use the GPT4All model, you need to download
-the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model. If you prefer a
-different model, you can download it from [GPT4All](https://gpt4all.io) and configure path to it in the configuration
-and specify its
-path in the configuration. If you want some files to be ignored, add them to .gitignore.
+key [api-keys](https://platform.openai.com/account/api-keys). Additionally, if you want to use the GPT4All model, you
+need to download the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model.
+If you prefer a different model, you can download it from [GPT4All](https://gpt4all.io) and configure path to it in the
+configuration and specify its path in the configuration. If you want some files to be ignored, add them to .gitignore.
 
 To install `git-llm`, run the following command in your terminal:
 
 ```bash
 pip install git-llm
 ```
 
-Once `git-llm` is installed, you can run it from the command line:
+### Usage
+
+To use `git-llm`, you need to configure it first. To do this, run the following command:
+
+```bash
+git-llm config
+```
+
+`changelog` - generates a list of changes from output `git diff --staged`
+
+```bash
+git-llm changelog
+```
+
+This command reviews the changes staged for commit using `git diff --staged` and writes a commit message following the
+Conventional format.
 
 ```bash
-talk-codebase config
+git-llm commit
 ```
 
-You can also edit the configuration manually by editing the `~/.git_llm_config.yaml` file.
-If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
-the path to the configuration file.
+You can also edit the configuration manually by editing the `~/.git_llm_config.yaml` file. If for some reason you cannot
+find the configuration file, just run the tool and at the very beginning it will output the path to the configuration
+file.
 
 ```yaml
 # The OpenAI API key. You can get it from https://beta.openai.com/account/api-keys
 api_key: sk-xxx
 # maximum size of a chunk of text to be sent to the model
 chunk_size: 500
 # the maximum tokens
@@ -47,14 +55,14 @@
 model_name: gpt-3.5-turbo
 # model path for the local model
 model_path: models/ggml-gpt4all-j-v1.3-groovy.bin
 # model type: openai or local
 model_type: openai
 ```
 
-## Features
+### Features
 
 More commands will be added in the future.
 
-## Contributing
+### Contributing
 
 Contributions are always welcome!
```

### Comparing `git_llm-0.1.0/pyproject.toml` & `git_llm-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "git-llm"
-version = "0.1.0"
+version = "0.1.2"
 description = "The project integrates Git with a llm (OpenAI, LlamaCpp, and GPT-4-All) to extend the capabilities of git."
 authors = ["Saryev Rustam <rsaryev1997@gmail.com>"]
 readme = "README.md"
 keywords = ["chatgpt", "openai", "cli"]
-packages = [{ include = "src" }]
+packages = [{ include = "git_llm" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 gitpython = "^3.1.31"
 langchain = "^0.0.184"
 halo = "^0.0.31"
 fire = "^0.5.0"
@@ -26,8 +26,8 @@
 "Bug Tracker" = "https://github.com/rsaryev/git-llm/issues"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-git-llm = "src.cli:main"
+git-llm = "git_llm.cli:main"
```

### Comparing `git_llm-0.1.0/src/cli.py` & `git_llm-0.1.2/git_llm/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,52 @@
 import fire
 import questionary
 
-from .gitutils import git
-from .llm import factory_llm
-from .prompt import c_changelog_prompt, m_changelog_prompt
-from .utils import get_config, DEFAULT_CONFIG, save_config
+from git_llm.llm import factory_llm
+from git_llm.prompt import c_changelog_prompt, m_changelog_prompt, m_commit_prompt, c_commit_prompt
+from git_llm.utils.git import git
+from git_llm.utils.helpers import get_config, DEFAULT_CONFIG, save_config
+
+
+def check_for_changes():
+    diff = git.git_diff()
+    if not diff:
+        print("🤖 No changes found try git add .")
+        exit(0)
+    return diff
+
+
+def summarize_docs(llm, docs, message_prompt, changelog_prompt):
+    summary = llm.summarize_docs(docs, message_prompt, changelog_prompt)
+    print(f"\n{summary}")
+    return summary
 
 
 def changelog():
     config = get_config()
     llm = factory_llm(config)
 
-    diff = git.git_diff()
-    if not diff:
-        raise Exception("No changes found")
+    diff = check_for_changes()
     docs = llm.text_splitter(diff)
-    git_changelog_message = llm.summarize_docs(docs, m_changelog_prompt, c_changelog_prompt)
-    print(f"\n{git_changelog_message}")
+    summarize_docs(llm, docs, m_changelog_prompt, c_changelog_prompt)
+
+
+def commit():
+    config = get_config()
+    llm = factory_llm(config)
+
+    diff = check_for_changes()
+    docs = llm.text_splitter(diff)
+
+    summary = summarize_docs(llm, docs, m_commit_prompt, c_commit_prompt)
+    ask = questionary.confirm(f"🤖 Do you want to commit with message: {summary}?").ask()
+    if not ask:
+        print("🤖 Bye!")
+        exit(0)
+    git.git_commit(summary)
 
 
 def configure():
     config = get_config()
     model_type = questionary.select(
         "🤖 Select model type:",
         choices=[
@@ -43,14 +69,15 @@
 
 
 def main():
     try:
         fire.Fire({
             "changelog": changelog,
             "config": configure,
+            "commit": commit,
         })
     except KeyboardInterrupt:
         print("\n🤖 Bye!")
     except Exception as e:
         if str(e) == "<empty message>":
             print("🤖 Please configure your API key. Use talk-codebase configure")
         else:
```

### Comparing `git_llm-0.1.0/src/gitutils.py` & `git_llm-0.1.2/git_llm/utils/git.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,9 +14,12 @@
     def has_repository(self):
         return self.repo.bare is False
 
     def git_diff(self):
         allowed_extensions = [f"*{ext}" for ext in ALLOW_FILES]
         return self.repo.git.diff("--staged", "--diff-filter=ACMRT", "--", *allowed_extensions)
 
+    def git_commit(self, message):
+        return self.repo.git.commit("-m", message)
+
 
 git = Git()
```

### Comparing `git_llm-0.1.0/src/llm.py` & `git_llm-0.1.2/git_llm/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         raise NotImplementedError("Subclasses must implement this method.")
 
     @Halo(text='Summarizing', spinner='dots')
     def summarize_docs(self, docs, m_prompt, c_prompt):
         summarize_chain = load_summarize_chain(self.llm,
                                                chain_type="map_reduce",
                                                combine_prompt=c_prompt,
-                                               map_prompt=m_prompt, verbose=True)
+                                               map_prompt=m_prompt)
         return summarize_chain.run(docs)
 
     def text_splitter(self, text):
         texts = RecursiveCharacterTextSplitter(chunk_size=int(self.config.get("chunk_size")),
                                                chunk_overlap=int(self.config.get("chunk_overlap"))
                                                ).split_text(text)
         docs = [Document(page_content=t) for t in texts]
```

### Comparing `git_llm-0.1.0/src/utils.py` & `git_llm-0.1.2/git_llm/utils/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def save_config(config):
     print(f"🤖 Saving config to {config_path}")
     with open(config_path, "w") as f:
         yaml.dump(config, f)
 
 
 def get_config():
-    print(f"🤖 Loading config from {config_path}")
+    print(f"🤖 Loaded config from {config_path}")
     if os.path.exists(config_path):
         with open(config_path, "r") as f:
             config = yaml.safe_load(f)
     else:
         config = DEFAULT_CONFIG
         save_config(config)
     return config
```

### Comparing `git_llm-0.1.0/PKG-INFO` & `git_llm-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-llm
-Version: 0.1.0
+Version: 0.1.2
 Summary: The project integrates Git with a llm (OpenAI, LlamaCpp, and GPT-4-All) to extend the capabilities of git.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rsaryev1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -21,49 +21,57 @@
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers (>=4.29.2,<5.0.0)
 Requires-Dist: urllib3 (==1.26.6)
 Description-Content-Type: text/markdown
 
 ## git-llm
 
-The project integrates Git with a llm (OpenAI, LlamaCpp, and GPT-4-All) to extend the capabilities of git.
+The project integrates Git with a llm (OpenAI, LlamaCpp, and GPT-4-All) to extend the capabilities of git. It supports
+offline processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third parties, or
+you can use OpenAI if privacy is not a concern for you. It is only recommended for educational purposes and not for
+production use.
 
-## Description
-
-git-llm is a tool that allows you to generate changelog entries, and other things using OpenAI, LlamaCpp, and GPT-4-All.
-It supports
-offline processing using [GPT4All](https://github.com/nomic-ai/gpt4all) without sharing your code with third
-parties, or you can use OpenAI if privacy is not a concern for you. It is only recommended for educational purposes and
-not for production use.
-
-## Installation
+### Installation
 
 To install `git-llm`, you need to have Python 3.9 and an OpenAI API
-key [api-keys](https://platform.openai.com/account/api-keys).
-Additionally, if you want to use the GPT4All model, you need to download
-the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model. If you prefer a
-different model, you can download it from [GPT4All](https://gpt4all.io) and configure path to it in the configuration
-and specify its
-path in the configuration. If you want some files to be ignored, add them to .gitignore.
+key [api-keys](https://platform.openai.com/account/api-keys). Additionally, if you want to use the GPT4All model, you
+need to download the [ggml-gpt4all-j-v1.3-groovy.bin](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin) model.
+If you prefer a different model, you can download it from [GPT4All](https://gpt4all.io) and configure path to it in the
+configuration and specify its path in the configuration. If you want some files to be ignored, add them to .gitignore.
 
 To install `git-llm`, run the following command in your terminal:
 
 ```bash
 pip install git-llm
 ```
 
-Once `git-llm` is installed, you can run it from the command line:
+### Usage
+
+To use `git-llm`, you need to configure it first. To do this, run the following command:
+
+```bash
+git-llm config
+```
+
+`changelog` - generates a list of changes from output `git diff --staged`
+
+```bash
+git-llm changelog
+```
+
+This command reviews the changes staged for commit using `git diff --staged` and writes a commit message following the
+Conventional format.
 
 ```bash
-talk-codebase config
+git-llm commit
 ```
 
-You can also edit the configuration manually by editing the `~/.git_llm_config.yaml` file.
-If for some reason you cannot find the configuration file, just run the tool and at the very beginning it will output
-the path to the configuration file.
+You can also edit the configuration manually by editing the `~/.git_llm_config.yaml` file. If for some reason you cannot
+find the configuration file, just run the tool and at the very beginning it will output the path to the configuration
+file.
 
 ```yaml
 # The OpenAI API key. You can get it from https://beta.openai.com/account/api-keys
 api_key: sk-xxx
 # maximum size of a chunk of text to be sent to the model
 chunk_size: 500
 # the maximum tokens
@@ -72,14 +80,14 @@
 model_name: gpt-3.5-turbo
 # model path for the local model
 model_path: models/ggml-gpt4all-j-v1.3-groovy.bin
 # model type: openai or local
 model_type: openai
 ```
 
-## Features
+### Features
 
 More commands will be added in the future.
 
-## Contributing
+### Contributing
 
 Contributions are always welcome!
```

