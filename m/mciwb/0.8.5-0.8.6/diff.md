# Comparing `tmp/mciwb-0.8.5.tar.gz` & `tmp/mciwb-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mciwb-0.8.5.tar", last modified: Tue Mar 14 16:54:07 2023, max compression
+gzip compressed data, was "mciwb-0.8.6.tar", last modified: Wed May 31 00:17:06 2023, max compression
```

## Comparing `mciwb-0.8.5.tar` & `mciwb-0.8.6.tar`

### file list

```diff
@@ -1,178 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.057243 mciwb-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-14 16:53:57.000000 mciwb-0.8.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.029242 mciwb-0.8.5/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-14 16:53:57.000000 mciwb-0.8.5/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.029242 mciwb-0.8.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.025242 mciwb-0.8.5/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.029242 mciwb-0.8.5/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.029242 mciwb-0.8.5/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.029242 mciwb-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-14 16:53:57.000000 mciwb-0.8.5/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-14 16:53:57.000000 mciwb-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-14 16:53:57.000000 mciwb-0.8.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.029242 mciwb-0.8.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-14 16:53:57.000000 mciwb-0.8.5/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-14 16:53:57.000000 mciwb-0.8.5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-14 16:53:57.000000 mciwb-0.8.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-14 16:53:57.000000 mciwb-0.8.5/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-14 16:53:57.000000 mciwb-0.8.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-14 16:53:57.000000 mciwb-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-03-14 16:54:07.057243 mciwb-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-14 16:53:57.000000 mciwb-0.8.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.029242 mciwb-0.8.5/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-03-14 16:53:57.000000 mciwb-0.8.5/blocks/gate.json
--rw-r--r--   0 runner    (1001) docker     (123)  3455491 2023-03-14 16:53:57.000000 mciwb-0.8.5/blocks/ground.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.033242 mciwb-0.8.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.033242 mciwb-0.8.5/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.033242 mciwb-0.8.5/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.037242 mciwb-0.8.5/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.037242 mciwb-0.8.5/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.037242 mciwb-0.8.5/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/reference/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.037242 mciwb-0.8.5/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.037242 mciwb-0.8.5/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    85039 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.037242 mciwb-0.8.5/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.037242 mciwb-0.8.5/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/explanations/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/explanations/docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/explanations/mcipc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/explanations/scope.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/explanations/server-config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.037242 mciwb-0.8.5/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/how-to/backup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/how-to/completion.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/how-to/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/how-to/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/how-to/startup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/how-to/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/how-to/wsl2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.049243 mciwb-0.8.5/docs/user/images/
--rw-r--r--   0 runner    (1001) docker     (123)  2170233 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/castle.png
--rw-r--r--   0 runner    (1001) docker     (123)   148941 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/compass.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/compass.png:Zone.Identifier
--rw-r--r--   0 runner    (1001) docker     (123)  1232938 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/coords.excalidraw.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/coords.excalidraw.png:Zone.Identifier
--rw-r--r--   0 runner    (1001) docker     (123)  1054340 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/golem.png
--rw-r--r--   0 runner    (1001) docker     (123)   713460 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/launcher.png
--rw-r--r--   0 runner    (1001) docker     (123)  1093134 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/pagoda.png
--rw-r--r--   0 runner    (1001) docker     (123)   500903 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/portal.png
--rw-r--r--   0 runner    (1001) docker     (123)    31873 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/prompt.excalidraw.png
--rw-r--r--   0 runner    (1001) docker     (123)    89820 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/pylance.png
--rw-r--r--   0 runner    (1001) docker     (123)   105651 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/remote_ubuntu.excalidraw.png
--rw-r--r--   0 runner    (1001) docker     (123)   222406 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/remote_wsl2.excalidraw.png
--rw-r--r--   0 runner    (1001) docker     (123)    32166 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/server_address.png
--rw-r--r--   0 runner    (1001) docker     (123)    87855 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/split_term.png
--rw-r--r--   0 runner    (1001) docker     (123)    91403 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/table_json.png
--rw-r--r--   0 runner    (1001) docker     (123)   123548 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/terminals.png
--rw-r--r--   0 runner    (1001) docker     (123)   156885 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/trust.png
--rw-r--r--   0 runner    (1001) docker     (123)   226868 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/typewriter.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   624814 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/images/vscode_hello.excalidraw.png
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.049243 mciwb-0.8.5/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/reference/demo.rst
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.049243 mciwb-0.8.5/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/00-prereq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/01-setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/02-orientation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/03-variables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/04-loops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/05-functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/05a-modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/06-if-then.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/07-lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/08-classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-14 16:53:57.000000 mciwb-0.8.5/docs/user/tutorials/09-dictionaries.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-14 16:53:57.000000 mciwb-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-14 16:53:57.000000 mciwb-0.8.5/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 16:54:07.057243 mciwb-0.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.029242 mciwb-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.053243 mciwb-0.8.5/src/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/arrows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/background.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/bat.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/example2player.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/house.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/pagoda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/snowball.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/village.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/demo/walls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.053243 mciwb-0.8.5/src/mciwb/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-14 16:54:06.000000 mciwb-0.8.5/src/mciwb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/copier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/iwb.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/nbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/signs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-03-14 16:53:57.000000 mciwb-0.8.5/src/mciwb/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.053243 mciwb-0.8.5/src/mciwb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-03-14 16:54:06.000000 mciwb-0.8.5/src/mciwb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-03-14 16:54:07.000000 mciwb-0.8.5/src/mciwb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 16:54:06.000000 mciwb-0.8.5/src/mciwb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-14 16:54:06.000000 mciwb-0.8.5/src/mciwb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-14 16:54:06.000000 mciwb-0.8.5/src/mciwb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-14 16:54:06.000000 mciwb-0.8.5/src/mciwb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.057243 mciwb-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/mockclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/mockplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_mciwb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.057243 mciwb-0.8.5/tests/test_system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_system/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_system/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_system/test_poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_system/test_world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:54:07.057243 mciwb-0.8.5/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_unit/test_copier.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_unit/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-14 16:53:57.000000 mciwb-0.8.5/tests/test_unit/test_player.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-14 16:53:57.000000 mciwb-0.8.5/todo.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.440762 mciwb-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-31 00:16:52.000000 mciwb-0.8.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.392762 mciwb-0.8.6/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-31 00:16:52.000000 mciwb-0.8.6/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.392762 mciwb-0.8.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.384761 mciwb-0.8.6/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.392762 mciwb-0.8.6/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.392762 mciwb-0.8.6/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.392762 mciwb-0.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-31 00:16:52.000000 mciwb-0.8.6/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-31 00:16:52.000000 mciwb-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-31 00:16:52.000000 mciwb-0.8.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.392762 mciwb-0.8.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 00:16:52.000000 mciwb-0.8.6/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-31 00:16:52.000000 mciwb-0.8.6/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-31 00:16:52.000000 mciwb-0.8.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-31 00:16:52.000000 mciwb-0.8.6/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-31 00:16:52.000000 mciwb-0.8.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 00:16:52.000000 mciwb-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-05-31 00:17:06.440762 mciwb-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-31 00:16:52.000000 mciwb-0.8.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.392762 mciwb-0.8.6/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-31 00:16:52.000000 mciwb-0.8.6/blocks/gate.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3455491 2023-05-31 00:16:52.000000 mciwb-0.8.6/blocks/ground.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.400762 mciwb-0.8.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.400762 mciwb-0.8.6/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.400762 mciwb-0.8.6/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.400762 mciwb-0.8.6/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.404762 mciwb-0.8.6/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.404762 mciwb-0.8.6/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/reference/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.404762 mciwb-0.8.6/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.404762 mciwb-0.8.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    85039 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.404762 mciwb-0.8.6/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.404762 mciwb-0.8.6/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/explanations/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/explanations/docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/explanations/mcee.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/explanations/mcipc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/explanations/scope.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/explanations/server-config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.408762 mciwb-0.8.6/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/how-to/backup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/how-to/completion.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/how-to/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/how-to/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/how-to/startup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/how-to/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/how-to/wsl2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.424762 mciwb-0.8.6/docs/user/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  2170233 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/castle.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148941 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/compass.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/compass.png:Zone.Identifier
+-rw-r--r--   0 runner    (1001) docker     (123)  1232938 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/coords.excalidraw.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/coords.excalidraw.png:Zone.Identifier
+-rw-r--r--   0 runner    (1001) docker     (123)  1054340 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/golem.png
+-rw-r--r--   0 runner    (1001) docker     (123)   713460 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/launcher.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1093134 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/pagoda.png
+-rw-r--r--   0 runner    (1001) docker     (123)   500903 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/portal.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31873 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/prompt.excalidraw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89820 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/pylance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105651 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/remote_ubuntu.excalidraw.png
+-rw-r--r--   0 runner    (1001) docker     (123)   222406 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/remote_wsl2.excalidraw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32166 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/server_address.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87855 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/split_term.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91403 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/table_json.png
+-rw-r--r--   0 runner    (1001) docker     (123)   123548 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/terminals.png
+-rw-r--r--   0 runner    (1001) docker     (123)   156885 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/trust.png
+-rw-r--r--   0 runner    (1001) docker     (123)   226868 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/typewriter.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   624814 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/images/vscode_hello.excalidraw.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.424762 mciwb-0.8.6/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/reference/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.428762 mciwb-0.8.6/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/00-prereq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/01-setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/02-orientation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/03-variables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/04-loops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/05-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/05a-modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/06-if-then.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/07-lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/08-classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/09-dictionaries.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/10-threading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/11-switches.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/12-signs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 00:16:52.000000 mciwb-0.8.6/docs/user/tutorials/13-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-31 00:16:52.000000 mciwb-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 00:16:52.000000 mciwb-0.8.6/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:17:06.440762 mciwb-0.8.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.388762 mciwb-0.8.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.432762 mciwb-0.8.6/src/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/arrows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/example2player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/pagoda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/snowball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/village.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/demo/walls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.432762 mciwb-0.8.6/src/mciwb/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 00:17:06.000000 mciwb-0.8.6/src/mciwb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/iwb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/nbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/signs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-31 00:16:52.000000 mciwb-0.8.6/src/mciwb/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.436762 mciwb-0.8.6/src/mciwb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-05-31 00:17:06.000000 mciwb-0.8.6/src/mciwb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-31 00:17:06.000000 mciwb-0.8.6/src/mciwb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:17:06.000000 mciwb-0.8.6/src/mciwb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 00:17:06.000000 mciwb-0.8.6/src/mciwb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-31 00:17:06.000000 mciwb-0.8.6/src/mciwb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 00:17:06.000000 mciwb-0.8.6/src/mciwb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.436762 mciwb-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/mockclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/mockplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_mciwb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.436762 mciwb-0.8.6/tests/test_system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_system/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_system/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_system/test_poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_system/test_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:17:06.440762 mciwb-0.8.6/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_unit/test_copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_unit/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 00:16:52.000000 mciwb-0.8.6/tests/test_unit/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-31 00:16:52.000000 mciwb-0.8.6/todo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-31 00:16:52.000000 mciwb-0.8.6/video.md
```

### Comparing `mciwb-0.8.5/.devcontainer/devcontainer.json` & `mciwb-0.8.6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.github/CONTRIBUTING.rst` & `mciwb-0.8.6/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.github/actions/install_requirements/action.yml` & `mciwb-0.8.6/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.github/dependabot.yml` & `mciwb-0.8.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.github/pages/make_switcher.py` & `mciwb-0.8.6/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.github/workflows/code.yml` & `mciwb-0.8.6/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.github/workflows/docs.yml` & `mciwb-0.8.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.github/workflows/docs_clean.yml` & `mciwb-0.8.6/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.github/workflows/linkcheck.yml` & `mciwb-0.8.6/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.gitignore` & `mciwb-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/.vscode/launch.json` & `mciwb-0.8.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/Dockerfile` & `mciwb-0.8.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/LICENSE` & `mciwb-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/PKG-INFO` & `mciwb-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciwb
-Version: 0.8.5
+Version: 0.8.6
 Summary: Minecraft Interactive world builder
 Author-email: Firstname Lastname <email@address.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -222,14 +222,18 @@
 ===================================
 
 This project is intended as a fun way to learn the Python Programming Language.
 
 Experienced Python programmers can also use this library to create
 Minecraft worlds with interactive Python features.
 
+
+For the Reddit discussion see  
+`HERE <https://www.reddit.com/r/Minecraftbuilds/comments/11rqauh/build_things_using_python>`_
+
 Quick Start
 -----------
 
 To get started learning Python, see
 `Introduction <https://gilesknap.github.io/mciwb/main/user/tutorials/00-prereq.html>`_
 
 For existing Python developers, see
@@ -237,20 +241,22 @@
 
 Example Build
 -------------
 
 The pagoda and castle with working portcullis were all created programmatically
 with Python and the current version of MCIWB.
 
+
 .. figure:: https://gilesknap.github.io/mciwb/main/_images/castle.png
    :alt: castle
    :align: center
    :width: 600px
-
-   Example Build
+   :target: https://photos.app.goo.gl/utFt6KadWbdabR8x6
+   
+   Example Build - **Click for Video**
 
 Goals
 -----
 
 Minecraft Interactive World Builder's goals are:
 
  - Use Python to create anything inside of Minecraft worlds.
```

### Comparing `mciwb-0.8.5/README.rst` & `mciwb-0.8.6/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 ===================================
 
 This project is intended as a fun way to learn the Python Programming Language.
 
 Experienced Python programmers can also use this library to create
 Minecraft worlds with interactive Python features.
 
+
+For the Reddit discussion see  
+`HERE <https://www.reddit.com/r/Minecraftbuilds/comments/11rqauh/build_things_using_python>`_
+
 Quick Start
 -----------
 
 To get started learning Python, see
 `Introduction <https://gilesknap.github.io/mciwb/main/user/tutorials/00-prereq.html>`_
 
 For existing Python developers, see
@@ -20,20 +24,22 @@
 
 Example Build
 -------------
 
 The pagoda and castle with working portcullis were all created programmatically
 with Python and the current version of MCIWB.
 
+
 .. figure:: https://gilesknap.github.io/mciwb/main/_images/castle.png
    :alt: castle
    :align: center
    :width: 600px
-
-   Example Build
+   :target: https://photos.app.goo.gl/utFt6KadWbdabR8x6
+   
+   Example Build - **Click for Video**
 
 Goals
 -----
 
 Minecraft Interactive World Builder's goals are:
 
  - Use Python to create anything inside of Minecraft worlds.
```

### Comparing `mciwb-0.8.5/blocks/gate.json` & `mciwb-0.8.6/blocks/gate.json`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/blocks/ground.json` & `mciwb-0.8.6/blocks/ground.json`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/conf.py` & `mciwb-0.8.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `mciwb-0.8.6/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/explanations/decisions.rst` & `mciwb-0.8.6/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/how-to/build-docs.rst` & `mciwb-0.8.6/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/how-to/lint.rst` & `mciwb-0.8.6/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/how-to/make-release.rst` & `mciwb-0.8.6/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/how-to/pin-requirements.rst` & `mciwb-0.8.6/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/how-to/test-container.rst` & `mciwb-0.8.6/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/how-to/update-tools.rst` & `mciwb-0.8.6/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/index.rst` & `mciwb-0.8.6/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/reference/standards.rst` & `mciwb-0.8.6/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/developer/tutorials/dev-install.rst` & `mciwb-0.8.6/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/images/logo.png` & `mciwb-0.8.6/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/index.rst` & `mciwb-0.8.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/explanations/coordinates.rst` & `mciwb-0.8.6/docs/user/explanations/coordinates.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/explanations/docs-structure.rst` & `mciwb-0.8.6/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/explanations/mcipc.rst` & `mciwb-0.8.6/docs/user/explanations/mcipc.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/explanations/scope.rst` & `mciwb-0.8.6/docs/user/explanations/scope.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/explanations/server-config.rst` & `mciwb-0.8.6/docs/user/explanations/server-config.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/how-to/backup.rst` & `mciwb-0.8.6/docs/user/how-to/backup.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,58 +11,64 @@
 .. _backups:
 
 Backups of mciwb-server
 -----------------------
 
 Backups provide a way to save our world to a file when we are happy with it.
 Then we are protected from loosing our work if we make a programming error.
-When things go wrong we can just restore back to a previous version of the 
+When things go wrong we can just restore back to a previous version of the
 world.
 
 To backup the world type this at the Python Prompt::
 
     world.backup()
 
 This will create a backup with a name that is the current date and time. You
 can also specify a name if you want. Let's do that now::
-    
+
     world.backup('my-first-backup')
 
 It is better not to use spaces in backup names so I used dash to separate
 the words.
 
 Now lets do a restore. You can first have your player dig a hole in our
 flat area, this is to make a change that we don't want to keep.
 Then exit the Python Prompt using 'Ctrl+D'. Now we are back
 at the ``bash`` prompt and we can look in the backups folder to see our
-list of backups e.g::
+list of backups e.g
+
+This command::
+
+    ls $HOME/mciwb-backups
+
+Shows my backup files like this::
 
-    
-    (.venv) [giles@ws1 mciwb]$ ls $HOME/mciwb-backups
-    22-07-13.06.26.01.zip  22-07-13.06.34.06.zip  flat-area-backup.zip
+    22-07-13.06.26.01.zip  22-07-13.06.34.06.zip  my-first-backup.zip
 
 You backups are stored in a folder called $HOME/mciwb-backups and ``ls`` is
 a terminal command that lists the contents of that folder.
 
 Note
 that the backup files all end in ``.zip``. Some of them are dated but you also
 see the ``flat-area-backup.zip`` file that we named explicitly.
 
 Now you can restore from backup with the following command::
 
-    (.venv) [giles@ws1 mciwb]$ mciwb restore flat-area-backup
+    mciwb restore flat-area-backup
+
+The output should look something like this::
+
     INFO:   Stopping Minecraft Server mciwb-server ...
     INFO:   Restored /home/giles/mciwb-server/world from /home/giles/mciwb-backups/flat-area-backup.zip
     INFO:   Launching existing Minecraft server in /home/giles/mciwb-server
     INFO:   Launching Minecraft Server 'mciwb-server' on port 20101 ...
     INFO:   waiting for server to come online ...
     INFO:   Server mciwb-server is online on port 20101
 
-    (.venv) [giles@ws1 mciwb]$ 
-    
+
 The ``mciwb restore``
 command can be given the name of the backup to restore or if you specify no
 name it will restore the most recent backup.
 
 When the server restarts you can reconnect your client. You should see that
 the hole you dug has disappeared.
```

### Comparing `mciwb-0.8.5/docs/user/how-to/completion.rst` & `mciwb-0.8.6/docs/user/how-to/completion.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/how-to/coordinates.rst` & `mciwb-0.8.6/docs/user/how-to/coordinates.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/how-to/extensions.rst` & `mciwb-0.8.6/docs/user/how-to/extensions.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/how-to/startup.rst` & `mciwb-0.8.6/docs/user/how-to/startup.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/how-to/troubleshooting.rst` & `mciwb-0.8.6/docs/user/how-to/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/how-to/wsl2.rst` & `mciwb-0.8.6/docs/user/how-to/wsl2.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 Windows Subsystem for Linux 2 (or WSL2) should already have been 
 installed as part
 of the Docker Desktop install that was done in `docker`. 
 
 To make sure the correct version of WSL2 is installed you can open a
 CMD window in Administrator  mode and run the following commands:
 
-    wsl --install
-    wsl --set-version Ubuntu-22.04 2
+``wsl --install``
+
+``wsl --set-version Ubuntu-22.04 2``
 
 WSL2 is a Linux distribution that runs inside of Windows. It allows us to make
 the tutorials look exactly the same for Windows, Linux and MacOS. 
 The linux command line in Ubuntu Linux inside WSL2 is called ``bash`` and 
 is easier to use than Windows equivalents.
 
 Adding the WSL2 extension
```

### Comparing `mciwb-0.8.5/docs/user/images/castle.png` & `mciwb-0.8.6/docs/user/images/castle.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/compass.png` & `mciwb-0.8.6/docs/user/images/compass.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/coords.excalidraw.png` & `mciwb-0.8.6/docs/user/images/coords.excalidraw.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/golem.png` & `mciwb-0.8.6/docs/user/images/golem.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/launcher.png` & `mciwb-0.8.6/docs/user/images/launcher.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/pagoda.png` & `mciwb-0.8.6/docs/user/images/pagoda.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/portal.png` & `mciwb-0.8.6/docs/user/images/portal.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/prompt.excalidraw.png` & `mciwb-0.8.6/docs/user/images/prompt.excalidraw.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/pylance.png` & `mciwb-0.8.6/docs/user/images/pylance.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/remote_ubuntu.excalidraw.png` & `mciwb-0.8.6/docs/user/images/remote_ubuntu.excalidraw.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/remote_wsl2.excalidraw.png` & `mciwb-0.8.6/docs/user/images/remote_wsl2.excalidraw.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/server_address.png` & `mciwb-0.8.6/docs/user/images/server_address.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/split_term.png` & `mciwb-0.8.6/docs/user/images/split_term.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/table_json.png` & `mciwb-0.8.6/docs/user/images/table_json.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/terminals.png` & `mciwb-0.8.6/docs/user/images/terminals.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/trust.png` & `mciwb-0.8.6/docs/user/images/trust.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/typewriter.jpg` & `mciwb-0.8.6/docs/user/images/typewriter.jpg`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/images/vscode_hello.excalidraw.png` & `mciwb-0.8.6/docs/user/images/vscode_hello.excalidraw.png`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/index.rst` & `mciwb-0.8.6/docs/user/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,18 @@
             tutorials/04-loops
             tutorials/05-functions
             tutorials/05a-modules
             tutorials/06-if-then
             tutorials/07-lists
             tutorials/08-classes
             tutorials/09-dictionaries
+            tutorials/10-threading
+            tutorials/11-switches
+            tutorials/12-signs
+            tutorials/13-structures
 
         +++
 
         Tutorials for installation and typical usage. New users start here.
 
     .. grid-item-card:: :material-regular:`directions;3em`
 
@@ -55,14 +59,15 @@
             :maxdepth: 1
 
             explanations/docs-structure
             explanations/scope
             explanations/server-config
             explanations/coordinates
             explanations/mcipc
+            explanations/mcee
 
 
         +++
 
         Explanations of how the library works and why it works that way.
 
     .. grid-item-card:: :material-regular:`menu_book;3em`
```

### Comparing `mciwb-0.8.5/docs/user/reference/api.rst` & `mciwb-0.8.6/docs/user/reference/api.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/reference/index.rst` & `mciwb-0.8.6/docs/user/reference/index.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/tutorials/00-prereq.rst` & `mciwb-0.8.6/docs/user/tutorials/00-prereq.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/tutorials/01-setup.rst` & `mciwb-0.8.6/docs/user/tutorials/01-setup.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 - The Minecraft Java Client (with Minecraft account purchase)
 - Docker Desktop
 - Visual Studio Code
 - Python
 - Minecraft Interactive World Builder Python package
 
 .. warning::
-    
+
     The tutorials for this project are intended to be accessible for
-    complete beginners. However, this first step of getting all of the 
+    complete beginners. However, this first step of getting all of the
     software installed may need a little bit of knowledge of the basics of
-    your operating system. 
+    your operating system.
 
-    For this Setup Tutorial, I recommend that novices get a little help from 
-    someone with computer experience. This setup tutorial need only 
+    For this Setup Tutorial, I recommend that novices get a little help from
+    someone with computer experience. This setup tutorial need only
     be done once (per computer) and the remaining tutorials should not
     require prior knowledge.
 
 
 The Minecraft Java Client
 -------------------------
 
 If you already have the Minecraft Java Client installed proceed to `docker`.
 
 You will need to purchase a license for Minecraft from Microsoft.
 
 Go to this site to buy your copy, if you do not already have one:
 
-    https://www.minecraft.net/en-us/store/minecraft-java-bedrock-edition-pc  
+    https://www.minecraft.net/en-us/store/minecraft-java-bedrock-edition-pc
 
 Once you have a license, download the Java client to
-the computer where you will be trying out MCIWB. 
+the computer where you will be trying out MCIWB.
 This is the download link for the Java client:
-    
+
         https://www.minecraft.net/en-us/download
 
-Microsoft has now bundled the Java and Bedrock editions together. 
+Microsoft has now bundled the Java and Bedrock editions together.
 We are using the Java edition here but this project could be adapted to
 work for either in future.
 
 When you start Minecraft you will be asked to login with your Microsoft details,
 note that the 'Mojang Login' option is only for legacy users who have not
 yet migrated.
 
@@ -73,79 +73,79 @@
 use docker on your behalf.
 
 The easiest way to install Docker is to use Docker Desktop which is free to
 use for individuals.
 
 Windows:
     Docker Desktop requires WSL2 and a linux distribution to go with it.
-    So you should first install WSL2 and Ubuntu 22.04 LTS from here 
+    So you should first install WSL2 and Ubuntu 22.04 LTS from here
     - https://apps.microsoft.com/store/detail/ubuntu-2204-lts/9PN20MSR04DW
 
 All Platforms:
     Instructions for Docker Desktop installation for all platforms are here:
     - https://docs.docker.com/get-docker/
 
-For mciwb to work you will need Docker Desktop to be running before you 
-start Visual Studio Code. So start it from the start menu before moving to 
+For mciwb to work you will need Docker Desktop to be running before you
+start Visual Studio Code. So start it from the start menu before moving to
 the next step.
 
 To make things easier next time you could go into settings (accessed
-via the cog icon in the title bar of the Docker Desktop main window) 
-and tick the option 
+via the cog icon in the title bar of the Docker Desktop main window)
+and tick the option
 ``Start Docker Desktop when you log in``.
 
 
 .. _vscode:
 
 Visual Studio Code
 ------------------
 
 This is the tool we will use to edit our Python code. If you are already
 a developer then you can use your preferred IDE instead. The tutorials
-will use Visual Studio Code, so if you are new to programming this is 
+will use Visual Studio Code, so if you are new to programming this is
 a recommended install.
 
 VSCode is free, open-source software.
 
 This link provides downloads for all flavours of VSCode:
-    
+
     https://code.visualstudio.com/download
 
 
 Command Line
 ------------
 
 From now on we are going to start using the command line. You are free to use
-whatever terminal program you like, however I recommend that you use the 
+whatever terminal program you like, however I recommend that you use the
 integrated terminal inside of Visual Studio Code.
 
-Here we will set up our initial VSCode work folder and get a ``bash`` 
-command line prompt. ``bash`` is the most popular ``shell`` for Linux, 
-it provides a command line interface to all the utilities and services 
-on a Linux computer. On Windows we will be using the Linux Subsystem so will 
-also use ``bash``. On Mac we will be using ``zsh`` but this is pretty similar 
+Here we will set up our initial VSCode work folder and get a ``bash``
+command line prompt. ``bash`` is the most popular ``shell`` for Linux,
+it provides a command line interface to all the utilities and services
+on a Linux computer. On Windows we will be using the Linux Subsystem so will
+also use ``bash``. On Mac we will be using ``zsh`` but this is pretty similar
 to ``bash``.
 
 
 First open VSCode from the start menu.
 
 .. note::
 
     **Windows Users: Important**
 
     We are going to use 'Windows Subsystem for Linux 2' or WSL2.
-    Go here first to get VSCode connected to WSL2: 
+    Go here first to get VSCode connected to WSL2:
     `wsl2`
 
 
 Let's create a work folder for use in further tutorials and tell VSCode To
-open the folder. We'll call it  ``my_world`` but you are free to use your 
+open the folder. We'll call it  ``my_world`` but you are free to use your
 own name.
 
-First start a terminal by selecting from the menu bar 
+First start a terminal by selecting from the menu bar
 ``Terminal -> New Terminal``.
 
 The bottom half of your VSCode window will display a ``bash``
 prompt like this:
 
 .. image:: ../images/prompt.excalidraw.png
     :alt: VSCode Startup
@@ -155,19 +155,19 @@
 Type the following to make sure you are in in your home directory and then
 create a new folder called ``my_world``::
 
     cd
     mkdir my_world
 
 Now we want to reopen VSCode with the new folder set as its work area.
-From the menu bar choose ``File -> Open Folder``. You will see a list of 
+From the menu bar choose ``File -> Open Folder``. You will see a list of
 folders, select ``my_world`` and click OK.
 
-You will be asked if you trust the authors of files in this folder. 
-You do trust them because they are you! So click 
+You will be asked if you trust the authors of files in this folder.
+You do trust them because they are you! So click
 ``Yes I trust the authors``.
 
 .. image:: ../images/trust.png
     :alt: VSCode Startup
     :width: 500px
     :align: center
 
@@ -179,26 +179,26 @@
     :align: left
 
 From this point on all commands typed in the console and chosen from VSCode
 menus should be the same for Windows, Linux and MacOS. This is because you
 now have a bash shell for typing commands.
 
 .. warning::
-    There is one caveat here. When directed to install a software package with 
+    There is one caveat here. When directed to install a software package with
     ``sudo apt``, this will only apply if you are using a Debian derived
-    OS such as Ubuntu (this also covers Windows WSL2 users). 
-    Mac, CentOs, Arch based users - I'm hoping you will know the equivalent 
+    OS such as Ubuntu (this also covers Windows WSL2 users).
+    Mac, CentOs, Arch based users - I'm hoping you will know the equivalent
     commands. I will supply an appendix for other OSes in future.
 
 Python
 ------
 
 The Python Programming Language is also free and open-source.
 
-This is essential for working with MCIWB. 
+This is essential for working with MCIWB.
 Python 3.10 because the underlying RCON library requires it. This is the
 latest version of Python at the time of writing.
 
 These commands will install the necessary packages to make Python 3.10
 available on your system::
 
     sudo apt update
@@ -224,28 +224,29 @@
 separate from the packages you install for other projects.
 
 First create the Virtual Environment by typing (note the leading "."
 in the folder name ".venv")::
 
     python3.10 -m venv .venv
 
-Then activate it by typing the following. This command will need to be 
+Then activate it by typing the following. This command will need to be
 repeated each time you restart your terminal or open a new terminal::
 
     source .venv/bin/activate
 
-Note you can tell you have an active **Virtual Environment** because 
+Note you can tell you have an active **Virtual Environment** because
 your terminal prompt will change to have a leading (.venv) like this::
 
-    (.venv) giles@gkwin:~/my_world$
+    (.venv) $
+
 
 Minecraft Interactive World Builder library
 -------------------------------------------
 
-The final component is MCIWB itself. This needs to be added to the 
+The final component is MCIWB itself. This needs to be added to the
 Python environment we already made above. Again, this is free open open-source
 software.
 
 Before the next step, let's make sure that we are in the right folder and
 that we have the **Virtual Environment** activated::
 
     cd $HOME/my_world
@@ -260,15 +261,15 @@
 
 Everything is all set up ready so the following simple command will get
 mciwb from the Python Package Index (PyPi) and install it into the
 **Virtual Environment**::
 
     pip install mciwb
 
-Assuming all is well you should be able to verify everything is working 
+Assuming all is well you should be able to verify everything is working
 by typing the following::
 
     mciwb --help
 
-That's all the hard bits done and they only need to be done once. 
+That's all the hard bits done and they only need to be done once.
 You can now proceed to the next tutorial.
```

### Comparing `mciwb-0.8.5/docs/user/tutorials/02-orientation.rst` & `mciwb-0.8.6/docs/user/tutorials/02-orientation.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/tutorials/03-variables.rst` & `mciwb-0.8.6/docs/user/tutorials/03-variables.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/tutorials/04-loops.rst` & `mciwb-0.8.6/docs/user/tutorials/04-loops.rst`

 * *Files 6% similar despite different names*

```diff
@@ -12,50 +12,70 @@
 approach as that for the iron golem in the previous tutorial. But that would
 be a lot of typing. So instead we'll take a look at Python ``for loops``.
 
 Backups
 -------
 
 Before we proceed I recommend that you learn about making backups of the
-world. That way we can experiment as much as we like and restore our 
+world. That way we can experiment as much as we like and restore our
 world back to a good state. Go and read `backups` and then come back to
 this tutorial.
 
+Whitespace
+----------
+
+Python uses whitespace to delimit blocks of code. You can
+use the ``tab`` key to indent code that is part of a block.
+
+"For loops" are our first example of this. The code block that is controlled
+by the for loop is indented by 4 spaces. In Python when you write a for
+statement it always expects the next line to be indented. If you have multiple
+lines inside of your for loop they must all be indented by the same amount.
+
+In the later example you will see a for loop inside a for loop. In this case
+the inner loop is indented by 8 spaces (4 spaces more than the outer loop).
+
+.. note::
+
+    It is important to remember that spaces are significant in Python code.
+    This can occasionally cause problems if you are copying and pasting code
+    between a web page and a text editor.
+
 For Loops
 ---------
 
 For loops provide the mechanism to repeat a block of code a number of times.
 Try the following code in iPython, note that the second line
 is indented by 4 spaces, you can use the ``tab`` key to do this indent.
 
 .. code-block:: python
 
     for i in range(10):
         print("hello")
         print(i)
 
 The ``range`` function creates a list of numbers from 0 to 9 (i.e. it starts
-at 0 and does 10 numbers). 
+at 0 and does 10 numbers).
 
-Then ``for`` loops through those numbers. For 
-each of them it sets the variable ``i`` equal to the current number in the range 
+Then ``for`` loops through those numbers. For
+each of them it sets the variable ``i`` equal to the current number in the range
 and then executes the code block.
 
-An important concept in Python is that a block of code is declared by 
-indenting it (usually by 4 spaces). 
+An important concept in Python is that a block of code is declared by
+indenting it (usually by 4 spaces).
 
 Thus the two print functions above are inside of the block controlled
 by the for loop. This is why both of those print functions get called 10
-times each. 
+times each.
 
 The ``print()`` function simply outputs values to the terminal.
 
 .. note::
 
-    In the above code we used a ``string`` of characters which was the word 
+    In the above code we used a ``string`` of characters which was the word
     "hello". Python variables with this type of data are called ``str`` and
     you can make strings by enclosing your text in quotes as we did above
     for "hello".
 
 Nested Loops
 ------------
 
@@ -68,45 +88,45 @@
     for i in range(3):
         print("i is ", i)
         for j in range(3):
             print("    j is ", j)
             print("    j times i is ", j * i)
 
 This is two loops inside of each other, each loops 3 times and so the total
-number of times the code block is executed is 3 times 3 = 9. 
+number of times the code block is executed is 3 times 3 = 9.
 
 Exercise:
     Try executing the above nested loop in **iPython** and see if you can
     work out why the output looks like it does.
 
 .. note::
-    
+
     We used a new operator here. The ``*`` operator is used to multiply two
-    numbers together. It is just the same as multiplication in basic 
-    arithmetic. 
-    
+    numbers together. It is just the same as multiplication in basic
+    arithmetic.
+
     Most computer languages use the star symbol to signify
-    multiplication. This is because there is no multiply symbol on 
+    multiplication. This is because there is no multiply symbol on
     computer keyboards since they evolved from typewriter keyboards!
 
     Similarly the symbol ``/`` is used to represent "divide by".
 
-    The picture below is the advanced IBM 'Selectric' typewriter that came 
-    out in 1961. At this point IBM did not think that people needed 
-    mathematical symbols on their keyboards. As computers took over in the 
+    The picture below is the advanced IBM 'Selectric' typewriter that came
+    out in 1961. At this point IBM did not think that people needed
+    mathematical symbols on their keyboards. As computers took over in the
     next few decades they just copied the same layout.
 
     .. figure:: ../images/typewriter.jpg
         :alt: nether portal
         :width: 500px
         :align: center
 
         IBM Selectric typewriter 1961
 
-    In case you don't know, typewriters printed what you typed directly to 
+    In case you don't know, typewriters printed what you typed directly to
     paper and did not save it! Imagine that!
 
 .. _portal:
 
 Nether Portal
 -------------
 
@@ -122,74 +142,74 @@
     for x in range(4):
         # bottom row
         world.set_block(pos + Direction.EAST * x, Item.OBSIDIAN)
         # top row
         world.set_block(pos + Direction.EAST * x + Direction.UP * 4 , Item.OBSIDIAN)
 
     for y in range(4):
-        # left side 
+        # left side
         world.set_block(pos + Direction.UP * y, Item.OBSIDIAN)
-        # top row
+        # right side
         world.set_block(pos + Direction.UP * y + Direction.EAST * 3 , Item.OBSIDIAN)
 
     c = get_client()
     c.give("@a", Item.FLINT_AND_STEEL)
 
 .. image:: ../images/portal.png
     :alt: nether portal
     :width: 500px
     :align: center
 
-The most important thing to note here is that I used multiplication on the 
+The most important thing to note here is that I used multiplication on the
 Direction values to add them multiple times to a starting position. This means
 that:
 
 .. code-block:: python
 
     # bottom row
     world.set_block(pos + Direction.EAST * x, Item.OBSIDIAN)
 
-places an obsidian block at the position offset from ``pos`` in an Easterly 
-direction. How much it is offset is determined by the value of ``x``. We know 
+places an obsidian block at the position offset from ``pos`` in an Easterly
+direction. How much it is offset is determined by the value of ``x``. We know
 that the for loop is looping over values of ``x`` from 0 to 3. So we have::
 
     Loop 1 with x = 0
         set block at pos
     Loop 2 with x = 1
         set block at 1 step EAST from pos
     Loop 3 with x = 2
         set block at 2 steps EAST from pos
     Loop 4 with x = 3
         set block at 3 steps EAST from pos
 
-For the top row we do the same thing but also add 4 steps upwards. The 
+For the top row we do the same thing but also add 4 steps upwards. The
 loop over ``y`` does a similar thing for the two sides of the portal.
 
 Exercise:
     See if you can experiment with creating different sizes of nether portals.
-    Maybe you can create other shapes? If you used a nested loop you could make 
+    Maybe you can create other shapes? If you used a nested loop you could make
     steps for example?
 
 .. _comments:
 
 Comments
 --------
 
 Some of the lines in the above code example are comments. In Python we
-precede comments with ``#``. This instructs Python to ignore the rest of 
+precede comments with ``#``. This instructs Python to ignore the rest of
 the line.
 
 Comments do not change the behaviour of the code, rather they help you
-understand what the code is supposed to do. Good programmers always 
+understand what the code is supposed to do. Good programmers always
 comment their code, especially when they are doing something that may
 not be immediately easy to understand.
 
 Flint and Steel
 ---------------
 
-Did you notice the ``get_client`` and ``c.give()`` at the end of the code 
-snippet? This handed a Flint and Steel to every player in the world. 
+Did you notice the ``get_client`` and ``c.give()`` at the end of the code
+snippet? This handed a Flint and Steel to every player in the world.
 You can equip this in your hand and ignite
 your portal by left clicking in the interior of the portal. It should then
 look like my picture above and you can jump through to see the Nether.
 
 For an advanced, in-depth description of the use of ``get_client()`` see `mcipc`
```

### Comparing `mciwb-0.8.5/docs/user/tutorials/05-functions.rst` & `mciwb-0.8.6/docs/user/tutorials/05-functions.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/tutorials/05a-modules.rst` & `mciwb-0.8.6/docs/user/tutorials/05a-modules.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/docs/user/tutorials/06-if-then.rst` & `mciwb-0.8.6/docs/user/tutorials/06-if-then.rst`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/pyproject.toml` & `mciwb-0.8.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 description = "Minecraft Interactive world builder"
 dependencies = [
     "numpy==1.23.5",
     "typer==0.7.0",
     "mcwb>=0.2.3",
     "ipython==8.10.0",
-    "docker==5.0.3",
+    "docker>=6",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
@@ -30,14 +30,15 @@
     "flake8-isort",
     "Flake8-pyproject",
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
     "pytest",
     "pytest-cov",
+    "sphinx<7",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
     "tox-direct",
     "types-mock",
 ]
```

### Comparing `mciwb-0.8.5/src/demo/arrows.py` & `mciwb-0.8.6/src/demo/arrows.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/background.py` & `mciwb-0.8.6/src/demo/background.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/example2player.py` & `mciwb-0.8.6/src/demo/example2player.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/gate.py` & `mciwb-0.8.6/src/demo/gate.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/gateway.py` & `mciwb-0.8.6/src/demo/gateway.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/house.py` & `mciwb-0.8.6/src/demo/house.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/pagoda.py` & `mciwb-0.8.6/src/demo/pagoda.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/snowball.py` & `mciwb-0.8.6/src/demo/snowball.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/village.py` & `mciwb-0.8.6/src/demo/village.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/demo/walls.py` & `mciwb-0.8.6/src/demo/walls.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/__main__.py` & `mciwb-0.8.6/src/mciwb/__main__.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/backup.py` & `mciwb-0.8.6/src/mciwb/backup.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/copier.py` & `mciwb-0.8.6/src/mciwb/copier.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/imports.py` & `mciwb-0.8.6/src/mciwb/imports.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/iwb.py` & `mciwb-0.8.6/src/mciwb/iwb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
 from mcipc.rcon.exceptions import NoPlayerFound
 from mcipc.rcon.item import Item
 from mcipc.rcon.je import Client
 from mcwb import Anchor3, Blocks, Direction, Vec3, Volume
 from mcwb.itemlists import grab, load_items, save_items
 from rcon.exceptions import SessionTimeout
@@ -13,14 +13,15 @@
 from mciwb.copier import CopyPaste
 from mciwb.logging import init_logging, log
 from mciwb.monitor import Monitor
 from mciwb.player import Player, PlayerNotInWorld
 from mciwb.server import HOST, def_port
 from mciwb.signs import Signs
 from mciwb.threads import get_client, set_client
+from mciwb.utils import Utils
 
 world: "Iwb" = None  # type: ignore
 
 
 def get_world():
     return Iwb.the_world
 
@@ -45,14 +46,15 @@
         :param port: the server port
         :param passwd: the server password
 
         :raises SessionTimeout: if the connection to the server fails
 
         """
         Iwb.the_world = self
+        self.utils = Utils(self)
 
         self._server: str = server
         self._port: int = port
         self._passwd: str = passwd
 
         self.connect()
 
@@ -70,21 +72,25 @@
         else:
             self._backup = None
 
     def debug(self, enable: bool = True):
         """
         Enable/disable debug log. Enabling this will also enable
         full Traceback log.
+
+        :param enable: True to enable debug log, False to disable
         """
         init_logging(debug=enable)
 
     def backup(self, name=None) -> None:
         """
         Backup the Minecraft world to a file. If no name is given then the
         backup will be named using the current date and time.
+
+        :param name: the name of the backup file
         """
         if self._backup is None:
             log.warning("no backup available")
         else:
             self._backup.backup(name=name)
 
     def connect(self) -> Client:
@@ -101,27 +107,45 @@
 
         log.info(f"Connected to {self._server} on {self._port}")
         # don't announce every rcon command
         client.gamerule("sendCommandFeedback", False)
 
         return client
 
+    def get_player(self, name: str) -> Player:
+        """
+        Get the player object for the given player name.
+
+        :param name: the name of the player
+        """
+        return self._players[name]
+
+    @property
+    def players(self) -> List[str]:
+        """
+        Get a list of the names of players being monitored.
+        """
+        return list(self._players.keys())
+
     def add_player(self, name: str, me=True):
         """
         Add a player to the world object. This provides monitoring of the
         player's position and handles the player's placing of action signs.
 
         If me is True then the player will be set as the current default
         player. The default player is available using::
 
             Iwb.the_world.player
 
         All players are available using::
 
             Iwb.the_world._players
+
+        :param name: the name of the player
+        :param me: if True, set this player as the default player
         """
         try:
             player = Player(name)
             self._players[name] = player
 
             self.signs = Signs(player)
             Monitor(self.signs._poll, name=name)
@@ -137,23 +161,44 @@
             log.error("failed to give signs to player, %s", e)
 
         log.info(f"Monitoring player {name} enabled for sign commands")
 
     def stop(self):
         Monitor.stop_all()
 
-    def set_block(self, pos: Vec3, block: Item, facing: Optional[Vec3] = None):
+    def set_block(
+        self,
+        pos: Vec3,
+        block: Item,
+        facing: Optional[Vec3] = None,
+        nbt: Optional[List[str]] = None,
+    ):
         """
-        Sets a block in the world
+        Places a block in the world
+
+        :param pos: the position to place the block
+        :param block: the type of block
+        :param facing: the direction the block should face (if applicable)
+        :param nbt: a list of NBT tags to apply to the block
+
+        nbt examples:
+
+        Placing a top half of a door, open, with hinge on the left:
+
+        nbt=["half=upper", "hinge=left", "open=true"]
+
+        TODO at present the nbt are free form strings. In the spirit of mcwb
+        we should provide a set of types that represent the NBT tags and
+        provide a way to convert them to strings (but that is a large task)
         """
         client = get_client()
 
         pos = Vec3(*pos)
         int_pos = pos.with_ints()
-        nbt = []
+        nbt = nbt or []
 
         if facing:
             nbt.append(f"""facing={Direction.name(facing)}""")
         block_str = f"""{block}[{",".join(nbt)}]"""
 
         result = client.setblock(int_pos, block_str)
         log.debug("setblock: " + result)
@@ -163,14 +208,16 @@
             x in result for x in ["Changed the block", "Could not set the block", ""]
         ):
             log.error(result)
 
     def get_block(self, pos: Vec3) -> Item:
         """
         Gets a block in the world
+
+        :param pos: the position to get the block from
         """
         client = get_client()
 
         int_pos = Vec3(*pos).with_ints()
 
         grab_volume = Volume.from_corners(int_pos, int_pos)
         blocks = grab(client, grab_volume)
@@ -182,29 +229,37 @@
         if self.copier is not None:
             report += (
                 "  copy buffer start: {o.copier.start_pos}\n"
                 "  copy buffer stop: {o.copier.stop_pos}\n"
                 "  copy buffer size: {o.copier.size}\n"
                 "  paste point: {o.copier.paste_pos}\n"
             )
-        if self.player is not None:
+        for name, player in self._players.items():
             report += (
-                "  player: {o.player.name}\n"
-                "  player position: {o.player.pos}\n"
-                "  player facing: {o.player.facing}\n"
+                f"  player: {name}\n"
+                f"    position: {player.pos}\n"
+                f"    facing: {player.facing}\n"
             )
-        else:
-            report += "  no player selected\n"
+        if len(self._players.items()) == 0:
+            report += "  no players\n"
 
         return report.format(o=self)
 
     def save(self, filename: str, vol: Optional[Volume] = None):
         """
         Save a Volume of blocks to a file. The volume can be specified in
         the *vol* parameter or alternatively defaults to the current copy buffer.
+
+        The file is saved in the mcwb format which is a JSON file containing
+        a 3d array of Item objects.
+
+        The file can be loaded into a world using the `load` method.
+
+        :param filename: the name of the file to save to
+        :param vol: the volume to save
         """
         if not vol:
             vol = self.copier.to_volume()
 
         blocks = grab(get_client(), vol)
         save_items(blocks, Path(filename))
 
@@ -214,14 +269,23 @@
         position: Optional[Vec3] = None,
         anchor: Anchor3 = Anchor3.BOTTOM_SW,
     ):
         """
         Load a saved set of blocks into a location. The location can be
         specified in argument *position* or alternatively defaults
         to the copy buffer start position.
+
+        The blocks are loaded from a file in the mcwb format which is a
+        JSON file containing a 3d array of Item objects.
+
+        The blocks are loaded into the world using the Blocks class.
+
+        :param filename: the name of the file to load from
+        :param position: the position to load the blocks to
+        :param anchor: the anchor point for the blocks
         """
         if not position:
             position = self.copier.start_pos
 
         # load a 3d array of Item from the file
         items = load_items(Path(filename), dimensions=3)
         # convert the items into a Blocks object which renders them in the world
@@ -229,14 +293,16 @@
 
         if self.copier:
             self.copier.apply_volume(blocks.volume)
 
     def cmd(self, cmd: str) -> str:
         """
         Run any arbitrary Minecraft console command on the server.
+
+        :param cmd: the command to run
         """
         encoding = "utf-8"
         client = get_client()
         request = Packet.make_command(cmd, encoding=encoding)
 
         response = client.communicate(request)
         if response.id != request.id:
```

### Comparing `mciwb-0.8.5/src/mciwb/logging.py` & `mciwb-0.8.6/src/mciwb/logging.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/monitor.py` & `mciwb-0.8.6/src/mciwb/monitor.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/nbt.py` & `mciwb-0.8.6/src/mciwb/nbt.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/player.py` & `mciwb-0.8.6/src/mciwb/player.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/server.py` & `mciwb-0.8.6/src/mciwb/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.backup_folder = backup_folder or backup_folder_default
         self.world = self.server_folder / "world"
         self.world_type = world_type
         self.container = None
         self.keep = keep
         self.test = test
 
-    def wait_server(self):
+    def wait_server(self: "MinecraftServer"):
         """
         Wait until the server is ready to accept rcon connections
         """
 
         start_time: datetime = datetime.now()
         timeout = 200
```

### Comparing `mciwb-0.8.5/src/mciwb/signs.py` & `mciwb-0.8.6/src/mciwb/signs.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/switch.py` & `mciwb-0.8.6/src/mciwb/switch.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/threads.py` & `mciwb-0.8.6/src/mciwb/threads.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb/wall.py` & `mciwb-0.8.6/src/mciwb/wall.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/src/mciwb.egg-info/PKG-INFO` & `mciwb-0.8.6/src/mciwb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciwb
-Version: 0.8.5
+Version: 0.8.6
 Summary: Minecraft Interactive world builder
 Author-email: Firstname Lastname <email@address.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -222,14 +222,18 @@
 ===================================
 
 This project is intended as a fun way to learn the Python Programming Language.
 
 Experienced Python programmers can also use this library to create
 Minecraft worlds with interactive Python features.
 
+
+For the Reddit discussion see  
+`HERE <https://www.reddit.com/r/Minecraftbuilds/comments/11rqauh/build_things_using_python>`_
+
 Quick Start
 -----------
 
 To get started learning Python, see
 `Introduction <https://gilesknap.github.io/mciwb/main/user/tutorials/00-prereq.html>`_
 
 For existing Python developers, see
@@ -237,20 +241,22 @@
 
 Example Build
 -------------
 
 The pagoda and castle with working portcullis were all created programmatically
 with Python and the current version of MCIWB.
 
+
 .. figure:: https://gilesknap.github.io/mciwb/main/_images/castle.png
    :alt: castle
    :align: center
    :width: 600px
-
-   Example Build
+   :target: https://photos.app.goo.gl/utFt6KadWbdabR8x6
+   
+   Example Build - **Click for Video**
 
 Goals
 -----
 
 Minecraft Interactive World Builder's goals are:
 
  - Use Python to create anything inside of Minecraft worlds.
```

### Comparing `mciwb-0.8.5/src/mciwb.egg-info/SOURCES.txt` & `mciwb-0.8.6/src/mciwb.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
 README.rst
 pyproject.toml
 run-tests.sh
 todo.md
+video.md
 .devcontainer/devcontainer.json
 .github/CONTRIBUTING.rst
 .github/dependabot.yml
 .github/actions/install_requirements/action.yml
 .github/pages/index.html
 .github/pages/make_switcher.py
 .github/workflows/code.yml
@@ -42,14 +43,15 @@
 docs/developer/reference/contributing.rst
 docs/developer/reference/standards.rst
 docs/developer/tutorials/dev-install.rst
 docs/images/logo.png
 docs/user/index.rst
 docs/user/explanations/coordinates.rst
 docs/user/explanations/docs-structure.rst
+docs/user/explanations/mcee.rst
 docs/user/explanations/mcipc.rst
 docs/user/explanations/scope.rst
 docs/user/explanations/server-config.rst
 docs/user/how-to/backup.rst
 docs/user/how-to/completion.rst
 docs/user/how-to/coordinates.rst
 docs/user/how-to/extensions.rst
@@ -87,14 +89,18 @@
 docs/user/tutorials/04-loops.rst
 docs/user/tutorials/05-functions.rst
 docs/user/tutorials/05a-modules.rst
 docs/user/tutorials/06-if-then.rst
 docs/user/tutorials/07-lists.rst
 docs/user/tutorials/08-classes.rst
 docs/user/tutorials/09-dictionaries.rst
+docs/user/tutorials/10-threading.rst
+docs/user/tutorials/11-switches.rst
+docs/user/tutorials/12-signs.rst
+docs/user/tutorials/13-structures.rst
 src/demo/__init__.py
 src/demo/arrows.py
 src/demo/background.py
 src/demo/bat.py
 src/demo/clear.py
 src/demo/example2player.py
 src/demo/follow.py
@@ -117,14 +123,15 @@
 src/mciwb/monitor.py
 src/mciwb/nbt.py
 src/mciwb/player.py
 src/mciwb/server.py
 src/mciwb/signs.py
 src/mciwb/switch.py
 src/mciwb/threads.py
+src/mciwb/utils.py
 src/mciwb/wall.py
 src/mciwb.egg-info/PKG-INFO
 src/mciwb.egg-info/SOURCES.txt
 src/mciwb.egg-info/dependency_links.txt
 src/mciwb.egg-info/entry_points.txt
 src/mciwb.egg-info/requires.txt
 src/mciwb.egg-info/top_level.txt
```

### Comparing `mciwb-0.8.5/tests/conftest.py` & `mciwb-0.8.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/tests/cube.py` & `mciwb-0.8.6/tests/cube.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/tests/mockclient.py` & `mciwb-0.8.6/tests/mockclient.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/tests/mockplayer.py` & `mciwb-0.8.6/tests/mockplayer.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/tests/test_system/test_cli.py` & `mciwb-0.8.6/tests/test_system/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def test_repr(tmp_path: Path, minecraft_container, minecraft_client, minecraft_player):
     """launch the cli in test mode and connect to the test server"""
     result = run_cli(
         "shell", "--test", "--server", HOST, "--port", RCON_PORT, "--passwd", RCON_P
     )
 
-    assert "no player selected" in result.stdout
+    assert "no players" in result.stdout
 
     result = run_cli(
         "shell",
         "--test",
         "--server",
         HOST,
         "--port",
```

### Comparing `mciwb-0.8.5/tests/test_system/test_poly.py` & `mciwb-0.8.6/tests/test_system/test_poly.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/tests/test_system/test_world.py` & `mciwb-0.8.6/tests/test_system/test_world.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/tests/test_unit/test_copier.py` & `mciwb-0.8.6/tests/test_unit/test_copier.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/tests/test_unit/test_monitor.py` & `mciwb-0.8.6/tests/test_unit/test_monitor.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/tests/test_unit/test_player.py` & `mciwb-0.8.6/tests/test_unit/test_player.py`

 * *Files identical despite different names*

### Comparing `mciwb-0.8.5/todo.md` & `mciwb-0.8.6/todo.md`

 * *Files identical despite different names*

