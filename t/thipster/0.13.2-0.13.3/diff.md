# Comparing `tmp/thipster-0.13.2.tar.gz` & `tmp/thipster-0.13.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.13.2.tar", last modified: Tue May 30 15:43:47 2023, max compression
+gzip compressed data, was "thipster-0.13.3.tar", last modified: Wed May 31 12:15:06 2023, max compression
```

## Comparing `thipster-0.13.2.tar` & `thipster-0.13.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.025070 thipster-0.13.2/
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-30 15:43:43.000000 thipster-0.13.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-30 15:43:47.025070 thipster-0.13.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2697 2023-05-30 15:43:43.000000 thipster-0.13.2/README.md
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-30 15:43:43.000000 thipster-0.13.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-30 15:43:43.000000 thipster-0.13.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 15:43:47.025070 thipster-0.13.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1057 2023-05-30 15:43:44.000000 thipster-0.13.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.013070 thipster-0.13.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.013070 thipster-0.13.2/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3218 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.013070 thipster-0.13.2/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.013070 thipster-0.13.2/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13247 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     4008 2023-05-30 15:43:43.000000 thipster-0.13.2/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.017070 thipster-0.13.2/thipster/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.017070 thipster-0.13.2/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)     1239 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/auth/Google.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.021070 thipster-0.13.2/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)     2273 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/Engine.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/I_Auth.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/I_Parser.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/I_Repository.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/I_Terraform.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/ParsedFile.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/ResourceModel.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.021070 thipster-0.13.2/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     6169 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.021070 thipster-0.13.2/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)    10350 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/AST.py
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/DSLExceptions.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/DSLParser.py
--rw-r--r--   0 root         (0) root         (0)    13788 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/Interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17548 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/Lexer.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/LexerPosition.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/Token.py
--rw-r--r--   0 root         (0) root         (0)    19857 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/TokenParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/parser/dsl_parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.025070 thipster-0.13.2/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/repository/GithubRepo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/repository/JSONRepo.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/repository/LocalRepo.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.025070 thipster-0.13.2/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)    11680 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/terraform/CDK.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:43:43.000000 thipster-0.13.2/thipster/terraform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:43:47.017070 thipster-0.13.2/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-30 15:43:46.000000 thipster-0.13.2/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1629 2023-05-30 15:43:47.000000 thipster-0.13.2/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 15:43:46.000000 thipster-0.13.2/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      205 2023-05-30 15:43:46.000000 thipster-0.13.2/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-30 15:43:46.000000 thipster-0.13.2/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-31 12:15:04.000000 thipster-0.13.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 12:15:06.918254 thipster-0.13.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-31 12:15:04.000000 thipster-0.13.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-31 12:15:04.000000 thipster-0.13.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-31 12:15:04.000000 thipster-0.13.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 12:15:06.918254 thipster-0.13.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-05-31 12:15:04.000000 thipster-0.13.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3218 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15546 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13247 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4682 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     3773 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/thipster/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/auth/Google.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/Engine.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/I_Auth.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/I_Parser.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/I_Repository.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/I_Terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/ParsedFile.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/ResourceModel.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     6169 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)    10350 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/AST.py
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/DSLExceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/DSLParser.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/Interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/Lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/LexerPosition.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/Token.py
+-rw-r--r--   0 root         (0) root         (0)    19857 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/TokenParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/repository/GithubRepo.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/repository/JSONRepo.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/repository/LocalRepo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)    11680 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/terraform/CDK.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/terraform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.13.2/PKG-INFO` & `thipster-0.13.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.13.2
+Version: 0.13.3
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `thipster-0.13.2/README.md` & `thipster-0.13.3/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/pyproject.toml` & `thipster-0.13.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/setup.py` & `thipster-0.13.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.13.2'
+__version__ = '0.13.3'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open("README.md") as rm:
     readme = rm.read()
```

### Comparing `thipster-0.13.2/tests/engine/test_engine.py` & `thipster-0.13.3/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.13.3/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/parser/dsl_parser/test_ast.py` & `thipster-0.13.3/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.13.3/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/parser/dsl_parser/test_token.py` & `thipster-0.13.3/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.13.3/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/parser/test_ParserFactory.py` & `thipster-0.13.3/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/parser/test_YAMLParser.py` & `thipster-0.13.3/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/parser/test_parsedfile.py` & `thipster-0.13.3/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/tests/test_e2e.py` & `thipster-0.13.3/tests/test_e2e.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 import os
 import shutil
-from thipster.auth.Google import GoogleAuth
+from cdktf_cdktf_provider_google.provider import GoogleProvider
 
 from thipster.engine.Engine import Engine
+from thipster.engine.I_Auth import I_Auth
 from thipster.parser.ParserFactory import ParserFactory
 import pytest
 from thipster.repository.LocalRepo import LocalRepo
 import thipster.terraform.CDK as cdk
 
 LOCAL_REPO = 'tests/resources/e2e/models'
 REMOTE_REPO = 'THipster/models'
 
 
+class MockAuth(I_Auth):
+    def authenticate(app):
+        GoogleProvider(
+            app, "default_google",
+            project="project_id",
+            credentials="credentials.token",
+        )
+
+
 def create_dir(dirname: str, files: dict[str, str]):
     if not os.path.isdir(dirname):
         os.mkdir(dirname)
 
     dirname = os.path.abspath(dirname)
     for name, content in files.items():
         create_file(name, content, dirname)
@@ -46,15 +56,15 @@
             file,
         },
     )
 
     engine = Engine(
         ParserFactory(),
         LocalRepo(local_repo),
-        GoogleAuth,
+        MockAuth,
         cdk.CDK(),
     )
     try:
         output = engine.run(path_input)
     except Exception as e:
         raise e
     finally:
@@ -62,71 +72,48 @@
 
         if os.path.exists('cdktf.out'):
             shutil.rmtree('cdktf.out')
 
     return output
 
 
-def e2e_test(func):
-    def internal_wrapper(*args, **kwargs):
-        g = os.getenv("GOOGLE_CREDENTIALS")
-        os.environ["GOOGLE_CREDENTIALS"] = """
-{
-  "type": "service_account",
-  "project_id": "test"
-}"""
-        res = func(*args, **kwargs)
-
-        if g:
-            os.environ["GOOGLE_CREDENTIALS"] = g
-        else:
-            del os.environ["GOOGLE_CREDENTIALS"]
-
-        return res
-    return internal_wrapper
-
-
-@e2e_test
 def test_bucket():
     out = __test_file(
         file="""
 bucket my-bucket:
 \tregion : euw
     """,
     )
 
     assert isinstance(out, list)
     assert len(out) == 1
 
     assert out[0] == 'cdktf.out/stacks/thipster_infrastructure'
 
 
-@e2e_test
 def test_dep_with_no_options():
     with pytest.raises(cdk.CDKMissingAttributeInDependency):
         __test_file(
             file="""
 bucket_bad_dep_parent my-bucket:
 \tregion : euw
         """,
         )
 
 
-@e2e_test
 def test_cyclic_deps():
     with pytest.raises(cdk.CDKCyclicDependencies):
         __test_file(
             file="""
 bucket_bad_dep_cyclic my-bucket:
 \tregion : euw
         """,
         )
 
 
-@e2e_test
 def test_lb():
     out = __test_file(
         file="""
 network lb-net:
 
 subnetwork lb-subnet:
 \tregion: europe-west1b
@@ -139,15 +126,14 @@
 
     assert isinstance(out, list)
     assert len(out) == 1
 
     assert 'cdktf.out/stacks/thipster_infrastructure' in out
 
 
-@e2e_test
 def test_lb_single_file():
     out = __test_file(
         file="""
 network lb-net:
 
 subnetwork lb-subnet:
 \tregion: europe-west1b
@@ -160,15 +146,14 @@
 
     assert isinstance(out, list)
     assert len(out) == 1
 
     assert 'cdktf.out/stacks/thipster_infrastructure' in out
 
 
-@e2e_test
 def test_internal_object():
     out = __test_file(
         file="""
 firewall testParent:
 \tdirection: EGRESS
         """,
     )
@@ -182,15 +167,14 @@
 \tallow:
 \t\tprotocol: http
         """,
     )
     assert 'cdktf.out/stacks/thipster_infrastructure' in out
 
 
-@e2e_test
 def test_bucket_cors():
     out = __test_file(
         file="""
 bucket corsBucket:
     cors:
         origin:
             - "http://image-store.com"
```

### Comparing `thipster-0.13.2/thipster/engine/Engine.py` & `thipster-0.13.3/thipster/engine/Engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/engine/I_Parser.py` & `thipster-0.13.3/thipster/engine/I_Parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/engine/I_Terraform.py` & `thipster-0.13.3/thipster/engine/I_Terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/engine/ParsedFile.py` & `thipster-0.13.3/thipster/engine/ParsedFile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/engine/ResourceModel.py` & `thipster-0.13.3/thipster/engine/ResourceModel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/ParserFactory.py` & `thipster-0.13.3/thipster/parser/ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/YAMLParser.py` & `thipster-0.13.3/thipster/parser/YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/dsl_parser/AST.py` & `thipster-0.13.3/thipster/parser/dsl_parser/AST.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/dsl_parser/DSLParser.py` & `thipster-0.13.3/thipster/parser/dsl_parser/DSLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/dsl_parser/Interpreter.py` & `thipster-0.13.3/thipster/parser/dsl_parser/Interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/dsl_parser/Lexer.py` & `thipster-0.13.3/thipster/parser/dsl_parser/Lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/dsl_parser/LexerPosition.py` & `thipster-0.13.3/thipster/parser/dsl_parser/LexerPosition.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/dsl_parser/Token.py` & `thipster-0.13.3/thipster/parser/dsl_parser/Token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/parser/dsl_parser/TokenParser.py` & `thipster-0.13.3/thipster/parser/dsl_parser/TokenParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/repository/GithubRepo.py` & `thipster-0.13.3/thipster/repository/GithubRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/repository/JSONRepo.py` & `thipster-0.13.3/thipster/repository/JSONRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster/terraform/CDK.py` & `thipster-0.13.3/thipster/terraform/CDK.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.2/thipster.egg-info/PKG-INFO` & `thipster-0.13.3/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.13.2
+Version: 0.13.3
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `thipster-0.13.2/thipster.egg-info/SOURCES.txt` & `thipster-0.13.3/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

