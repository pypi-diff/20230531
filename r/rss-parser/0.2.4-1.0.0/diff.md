# Comparing `tmp/rss-parser-0.2.4.tar.gz` & `tmp/rss_parser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rss-parser-0.2.4.tar", max compression
+gzip compressed data, was "rss_parser-1.0.0.tar", max compression
```

## Comparing `rss-parser-0.2.4.tar` & `rss_parser-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,16 @@
--rw-r--r--   0        0        0    35151 2022-06-07 13:16:40.659480 rss-parser-0.2.4/LICENSE
--rw-r--r--   0        0        0     2192 2022-06-07 13:16:40.659480 rss-parser-0.2.4/README.md
--rw-r--r--   0        0        0     1835 2022-06-07 13:16:40.659480 rss-parser-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       28 2022-06-07 13:16:40.659480 rss-parser-0.2.4/rss_parser/__init__.py
--rw-r--r--   0        0        0     5540 2022-06-07 13:16:40.659480 rss-parser-0.2.4/rss_parser/_parser.py
--rw-r--r--   0        0        0     1223 2022-06-07 13:16:40.659480 rss-parser-0.2.4/rss_parser/models.py
--rw-r--r--   0        0        0     2941 2022-06-07 13:17:30.479355 rss-parser-0.2.4/setup.py
--rw-r--r--   0        0        0     3554 2022-06-07 13:17:30.479635 rss-parser-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35151 2023-05-31 18:08:42.610093 rss_parser-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5717 2023-05-31 18:08:42.610093 rss_parser-1.0.0/README.md
+-rw-r--r--   0        0        0     2378 2023-05-31 18:08:42.610093 rss_parser-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/__init__.py
+-rw-r--r--   0        0        0     1158 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/_parser.py
+-rw-r--r--   0        0        0      885 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/__init__.py
+-rw-r--r--   0        0        0     4854 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/channel.py
+-rw-r--r--   0        0        0     1074 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/image.py
+-rw-r--r--   0        0        0     1475 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/item.py
+-rw-r--r--   0        0        0      321 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/rss.py
+-rw-r--r--   0        0        0      751 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/text_input.py
+-rw-r--r--   0        0        0       99 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/types/__init__.py
+-rw-r--r--   0        0        0      934 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/types/date.py
+-rw-r--r--   0        0        0     4666 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/types/tag.py
+-rw-r--r--   0        0        0      140 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/utils.py
+-rw-r--r--   0        0        0     7076 1970-01-01 00:00:00.000000 rss_parser-1.0.0/PKG-INFO
```

### Comparing `rss-parser-0.2.4/LICENSE` & `rss_parser-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rss-parser-0.2.4/pyproject.toml` & `rss_parser-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "rss-parser"
-version = "0.2.4"
+version = "1.0.0"
 description = "Typed pythonic RSS parser"
 authors = ["dhvcc <1337kwiz@gmail.com>"]
-license = "GPLv3"
+license = "GPL-3.0"
 readme = "README.md"
 keywords = [
     "python",
     "python3",
     "cli",
     "rss",
     "parser",
-    "scraper",
     "gplv3",
     "typed",
     "typed-python",
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
@@ -25,57 +24,75 @@
     "Topic :: Text Processing :: Markup :: XML",
     "Typing :: Typed",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
+packages = [{include = "rss_parser"}]
+
 
 [tool.poetry.urls]
 "Homepage" = "https://dhvcc.github.io/rss-parser"
 "Source" = "https://github.com/dhvcc/rss-parser"
 "Bug Tracker" = "https://github.com/dhvcc/rss-parser/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-bs4 = ">=0.0.1"
+python = "^3.8"
 pydantic = ">=1.6.1"
-lxml = ">=4.6.5"
-requests = ">=2.24.0"
 pytest = "^7.1.2"
+xmltodict = "^0.13.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+ipython = "*"
 black = "^22.3.0"
 pre-commit = "^2.12.0"
-flake8 = "^4.0.1"
-isort = "^5.8.0"
-flake8-docstrings = "^1.6.0"
+ruff = "*"
+rich = "*"
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.pytest.ini_options]
+addopts = "-color=yes"
 
 [tool.black]
-line-length = 88
-target-version = ['py37', 'py38', 'py39', 'py310']
-exclude = '''
-(
-    \.eggs
-  | \.git
-  | build
-  | dist
-  | venv
-  | .venv
-)
-'''
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-line_length = 88
-skip_gitignore = true
-skip_glob = ['**/.venv/**']
+line-length = 120
+target-version = ["py38"]
+
+[tool.ruff]
+line-length = 120
+target-version = "py38"
+respect-gitignore = true
+select = [
+    "PL",    # pylint
+    "F",     # pyflakes
+    "E",     # pycodestyle errors
+    "W",     # pycodestyle warnings
+    "I",     # isort
+    "N",     # pep8-naming
+    "S",     # flake8-bandit
+    "A",     # flake8-builtins
+    "C40",   # flake8-comprehensions
+    "T10",   # flake8-debugger
+    "EXE",   # flake8-executable
+    "T20",   # flake8-print
+    "TID",   # flake8-tidy-imports
+    "TCH",   # flake8-type-checking
+    "ARG",   # flake8-unused-arguments
+    "RUF",   # ruff
+]
+
+[tool.ruff.per-file-ignores]
+"tests/**.py" = [
+  "S101",    # Use of assert detected
+  "ARG001",  # Unused function argument
+  "S311",    # Allow use of random
+]
+"**/__init__.py" = [
+    "F401"
+]
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

