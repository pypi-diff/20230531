# Comparing `tmp/logedit-0.1.0.tar.gz` & `tmp/logedit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logedit-0.1.0.tar", last modified: Mon May 29 04:24:12 2023, max compression
+gzip compressed data, was "logedit-0.1.1.tar", last modified: Wed May 31 19:06:46 2023, max compression
```

## Comparing `logedit-0.1.0.tar` & `logedit-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-29 04:24:12.826684 logedit-0.1.0/
--rw-r--r--   0 gpriday    (501) staff       (20)     3119 2023-05-29 04:24:12.826568 logedit-0.1.0/PKG-INFO
--rw-r--r--   0 gpriday    (501) staff       (20)     2737 2023-05-28 20:02:57.000000 logedit-0.1.0/README.md
-drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-29 04:24:12.826400 logedit-0.1.0/logedit.egg-info/
--rw-r--r--   0 gpriday    (501) staff       (20)     3119 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/PKG-INFO
--rw-r--r--   0 gpriday    (501) staff       (20)      206 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/SOURCES.txt
--rw-r--r--   0 gpriday    (501) staff       (20)        1 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/dependency_links.txt
--rw-r--r--   0 gpriday    (501) staff       (20)       55 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/entry_points.txt
--rw-r--r--   0 gpriday    (501) staff       (20)       78 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/requires.txt
--rw-r--r--   0 gpriday    (501) staff       (20)        1 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/top_level.txt
--rw-r--r--   0 gpriday    (501) staff       (20)       38 2023-05-29 04:24:12.826722 logedit-0.1.0/setup.cfg
--rw-r--r--   0 gpriday    (501) staff       (20)      877 2023-05-29 04:22:06.000000 logedit-0.1.0/setup.py
+drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-31 19:06:46.747558 logedit-0.1.1/
+-rw-r--r--   0 gpriday    (501) staff       (20)       51 2023-05-31 18:59:12.000000 logedit-0.1.1/MANIFEST.in
+-rw-r--r--   0 gpriday    (501) staff       (20)     3169 2023-05-31 19:06:46.747298 logedit-0.1.1/PKG-INFO
+-rw-r--r--   0 gpriday    (501) staff       (20)     2787 2023-05-29 04:33:57.000000 logedit-0.1.1/README.md
+drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-31 19:06:46.745676 logedit-0.1.1/logedit/
+-rw-r--r--   0 gpriday    (501) staff       (20)        0 2023-05-31 18:52:20.000000 logedit-0.1.1/logedit/__init__.py
+-rwxr-xr-x   0 gpriday    (501) staff       (20)     8032 2023-05-29 05:51:41.000000 logedit-0.1.1/logedit/logedit.py
+-rw-r--r--   0 gpriday    (501) staff       (20)     1050 2023-05-28 21:41:29.000000 logedit-0.1.1/logedit/messages.json
+drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-31 19:06:46.746970 logedit-0.1.1/logedit/system/
+-rw-r--r--   0 gpriday    (501) staff       (20)      703 2023-05-28 18:56:42.000000 logedit-0.1.1/logedit/system/changelog_writer.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)      312 2023-05-29 05:38:59.000000 logedit-0.1.1/logedit/system/commit_summarizer.txt
+drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-31 19:06:46.746570 logedit-0.1.1/logedit.egg-info/
+-rw-r--r--   0 gpriday    (501) staff       (20)     3169 2023-05-31 19:06:46.000000 logedit-0.1.1/logedit.egg-info/PKG-INFO
+-rw-r--r--   0 gpriday    (501) staff       (20)      352 2023-05-31 19:06:46.000000 logedit-0.1.1/logedit.egg-info/SOURCES.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)        1 2023-05-31 19:06:46.000000 logedit-0.1.1/logedit.egg-info/dependency_links.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)       55 2023-05-31 19:06:46.000000 logedit-0.1.1/logedit.egg-info/entry_points.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)       95 2023-05-31 19:06:46.000000 logedit-0.1.1/logedit.egg-info/requires.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)        8 2023-05-31 19:06:46.000000 logedit-0.1.1/logedit.egg-info/top_level.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)       38 2023-05-31 19:06:46.747650 logedit-0.1.1/setup.cfg
+-rw-r--r--   0 gpriday    (501) staff       (20)      928 2023-05-31 19:05:43.000000 logedit-0.1.1/setup.py
```

### Comparing `logedit-0.1.0/PKG-INFO` & `logedit-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logedit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to auto-generate changelogs from git commits using OpenAI's APIs
 Home-page: https://github.com/gregpriday/logedit/
 Author: Greg Priday
 Author-email: greg@siteorigin.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -65,14 +65,18 @@
 
 Logedit retrieves all commits between the old and new versions specified. It then uses OpenAI's GPT-4 (or GPT-3.5 Turbo, if specified) to summarize each commit. 
 
 Next, it feeds the tail of your current `CHANGELOG.md` file, the new version (or its best guess if not specified or "HEAD" is provided), and the commit summaries to the selected AI model and generates a changelog entry in the same format as your existing `CHANGELOG.md`.
 
 If the `--append` option is used, the new entry is automatically added to your changelog file.
 
+## Change Log
+
+See [CHANGELOG.md](CHANGELOG.md).
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
```

### Comparing `logedit-0.1.0/README.md` & `logedit-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,18 @@
 
 Logedit retrieves all commits between the old and new versions specified. It then uses OpenAI's GPT-4 (or GPT-3.5 Turbo, if specified) to summarize each commit. 
 
 Next, it feeds the tail of your current `CHANGELOG.md` file, the new version (or its best guess if not specified or "HEAD" is provided), and the commit summaries to the selected AI model and generates a changelog entry in the same format as your existing `CHANGELOG.md`.
 
 If the `--append` option is used, the new entry is automatically added to your changelog file.
 
+## Change Log
+
+See [CHANGELOG.md](CHANGELOG.md).
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
```

### Comparing `logedit-0.1.0/logedit.egg-info/PKG-INFO` & `logedit-0.1.1/logedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logedit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to auto-generate changelogs from git commits using OpenAI's APIs
 Home-page: https://github.com/gregpriday/logedit/
 Author: Greg Priday
 Author-email: greg@siteorigin.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -65,14 +65,18 @@
 
 Logedit retrieves all commits between the old and new versions specified. It then uses OpenAI's GPT-4 (or GPT-3.5 Turbo, if specified) to summarize each commit. 
 
 Next, it feeds the tail of your current `CHANGELOG.md` file, the new version (or its best guess if not specified or "HEAD" is provided), and the commit summaries to the selected AI model and generates a changelog entry in the same format as your existing `CHANGELOG.md`.
 
 If the `--append` option is used, the new entry is automatically added to your changelog file.
 
+## Change Log
+
+See [CHANGELOG.md](CHANGELOG.md).
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## License
```

### Comparing `logedit-0.1.0/setup.py` & `logedit-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
-requirements = ["gitpython>=3.1.14", "tqdm>=4.60.0", "openai>=0.27.0", "backoff>=1.10.0", "tiktoken>=0.4.0"]
+requirements = ["gitpython>=3.1.14", "tqdm>=4.60.0", "openai>=0.27.0", "backoff>=1.10.0", "tiktoken>=0.4.0", "termcolor>=2.3.0"]
 
 setup(
     name="logedit",
-    version="0.1.0",
+    version="0.1.1",
     author="Greg Priday",
     author_email="greg@siteorigin.com",
     description="A package to auto-generate changelogs from git commits using OpenAI's APIs",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/gregpriday/logedit/",
     packages=find_packages(),
     install_requires=requirements,
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: MIT License",
     ],
     entry_points={
         "console_scripts": [
             "logedit=logedit.logedit:entrypoint",
```

