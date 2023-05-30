# Comparing `tmp/git_llm-0.1.2.tar.gz` & `tmp/git_llm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_llm-0.1.2.tar", max compression
+gzip compressed data, was "git_llm-0.1.3.tar", max compression
```

## Comparing `git_llm-0.1.2.tar` & `git_llm-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-30 22:27:54.731972 git_llm-0.1.2/LICENSE
--rw-r--r--   0        0        0     2221 2023-05-30 22:27:54.731972 git_llm-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/__init__.py
--rw-r--r--   0        0        0     2433 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/cli.py
--rw-r--r--   0        0        0     2497 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/llm.py
--rw-r--r--   0        0        0      852 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/prompt.py
--rw-r--r--   0        0        0        0 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/utils/__init__.py
--rw-r--r--   0        0        0      832 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/utils/git.py
--rw-r--r--   0        0        0      819 2023-05-30 22:27:54.735972 git_llm-0.1.2/git_llm/utils/helpers.py
--rw-r--r--   0        0        0      848 2023-05-30 22:27:54.735972 git_llm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 git_llm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 23:28:51.848699 git_llm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2221 2023-05-30 23:28:51.848699 git_llm-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 23:28:51.848699 git_llm-0.1.3/git_llm/__init__.py
+-rw-r--r--   0        0        0     2267 2023-05-30 23:28:51.848699 git_llm-0.1.3/git_llm/cli.py
+-rw-r--r--   0        0        0     2497 2023-05-30 23:28:51.848699 git_llm-0.1.3/git_llm/llm.py
+-rw-r--r--   0        0        0     1121 2023-05-30 23:28:51.848699 git_llm-0.1.3/git_llm/prompt.py
+-rw-r--r--   0        0        0        0 2023-05-30 23:28:51.848699 git_llm-0.1.3/git_llm/utils/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-30 23:28:51.848699 git_llm-0.1.3/git_llm/utils/git.py
+-rw-r--r--   0        0        0      819 2023-05-30 23:28:51.848699 git_llm-0.1.3/git_llm/utils/helpers.py
+-rw-r--r--   0        0        0      848 2023-05-30 23:28:51.852699 git_llm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 git_llm-0.1.3/PKG-INFO
```

### Comparing `git_llm-0.1.2/LICENSE` & `git_llm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `git_llm-0.1.2/README.md` & `git_llm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `git_llm-0.1.2/git_llm/cli.py` & `git_llm-0.1.3/git_llm/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,37 +11,32 @@
     diff = git.git_diff()
     if not diff:
         print("🤖 No changes found try git add .")
         exit(0)
     return diff
 
 
-def summarize_docs(llm, docs, message_prompt, changelog_prompt):
-    summary = llm.summarize_docs(docs, message_prompt, changelog_prompt)
-    print(f"\n{summary}")
-    return summary
-
-
 def changelog():
     config = get_config()
     llm = factory_llm(config)
 
     diff = check_for_changes()
     docs = llm.text_splitter(diff)
-    summarize_docs(llm, docs, m_changelog_prompt, c_changelog_prompt)
+    log = llm.summarize_docs(docs, m_changelog_prompt, c_changelog_prompt)
+    print(log)
 
 
 def commit():
     config = get_config()
     llm = factory_llm(config)
 
     diff = check_for_changes()
     docs = llm.text_splitter(diff)
 
-    summary = summarize_docs(llm, docs, m_commit_prompt, c_commit_prompt)
+    summary = llm.summarize_docs(docs, m_commit_prompt, c_commit_prompt)
     ask = questionary.confirm(f"🤖 Do you want to commit with message: {summary}?").ask()
     if not ask:
         print("🤖 Bye!")
         exit(0)
     git.git_commit(summary)
```

### Comparing `git_llm-0.1.2/git_llm/llm.py` & `git_llm-0.1.3/git_llm/llm.py`

 * *Files identical despite different names*

### Comparing `git_llm-0.1.2/git_llm/utils/git.py` & `git_llm-0.1.3/git_llm/utils/git.py`

 * *Files identical despite different names*

### Comparing `git_llm-0.1.2/git_llm/utils/helpers.py` & `git_llm-0.1.3/git_llm/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `git_llm-0.1.2/pyproject.toml` & `git_llm-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-llm"
-version = "0.1.2"
+version = "0.1.3"
 description = "The project integrates Git with a llm (OpenAI, LlamaCpp, and GPT-4-All) to extend the capabilities of git."
 authors = ["Saryev Rustam <rsaryev1997@gmail.com>"]
 readme = "README.md"
 keywords = ["chatgpt", "openai", "cli"]
 packages = [{ include = "git_llm" }]
 
 [tool.poetry.dependencies]
```

### Comparing `git_llm-0.1.2/PKG-INFO` & `git_llm-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-llm
-Version: 0.1.2
+Version: 0.1.3
 Summary: The project integrates Git with a llm (OpenAI, LlamaCpp, and GPT-4-All) to extend the capabilities of git.
 Keywords: chatgpt,openai,cli
 Author: Saryev Rustam
 Author-email: rsaryev1997@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

