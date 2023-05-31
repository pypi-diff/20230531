# Comparing `tmp/rekono-cli-2.0.0.tar.gz` & `tmp/rekono-cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rekono-cli-2.0.0.tar", last modified: Sun May  7 11:50:31 2023, max compression
+gzip compressed data, was "dist/rekono-cli-2.0.1.tar", last modified: Wed May 31 16:56:54 2023, max compression
```

## Comparing `rekono-cli-2.0.0.tar` & `rekono-cli-2.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/client/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/authentications.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/findings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/target_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/commands/wordlists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/framework/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono/framework/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/commands/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/framework/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/rekono/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/rekono_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 11:50:31.000000 rekono-cli-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-07 11:50:20.000000 rekono-cli-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/findings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/target_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/commands/wordlists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/framework/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono/framework/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/framework/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/framework/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/framework/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/framework/commands/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/framework/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/rekono/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/rekono_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:56:54.000000 rekono-cli-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-31 16:56:41.000000 rekono-cli-2.0.1/setup.py
```

### Comparing `rekono-cli-2.0.0/PKG-INFO` & `rekono-cli-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: rekono-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: CLI to make requests to Rekono API
 Home-page: https://github.com/pablosnt/rekono-cli
 Author: Pablo Santiago López
 License: UNKNOWN
 Project-URL: Rekono, https://github.com/pablosnt/rekono
 Project-URL: Rekono CLI, https://github.com/pablosnt/rekono-cli
 Description: <p align="center">
+          <a href="https://github.com/pablosnt/rekono-cli/actions/workflows/unit-testing.yml" alt="Unit testing"  target="_blank">
+            <img src="https://github.com/pablosnt/rekono-cli/actions/workflows/unit-testing.yml/badge.svg"/>
+          </a>
+          <a href="https://github.com/pablosnt/rekono-cli/actions/workflows/security-sast.yml" alt="SAST"  target="_blank">
+            <img src="https://github.com/pablosnt/rekono-cli/actions/workflows/security-sast.yml/badge.svg"/>
+          </a>
           <a href="https://snyk.io/test/github/pablosnt/rekono-cli" alt="SCA" target="_blank">
-            <img src="https://badgen.net/snyk/pablosnt/rekono-cli?label=Vulnerabilities&labelColor=black&icon=https://snyk.io/wp-content/uploads/patch-white.svg">
+            <img src="https://badgen.net/snyk/pablosnt/rekono-cli?label=SCA&labelColor=black&icon=https://snyk.io/wp-content/uploads/patch-white.svg"/>
           </a>
           <a href="https://github.com/pablosnt/rekono-cli/actions/workflows/security-secrets.yml" alt="Secrets scanning" target="_blank">
             <img src="https://github.com/pablosnt/rekono-cli/actions/workflows/security-secrets.yml/badge.svg"/>
           </a>
           <a href="https://github.com/pablosnt/rekono-cli/actions/workflows/code-style.yml" alt="Code style" target="_blank">
             <img src="https://github.com/pablosnt/rekono-cli/actions/workflows/code-style.yml/badge.svg"/>
           </a>
@@ -56,16 +62,15 @@
         
         ```bash
         pip3 install rekono-cli
         ```
         
         ### From Source
         
-        1. Install the required technologies:
-            - Python 3 & PIP
+        1. Install the required technologies: Python 3 & PIP
         
         2. Install the dependencies:
         
             ```bash
             pip3 install -r src/requirements.txt
             ```
```

#### html2text {}

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 2.1 Name: rekono-cli Version: 2.0.0 Summary: CLI to make
+Metadata-Version: 2.1 Name: rekono-cli Version: 2.0.1 Summary: CLI to make
 requests to Rekono API Home-page: https://github.com/pablosnt/rekono-cli
 Author: Pablo Santiago LÃ³pez License: UNKNOWN Project-URL: Rekono, https://
 github.com/pablosnt/rekono Project-URL: Rekono CLI, https://github.com/
 pablosnt/rekono-cli Description:
-                   [https://badgen.net/snyk/pablosnt/rekono-
-  cli?label=Vulnerabilities&labelColor=black&icon=https://snyk.io/wp-content/
-   uploads/patch-white.svg] [https://github.com/pablosnt/rekono-cli/actions/
-workflows/security-secrets.yml/badge.svg] [https://github.com/pablosnt/rekono-
-cli/actions/workflows/code-style.yml/badge.svg] [https://img.shields.io/badge/
-     Discord-Join-black?style=social&logo=discord] [https://ko-fi.com/img/
-                    githubbutton_sm.svg] [Buy_Me_A_Coffee]
+  [https://github.com/pablosnt/rekono-cli/actions/workflows/unit-testing.yml/
+badge.svg] [https://github.com/pablosnt/rekono-cli/actions/workflows/security-
+         sast.yml/badge.svg] [https://badgen.net/snyk/pablosnt/rekono-
+ cli?label=SCA&labelColor=black&icon=https://snyk.io/wp-content/uploads/patch-
+white.svg] [https://github.com/pablosnt/rekono-cli/actions/workflows/security-
+    secrets.yml/badge.svg] [https://github.com/pablosnt/rekono-cli/actions/
+workflows/code-style.yml/badge.svg] [https://img.shields.io/badge/Discord-Join-
+ black?style=social&logo=discord] [https://ko-fi.com/img/githubbutton_sm.svg]
+                               [Buy_Me_A_Coffee]
 #
 [https://raw.githubusercontent.com/pablosnt/rekono/main/rekono/frontend/public/
                             static/logo-black.png]
 Command Line Interface to make requests to the [Rekono](https://github.com/
 pablosnt/rekono) API REST. ## Usage [usage] > Rekono API documentation is
 available in `/api/schema/swagger-ui.html` and `/api/schema/redoc/` of Rekono
 instances ## Library usage Rekono CLI can be also used as Python 3 library, so
 that it's possible to create custom Rekono scripts. For example, with the
 following code it's possible to create a Rekono client to make custom API
 requests: ```python from rekono.client.api import Rekono client = Rekono
 (url='https://127.0.0.1', token='my secret api token') # Create Rekono client
 response = client.get('/api/tools/1/') # GET request to get tool with ID 1 ```
 ## Installation ### PIP ```bash pip3 install rekono-cli ``` ### From Source 1.
-Install the required technologies: - Python 3 & PIP 2. Install the
-dependencies: ```bash pip3 install -r src/requirements.txt ``` 3. Execute the
-CLI: ```bash python3 src/rekono/main.py --help ``` ## Configuration You can use
-the `REKONO_TOKEN` environment variable to configure the API token for Rekono
+Install the required technologies: Python 3 & PIP 2. Install the dependencies:
+```bash pip3 install -r src/requirements.txt ``` 3. Execute the CLI: ```bash
+python3 src/rekono/main.py --help ``` ## Configuration You can use the
+`REKONO_TOKEN` environment variable to configure the API token for Rekono
 authentication. ## Reach Us You can get support, ask questions, solve doubts or
 solve problems using:
 [https://github.com/fluidicon.png] [https://assets-global.website-files.com/
 6257adef93867e50d84d30e2/636e0a69f118df70ad7828d4_icon_clyde_blurple_RGB.svg]
 [https://www.gstatic.com/images/branding/product/2x/gmail_2020q4_512dp.png]
 Rekono is an open source project that we really love to maintain and it's
 absolutely our pleasure, but we would like to offer the possibility of
```

### Comparing `rekono-cli-2.0.0/rekono/client/api.py` & `rekono-cli-2.0.1/rekono/client/api.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/client/enums.py` & `rekono-cli-2.0.1/rekono/client/enums.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/client/exceptions.py` & `rekono-cli-2.0.1/rekono/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/authentications.py` & `rekono-cli-2.0.1/rekono/commands/authentications.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/configurations.py` & `rekono-cli-2.0.1/rekono/commands/configurations.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/executions.py` & `rekono-cli-2.0.1/rekono/commands/executions.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/findings.py` & `rekono-cli-2.0.1/rekono/commands/findings.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/processes.py` & `rekono-cli-2.0.1/rekono/commands/processes.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/profile.py` & `rekono-cli-2.0.1/rekono/commands/profile.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/projects.py` & `rekono-cli-2.0.1/rekono/commands/projects.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/settings.py` & `rekono-cli-2.0.1/rekono/commands/settings.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/steps.py` & `rekono-cli-2.0.1/rekono/commands/steps.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/target_ports.py` & `rekono-cli-2.0.1/rekono/commands/target_ports.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/targets.py` & `rekono-cli-2.0.1/rekono/commands/targets.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/tasks.py` & `rekono-cli-2.0.1/rekono/commands/tasks.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/tools.py` & `rekono-cli-2.0.1/rekono/commands/tools.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/users.py` & `rekono-cli-2.0.1/rekono/commands/users.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/commands/wordlists.py` & `rekono-cli-2.0.1/rekono/commands/wordlists.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/framework/commands/api.py` & `rekono-cli-2.0.1/rekono/framework/commands/api.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/framework/commands/command.py` & `rekono-cli-2.0.1/rekono/framework/commands/command.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/framework/commands/entity.py` & `rekono-cli-2.0.1/rekono/framework/commands/entity.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/framework/options.py` & `rekono-cli-2.0.1/rekono/framework/options.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono/main.py` & `rekono-cli-2.0.1/rekono/main.py`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/rekono_cli.egg-info/PKG-INFO` & `rekono-cli-2.0.1/rekono_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: rekono-cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: CLI to make requests to Rekono API
 Home-page: https://github.com/pablosnt/rekono-cli
 Author: Pablo Santiago López
 License: UNKNOWN
 Project-URL: Rekono, https://github.com/pablosnt/rekono
 Project-URL: Rekono CLI, https://github.com/pablosnt/rekono-cli
 Description: <p align="center">
+          <a href="https://github.com/pablosnt/rekono-cli/actions/workflows/unit-testing.yml" alt="Unit testing"  target="_blank">
+            <img src="https://github.com/pablosnt/rekono-cli/actions/workflows/unit-testing.yml/badge.svg"/>
+          </a>
+          <a href="https://github.com/pablosnt/rekono-cli/actions/workflows/security-sast.yml" alt="SAST"  target="_blank">
+            <img src="https://github.com/pablosnt/rekono-cli/actions/workflows/security-sast.yml/badge.svg"/>
+          </a>
           <a href="https://snyk.io/test/github/pablosnt/rekono-cli" alt="SCA" target="_blank">
-            <img src="https://badgen.net/snyk/pablosnt/rekono-cli?label=Vulnerabilities&labelColor=black&icon=https://snyk.io/wp-content/uploads/patch-white.svg">
+            <img src="https://badgen.net/snyk/pablosnt/rekono-cli?label=SCA&labelColor=black&icon=https://snyk.io/wp-content/uploads/patch-white.svg"/>
           </a>
           <a href="https://github.com/pablosnt/rekono-cli/actions/workflows/security-secrets.yml" alt="Secrets scanning" target="_blank">
             <img src="https://github.com/pablosnt/rekono-cli/actions/workflows/security-secrets.yml/badge.svg"/>
           </a>
           <a href="https://github.com/pablosnt/rekono-cli/actions/workflows/code-style.yml" alt="Code style" target="_blank">
             <img src="https://github.com/pablosnt/rekono-cli/actions/workflows/code-style.yml/badge.svg"/>
           </a>
@@ -56,16 +62,15 @@
         
         ```bash
         pip3 install rekono-cli
         ```
         
         ### From Source
         
-        1. Install the required technologies:
-            - Python 3 & PIP
+        1. Install the required technologies: Python 3 & PIP
         
         2. Install the dependencies:
         
             ```bash
             pip3 install -r src/requirements.txt
             ```
```

#### html2text {}

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 2.1 Name: rekono-cli Version: 2.0.0 Summary: CLI to make
+Metadata-Version: 2.1 Name: rekono-cli Version: 2.0.1 Summary: CLI to make
 requests to Rekono API Home-page: https://github.com/pablosnt/rekono-cli
 Author: Pablo Santiago LÃ³pez License: UNKNOWN Project-URL: Rekono, https://
 github.com/pablosnt/rekono Project-URL: Rekono CLI, https://github.com/
 pablosnt/rekono-cli Description:
-                   [https://badgen.net/snyk/pablosnt/rekono-
-  cli?label=Vulnerabilities&labelColor=black&icon=https://snyk.io/wp-content/
-   uploads/patch-white.svg] [https://github.com/pablosnt/rekono-cli/actions/
-workflows/security-secrets.yml/badge.svg] [https://github.com/pablosnt/rekono-
-cli/actions/workflows/code-style.yml/badge.svg] [https://img.shields.io/badge/
-     Discord-Join-black?style=social&logo=discord] [https://ko-fi.com/img/
-                    githubbutton_sm.svg] [Buy_Me_A_Coffee]
+  [https://github.com/pablosnt/rekono-cli/actions/workflows/unit-testing.yml/
+badge.svg] [https://github.com/pablosnt/rekono-cli/actions/workflows/security-
+         sast.yml/badge.svg] [https://badgen.net/snyk/pablosnt/rekono-
+ cli?label=SCA&labelColor=black&icon=https://snyk.io/wp-content/uploads/patch-
+white.svg] [https://github.com/pablosnt/rekono-cli/actions/workflows/security-
+    secrets.yml/badge.svg] [https://github.com/pablosnt/rekono-cli/actions/
+workflows/code-style.yml/badge.svg] [https://img.shields.io/badge/Discord-Join-
+ black?style=social&logo=discord] [https://ko-fi.com/img/githubbutton_sm.svg]
+                               [Buy_Me_A_Coffee]
 #
 [https://raw.githubusercontent.com/pablosnt/rekono/main/rekono/frontend/public/
                             static/logo-black.png]
 Command Line Interface to make requests to the [Rekono](https://github.com/
 pablosnt/rekono) API REST. ## Usage [usage] > Rekono API documentation is
 available in `/api/schema/swagger-ui.html` and `/api/schema/redoc/` of Rekono
 instances ## Library usage Rekono CLI can be also used as Python 3 library, so
 that it's possible to create custom Rekono scripts. For example, with the
 following code it's possible to create a Rekono client to make custom API
 requests: ```python from rekono.client.api import Rekono client = Rekono
 (url='https://127.0.0.1', token='my secret api token') # Create Rekono client
 response = client.get('/api/tools/1/') # GET request to get tool with ID 1 ```
 ## Installation ### PIP ```bash pip3 install rekono-cli ``` ### From Source 1.
-Install the required technologies: - Python 3 & PIP 2. Install the
-dependencies: ```bash pip3 install -r src/requirements.txt ``` 3. Execute the
-CLI: ```bash python3 src/rekono/main.py --help ``` ## Configuration You can use
-the `REKONO_TOKEN` environment variable to configure the API token for Rekono
+Install the required technologies: Python 3 & PIP 2. Install the dependencies:
+```bash pip3 install -r src/requirements.txt ``` 3. Execute the CLI: ```bash
+python3 src/rekono/main.py --help ``` ## Configuration You can use the
+`REKONO_TOKEN` environment variable to configure the API token for Rekono
 authentication. ## Reach Us You can get support, ask questions, solve doubts or
 solve problems using:
 [https://github.com/fluidicon.png] [https://assets-global.website-files.com/
 6257adef93867e50d84d30e2/636e0a69f118df70ad7828d4_icon_clyde_blurple_RGB.svg]
 [https://www.gstatic.com/images/branding/product/2x/gmail_2020q4_512dp.png]
 Rekono is an open source project that we really love to maintain and it's
 absolutely our pleasure, but we would like to offer the possibility of
```

### Comparing `rekono-cli-2.0.0/rekono_cli.egg-info/SOURCES.txt` & `rekono-cli-2.0.1/rekono_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rekono-cli-2.0.0/setup.py` & `rekono-cli-2.0.1/setup.py`

 * *Files identical despite different names*

