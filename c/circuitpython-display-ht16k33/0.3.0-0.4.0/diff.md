# Comparing `tmp/circuitpython-display_ht16k33-0.3.0.tar.gz` & `tmp/circuitpython-display_ht16k33-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-display_ht16k33-0.3.0.tar", last modified: Sun May 28 20:33:51 2023, max compression
+gzip compressed data, was "circuitpython-display_ht16k33-0.4.0.tar", last modified: Wed May 31 19:32:33 2023, max compression
```

## Comparing `circuitpython-display_ht16k33-0.3.0.tar` & `circuitpython-display_ht16k33-0.4.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:51.477272 circuitpython-display_ht16k33-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:51.469272 circuitpython-display_ht16k33-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:51.473272 circuitpython-display_ht16k33-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-28 20:33:51.477272 circuitpython-display_ht16k33-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:51.473272 circuitpython-display_ht16k33-0.3.0/circuitpython_display_ht16k33.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-28 20:33:51.000000 circuitpython-display_ht16k33-0.3.0/circuitpython_display_ht16k33.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-28 20:33:51.000000 circuitpython-display_ht16k33-0.3.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 20:33:51.000000 circuitpython-display_ht16k33-0.3.0/circuitpython_display_ht16k33.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 20:33:51.000000 circuitpython-display_ht16k33-0.3.0/circuitpython_display_ht16k33.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 20:33:51.000000 circuitpython-display_ht16k33-0.3.0/circuitpython_display_ht16k33.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:51.473272 circuitpython-display_ht16k33-0.3.0/display_ht16k33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/display_ht16k33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/display_ht16k33/ht16k33.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/display_ht16k33/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    23170 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/display_ht16k33/segments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:51.477272 circuitpython-display_ht16k33-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/7mwahe.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:51.477272 circuitpython-display_ht16k33-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38124 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/docs/segments.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:33:51.477272 circuitpython-display_ht16k33-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_segments_14x4.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_segments_count_down.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_segments_custom_chars.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_segments_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-28 20:33:44.000000 circuitpython-display_ht16k33-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 20:33:34.000000 circuitpython-display_ht16k33-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 20:33:51.477272 circuitpython-display_ht16k33-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.544212 circuitpython-display_ht16k33-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.552212 circuitpython-display_ht16k33-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.552212 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.552212 circuitpython-display_ht16k33-0.4.0/display_ht16k33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/display_ht16k33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/display_ht16k33/ht16k33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/display_ht16k33/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/display_ht16k33/segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.556212 circuitpython-display_ht16k33-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/7mwahe.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48491 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/segments.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_advanced_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_14x4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_count_down.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_custom_chars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_marquee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/setup.cfg
```

### Comparing `circuitpython-display_ht16k33-0.3.0/.github/workflows/build.yml` & `circuitpython-display_ht16k33-0.4.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/.github/workflows/release_gh.yml` & `circuitpython-display_ht16k33-0.4.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/.gitignore` & `circuitpython-display_ht16k33-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/.pre-commit-config.yaml` & `circuitpython-display_ht16k33-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/.pylintrc` & `circuitpython-display_ht16k33-0.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/LICENSE` & `circuitpython-display_ht16k33-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/PKG-INFO` & `circuitpython-display_ht16k33-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-display_ht16k33
-Version: 0.3.0
+Version: 0.4.0
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -41,15 +41,15 @@
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/7mwahe.gif
 
-Also work with segments with a very similar sintax to the Adafruit Segments library
+Also work with segments 7x4 and 14x4 with a very similar syntax to the Adafruit Segments library
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/segments.jpg
 
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython-display_ht16k33-0.3.0/README.rst` & `circuitpython-display_ht16k33-0.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/7mwahe.gif
 
-Also work with segments with a very similar sintax to the Adafruit Segments library
+Also work with segments 7x4 and 14x4 with a very similar syntax to the Adafruit Segments library
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/segments.jpg
 
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython-display_ht16k33-0.3.0/circuitpython_display_ht16k33.egg-info/PKG-INFO` & `circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-display-ht16k33
-Version: 0.3.0
+Version: 0.4.0
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -41,15 +41,15 @@
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/7mwahe.gif
 
-Also work with segments with a very similar sintax to the Adafruit Segments library
+Also work with segments 7x4 and 14x4 with a very similar syntax to the Adafruit Segments library
 
 .. image:: https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33/blob/master/docs/segments.jpg
 
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython-display_ht16k33-0.3.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt` & `circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,13 +29,15 @@
 docs/segments.jpg
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/display_ht16k33_advanced_example.py
 examples/display_ht16k33_segments_14x4.py
 examples/display_ht16k33_segments_count_down.py
 examples/display_ht16k33_segments_custom_chars.py
+examples/display_ht16k33_segments_marquee.py
 examples/display_ht16k33_segments_simpletest.py
 examples/display_ht16k33_simpletest.py
 examples/display_ht16k33_text.py
```

### Comparing `circuitpython-display_ht16k33-0.3.0/display_ht16k33/ht16k33.py` & `circuitpython-display_ht16k33-0.4.0/display_ht16k33/ht16k33.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """
 from vectorio import Circle
 import displayio
 import ulab.numpy as np
 
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
 # pylint: disable=too-many-arguments, too-many-instance-attributes
 class HT16K33:
     """
     Main class
```

### Comparing `circuitpython-display_ht16k33-0.3.0/display_ht16k33/matrix.py` & `circuitpython-display_ht16k33-0.4.0/display_ht16k33/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from typing import Optional, Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
 class Matrix8x8(HT16K33):
     """A single matrix."""
 
     def __init__(self, x, y, radius, text):
```

### Comparing `circuitpython-display_ht16k33-0.3.0/docs/7mwahe.gif` & `circuitpython-display_ht16k33-0.4.0/docs/7mwahe.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/docs/_static/Logo.png` & `circuitpython-display_ht16k33-0.4.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/docs/_static/favicon.ico` & `circuitpython-display_ht16k33-0.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/docs/conf.py` & `circuitpython-display_ht16k33-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/docs/font5x8.bin` & `circuitpython-display_ht16k33-0.4.0/docs/font5x8.bin`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_segments_custom_chars.py` & `circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_custom_chars.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_simpletest.py` & `circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/examples/display_ht16k33_text.py` & `circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_text.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.3.0/pyproject.toml` & `circuitpython-display_ht16k33-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-display_ht16k33"
 description = "On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices."
-version = "0.3.0"
+version = "0.4.0"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxxy@mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33"}
 keywords = [
     "sensor",
```

