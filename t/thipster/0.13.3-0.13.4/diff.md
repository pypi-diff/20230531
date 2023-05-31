# Comparing `tmp/thipster-0.13.3.tar.gz` & `tmp/thipster-0.13.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.13.3.tar", last modified: Wed May 31 12:15:06 2023, max compression
+gzip compressed data, was "thipster-0.13.4.tar", last modified: Wed May 31 12:48:10 2023, max compression
```

## Comparing `thipster-0.13.3.tar` & `thipster-0.13.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-31 12:15:04.000000 thipster-0.13.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 12:15:06.918254 thipster-0.13.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2697 2023-05-31 12:15:04.000000 thipster-0.13.3/README.md
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-31 12:15:04.000000 thipster-0.13.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-31 12:15:04.000000 thipster-0.13.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 12:15:06.918254 thipster-0.13.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1057 2023-05-31 12:15:04.000000 thipster-0.13.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3218 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13247 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     3773 2023-05-31 12:15:04.000000 thipster-0.13.3/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.914255 thipster-0.13.3/thipster/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      799 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/auth/Google.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)     2273 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/Engine.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/I_Auth.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/I_Parser.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/I_Repository.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/I_Terraform.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/ParsedFile.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/ResourceModel.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     6169 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)    10350 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/AST.py
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/DSLExceptions.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/DSLParser.py
--rw-r--r--   0 root         (0) root         (0)    13788 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/Interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17548 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/Lexer.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/LexerPosition.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/Token.py
--rw-r--r--   0 root         (0) root         (0)    19857 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/TokenParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/parser/dsl_parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/repository/GithubRepo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/repository/JSONRepo.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/repository/LocalRepo.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)    11680 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/terraform/CDK.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:15:04.000000 thipster-0.13.3/thipster/terraform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:15:06.918254 thipster-0.13.3/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1629 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      225 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 12:15:06.000000 thipster-0.13.3/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.012261 thipster-0.13.4/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-31 12:48:07.000000 thipster-0.13.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 12:48:10.012261 thipster-0.13.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-31 12:48:07.000000 thipster-0.13.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-31 12:48:07.000000 thipster-0.13.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-31 12:48:07.000000 thipster-0.13.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 12:48:10.012261 thipster-0.13.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-05-31 12:48:08.000000 thipster-0.13.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.004261 thipster-0.13.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.004261 thipster-0.13.4/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3218 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.004261 thipster-0.13.4/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.004261 thipster-0.13.4/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15546 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13247 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4682 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-05-31 12:48:07.000000 thipster-0.13.4/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.004261 thipster-0.13.4/thipster/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.004261 thipster-0.13.4/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/auth/Google.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.008261 thipster-0.13.4/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/engine/Engine.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/engine/I_Auth.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/engine/I_Parser.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/engine/I_Repository.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/engine/I_Terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/engine/ParsedFile.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/engine/ResourceModel.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.008261 thipster-0.13.4/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     6169 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.008261 thipster-0.13.4/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)    10350 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/AST.py
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/DSLExceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/DSLParser.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/Interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/Lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/LexerPosition.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/Token.py
+-rw-r--r--   0 root         (0) root         (0)    20153 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/TokenParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/parser/dsl_parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.008261 thipster-0.13.4/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/repository/GithubRepo.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/repository/JSONRepo.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/repository/LocalRepo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.012261 thipster-0.13.4/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)    11680 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/terraform/CDK.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:48:07.000000 thipster-0.13.4/thipster/terraform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:48:10.004261 thipster-0.13.4/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 12:48:09.000000 thipster-0.13.4/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-05-31 12:48:09.000000 thipster-0.13.4/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:48:09.000000 thipster-0.13.4/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-31 12:48:09.000000 thipster-0.13.4/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 12:48:09.000000 thipster-0.13.4/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.13.3/PKG-INFO` & `thipster-0.13.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.13.3
+Version: 0.13.4
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `thipster-0.13.3/README.md` & `thipster-0.13.4/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/pyproject.toml` & `thipster-0.13.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/setup.py` & `thipster-0.13.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.13.3'
+__version__ = '0.13.4'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open("README.md") as rm:
     readme = rm.read()
```

### Comparing `thipster-0.13.3/tests/engine/test_engine.py` & `thipster-0.13.4/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.13.4/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/parser/dsl_parser/test_ast.py` & `thipster-0.13.4/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.13.4/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/parser/dsl_parser/test_token.py` & `thipster-0.13.4/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.13.4/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/parser/test_ParserFactory.py` & `thipster-0.13.4/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/parser/test_YAMLParser.py` & `thipster-0.13.4/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/parser/test_parsedfile.py` & `thipster-0.13.4/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/tests/test_e2e.py` & `thipster-0.13.4/tests/test_e2e.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,14 +86,42 @@
 
     assert isinstance(out, list)
     assert len(out) == 1
 
     assert out[0] == 'cdktf.out/stacks/thipster_infrastructure'
 
 
+def test_empty_bucket():
+    out = __test_file(
+        file="""
+bucket dzvhvzarbazkhr:
+
+    """,
+    )
+
+    assert isinstance(out, list)
+    assert len(out) == 1
+
+    assert out[0] == 'cdktf.out/stacks/thipster_infrastructure'
+
+    out = __test_file(
+        file="""
+bucket dzvhvzarbazkhr:
+
+bucket ezezeaz:
+    region: europe
+    """,
+    )
+
+    assert isinstance(out, list)
+    assert len(out) == 1
+
+    assert out[0] == 'cdktf.out/stacks/thipster_infrastructure'
+
+
 def test_dep_with_no_options():
     with pytest.raises(cdk.CDKMissingAttributeInDependency):
         __test_file(
             file="""
 bucket_bad_dep_parent my-bucket:
 \tregion : euw
         """,
```

### Comparing `thipster-0.13.3/thipster/auth/Google.py` & `thipster-0.13.4/thipster/auth/Google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/engine/Engine.py` & `thipster-0.13.4/thipster/engine/Engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/engine/I_Parser.py` & `thipster-0.13.4/thipster/engine/I_Parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/engine/I_Terraform.py` & `thipster-0.13.4/thipster/engine/I_Terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/engine/ParsedFile.py` & `thipster-0.13.4/thipster/engine/ParsedFile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/engine/ResourceModel.py` & `thipster-0.13.4/thipster/engine/ResourceModel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/ParserFactory.py` & `thipster-0.13.4/thipster/parser/ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/YAMLParser.py` & `thipster-0.13.4/thipster/parser/YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/dsl_parser/AST.py` & `thipster-0.13.4/thipster/parser/dsl_parser/AST.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/dsl_parser/DSLParser.py` & `thipster-0.13.4/thipster/parser/dsl_parser/DSLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/dsl_parser/Interpreter.py` & `thipster-0.13.4/thipster/parser/dsl_parser/Interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/dsl_parser/Lexer.py` & `thipster-0.13.4/thipster/parser/dsl_parser/Lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/dsl_parser/LexerPosition.py` & `thipster-0.13.4/thipster/parser/dsl_parser/LexerPosition.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/dsl_parser/Token.py` & `thipster-0.13.4/thipster/parser/dsl_parser/Token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/parser/dsl_parser/TokenParser.py` & `thipster-0.13.4/thipster/parser/dsl_parser/TokenParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,27 +231,37 @@
 
         return parameter
 
     def __get_properties(self, indent: int) -> list[ast.ParameterNode]:
         """(list | dict)
         """
         i = indent
-        next = self.__get_next_type(indent)
-        while next == TT.WHITESPACE:
-            i += 1
-            next = self.__get_next_type(i)
+        try:
+            next = self.__get_next_type(indent)
+            while next == TT.WHITESPACE:
+                i += 1
+                next = self.__get_next_type(i)
 
-        if next == TT.STRING:
-            props = self.__get_dict(indent)
+            if next == TT.STRING:
+                props = self.__get_dict(indent)
 
-        elif next == TT.MINUS:
-            props = self.__get_list(indent)
+            elif next == TT.MINUS:
+                props = self.__get_list(indent)
 
-        else:
-            raise DSLSyntaxException(self.__next(), TT.TAB)
+            else:
+                raise DSLSyntaxException(self.__next(), TT.TAB)
+
+        except DSLUnexpectedEOF as eof:
+            if indent > 1:
+                raise DSLUnexpectedEOF from eof
+
+            if eof.__cause__:
+                raise DSLUnexpectedEOF from eof.__cause__
+
+            props = ast.DictNode([])
 
         return props
 
     def __get_list(self, indent: int) -> ast.ListNode:
         """{ "-", value, [amt_ctrl], [if_else_ctrl], "\\n"}"""
         items = []
```

### Comparing `thipster-0.13.3/thipster/repository/GithubRepo.py` & `thipster-0.13.4/thipster/repository/GithubRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/repository/JSONRepo.py` & `thipster-0.13.4/thipster/repository/JSONRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster/terraform/CDK.py` & `thipster-0.13.4/thipster/terraform/CDK.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.3/thipster.egg-info/PKG-INFO` & `thipster-0.13.4/thipster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.13.3
+Version: 0.13.4
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `thipster-0.13.3/thipster.egg-info/SOURCES.txt` & `thipster-0.13.4/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

