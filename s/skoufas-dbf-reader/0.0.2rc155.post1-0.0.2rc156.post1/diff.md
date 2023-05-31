# Comparing `tmp/skoufas_dbf_reader-0.0.2rc155.post1.tar.gz` & `tmp/skoufas_dbf_reader-0.0.2rc156.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skoufas_dbf_reader-0.0.2rc155.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skoufas_dbf_reader-0.0.2rc156.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skoufas_dbf_reader-0.0.2rc155.post1.tar` & `skoufas_dbf_reader-0.0.2rc156.post1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      358 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2310 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       93 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.flake8
--rw-r--r--   0        0        0      239 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.github/dependabot.yml
--rw-r--r--   0        0        0     1552 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1521 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.github/workflows/jekyll-gh-pages.yml
--rw-r--r--   0        0        0      263 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1824 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.pypirc
--rw-r--r--   0        0        0      129 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.vscode/extensions.json
--rw-r--r--   0        0        0      127 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/.vscode/settings.json
--rw-r--r--   0        0        0    34523 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/LICENSE
--rw-r--r--   0        0        0     6247 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/README.md
--rw-r--r--   0        0        0     5747 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/pyproject.toml
--rw-r--r--   0        0        0       95 2023-05-31 17:41:30.685676 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/__init__.py
--rw-r--r--   0        0        0     4563 2023-05-31 17:41:27.713693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/correction_data.py
--rw-r--r--   0        0        0   678429 2023-05-31 17:41:27.717693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/author_corrections.yml
--rw-r--r--   0        0        0 17966201 2023-05-31 17:41:27.781693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/converted_entries.yml
--rw-r--r--   0        0        0   261526 2023-05-31 17:41:27.781693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
--rw-r--r--   0        0        0  6059317 2023-05-31 17:41:27.809693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/entries.yml
--rw-r--r--   0        0        0     2236 2023-05-31 17:41:27.809693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
--rw-r--r--   0        0        0     1492 2023-05-31 17:41:27.809693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
--rw-r--r--   0        0        0     1637 2023-05-31 17:41:27.809693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
--rw-r--r--   0        0        0     2149 2023-05-31 17:41:27.809693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
--rw-r--r--   0        0        0   133171 2023-05-31 17:41:27.809693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
--rw-r--r--   0        0        0    12404 2023-05-31 17:41:27.809693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
--rw-r--r--   0        0        0      493 2023-05-31 17:41:27.809693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
--rw-r--r--   0        0        0      440 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
--rw-r--r--   0        0        0     1816 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
--rw-r--r--   0        0        0    43006 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
--rw-r--r--   0        0        0     1081 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
--rw-r--r--   0        0        0    38584 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
--rw-r--r--   0        0        0      247 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
--rw-r--r--   0        0        0    24127 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
--rw-r--r--   0        0        0     6773 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/first_names.yml
--rw-r--r--   0        0        0       50 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/language_codes.yml
--rw-r--r--   0        0        0    65691 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
--rw-r--r--   0        0        0   107848 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
--rw-r--r--   0        0        0     1192 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
--rw-r--r--   0        0        0    21896 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/field_extractors.py
--rw-r--r--   0        0        0    26321 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/generate_reports.py
--rw-r--r--   0        0        0     6286 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/utilities.py
--rw-r--r--   0        0        0    18619 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/tests/test_field_extractors.py
--rw-r--r--   0        0        0    17733 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/tests/test_reports.py
--rw-r--r--   0        0        0     1173 2023-05-31 17:41:27.813693 skoufas_dbf_reader-0.0.2rc155.post1/tests/test_utilities.py
--rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.2rc155.post1/PKG-INFO
+-rw-r--r--   0        0        0      358 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2310 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       93 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.flake8
+-rw-r--r--   0        0        0      239 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1552 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1521 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.github/workflows/jekyll-gh-pages.yml
+-rw-r--r--   0        0        0      263 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1824 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.pypirc
+-rw-r--r--   0        0        0      129 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      127 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/.vscode/settings.json
+-rw-r--r--   0        0        0    34523 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/LICENSE
+-rw-r--r--   0        0        0     6247 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/README.md
+-rw-r--r--   0        0        0     5747 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-05-31 17:43:25.063128 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/__init__.py
+-rw-r--r--   0        0        0     4563 2023-05-31 17:43:22.159089 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/correction_data.py
+-rw-r--r--   0        0        0   678429 2023-05-31 17:43:22.163089 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/author_corrections.yml
+-rw-r--r--   0        0        0 17966201 2023-05-31 17:43:22.223090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/converted_entries.yml
+-rw-r--r--   0        0        0   261526 2023-05-31 17:43:22.223090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
+-rw-r--r--   0        0        0  6059317 2023-05-31 17:43:22.247090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/entries.yml
+-rw-r--r--   0        0        0     2236 2023-05-31 17:43:22.247090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
+-rw-r--r--   0        0        0     1492 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
+-rw-r--r--   0        0        0     1637 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
+-rw-r--r--   0        0        0     2149 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
+-rw-r--r--   0        0        0   133171 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
+-rw-r--r--   0        0        0    12404 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
+-rw-r--r--   0        0        0      493 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
+-rw-r--r--   0        0        0      440 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
+-rw-r--r--   0        0        0     1816 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
+-rw-r--r--   0        0        0    43006 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
+-rw-r--r--   0        0        0     1081 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
+-rw-r--r--   0        0        0    38584 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
+-rw-r--r--   0        0        0      247 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
+-rw-r--r--   0        0        0    24127 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
+-rw-r--r--   0        0        0     6773 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/first_names.yml
+-rw-r--r--   0        0        0       50 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/language_codes.yml
+-rw-r--r--   0        0        0    65691 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
+-rw-r--r--   0        0        0   107848 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
+-rw-r--r--   0        0        0     1192 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
+-rw-r--r--   0        0        0    21896 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/field_extractors.py
+-rw-r--r--   0        0        0    26326 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/generate_reports.py
+-rw-r--r--   0        0        0     6286 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/utilities.py
+-rw-r--r--   0        0        0    18619 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/tests/test_field_extractors.py
+-rw-r--r--   0        0        0    17733 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/tests/test_reports.py
+-rw-r--r--   0        0        0     1173 2023-05-31 17:43:22.251090 skoufas_dbf_reader-0.0.2rc156.post1/tests/test_utilities.py
+-rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.2rc156.post1/PKG-INFO
```

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/.devcontainer/devcontainer.json` & `skoufas_dbf_reader-0.0.2rc156.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/.github/workflows/CI.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/.github/workflows/jekyll-gh-pages.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/.github/workflows/jekyll-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/.gitignore` & `skoufas_dbf_reader-0.0.2rc156.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/.pre-commit-config.yaml` & `skoufas_dbf_reader-0.0.2rc156.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/LICENSE` & `skoufas_dbf_reader-0.0.2rc156.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/README.md` & `skoufas_dbf_reader-0.0.2rc156.post1/README.md`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/pyproject.toml` & `skoufas_dbf_reader-0.0.2rc156.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/correction_data.py` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/correction_data.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/author_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/author_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/converted_entries.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/converted_entries.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/editor_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/editor_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/entries.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/entries.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field04_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field04_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field05_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field05_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field06_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field06_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field07_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field07_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field08_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field08_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field09_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field09_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field16_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field16_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field17_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field17_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field18_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field18_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field19_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field19_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/field30_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/field30_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/first_names.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/first_names.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/topic_replacements.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/topic_replacements.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/data/translator_corrections.yml` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/data/translator_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/dbf_to_yaml.py` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/dbf_to_yaml.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/field_extractors.py` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/generate_reports.py` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/generate_reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         with open(
             os.path.join(reports_directory, "single-field", f"field_{i:02}.md"), "w", encoding="utf-8"
         ) as outfile:
             outfile.write(str(doc))
 
     doc = Document()
     doc.add_heading("Τιμές στις στήλες των καρτελών")
-    doc.add_unordered_list([Inline(f"Στήλη {i}", link=f"./field_{i:02}.html") for i in range(1, 31)])
+    doc.add_unordered_list([str(Inline(f"Στήλη {i}", link=f"./field_{i:02}.html")) for i in range(1, 31)])
     with open(os.path.join(reports_directory, "single-field", "index.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(doc))
 
 
 def report_single_extracted_fields(reports_directory: str):
     field_values: defaultdict[str, list[str | list[str]]] = defaultdict(list)
     for entry in all_entries():
```

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/src/skoufas_dbf_reader/utilities.py` & `skoufas_dbf_reader-0.0.2rc156.post1/src/skoufas_dbf_reader/utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/tests/test_field_extractors.py` & `skoufas_dbf_reader-0.0.2rc156.post1/tests/test_field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/tests/test_reports.py` & `skoufas_dbf_reader-0.0.2rc156.post1/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/tests/test_utilities.py` & `skoufas_dbf_reader-0.0.2rc156.post1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc155.post1/PKG-INFO` & `skoufas_dbf_reader-0.0.2rc156.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skoufas-dbf-reader
-Version: 0.0.2rc155.post1
+Version: 0.0.2rc156.post1
 Summary: Library for reading legacy DBF file with library data
 Author-email: Claudio Bantaloukas <rockreamer@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

