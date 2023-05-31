# Comparing `tmp/sparrow-patterns-0.6.0.dev1685568389.tar.gz` & `tmp/sparrow-patterns-0.6.0.dev1685568436.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrow-patterns-0.6.0.dev1685568389.tar", last modified: Wed May 31 21:26:41 2023, max compression
+gzip compressed data, was "sparrow-patterns-0.6.0.dev1685568436.tar", last modified: Wed May 31 21:27:28 2023, max compression
```

## Comparing `sparrow-patterns-0.6.0.dev1685568389.tar` & `sparrow-patterns-0.6.0.dev1685568436.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.877608 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.877608 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dependencies/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.877608 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dependencies/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dependencies/templates/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dependencies/templates/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.877608 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/devcontainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/devcontainer/devcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/devcontainer/devcontainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.877608 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/devcontainer/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/devcontainer/templates/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dockerfile/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dockerfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dockerfile/dockerfile_.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dockerfile/dockerfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dockerfile/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dockerfile/templates/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/github/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/github/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/github/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/github/templates/build.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/gitignore/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/gitignore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/gitignore/gitignore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/gitignore/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/gitignore/templates/gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/makefile/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/makefile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/makefile/makefile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/makefile/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/makefile/templates/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/notebooks/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/readme/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/readme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/readme/readme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/readme/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/readme/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.881609 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/vscode/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/vscode/templates/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-31 21:26:00.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/vscode/vscode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:26:41.877608 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 21:26:41.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-31 21:26:41.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:26:41.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 21:26:41.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 21:26:41.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 21:26:41.000000 sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.175961 sparrow-patterns-0.6.0.dev1685568436/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 21:27:28.175961 sparrow-patterns-0.6.0.dev1685568436/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-31 21:27:28.175961 sparrow-patterns-0.6.0.dev1685568436/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dependencies/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dependencies/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dependencies/templates/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dependencies/templates/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/devcontainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/devcontainer/devcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/devcontainer/devcontainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/devcontainer/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/devcontainer/templates/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dockerfile/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dockerfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dockerfile/dockerfile_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dockerfile/dockerfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dockerfile/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dockerfile/templates/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/github/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/github/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/github/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/github/templates/build.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/gitignore/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/gitignore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/gitignore/gitignore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/gitignore/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/gitignore/templates/gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/makefile/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/makefile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/makefile/makefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/makefile/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/makefile/templates/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/notebooks/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.175961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/readme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/readme/readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.175961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/readme/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/readme/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.175961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.175961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/vscode/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/vscode/templates/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-31 21:26:44.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/vscode/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:27:28.171961 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 21:27:28.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-31 21:27:28.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:27:28.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 21:27:28.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 21:27:28.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 21:27:28.000000 sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns.egg-info/top_level.txt
```

### Comparing `sparrow-patterns-0.6.0.dev1685568389/LICENSE` & `sparrow-patterns-0.6.0.dev1685568436/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/setup.cfg` & `sparrow-patterns-0.6.0.dev1685568436/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sparrow-patterns
-version = 0.6.0.dev1685568389
+version = 0.6.0.dev1685568436
 description = A CLI for updating code patterns in Python projects
 author = Sparrow Computing
 author_email = ben@sparrow.dev
 license = MIT
 
 [options]
 install_requires =
```

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/__main__.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/__main__.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dependencies/dependencies.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dependencies/dependencies.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dependencies/templates/setup.cfg` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dependencies/templates/setup.cfg`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/devcontainer/devcontainer.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/devcontainer/devcontainer.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/devcontainer/templates/devcontainer.json` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/devcontainer/templates/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                 "ms-python.python",
                 "ms-python.vscode-pylance",
             ],            
         }
     },
     "mounts": [
         "source=projectname-bashhistory,target=/commandhistory,type=volume",
+        "source=${localEnv:HOME}/.ssh,target=/home/${localEnv:USER}/.ssh,type=bind,consistency=cached",
     ],
     "workspaceFolder": "/code",
     "workspaceMount": "source=${localWorkspaceFolder},target=/code,type=bind,consistency=cached",
     "runArgs": [
         "--ipc=host",{% if gpu %}
         "--gpus=all",{% endif %}
         // "--env-file=.env"
```

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dockerfile/dockerfile_.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dockerfile/dockerfile_.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/dockerfile/templates/Dockerfile` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/dockerfile/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/github/github.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/github/github.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/github/templates/build.yml` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/github/templates/build.yml`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/gitignore/gitignore.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/gitignore/gitignore.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/gitignore/templates/gitignore` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/gitignore/templates/gitignore`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/makefile/makefile.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/makefile/makefile.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/makefile/templates/Makefile` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/makefile/templates/Makefile`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/notebooks/notebooks.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/project.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/project.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/readme/readme.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/readme/readme.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/vscode/templates/launch.json` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/vscode/templates/launch.json`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns/vscode/vscode.py` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns/vscode/vscode.py`

 * *Files identical despite different names*

### Comparing `sparrow-patterns-0.6.0.dev1685568389/sparrow_patterns.egg-info/SOURCES.txt` & `sparrow-patterns-0.6.0.dev1685568436/sparrow_patterns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

