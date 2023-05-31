# Comparing `tmp/dls-servbase-1.4.1.tar.gz` & `tmp/dls-servbase-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-servbase-1.4.1.tar", last modified: Mon May 29 14:11:43 2023, max compression
+gzip compressed data, was "dls-servbase-1.5.0.tar", last modified: Wed May 31 15:41:59 2023, max compression
```

## Comparing `dls-servbase-1.4.1.tar` & `dls-servbase-1.5.0.tar`

### file list

```diff
@@ -1,138 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.166787 dls-servbase-1.4.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.174787 dls-servbase-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.166787 dls-servbase-1.4.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/good_config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.170787 dls-servbase-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/src/dls_servbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.178787 dls-servbase-1.4.1/src/dls_servbase_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 14:11:43.000000 dls-servbase-1.4.1/src/dls_servbase_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    29692 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.182787 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/contexts/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/cookies/dataface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/guis/html/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.186787 dls-servbase-1.4.1/src/dls_servbase_lib/guis/html/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/guis/html/javascript/version.js
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/src/dls_servbase_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:11:43.190787 dls-servbase-1.4.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/configurations/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/configurations/sqlite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_dataface_takeover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-29 14:11:30.000000 dls-servbase-1.4.1/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.664093 dls-servbase-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.648093 dls-servbase-1.5.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.648093 dls-servbase-1.5.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.652094 dls-servbase-1.5.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/good_config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:41:59.664093 dls-servbase-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.648093 dls-servbase-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/start_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 15:41:59.000000 dls-servbase-1.5.0/src/dls_servbase_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.656093 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/contexts/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/cookie_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/cookies/dataface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/guis/html/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/src/dls_servbase_lib/guis/html/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/guis/html/javascript/version.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/src/dls_servbase_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:41:59.660093 dls-servbase-1.5.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/configurations/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/configurations/sqlite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_dataface_takeover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 15:41:49.000000 dls-servbase-1.5.0/tests/test_parse_cookie.py
```

### Comparing `dls-servbase-1.4.1/.dae-devops/Makefile` & `dls-servbase-1.5.0/.dae-devops/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 # ---------------------------------------------------------------------
 # These make targets are designed to be called from the command line and from .gitlab-ci.yml.
 # ---------------------------------------------------------------------
 
 # I put the package_pip artifacts int this place for now until I can use the corporate internal pipserver.
@@ -65,8 +65,8 @@
 	cp -v -p dist/*.whl $(PIP_FIND_LINKS)
 
 publish_docs:
 	mkdir -p $(DOCS_PUBLISH_ROOT)
 	cp -r build/html/* $(DOCS_PUBLISH_ROOT)
 	
 
-# dae_devops_fingerprint 7a40fdc6afce4991715aeda7ae70c444
+# dae_devops_fingerprint 2d453caef2662f6d4cfd06d459312f02
```

### Comparing `dls-servbase-1.4.1/.dae-devops/docs/conventions.rst` & `dls-servbase-1.5.0/.dae-devops/docs/conventions.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.3.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-servbase
 
 Naming conventions
 =======================================================================
 
 Here are the naming conventions used within the source code.
 
@@ -27,8 +27,8 @@
 python packages
     lowercase, underscores
 
 repository
     lowercase, hyphens
 
 
-.. # dae_devops_fingerprint cbd0a78343b6577aa4ddb9d59a242b04
+.. # dae_devops_fingerprint 377aec0d2a3859ddaaadcf7d54438742
```

### Comparing `dls-servbase-1.4.1/.dae-devops/docs/developing.rst` & `dls-servbase-1.5.0/.dae-devops/docs/developing.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.3.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-servbase
 
 Developing
 =======================================================================
 
 If you plan to make change to the code in this repository, you can use the steps below.
 
 Clone the repository::
 
+    $ cd <your development area>
     $ git clone https://gitlab.diamond.ac.uk/kbp43231/dls-servbase.git
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software.
-Make sure to have at least python version 3.9 then::
+Make sure to have at least python version 3.10 then::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 Install the package in edit mode which will also install all its dependencies::
 
     $ cd dls-servbase
-    $ pip install -e .[dev]
+    $ pip install -e .[dev,docs]
 
 Now you may begin modifying the code.
 
-|
 
-If you plan to modify the docs, you will need to::
-
-    $ pip install -e .[docs]
-
-    
-
-
-.. # dae_devops_fingerprint ac891cf352ef89b3b20d2c601dd9ddc4
+.. # dae_devops_fingerprint 0fd7e3e20b23c566fad722262ab9f97a
```

### Comparing `dls-servbase-1.4.1/.dae-devops/docs/devops.rst` & `dls-servbase-1.5.0/.dae-devops/docs/devops.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.3.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-servbase
 
 Devops
 =======================================================================
 
 In the top level of the repository there exists a configuration file called ``.dae-devops/project.yaml``.
 
@@ -40,8 +40,8 @@
 Publishing (for the Diamond intranet)::
 
     $ make -f .dae-devops/Makefile publish_pip
     $ make -f .dae-devops/Makefile publish_docs
     
 The Diamond intranet commands are not used for production. The production packaging and publishing are handled in the GitHub Actions workflows mechanism.
 
-.. # dae_devops_fingerprint 84e8a32100211cbba64804a3e5c5b337
+.. # dae_devops_fingerprint e8dff03fd491f40bda262817af6bf646
```

### Comparing `dls-servbase-1.4.1/.dae-devops/docs/docs_structure.rst` & `dls-servbase-1.5.0/.dae-devops/docs/docs_structure.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.3.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-servbase
 
 About the documentation
 -----------------------
 
   :material-regular:`format_quote;2em`
 
@@ -17,8 +17,8 @@
 They are: *tutorials*, *how-to guides*, *technical reference* and *explanation*.
 They represent four different purposes or functions, and require four different
 approaches to their creation. Understanding the implications of this will help
 improve most documentation - often immensely.
 
 `More information on this topic. <https://documentation.divio.com>`_
 
-.. # dae_devops_fingerprint 6ef08be920f12050c1c579cf6e9d4253
+.. # dae_devops_fingerprint 505d623863ca025fcddb20fe31db39d4
```

### Comparing `dls-servbase-1.4.1/.dae-devops/docs/installing.rst` & `dls-servbase-1.5.0/.dae-devops/docs/installing.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.3.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-servbase
 
 Installing
 =======================================================================
 
 
-You will need python 3.9 or later. 
+You will need python 3.10 or later. 
 
-On a Diamond Light Source internal computer, you can achieve Python 3.9 by::
+On a Diamond Light Source internal computer, you can achieve Python 3.10 by::
 
-    $ module load python/3.9
+    $ module load python/3.10
 
 You can check your version of python by typing into a terminal::
 
     $ python3 --version
 
 It is recommended that you install into a virtual environment so this
 installation will not interfere with any existing Python software::
 
     $ python3 -m venv /scratch/$USER/myvenv
     $ source /scratch/$USER/myvenv/bin/activate
     $ pip install --upgrade pip
 
 
-You can now use ``pip`` to install the library and its dependencies::
+You can now use ``pip`` to install the package and its dependencies::
 
     $ python3 -m pip install dls-servbase
 
-If you require a feature that is not currently released you can also install
+If you require a feature that is not currently released, you can also install
 from git::
 
     $ python3 -m pip install git+https://gitlab.diamond.ac.uk/kbp43231/dls-servbase.git
 
-The library should now be installed and the commandline should be available.
+The package should now be installed and the command line should be available.
 You can check the version that has been installed by typing::
 
     $ dls-servbase --version
     $ dls-servbase --version-json
 
-.. # dae_devops_fingerprint 64d7ae0dde8939e479b9c793df928d15
+.. # dae_devops_fingerprint f5c12f1646c65db4968cb1f7cc1306d0
```

### Comparing `dls-servbase-1.4.1/.dae-devops/project.yaml` & `dls-servbase-1.5.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/.devcontainer/Dockerfile` & `dls-servbase-1.5.0/.devcontainer/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 # This file is for use as a devcontainer and a runtime container
 #
 # The devcontainer should use the build target and run as root with podman
 # or docker with user namespaces.
 #
@@ -36,8 +36,8 @@
 COPY --from=build /venv/ /venv/
 ENV PATH=/venv/bin:$PATH
 
 # change this entrypoint if it is not the same as the repo
 ENTRYPOINT ["dls-servbase"]
 CMD ["--version"]
 
-# dae_devops_fingerprint 80986671f8602f6e4666f78f98141826
+# dae_devops_fingerprint 0534faa0b5641c6bf5a6865dc868c633
```

### Comparing `dls-servbase-1.4.1/.devcontainer/devcontainer.json` & `dls-servbase-1.5.0/.devcontainer/devcontainer.json`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // ********** Please don't edit this file!
-// ********** It has been generated automatically by dae_devops version 0.5.3.
+// ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 // ********** For repository_name dls-servbase
 
 // For format details, see https://containers.dev/implementors/json_reference/
 {
     "name": "Python 3 Developer Container",
     "build": {
         "dockerfile": "Dockerfile",
@@ -53,8 +53,8 @@
     // make the workspace folder the same inside and outside of the container
     "workspaceMount": "source=${localWorkspaceFolder},target=${localWorkspaceFolder},type=bind",
     "workspaceFolder": "${localWorkspaceFolder}",
     // After the container is created, install the python project in editable form
     "postCreateCommand": "pip install -e .[dev]"
 }
 
-// dae_devops_fingerprint 35358278c2556f05447815a0833301dc
+// dae_devops_fingerprint 41cc023010f4dbc2a199785da970798f
```

### Comparing `dls-servbase-1.4.1/.github/CONTRIBUTING.rst` & `dls-servbase-1.5.0/.github/CONTRIBUTING.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .. # ********** Please don't edit this file!
-.. # ********** It has been generated automatically by dae_devops version 0.5.3.
+.. # ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 .. # ********** For repository_name dls-servbase
 
 Contributing to the project
 ===========================
 
 Contributions and issues are most welcome! All issues and pull requests are
 handled through GitHub_. Also, please check for any existing issues before
@@ -34,8 +34,8 @@
 
 The `Developer Guide`_ contains information on setting up a development
 environment, running the tests and what standards the code and documentation
 should follow.
 
 .. _Developer Guide: https://diamondlightsource.github.io/dls-servbase/main/developer/how-to/contribute.html
 
-.. # dae_devops_fingerprint 0f4cbc1f77b787f03a9a4d268ed08055
+.. # dae_devops_fingerprint 5554a59e62e5009c44a967ba6a56e3ea
```

### Comparing `dls-servbase-1.4.1/.github/actions/install_requirements/action.yml` & `dls-servbase-1.5.0/.github/actions/install_requirements/action.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 name: Install requirements
 description: Run pip install with requirements and upload resulting requirements
 inputs:
   requirements_file:
     description: Name of requirements file to use and upload
@@ -57,8 +57,8 @@
             echo "Error: ${{ inputs.requirements_file }} need the above changes to be exhaustive"
             exit 1
           fi
         fi
       shell: bash
 
 
-# dae_devops_fingerprint 492458ca501cde9a298a80a102ff22a4
+# dae_devops_fingerprint 967212425bc2c65a1fcab3e8aaacd538
```

### Comparing `dls-servbase-1.4.1/.github/dependabot.yml` & `dls-servbase-1.5.0/.github/dependabot.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 # To get started with Dependabot version updates, you'll need to specify which
 # package ecosystems to update and where the package manifests are located.
 # Please see the documentation for all configuration options:
 # https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates
 
@@ -15,8 +15,8 @@
       interval: "weekly"
 
   - package-ecosystem: "pip"
     directory: "/"
     schedule:
       interval: "weekly"
 
-# dae_devops_fingerprint b5838c5e0d9b5041500c5cb701fb5e5b
+# dae_devops_fingerprint f3e273cc476ab516308a7a53ad8e30c6
```

### Comparing `dls-servbase-1.4.1/.github/pages/make_switcher.py` & `dls-servbase-1.5.0/.github/pages/make_switcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
@@ -98,8 +98,8 @@
     versions = get_versions("origin/gh-pages", args.add, args.remove)
     write_json(args.output, args.repository, versions)
 
 
 if __name__ == "__main__":
     main()
 
-# dae_devops_fingerprint 7a1b58b851c5198d7d380e4ab78d0b49
+# dae_devops_fingerprint b0c90a9621cff9b99133ac54ac310ade
```

### Comparing `dls-servbase-1.4.1/.github/workflows/code.yml` & `dls-servbase-1.5.0/.github/workflows/code.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 name: Code CI
 
 on:
   push:
   pull_request:
@@ -37,19 +37,14 @@
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
         python: ["3.10"]
         install: ["-e .[dev,docs]"]
-        # Make one version be non-editable to test both paths of version code
-        include:
-          - os: "ubuntu-latest"
-            python: "3.9"
-            install: ".[dev,docs]"
 
     runs-on: ${{ matrix.os }}
     env:
       # https://github.com/pytest-dev/pytest/issues/2042
       PY_IGNORE_IMPORTMISMATCH: "1"
 
     steps:
@@ -212,8 +207,8 @@
 
       - name: Publish to PyPI
         if: ${{ env.HAS_PYPI_TOKEN }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
 
-# dae_devops_fingerprint 480a147d8af93a934e6ad0fd272e60e5
+# dae_devops_fingerprint 20cc3e951a4652adfe1bdb16f0746054
```

### Comparing `dls-servbase-1.4.1/.github/workflows/docs.yml` & `dls-servbase-1.5.0/.github/workflows/docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 name: Docs CI
 
 on:
   push:
   pull_request:
@@ -52,8 +52,8 @@
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
         uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
 
-# dae_devops_fingerprint fb2dde86086783119d0b0b805151bf09
+# dae_devops_fingerprint e20397fc0e4761c7e1a235ec1ea95642
```

### Comparing `dls-servbase-1.4.1/.github/workflows/docs_clean.yml` & `dls-servbase-1.5.0/.github/workflows/docs_clean.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 name: Docs Cleanup CI
 
 # delete branch documentation when a branch is deleted
 # also allow manually deleting a documentation version
 on:
@@ -42,8 +42,8 @@
           rm -r $DOCS_VERSION
           python make_switcher.py --remove $DOCS_VERSION ${{ github.repository }} switcher.json
           git config --global user.name 'GitHub Actions Docs Cleanup CI'
           git config --global user.email 'GithubActionsCleanup@noreply.github.com'
           git commit -am "Removing redundant docs version $DOCS_VERSION"
           git push
 
-# dae_devops_fingerprint d46d59a6f5197bd11b1cece615feb4df
+# dae_devops_fingerprint 1f0958e89021d3ef04512fb059911cf4
```

### Comparing `dls-servbase-1.4.1/.gitignore` & `dls-servbase-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/.gitlab-ci.yml` & `dls-servbase-1.5.0/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 variables:
   # I put the package_pip artifacts int his place just until I can use the corporate internal pipserver.
   # Maybe /dls_sw/work/python3/RHEL7-x86_64/distributions would be a better place?
   PIP_FIND_LINKS: "/dls_sw/apps/bxflow/artifacts"
 
@@ -83,8 +83,8 @@
 
 # publish_docs:
 #   stage: publish
 #   script:
 #     # The validate_docs artifacts are in the build/html folder.
 #     - make -f .dae-devops/Makefile publish_docs
 
-# dae_devops_fingerprint 814043c19b1379f7f1d7b188546a7734
+# dae_devops_fingerprint 8c0d6830168b3a593396882beae5df6a
```

### Comparing `dls-servbase-1.4.1/.vscode/launch.json` & `dls-servbase-1.5.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/LICENSE` & `dls-servbase-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/PKG-INFO` & `dls-servbase-1.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.4.1
+Version: 1.5.0
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,60 +204,22 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://gitlab.diamond.ac.uk/kbp43231/dls-servbase
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 dls-servbase
 =======================================================================
 
 Simple HTTP service for database operations.
 
-Intended advantages:
-
-- agnostic of type of underlying sql client
-- single-connection access to database
-- hosts a few predefined common database schema
-
-Installation
------------------------------------------------------------------------
-::
-
-    pip install git+https://gitlab.diamond.ac.uk/kbp43231/dls-servbase.git 
-
-    dls-servbase --version
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/dls-servbase for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/kbp43231/dls-servbase.git 
-    cd dls-servbase
-    virtualenv /scratch/$USER/venv/dls-servbase
-    source /scratch/$USER/venv/dls-servbase/bin/activate 
-    pip install -e .[dev]
-    make -f .dls-servbase/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/dls-servbase/build/html/index.html
-
-Topics for further documentation:
-
-- TODO list of improvements
-- change log
-
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+Agnostic of type of underlying sql client, provides single-writer access to native database and has a predefined database schema for cookies.
 
+For documentation see: https://diamondlightsource.github.io/dls-servbase
```

### Comparing `dls-servbase-1.4.1/docs/conf.py` & `dls-servbase-1.5.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 from pathlib import Path
 from subprocess import check_output
 
 # Configuration file for the Sphinx documentation builder.
 #
@@ -184,17 +184,17 @@
 
 # I got this from https://github.com/sphinx-doc/sphinx/issues/4054.
 # It will allow the ${token} replacement in the rst documents.
 ultimate_replacements = {
     "$" + "{repository_name}": "dls-servbase",
     "$" + "{package_name}": "dls_servbase_lib",
     "$" + "{git_url}": "https://gitlab.diamond.ac.uk/kbp43231",
-    "$" + "{python_version_at_least}": "3.9",
+    "$" + "{python_version_at_least}": "3.10",
 }
 
 
 def setup(app):
     app.add_config_value("ultimate_replacements", {}, True)
     app.connect("source-read", ultimateReplace)
 
 
-# dae_devops_fingerprint 529445ac120d879ddd71245754e51ecb
+# dae_devops_fingerprint a8d7b8d65abc276648e440edf32e0454
```

### Comparing `dls-servbase-1.4.1/docs/images/dls-favicon.ico` & `dls-servbase-1.5.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/docs/images/dls-logo.svg` & `dls-servbase-1.5.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/pyproject.toml` & `dls-servbase-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # ********** Please don't edit this file!
-# ********** It has been generated automatically by dae_devops version 0.5.3.
+# ********** It has been generated automatically by dae_devops version 0.5.4.dev0+g1fb30ef.d20230527.
 # ********** For repository_name dls-servbase
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dls-servbase"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
 ]
 description = "Simple HTTP service for database operations."
 dependencies = ["aiohttp==3.8.3", "dls_mainiac", "dls_multiconf", "dls_normsql", "dls_utilpack", "setproctitle"]
 dynamic = ["version"]
 license.file = "LICENSE"
-readme = "README.rst"
-requires-python = ">=3.9"
+readme = "README.md"
+requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
     "black==22.12.0",
     "mypy",
     "flake8-isort",
     "Flake8-pyproject",
@@ -98,8 +96,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint ca7c759c4aa01b455a13284486cf7eaa
+# dae_devops_fingerprint cde1577a97f0e28d7fd63100e14d53ab
```

### Comparing `dls-servbase-1.4.1/src/dls_servbase.egg-info/PKG-INFO` & `dls-servbase-1.5.0/src/dls_servbase.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-servbase
-Version: 1.4.1
+Version: 1.5.0
 Summary: Simple HTTP service for database operations.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,60 +204,22 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitLab, https://gitlab.diamond.ac.uk/kbp43231/dls-servbase
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 dls-servbase
 =======================================================================
 
 Simple HTTP service for database operations.
 
-Intended advantages:
-
-- agnostic of type of underlying sql client
-- single-connection access to database
-- hosts a few predefined common database schema
-
-Installation
------------------------------------------------------------------------
-::
-
-    pip install git+https://gitlab.diamond.ac.uk/kbp43231/dls-servbase.git 
-
-    dls-servbase --version
-
-Documentation
------------------------------------------------------------------------
-
-See https://www.cs.diamond.ac.uk/dls-servbase for more detailed documentation.
-
-Building and viewing the documents locally::
-
-    git clone git+https://gitlab.diamond.ac.uk/kbp43231/dls-servbase.git 
-    cd dls-servbase
-    virtualenv /scratch/$USER/venv/dls-servbase
-    source /scratch/$USER/venv/dls-servbase/bin/activate 
-    pip install -e .[dev]
-    make -f .dls-servbase/Makefile validate_docs
-    browse to file:///scratch/$USER/venvs/dls-servbase/build/html/index.html
-
-Topics for further documentation:
-
-- TODO list of improvements
-- change log
-
-
-..
-    Anything below this line is used when viewing README.rst and will be replaced
-    when included in index.rst
+Agnostic of type of underlying sql client, provides single-writer access to native database and has a predefined database schema for cookies.
 
+For documentation see: https://diamondlightsource.github.io/dls-servbase
```

### Comparing `dls-servbase-1.4.1/src/dls_servbase.egg-info/SOURCES.txt` & `dls-servbase-1.5.0/src/dls_servbase.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 LICENSE
-README.rst
+README.md
 good_config1.yaml
 pyproject.toml
 .dae-devops/Makefile
 .dae-devops/prepare_git_dependencies.sh
 .dae-devops/project.yaml
 .dae-devops/docs/conventions.rst
 .dae-devops/docs/developing.rst
 .dae-devops/docs/devops.rst
 .dae-devops/docs/docs_structure.rst
+.dae-devops/docs/documenting.rst
 .dae-devops/docs/installing.rst
 .dae-devops/docs/testing.rst
 .devcontainer/Dockerfile
 .devcontainer/devcontainer.json
 .github/CONTRIBUTING.rst
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
@@ -71,14 +72,15 @@
 src/dls_servbase_lib/version.py
 src/dls_servbase_lib/contexts/__init__.py
 src/dls_servbase_lib/contexts/base.py
 src/dls_servbase_lib/contexts/classic.py
 src/dls_servbase_lib/contexts/contexts.py
 src/dls_servbase_lib/cookies/__init__.py
 src/dls_servbase_lib/cookies/base.py
+src/dls_servbase_lib/cookies/cookie_parser.py
 src/dls_servbase_lib/cookies/cookies.py
 src/dls_servbase_lib/cookies/dataface.py
 src/dls_servbase_lib/datafaces/__init__.py
 src/dls_servbase_lib/datafaces/aiohttp.py
 src/dls_servbase_lib/datafaces/context.py
 src/dls_servbase_lib/datafaces/datafaces.py
 src/dls_servbase_lib/datafaces/normsql.py
@@ -97,9 +99,10 @@
 tests/base_tester.py
 tests/conftest.py
 tests/test_aiohttp.py
 tests/test_database.py
 tests/test_dataface.py
 tests/test_dataface_takeover.py
 tests/test_gui.py
+tests/test_parse_cookie.py
 tests/configurations/mysql.yaml
 tests/configurations/sqlite.yaml
```

### Comparing `dls-servbase-1.4.1/src/dls_servbase_api/aiohttp_client.py` & `dls-servbase-1.5.0/src/dls_servbase_api/aiohttp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,25 +89,31 @@
         """"""
         await self._establish_client_session()
 
         async with self._client_session.get("/get_info") as response:
             return await response.json()
 
     # ----------------------------------------------------------------------------------------
-    async def client_protocolj(self, request_object, cookies=None):
+    async def client_protocolj(
+        self,
+        request_object,
+        cookies=None,
+        headers=None,
+    ):
         """"""
         await self._establish_client_session()
 
         # logger.info(describe("request_object", request_object))
 
         try:
             async with self._client_session.post(
                 f"{self.__client_netloc}/protocolj",
                 json=request_object,
                 cookies=cookies,
+                headers=headers,
             ) as response:
                 if response.status == 200:
                     response_json = await response.json()
                     if cookies is not None:
                         if response_json is None:
                             response_json = {}
                         response_json["__cookies"] = response.cookies
```

### Comparing `dls-servbase-1.4.1/src/dls_servbase_api/databases/database_definition.py` & `dls-servbase-1.5.0/src/dls_servbase_api/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_api/databases/table_definitions.py` & `dls-servbase-1.5.0/src/dls_servbase_api/databases/table_definitions.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_api/datafaces/aiohttp.py` & `dls-servbase-1.5.0/src/dls_servbase_api/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_api/datafaces/context.py` & `dls-servbase-1.5.0/src/dls_servbase_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_api/datafaces/datafaces.py` & `dls-servbase-1.5.0/src/dls_servbase_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_cli/main.py` & `dls-servbase-1.5.0/src/dls_servbase_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/base.py` & `dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_cli/subcommands/start_services.py` & `dls-servbase-1.5.0/src/dls_servbase_cli/subcommands/start_services.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_cli/version.py` & `dls-servbase-1.5.0/src/dls_servbase_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/__main__.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/base_aiohttp.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/base_aiohttp.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 import aiohttp
 import aiohttp.web
 import aiohttp.web_runner
 from dls_logformatter.functions import list_exception_causes
 from dls_mainiac_lib.mainiac import Mainiac
 from dls_multiconf_lib.multiconfs import multiconfs_get_default, multiconfs_has_default
 from dls_utilpack.callsign import callsign
+from dls_utilpack.describe import describe
 from dls_utilpack.explain import explain
 from dls_utilpack.global_signals import global_sigint
 from dls_utilpack.modify_process_title import modify_process_title
 from dls_utilpack.qualname import qualname
 from dls_utilpack.search_file import SearchFileNotFound, search_file
 
 from dls_servbase_api.aiohttp_client import AiohttpClient  # noqa: I001
 from dls_servbase_api.constants import Keywords  # noqa: I001
+from dls_servbase_lib.cookies.cookie_parser import CookieParser
 from dls_servbase_lib.cookies.cookies import Cookies
 
 logger = logging.getLogger(__name__)
 
 
 class Opaque:
     def __init__(self):
@@ -503,19 +505,38 @@
         if self.__cookie_specification is None:
             # Just don't do cookies.
             # Other calls may fail, alerting the developer to the mis-configuration.
             return
 
         logger.debug(f"[COOKOFF] registering cookies {cookie_names}")
 
+        # We have to parse the Cookie header ourselves from the raw
+        # since web_request.cookies uses SimpleCookie which doesn't work for
+        # Chrome's ill-formed: CookieControl={"necessaryCookies":[]
+        raw_header_cookie = web_request.headers.get("Cookie")
+        parsed_cookies = CookieParser().parse_raw(raw_header_cookie)
+        logger.debug(describe("[COOKOFF] parsed_cookies are", parsed_cookies))
+
+        # from http import cookies
+
+        # http_cookies = cookies.SimpleCookie()
+        # http_cookies.load(web_request.headers["Cookie"])
+        # logger.debug(
+        #     describe(
+        #         "[COOKOFF] http_cookies keys",
+        #         list(http_cookies.keys()),
+        #     )
+        # )
+
         # The caller gives the list of cookies that are interesting.
         for cookie_name in cookie_names:
             # We have a uuid for this cookie name already?
-            if cookie_name in web_request.cookies:
-                _uuid = web_request.cookies[cookie_name]
+            _uuid = parsed_cookies.get(cookie_name)
+
+            if _uuid is not None:
                 logger.debug(
                     f"[COOKOFF] registering cookie {cookie_name} from existing uuid {_uuid}"
                 )
                 if _uuid == "" or _uuid == "None":
                     _uuid = None
             else:
                 _uuid = None
@@ -727,18 +748,25 @@
 
     # ----------------------------------------------------------------------------------------
     def client_url(self):
         """"""
         return self.__callsign_url
 
     # ----------------------------------------------------------------------------------------
-    async def client_protocolj(self, request_object, cookies=None):
+    async def client_protocolj(
+        self,
+        request_object,
+        cookies=None,
+        headers=None,
+    ):
         """"""
         return await self.__aiohttp_client.client_protocolj(
-            request_object, cookies=cookies
+            request_object,
+            cookies=cookies,
+            headers=headers,
         )
 
     # ----------------------------------------------------------------------------------------
     async def client_get_json(self, url):
         """"""
         return await self.__aiohttp_client.client_get_json(url)
```

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/contexts/base.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/contexts/classic.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/contexts/classic.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/contexts/contexts.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/contexts/contexts.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/cookies/base.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/cookies/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/cookies/cookies.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/cookies/cookies.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/cookies/dataface.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/cookies/dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/aiohttp.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/context.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/datafaces.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/datafaces/normsql.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/datafaces/normsql.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/envvar.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/guis/aiohttp.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/guis/context.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/guis/guis.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/src/dls_servbase_lib/version.py` & `dls-servbase-1.5.0/src/dls_servbase_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/base.py` & `dls-servbase-1.5.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/base_context_tester.py` & `dls-servbase-1.5.0/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/base_specification_tester.py` & `dls-servbase-1.5.0/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/base_tester.py` & `dls-servbase-1.5.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/configurations/mysql.yaml` & `dls-servbase-1.5.0/tests/configurations/mysql.yaml`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/configurations/sqlite.yaml` & `dls-servbase-1.5.0/tests/configurations/sqlite.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 type: dls_servbase_lib.dls_servbase_contexts.classic
 
 logging_settings:
     console:
         enabled: True
         verbose: True
         filters:
-            markers:
+            Xmarkers:
                 - "[RELCOOK]"
                 - "[COOKSEL]"
                 - "[COOKOFF]"
                 - "[GUITABS]"
                 - "[SETTINGVAL]"
     logfile:
         enabled: True
```

### Comparing `dls-servbase-1.4.1/tests/conftest.py` & `dls-servbase-1.5.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     logging.getLogger("luigi-interface").setLevel("WARNING")
     logging.getLogger("luigi.dls_servbase_scheduler").setLevel("INFO")
     logging.getLogger("urllib3.connectionpool").setLevel("INFO")
 
     logging.getLogger("dls_servbase_lib.things").setLevel("INFO")
 
     # Messages about starting and stopping services.
-    logging.getLogger("dls_servbase_lib.base_aiohttp").setLevel("INFO")
+    # logging.getLogger("dls_servbase_lib.base_aiohttp").setLevel("INFO")
 
     # All dls_servbase database sql commands.
     # logging.getLogger("dls_servbase_lib.databases.aiosqlite").setLevel("INFO")
 
     logging.getLogger("dls_servbase_lib.dls_servbase_contexts.classic").setLevel("INFO")
     logging.getLogger("dls_servbase_lib.datafaces.context").setLevel("INFO")
```

### Comparing `dls-servbase-1.4.1/tests/test_aiohttp.py` & `dls-servbase-1.5.0/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/test_database.py` & `dls-servbase-1.5.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/test_dataface.py` & `dls-servbase-1.5.0/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/test_dataface_takeover.py` & `dls-servbase-1.5.0/tests/test_dataface_takeover.py`

 * *Files identical despite different names*

### Comparing `dls-servbase-1.4.1/tests/test_gui.py` & `dls-servbase-1.5.0/tests/test_gui.py`

 * *Files 13% similar despite different names*

```diff
@@ -67,49 +67,57 @@
             # Load tabs, of which there are none at the start.
             # This establishes the cookie though.
             load_tabs_request = {
                 Keywords.COMMAND: Commands.LOAD_TABS,
                 ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
             }
 
+            logger.debug("---------------------- making request 1 --------------------")
             response = await dls_servbase_guis_get_default().client_protocolj(
                 load_tabs_request, cookies={}
             )
 
             # The response is json, with the last saved tab_id, which is None at first.
             assert Keywords.TAB_ID in response
             assert response[Keywords.TAB_ID] is None
 
             # We should also have cookies back.
             assert "__cookies" in response
             cookies = response["__cookies"]
             assert Cookies.TABS_MANAGER in cookies
 
-            # Use the cookie name in the next requests.
-            cookie_uuid = cookies[Cookies.TABS_MANAGER]
+            # Use the tabs manager cookie value in the next requests.
+            cookie_uuid = cookies[Cookies.TABS_MANAGER].value
 
             # --------------------------------------------------------------------
             # Select a tab.
             # The response is json, but nothing really to see in it.
 
             select_tab_request = {
                 Keywords.COMMAND: Commands.SELECT_TAB,
                 ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
                 Keywords.TAB_ID: "123",
             }
 
+            logger.debug("---------------------- making request 2 --------------------")
             response = await dls_servbase_guis_get_default().client_protocolj(
                 select_tab_request, cookies={Cookies.TABS_MANAGER: cookie_uuid}
             )
 
             # --------------------------------------------------------------------
             # Load tabs again, this time we should get the saved tab_id.
 
+            logger.debug("---------------------- making request 3 --------------------")
+            # Put a deliberately funky cookie string into the header.
+            raw_cookie_header = (
+                'BadCookie={"something"}; ' + f"{Cookies.TABS_MANAGER} = {cookie_uuid};"
+            )
             response = await dls_servbase_guis_get_default().client_protocolj(
-                load_tabs_request, cookies={Cookies.TABS_MANAGER: cookie_uuid}
+                load_tabs_request,
+                headers={"Cookie": raw_cookie_header},
             )
 
             logger.debug(describe("second load_tabs response", response))
             assert Keywords.TAB_ID in response
             assert response[Keywords.TAB_ID] == "123"
 
             # --------------------------------------------------------------------
@@ -118,24 +126,42 @@
 
             select_tab_request = {
                 Keywords.COMMAND: Commands.SELECT_TAB,
                 ProtocoljKeywords.ENABLE_COOKIES: [Cookies.TABS_MANAGER],
                 Keywords.TAB_ID: "456",
             }
 
+            logger.debug("---------------------- making request 4 --------------------")
             response = await dls_servbase_guis_get_default().client_protocolj(
-                select_tab_request, cookies={Cookies.TABS_MANAGER: cookie_uuid}
+                select_tab_request,
+                cookies={Cookies.TABS_MANAGER: cookie_uuid},
+            )
+
+            # --------------------------------------------------------------------
+            # Load tabs again, this time we should get the updated tab_id.
+
+            logger.debug("---------------------- making request 5 --------------------")
+            response = await dls_servbase_guis_get_default().client_protocolj(
+                load_tabs_request,
+                cookies={Cookies.TABS_MANAGER: cookie_uuid},
             )
 
+            logger.debug(describe("third load_tabs response", response))
+            assert Keywords.TAB_ID in response
+            assert response[Keywords.TAB_ID] == "456"
+
             # --------------------------------------------------------------------
             # Write a text file and fetch it through the http server.
             filename = "test.html"
             contents = "some test html"
             with open(f"{output_directory}/{filename}", "wt") as file:
                 file.write(contents)
+            logger.debug(
+                "---------------------- making request 6 (html file) --------------------"
+            )
             text = await dls_servbase_guis_get_default().client_get_file(filename)
             # assert text == contents
 
             # Write a binary file and fetch it through the http server.
             filename = "test.exe"
             contents = "some test binary"
             with open(f"{output_directory}/{filename}", "wt") as file:
```

