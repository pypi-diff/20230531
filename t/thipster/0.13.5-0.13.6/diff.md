# Comparing `tmp/thipster-0.13.5.tar.gz` & `tmp/thipster-0.13.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.13.5.tar", last modified: Wed May 31 13:14:48 2023, max compression
+gzip compressed data, was "thipster-0.13.6.tar", last modified: Wed May 31 13:17:02 2023, max compression
```

## Comparing `thipster-0.13.5.tar` & `thipster-0.13.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.447918 thipster-0.13.5/
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-31 13:14:45.000000 thipster-0.13.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 13:14:48.443918 thipster-0.13.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2697 2023-05-31 13:14:45.000000 thipster-0.13.5/README.md
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-31 13:14:45.000000 thipster-0.13.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      137 2023-05-31 13:14:45.000000 thipster-0.13.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 13:14:48.447918 thipster-0.13.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1057 2023-05-31 13:14:46.000000 thipster-0.13.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.435918 thipster-0.13.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.435918 thipster-0.13.5/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3226 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.439918 thipster-0.13.5/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.439918 thipster-0.13.5/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13247 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     4290 2023-05-31 13:14:45.000000 thipster-0.13.5/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.439918 thipster-0.13.5/thipster/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.439918 thipster-0.13.5/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      799 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/auth/Google.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.443918 thipster-0.13.5/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)     3472 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/engine/Engine.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/engine/I_Auth.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/engine/I_Parser.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/engine/I_Repository.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/engine/I_Terraform.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/engine/ParsedFile.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/engine/ResourceModel.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.443918 thipster-0.13.5/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     6169 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.443918 thipster-0.13.5/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)    10350 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/AST.py
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/DSLExceptions.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/DSLParser.py
--rw-r--r--   0 root         (0) root         (0)    13788 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/Interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17548 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/Lexer.py
--rw-r--r--   0 root         (0) root         (0)     4770 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/LexerPosition.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/Token.py
--rw-r--r--   0 root         (0) root         (0)    20153 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/TokenParser.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/parser/dsl_parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.443918 thipster-0.13.5/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/repository/GithubRepo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/repository/JSONRepo.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/repository/LocalRepo.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.443918 thipster-0.13.5/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)    11680 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/terraform/CDK.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:14:45.000000 thipster-0.13.5/thipster/terraform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:14:48.439918 thipster-0.13.5/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 13:14:48.000000 thipster-0.13.5/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1629 2023-05-31 13:14:48.000000 thipster-0.13.5/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 13:14:48.000000 thipster-0.13.5/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      225 2023-05-31 13:14:48.000000 thipster-0.13.5/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 13:14:48.000000 thipster-0.13.5/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.670935 thipster-0.13.6/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-31 13:17:00.000000 thipster-0.13.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 13:17:02.670935 thipster-0.13.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-31 13:17:00.000000 thipster-0.13.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-31 13:17:00.000000 thipster-0.13.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-31 13:17:00.000000 thipster-0.13.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 13:17:02.670935 thipster-0.13.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-05-31 13:17:00.000000 thipster-0.13.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15546 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13247 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4682 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2023-05-31 13:17:00.000000 thipster-0.13.6/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/thipster/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      799 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/auth/Google.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.666935 thipster-0.13.6/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)     3472 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/Engine.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/I_Auth.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/I_Parser.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/I_Repository.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/I_Terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/ParsedFile.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/ResourceModel.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.666935 thipster-0.13.6/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.666935 thipster-0.13.6/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)    10350 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/AST.py
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/DSLExceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/DSLParser.py
+-rw-r--r--   0 root         (0) root         (0)    13788 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/Interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/Lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/LexerPosition.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/Token.py
+-rw-r--r--   0 root         (0) root         (0)    20153 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/TokenParser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/parser/dsl_parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.670935 thipster-0.13.6/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/repository/GithubRepo.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/repository/JSONRepo.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/repository/LocalRepo.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.670935 thipster-0.13.6/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)    11680 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/terraform/CDK.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:17:00.000000 thipster-0.13.6/thipster/terraform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:17:02.662935 thipster-0.13.6/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      225 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-31 13:17:02.000000 thipster-0.13.6/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.13.5/PKG-INFO` & `thipster-0.13.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.13.5
+Version: 0.13.6
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `thipster-0.13.5/README.md` & `thipster-0.13.6/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/pyproject.toml` & `thipster-0.13.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/setup.py` & `thipster-0.13.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.13.5'
+__version__ = '0.13.6'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open("README.md") as rm:
     readme = rm.read()
```

### Comparing `thipster-0.13.5/tests/engine/test_engine.py` & `thipster-0.13.6/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.13.6/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/tests/parser/dsl_parser/test_ast.py` & `thipster-0.13.6/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.13.6/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/tests/parser/dsl_parser/test_token.py` & `thipster-0.13.6/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.13.6/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/tests/parser/test_ParserFactory.py` & `thipster-0.13.6/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/tests/parser/test_YAMLParser.py` & `thipster-0.13.6/tests/parser/test_YAMLParser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from thipster.engine.ParsedFile import ParsedDict, ParsedFile, ParsedList, ParsedLiteral
+import thipster.engine.ParsedFile as pf
 from thipster.parser.YAMLParser import YAMLParser, YAMLParserNoName
 import os
 import pytest
 
 
 def __test_parser_raises(mocker, input: str, exception: Exception)\
         -> pytest.ExceptionInfo:
@@ -50,15 +50,15 @@
         },
     )
 
     parser = YAMLParser
     try:
         output = parser.run(path_input)
 
-        assert type(output) == ParsedFile
+        assert isinstance(output, pf.ParsedFile)
     except Exception as e:
         raise e
     finally:
         _destroy_dir()
 
     return output
 
@@ -75,15 +75,15 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'my-bucket'
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'region'
-    assert type(region._ParsedAttribute__value) == ParsedLiteral
+    assert isinstance(region._ParsedAttribute__value, pf.ParsedLiteral)
     assert region.value == 'euw'
 
 
 def test_parse_simple_jinja_file():
     out = __test_file(
         file="""
 {% set name = "test_name" %}
@@ -98,15 +98,15 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'test_name'
     assert len(bucket.attributes) == 1
 
     region = bucket.attributes[0]
     assert region.name == 'region'
-    assert type(region._ParsedAttribute__value) == ParsedLiteral
+    assert isinstance(region._ParsedAttribute__value, pf.ParsedLiteral)
     assert region.value == 'europe-west1'
 
 
 def test_parse_two_resources():
     out = __test_file(
         file="""bucket:
   - name: my-bucket1
@@ -145,15 +145,15 @@
 
     region = bucket.attributes[0]
     assert region.name == 'region'
     assert region.value == 'euw'
 
     toto = bucket.attributes[1]
     assert toto.name == 'toto'
-    assert type(toto._ParsedAttribute__value) == ParsedDict
+    assert isinstance(toto._ParsedAttribute__value, pf.ParsedDict)
 
 
 def test_parse_list():
     out = __test_file(
         file="""bucket:
   name: my-bucket
   toto:
@@ -166,17 +166,50 @@
     bucket = out.resources[0]
     assert bucket.type == 'bucket'
     assert bucket.name == 'my-bucket'
     assert len(bucket.attributes) == 1
 
     toto = bucket.attributes[0]
     assert toto.name == 'toto'
-    assert type(toto._ParsedAttribute__value) == ParsedList
+    assert isinstance(toto._ParsedAttribute__value, pf.ParsedList)
     assert len(toto.value) == 2
 
+    for val in toto.value:
+        assert isinstance(val, pf.ParsedLiteral)
+
+
+def test_parse_dict_in_list():
+    out = __test_file(
+        file="""bucket:
+  name: my-bucket
+  toto:
+    - aaa : 12
+      bbb : OK
+    - ccc : 10
+      ddd : OK
+""",
+    )
+    assert len(out.resources) == 1
+
+    bucket = out.resources[0]
+    assert bucket.type == 'bucket'
+    assert bucket.name == 'my-bucket'
+    assert len(bucket.attributes) == 1
+
+    toto = bucket.attributes[0]
+    assert toto.name == 'toto'
+    assert isinstance(toto._ParsedAttribute__value, pf.ParsedList)
+    assert len(toto.value) == 2
+
+    for val in toto.value:
+        assert isinstance(val, pf.ParsedDict)
+        assert len(val.value) == 2
+        for v in val.value:
+            assert isinstance(v, pf.ParsedAttribute)
+
 
 def test_syntax_error_no_name(mocker):
     input = """bucket:
   toto:
     - aaa
     - bbb
 """
```

### Comparing `thipster-0.13.5/tests/parser/test_parsedfile.py` & `thipster-0.13.6/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/tests/test_e2e.py` & `thipster-0.13.6/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/auth/Google.py` & `thipster-0.13.6/thipster/auth/Google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/engine/Engine.py` & `thipster-0.13.6/thipster/engine/Engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/engine/I_Parser.py` & `thipster-0.13.6/thipster/engine/I_Parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/engine/I_Terraform.py` & `thipster-0.13.6/thipster/engine/I_Terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/engine/ParsedFile.py` & `thipster-0.13.6/thipster/engine/ParsedFile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/engine/ResourceModel.py` & `thipster-0.13.6/thipster/engine/ResourceModel.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/parser/ParserFactory.py` & `thipster-0.13.6/thipster/parser/ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/parser/YAMLParser.py` & `thipster-0.13.6/thipster/parser/YAMLParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,10 +229,13 @@
         -------
         ParsedList
             Converted list
         """
         attr = []
 
         for val in input:
-            attr.append(pf.ParsedList(val))
+            if isinstance(val, dict):
+                attr.append(YAMLParser.__get_dict(val))
+            else:
+                attr.append(pf.ParsedLiteral(val))
 
         return pf.ParsedList(attr)
```

### Comparing `thipster-0.13.5/thipster/parser/dsl_parser/AST.py` & `thipster-0.13.6/thipster/parser/dsl_parser/AST.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/parser/dsl_parser/DSLParser.py` & `thipster-0.13.6/thipster/parser/dsl_parser/DSLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/parser/dsl_parser/Interpreter.py` & `thipster-0.13.6/thipster/parser/dsl_parser/Interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/parser/dsl_parser/Lexer.py` & `thipster-0.13.6/thipster/parser/dsl_parser/Lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/parser/dsl_parser/LexerPosition.py` & `thipster-0.13.6/thipster/parser/dsl_parser/LexerPosition.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/parser/dsl_parser/Token.py` & `thipster-0.13.6/thipster/parser/dsl_parser/Token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/parser/dsl_parser/TokenParser.py` & `thipster-0.13.6/thipster/parser/dsl_parser/TokenParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/repository/GithubRepo.py` & `thipster-0.13.6/thipster/repository/GithubRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/repository/JSONRepo.py` & `thipster-0.13.6/thipster/repository/JSONRepo.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster/terraform/CDK.py` & `thipster-0.13.6/thipster/terraform/CDK.py`

 * *Files identical despite different names*

### Comparing `thipster-0.13.5/thipster.egg-info/PKG-INFO` & `thipster-0.13.6/thipster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.13.5
+Version: 0.13.6
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
```

### Comparing `thipster-0.13.5/thipster.egg-info/SOURCES.txt` & `thipster-0.13.6/thipster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

