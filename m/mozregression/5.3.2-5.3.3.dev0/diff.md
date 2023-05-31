# Comparing `tmp/mozregression-5.3.2.tar.gz` & `tmp/mozregression-5.3.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozregression-5.3.2.tar", last modified: Tue Feb 21 14:53:46 2023, max compression
+gzip compressed data, was "mozregression-5.3.3.dev0.tar", last modified: Wed May 31 15:16:27 2023, max compression
```

## Comparing `mozregression-5.3.2.tar` & `mozregression-5.3.3.dev0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:53:46.065837 mozregression-5.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-21 14:52:37.000000 mozregression-5.3.2/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:53:46.045837 mozregression-5.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-21 14:52:37.000000 mozregression-5.3.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:53:46.049837 mozregression-5.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-02-21 14:52:37.000000 mozregression-5.3.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-02-21 14:52:37.000000 mozregression-5.3.2/.github/workflows/compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-02-21 14:52:37.000000 mozregression-5.3.2/.github/workflows/deploy-gui.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-02-21 14:52:37.000000 mozregression-5.3.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-21 14:52:37.000000 mozregression-5.3.2/.github/workflows/glean-probe-scraper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-21 14:52:37.000000 mozregression-5.3.2/.github/workflows/run-compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-02-21 14:52:37.000000 mozregression-5.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-21 14:52:37.000000 mozregression-5.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-21 14:53:46.061838 mozregression-5.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-02-21 14:52:37.000000 mozregression-5.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:53:46.057838 mozregression-5.3.2/mozregression/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/approx_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/bisector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/build_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/fetch_build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/fetch_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/json_pushes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/mach_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/persist_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/pings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/tc_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-02-21 14:52:37.000000 mozregression-5.3.2/mozregression/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-21 14:53:45.000000 mozregression-5.3.2/mozregression/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:53:46.061838 mozregression-5.3.2/mozregression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-21 14:53:45.000000 mozregression-5.3.2/mozregression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-21 14:53:46.000000 mozregression-5.3.2/mozregression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 14:53:45.000000 mozregression-5.3.2/mozregression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-21 14:53:45.000000 mozregression-5.3.2/mozregression.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-21 14:53:45.000000 mozregression-5.3.2/mozregression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-21 14:53:45.000000 mozregression-5.3.2/mozregression.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-21 14:52:37.000000 mozregression-5.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 14:53:46.065837 mozregression-5.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-02-21 14:52:37.000000 mozregression-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:27.411188 mozregression-5.3.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:27.395187 mozregression-5.3.3.dev0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:27.399187 mozregression-5.3.3.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/.github/workflows/compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/.github/workflows/deploy-gui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/.github/workflows/glean-probe-scraper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/.github/workflows/run-compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 15:16:27.411188 mozregression-5.3.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:27.411188 mozregression-5.3.3.dev0/mozregression/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/approx_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/bisector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/build_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/fetch_build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/fetch_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/json_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/mach_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/persist_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/pings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/releases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/tc_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/mozregression/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-31 15:16:27.000000 mozregression-5.3.3.dev0/mozregression/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:16:27.411188 mozregression-5.3.3.dev0/mozregression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 15:16:27.000000 mozregression-5.3.3.dev0/mozregression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-31 15:16:27.000000 mozregression-5.3.3.dev0/mozregression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:16:27.000000 mozregression-5.3.3.dev0/mozregression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 15:16:27.000000 mozregression-5.3.3.dev0/mozregression.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-31 15:16:27.000000 mozregression-5.3.3.dev0/mozregression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 15:16:27.000000 mozregression-5.3.3.dev0/mozregression.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:16:27.411188 mozregression-5.3.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-31 15:15:32.000000 mozregression-5.3.3.dev0/setup.py
```

### Comparing `mozregression-5.3.2/.github/workflows/build.yml` & `mozregression-5.3.3.dev0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/.github/workflows/compile-requirements.yml` & `mozregression-5.3.3.dev0/.github/workflows/compile-requirements.yml`

 * *Files 4% similar despite different names*

```diff
@@ -75,8 +75,8 @@
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           git status
           git pull --rebase
           find temp-requirements -name "requirements-*" -type f -exec mv -f -t requirements {} +
           git add -A
           git commit -m "Automatically generated requirements"
-          git push -f https://x-access-token:${GITHUB_TOKEN}@github.com/${GITHUB_REPOSITORY}.git
+          until git push -f https://x-access-token:${GITHUB_TOKEN}@github.com/${GITHUB_REPOSITORY}.git; do git pull --rebase; done
```

### Comparing `mozregression-5.3.2/.github/workflows/deploy-gui.yml` & `mozregression-5.3.3.dev0/.github/workflows/deploy-gui.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/.github/workflows/deploy.yml` & `mozregression-5.3.3.dev0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/.github/workflows/run-compile-requirements.yml` & `mozregression-5.3.3.dev0/.github/workflows/run-compile-requirements.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,19 @@
     uses: ./.github/workflows/compile-requirements.yml
     with:
       requirements_files: '["base.in dev.in gui-dev.in gui.in linters.in"]'
       os: '["ubuntu-latest"]'
       python: '["3.7", "3.8", "3.9", "3.10", "3.11"]'
 
   call-compile-requirements-windows:
-    needs: call-compile-requirements-linux
     uses: ./.github/workflows/compile-requirements.yml
     with:
       requirements_files: '["base.in dev.in gui-dev.in gui.in linters.in"]'
       os: '["windows-latest"]'
       python: '["3.9", "3.10", "3.11"]'
 
   call-compile-requirements-macos:
-    needs: call-compile-requirements-windows
     uses: ./.github/workflows/compile-requirements.yml
     with:
       requirements_files: '["base.in dev.in gui-dev.in gui.in linters.in"]'
       os: '["macos-latest"]'
       python: '["3.9", "3.10", "3.11"]'
```

### Comparing `mozregression-5.3.2/LICENSE` & `mozregression-5.3.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/PKG-INFO` & `mozregression-5.3.3.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.3.2
+Version: 5.3.3.dev0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.3.2/README.md` & `mozregression-5.3.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/approx_persist.py` & `mozregression-5.3.3.dev0/mozregression/approx_persist.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/bisector.py` & `mozregression-5.3.3.dev0/mozregression/bisector.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/branches.py` & `mozregression-5.3.3.dev0/mozregression/branches.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/bugzilla.py` & `mozregression-5.3.3.dev0/mozregression/bugzilla.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/build_info.py` & `mozregression-5.3.3.dev0/mozregression/build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/build_range.py` & `mozregression-5.3.3.dev0/mozregression/build_range.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/class_registry.py` & `mozregression-5.3.3.dev0/mozregression/class_registry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/cli.py` & `mozregression-5.3.3.dev0/mozregression/cli.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/config.py` & `mozregression-5.3.3.dev0/mozregression/config.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/dates.py` & `mozregression-5.3.3.dev0/mozregression/dates.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/download_manager.py` & `mozregression-5.3.3.dev0/mozregression/download_manager.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/errors.py` & `mozregression-5.3.3.dev0/mozregression/errors.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/fetch_build_info.py` & `mozregression-5.3.3.dev0/mozregression/fetch_build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/fetch_configs.py` & `mozregression-5.3.3.dev0/mozregression/fetch_configs.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/history.py` & `mozregression-5.3.3.dev0/mozregression/history.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/json_pushes.py` & `mozregression-5.3.3.dev0/mozregression/json_pushes.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/launchers.py` & `mozregression-5.3.3.dev0/mozregression/launchers.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/log.py` & `mozregression-5.3.3.dev0/mozregression/log.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/mach_interface.py` & `mozregression-5.3.3.dev0/mozregression/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/main.py` & `mozregression-5.3.3.dev0/mozregression/main.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/metrics.yaml` & `mozregression-5.3.3.dev0/mozregression/metrics.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,81 +3,81 @@
 
 usage:
   variant:
     type: string
     description: >
       The variant of mozregression used to perform the bisection (gui,
       console, mach, etc.)
-    notification_emails: [wlachance@mozilla.com]
+    notification_emails: [zeid@mozilla.com]
     bugs:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1581647
     data_reviews:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1581647#c9
     expires: never
     send_in_pings:
       - usage
   app:
     type: string
     description: >
       The name of the app being used (firefox, gve, etc.)
-    notification_emails: [wlachance@mozilla.com]
+    notification_emails: [zeid@mozilla.com]
     bugs:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1581647
     data_reviews:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1581647#c9
     expires: never
     send_in_pings:
       - usage
   build_type:
     type: string
     description: >
       The build type being bisected (asan, debug, opt, pgo, shippable, ...)
-    notification_emails: [wlachance@mozilla.com]
+    notification_emails: [zeid@mozilla.com]
     bugs:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1651401
     data_reviews:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1651401#c5
     expires: never
     send_in_pings:
       - usage
   good_date:
     type: datetime
     time_unit: day
     description: >
       The good date parameter used in a bisection, if present and specified
       as a date
-    notification_emails: [wlachance@mozilla.com]
+    notification_emails: [zeid@mozilla.com]
     bugs:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1651401
     data_reviews:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1651401#c5
     expires: never
     send_in_pings:
       - usage
   bad_date:
     type: datetime
     time_unit: day
     description: >
       The bad date parameter used in a bisection, if present and specified as
       a date
-    notification_emails: [wlachance@mozilla.com]
+    notification_emails: [zeid@mozilla.com]
     bugs:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1651401
     data_reviews:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1651401#c5
     expires: never
     send_in_pings:
       - usage
   launch_date:
     type: datetime
     time_unit: day
     description: >
       The launch parameter used when running a single build, if present
       and specified as a date
-    notification_emails: [wlachance@mozilla.com]
+    notification_emails: [zeid@mozilla.com]
     bugs:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1651401
     data_reviews:
       - https://bugzilla.mozilla.org/show_bug.cgi?id=1651401#c5
     expires: never
     send_in_pings:
       - usage
```

### Comparing `mozregression-5.3.2/mozregression/network.py` & `mozregression-5.3.3.dev0/mozregression/network.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/persist_limit.py` & `mozregression-5.3.3.dev0/mozregression/persist_limit.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/pings.yaml` & `mozregression-5.3.3.dev0/mozregression/pings.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -9,12 +9,12 @@
     shared except in aggregated form. Although not a consumer product,
     mozregression strives to follow Mozilla's general guidelines on
     [lean data practices](https://www.mozilla.org/en-US/about/policy/lean-data/)
     and is also subject to Mozilla's
     [privacy policy](https://www.mozilla.org/en-US/privacy/websites/).
   include_client_id: true
   notification_emails:
-    - wlachance@mozilla.com
+    - zeid@mozilla.com
   bugs:
     - https://bugzilla.mozilla.org/show_bug.cgi?id=1581647
   data_reviews:
     - https://bugzilla.mozilla.org/show_bug.cgi?id=1581647#c9
```

### Comparing `mozregression-5.3.2/mozregression/releases.py` & `mozregression-5.3.3.dev0/mozregression/releases.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/tc_authenticate.py` & `mozregression-5.3.3.dev0/mozregression/tc_authenticate.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/telemetry.py` & `mozregression-5.3.3.dev0/mozregression/telemetry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/tempdir.py` & `mozregression-5.3.3.dev0/mozregression/tempdir.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression/test_runner.py` & `mozregression-5.3.3.dev0/mozregression/test_runner.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/mozregression.egg-info/PKG-INFO` & `mozregression-5.3.3.dev0/mozregression.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.3.2
+Version: 5.3.3.dev0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.3.2/mozregression.egg-info/SOURCES.txt` & `mozregression-5.3.3.dev0/mozregression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/pyproject.toml` & `mozregression-5.3.3.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozregression-5.3.2/setup.py` & `mozregression-5.3.3.dev0/setup.py`

 * *Files identical despite different names*

