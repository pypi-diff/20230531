# Comparing `tmp/skoufas-dbf-reader-0.0.2rc140.post1.tar.gz` & `tmp/skoufas_dbf_reader-0.0.2rc152.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skoufas-dbf-reader-0.0.2rc140.post1.tar", last modified: Wed Apr  5 20:28:15 2023, max compression
+gzip compressed data, was "skoufas_dbf_reader-0.0.2rc152.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skoufas-dbf-reader-0.0.2rc140.post1.tar` & `skoufas_dbf_reader-0.0.2rc152.post1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      730 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2165 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       93 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.flake8
--rw-r--r--   0        0        0      239 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.github/dependabot.yml
--rw-r--r--   0        0        0     1554 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1521 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.github/workflows/jekyll-gh-pages.yml
--rw-r--r--   0        0        0      263 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1824 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.pypirc
--rw-r--r--   0        0        0      128 2023-04-05 20:28:11.715057 skoufas-dbf-reader-0.0.2rc140.post1/.vscode/extensions.json
--rw-r--r--   0        0        0      127 2023-04-05 20:28:11.719057 skoufas-dbf-reader-0.0.2rc140.post1/.vscode/settings.json
--rw-r--r--   0        0        0    34523 2023-04-05 20:28:11.719057 skoufas-dbf-reader-0.0.2rc140.post1/LICENSE
--rw-r--r--   0        0        0     6247 2023-04-05 20:28:11.719057 skoufas-dbf-reader-0.0.2rc140.post1/README.md
--rw-r--r--   0        0        0     5748 2023-04-05 20:28:11.719057 skoufas-dbf-reader-0.0.2rc140.post1/pyproject.toml
--rw-r--r--   0        0        0       95 2023-04-05 20:28:15.511208 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/__init__.py
--rw-r--r--   0        0        0     4563 2023-04-05 20:28:11.719057 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/correction_data.py
--rw-r--r--   0        0        0   678429 2023-04-05 20:28:11.723057 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/author_corrections.yml
--rw-r--r--   0        0        0 17749273 2023-04-05 20:28:11.787059 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/converted_entries.yml
--rw-r--r--   0        0        0   261526 2023-04-05 20:28:11.791060 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
--rw-r--r--   0        0        0  5982876 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/entries.yml
--rw-r--r--   0        0        0     2236 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
--rw-r--r--   0        0        0     1492 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
--rw-r--r--   0        0        0     1637 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
--rw-r--r--   0        0        0     2149 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
--rw-r--r--   0        0        0   133171 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
--rw-r--r--   0        0        0    12404 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
--rw-r--r--   0        0        0      493 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
--rw-r--r--   0        0        0      422 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
--rw-r--r--   0        0        0     1816 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
--rw-r--r--   0        0        0    43006 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
--rw-r--r--   0        0        0     1081 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
--rw-r--r--   0        0        0    38584 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
--rw-r--r--   0        0        0      247 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
--rw-r--r--   0        0        0    24127 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
--rw-r--r--   0        0        0     6773 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/first_names.yml
--rw-r--r--   0        0        0       50 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/language_codes.yml
--rw-r--r--   0        0        0    65691 2023-04-05 20:28:11.819061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
--rw-r--r--   0        0        0   107848 2023-04-05 20:28:11.823061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
--rw-r--r--   0        0        0     1156 2023-04-05 20:28:11.823061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
--rw-r--r--   0        0        0    21896 2023-04-05 20:28:11.823061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/field_extractors.py
--rw-r--r--   0        0        0    27306 2023-04-05 20:28:11.823061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/generate_reports.py
--rw-r--r--   0        0        0     6286 2023-04-05 20:28:11.823061 skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/utilities.py
--rw-r--r--   0        0        0    18619 2023-04-05 20:28:11.823061 skoufas-dbf-reader-0.0.2rc140.post1/tests/test_field_extractors.py
--rw-r--r--   0        0        0    17733 2023-04-05 20:28:11.823061 skoufas-dbf-reader-0.0.2rc140.post1/tests/test_reports.py
--rw-r--r--   0        0        0     1173 2023-04-05 20:28:11.823061 skoufas-dbf-reader-0.0.2rc140.post1/tests/test_utilities.py
--rw-r--r--   0        0        0     7953 1970-01-01 00:00:00.000000 skoufas-dbf-reader-0.0.2rc140.post1/PKG-INFO
+-rw-r--r--   0        0        0      358 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2310 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       93 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.flake8
+-rw-r--r--   0        0        0      239 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1552 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1521 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.github/workflows/jekyll-gh-pages.yml
+-rw-r--r--   0        0        0      263 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1824 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.pypirc
+-rw-r--r--   0        0        0      129 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      127 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/.vscode/settings.json
+-rw-r--r--   0        0        0    34523 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/LICENSE
+-rw-r--r--   0        0        0     6247 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/README.md
+-rw-r--r--   0        0        0     5747 2023-05-31 16:39:10.567448 skoufas_dbf_reader-0.0.2rc152.post1/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-05-31 16:39:13.663484 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/__init__.py
+-rw-r--r--   0        0        0     4563 2023-05-31 16:39:10.571447 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/correction_data.py
+-rw-r--r--   0        0        0   678429 2023-05-31 16:39:10.571447 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/author_corrections.yml
+-rw-r--r--   0        0        0 17966201 2023-05-31 16:39:10.631448 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/converted_entries.yml
+-rw-r--r--   0        0        0   261526 2023-05-31 16:39:10.635448 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
+-rw-r--r--   0        0        0  6059317 2023-05-31 16:39:10.659449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/entries.yml
+-rw-r--r--   0        0        0     2236 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
+-rw-r--r--   0        0        0     1492 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
+-rw-r--r--   0        0        0     1637 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
+-rw-r--r--   0        0        0     2149 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
+-rw-r--r--   0        0        0   133171 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
+-rw-r--r--   0        0        0    12404 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
+-rw-r--r--   0        0        0      493 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
+-rw-r--r--   0        0        0      440 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
+-rw-r--r--   0        0        0     1816 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
+-rw-r--r--   0        0        0    43006 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
+-rw-r--r--   0        0        0     1081 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
+-rw-r--r--   0        0        0    38584 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
+-rw-r--r--   0        0        0      247 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
+-rw-r--r--   0        0        0    24127 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
+-rw-r--r--   0        0        0     6773 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/first_names.yml
+-rw-r--r--   0        0        0       50 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/language_codes.yml
+-rw-r--r--   0        0        0    65691 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
+-rw-r--r--   0        0        0   107848 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
+-rw-r--r--   0        0        0     1192 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
+-rw-r--r--   0        0        0    21896 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/field_extractors.py
+-rw-r--r--   0        0        0    26171 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/generate_reports.py
+-rw-r--r--   0        0        0     6286 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/utilities.py
+-rw-r--r--   0        0        0    18619 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/tests/test_field_extractors.py
+-rw-r--r--   0        0        0    17733 2023-05-31 16:39:10.663449 skoufas_dbf_reader-0.0.2rc152.post1/tests/test_reports.py
+-rw-r--r--   0        0        0     1173 2023-05-31 16:39:10.667449 skoufas_dbf_reader-0.0.2rc152.post1/tests/test_utilities.py
+-rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.2rc152.post1/PKG-INFO
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/.devcontainer/devcontainer.json` & `skoufas_dbf_reader-0.0.2rc152.post1/.devcontainer/devcontainer.json`

 * *Files 24% similar despite different names*

```diff
@@ -4,63 +4,67 @@
 	"build": {
 		"context": "..",
 		"dockerfile": "Dockerfile",
 		"args": {
 			"XDG_RUNTIME_DIR": "${localEnv:XDG_RUNTIME_DIR}"
 		}
 	},
-	// Set *default* container specific settings.json values on container create.
-	"settings": {
-		"editor.trimAutoWhitespace": true,
-		"editor.formatOnSave": true,
-		"editor.formatOnPaste": true,
-		"files.trimTrailingWhitespace": true,
-		"files.autoSave": "onFocusChange",
-		"python.analysis.typeCheckingMode": "strict",
-		"python.defaultInterpreterPath": "/usr/local/bin/python",
-		"python.formatting.autopep8Path": "/usr/local/py-utils/bin/autopep8",
-		"python.formatting.blackPath": "/usr/local/py-utils/bin/black",
-		"python.formatting.blackArgs": [
-			"--config",
-			"pyproject.toml"
-		],
-		"python.formatting.provider": "black",
-		"python.formatting.yapfPath": "/usr/local/py-utils/bin/yapf",
-		"python.linting.enabled": true,
-		"python.linting.lintOnSave": true,
-		"python.linting.banditArgs": [
-			"--configfile",
-			"pyproject.toml"
-		],
-		"python.linting.banditEnabled": true,
-		"python.linting.banditPath": "/usr/local/py-utils/bin/bandit",
-		"python.linting.flake8Args": [
-			"--config",
-			".flake8"
-		],
-		"python.linting.flake8Enabled": true,
-		"python.linting.flake8Path": "/usr/local/py-utils/bin/flake8",
-		"python.linting.mypyEnabled": true,
-		"python.linting.mypyArgs": [
-			"--config-file",
-			".pyproject.toml"
-		],
-		"python.linting.mypyPath": "/usr/local/py-utils/bin/mypy",
-		"python.linting.pycodestylePath": "/usr/local/py-utils/bin/pycodestyle",
-		"python.linting.pydocstylePath": "/usr/local/py-utils/bin/pydocstyle",
-		"python.linting.pylintEnabled": true,
-		"python.linting.pylintPath": "/usr/local/py-utils/bin/pylint"
+	"customizations": {
+		"vscode": {
+			// Set *default* container specific settings.json values on container create.
+			"settings": {
+				"editor.trimAutoWhitespace": true,
+				"editor.formatOnSave": true,
+				"editor.formatOnPaste": true,
+				"files.trimTrailingWhitespace": true,
+				"files.autoSave": "onFocusChange",
+				"python.analysis.typeCheckingMode": "strict",
+				"python.defaultInterpreterPath": "/usr/local/bin/python",
+				"python.formatting.autopep8Path": "/usr/local/py-utils/bin/autopep8",
+				"python.formatting.blackPath": "/usr/local/py-utils/bin/black",
+				"python.formatting.blackArgs": [
+					"--config",
+					"pyproject.toml"
+				],
+				"python.formatting.provider": "black",
+				"python.formatting.yapfPath": "/usr/local/py-utils/bin/yapf",
+				"python.linting.enabled": true,
+				"python.linting.lintOnSave": true,
+				"python.linting.banditArgs": [
+					"--configfile",
+					"pyproject.toml"
+				],
+				"python.linting.banditEnabled": true,
+				"python.linting.banditPath": "/usr/local/py-utils/bin/bandit",
+				"python.linting.flake8Args": [
+					"--config",
+					".flake8"
+				],
+				"python.linting.flake8Enabled": true,
+				"python.linting.flake8Path": "/usr/local/py-utils/bin/flake8",
+				"python.linting.mypyEnabled": true,
+				"python.linting.mypyArgs": [
+					"--config-file",
+					".pyproject.toml"
+				],
+				"python.linting.mypyPath": "/usr/local/py-utils/bin/mypy",
+				"python.linting.pycodestylePath": "/usr/local/py-utils/bin/pycodestyle",
+				"python.linting.pydocstylePath": "/usr/local/py-utils/bin/pydocstyle",
+				"python.linting.pylintEnabled": true,
+				"python.linting.pylintPath": "/usr/local/py-utils/bin/pylint"
+			},
+			"extensions": [
+				"ms-python.python",
+				"ms-python.vscode-pylance",
+				"ms-python.pylint",
+				"ms-python.black-formatter",
+				"ms-vsliveshare.vsliveshare",
+				"ryanluker.vscode-coverage-gutters",
+				"bungcip.better-toml"
+			]
+		}
 	},
-	"extensions": [
-		"ms-python.python",
-		"ms-python.vscode-pylance",
-		"ms-python.pylint",
-		"ms-python.black-formatter",
-		"ms-vsliveshare.vsliveshare",
-		"ryanluker.vscode-coverage-gutters",
-		"bungcip.better-toml"
-	],
 	// Use 'postCreateCommand' to run commands after the container is created.
 	// "postCreateCommand": "python --version",
 	"remoteUser": "vscode",
 	"features": {}
-}
+}
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/.github/workflows/CI.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/.github/workflows/CI.yml`

 * *Files 0% similar despite different names*

```diff
@@ -49,8 +49,7 @@
 
       - name: Publish Release to PyPi
         uses: rockdreamer/pyaction@main
         if: ${{ github.event_name == 'release' }}
         with:
           pypi_publish: true
           pypi_password: ${{ secrets.PYPI_PASSWORD }}
-
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/.github/workflows/jekyll-gh-pages.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/.github/workflows/jekyll-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/.gitignore` & `skoufas_dbf_reader-0.0.2rc152.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/.pre-commit-config.yaml` & `skoufas_dbf_reader-0.0.2rc152.post1/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -20,28 +20,28 @@
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         args: ["-a", "from __future__ import annotations"]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args: [--py39-plus]
 
   - repo: https://github.com/hadialqattan/pycln
-    rev: v2.1.3
+    rev: v2.1.4
     hooks:
       - id: pycln
         args: [--config=pyproject.toml]
         stages: [manual]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/LICENSE` & `skoufas_dbf_reader-0.0.2rc152.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/README.md` & `skoufas_dbf_reader-0.0.2rc152.post1/README.md`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/pyproject.toml` & `skoufas_dbf_reader-0.0.2rc152.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.10"
 dynamic = ["version"]
 dependencies = [
     "dbfread==2.0.7",
-    "snakemd==0.15.0",
+    "snakemd==2.1.0",
     "PyYAML==6.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "bandit[toml]==1.7.5",
     "black==23.3.0",
@@ -32,18 +32,18 @@
     "flake8-bugbear==23.3.23",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8==6.0.0",
     "pre-commit==3.2.2",
     "pylint==2.17.2",
     "pylint_junit",
-    "pytest-cov==4.0.0",
+    "pytest-cov==4.1.0",
     "pytest-mock<3.10.1",
     "pytest-runner",
-    "pytest==7.2.2",
+    "pytest==7.3.1",
     "pytest-github-actions-annotate-failures",
     "shellcheck-py==0.9.0.2"
 ]
 
 [project.scripts]
 dbf-to-yaml = "skoufas_dbf_reader.dbf_to_yaml:main"
 generate-reports = "skoufas_dbf_reader.generate_reports:main"
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/correction_data.py` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/correction_data.py`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/author_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/author_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/converted_entries.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/converted_entries.yml`

 * *Files 0% similar despite different names*

```diff
@@ -773,15 +773,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 16
     1: ΑΛΕΞΙΟΥ,ΑΘΑΝΑΣΙΟΣ
     2: ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ
-    4: 938 ΑΛΕ
+    4: 938ΑΛΕ
     5: '2055'
     7: 15ΕΚΔ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 806Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΕΝΙΚΗ
@@ -1035,15 +1035,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 21
     1: ΑΜΑΝΤΟΣ,Ι.ΚΩΝΣΤΑΝΤΙΝΟΣ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΑΔΟΣ
     3: ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΤΟΥ 1071Μ.Χ
-    4: 938 ΑΜΑ
+    4: 938ΑΜΑ
     5: '1916'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 29ΙΣ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΟΤΗΤΑ-ΙΟ71Μ.Χ
@@ -1171,34 +1171,34 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 24
   authors:
-  - ΑΝΑΓΝΩΣΤΑΚΗΣ,ΗΛΙΑΣ
+  - ΙΕΡΟΜΟΝΑΧΟΥ,ΕΥΘΥΜΙΟΥ
   title: ΧΡΟΝΙΚΟ ΓΑΛΑΞΕΙΔΙΟΥ
-  dewey: 938.91 ΑΝΑ
+  dewey: 938.91 ΙΕΡ
   entry_numbers:
   - '1725'
   editor: ΑΚΡΙΤΑ // ΑΘΗΝΑ
   edition_year: 1985
   pages: 93
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΓΑΛΑΞΕΙΔΙ
   - ΧΡΟΝΙΚΟ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 24
-    1: ΑΝΑΓΝΩΣΤΑΚΗΣ,ΗΛΙΑΣ    .
+    1: ΙΕΡΟΜΟΝΑΧΟΥ,ΕΥΘΥΜΙΟΥ
     2: ΧΡΟΝΙΚΟ ΓΑΛΑΞΕΙΔΙΟΥ
-    4: 938.91 ΑΝΑ
+    4: 938.91ΙΕΡ
     5: '1725'
     8: ΑΚΡΙΤΑ
     9: ΑΘΗΝΑ
     10: '1985'
     11: 93Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΑΛΑΞΕΙΔΙ
     13: ΓΑΛΑΞΕΙΔΙ-ΧΡΟΝΙΚΟ
@@ -1595,15 +1595,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 32
     1: ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ ΕΜΜ
     2: ΕΛΛΗΝΙΣΜΟΣ ΚΑΙ ΔΗΜΟΚΡΑΤΙΑ
-    4: 938 ΑΝΤ
+    4: 938ΑΝΤ
     5: '2533'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1971'
     11: 607Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΗΜΟΚΡΑΤΙΑ
     13: ΕΛΛΗΝΙΣΜΟΣ
@@ -1647,15 +1647,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 33
     1: ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ ΕΜΜ
     2: Η ΕΠΑΡΧΙΑ
     3: ΕΛΛΑΔΑ ΔΕΝ ΕΙΝΑΙ ΜΟΝΑΧΑ Η ΑΘΗΝΑ
-    4: 938 ΑΝΤ
+    4: 938ΑΝΤ
     5: '2522'
     7: 2ΕΚΔ
     8: ΗΠΕΙΡΩΤΙΚΗ ΕΣΤΙΑ
     9: ΙΩΑΝΝΙΝΑ
     10: '1953'
     11: 184Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΡΧΙΑ
@@ -2424,15 +2424,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 48
     1: ΑΡΓΥΡΟΣ,ΣΠΥΡΙΔΩΝΟΣ
     2: Η ΠΕΙΡΑΤΕΙΑ ΑΠΟ ΤΟ 1500 Π.Χ ΕΩΣ ΤΟ 1860
-    4: 938 ΑΡΓ
+    4: 938ΑΡΓ
     5: '2319'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1956'
     11: 192Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΕΙΡΑΤΕΙΑ-1550Π.Χ-1860
     13: ΠΕΙΡΑΤΕΙΑ-1550Π.Χ-1860
@@ -2906,15 +2906,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 57
     1: ΑΣΤΡΙΝΟΣ,ΘΕΜΗΣ
     2: Η ΜΕΓΑΛΗ ΙΔΕΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-    4: 938 ΑΣΤ
+    4: 938ΑΣΤ
     5: '2484'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1945'
     11: 230Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΛΗ ΙΔΕΑ
     13: ΕΛΛΗΝΙΣΜΟΣ-ΜΕΛΑΛΗ ΙΔΕΑ
@@ -2959,15 +2959,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 58
     1: ΑΣΩΠΙΟΣ,ΕΙΡΗΝΑΙΟΣ Κ
     2: ΠΑΛΑΙΑ ΚΑΙ ΝΕΑ
-    4: 938 ΑΣΩ
+    4: 938ΑΣΩ
     5: '2102'
     8: ΣΑΚΕΛΛΑΡΙΟΥ
     9: ΑΘΗΝΑ
     10: '1903'
     11: 672Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΑΜΝΗΣΕΙΣ-1845
     13: ΙΤΑΛΙΑ-ΑΝΑΜΝΗΣΕΙΣ-1845
@@ -3589,15 +3589,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 70
     1: ΒΑΛΕΤΑΣ,Γ
     2: ΤΟ ΠΡΟΔΟΜΕΝΟ ΕΙΚΟΣΙΕΝΑ
-    4: 938.5 ΒΑΛ
+    4: 938.5ΒΑΛ
     5: '1845'
     7: 2ΕΚΔ
     8: ΦΙΛΙΠΠΟΤΗ
     9: ΑΘΗΝΑ
     10: '1979'
     11: 195Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΙΚΟΣΙΕΝΑ
@@ -5690,15 +5690,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 111
   authors:
   - ΒΕΝΙΖΕΛΟΣ,ΕΛΕΥΘΕΡΙΟΣ
   title: ΙΔΙΟΓΡΑΦΟΝ ΗΜΕΡΟΛΟΓΙΟ
-  dewey: 938.672 ΒΕΝ
+  dewey: 938.672 ΧΣ
   entry_numbers:
   - '2115'
   editor: None // ΧΑΝΙΑ
   edition_year: 1979
   pages: 57
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -5708,15 +5708,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 111
     1: ΒΕΝΙΖΕΛΟΣ,ΕΛΕΥΘΕΡΙΟΣ
     2: ΙΔΙΟΓΡΑΦΟΝ ΗΜΕΡΟΛΟΓΙΟ
-    4: 938.672ΒΕΝ
+    4: 938.672Χ.Σ
     5: '2115'
     8: Χ.Ε
     9: ΧΑΝΙΑ
     10: '1979'
     11: 57Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ-ΗΜΕΡΟΛΟΓΙΟ
     13: ΒΕΝΙΖΕΛΟΣ-ΗΜΕΡΟΛΟΓΙΟ
@@ -5738,17 +5738,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 112
   authors:
-  - ΒΕΝΙΖΕΛΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  - ΣΤΕΦΑΝΟΥ,Σ.Ι.
   title: ΠΟΛΙΤΙΚΑΙ ΥΠΟΘΗΚΑΙ
-  dewey: 938.672 ΒΕΝ
+  dewey: 938.672 ΣΤΕ
   entry_numbers:
   - '2391'
   - '2784'
   - '2785'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
   pages: 306
@@ -5758,17 +5758,17 @@
   - ΠΟΛΙΤΙΚΑΙ ΥΠΟΘΗΚΑΙ
   - ΠΟΛΙΤΙΚΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 112
-    1: ΒΕΝΙΖΕΛΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+    1: ΣΤΕΦΑΝΟΥ,Σ.Ι.
     2: ΠΟΛΙΤΙΚΑΙ ΥΠΟΘΗΚΑΙ
-    4: 938.672ΒΕΝ
+    4: 938.672ΣΤΕ
     5: 2391-2784-2785
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1965'
     11: 306Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ-ΠΟΛΙΤΙΚΑΙ ΥΠΟΘΗΚΑΙ
     13: ΒΕΝΙΖΕΛΟΣ-ΠΟΛΙΤΙΚΑΙ ΥΠΟΘΗΚΑΙ
@@ -5864,15 +5864,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 114
     1: ΒΕΡΕΜΗΣ,ΘΑΝΟΣ
     2: ΟΙ ΕΠΕΜΒΑΣΕΙΣ ΤΟΥ ΣΤΡΑΤΟΥ ΣΤΗΝ ΕΛΛΗΝΙΚΗ ΠΟΛΙΤΙΚΗ 1916-1936
-    4: 938.7 ΒΕΡ
+    4: 938.7ΒΕΡ
     5: '2010'
     8: ΕΞΑΝΤΑΣ
     9: ΑΘΗΝΑ
     10: '1977'
     11: 467Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΤΡΑΤΟΣ-(1916-1936)
     13: ΣΤΡΑΤΟΣ-(1916-1936)-ΕΠΕΜΒΑΣΕΙΣ
@@ -6253,58 +6253,50 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 122
   authors:
-  - ΒΟΓΑΣ,ΙΩΑΝΝΗΣ
-  title: Η ΘΕΣΙΣ ΤΟΥ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟΥ ΖΗΤΗΜΑΤΟΣ
-  dewey: 938.751 ΒΟΓ
+  - ΔΙΑΜΑΝΤΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  title: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ ΚΑΙ ΧΕΙΡΟΓΡΑΦΑ
+  dewey: 938.915 ΔΙΑ
   entry_numbers:
-  - '2024'
-  - '2762'
-  - '2739'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1970
-  pages: 26
+  - '22924'
+  pages: 32
   topics:
-  - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
-  - ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
-  - ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
-  - ΘΕΣΕΙΣ
-  - ΘΕΣΙΣ
-  notes: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ 30
+  - ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ
+  - ΧΕΙΡΟΓΡΑΦΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 122
-    1: ΒΟΓΑΣ,ΙΩΑΝΝΗΣ
-    2: Η ΘΕΣΙΣ ΤΟΥ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟΥ ΖΗΤΗΜΑΤΟΣ
-    4: 938.751ΒΟΓ
-    5: 2024-2762-2739
-    8: Χ.Ε
-    9: ΑΘΗΝΑ
-    10: '1970'
-    11: 26Σ
-    12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
-    13: ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
-    14: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ-ΘΕΣΕΙΣ
-    21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ 30
-    22: ΘΕΣΙΣ
+    1: ΔΙΑΜΑΝΤΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+    2: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ ΚΑΙ ΧΕΙΡΟΓΡΑΦΑ
+    4: 938.915ΔΙΑ
+    5: '22924'
+    11: '32'
+    12: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ-ΧΕΙΡΟΓΡΑΦΑ
+    13: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ-ΧΕΙΡΟΓΡΑΦΑ
+    14: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ-ΧΕΙΡΟΓΡΑΦΑ
     3: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
+    21: null
+    22: null
     23: null
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
@@ -6823,15 +6815,15 @@
     29: null
     30: null
 - dbase_number: 133
   authors:
   - ΒΟΥΡΝΑΣ,ΤΑΣΟΣ
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΩΤΕΡΗΣ ΕΛΛΑΔΑΣ
   subtitle: ΑΠΟ ΤΗΝ ΕΠΑΝΑΣΤΑΣΗ ΤΟΥ 1821 ΩΣ ΤΟ ΚΙΝΗΜΑ ΤΟΥ ΓΟΥΔΙ(1909)
-  dewey: 938.5 ΒΟΥ
+  dewey: 938.7 ΒΟΥ
   entry_numbers:
   - '1846'
   editor: ΤΟΛΙΔΗ // ΑΘΗΝΑ
   pages: 620
   topics:
   - 1821-1909
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -6843,15 +6835,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 133
     1: ΒΟΥΡΝΑΣ,ΤΑΣΟΣ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΩΤΕΡΗΣ ΕΛΛΑΔΑΣ
     3: ΑΠΟ ΤΗΝ ΕΠΑΝΑΣΤΑΣΗ ΤΟΥ 1821 ΩΣ ΤΟ ΚΙΝΗΜΑ ΤΟΥ ΓΟΥΔΙ(1909)
-    4: 938.5 ΒΟΥ
+    4: 938.7ΒΟΥ
     5: '1846'
     8: ΤΟΛΙΔΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 620Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-(1821-1909)
     13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΟΥΔΙ-ΚΙΝΗΜΑ-1909
@@ -12464,15 +12456,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 243
     1: ΔΙΑΚΟΓΙΑΝΝΗΣ,ΚΥΡΙΑΚΟΣ Ι
     2: ΟΙ ΣΑΡΚΟΦΑΓΟΙ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-    4: 938.8 ΔΙΑ
+    4: 938.8ΔΙΑ
     5: '2314'
     8: ΛΑΔΙΑ
     9: ΑΘΗΝΑ
     10: '1979'
     11: 557Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΗΜΟΚΡΑΤΙΑ
     13: ΔΗΜΟΚΡΑΤΙΑ-ΙΣΤΟΡΙΑ
@@ -13129,15 +13121,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 256
     1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
     2: ΤΟ ΝΗΣΙ ΤΟΥ ΗΛΙΟΥ
-    4: 889.1 ΔΙΑ
+    4: 889.1ΔΙΑ
     5: '346'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1982'
     11: 69Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΥΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
@@ -13179,15 +13171,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 257
     1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
     2: ΦΩΝΕΣ ΣΤΟ ΧΑΟΣ
-    4: 889.1 ΔΙΑ
+    4: 889.1ΔΙΑ
     5: '1198'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1986'
     11: 46Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
@@ -13229,15 +13221,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 258
     1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
     2: Η ΤΕΛΕΥΤΑΙΑ ΦΛΟΓΑ
-    4: 889.1 ΔΙΑ
+    4: 889.1ΔΙΑ
     5: '1201'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1983'
     11: 119Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ
@@ -13280,15 +13272,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 259
     1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
     2: ΑΝΕΜΩΝΕΣ ΣΤΗ ΘΥΕΛΛΑ
-    4: 889.1 ΔΙΑ
+    4: 889.1ΔΙΑ
     5: 1200-1199
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 58Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΝΝΟΥ
@@ -13990,15 +13982,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 273
     1: ΔΡΟΣΟΠΟΥΛΟΣ,Κ Η
     2: ΟΙ ΑΘΗΝΑΙΟΙ ΩΣ ΠΟΛΕΜΙΣΤΑΙ
-    4: 938.13 ΔΡΟ
+    4: 938.13ΔΡΟ
     5: '2321'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1944'
     11: 15Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ-ΑΘΗΝΑΙΟΙ
     13: ΑΘΗΝΑ-ΑΡΧΑΙΑ
@@ -14123,17 +14115,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 276
   authors:
-  - ΕΙΣΙΤΑΛ,ΚΟΥΣΤΑΒ
+  - EICHTHAL,GUSTAVE
   title: Η ΕΛΛΑΣ ΤΟΥ 1833-1835
-  dewey: 938.62 ΕΙΣ
+  dewey: 938.62 EIC
   entry_numbers:
   - '2501'
   translators:
   - ΒΙΚΕΛΑ,Δ.
   editor: None // ΑΘΗΝΑ
   edition_year: 1968
   pages: 120
@@ -14143,17 +14135,17 @@
   - '1833'
   - '1835'
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 276
-    1: ΕΙΣΙΤΑΛ,ΚΟΥΣΤΑΒ
+    1: EICHTHAL,GUSTAVE
     2: Η ΕΛΛΑΣ ΤΟΥ 1833-1835
-    4: 938.62 ΕΙΣ
+    4: 938.62EIC
     5: '2501'
     6: ΒΙΚΕΛΑ,Δ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1968'
     11: 120Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
@@ -16447,15 +16439,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 321
     1: ΖΑΝΑΝΤΡΙΣ,ΚΑΣ
     2: ΕΛΛΗΝΕΣ ΑΔΕΡΦΟΙ ΜΟΥ ΑΣ ΠΟΛΕΜΗΣΩΜΕΝ
-    4: 938 ΖΑΝ
+    4: 938ΖΑΝ
     5: '2558'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1948'
     11: 88Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ ΤΗΣ ΠΕΝΝΑΣ
     13: ΠΟΛΕΜΟΣ ΤΗΣ ΠΕΝΝΑΣ
@@ -16577,15 +16569,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 324
   authors:
   - ΖΕΝΕΒΟΥΑ,ΜΩΡΙΣ
   title: Η ΕΛΛΑΣ ΤΟΥ ΚΑΡΑΜΑΝΛΗ Ή Η ΔΗΜΟΚΡΑΤΙΑ ΔΥΣΧΕΡΗΣ
-  dewey: 938.792 ΖΕΝ
+  dewey: 938.497 ΖΕΝ
   entry_numbers:
   - '2575'
   editor: ΣΙΔΕΡΗΣ // ΑΘΗΝΑ
   edition_year: 1972
   pages: 270
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -16594,15 +16586,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 324
     1: ΖΕΝΕΒΟΥΑ,ΜΩΡΙΣ
     2: Η ΕΛΛΑΣ ΤΟΥ ΚΑΡΑΜΑΝΛΗ Ή Η ΔΗΜΟΚΡΑΤΙΑ ΔΥΣΧΕΡΗΣ
-    4: 938.792ΖΕΝ
+    4: 938.497ΖΕΝ
     5: '2575'
     8: ΣΙΔΕΡΗΣ
     9: ΑΘΗΝΑ
     10: '1972'
     11: 270Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΗΜΟΚΡΑΤΙΑ
     13: ΔΗΜΟΚΡΑΤΙΑ-ΚΑΡΑΜΑΝΛΗΣ
@@ -17619,15 +17611,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 344
     1: ΘΕΟΔΩΡΑΚΟΠΟΥΛΟΣ,Ι.Ν
     2: ΤΟ ΠΝΕΥΜΑ ΤΟΥ ΝΕΟΕΛΛΗΝΙΣΜΟΥ ΚΑΙ Η ΤΡΟΠΗ ΤΩΝ ΚΑΙΡΩΝ
-    4: 938 ΘΕΟ
+    4: 938ΘΕΟ
     5: '2506'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1945'
     11: 64Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΕΟΕΛΛΗΝΙΣΜΟΣ
     13: ΝΕΟΕΛΛΗΝΙΣΜΟΣ
@@ -17669,15 +17661,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 345
     1: ΘΕΟΔΩΡΟΠΟΥΛΟΥ-ΛΙΒΑΔΑ,ΒΑΡΒΑΡΑ
     2: Ο ΕΓΚΑΙΝΙΣΤΗΣ ΚΑΙ ΠΡΩΤΟΣ ΣΠΟΡΕΥΣ ΤΟΥ ΡΙΖΟΣΠΑΣΤΙΣΜΟΥ
-    4: 938 ΘΕΟ
+    4: 938ΘΕΟ
     5: '1970'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1966'
     11: 99Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΙΖΟΣΠΑΣΤΙΣΜΟΣ
     13: ΡΙΖΟΣΠΑΣΤΙΣΜΟΣ-ΛΙΒΑΔΑΣ
@@ -18521,17 +18513,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 362
   authors:
-  - ΘΥΕΡ,ΑΜΕΝΤ
+  - THIERRY,AMEDEE
   title: ΙΣΤΟΡΙΑ ΤΟΥ ΑΤΤΙΛΑ ΚΑΙ ΤΩΝ ΔΙΑΔΟΧΩΝ ΑΥΤΟΥ
-  dewey: 938.322 ΘΥΕ
+  dewey: 938.322 THI
   entry_numbers:
   - '1764'
   - '1982'
   - '1984'
   translators:
   - ΒΟΥΤΥΡΑΣ,Σ.Ι.
   editor: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ // ΑΘΗΝΑ
@@ -18543,17 +18535,17 @@
   - ΕΠΙΔΡΟΜΕΣ
   - ΑΤΤΙΛΑΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 362
-    1: ΘΥΕΡ,ΑΜΕΝΤ
+    1: THIERRY,AMEDEE
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΑΤΤΙΛΑ ΚΑΙ ΤΩΝ ΔΙΑΔΟΧΩΝ ΑΥΤΟΥ
-    4: 938.322ΘΥΕ
+    4: 938.322THI
     5: 1764-1982-1984
     6: ΒΟΥΤΥΡΑΣ,Σ.Ι
     8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '1903'
     11: 603Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΒΥΖΑΝΤΙΟ
@@ -18598,15 +18590,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 363
     1: ΘΡΥΛΟΣ,ΑΛΚΗΣ
     2: ΤΟ ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ
-    4: 886.2 ΘΡΥ
+    4: 886.2ΘΡΥ
     5: 1414-1415-1416-1417-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 491Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-(1927-1955)
@@ -18648,15 +18640,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 364
     1: ΘΡΥΛΟΣ,ΑΛΚΗΣ
     2: ΜΟΡΦΕΣ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΠΕΖΟΓΡΑΦΙΑΣ
-    4: 880.3 ΘΡΥ
+    4: 880.3ΘΡΥ
     5: '210'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 242Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -18750,15 +18742,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 366
     1: ΘΡΥΛΟΣ,ΑΛΚΗΣ
     2: ΜΟΡΦΕΣ ΚΑΙ ΘΕΜΑΤΑ ΤΟΥ ΘΕΑΤΡΟΥ
-    4: 886.2 ΘΡΥ
+    4: 886.2ΘΡΥ
     5: 1413-1412
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1961'
     11: 271Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΜΟΡΦΕΣ ΚΑΙ ΘΕΜΑΤΑ
@@ -18955,15 +18947,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 370
     1: ΙΑΚΩΒΙΔΗ,ΛΙΛΗ
     2: ΘΕΑΤΡΟ
-    4: 886.2 ΙΑΚ
+    4: 886.2ΙΑΚ
     5: '1500'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 344Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
@@ -19058,15 +19050,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 372
     1: ΙΨΕΝ,ΕΡΡΙΚΟΣ
     2: ΟΙ ΜΝΗΣΤΗΡΕΣ ΤΟΥ ΘΡΟΝΟΥ
-    4: 832 ΙΨΕ
+    4: 832ΙΨΕ
     5: '1371'
     6: ΚΑΣΤΡΟ,ΚΑΙΤΗ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: '1975'
     11: 192Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -19115,15 +19107,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 373
     1: ΙΨΕΝ,ΕΡΡΙΚΟΣ
     2: ΕΝΤΑ ΓΚΑΜΛΕΡ
     3: ΔΡΑΜΑ
-    4: 832 ΙΨΕ
+    4: 832ΙΨΕ
     5: 1398-8112
     6: ΚΟΥΚΟΥΛΑ,Λ
     8: ΓΚΟΒΟΣΤΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 142Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -19169,15 +19161,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 374
     1: ΙΨΕΝ,ΕΡΡΙΚΟΣ
     2: Η ΓΙΟΡΤΗ ΣΤΟ ΣΟΛΧΑΟΥΓΚ
     3: ΔΡΑΜΑ
-    4: 832 ΙΨΕ
+    4: 832ΙΨΕ
     5: '1397'
     6: ΚΟΥΚΟΥΛΑ,Λ
     8: ΓΚΟΒΟΣΤΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 72Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -19267,15 +19259,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 376
     1: ΙΩΑΝΝΙΔΗΣ,ΑΛΚΙΒΙΑΔΗΣ
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ
-    4: 938 ΙΩΑ
+    4: 938ΙΩΑ
     5: '2408'
     8: ΚΟΛΛΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1904'
     11: 112Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΘΝΟΣ
     13: ΕΘΝΟΣ-ΙΣΤΟΡΙΑ
@@ -19473,15 +19465,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 380
     1: ΚΑΒΒΑΘΑΣ,ΒΑΣΙΛΗΣ
     2: ΑΙΘΙΟΠΙΑ
     3: 13 ΜΗΝΕΣ ΗΛΙΑΣ 13 ΜΗΝΕΣ ΘΑΝΑΤΟΣ
-    4: 915.39 ΚΑΒ
+    4: 915.39ΚΑΒ
     5: 418-419
     8: ΑΛΚΥΩΝ
     9: ΑΘΗΝΑ
     10: '1984'
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΑΙΘΙΟΠΙΑ
     13: ΤΑΞΙΔΙΑ-ΑΙΘΙΟΠΙΑ
     14: ΑΙΘΙΟΠΙΑ-ΤΑΞΙΔΙΑ
@@ -19524,15 +19516,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 381
     1: ΚΑΒΑΝΕΣ,ΠΙΕΡ
     2: L'EPIRE DE LA MORT DE PYRROS
     3: A LA CONGUTE ROMAINE(272-167M.X)
-    4: 938.21 CAB
+    4: 938.21CAB
     5: '2177'
     8: X.E
     9: PARIS
     10: '1976'
     11: 644S
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-(272-167Μ.Χ)
     13: ΗΠΕΙΡΟΣ-(272-167Μ.Χ)
@@ -21634,15 +21626,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 422
     1: ΚΑΝΑΤΣΟΥΛΗΣ,ΔΗΜ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ ΜΕΧΡΙ ΤΟΥ ΜΕΓΑΛΟΥ ΚΩΝΣΑΝΤΙΝΟΥ
-    4: 938.21 ΚΑΝ
+    4: 938.21ΚΑΝ
     5: '2199'
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1964'
     11: 188Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΑ-ΚΩΝΣΤΑΝΤΙΚΟΣ
@@ -21686,15 +21678,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 423
     1: ΚΑΝΑΤΣΟΥΛΗΣ,ΔΗΜ
     2: Η ΜΑΚΕΔΟΝΙΑ ΑΠΟ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ
     3: ΜΕΧΡΙ ΤΗΣ ΑΝΟΔΟΥ ΤΟΥ ΦΙΛΙΠΠΟΥ Β'
-    4: 938.21 ΚΑΝ
+    4: 938.21ΚΑΝ
     5: 2202-2203
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1976'
     11: 134Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΑ-ΦΙΛΙΠΠΟΣ Β'
@@ -21822,15 +21814,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 426
   authors:
   - ΚΑΠΟΔΙΣΤΡΙΑΣ,ΙΩΑΝΝΗΣ
   title: ΑΡΧΕΙΟΝ ΙΩΑΝΝΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
-  dewey: 938.571 ΚΑΠ
+  dewey: 938.571 ΧΣ
   entry_numbers:
   - '1779'
   - '1780'
   - '1781'
   - '1782'
   editor: None // ΚΕΡΚΥΡΑ
   edition_year: 1976
@@ -21842,15 +21834,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 426
     1: ΚΑΠΟΔΙΣΤΡΙΑΣ,ΙΩΑΝΝΗΣ
     2: ΑΡΧΕΙΟΝ ΙΩΑΝΝΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
-    4: 938.571ΚΑΠ
+    4: 938.571Χ.Σ
     5: 1779-1780-1781-1782-
     8: Χ.Ε
     9: ΚΕΡΚΥΡΑ
     10: '1976'
     11: 320Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
     13: ΚΑΠΟΔΙΣΤΡΙΑΣ-ΑΡΧΕΙΟ
@@ -24283,15 +24275,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 474
     1: ΚΑΣΙΜΑΤΗΣ,ΓΡΗΓ Π
     2: Η ΕΛΛΑΣ ΚΑΙ Ο ΚΟΣΜΟΣ
-    4: 938 ΚΑΣ
+    4: 938ΚΑΣ
     5: '2490'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1961'
     11: 422Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΟΣΜΟΣ
     13: ΕΛΛΑΣ-ΚΟΣΜΟΣ
@@ -24315,15 +24307,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 475
   authors:
   - ΚΑΣΙΜΑΤΗΣ,ΓΡΗΓ.Π
   title: ΤΟ ΜΗΝΥΜΑ ΤΟΥ ΓΚΑΝΤΙ
-  dewey: 938.001 ΚΑΣ
+  dewey: 938 ΚΑΣ
   entry_numbers:
   - '2339'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
   pages: 39
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -24333,15 +24325,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 475
     1: ΚΑΣΙΜΑΤΗΣ,ΓΡΗΓ.Π
     2: ΤΟ ΜΗΝΥΜΑ ΤΟΥ ΓΚΑΝΤΙ
-    4: 938.001ΚΑΣ
+    4: 938ΚΑΣ
     5: '2339'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1969'
     11: 39Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΗΝΥΜΑ ΓΚΑΝΤΙ
     13: ΓΚΑΝΤΙ-ΜΗΝΥΜΑ
@@ -24535,15 +24527,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 479
     1: ΚΑΣΤΟΡΙΑΔΗΣ,ΚΟΡΝΗΛΙΟΣ
     2: ΜΠΡΟΣΤΑ ΣΤΟΝ ΠΟΛΕΜΟ
-    4: 938.ΚΑΣ
+    4: 938ΚΑΣ
     5: '2503'
     6: ΧΡΙΣΤΟΦΙΔΗ-ΚΑΣΤΟΡΙΑΔ
     8: Χ.Ε
     9: ΠΑΡΙΣΙ
     10: '1981'
     11: 338Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
@@ -25402,15 +25394,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 496
     1: ΚΟΚΚΙΝΗΣ,ΔΙΟΝΥΣΙΟΣ
     2: ΟΙ ΔΥΟ ΠΟΛΕΜΟΙ 1940-1941
-    4: 938.75 ΚΟΚ
+    4: 938.75ΚΟΚ
     5: '2404'
     8: Ο ΠΛΑΤΩΝ
     9: ΑΘΗΝΑ
     10: '1945'
     11: 310Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΙ-(1940-1941)
     13: ΠΟΛΕΜΟΙ-(1940-1941)
@@ -25775,15 +25767,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 503
     1: ΚΟΛΙΑΤΣΟΣ,ΧΡΗΣΤΟΣ
     2: ΣΕΛΙΔΕΣ ΔΟΞΗΣ
     3: ΓΡΑΜΜΕΝΕΣ ΜΕ ΤΟ ΑΙΜΑ ΤΩΝ ΠΑΙΔΙΩΝ ΤΗΣ ΕΛΛΑΔΟΣ ΕΙΣ ΤΑ Β.ΗΠΕΙΡΩ
-    4: 938.75 ΚΟΛ
+    4: 938.75ΚΟΛ
     5: 1958-2632
     7: 2ΕΚΔ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1948'
     11: 321Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ-1940
@@ -26030,15 +26022,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 508
     1: ΚΟΜΠΟΡΡΟΖΟΣ,ΙΩΑΝΝΗΣ
     2: ΕΛΛΑΔΑ ΚΑΙ ΜΟΝΟΝ ΕΛΛΑΔΑ
-    4: 938.75 ΚΟΜ
+    4: 938.75ΚΟΜ
     5: '2514'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1952'
     11: 120Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
     13: 1940-ΕΛΛΑΔΑ
@@ -26287,15 +26279,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 513
     1: ΚΟΝΟΜΟΣ,ΝΤΙΝΟΣ
     2: ΗΠΕΙΡΩΤΕΣ ΣΤΗ ΖΑΚΥΝΘΟ
-    4: 938.93 ΚΟΝ
+    4: 938.93ΚΟΝ
     5: 2165-5257
     8: ΕΤΑΙΡ.ΗΠΕΙΡ.ΜΕΛΕΤΩΝ
     9: ΙΩΑΝΝΙΝΑ
     10: '1964'
     11: 72Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΕΣ
     13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΕΣ
@@ -26536,15 +26528,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 518
     1: ΚΟΝΤΟΓΕΩΡΓΗΣ,ΓΕΩΡΓΙΟΣ Λ
     2: Η ΕΛΛΑΔΑ ΣΤΗΝ ΕΥΡΩΠΗ
-    4: 938.8 ΚΟΝ
+    4: 938.8ΚΟΝ
     5: '923'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 311Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
     13: ΕΥΡΩΠΗ-ΕΛΛΑΔΑ
@@ -26589,15 +26581,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 519
     1: ΚΟΝΤΟΜΙΧΗΣ,ΠΑΝΤΑΖΗΣ
     2: ΤΟ ΝΕΟΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ ΣΤΗ ΛΕΥΚΑΔΑ (1800-1964)
-    4: 886.2 ΚΟΝ
+    4: 886.2ΚΟΝ
     5: 1428-1429
     8: ΜΕΛΙΣΣΑ
     9: ΑΘΗΝΑ
     10: '1964'
     11: 108Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΛΕΥΚΑΔΑ (1800-1964)
@@ -26639,15 +26631,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 520
     1: ΚΟΝΤΥΛΑΚΗΣ.Ι
     2: Ο ΠΑΤΟΥΧΑΣ
-    4: 889.38 ΚΟΝ
+    4: 889.38ΚΟΝ
     5: '1178'
     8: ΓΡΗΓΟΡΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 190Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -26690,15 +26682,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 521
     1: ΚΟΝΤΥΛΑΚΗΣ,Ι
     2: ΟΤΑΝ ΗΜΟΥΝ ΔΑΣΚΑΛΟΣ
-    4: 889.38 ΚΟΝ
+    4: 889.38ΚΟΝ
     5: '1179'
     8: ΓΡΗΓΟΡΗ
     9: ΑΘΗΝΑ
     10: '1972'
     11: 134Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -26738,15 +26730,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 522
     1: ΚΟΡΑΗΣ,Α
     2: ΠΡΟΔΡΟΜΟΣ ΕΛΛΗΝΙΚΗΣ ΒΙΒΛΙΟΘΗΚΗΣ
-    4: 880.08 ΚΟΡ
+    4: 880.08ΚΟΡ
     5: '1220'
     8: ΔΙΔΟΤΟΥ
     9: ΠΑΡΙΣΙ
     11: 425Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΚΟΡΑΗΣ
     14: ΚΟΡΑΗΣ
@@ -26789,15 +26781,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 523
     1: ΚΟΡΑΗΣ,Α
     2: ΕΠΙΣΤΟΛΑΙ ΑΔΑΜΑΝΤΙΟΥ ΚΟΡΑΗ
-    4: 880.08 ΚΟΡ
+    4: 880.08ΚΟΡ
     5: 2683-2682-
     8: ΠΕΡΡΗ
     9: ΑΘΗΝΑ
     10: '1885'
     11: 1007Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΚΟΡΑΗΣ
@@ -27564,15 +27556,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 538
     1: ΚΟΥΡΟΥΚΛΗΣ,Γ
     2: ΤΟ ΠΟΛΕΜΙΚΟΝ ΗΜΕΡΟΛΟΓΙΟΝ ΤΗΣ Δ'ΜΟΙΡΑΣ ΠΥΡΟΒΟΛΙΚΟΥ
-    4: 938.75 ΚΟΥ
+    4: 938.75ΚΟΥ
     5: '2390'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1973'
     11: 185Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΙΚΟ ΗΜΕΡΟΛΟΓΙΟ 1941
     13: ΗΜΕΡΟΛΟΓΙΟ-ΠΟΛΕΜΙΚΟ-1941
@@ -27998,15 +27990,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 547
   authors:
   - ΚΡΑΨΙΤΗΣ,ΒΑΣΙΛΗΣ
-  title: ΟΙ ΜΟΥΣΑΛΜΑΝΟΙ ΤΣΑΜΗΔΕΣ ΤΗΣ ΘΕΣΠΡΩΤΙΑΣ
+  title: Η ΙΣΤΟΡΙΚΟΙ ΑΛΗΘΕΙΑ ΓΙΑ ΤΟΥΣ ΜΟΥΣΑΛΜΑΝΟΥΣ ΤΣΑΜΗΔΕΣ
   dewey: 938.492 ΚΡΑ
   entry_numbers:
   - '2253'
   - '8783'
   editor: None // ΑΘΗΝΑ
   pages: 236
   topics:
@@ -28017,15 +28009,15 @@
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 547
     1: ΚΡΑΨΙΤΗΣ,ΒΑΣΙΛΗΣ
-    2: ΟΙ ΜΟΥΣΑΛΜΑΝΟΙ ΤΣΑΜΗΔΕΣ ΤΗΣ ΘΕΣΠΡΩΤΙΑΣ
+    2: Η ΙΣΤΟΡΙΚΟΙ ΑΛΗΘΕΙΑ ΓΙΑ ΤΟΥΣ ΜΟΥΣΑΛΜΑΝΟΥΣ ΤΣΑΜΗΔΕΣ
     4: 938.492ΚΡΑ
     5: 2253-8783
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 236Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΠΡΩΤΙΑ
@@ -29289,15 +29281,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 572
     1: ΚΥΡΙΑΚΟΠΟΥΛΟΣ,ΚΩΣΤΑΣ
     2: ΣΕΛΙΔΕΣ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΤΩΝ ΕΛΛΗΝΩΝ
     3: ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΚΑΙ ΤΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ ΤΟΥ 21
-    4: 938 ΚΥΡ
+    4: 938ΚΥΡ
     5: '1911'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 453Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ ΕΩΣ 1821
     13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ
@@ -29492,15 +29484,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 576
     1: ΚΩΝΣΤΑΝΤΟΠΟΥΛΟΣ,ΣΑΒΒΑΣ
     2: ΣΟΒΙΕΤΙΚΗ ΡΩΣΙΑ ΚΑΙ ΕΛΛΑΣ
-    4: 938 ΚΩΝ
+    4: 938ΚΩΝ
     5: '1683'
     8: ΕΛΕΥΘΕΡΟΣ ΚΟΣΜΟΣ
     9: ΑΘΗΝΑ
     10: '1968'
     11: 164Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΣΙΑ
     13: ΡΩΣΙΑ-ΕΛΛΑΣ
@@ -29745,15 +29737,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 581
     1: ΛΑΖΑΡΟΥ,ΑΝΑΣΤ
     2: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗ
-    4: 938 ΛΑΖ
+    4: 938ΛΑΖ
     5: '2407'
     8: ΟΕΣΒ
     9: ΑΘΗΝΑ
     10: '1940'
     11: 263Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
     13: ΕΛΛΑΣ-ΙΣΤΟΡΙΑ
@@ -29797,15 +29789,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 582
     1: ΛΑΖΑΡΙΔΗΣ,ΚΩΣΤΑΣ
     2: ΤΟ ΧΩΡΙΟ ΜΟΥ
     3: ΤΟ ΚΟΥΚΟΥΛΙ
-    4: 938.93 ΛΑΖ
+    4: 938.93ΛΑΖ
     5: '312'
     8: Χ.Ε
     9: ΓΙΑΝΝΙΝΑ
     10: '1977'
     11: 51Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΚΟΥΚΟΥΛΙ
@@ -30707,15 +30699,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 600
     1: ΛΑΠΠΑΣ,ΤΑΚΗΣ
     2: ΘΕΑΤΡΙΚΕΣ ΕΙΚΟΝΕΣ ΑΠ'ΤΟ ΕΙΚΟΣΙΕΝΑ
-    4: 886.2 ΛΑΠ
+    4: 886.2ΛΑΠ
     5: '2672'
     8: ΠΕΧΛΙΒΑΝΙΔΗΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 161Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΙΚΟΣΙΕΝΑ
@@ -30856,15 +30848,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 603
     1: ΛΑΣΚΑΡΙΣ,ΘΕΟΔΟΣΙΟΣ
     2: Ο ΔΙΑΚΟΣ ΣΤΟ ΜΟΝΑΣΤΗΡΙ ΚΑΙ ΚΡΥΣΤΑΛΛΩ
-    4: 886.2 ΛΑΣ
+    4: 886.2ΛΑΣ
     5: '1464'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 85Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
@@ -30991,15 +30983,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 606
   authors:
   - ΛΕΣΚΥ,ΑΛΠΙΝ
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-  dewey: 881.09 LES
+  dewey: 881.09 ΛΕΣ
   entry_numbers:
   - '2563'
   editor: ΚΥΡΙΑΚΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1978
   pages: 1271
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -31008,15 +31000,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 606
     1: ΛΕΣΚΥ,ΑΛΠΙΝ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-    4: 881.09 LES
+    4: 881.09ΛΕΣ
     5: '2563'
     8: ΚΥΡΙΑΚΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1978'
     11: 1271Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΑΡΧΑΙΑ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -31040,15 +31032,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 607
   authors:
   - ΛΙΑΠΗΣ,ΚΩΣΤΑΣ
   title: ΣΕΛΙΔΕΣ ΑΠ'ΤΗΝ ΙΣΤΟΡΙΑ ΤΟΥ ΑΝΑΤΟΛΙΚΟΥ ΠΗΛΙΟΥ
-  dewey: 938.931 ΛΙΑ
+  dewey: 931 ΛΙΑ
   entry_numbers:
   - '2325'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
   pages: 56
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -31058,15 +31050,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 607
     1: ΛΙΑΠΗΣ,ΚΩΣΤΑΣ
     2: ΣΕΛΙΔΕΣ ΑΠ'ΤΗΝ ΙΣΤΟΡΙΑ ΤΟΥ ΑΝΑΤΟΛΙΚΟΥ ΠΗΛΙΟΥ
-    4: 938.931ΛΙΑ
+    4: 931ΛΙΑ
     5: '2325'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1969'
     11: 56Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΣΑΛΙΑ
     13: ΘΕΣΣΑΛΙΑ-ΜΑΓΝΗΣΙΑ-ΠΗΛΙΟ
@@ -31108,15 +31100,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 608
     1: ΛΙΑΤΣΟΣ,ΔΗΜΗΤΡΙΟΣ Π
     2: Η ΒΑΥΑΡΟΚΡΑΤΙΑ ΚΑΙ ΟΙ ΑΓΩΝΙΣΤΕΣ ΤΟΥ '21
-    4: 938.5 ΛΙΑ
+    4: 938.5ΛΙΑ
     5: '1808'
     8: ΕΛΛΗΝΙΚΟ ΒΙΒΛΙΟ
     9: ΑΘΗΝΑ
     10: '1976'
     11: 119Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821-ΑΓΩΝΙΣΤΕΣ
     13: 1821-ΑΓΩΝΙΣΤΕΣ
@@ -31160,15 +31152,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 609
     1: ΛΙΔΩΡΙΚΗΣ,ΑΛΕΚΟΣ
     2: ΟΙ ΞΕΡΡΙΖΩΜΕΝΟΙ
-    4: 886.2 ΛΙΔ
+    4: 886.2ΛΙΔ
     5: '1588'
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: '1979'
     11: 119Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -31212,15 +31204,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 610
     1: ΛΙΔΩΡΙΚΗΣ ΑΛΕΚΟΣ
     2: ΧΩΡΙΣ ΓΑΝΤΙ
     3: ΣΑΤΙΡΙΚΗ ΚΩΜΩΔΙΑ
-    4: 886.2 ΛΙΔ
+    4: 886.2ΛΙΔ
     5: '1362'
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 132Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΑΤΥΡΑ
     13: ΕΛΛΗΝΙΚΗ ΣΑΤΥΡΑ-ΕΡΓΟ
@@ -31312,15 +31304,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 612
     1: ΚΟΥΡΕΤΑΣ,Δ
     2: ΑΝΩΜΑΛΟΙ ΧΑΡΑΚΤΗΡΕΣ ΕΙΣ ΤΟ ΑΡΧΑΙΟΝ ΔΡΑΜΑ
-    4: 881.2 ΚΟΥ
+    4: 881.2ΚΟΥ
     5: '1445'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1951'
     11: 325Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -31365,15 +31357,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 613
     1: ΛΑΔΙΑ,ΕΛΕΝΗ
     2: ΠΟΙΗΤΕΣ ΚΑΙ ΑΡΧΑΙΑ ΕΛΛΑΔΑ
     3: ΣΙΚΕΛΙΑΝΟΣ-ΣΕΦΕΡΗΣ-ΠΑΠΑΔΙΤΣΑΣ
-    4: 881.2 ΛΑΔ
+    4: 881.2ΛΑΔ
     5: '225'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1983'
     11: 146Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΠΑΠΑΔΙΤΣΑΣ
@@ -31516,15 +31508,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 616
     1: ΛΑΣΚΑΡΗΣ,ΝΙΚΟΛΑΟΣ
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΝΕΟΕΛΛΗΝΙΚΟΥ ΘΕΑΤΡΟΥ
-    4: 886.2 ΛΑΣ
+    4: 886.2ΛΑΣ
     5: 1423-1424-1422-
     8: ΒΑΣΙΛΕΙΟΥ
     9: ΑΘΗΝΑ
     10: '1938'
     11: 333Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
@@ -31723,15 +31715,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 620
     1: ΛΟΓΟΘΕΤΗΣ,ΚΩΝΣΤ
     2: ΕΘΝΙΚΑ ΚΑΙ ΕΠΙΣΤΗΜΟΝΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
-    4: 938.04 ΛΟΓ
+    4: 938.04ΛΟΓ
     5: '2535'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1971'
     11: 563Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΛΕΤΗΜΑΤΑ
     13: ΜΕΛΕΤΗΜΑΤΑ-ΕΘΝΙΚΑ
@@ -31773,15 +31765,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 621
     1: ΛΟΓΟΘΕΤΗΣ,ΚΩΝΣΤ.Ι.
     2: ΚΡΙΤΙΚΑ ΚΑΙ ΕΡΜΗΝΕΥΤΙΚΑ ΕΙΣ ΕΛΛΗΝΑΣ ΣΥΓΓΡΑΦΕΙΣ
-    4: 880.3 ΛΟΓ
+    4: 880.3ΛΟΓ
     5: 2699-2700
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 171Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΚΡΙΤΙΚΑ
@@ -31876,15 +31868,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 623
     1: ΛΥΓΙΖΟΣ,ΜΗΤΣΟΣ
     2: ΘΕΜΑΤΑ ΚΑΙ ΠΟΙΗΤΕΣ
     3: ΔΟΚΙΜΙΑ ΚΑΙ ΜΕΛΕΤΕΣ
-    4: 880.4 ΛΥΓ
+    4: 880.4ΛΥΓ
     5: '1007'
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: '1977'
     11: 396Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
@@ -31928,15 +31920,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 624
     1: ΛΥΓΙΖΟΣ,ΜΗΤΣΟΣ
     2: ΤΟ ΝΕΟΕΛΛΗΝΙΚΟ ΠΛΑΙ ΣΤΟ ΠΑΓΚΟΣΜΙΟ ΘΕΑΤΡΟ
-    4: 886.2 ΛΥΓ
+    4: 886.2ΛΥΓ
     5: '1427'
     8: ΣΑΛΙΒΕΡΟΥ
     9: ΑΘΗΝΑ
     10: '1958'
     11: 672Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΑΓΚΟΣΜΙΟ
@@ -31980,15 +31972,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 625
     1: ΛΥΓΙΖΟΣ,ΜΗΤΣΟΣ
     2: ΤΟΜΗ ΣΤΟ ΣΥΓΧΡΟΝΟ ΘΕΑΤΡΟ
-    4: 886.2 ΛΥΓ
+    4: 886.2ΛΥΓ
     5: '1430'
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: '1975'
     11: 205Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΣΥΓΧΡΟΝΟ
@@ -32081,15 +32073,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 627
     1: ΛΩΛΗΣ,ΝΙΚΟΛΑΟΣ Β.
     2: ΤΟΠΟΙ ΚΑΙ ΘΡΥΛΟΙ ΤΗΣ ΗΠΕΙΡΟΥ
-    4: 398 ΛΩΛ
+    4: 398ΛΩΛ
     5: '271'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1961'
     11: 76Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΗΠΕΙΡΟΣ
     13: ΤΑΞΙΔΙΑ-ΗΠΕΙΡΟΣ
@@ -32233,15 +32225,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 630
     1: ΜΑΚΡΗΣ,ΕΥΡΙΠΙΔΗΣ
     2: ΖΩΗ ΚΑΙ ΠΑΡΑΔΟΣΗ ΤΩΝ ΣΑΡΑΚΑΤΣΑΙΩΝ
-    4: 398 ΚΑΜ
+    4: 398ΚΑΜ
     5: '304'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1990'
     11: 350Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΙΩΑΝΝΙΝΑ
     13: ΗΠΕΙΡΟΣ-ΙΩΑΝΝΙΝΑ
@@ -32337,15 +32329,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 632
     1: ΜΑΛΑΜΑΣ,ΛΑΜΠΡΟΣ
     2: ΤΟΥΡΙΣΤΙΚΗ ΗΠΕΙΡΟΣ
-    4: 914.95 ΜΑΛ
+    4: 914.95ΜΑΛ
     5: 273-274-275
     8: Χ.Ε
     9: ΓΙΑΝΝΙΝΑ
     10: Χ.Ε
     11: '1971'
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΗΠΕΙΡΟΣ
     13: ΤΑΞΙΔΙΑ-ΗΠΕΙΡΟΣ
@@ -32392,15 +32384,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 633
     1: ΜΑΛΑΜΑΣ,ΛΑΜΠΡΟΣ
     2: ΤΟ ΚΟΜΠΟΛΟΙ ΤΟΥ ΑΛΗ
     3: ΘΕΑΤΡΙΚΟ ΙΣΤΟΡΙΚΟ ΔΡΑΜΑ
-    4: 883.2 ΜΑΛ
+    4: 883.2ΜΑΛ
     5: 1523-5370
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1972'
     11: 90Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -32444,15 +32436,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 634
     1: ΜΑΛΑΜΑΣ,ΛΑΜΠΡΟΣ
     2: ΕΛΛΑΔΑ
     3: ΠΕΡΙΗΓΗΣΗ (1967-1974)
-    4: 914.95 ΜΑΛ
+    4: 914.95ΜΑΛ
     5: 360-361
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1974'
     11: 512Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
     13: ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
@@ -32651,15 +32643,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 638
     1: ΜΑΛΑΝΟΣ,ΤΙΜΟΣ
     2: ΔΕΙΓΜΑΤΟΛΟΓΙΟ
     3: ΚΡΙΤΙΚΑ ΔΙΑΦΟΡΑ
-    4: 880.3 ΜΑΛ
+    4: 880.3ΜΑΛ
     5: '2660'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 237Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΚΡΙΤΙΚΗ
@@ -32757,15 +32749,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 640
     1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞΑΝΔΡΟΣ
     2: ΓΕΩΡΓΙΟΣ ΚΑΣΤΡΙΩΤΗΣ
     3: ΣΚΕΝΤΕΡΜΠΕΗΣ
-    4: 938.4 ΜΑΜ
+    4: 938.4ΜΑΜ
     5: 2026-2027-9247
     8: X.E
     9: ΑΘΗΝΑ
     10: '1968'
     11: 34Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΟΠΛΑΡΧΗΓΟΣ
     13: ΟΠΛΑΡΧΗΓΟΣ-ΚΑΣΤΡΙΩΤΗΣ
@@ -32810,15 +32802,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 641
     1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞ Χ.
     2: ΣΧΟΛΕΙΑ ΚΑΙ ΔΙΔΑΣΚΑΛΟΙ ΤΟΥ ΑΛΥΤΡΩΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-    4: 938.5 ΜΑΜ
+    4: 938.5ΜΑΜ
     5: 2040-2041-9271
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 38Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΙΔΕΙΑ
     13: ΠΑΙΔΕΙΑ-ΔΙΔΑΣΚΑΛΟΙ
@@ -32862,15 +32854,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 642
     1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞ Χ.
     2: Ο ΑΠΟΣΤΟΛΟΣ ΑΡΣΑΚΗΣ ΚΑΙ Η ΦΙΛΕΚΠΑΙΔΕΥΤΙΚΗ ΕΤΑΙΡΕΙΑ
-    4: 938 ΜΑΜ
+    4: 938ΜΑΜ
     5: 2044-2045-9262
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 53Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΣΑΚΗΣ
     13: ΑΡΣΑΚΗΣ-ΦΙΛΕΚΠΑΙΔΕΥΤΙΚΗ ΕΤΑΙΡΕΙΑ
@@ -32916,15 +32908,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 643
     1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞΑΝΔΡΟΣ Χ.
     2: ΗΠΕΙΡΟΣ ΚΑΙ ΛΑΚΩΝΙΑ ΑΠΟ ΤΗΝ ΣΠΛΑΝΤΖΑ
     3: ΕΩΣ ΤΟΝ ΑΥΤΟΝΟΜΙΑΚΟΝ ΑΓΩΝΑ 1914
-    4: 938.68 ΜΑΜ
+    4: 938.68ΜΑΜ
     5: 2042-2043-9250Α
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1968'
     11: 38Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΛΑΚΩΝΙΑ
@@ -32970,15 +32962,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 644
     1: ΜΑΝΘΟΣ,ΑΛΚΗΣ
     2: ΘΩΜΑΣ ΠΑΣΧΙΔΗΣ
     3: ΗΠΕΙΡΩΤΑΙ ΔΗΜΟΣΙΟΓΡΑΦΟΙ ΣΤΗ ΡΟΥΜΑΝΙΑ
-    4: 938 ΜΑΝ
+    4: 938ΜΑΝ
     5: 2032-2033-9261
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 56Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΔΗΜΟΣΙΟΓΡΑΦΟΙ
     13: ΗΠΕΙΡΟΣ-ΔΗΜΟΣΙΟΓΡΑΦΟΙ
@@ -33022,15 +33014,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 645
     1: ΜΑΝΘΟΣ,ΑΛΚΗΣ
     2: ΗΠΕΙΡΩΤΑΙ ΕΙΣ ΤΗΝ ΡΟΥΜΑΝΙΑΝ
-    4: 938 ΜΑΝ
+    4: 938ΜΑΝ
     5: 2034-2035-9249
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 51Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΕΣ
@@ -33167,15 +33159,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 648
     1: ΜΑΝΟΣ,ΜΙΧΑΗΛ ΧΑΡ
     2: ΗΠΕΙΡΩΤΙΚΗ ΑΝΘΟΛΟΓΙΑ
-    4: 938.93 ΜΑΝ
+    4: 938.93ΜΑΝ
     5: '2154'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1955'
     11: 224Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΑΝΘΟΛΟΓΙΑ
@@ -33272,15 +33264,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 650
     1: ΜΑΝΟΥΣΑΚΑΣ,Μ.Ι
     2: Η ΕΝ ΚΡΗΤΗ ΣΥΝΩΜΟΣΙΑ ΤΟΥ ΣΗΦΗ ΒΛΑΣΤΟΥ (1453-1454)
     3: ΚΑΙ Η ΝΕΑ ΣΥΝΩΜΟΤΙΚΗ ΚΙΝΗΣΙΣ ΤΟΥ (1460-1462)
-    4: 938.42 ΜΑΝ
+    4: 938.42ΜΑΝ
     5: '1906'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1960'
     11: 168Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ-ΚΡΗΤΗ
     13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΚΡΗΤΗ
@@ -33323,15 +33315,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 651
     1: ΜΑΡΑΖΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
     2: Ο ΗΠΕΙΡΩΤΗΣ ΕΘΝΑΠΟΣΤΟΛΟΣ ΠΕΤΡΟΣ ΗΠΙΤΗΣ
-    4: 938.5 ΜΑΡ
+    4: 938.5ΜΑΡ
     5: 2061-2760-9258
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1973'
     11: 50Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΕΘΝΑΠΟΣΤΟΛΟΣ
     13: ΗΠΕΙΡΟΣ-ΗΠΙΤΗΣ
@@ -33374,15 +33366,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 652
     1: ΜΑΡΙΔΑΚΗΣ,ΓΕΩΡΓΙΟΣ
     2: Η ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΙΣ ΩΣ ΕΚΦΡΑΣΙΣ ΤΟΥ ΕΥΡΩΠΑΙΚΟΥ ΠΝΕΥΜΑΤΟΣ
-    4: 938.5 ΜΑΡ
+    4: 938.5ΜΑΡ
     5: '2126'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1951'
     11: 21Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ
     13: ΕΠΑΝΑΣΤΑΣΗ-ΕΛΛΗΝΙΚΗ
@@ -33428,15 +33420,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 653
     1: ΜΑΡΚΑΝΤΩΝΑΤΟΣ,ΔΙΟΝΥΣΙΟΣ
     2: ΑΛΕΞΑΝΔΡΟΣ
     3: ΤΡΑΓΩΔΙΑ
-    4: 886.2 ΜΑΡ
+    4: 886.2ΜΑΡ
     5: '1526'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 73Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
@@ -33526,15 +33518,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 655
     1: ΜΑΡΚΟΓΙΑΝΝΗΣ,ΧΡΗΣΤΟΣ
     2: ΕΘΝΙΚΑΙ ΑΝΑΞΙΟΤΗΤΕΣ
-    4: 938.8 ΜΑΡ
+    4: 938.8ΜΑΡ
     5: '2230'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1981'
     11: 55Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΘΝΙΚΑ
     13: ΕΘΝΙΚΕΣ ΑΝΑΞΙΟΤΗΤΕΣ
@@ -33680,15 +33672,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 658
     1: ΜΑΤΕΣΙ,ΑΝΤΩΝΙΟΣ
     2: Ο ΒΑΣΙΛΙΚΟΣ
-    4: 886.2 ΜΑΤ
+    4: 886.2ΜΑΤ
     5: '1477'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1964'
     11: 182Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -33729,15 +33721,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 659
     1: ΜΑΥΡΟΕΙΔΗΣ,ΦΑΝΗΣ
     2: ΣΥΜΒΟΛΗ ΣΤΗΝ ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΑΔΕΛΦΟΤΗΤΑΣ ΒΕΝΕΤΙΑΣ
     3: ΣΤΟ ΙΣΤ' ΑΙΩΝΑ
-    4: 938.4 ΜΑΥ
+    4: 938.4ΜΑΥ
     5: '2077'
     8: ΚΑΡΑΒΙΑ
     9: ΑΘΗΝΑ
     11: 372Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΔΕΛΦΟΤΗΤΑ ΒΕΝΕΤΙΑΣ
     13: ΑΔΕΛΦΟΤΗΤΑ ΒΕΝΕΤΙΑΣ
     6: null
@@ -33778,15 +33770,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 660
     1: ΜΑΥΡΟΧΑΛΥΒΙΔΗΣ,ΓΕΩΡΓΙΟΣ
     2: Η ΑΞΟ ΚΑΠΑΔΟΚΙΑΣ
-    4: 938.99 ΜΑΥ
+    4: 938.99ΜΑΥ
     5: 2442-2443-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1990'
     11: 338Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΠΑΔΟΚΙΑ-ΑΞΟ
     13: ΚΑΠΠΑΔΟΚΙΑ-ΑΞΟ
@@ -33927,15 +33919,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 663
     1: ΜΑΤΕΣΙΣ,ΠΑΥΛΟΣ
     2: ΒΙΟΧΗΜΕΙΑ ΚΑΙ Ο ΣΤΑΘΜΟΣ
-    4: 880.2 ΜΑΤ
+    4: 880.2ΜΑΤ
     5: '1361'
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 103Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
@@ -33980,15 +33972,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 664
     1: ΜΑΤΣΑΣ,ΑΛΕΞΑΝΔΡΟΣ
     2: ΚΡΟΙΣΟΣ
     3: ΕΜΜΕΤΡΟΝ ΔΡΑΜΑ ΕΙΣ ΠΡΑΞΕΙΣ ΤΡΕΙΣ
-    4: 881.2 ΜΑΤ
+    4: 881.2ΜΑΤ
     5: '1495'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1959'
     11: 84Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -34176,15 +34168,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 668
     1: ΜΕΛΑΣ,ΛΕΟΝΤΟΣ
     2: ΣΕΛΙΔΕΣ ΤΗΣ ΗΠΕΙΡΟΥ
-    4: 938.21 ΜΕΛ
+    4: 938.21ΜΕΛ
     5: '2179'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1963'
     11: 243Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ
@@ -34278,15 +34270,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 670
     1: ΜΕΛΑΣ,ΣΠΥΡΟΣ
     2: ΟΙ ΠΟΛΕΜΟΙ 1912-1913
-    4: 938.68 ΜΕΛ
+    4: 938.68ΜΕΛ
     5: '1988'
     8: ΜΠΙΡΗΣ
     9: ΑΘΗΝΑ
     10: '1958'
     11: 546Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΙ-(1912-1913)
     13: ΠΟΛΕΜΟΙ-(1912-1913)
@@ -34329,15 +34321,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 671
     1: ΜΕΛΑΣ,ΣΠΥΡΟΣ
     2: ΝΕΟΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-    4: 880.09 ΜΕΛ
+    4: 880.09ΜΕΛ
     5: '186'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 507Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΝΕΩΤΕΡΗ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΝΕΩΤΕΡΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -34681,15 +34673,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 678
     1: ΜΕΡΑΝΑΙΟΣ,Κ.Λ
     2: ΜΕΛΕΤΗΜΑΤΑ
-    4: 880.4 ΜΕΡ
+    4: 880.4ΜΕΡ
     5: '492'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1957'
     11: 127Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΜΕΛΕΤΗΜΑΤΑ
@@ -34732,15 +34724,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 679
     1: ΜΕΡΕΝΤΙΤΟΣ,ΙΩΑΝΝΗΣ ΚΩΝΣΤ
     2: ΣΥΓΚΡΙΣΙΣ ΤΟΥ "ΒΙΟΥ ΚΑΙΣΑΡΟΣ" ΠΑΡΑ ΣΟΥΗΤΩΝΙΩ ΠΡΟΣ ΤΟΝ
     3: '''ΒΙΟΝ ΚΑΙΣΑΡΟΣ"ΠΑΡΑ ΠΛΟΥΤΑΡΧΩ'
-    4: 920 ΜΕΡ
+    4: 920ΜΕΡ
     5: '2413'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1982'
     12: ΕΛΛΗΝΙΚΗ ΒΙΟΓΡΑΦΙΑ-ΠΛΟΥΤΑΡΧΟΣ
     13: ΠΛΟΥΤΑΡΧΟΣ-ΒΙΟΓΡΑΦΙΑ
     14: ΒΙΟΓΡΑΦΙΑ-ΠΛΟΥΤΑΡΧΟΣ
@@ -34832,15 +34824,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 681
     1: ΜΕΡΚΟΥΡΗΣ,ΣΤΑΜΑΤΗΣ Σ
     2: ΓΕΩΡΓΙΟΣ ΚΟΝΔΥΛΗΣ (1879-1936)
-    4: 938.6 ΜΕΡ
+    4: 938.6ΜΕΡ
     5: '1917'
     8: ΜΑΥΡΙΔΗΣ
     9: Χ.Τ
     10: '1954'
     11: 258Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΠΡΟΣΩΠΑ-ΚΟΝΔΥΛΗΣ
@@ -34937,15 +34929,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 683
     1: ΜΗΤΣΑΚΗΣ,Κ
     2: ΝΕΟΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
     3: Η ΓΕΝΙΑ ΤΟΥ '30
-    4: 880.3 ΜΗΤ
+    4: 880.3ΜΗΤ
     5: 212-213
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 161Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-Η ΓΕΝΙΑ ΤΟΥ '30
@@ -34990,15 +34982,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 684
     1: ΜΗΤΣΟΠΟΥΛΟΣ,ΦΑΝΗΣ Γ
     2: Ο ΡΟΒΑΣ
     3: ΤΡΑΓΩΔΙΑ
-    4: 881.2 ΜΗΤ
+    4: 881.2ΜΗΤ
     5: '2677'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 142Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
@@ -35039,15 +35031,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 685
     1: ΜΗΤΣΟΤΑΚΗΣ,ΚΥΡΙΑΚΟΣ
     2: ΠΡΟΣΩΠΑ ΚΑΙ ΤΟΠΟΙ
-    4: 889.21 ΜΗΤ
+    4: 889.21ΜΗΤ
     5: '2533'
     8: ΑΙΓΑΓΡΟΣ
     9: ΑΘΗΝΑ
     10: '1966'
     11: 116Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΠΡΟΣΩΠΑ-ΕΛΛΑΔΑ
@@ -35196,15 +35188,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 688
     1: ΜΙΛΛΕΡ,ΟΥΙΛΛΙΑΜ
     2: Η ΤΟΥΡΚΙΑ ΚΑΤΑΡΡΕΟΥΣΑ ΙΣΤΟΡΙΑ ΤΗΣ ΟΘΩΜΑΝΙΚΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
-    4: 956.1 ΜΙΛ
+    4: 956.1ΜΙΛ
     5: '2301'
     6: ΛΑΜΠΡΟΥ,ΣΠΥΡ.
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1914'
     11: 704Σ
     12: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-(1801-1913)
@@ -35298,15 +35290,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 690
     1: ΜΙΣΑΗΛΙΔΗΣ,ΧΑΡΙΤΩΝΟΣ
     2: ΤΟ ΘΕΑΤΡΟ ΤΗΣ ΠΟΛΗΣ (1800-1900)
-    4: 886.2 ΜΙΣ
+    4: 886.2ΜΙΣ
     5: '1421'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1960'
     11: 12Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΟΛΗ(1800-1900)
@@ -35347,15 +35339,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 691
     1: ΜΙΤΑΚΗΣ,ΔΙΟΝΥΣΗΣ
     2: ΓΙΑΝΝΑΚΗΣ ΣΟΥΛΤΑΝΗΣ
-    4: 938.4 ΜΙΤ
+    4: 938.4ΜΙΤ
     5: '2605'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1971'
     11: 21Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΠΡΟΣΩΠΑ-ΣΟΥΛΤΑΝΗΣ
@@ -35398,15 +35390,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 692
     1: ΜΙΤΣΟΥ,ΜΑΡΚΕΛΟΥ Θ
     2: Η ΕΚΣΤΡΑΤΕΙΑ ΤΟΥ ΚΛΕΥΜΕΝΟΥΣ ΚΑΤΑ ΤΟΥ ΑΡΓΟΥΣ
-    4: 938.15 ΜΙΤ
+    4: 938.15ΜΙΤ
     5: '2320'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1979'
     11: 6Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΚΣΤΡΑΤΕΙΑ-ΚΛΕΟΜΕΝΟΥΣ
     13: ΕΚΣΤΡΑΤΕΙΑ-ΚΛΕΟΜΕΝΟΥΣ
@@ -35449,15 +35441,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 693
     1: ΜΙΧΑΗΛΙΔΗΣ-ΚΡΙΝΑΙΟΣ,ΜΠΑΜΠΗΣ
     2: Η ΜΕΤΑΒΟΛΗ ΤΗΣ ΔΟΜΗΣ ΤΟΥ ΜΕΤΑΠΟΛΕΜΙΚΟΥ ΜΥΘΙΣΤΟΡΗΜΑΤΟΣ ΚΑΙ
     3: Η ΝΕΟΕΛΛΗΝΙΚΗ ΚΟΙΝΩΝΙΑ
-    4: 880.3 ΜΙΧ
+    4: 880.3ΜΙΧ
     5: '219'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΜΕΤΑΒΟΛΗ
     14: ΜΥΘΙΣΤΟΡΗΜΑ-ΔΟΜΗ
@@ -35550,15 +35542,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 695
     1: ΜΟΛΙΕΡΟΥ
     2: ΝΤΟΝ ΖΟΥΑΝ
-    4: 842 ΜΟΛ
+    4: 842ΜΟΛ
     5: '1439'
     6: ΠΡΕΒΕΛΑΚΗΣ,ΠΑΝΤΕΛΗΣ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1973'
     12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΓΑΛΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -35599,15 +35591,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 696
     1: ΜΟΛΟΣΣΟΣ,ΖΩΤΟΣ
     2: ΗΠΕΙΡΩΤΙΚΑΙ ΜΕΛΕΤΑΙ
-    4: 938.21 ΜΟΛ
+    4: 938.21ΜΟΛ
     5: '2178'
     8: ΑΝΤΩΝΙΑΔΗ
     9: ΑΘΗΝΑ
     10: '1875'
     11: 144Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΜΕΛΕΤΕΣ
@@ -35649,15 +35641,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 697
     1: ΜΟΣΤΡΑΤΟΥ,ΣΜΑΡΑΓΔΑ
     2: ΚΑΡΓΚΕΖΕ
     3: ΤΟ ΕΛΛΗΝΙΚΟ ΧΩΡΙΟ
-    4: 914 ΜΟΣ
+    4: 914ΜΟΣ
     5: '425'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 105Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΑΡΓΚΕΖΕ
     13: ΤΑΞΙΔΙΑ-ΚΑΡΓΚΕΖΕ
@@ -35698,15 +35690,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 698
     1: ΜΟΥΓΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
     2: Ο ΒΟΛΙΩΤΙΚΟΣ ΠΟΛΙΤΙΣΜΟΣ ΤΟΥ ΜΕΣΟΠΟΛΕΜΟΥ
-    4: 938.7 ΜΟΥ
+    4: 938.7ΜΟΥ
     5: '1653'
     8: ΠΥΛΗ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 110Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΛΟΣ
     13: ΒΟΛΟΣ-ΠΟΛΙΤΙΣΜΟΣ
@@ -35747,15 +35739,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 699
     1: ΜΟΥΓΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
     2: ΜΟΝΟΠΑΤΙΑ ΤΟΥ ΒΙΟΥ
-    4: 910 ΜΟΥ
+    4: 910ΜΟΥ
     5: '1669'
     8: ΠΥΛΗ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 126Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΩΤΙΚΑ
     13: ΤΑΞΙΩΤΙΚΑ-ΓΕΩΓΡΑΦΙΑ
@@ -35798,15 +35790,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 700
     1: ΜΟΥΓΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
     2: ΠΤΥΧΕΣ ΤΟΥ ΒΟΛΙΩΤΙΚΟΥ ΠΟΛΙΤΙΣΜΟΥ
-    4: 938.7 ΜΟΥ
+    4: 938.7ΜΟΥ
     5: '1691'
     8: Χ.Ε
     9: ΒΟΛΟΣ
     10: '1992'
     11: 254Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΛΟΣ
     13: ΒΟΛΟΣ-ΠΟΛΙΤΙΣΜΟΣ (1940-1990)
@@ -36026,36 +36018,35 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 705
   authors:
-  - ΜΟΥΡΑΤ,ΤΖΟΝ
+  - MURAT,JOHN
   title: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
   subtitle: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  dewey: 938 MUR
   entry_numbers:
   - '2082'
   - '1950'
   edition_year: 1982
   pages: 542
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΕΛΛΗΝΙΣΜΟΣ
   - ΞΕΚΛΗΡΙΣΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 705
-    1: ΜΟΥΡΑΤ,ΤΖΟΝ
+    1: MURAT,JOHN
     2: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
     3: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-    4: 938 MUR
+    4: 938.ΟΟ1MUR
     5: 2082-1950
     8: Χ.Ε
     9: Χ.Τ
     10: '1982'
     11: 542Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
     13: ΕΛΛΗΝΙΣΜΟΣ-ΞΕΚΛΗΡΙΣΜΑ
@@ -36296,15 +36287,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 710
     1: ΜΟΥΣΕΛΙΜΗΣ,ΣΠΥΡΟΣ Γ.
     2: ΑΡΧΑΙΟΤΗΤΕΣ ΤΗΣ ΘΕΣΠΡΩΤΙΑΣ
-    4: 938.21 ΜΟΥ
+    4: 938.21ΜΟΥ
     5: '2349'
     8: Χ.Ε
     9: ΓΙΑΝΝΙΝΑ
     10: '1980'
     11: 319Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΠΡΩΤΙΑ
     13: ΘΕΣΠΡΩΤΙΑ-ΑΡΧΑΙΟΤΗΤΕΣ
@@ -36348,15 +36339,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 711
     1: ΜΟΥΣΤΑΚΗΣ,ΒΑΣ
     2: ΠΝΕΥΜΑ ΚΑΙ ΠΗΛΟΣ
     3: ΚΡΙΤΙΚΑ ΚΕΙΜΕΝΑ
-    4: 880.4 ΜΟΥ
+    4: 880.4ΜΟΥ
     5: '2705'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1980'
     11: 79Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΗΛΟΣ
     13: ΠΗΛΟΣ-ΛΟΓΟΤΕΧΝΙΑ
@@ -36496,15 +36487,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 714
     1: ΜΠΑΚΟΓΙΑΝΝΗΣ,ΣΤΕΦΑΝΟΣ
     2: ΕΝΤΥΠΩΣΕΙΣ ΣΚΕΨΕΙΣ ΣΥΜΠΕΡΑΣΜΑΤΑ ΑΠΟ ΤΟ ΙΣΡΑΗΛ
-    4: 950 ΜΠΑ
+    4: 950ΜΠΑ
     5: 2526-2556
     8: Χ.Ε
     9: ΑΡΤΑ
     10: '1965'
     11: 51Σ
     12: ΙΣΡΑΗΛΙΝΗ ΙΣΤΟΡΙΑ
     13: ΙΣΡΑΗΛ-ΙΣΤΟΡΙΑ
@@ -36746,15 +36737,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 719
     1: ΜΠΕΡΤΩ,ΣΙΜΟΝ
     2: ΕΝΤΙΘ ΠΙΑΦ
-    4: 840 ΜΠΕ
+    4: 840ΜΠΕ
     5: '2631'
     6: ΑΞΙΩΤΗ,ΜΕΛΠΩ
     8: ΡΑΠΠΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 504Σ
     12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΒΙΟΓΡΑΦΙΑ
@@ -36796,15 +36787,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 720
     1: ΜΠΙΝΙΑΡΗΣ,ΓΚΙΚΑΣ
     2: ΕΚΑΤΟ ΧΡΟΝΙΑ ΘΕΑΤΡΙΚΗΣ ΠΕΙΡΑΙΚΗΣ ΖΩΗΣ
-    4: 886.2 ΜΠΙ
+    4: 886.2ΜΠΙ
     5: '2720'
     8: Χ.Ε
     9: ΠΕΙΡΑΙΑΣ
     10: '1976'
     11: 35Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΕΙΡΑΙΑΣ
@@ -37047,15 +37038,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 725
     1: ΜΠΟΥΡΑΝΤΑΣ,ΛΑΜΠΡΟΣ Κ
     2: Ο ΑΜΒΡΑΚΙΚΟΣ ΚΟΛΠΟΣ ΚΑΙ ΑΙ ΓΥΡΩΘΕΝ ΑΥΤΟΥ ΛΙΜΝΟΘΑΛΑΣΣΑ
-    4: 938 ΜΠΟ
+    4: 938ΜΠΟ
     5: 2487-2524
     8: Χ.Ε
     9: ΑΡΤΑ
     10: '1982'
     11: 24Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
     13: ΑΡΤΑ-ΑΜΒΡΑΚΙΚΟΣ ΚΟΛΠΟΣ
@@ -37150,15 +37141,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 727
     1: ΜΠΡΕΔΗΜΑΣ,ΠΙΝΔΑΡΟΣ
     2: ΜΑΡΤΙΝΟΣ ΛΟΥΘΗΡΟΣ
     3: ΙΣΤΟΡΙΚΟ ΔΡΑΜΑ
-    4: 886.2 ΜΠΡ
+    4: 886.2ΜΠΡ
     5: '1501'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1958'
     11: 95Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -37203,15 +37194,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 728
     1: ΜΠΡΕΔΗΜΑΣ,ΠΙΝΔΑΡΟΣ
     2: ΠΕΛΟΠΟΝΝΗΣΙΑΚΟΣ ΠΟΛΕΜΟΣ
     3: ΙΣΤΟΡΙΚΟ ΔΡΑΜΑ
-    4: 881.2 ΜΠΡ
+    4: 881.2ΜΠΡ
     5: '1502'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1959'
     11: 83Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΗ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ-ΔΡΑΜΑ
@@ -37255,15 +37246,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 729
     1: ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
     2: Η ΜΑΝΑ ΚΟΥΡΑΓΙΟ ΚΑΙ ΤΑ ΠΑΙΔΙΑ ΤΗΣ
-    4: 832 ΜΠΡ
+    4: 832ΜΠΡ
     5: '1558'
     6: ΑΡΖΟΓΛΟΥ,ΙΟΡΔΑΝΗΣ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Ε
     11: 162Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -37309,15 +37300,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 730
     1: ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
     2: ΤΡΟΜΟΣ ΚΑΙ ΑΘΛΙΟΤΗΤΑ ΤΟΥ ΤΡΙΤΟΥ ΡΑΙΧ
-    4: 832 ΜΠΡ
+    4: 832ΜΠΡ
     5: '1575'
     6: ΒΕΡΥΚΟΚΑΚΗ,ΑΓΓΕΛΑ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 145Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -37363,15 +37354,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 731
     1: ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΝΤ
     2: Ο ΚΑΛΟΣ ΑΝΘΡΩΠΟΣ ΤΟΥ ΣΕΤΣΟΥΑΝ
-    4: 832 ΜΠΡ
+    4: 832ΜΠΡ
     5: '1572'
     6: ΠΛΩΡΙΤΗΣ,ΜΑΡΙΟΣ
     8: ΙΘΑΚΗ
     9: ΑΘΗΝΑ
     10: '1980'
     11: 135Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -37418,15 +37409,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 732
     1: ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
     2: Ο ΚΑΥΚΑΣΙΑΝΟΣ ΚΥΚΛΟΣ ΜΕ ΤΗ ΚΙΜΩΛΙΑ
-    4: 832 ΜΠΡ
+    4: 832ΜΠΡ
     5: '1573'
     6: ΒΑΜΒΑΛΗΣ,ΓΙΩΡΓΟΣ
     7: 4ΕΚΔ
     8: ΜΟΥΚΟΥΜΑΝΗ
     9: ΑΘΗΝΑ
     10: '1970'
     11: 164Σ
@@ -37470,15 +37461,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 733
     1: ΜΥΛΩΝΑΣ,ΠΟΛΥΣ
     2: ΠΟΛΩΝΙΑ,ΣΥΡΙΑ
     3: ΤΑΞΙΔΕΥΟΝΤΑΣ
-    4: 914.49 ΜΥΛ
+    4: 914.49ΜΥΛ
     5: '426'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1982'
     11: 131Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΠΟΛΩΝΙΑ
     13: ΤΑΞΙΔΙΑ-ΠΟΛΩΝΙΑ
@@ -38066,15 +38057,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 745
     1: ΜΥΡΤΙΩΤΙΣΣΑ
     2: ΤΡΑΓΟΥΔΙΑ
-    4: 782.42 ΜΥΡ
+    4: 782.42ΜΥΡ
     5: '2626'
     8: ΤΥΠΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 31Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -38116,15 +38107,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 746
     1: ΜΩΥΣΕΙΔΗΣ,ΣΤΥΛ Μ
     2: '"ΑΥΤΟΚΡΑΤΩΡ ΘΕΣΣΑΛΟΝΙΚΗΣ"'
-    4: 886.2 ΜΩΥ
+    4: 886.2ΜΩΥ
     5: 1687-1486
     8: ΒΑΚΩΝ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 90Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΔΡΑΜΑ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -38315,15 +38306,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 750
     1: ΙΩΑΝΝΙΔΗΣ,ΛΑΚΗ Α
     2: ΕΥΡΩΠΗ
     3: ΣΚΕΨΕΙΣ ΔΙΑ ΤΗΝ ΙΔΕΑΝ ΤΗΣ ΕΝΩΣΕΩΣ ΤΗΣ
-    4: 914 ΙΩΑ
+    4: 914ΙΩΑ
     5: '2775'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1968'
     11: 173Σ
     12: ΠΑΓΚΟΣΜΙΑ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
     13: ΕΥΡΩΠΗ-ΙΣΤΟΡΙΑ
@@ -38516,15 +38507,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 754
     1: ΚΙΤΣΟΥ-ΠΙΤΟΥΛΗ,ΧΡΙΣΤΙΝΑ
     2: ΗΠΕΙΡΩΤΕΣ ΕΚΔΟΤΕΣ ΚΑΙ ΤΥΠΟΓΡΑΦΟΙ ΤΗΣ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
-    4: 938.4 ΚΙΤ
+    4: 938.4ΚΙΤ
     5: 2725-2726
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1980'
     11: 286Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΤΟΥΡΚΟΚΡΑΤΙΑ
     13: ΗΠΕΙΡΟΣ-ΤΟΥΡΚΟΚΡΑΤΙΑ
@@ -38568,15 +38559,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 755
     1: ΚΑΛΥΔΟΠΟΥΛΟΣ,Γ.Δ
     2: ΤΟ ΕΛΛΗΝΙΚΟ ΧΩΡΙΟ
     3: ΑΝΑΓΚΗ ΔΙΑΣΩΣΕΩΣ ΤΟΥ ΔΙΑΜΑΝΤΕΝΙΟΥ ΑΥΤΟΥ ΘΕΜΕΛΙΟΥ ΤΟΥ ΕΛΛΗΝΙΚ
-    4: 938 ΚΑΛ
+    4: 938ΚΑΛ
     5: '2774'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1961'
     11: 278Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΧΩΡΙΟ
     13: ΧΩΡΙΟ-ΕΛΛΑΔΑ
@@ -38667,15 +38658,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 757
     1: ΛΥΚΙΣΣΑΣ,ΜΙΧΑΛΗΣ Γ
     2: Η ΙΣΤΟΡΙΑ ΤΗΣ ΙΟΝΙΟΥ ΑΚΑΔΗΜΙΑΣ
-    4: 938 ΛΥΚ
+    4: 938ΛΥΚ
     5: '2805'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1993'
     11: 84Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΟΝΙΟΣ ΑΚΑΔΗΜΙΑ
     13: ΙΟΝΙΟΣ ΑΚΑΔΗΜΙΑ-ΙΣΤΟΡΙΑ
@@ -38820,15 +38811,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 760
     1: ΜΑΥΡΟΥΛΙΔΟΥ,ΛΟΥΛΑ
     2: ΤΟ ΚΟΥΡΣΕΜΑ ΤΗΣ ΠΟΛΗΣ ΑΠ'ΤΟΥΣ ΦΡΑΓΚΟΥΣ ΚΑΙ ΣΤΕΡΓΙΩΜΑ ΤΟΥΣ
     3: ΣΤΟΝ ΕΛΛΗΝΙΚΟ ΝΟΤΙΑ
-    4: 889.21 ΜΑΥ
+    4: 889.21ΜΑΥ
     5: '2549'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1957'
     11: 305Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
     13: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΦΡΑΓΚΟΙ
@@ -38971,15 +38962,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 763
     1: ΝΑΚΟΣ,ΓΡΗΓΟΡΙΟΣ ΧΡ
     2: Η ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΤΗΣ
     3: ΑΠΟ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΤΩΝ ΚΑΘ'ΗΜΑΣ
-    4: 938.21 ΝΑΚ
+    4: 938.21ΝΑΚ
     5: '2518'
     8: Χ.Ε
     9: ΑΡΤΑ
     10: '1969'
     11: 144Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΑΡΤΑ
@@ -39055,14 +39046,15 @@
   authors:
   - ΝΑΛΤΣΑΣ,ΧΡΙΣΤΟΦΟΡΟΣ Α.
   title: ΦΙΛΙΠΠΟΣ Β' Ο ΜΑΚΕΔΩΝ
   subtitle: Ο ΕΝΩΤΗΣ ΤΩΝ ΕΛΛΗΝΩΝ
   dewey: 938.171 ΝΑΛ
   entry_numbers:
   - '1951'
+  - '15688'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1970
   pages: 885
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΑΚΕΔΟΝΙΑ
   - ΦΙΛΙΠΠΟΣ Β
@@ -39072,15 +39064,15 @@
   offprint: false
   original_entry:
     0: 765
     1: ΝΑΛΤΣΑΣ,ΧΡΙΣΤΟΦΟΡΟΣ Α.
     2: ΦΙΛΙΠΠΟΣ Β' Ο ΜΑΚΕΔΩΝ
     3: Ο ΕΝΩΤΗΣ ΤΩΝ ΕΛΛΗΝΩΝ
     4: 938.171ΝΑΛ
-    5: '1951'
+    5: 1951-15688
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1970'
     11: 885Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ-ΦΙΛΙΠΠΟΣ Β'
     13: ΜΑΚΕΔΟΝΙΑ-ΦΙΛΙΠΠΟΣ Β'
     14: ΦΙΛΙΠΠΟΣ Β'
@@ -39221,15 +39213,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 768
     1: ΝΕΖΕΡΙΤΟΣ,ΑΓΓΕΛΟΣ
     2: '"ΕΝΟΤΗΣ ΠΑΝΤΩΝ ΤΩΝ ΕΛΛΗΝΩΝ ΜΟΝΗ ΣΩΤΗΡΙΑ ΤΗΣ ΠΑΤΡΙΔΑΣ"'
     3: Ο ΣΛΑΒΙΚΟΣ ΚΙΝΔΥΝΟΣ
-    4: 938 ΝΕΖ
+    4: 938ΝΕΖ
     5: '2345'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1947'
     11: 47Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-Ο ΣΛΑΒΙΚΟΣ ΚΙΝΔΥΝΟΣ
     13: ΣΛΑΒΙΚΟΣ ΚΙΝΔΥΝΟΣ
@@ -39321,15 +39313,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 770
     1: ΝΙΚΟΛΑΟΥ,Χ.Ν
     2: ΕΠΙΤΙΜΟΣ ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ ΕΙΣ ΕΡΩΤΗΣΕΙΣ
-    4: 938 ΝΙΚ
+    4: 938ΝΙΚ
     5: '2336'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 178Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΡΩΤΗΣΕΙΣ
     13: ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΡΩΤΗΣΕΙΣ
@@ -39666,15 +39658,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 777
     1: ΝΤΟΡΕΝ,ΚΑΡΛ
     2: ΣΥΝΤΟΜΗ ΙΣΤΟΡΙΑ ΤΗΣ ΑΜΕΡΙΚΑΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-    4: 810 ΝΤΟ
+    4: 810ΝΤΟ
     5: '381'
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1953'
     11: 122Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
     3: null
@@ -39716,15 +39708,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 778
     1: ΝΤΟΥΡΑΝ,ΓΟΥΙΛ
     2: ΕΚΦΡΑΣΕΙΣ ΤΗΣ ΖΩΗΣ
-    4: 800 ΝΤΟ
+    4: 800ΝΤΟ
     5: 1255-2701
     6: ΜΑΡΔΑ,ΕΛΕΝΗ
     8: ΜΠΕΡΓΑΔΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 394Σ
     12: ΠΑΓΚΟΣΜΙΑ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -39817,15 +39809,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 780
     1: ΝΟΥΤΣΟΣ,ΠΑΝΑΓΙΩΤΗΣ ΧΡ
     2: ΟΥΤΟΠΙΑ ΚΑΙ ΙΣΤΟΡΙΑ
-    4: 938 ΝΟΥ
+    4: 938ΝΟΥ
     5: '2367'
     8: ΚΕΔΡΟΣ
     9: ΑΘΗΝΑ
     10: '1979'
     11: 186Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΟΥΤΟΠΙΑ
     13: ΟΥΤΟΠΙΑ ΚΑΙ ΙΣΤΟΡΙΑ
@@ -39971,15 +39963,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 783
     1: ΝΤΟΒΑΣ,ΙΩΑΝΝΗΣ Ν
     2: ΟΙ ΝΤΟΒΑΙΟΙ
     3: ΛΗΣΜΟΝΗΜΕΝΟΙ ΖΥΓΙΩΤΕΣ ΑΓΩΝΙΣΤΕΣ
-    4: 938.5 ΝΤΟ
+    4: 938.5ΝΤΟ
     5: '1901'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1965'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΩΝΙΣΤΕΣ 1821
     13: 1821-ΑΓΩΝΙΣΤΕΣ
     14: ΝΤΟΒΑΙΟΙ-ΑΓΩΝΙΣΤΕΣ
@@ -40072,15 +40064,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 785
     1: ΝΤΥΡΡΕΝΜΑΤ,ΦΡΕΙΔΕΡΙΚΟΣ
     2: Η ΕΠΙΣΚΕΨΗ ΤΗΣ ΓΗΡΑΙΑΣ ΚΥΡΙΑΣ
-    4: 832 ΝΤΥ
+    4: 832ΝΤΥ
     5: '1368'
     6: ΑΜΑΝΑΚΗΣ,ΗΩ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 140Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -40173,15 +40165,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 787
     1: ΞΑΝΘΟΥΔΙΔΟΥ,ΣΤΕΦ
     2: ΕΠΙΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΚΡΗΤΗΣ
     3: ΑΠΟ ΤΗΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΤΩΝ ΚΑΘ'ΗΜΑΣ
-    4: 938.98 ΞΑΝ
+    4: 938.98ΞΑΝ
     5: '2074'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1909'
     11: 173Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΡΗΤΗ
     13: ΚΡΗΤΗ
@@ -40223,15 +40215,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 788
     1: ΞΕΝΟΣ,ΝΙΚΟΣ Γ
     2: ΠΤΥΧΕΣ ΕΥΡΩΠΗΣ
     3: ΟΔΟΙΠΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ
-    4: 940 ΞΕΝ
+    4: 940ΞΕΝ
     5: 387-2577
     8: ΚΑΣΤΑΛΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 280Σ
     12: ΕΥΡΩΠΑΙΚΗ ΙΣΤΟΡΙΑ-ΠΤΥΧΕΣ
     13: ΕΥΡΩΠΗ-ΠΤΥΧΕΣ
@@ -40373,15 +40365,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 791
     1: ΞΕΝΟΠΟΥΛΟΣ,ΓΡΗΓΟΡΗΣ
     2: Ο ΚΑΚΟΣ ΔΡΟΜΟΣ
-    4: 884.22 ΞΕΝ
+    4: 884.22ΞΕΝ
     5: '1049'
     7: 2ΕΚΔ
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1922'
     11: 102Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -40683,15 +40675,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 797
     1: ΟΙΚΟΝΟΜΟΥ,ΑΛΕΞΑΝΔΡΟΣ
     2: ΤΡΕΙΣ ΑΝΘΡΩΠΟΙ
     3: ΣΥΜΒΟΛΗ ΕΙΣ ΤΗΝ ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΛΑΟΥ (1780-1935)
-    4: 938.6 ΟΙΚ
+    4: 938.6ΟΙΚ
     5: '1809'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1950'
     11: 551Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΟΙΚΟΝΟΜΟΣ-ΙΣΤΟΡΙΑ
@@ -40785,15 +40777,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 799
     1: ΟΙΚΟΝΟΜΟΥ,ΓΕΩΡΓΙΟΣ
     2: ΙΣΤΟΡΙΑ ΤΩΝ ΤΡΙΩΝ ΕΛΙΣΑΒΕΤΕΙΩΝ ΠΑΡΘΕΝΑΓΩΓΕΙΩΝ ΤΩΝ ΙΩΑΝΝΙΝΩΝ
     3: ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ (1848-1913)
-    4: 938.4 ΟΙΚ
+    4: 938.4ΟΙΚ
     5: '2365'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1957'
     11: 91Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΩΑΝΝΙΝΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
     13: ΙΩΑΝΝΙΝΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
@@ -40942,15 +40934,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 802
     1: ΟΣΜΠΟΡΝ,ΤΖΩΝ
     2: ΞΕΝΟΔΟΧΕΙΟ ΣΤΟ ΑΜΣΤΕΡΝΤΑΜ ΚΑΙ ΤΩΡΙΝΟΣ ΚΑΙΡΟΣ
-    4: 822 ΟΣΜ
+    4: 822ΟΣΜ
     5: '1374'
     6: ΜΗΤΡΟΠΟΥΛΟΣ,ΚΩΣΤ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 175Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -40995,15 +40987,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 803
     1: ΟΣΤΡΟΓΚΟΣΚΗ,ΤΖΙΟΡΤΖΙΟ
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΒΥΖΑΝΤΙΝΟΥ ΚΡΑΤΟΥΣ
-    4: 938.3 ΟΣΤ
+    4: 938.3ΟΣΤ
     5: 1766-1767-
     6: ΠΑΝΑΓΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ
     8: ΒΑΣΙΛΟΠΟΥΛΟΣ
     9: ΑΘΗΝΑ
     10: '1979'
     11: 329Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
@@ -41094,15 +41086,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 805
     1: ΟΥΡΑΝΗΣ,ΚΩΣΤΑΣ
     2: ΙΣΠΑΝΙΑ
     3: ΤΑΞΙΔΙΑ
-    4: 889.21 ΟΥΡ
+    4: 889.21ΟΥΡ
     5: '396'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 352Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΙΣΠΑΝΙΑ
     13: ΤΑΞΙΔΙΑ-ΙΣΠΑΝΙΑ
@@ -41193,15 +41185,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 807
     1: ΟΥΡΑΝΗΣ,ΚΩΣΤΑΣ
     2: ΙΤΑΛΙΑ
     3: ΤΑΞΙΔΙΑ
-    4: 889.21 ΟΥΡ
+    4: 889.21ΟΥΡ
     5: '393'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 220Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΙΤΑΛΙΑ
     13: ΤΑΞΙΔΙΑ-ΙΤΑΛΙΑ
@@ -41242,15 +41234,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 808
     1: ΟΥΡΑΝΗΣ,ΚΩΣΤΑΣ
     2: ΕΛΛΑΔΑ
     3: ΤΑΞΙΔΙΑ
-    4: 899.21 ΟΥΡ
+    4: 899.21ΟΥΡ
     5: '373'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 425Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
     13: ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
@@ -41290,15 +41282,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 809
     1: ΟΥΩΛΤΕΡ,ΤΟΜΑΣ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΓΕΡΜΑΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-    4: 830 ΟΥΩ
+    4: 830ΟΥΩ
     5: '201'
     6: ΣΕΡΟΥΙΟΥ,Γ
     8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '1931'
     11: 280Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -41441,15 +41433,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 812
     1: ΠΑΛΑΙΟΛΟΓΟΣ,ΠΑΥΛΟΣ
     2: Η ΡΩΣΙΑ ΟΠΩΣ ΤΗΝ ΕΙΔΑ
-    4: 914.47 ΠΑΛ
+    4: 914.47ΠΑΛ
     5: '407'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1957'
     11: 170Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΡΩΣΙΑ
     13: ΤΑΞΙΔΙΑ-ΡΩΣΙΑ
@@ -41637,15 +41629,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 816
     1: ΠΑΛΑΜΑΣ,ΚΩΣΤΗΣ
     2: ΑΡΙΣΤΟΤΕΛΗΣ ΒΑΛΑΩΡΙΤΗΣ(1824-1924)
-    4: 889.25 ΠΑΛ
+    4: 889.25ΠΑΛ
     5: '997'
     8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '1924'
     11: 141Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΒΑΛΑΩΡΙΤΗΣ
@@ -41836,15 +41828,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 820
     1: ΠΑΜΠΟΥΚΗΣ,ΠΑΝΟΣ Χ
     2: ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
-    4: 938.99 ΠΑΜ
+    4: 938.99ΠΑΜ
     5: 369-2382
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1955'
     11: 115Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
     13: ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
@@ -41886,15 +41878,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 821
     1: ΠΑΝΑΣ,Κ.Ι.
     2: Η ΕΛΛΗΝΙΚΗ ΜΟΥΣΙΚΗ ΚΑΙ ΤΟ ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ
-    4: 782.42 ΠΑΝ
+    4: 782.42ΠΑΝ
     5: '714'
     8: ΚΑΓΙΑΦΑ
     9: ΑΘΗΝΑ
     10: '1958'
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
     14: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
@@ -42042,15 +42034,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 824
     1: ΠΑΝΑΓΙΩΤΟΠΟΥΛΟΣ,ΜΕΜΟΣ
     2: ΝΕΟΕΛΛΗΝΙΚΗ ΠΟΙΗΤΙΚΗ ΑΝΘΟΛΟΓΙΑ
-    4: 880.08 ΠΑΝ
+    4: 880.08ΠΑΝ
     5: 625-626-627-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 492Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΑΝΘΟΛΟΓΙΑ
@@ -42091,15 +42083,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 825
     1: ΠΑΝΑΓΙΩΤΟΠΟΥΛΟΣ,ΙΜ
     2: Η ΑΦΡΙΚΗ ΑΦΥΠΝΙΖΕΤΑΙ
-    4: 916 ΠΑΝ
+    4: 916ΠΑΝ
     5: '414'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1963'
     11: 199Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΑΦΡΙΚΗ
     13: ΤΑΞΙΔΙΑ-ΑΦΡΙΚΗ
@@ -42188,15 +42180,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 827
     1: ΠΑΝΑΓΙΩΤΟΠΟΥΛΟΣ,Ι.Μ.
     2: ΕΛΛΗΝΙΚΟΙ ΟΡΙΖΟΝΤΕΣ
-    4: 914.95 ΠΑΝ
+    4: 914.95ΠΑΝ
     5: '372'
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 413Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΗΝΙΚΟΙ ΟΡΙΖΟΝΤΕΣ
     13: ΤΑΞΙΔΙΑ-ΕΛΛΗΝΙΚΟΙ ΟΡΙΖΟΝΤΕΣ
@@ -42238,15 +42230,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 828
     1: ΠΑΝΑΓΙΩΤΟΠΟΥΛΟΣ,Ι.Μ
     2: ΤΑ ΠΡΟΣΩΠΑ ΚΑΙ ΤΑ ΚΕΙΜΕΝΑ
-    4: 880.4 ΠΑΝ
+    4: 880.4ΠΑΝ
     5: '2639'
     8: ΑΕΤΟΣ
     9: ΑΘΗΝΑ
     10: '1944'
     11: 258Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΡΟΣΩΠΑ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
@@ -42288,15 +42280,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 829
     1: ΠΑΝΙΤΣΑΣ,ΓΙΑΝΝΗΣ
     2: ΤΑΞΙΔΕΥΟΝΤΑΣ
     3: ΜΟΡΙΑΣ
-    4: 914.95 ΠΑΝ
+    4: 914.95ΠΑΝ
     5: '2574'
     8: Χ.Ε
     9: Χ.Τ
     10: '1965'
     11: 126Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΜΟΡΙΑΣ
     13: ΤΑΞΙΔΙΑ-ΜΟΡΙΑΣ
@@ -42386,15 +42378,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 831
     1: ΠΑΝΤΑΖΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ Ι.
     2: ΕΛΛΗΝΩΝ ΣΥΣΣΩΜΑΤΩΣΕΙΣ ΚΑΤΑ ΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑΝ
-    4: 938.4 ΠΑΝ
+    4: 938.4ΠΑΝ
     5: '1842'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1958'
     11: 39Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
     13: ΤΟΥΡΚΟΚΡΑΤΙΑ
@@ -42537,15 +42529,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 834
     1: ΠΑΝΤΑΖΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ Ι.
     2: ΚΟΙΝΟΤΙΚΟΣ ΒΙΟΣ ΕΙΣ ΤΗΝ ΘΕΤΤΑΛΟΜΑΓΝΗΣΙΑΝ ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑ
-    4: 938.4 ΠΑΝ
+    4: 938.4ΠΑΝ
     5: '1905'
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1967'
     11: 103Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
     13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΘΕΤΤΑΛΟΜΑΓΝΗΣΙΑ
@@ -42586,15 +42578,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 835
     1: ΠΑΝΣΕΛΗΝΟΣ,ΑΣΗΜΑΚΗΣ
     2: Η ΚΙΝΑ Η ΔΙΚΗ ΜΟΥ
-    4: 915.31 ΠΑΝ
+    4: 915.31ΠΑΝ
     5: '457'
     8: ΚΕΔΡΟΣ
     9: ΑΘΗΝΑ
     10: '1983'
     11: 140Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΙΝΑ
     13: ΤΑΞΙΔΙΑ-ΚΙΝΑ
@@ -42687,15 +42679,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 837
     1: ΠΑΝΤΟΠΟΥΛΟΣ,ΕΥΑΓ.
     2: Η ΝΥΦΗ ΤΗΣ ΚΟΥΛΟΥΡΗΣ
-    4: 880.2 ΠΑΝ
+    4: 880.2ΠΑΝ
     5: '1436'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 68Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -42740,15 +42732,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 838
     1: ΠΑΠΠΑΣ,ΣΤΕΦΑΝΟΣ Β.
     2: ΤΑ ΝΕΑ ΨΑΡΑ
     3: ΔΡΑΜΑ
-    4: 886.2 ΠΑΠ
+    4: 886.2ΠΑΠ
     5: '1476'
     8: ΚΑΓΙΑΦΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 32Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -42789,15 +42781,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 839
     1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ-ΦΙΛΙΑΣ,ΓΕΩΡΓΙΟΣ Β.
     2: ΕΛΠΙΔΕΣ-ΕΝΘΟΥΣΙΑΣΜΟΙ ΠΟΝΟΙ ΚΑΙ ΑΠΟΓΟΗΤΕΥΣΕΙΣ
-    4: 938.7 ΠΑΠ
+    4: 938.7ΠΑΠ
     5: '2551'
     8: ΑΝΤΙΚΟΣΜΟΙ
     9: ΑΘΗΝΑ
     10: '1992'
     11: 394Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΙΚΑ ΓΕΓΟΝΟΤΑ
     13: ΠΟΛΕΜΙΚΑ ΓΕΓΟΝΟΤΑ
@@ -42893,15 +42885,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 841
     1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΠΥΡΟΣ
     2: ΑΚΕΛ ΤΟ ΑΛΛΟ ΚΚΕ
-    4: 938.8 ΠΑΠ
+    4: 938.8ΠΑΠ
     5: 2312-2313
     8: ΛΑΔΙΑΣ
     9: ΑΘΗΝΑ
     10: '1984'
     11: 379Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΚΕΛ
     13: ΑΚΕΛ-ΙΣΤΟΡΙΑ
@@ -43105,15 +43097,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 845
     1: ΠΑΠΑΓΙΑΝΝΗΣ,ΓΕΩΡΓΙΟΣ ΕΠ.
     2: ΑΙ ΤΡΕΙΣ ΜΕΓΑΛΥΤΕΡΑΙ ΣΥΜΦΟΡΑΙ ΤΩΝ ΕΛΛΗΝΩΝ
     3: ΚΑΤΑ ΤΟΝ ΙΕΡΟΝ ΑΓΩΝΑ
-    4: 938.5 ΠΑΠ
+    4: 938.5ΠΑΠ
     5: '1847'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 500Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΕΡΟΣ ΑΓΩΝΑΣ
     13: ΙΕΡΟΣ ΑΓΩΝΑΣ
@@ -43155,15 +43147,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 846
     1: ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΤΑΚΗΣ Ε.
     2: ΕΛΛΑΣ-ΚΟΡΕΑ
     3: ΑΡΧΑΙΟΙ ΚΑΙ ΣΥΓΧΡΟΝΟΙ ΔΕΣΜΟΙ ΤΩΝ ΔΥΟ ΛΑΩΝ
-    4: 938 ΠΑΠ
+    4: 938ΠΑΠ
     5: '366'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1976'
     11: 272Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
     13: ΕΛΛΑΣ-ΚΟΡΕΑ
@@ -43207,15 +43199,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 847
     1: ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΤΑΚΗΣ Ε.
     2: Η ΕΠΟΠΟΙΙΑ ΤΟΥ ΜΠΙΖΑΝΙΟΥ
     3: ΗΘΙΚΟΣ ΘΡΙΑΜΒΟΣ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-    4: 938.68 ΠΑΠ
+    4: 938.68ΠΑΠ
     5: '1943'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1980'
     11: 51Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΠΙΖΑΝΙ
     13: ΜΠΙΖΑΝΙ-ΕΠΟΠΟΙΙΑ
@@ -43309,15 +43301,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 849
     1: ΠΑΠΑΔΑΚΗΣ,Β.Π.
     2: ΔΙΠΛΩΜΑΤΙΚΗ ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΠΟΛΕΜΟΥ 1940-1945
-    4: 938.75 ΠΑΠ
+    4: 938.75ΠΑΠ
     5: '2008'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1956'
     11: 510Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΙΠΛΩΜΑΤΙΑ
     13: ΔΙΠΛΩΜΑΤΙΚΗ ΙΣΤΟΡΙΑ-1940
@@ -43416,15 +43408,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 851
     1: ΠΑΠΑΔΗΜΗΤΡΙΟΥ,ΒΙΒΗ ΔΗΜ
     2: Η ΚΟΙΝΩΝΙΚΗ ΠΟΛΙΤΙΚΗ ΚΑΙ ΟΙ ΗΠΕΙΡΩΤΑΙ ΕΘΝΙΚΟΙ ΕΥΕΡΓΕΤΑΙ
-    4: 938 ΠΑΠ
+    4: 938ΠΑΠ
     5: 2038-2039-9270
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 26Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΟΙΝΩΝΙΚΗ ΠΟΛΙΤΙΚΗ
     13: ΠΟΛΙΤΙΚΗ -ΚΟΙΝΩΝΙΚΗ
@@ -43467,15 +43459,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 852
     1: ΠΑΠΑΔΗΜΗΤΡΙΟΥ,Γ.Α
     2: ΜΝΗΜΗ ΑΠΟΣΤΟΛΟΥ ΑΡΣΑΚΗ
-    4: 938 ΠΑΠ
+    4: 938ΠΑΠ
     5: '2051'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 69Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΠΡΟΣΩΠΑ=ΑΡΣΑΚΗΣ
@@ -43517,15 +43509,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 853
     1: ΠΑΠΑΔΗΜΗΤΡΙΟΥ,ΡΟΥΛΑ
     2: ΣΤΗΝ ΕΠΟΠΟΙΙΑ ΤΟΥ 40
-    4: 938.75 ΠΑΠ
+    4: 938.75ΠΑΠ
     5: '2009'
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1958'
     11: 108Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΟΠΟΙΙΑ ΤΟΥ 40
     13: ΕΠΟΠΟΙΙΑ-1940
@@ -44102,14 +44094,15 @@
   authors:
   - ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ
   title: ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
   dewey: 938.5 ΠΑΠ
   entry_numbers:
   - '2127'
   - '1852'
+  - '14176'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1969
   pages: 62
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΤΟΥΡΚΟΚΡΑΤΙΑ
   - ΑΓΩΝΕΣ
@@ -44118,16 +44111,16 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 865
     1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ
     2: ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
-    4: 938.5 ΠΑΠ
-    5: 2127-1852
+    4: 938.5ΠΑΠ
+    5: 2127-1852-14176
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1969'
     11: 62Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
     13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΑΓΩΝΕΣ
     14: ΑΓΩΝΕΣ-ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ
@@ -44149,15 +44142,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 866
   authors:
   - ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ Ι.
-  title: ΤΑ ΤΕΛΕΥΤΑΙ ΕΤΗ ΤΟΥ ΑΓΩΝΟΣ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ ΚΑΙ Η ΠΕΡΙΟΔΟΣ
+  title: ΤΑ ΤΕΛΕΥΤΑΙΑ ΕΤΗ ΤΟΥ ΑΓΩΝΟΣ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ ΚΑΙ Η ΠΕΡΙΟΔΟΣ
   subtitle: ΔΙΑΚΥΒΕΡΝΗΣΕΙΣ ΤΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
   dewey: 938.571 ΠΑΠ
   entry_numbers:
   - '1790'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1976
   pages: 131
@@ -44167,15 +44160,15 @@
   - ΑΝΕΞΑΡΤΗΣΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 866
     1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ Ι.
-    2: ΤΑ ΤΕΛΕΥΤΑΙ ΕΤΗ ΤΟΥ ΑΓΩΝΟΣ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ ΚΑΙ Η ΠΕΡΙΟΔΟΣ
+    2: ΤΑ ΤΕΛΕΥΤΑΙΑ ΕΤΗ ΤΟΥ ΑΓΩΝΟΣ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ ΚΑΙ Η ΠΕΡΙΟΔΟΣ
     3: ΔΙΑΚΥΒΕΡΝΗΣΕΙΣ ΤΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
     4: 938.571ΠΑΠ
     5: '1790'
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1976'
     11: 131Σ
@@ -44522,15 +44515,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 873
     1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΩΤΕΡΗΣ ΕΛΛΑΔΟΣ
-    4: 938.57 ΠΑΠ
+    4: 938.57ΠΑΠ
     5: '1853'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1983'
     11: 115Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΕΩΤΕΡΗ
     13: ΝΕΩΤΕΡΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
@@ -44573,15 +44566,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 874
     1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ
     2: ΣΥΜΜΕΙΚΤΑ ΝΕΩΤΕΡΗΣ ΙΣΤΟΡΙΑΣ
-    4: 938.6 ΠΑΠ
+    4: 938.6ΠΑΠ
     5: '1856'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1982'
     11: 111Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΕΩΤΕΡΗ
     13: ΝΕΩΤΕΡΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
@@ -44729,15 +44722,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 877
     1: ΠΑΠΑΖΟΓΛΟΥ,ΘΕΟΔΩΡΟΣ Π.
     2: Η ΦΙΛΙΑ ΕΙΝΑΙ ΣΥΜΦΕΡΟΝ
     3: ΚΩΜΩΔΙΑ
-    4: 886.2 ΠΑΠ
+    4: 886.2ΠΑΠ
     5: '1524'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1956'
     11: 74Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
@@ -44830,15 +44823,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 879
     1: ΠΑΠΑΘΑΝΑΣΟΠΟΥΛΟΣ,ΘΑΝΑΣΗΣ
     2: ΛΟΓΟΤΕΧΝΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
-    4: 880.4 ΠΑΠ
+    4: 880.4ΠΑΠ
     5: '195'
     8: ΘΟΥΚΥΔΙΔΗΣ
     9: ΑΘΗΝΑ
     10: '1982'
     11: 258Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΜΕΛΕΤΗΜΑΤΑ
@@ -44982,15 +44975,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 882
     1: ΠΑΠΑΘΕΟΔΩΡΟΥ,ΑΠΟΣΤ Π.
     2: ΣΥΜΒΟΛΗ ΣΤΗΝ ΝΕΩΤΕΡΗ ΙΣΤΟΡΙΑ ΤΗΣ ΠΕΡΙΟΧΗΣ ΔΩΔΩΝΗΣ
-    4: 938 ΠΑΠ
+    4: 938ΠΑΠ
     5: '2060'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1980'
     11: 34Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΩΔΩΝΗ
     13: ΔΩΔΩΝΗ-ΙΣΤΟΡΙΑ
@@ -45036,15 +45029,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 883
     1: ΠΑΠΑΙΩΑΝΝΟΥ,ΔΗΜΗΤΡΙΟΣ
     2: ΣΧΟΛΙΚΑ ΤΡΑΓΟΥΔΙΑ
-    4: 782.42 ΠΑΠ
+    4: 782.42ΠΑΠ
     5: 712-713
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1959'
     11: 18Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -45088,15 +45081,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 884
     1: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΣ,Θ.Φ
     2: Η ΜΑΧΗ ΤΗΣ ΕΛΛΑΔΟΣ(1940-1941)
-    4: 938.75 ΠΑΠ
+    4: 938.75ΠΑΠ
     5: 2602-1956
     8: ΓΑΛΑΞΙΑΣ
     9: ΑΘΗΝΑ
     10: '1966'
     11: 483Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-Η ΜΑΧΗ ΤΗΣ ΕΛΛΑΔΟΣ
     13: Η ΜΑΧΗ ΤΗΣ ΕΛΛΑΔΟΣ(1940-1941)
@@ -45193,15 +45186,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 886
     1: ΠΑΠΑΝΤΩΝΙΟΥ,ΓΕΩΡΓΙΟΣ
     2: ΑΡΧΑΙΑ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
-    4: 938.1 ΠΑΠ
+    4: 938.1ΠΑΠ
     5: 1913-1912-1927-1928-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1979'
     11: 717Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΜΥΔΙΚΟΙ-ΑΧΑΙΑ
@@ -45244,15 +45237,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 887
     1: ΠΑΠΑΠΑΝΑΓΙΩΤΟΥ,ΚΩΣΤΑΣ
     2: ΒΑΣΙΛΕΙΟΣ Ο ΒΟΥΛΓΑΡΟΚΤΟΝΟΣ
-    4: 886.2 ΠΑΠ
+    4: 886.2ΠΑΠ
     5: '1467'
     8: ΚΑΜΠΑΝΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 182Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΙΛΟΓΙΑ
@@ -45324,15 +45317,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 889
   authors:
   - ΠΑΠΑΣΤΡΑΤΟΣ,ΕΥΑΓΓΕΛΟΣ Α.
   title: Η ΔΟΥΛΕΙΑ ΚΙ Ο ΚΟΠΟΣ ΤΗΣ
-  dewey: 938.09 ΠΑΠ
+  dewey: 938.009 ΠΑΠ
   entry_numbers:
   - '2431'
   - '5748'
   editor: None // ΑΘΗΝΑ
   edition_year: 1964
   pages: 255
   topics:
@@ -45341,15 +45334,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 889
     1: ΠΑΠΑΣΤΡΑΤΟΣ,ΕΥΑΓΓΕΛΟΣ Α.
     2: Η ΔΟΥΛΕΙΑ ΚΙ Ο ΚΟΠΟΣ ΤΗΣ
-    4: 938.09ΠΑΠ
+    4: 938.009ΠΑΠ
     5: 2431-5748
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1964'
     11: 255Σ
     12: ΒΙΟΓΡΑΦΙΑ
     13: ΒΙΟΓΡΑΦΙΕΣ
@@ -45394,15 +45387,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 890
     1: ΠΑΠΑΣΤΑΥΡΟΣ,ΙΩΑΝΝΗΣ ΣΤ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΑΔΟΣ ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ
     3: ΜΕΧΡΙ ΤΩΝ ΠΑΡΑΜΟΝΩΝ ΤΗΣ ΡΩΜΑΙΚΗΣ ΚΥΡΙΑΡΧΙΑΣ
-    4: 938.1 ΠΑΠ
+    4: 938.1ΠΑΠ
     5: '1910'
     8: ΧΟΥΡΖΑΜΑΝΗ
     9: ΑΘΗΝΑ
     10: '1968'
     11: 543Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ
@@ -45493,15 +45486,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 892
     1: ΠΑΡΑΣΧΟΣ,ΚΛΕΩΝΟΣ Β.
     2: ΜΕΣΟΓΕΙΟ
-    4: 910 ΠΑΡ
+    4: 910ΠΑΡ
     5: '384'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 173Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΜΕΣΟΓΕΙΟΣ
     13: ΤΑΞΙΔΙΑ-ΜΕΣΟΓΕΙΟΣ
@@ -45545,15 +45538,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 893
     1: ΠΑΡΑΣΧΟΣ,ΚΛΕΩΝΟΣ
     2: ΕΥΡΩΠΑΙΚΗ ΠΕΖΟΓΡΑΦΙΑ ΚΑΙ ΠΟΙΗΣΗ
-    4: 800.1 ΠΑΡ
+    4: 800.1ΠΑΡ
     5: '2651'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1956'
     11: 214Σ
     12: ΕΥΡΩΠΑΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
     13: ΠΕΖΟΓΡΑΦΙΑ-ΕΥΡΩΠΗ
@@ -45647,15 +45640,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 895
     1: ΠΑΡΑΣΧΟΣ,ΚΛΕΩΝΟΣ Β.
     2: ΕΛΛΗΝΕΣ ΛΥΡΙΚΟΙ
     3: ΑΠΟ ΤΟΝ ΣΟΛΩΜΟ ΕΩΣ ΣΗΜΕΡΑ
-    4: 880.3 ΠΑΡ
+    4: 880.3ΠΑΡ
     5: '226'
     8: ΣΠΥΡΟΠΟΥΛΟΣ
     9: ΑΘΗΝΑ
     10: '1953'
     11: 260Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΤΕΧΝΙΑ-ΛΥΡΙΚΟΙ
     13: ΛΥΡΙΚΟΙ-ΕΛΛΗΝΕΣ
@@ -45697,15 +45690,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 896
     1: ΠΑΡΑΣΧΟΣ,ΚΛΕΩΝΟΣ Β.
     2: ΔΕΚΑ ΕΛΛΗΝΕΣ ΛΥΡΙΚΟΙ
-    4: 880.3 ΠΑΡ
+    4: 880.3ΠΑΡ
     5: '1008'
     7: 2ΕΚΔ
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 214Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΛΥΡΙΚΟΙ
@@ -45847,15 +45840,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 899
     1: ΠΑΤΑΤΖΗΣ,ΣΩΤΗΡΗΣ
     2: ΔΟΝ ΚΑΜΙΛΛΟ
-    4: 886.2 ΠΑΤ
+    4: 886.2ΠΑΤ
     5: '2663'
     8: ΦΙΛΙΠΠΟΤΗ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 86Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΑΤΥΡΑ
     13: ΣΑΤΥΡΑ-ΕΡΓΟ
@@ -45900,15 +45893,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 900
     1: ΠΑΤΡΙΑΡΧΕΑΣ,ΒΑΣΙΛΕΙΟΣ Δ.
     2: ΑΙ ΤΕΛΕΥΤΑΙΑΙ ΗΜΕΡΑΙ ΤΟΥ ΒΥΖΑΝΤΙΟΥ
     3: ΔΡΑΜΑ
-    4: 886.2 ΠΑΤ
+    4: 886.2ΠΑΤ
     5: '1466'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 90Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΒΥΖΑΝΤΙΟ
@@ -45953,15 +45946,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 901
     1: ΠΑΤΡΙΑΡΧΕΑΣ,ΒΑΣ.Δ.
     2: Ο ΑΡΙΣΤΟΤΕΛΗΣ ΒΑΛΑΩΡΙΤΗΣ ΠΕΡΙ ΤΗΣ ΑΓΓΛΟΚΡΑΤΙΑΣ
     3: ΕΝ ΤΑΙΣ ΙΟΝΙΟΙΣ ΝΗΣΟΙΣ
-    4: 889.25 ΠΑΤ
+    4: 889.25ΠΑΤ
     5: 1000-999
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1955'
     11: 64Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
@@ -46156,15 +46149,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 905
     1: ΠΑΤΣΙΟΥ,ΒΙΚΥ
     2: ΤΑ ΠΡΟΣΩΠΑ ΤΟΥ ΠΑΙΔΙΟΥ ΣΤΗΝ ΠΕΖΟΓΡΑΦΙΑ(1880-1930)
-    4: 880.3 ΠΑΤ
+    4: 880.3ΠΑΤ
     5: '1634'
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: '1991'
     11: 153Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -46255,15 +46248,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 907
     1: ΠΑΧΥΣ,ΓΕΩΡΓΙΟΣ
     2: ΤΟ ΕΝ ΗΠΕΙΡΩ ΑΓΡΟΤΙΚΟΝ ΖΗΤΗΜΑ
-    4: 938.93 ΠΑΧ
+    4: 938.93ΠΑΧ
     5: '2153'
     8: ΠΕΡΡΗ
     9: ΑΘΗΝΑ
     10: '1882'
     11: 85Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
@@ -46310,15 +46303,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 908
     1: ΠΑΧΥΣ,ΓΕΩΡΓΙΟΣ
     2: ΝΤΟΚΟΥΜΕΝΤΑ
-    4: 938.65 ΠΑΧ
+    4: 938.65ΠΑΧ
     5: 2078-2138-2176
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1981'
     11: 49Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΤΟΚΟΥΜΕΝΤΑ
     13: ΚΑΡΑΠΑΝΟΣ-ΔΗΜΟΚΡΑΤΙΑ
@@ -46363,15 +46356,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 909
     1: ΠΕΛΕΚΙΔΗ,ΧΡΥΣΗ Σ.
     2: ΙΔΕΟΛΟΓΙΚΑ ΡΕΥΜΑΤΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ ΤΗΣ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
     3: ΠΑΝΗΓΥΡΙΚΟΣ ΛΟΓΟΣ
-    4: 938.4 ΠΕΛ
+    4: 938.4ΠΕΛ
     5: '2555'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1974'
     11: 21Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
     13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΛΟΓΟΣ
@@ -46413,15 +46406,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 910
     1: ΠΕΛΕΚΙΔΗ,ΧΡΥΣΗ
     2: ΜΕΛΕΤΕΣ ΑΡΧΑΙΑΣ ΙΣΤΟΡΙΑΣ
-    4: 938.1 ΠΕΛ
+    4: 938.1ΠΕΛ
     5: '1914'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1979'
     11: 95Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ-ΜΕΛΕΤΕΣ
     13: ΑΡΧΑΙΟΤΗΤΑ-ΜΕΛΕΤΕΣ
@@ -46463,15 +46456,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 911
     1: ΠΕΝΛΙΔΗΣ,ΚΩΝ/ΝΟΣ
     2: Η ΔΙΔΑΣΚΑΛΙΑ ΤΟΥ ΠΕΖΟΓΡΑΦΗΜΑΤΟΣ
-    4: 880.09 ΠΕΝ
+    4: 880.09ΠΕΝ
     5: '2625'
     8: ΧΣ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1962'
     11: 74Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΔΙΔΑΣΚΑΛΙΑ
@@ -46513,15 +46506,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 912
     1: ΠΕΝΙΝΤΖΟΝ,ΧΕΛ
     2: ΔΥΟ ΚΟΣΜΟΙ
     3: ΑΜΕΡΙΚΗ ΚΑΙ ΡΩΣΙΑ
-    4: 970 ΡΕΝ
+    4: 970ΡΕΝ
     5: '439'
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 179Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ
     13: ΑΜΕΡΙΚΗ-ΙΣΤΟΡΙΑ
@@ -46812,15 +46805,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 918
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
     2: Ο ΤΣΕΛΙΓΚΑΣ
-    4: 889.30 ΠΕΡ
+    4: 889.30ΠΕΡ
     5: '1167'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 319Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑΤΙΚΗ ΒΙΟΓΡΑΦΙΑ
     13: ΚΡΥΣΤΑΛΛΗΣ-ΒΙΟΓΡΑΦΙΑ
@@ -46866,15 +46859,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 919
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧΑΗΛ
     2: Η ΣΚΛΗΡΗ ΒΡΟΧΗ
     3: ΧΡΟΝΙΚΟ ΤΟΥ ΠΟΛΕΜΟΥ
-    4: 889.30 ΠΕΡ
+    4: 889.30ΠΕΡ
     5: '1175'
     7: 2ΕΚΔ
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1961'
     11: 161Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -46916,15 +46909,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 920
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
     2: Ο ΔΑΙΜΟΝΑΣ
-    4: 889.30 ΠΕΡ
+    4: 889.30ΠΕΡ
     5: 1172-1173-1174-
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1974'
     11: 429Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΑΝΔΡΟΥΤΣΟΣ
@@ -46964,15 +46957,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 921
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
     2: ΤΟ ΧΡΩΜΑ ΤΗΣ ΘΑΛΑΣΣΑΣ
-    4: 889.30 ΠΕΡ
+    4: 889.30ΠΕΡ
     5: '1171'
     8: ΑΡΓΩ
     9: ΑΘΗΝΑ
     10: '1963'
     11: 392Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     3: null
@@ -47016,15 +47009,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 922
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
     2: ΣΟΥΛΙΩΤΕΣ
-    4: 889.30 ΠΕΡ
+    4: 889.30ΠΕΡ
     5: 1177-1176-1170
     6: 2ΕΚΔ
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1957'
     11: 475Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -47122,15 +47115,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 924
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
     2: ΑΝΘΟΛΟΓΙΑ ΤΗΣ ΠΟΙΗΣΕΩΣ
     3: ΑΠΟ ΤΗΝ ΑΛΩΣΗ ΩΣ ΣΗΜΕΡΑ
-    4: 880.08 ΠΕΡ
+    4: 880.08ΠΕΡ
     5: 628-629-630-
     8: ΠΕΡΑΝΘΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 781Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΑΝΘΟΛΟΓΙΑ
@@ -47158,14 +47151,15 @@
   - ΠΕΡΑΝΘΗΣ,ΜΙΧ
   title: ΑΜΒΡΑΚΙΑ
   subtitle: ΧΡΟΝΟΓΡΑΦΙΑ ΜΙΑΣ ΠΡΩΤΕΥΟΥΣΑΣ
   dewey: 938.21 ΠΕΡ
   entry_numbers:
   - '2187'
   - '2273'
+  - '13268'
   editor: None // ΑΘΗΝΑ
   edition_year: 1954
   pages: 212
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΑΜΒΡΑΚΙΑ
   - ΧΡΟΝΟΓΡΑΦΙΑ
@@ -47173,16 +47167,16 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 925
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
     2: ΑΜΒΡΑΚΙΑ
     3: ΧΡΟΝΟΓΡΑΦΙΑ ΜΙΑΣ ΠΡΩΤΕΥΟΥΣΑΣ
-    4: 938.21 ΠΕΡ
-    5: 2187-2273
+    4: 938.21ΠΕΡ
+    5: 2187-2273-13268
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1954'
     11: 212Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΜΒΡΑΚΙΑ
     13: ΑΜΒΡΑΚΙΑ-ΧΡΟΝΟΓΡΑΦΙΑ
     14: ΧΡΟΝΟΓΡΑΦΙΑ
@@ -47275,15 +47269,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 927
     1: ΠΕΡΙΣΤΕΡΗΣ,ΣΠΥΡΟΣ Δ.
     2: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ ΗΠΕΙΡΟΥ ΚΑΙ ΜΩΡΗΑ
-    4: 782.42 ΠΕΡ
+    4: 782.42ΠΕΡ
     5: '2622'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1950'
     11: 135Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΜΩΡΗΑΣ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
@@ -47328,15 +47322,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 928
     1: ΠΕΡΕΣΙΑΔΟΣ,ΣΠΥΡΙΔΩΝΟΣ
     2: Η ΣΚΛΑΒΑ
     3: ΔΡΑΜΑ
-    4: 886.2 ΠΕΡ
+    4: 886.2ΠΕΡ
     5: '2674'
     8: ΣΑΛΙΒΕΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 68Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -47428,15 +47422,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 930
     1: ΠΕΤΙΜΕΖΑΣ,ΝΙΚΟΛΑΟΣ Η.
     2: ΗΜΕΡΟΛΟΓΙΟΝ ΕΚΣΤΡΑΤΕΙΑΣ 1912-13
-    4: 938.68 ΠΕΤ
+    4: 938.68ΠΕΤ
     5: '2079'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1981'
     11: 287Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΜΕΡΟΛΟΓΙΟ
     13: ΗΜΕΡΟΛΟΓΙΟ-1912
@@ -47477,15 +47471,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 931
     1: ΠΕΤΡΑΚΑΚΟΣ,ΔΗΜΗΤΡΙΟΣ Α.
     2: ΚΟΙΝΟΒΟΥΛΕΥΤΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΑΔΟΣ
-    4: 938.62 ΠΕΤ
+    4: 938.62ΠΕΤ
     5: 2143-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1946'
     11: 565Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΟΙΝΟΒΟΥΛΙΟ
     13: ΚΟΙΝΟΒΟΥΛΙΟ-ΙΣΤΟΡΙΑ
@@ -47625,15 +47619,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 934
     1: ΧΑΡΗ, ΠΕΤΡΟΥ
     2: ΔΑΛΜΑΤΙΚΕΣ ΑΚΤΕΣ ΚΑΙ ΟΙ ΠΟΛΙΤΕΙΕΣ ΚΑΙ ΘΑΛΑΣΣΕΣ
-    4: 919 ΧΑΡ
+    4: 919ΧΑΡ
     5: '421'
     7: 2ΕΚΔ
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1961'
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΔΑΛΜΑΤΙΚΕΣ ΑΚΤΕΣ
     13: ΤΑΞΙΔΙΑ-ΔΑΛΜΑΤΙΚΕΣ ΑΚΤΕΣ
@@ -47828,15 +47822,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 938
     1: ΠΕΤΣΑΛΗΣ-ΔΙΟΜΗΔΗΣ,Θ.
     2: Ο ΜΕΓΑΣ ΕΣΠΕΡΙΝΟΣ
     3: ΔΡΑΜΑ
-    4: 886.2 ΠΕΤ
+    4: 886.2ΠΕΤ
     5: '1520'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1960'
     11: 93Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -47878,15 +47872,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 939
     1: ΠΕΤΣΚΟΥ,ΧΑΡ.Δ.
     2: Η ΠΗΝΕΛΟΠΗ ΣΕ ΗΠΕΙΡΩΤΙΚΟ ΧΩΡΙΟ
-    4: 886.2 ΠΕΤ
+    4: 886.2ΠΕΤ
     5: '1465'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 151Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -47928,15 +47922,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 940
     1: ΠΙΕΡΙΔΗΣ,Γ
     2: ΕΝΑ ΤΑΞΙΔΙ ΤΟΥ Π.ΜΕΛΕΤΙΟΥ ΣΤΗ Β.ΑΦΡΙΚΗ
-    4: 916 ΠΙΕ
+    4: 916ΠΙΕ
     5: '415'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1955'
     11: 29Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-Β.ΑΦΡΙΚΗ
     13: ΑΦΡΙΚΗ-ΤΑΞΙΔΙΑ
@@ -47981,15 +47975,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 941
     1: ΠΙΜΠΛΗΣ,ΣΠΥΡΟΣ
     2: ΔΡΑΜΑΤΟΥΡΓΙΑ
     3: Η ΘΕΑΤΡΙΚΗ ΔΡΑΣΗ
-    4: 886.2 ΠΙΜ
+    4: 886.2ΠΙΜ
     5: '2689'
     8: ΑΘΗΝΑ
     9: Χ.Ε
     10: '1980'
     11: 137Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -48032,15 +48026,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 942
     1: ΠΙΝΤΕΡ,ΧΑΡΟΛΝΤ
     2: ΠΑΛΙΟΙ ΚΑΙΡΟΙ
-    4: 822 ΠΙΝ
+    4: 822ΠΙΝ
     5: '1405'
     6: ΤΟΛΙΚΑ,ΟΛΥΜΠΙΑ
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 28Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -48084,15 +48078,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 943
     1: ΠΙΝΤΕΡ,ΧΑΡΟΛΝΤ
     2: ΤΟ ΘΕΡΜΟΚΗΠΙΟ
-    4: 822 ΠΙΝ
+    4: 822ΠΙΝ
     5: '1406'
     6: ΤΟΛΙΚΑ,ΟΛΥΜΠΙΑ
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 79Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -48237,15 +48231,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 946
     1: ΠΙΡΑΝΤΕΛΛΟ,ΛΟΥΙΤΖΙ
     2: ΕΤΣΙ ΕΙΝΑΙ (ΑΝ ΕΤΣΙ ΝΟΜΙΖΕΤΕ)
-    4: 852 ΠΙΡ
+    4: 852ΠΙΡ
     5: '1557'
     6: ΠΛΩΡΙΤΗΣ,ΜΑΡΙΟΣ
     8: ΓΝΩΣΗ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 87Σ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -48290,15 +48284,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 947
     1: ΠΙΡΑΝΤΕΛΛΟ,ΛΟΥΙΤΖΙ
     2: ΑΠΟΨΕ ΑΥΤΟΣΧΕΔΙΑΖΟΥΜΕ
-    4: 852 ΠΙΡ
+    4: 852ΠΙΡ
     5: '1559'
     6: ΜΥΡΑΤ,ΔΗΜΗΤΡΙΟΣ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 105Σ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -48342,15 +48336,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 948
     1: ΠΙΡΑΝΤΕΛΛΟ,ΛΟΥΙΤΖΙ
     2: ΘΕΑΤΡΙΚΑ ΕΡΓΑ
-    4: 852 ΠΙΡ
+    4: 852ΠΙΡ
     5: '1578'
     8: ΓΚΟΝΗ
     9: ΑΘΗΝΑ
     10: '1966'
     11: 262Σ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΙΤΑΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
@@ -48396,15 +48390,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 949
     1: ΠΙΡΑΝΤΕΛΛΟ,ΛΟΥΙΤΖΙ
     2: ΝΑ ΝΤΥΣΟΥΜΕ ΤΟΥΣ ΓΥΜΝΟΥΣ
-    4: 852 ΠΙΡ
+    4: 852ΠΙΡ
     5: '1556'
     6: ΠΛΩΡΙΤΗΣ,ΜΑΡΙΟΣ
     8: ΓΝΩΣΗ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 89Σ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -48450,15 +48444,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 950
     1: ΠΛΑΤΕΡΟ,ΝΤΑΝΙΕΛ
     2: ΟΛΥΜΠΙΑΔΑ
     3: Η ΜΗΤΕΡΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
-    4: 938.17 ΔΗΜ
+    4: 938.17ΔΗΜ
     5: '1710'
     6: ΣΚΑΡΑ,ΜΙΡΚΑ
     8: ΝΕΑ ΣΥΝΟΡΑ
     9: ΑΘΗΝΑ
     10: '1991'
     11: 400Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
@@ -48547,15 +48541,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 952
     1: ΠΛΙΑΤΣΙΚΑΣ,ΒΑΣΙΛΕΙΟΣ Α.
     2: ΗΠΕΙΡΩΤΙΚΕΣ ΑΝΑΔΡΟΜΕΣ
-    4: 938.7 ΠΛΙ
+    4: 938.7ΠΛΙ
     5: '2068'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 213Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΑΝΑΔΡΟΜΕΣ
@@ -48597,15 +48591,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 953
     1: ΠΛΙΑΤΣΙΚΑΣ,ΒΑΣΙΛΕΙΟΣ Α
     2: ΠΛΑΝΕΜΜΑΤΑ ΣΤΑ ΞΕΝΑ
-    4: 938.99 ΠΛΙ
+    4: 938.99ΠΛΙ
     5: '368'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1969'
     11: 254Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΔΙΑΣΠΟΡΑΣ
     13: ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΔΙΑΣΠΟΡΑΣ
@@ -48804,15 +48798,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 957
     1: ΠΟΛΙΤΑΡΧΗΣ,Γ.Μ.
     2: ΠΡΟΣΩΠΑ ΚΑΙ ΙΔΕΕΣ
-    4: 880.4 ΠΟΛ
+    4: 880.4ΠΟΛ
     5: '1002'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1963'
     11: 133Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΔΟΚΙΜΙΑ
@@ -48852,15 +48846,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 958
     1: ΠΟΛΙΤΑΡΧΗΣ,Γ.Μ.
     2: ΚΡΙΤΙΚΑ ΔΟΚΙΜΙΑ
-    4: 880.4 ΠΟΛ
+    4: 880.4ΠΟΛ
     5: '1012'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 260Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΡΙΤΙΚΑ ΔΟΚΙΜΙΑ
     13: ΚΡΙΤΙΚΑ ΔΟΚΙΜΙΑ
@@ -48902,15 +48896,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 959
     1: ΠΟΛΙΤΗΣ,ΛΙΝΟΣ
     2: Ο ΣΟΛΩΜΟΣ ΣΤΑ ΓΡΑΜΜΑΤΑ ΤΟΥ
-    4: 889.15 ΠΟΛ
+    4: 889.15ΠΟΛ
     5: '1208'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 78Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
@@ -48953,15 +48947,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 960
     1: ΠΟΛΙΤΗΣ,ΛΙΝΟΣ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΟΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-    4: 880.09 ΠΟΛ
+    4: 880.09ΠΟΛ
     5: 1286-2564-2787
     7: 4ΕΚΔ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1985'
     11: 446Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -49003,15 +48997,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 961
     1: ΠΟΛΙΤΗΣ,ΛΙΝΟΣ
     2: ΣΥΝΟΠΤΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΑΣ ΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-    4: 880.9 ΠΟΛ
+    4: 880.9ΠΟΛ
     5: '184'
     7: 3ΕΚΔ
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1977'
     11: 167Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -49103,15 +49097,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 963
     1: ΠΟΛΙΤΗΣ,Ν.Γ.
     2: ΕΚΛΟΓΑΙ ΑΠΟ ΤΑ ΤΡΑΓΟΥΔΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΛΑΟΥ
-    4: 880.14 ΠΟΛ
+    4: 880.14ΠΟΛ
     5: '2636'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 309Σ
     12: ΕΛΛΗΝΙΚ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
@@ -49135,15 +49129,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 964
   authors:
   - ΠΟΛΙΤΗΣ,ΝΙΚΟΛΑΟΣ Γ
   title: ΠΑΡΟΙΜΙΑΙ
-  dewey: 398 ΠΟΛΙ
+  dewey: 398 ΠΟΛ
   entry_numbers:
   - '233'
   - '234'
   editor: None // ΑΘΗΝΑ
   pages: 503
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -49151,15 +49145,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 964
     1: ΠΟΛΙΤΗΣ,ΝΙΚΟΛΑΟΣ Γ
     2: ΠΑΡΟΙΜΙΑΙ
-    4: 398 ΠΟΛΙ
+    4: 398ΠΟΛ
     5: 233-234-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 503Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΑΡΟΙΜΙΕΣ
     13: ΠΑΡΟΙΜΙΕΣ
@@ -49251,15 +49245,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 966
     1: ΠΟΛΙΤΗΣ,ΦΩΤΗΣ
     2: ΘΕΑΤΡΙΚΕΣ ΕΠΙΦΥΛΛΙΔΕΣ
-    4: 880.09 ΠΟΛ
+    4: 880.09ΠΟΛ
     5: '1408'
     8: ΓΑΛΑΞΙΑ
     9: ΑΘΗΝΑ
     10: '1964'
     11: 306Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
@@ -49302,15 +49296,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 967
     1: ΠΟΛΙΤΗΣ,Ν.Γ.
     2: ΚΛΕΦΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
-    4: 782.42 ΠΟΛ
+    4: 782.42ΠΟΛ
     5: '2630'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 110Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -49450,15 +49444,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 970
     1: ΠΟΛΥΧΡΟΝΟΠΟΥΛΟΣ,ΠΑΝΟΣ
     2: ΤΑΞΙΔΙΑ ΣΤΙΣ ΧΩΡΕΣ ΤΟΥ ΗΛΙΟΥ ΚΑΙ ΤΗΣ ΟΜΙΧΛΗΣ
-    4: 914.46 ΠΟΛ
+    4: 914.46ΠΟΛ
     5: '399'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1965'
     11: 158Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΙΣΠΑΝΙΑ
     13: ΤΑΞΙΔΙΑ-ΙΣΠΑΝΙΑ
@@ -49503,15 +49497,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 971
     1: ΠΟΛΥΧΡΟΝΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ ΕΥΣΤ.
     2: ΟΙ ΒΑΣΙΛΕΙΣ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΙ Η ΒΥΖΑΝΤΙΝΗ ΤΩΝ ΚΑΤΑΓΩΓΗ
-    4: 938.6 ΠΟΛ
+    4: 938.6ΠΟΛ
     5: 2002-2003-2004
     8: ΔΗΜΟΠΟΥΛΟΥ
     9: ΑΘΗΝΑ
     10: '1961'
     11: 174Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΑΣΙΛΕΙΑΔΕΣ
     13: ΒΑΣΙΛΕΙΑΣ-ΕΛΛΗΝΕΣ
@@ -49606,15 +49600,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 973
     1: ΠΟΥΛΟΥ,ΙΩΑΝΝΗΣ ΧΡ.
     2: ΤΟ ΕΠΕΙΣΟΔΙΟΝ ΜΟΥΣΟΥΡΟΥ
     3: Η ΕΛΛΗΝΟΤΟΥΡΚΙΚΗ ΔΙΕΝΕΞΙΣ ΤΟΥ 1847
-    4: 938.63 ΠΟΥ
+    4: 938.63ΠΟΥ
     6: '1836'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1958'
     11: 116Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΟΤΟΥΡΚΙΚΗ-ΔΙΕΝΕΞΗ
     13: ΕΛΛΗΝΟΤΟΥΡΚΙΚΗ ΔΙΕΝΕΞΗ
@@ -49783,18 +49777,17 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 977
-  authors:
-  - ΠΡΕΒΕΛΑΚΗΣ,ΕΛΕΥΘΕΡΙΟΣ
-  title: ΕΠΙΤΟΜΑΙ ΕΓΓΡΑΦΩΝ ΤΟΥ ΒΡΕΤΑΝΝΙΚΟΥ ΥΠΟΥΡΓΕΙΟΥ ΤΩΝ ΕΞΩΤΕΡΙΚΩΝ
-  dewey: 938.501 ΠΡΕ
+  authors: []
+  title: ΜΝΗΜΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑΣ
+  dewey: 938.501 ΧΣ
   entry_numbers:
   - '1805'
   - '1857'
   - '1806'
   editor: None // ΑΘΗΝΑ
   edition_year: 1975
   pages: 270
@@ -49804,17 +49797,17 @@
   - ΕΞΩΤΕΡΙΚΟΥ
   - ΒΡΕΤΑΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 977
-    1: ΠΡΕΒΕΛΑΚΗΣ,ΕΛΕΥΘΕΡΙΟΣ
-    2: ΕΠΙΤΟΜΑΙ ΕΓΓΡΑΦΩΝ ΤΟΥ ΒΡΕΤΑΝΝΙΚΟΥ ΥΠΟΥΡΓΕΙΟΥ ΤΩΝ ΕΞΩΤΕΡΙΚΩΝ
-    4: 938.501ΠΡΕ
+    1: Χ.Σ
+    2: ΜΝΗΜΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑΣ
+    4: 938.501Χ.Σ
     5: 1805-1857-1806-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 270Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΓΓΡΑΦΑ
     13: ΕΓΓΡΑΦΑ-ΕΞΩΤΕΡΙΚΟΥ
@@ -49910,15 +49903,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 979
     1: ΠΡΕΒΕΛΑΚΗΣ,Π
     2: ΤΟ ΗΦΑΙΣΤΕΙΟ
     3: ΔΡΑΜΑ
-    4: 886.2 ΠΡΕ
+    4: 886.2ΠΡΕ
     5: '1508'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1962'
     11: 133Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -50066,15 +50059,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 982
     1: ΠΡΟΔΡΟΜΟΥ,ΘΕΟΔΩΡΟΣ
     2: ΚΑΤΟΜΥΟΜΑΧΙΑ(ΠΟΝΤΙΚΟΓΑΤΟΠΟΛΕΜΟΣ)
-    4: 886.2 ΠΡΟ
+    4: 886.2ΠΡΟ
     5: 1510-1511
     6: ΜΑΡΚΑΚΗΣ,ΠΕΤΡΟΣ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1955'
     11: 18Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -50117,15 +50110,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 983
     1: ΠΡΩΤΟΠΑΠΑ-ΜΠΟΥΜΠΟΥΛΙΔΟΥ,ΓΛΥΚΕΡΙΑ
     2: ΤΟ ΘΕΑΤΡΟΝ ΕΝ ΖΑΚΥΝΘΟ ΑΠΟ ΤΟΥ ΙΖ' ΤΟΥ ΙΘ' ΑΙΩΝΟΣ
-    4: 886.2 ΠΡΩ
+    4: 886.2ΠΡΩ
     5: 1425-1426
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1958'
     11: 101Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ0ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΖΑΚΥΝΘΟΣ
@@ -50247,15 +50240,16 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 986
   authors:
   - ΠΡΩΤΟΨΑΛΤΗΣ,ΕΜΜΑΝ Γ.
-  title: ΙΓΝΑΤΙΟΣ ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ (1766-1828)
+  title: ΜΝΗΜΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑΣ ΤΕΥΧΟΣ 1-2
+  subtitle: ΙΓΝΑΤΙΟΣ ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ (1766-1828)
   dewey: 938.488 ΠΡΩ
   entry_numbers:
   - '1707'
   - '1714'
   editor: None // ΑΘΗΝΑ
   edition_year: 1959
   pages: 295
@@ -50266,26 +50260,26 @@
   - ΟΥΓΓΡΟΒΛΑΧΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 986
     1: ΠΡΩΤΟΨΑΛΤΗΣ,ΕΜΜΑΝ Γ.
-    2: ΙΓΝΑΤΙΟΣ ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ (1766-1828)
+    2: ΜΝΗΜΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑΣ ΤΕΥΧΟΣ 1-2
+    3: ΙΓΝΑΤΙΟΣ ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ (1766-1828)
     4: 938.488ΠΡΩ
     5: 1707-1714-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1959'
     11: 295Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ
     13: ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ
     14: ΙΓΝΑΤΙΟΣ-ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ
-    15: ΟΥΓΓΡΟΒΛΑΧΙΑ-ΙΓΑΝΑΤΙΟΣ
-    3: null
+    15: ΟΥΓΓΡΟΒΛΑΧΙΑ-ΙΓΝΑΤΙΟΣ
     6: null
     7: null
     16: null
     17: null
     18: null
     19: null
     20: null
@@ -50367,15 +50361,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 988
     1: ΠΡΩΤΟΨΑΛΤΗΣ,ΕΜΜΑΝΟΥΗΛ
     2: ΔΙΔΑΓΜΑΤΑ ΑΠΟ ΤΗΝ ΕΠΑΝΑΣΤΑΣΙΝ ΤΟΥ 1821
-    4: 938.5 ΠΡΩ
+    4: 938.5ΠΡΩ
     5: '2702'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 23Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ 1821
     13: ΕΠΑΝΑΣΤΑΣΗ 1821-ΔΙΔΑΓΜΑΤΑ
@@ -50470,15 +50464,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 990
     1: ΠΡΩΤΟΨΑΛΤΗΣ,ΕΜΜΑΝΟΥΗΛ Γ.
     2: ΤΟ ΕΙΚΟΣΙΕΝΑ ΚΑΙ Η ΗΠΕΙΡΟΣ
-    4: 938.5 ΠΡΩ
+    4: 938.5ΠΡΩ
     5: 2722-2723
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 50Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-1821
     13: ΗΠΕΙΡΟΣ-1821
@@ -51419,15 +51413,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1009
     1: ΡΟΖΑΚΗΣ,ΣΤΕΦΑΝΟΣ
     2: ΔΟΚΙΜΙΑ ΚΡΙΤΙΚΗΣ
     3: Ο ΜΥΘΟΣ ΚΑΙ ΤΟ ΠΕΡΙΒΛΗΜΑ
-    4: 880.4 ΡΟΖ
+    4: 880.4ΡΟΖ
     5: '2654'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 153Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΟΚΙΜΙΑ
     13: ΔΟΚΙΜΙΑ-ΚΡΙΤΙΚΗ
@@ -51467,15 +51461,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1010
     1: ΡΟΖΑΚΗΣ,ΠΑΝΤΕΛΗΣ Μ.
     2: ΔΙΠΛΩΜΑΤΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΕΥΡΩΠΗΣ (1920-1970)
-    4: 940 ΡΟΖ
+    4: 940ΡΟΖ
     5: '2310'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 554Σ
     12: ΕΥΡΩΠΑΙΚΗ ΙΣΤΟΡΙΑ-ΔΙΠΛΩΜΑΤΙΚΗ
     13: ΔΙΠΛΩΜΑΤΙΚΗ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
@@ -51625,15 +51619,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1013
     1: ΡΟΥΦΟΥ,ΡΟΔΗΣ
     2: Η ΜΕΡΑ ΤΗΣ ΚΡΙΣΗΣ
     3: ΣΚΗΝΙΚΟΣ ΜΥΘΟΣ
-    4: 886.2 ΡΟΥ
+    4: 886.2ΡΟΥ
     5: '1507'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1957'
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
     14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΜΥΘΟΣ
@@ -51674,15 +51668,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1014
     1: ΡΩΜΑΝΟΣ,ΙΩΑΝΝΗΣ
     2: ΙΣΤΟΡΙΚΑ ΕΡΓΑ
-    4: 938 ΡΩΜ
+    4: 938ΡΩΜ
     5: '2155'
     8: Χ.Ε
     9: ΚΕΡΚΥΡΑ
     10: '1959'
     11: 405Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΡΓΑ
     13: ΙΣΤΟΡΙΚΑ ΕΡΓΑ
@@ -51773,15 +51767,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1016
     1: ΣΑΘΑΣ,ΚΩΝ
     2: ΤΟΥΡΚΟΚΡΑΤΟΥΜΕΝΗ ΕΛΛΑΣ(1453-1821)
-    4: 938.4 ΣΑΘ
+    4: 938.4ΣΑΘ
     5: '1851'
     8: ΚΑΜΑΡΙΝΟΠΟΥΛΟΥ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 666Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
     13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΕΛΛΑΣ
@@ -51809,14 +51803,15 @@
   authors:
   - ΣΑΘΑΣ,ΚΩΝ/ΝΟΣ Ν.
   title: ΙΣΤΟΡΙΚΟΝ ΔΟΚΙΜΙΟΝΠΕΡΙ ΤΩΝ ΠΡΟΣ ΑΠΟΤΙΝΑΞΙΝ ΤΟΥ ΟΘΩΜΑΝΙΚΟΥ
   subtitle: ΖΥΓΟΥ ΕΠΑΝΑΣΤΑΣΕΩΝ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ(1453-1821)
   dewey: 938.401 ΣΑΘ
   entry_numbers:
   - '1712'
+  - '21719'
   editor: None // ΑΘΗΝΑ
   edition_year: 1869
   pages: 666
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΤΟΥΡΚΟΚΡΑΤΙΑ
   - ΔΟΚΙΜΙΟ
@@ -51828,15 +51823,15 @@
   offprint: false
   original_entry:
     0: 1017
     1: ΣΑΘΑΣ,ΚΩΝ/ΝΟΣ Ν.
     2: ΙΣΤΟΡΙΚΟΝ ΔΟΚΙΜΙΟΝΠΕΡΙ ΤΩΝ ΠΡΟΣ ΑΠΟΤΙΝΑΞΙΝ ΤΟΥ ΟΘΩΜΑΝΙΚΟΥ
     3: ΖΥΓΟΥ ΕΠΑΝΑΣΤΑΣΕΩΝ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ(1453-1821)
     4: 938.401ΣΑΘ
-    5: '1712'
+    5: 1712-21719
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1869'
     11: 666Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
     13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΔΟΚΙΜΙΟ
     14: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ
@@ -51931,15 +51926,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1019
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΒΑΣΙΛΙΑΣ ΛΗΡ
     3: ΤΡΑΓΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: 1329-1382
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 140Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -51984,15 +51979,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1020
     1: ΣΑΙΞΠΗΡ,ΟΥΛΛΙΑΜ
     2: ΔΩΔΕΚΑΤΗ ΝΥΧΤΑ Η ΟΤΙ ΘΕΛΕΤΕ
     3: ΚΩΜΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1330'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 108Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52038,15 +52033,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1021
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΙΟΥΛΙΟΣ ΚΑΙΣΑΡΑΣ
     3: ΤΡΑΓΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1327'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 109Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52092,15 +52087,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1022
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΛΙΑΣ ΡΙΧΑΡΔΟΣ Ο Γ'
     3: ΤΡΑΓΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1383'
     6: ΚΑΡΘΑΙΟΣ,Κ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 190Σ
     12: ΑΓΓΚΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52146,15 +52141,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1023
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΙΟΥΛΙΟΣ ΚΑΙΣΑΡΑΣ
     3: ΤΡΑΓΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1381'
     6: ΚΑΡΘΑΙΟΣ,Κ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 147Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52200,15 +52195,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1024
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΧΕΙΜΩΝΙΑΤΙΚΟ ΠΑΡΑΜΥΘΙ
     3: ΚΩΜΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1384'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 125Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52252,15 +52247,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1025
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο Δ'
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1389'
     6: ΠΑΛΛΗΣ,Α
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 109Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52307,15 +52302,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1026
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΑΛΜΕΤ
     3: ΤΡΑΓΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1390'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 151Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52361,15 +52356,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1027
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Η ΤΡΙΚΥΜΙΑ
     3: ΚΩΜΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1387'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 101Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52413,15 +52408,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1028
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΛΙΑΣ ΡΙΧΑΡΔΟΣ Ο Β'
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1331'
     6: ΚΑΡΘΑΙΟΣ,Κ
     8: ΒΑΣΙΛΕΙΟΥ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 156Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52466,15 +52461,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1029
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΕΜΠΟΡΟΣ ΤΗΣ ΒΕΝΕΤΙΑΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1388'
     6: ΠΑΛΛΗΣ,ΑΛΕΞ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 98Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52521,15 +52516,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1030
     1: ΣΑΙΞΠΗΡ.ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΑΣ ΕΡΡΙΚΟΣ Ο ΣΤ'
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: 2475-2474-
     6: ΡΩΤΑΣ.ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 142Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52575,15 +52570,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1031
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΠΟΛΥ ΚΑΚΟ ΓΙΑ ΤΙΠΟΤΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1350'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 132Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52630,15 +52625,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1032
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΜΑΚΜΠΕΘ
     3: ΤΡΑΓΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1385'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 102Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52683,15 +52678,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1033
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΔΩΔΕΚΑΤΗ ΝΥΧΤΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1335'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 134Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52737,15 +52732,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1034
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΜΕ ΤΟ ΙΔΙΟ ΜΕΤΡΟ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1348'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 135Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52791,15 +52786,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1035
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΤΟ ΧΕΙΜΩΝΙΑΤΙΚΟ ΠΑΡΑΜΥΘΙ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1340'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 154Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52845,15 +52840,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1036
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Η ΚΩΜΩΔΙΑ ΜΕ ΠΛΑΝΕΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1346'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 94Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52899,15 +52894,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1037
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΟΝΕΙΡΟ ΚΑΛΟΚΑΙΡΙΝΗΣ ΝΥΧΤΑΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1353'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 115Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -52953,15 +52948,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1038
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΟΙ ΕΥΘΥΜΕΣ ΚΥΡΑΔΕΣ ΤΟΥ ΟΥΙΝΖΟΡ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1333'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 141Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53007,15 +53002,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1039
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΤΡΩΙΛΟΣ ΚΑΙ ΧΡΥΣΙΔΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1357'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 175Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53060,15 +53055,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1040
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΟΝΕΙΡΟ ΚΑΛΟΚΑΙΡΙΝΗΣ ΝΥΧΤΑΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1386'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 96Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53114,15 +53109,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1041
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο ΣΤ'
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: 1324-1325-1326-
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -53168,15 +53163,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1042
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΡΩΜΑΙΟΣ ΚΑΙ ΙΟΥΛΙΕΤΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1356'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1991'
     11: 153Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53223,15 +53218,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1043
     1: ΣΑΙΞΠΗΡ,ΟΥΛΛΙΑΜ
     2: Ο ΕΜΠΟΡΟΣ ΤΗΣ ΒΕΝΕΤΙΑΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: 1352-2470-2471
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -53279,15 +53274,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1044
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΤΙΤΟΣ ΑΝΔΡΟΝΙΚΟΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: 1358-2472-2473
     6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 132Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53334,15 +53329,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1045
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΚΟΡΙΟΛΑΝΟΣ
     3: ΤΡΑΓΩΔΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1328'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 141Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53387,15 +53382,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1046
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Η ΤΡΙΚΥΜΙΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1354'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 121Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53441,15 +53436,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1047
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΑΝΤΩΝΙΟΣ ΚΑΙ ΚΛΕΟΠΑΤΡΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1345'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 175Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53495,15 +53490,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1048
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΑΜΛΕΤ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1343'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 194Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53550,15 +53545,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1049
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο Δ'
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: 1341-1338-
     6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1988'
     11: 147Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53604,15 +53599,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1050
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΒΑΣΙΛΙΑΣ ΙΩΑΝΝΗΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1349'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 126Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53658,15 +53653,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1051
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΤΙΜΩΝ Ο ΑΘΗΝΑΙΟΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1355'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 121Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53712,15 +53707,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1052
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο Ε'
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1347'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 164Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53766,15 +53761,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1053
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΤΟ ΗΜΕΡΩΜΑ ΤΗΣ ΣΤΡΙΓΓΛΑΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1351'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 132Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53820,15 +53815,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1054
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΤΕΛΟΣ ΚΑΛΟ ΟΛΑ ΚΑΛΑ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1336'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 143Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53874,15 +53869,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1055
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΠΕΡΙΚΛΗΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1339'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1988'
     11: 123Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53928,15 +53923,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1056
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΑΓΑΠΗΣ ΑΓΩΝΑΣ ΑΓΟΝΟΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1359'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1988'
     11: 135Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -53982,15 +53977,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1057
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΛΙΑΣ ΡΙΧΑΡΔΟΣ Ο Γ'
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1337'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1987'
     11: 176Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -54035,15 +54030,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1058
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο Η'
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1344'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -54090,15 +54085,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1059
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΚΟΡΙΟΛΑΝΟΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: 2468-2469
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 172Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -54144,15 +54139,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1060
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΚΥΜΒΕΛΙΝΟΣ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1334'
     6: ΡΩΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1988'
     11: 171Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -54197,15 +54192,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1061
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΜΑΚΒΕΘ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1332'
     6: ΚΑΡΘΑΙΟΣ,Κ
     8: ΒΑΣΙΛΕΙΟΥ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 103Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -54251,15 +54246,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1062
     1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
     2: ΟΠΩΣ ΑΓΑΠΑΤΕ
-    4: 822.33 ΣΑΙ
+    4: 822.33ΣΑΙ
     5: '1342'
     6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
     8: ΕΠΙΚΑΙΡΟΤΗΤΑ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 136Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -54353,15 +54348,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1064
     1: ΣΑΚΕΛΛΑΡΙΟΥ,ΧΑΡΗΣ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΠΑΙΔΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ ΕΛΛΗΝΙΚΗ ΚΑΙ ΠΑΓΚΟΣΜΙΑ
     3: ΑΠΟ ΤΗΝ ΑΡΧΑΙΟΤΗΤΑ ΩΣ ΤΙΣ ΜΕΡΕΣ ΜΑΣ
-    4: 880.09 ΣΑΚ
+    4: 880.09ΣΑΚ
     5: '1283'
     8: ΦΙΛΙΠΠΟΤΗ
     9: ΑΘΗΝΑ
     10: '1984'
     11: 571Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΑΙΔΙΚΗ-ΙΣΤΟΡΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -54453,15 +54448,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1066
     1: ΣΑΚΕΛΛΑΡΙΟΥ,ΧΑΡΗΣ
     2: ΠΑΘΟΛΟΓΙΑ ΤΗΣ ΠΝΕΥΜΑΤΙΚΗΣ ΖΩΗΣ
-    4: 880.4 ΣΑΚ
+    4: 880.4ΣΑΚ
     5: '1013'
     8: ΦΙΛΙΠΠΟΤΗ
     9: ΑΘΗΝΑ
     10: '1983'
     11: 131Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΟΚΙΜΙΑ
     13: ΔΟΚΙΜΙΑ-ΛΟΓΟΤΕΧΝΙΑ
@@ -54501,15 +54496,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1067
     1: ΣΑΚΕΛΛΑΡΙΔΗΣ,ΝΙΚΗΤΑΣ Ο.Δ.
     2: ΤΑΞΙΔΙ-ΠΡΟΣΚΥΝΗΜΑ
-    4: 914.95 ΣΑΚ
+    4: 914.95ΣΑΚ
     5: '413'
     8: Χ.Ε
     9: Χ.Τ
     10: '1976'
     11: 20Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΠΡΟΣΚΥΝΗΜΑ
     13: ΤΑΞΙΔΙΑ-ΠΡΟΣΚΥΝΗΜΑ
@@ -54599,15 +54594,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1069
     1: ΣΑΚΚΑΣ,ΓΡΗΓΟΡΙΟΣ ΣΠ.
     2: ΗΠΕΙΡΩΤΙΚΑ ΔΙΗΓΗΜΑΤΑ-ΧΡΟΝΟΓΡΑΦΗΜΑΤΑ
-    4: 889.21 ΣΑΚ
+    4: 889.21ΣΑΚ
     5: '2546'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1949'
     11: 100Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΧΡΟΝΟΓΡΑΦΗΜΑΤΑ
@@ -55149,15 +55144,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1080
     1: ΣΑΡΔΕΛΗΣ,ΚΩΣΤΑΣ
     2: ΓΕΩΡΓΙΟΣ ΒΑΡΝΑΚΩΤΗΣ
     3: Ο ΠΡΟΔΟΜΕΝΟΣ ΣΤΡΑΤΗΓΟΣ ΤΟΤ 1821
-    4: 938.5 ΣΑΡ
+    4: 938.5ΣΑΡ
     5: '1954'
     8: ΕΡΕΥΝΑ
     9: ΑΘΗΝΑ
     10: '1980'
     11: 470Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821
     13: 1821-ΣΤΡΑΤΗΓΟΣ
@@ -55248,15 +55243,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1082
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΤΟ ΓΑΙΤΑΝΑΚΙ
-    4: 880.2 ΣΑΡ
+    4: 880.2ΣΑΡ
     5: '1607'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 72Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -55349,15 +55344,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1084
     1: ΣΑΧΙΝΗΣ,ΑΠΟΣΤΟΛΟΣ
     2: ΤΟ ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
-    4: 880.3 ΣΑΧ
+    4: 880.3ΣΑΧ
     5: '221'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1957'
     11: 172Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
@@ -55400,15 +55395,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1085
     1: ΣΑΧΙΝΗΣ,ΑΠΟΣΤΟΛΟΣ
     2: ΤΟ ΝΕΟΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     3: ΙΣΤΟΡΙΑ ΚΑΙ ΚΡΙΤΙΚΗ
-    4: 880.3 ΣΑΧ
+    4: 880.3ΣΑΧ
     5: '220'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1958'
     11: 316Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
@@ -55499,15 +55494,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1087
     1: ΣΒΟΛΟΠΟΥΛΟΣ,Δ.Κ
     2: ΠΑΝΑΓΗΣ ΤΣΑΛΔΑΡΗΣ
     3: Ο ΚΗΡΥΞ ΤΗΣ ΝΟΜΙΜΟΤΗΤΑΣ ΚΑΙ ΕΙΡΗΝΕΥΤΗΣ ΤΟΥ ΛΑΟΥ
-    4: 938.6 ΣΒΟ
+    4: 938.6ΣΒΟ
     5: '1918'
     8: ΠΥΡΣΟΣ
     9: ΑΘΗΝΑ
     10: '1946'
     11: 222Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΣΑΛΔΑΡΗΣ
     13: ΤΣΑΛΔΑΡΗΣ
@@ -55896,15 +55891,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1095
     1: ΣΙΑΤΟΠΟΥΛΟΣ,ΔΗΜΗΤΡΗΣ
     2: ΣΗΜΕΡΙΝΗ ΕΥΡΩΠΗ
-    4: 914 ΣΙΑ
+    4: 914ΣΙΑ
     5: '383'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 171Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
     13: ΕΥΡΩΠΗ-ΤΑΞΙΔΙΑ
@@ -55993,15 +55988,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1097
     1: ΣΙΔΕΡΗΣ,ΓΙΑΝΝΗΣ
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΝΕΟΥ ΕΛΛΗΝΙΚΟΥ ΘΕΑΤΡΟΥ(1794-1944)
-    4: 886.2 ΣΙΔ
+    4: 886.2ΣΙΔ
     5: '1431'
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 247Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
@@ -56401,15 +56396,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1105
     1: ΣΙΝΟΣ,ΑΛΕΞΑΝΔΡΟΣ
     2: Η ΓΕΩΓΡΑΦΙΚΗ ΕΝΟΤΗΣ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΜΕΣΟΓΕΙΑΚΟΥ ΧΩΡΟΥ
-    4: 914.95 ΣΙΝ
+    4: 914.95ΣΙΝ
     5: 2221-2222-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1945'
     11: 95Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΜΕΣΟΓΕΙΟΣ
     13: ΜΕΣΟΓΕΙΟΣ-ΓΕΩΓΡΑΦΙΚΗ ΕΝΟΤΗΤΑ
@@ -56503,15 +56498,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1107
     1: ΣΙΩΜΟΠΟΥΛΟΣ,ΚΩΣΤΑΣ
     2: Η ΚΑΤΕΡΓΑΡΑ
-    4: 886.2 ΣΙΩ
+    4: 886.2ΣΙΩ
     5: '1529'
     8: Χ.Ε
     9: ΑΡΤΑ
     10: '1930'
     11: 86Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -56607,15 +56602,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1109
     1: ΣΙΩΜΟΠΟΥΛΟΣ,ΤΑΚΗΣ
     2: ΑΛΕΞΑΝΔΡΟΣ ΠΑΛΛΗΣ
     3: ΚΡΙΤΙΚΗ ΜΕΛΕΤΗ
-    4: 880.4 ΣΙΩ
+    4: 880.4ΣΙΩ
     5: '2649'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1955'
     11: 27Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΛΗΣ
@@ -56867,15 +56862,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1114
     1: ΣΙΩΜΟΠΟΥΛΟΣ,ΣΤΥΛΙΑΝΟΣ Κ.
     2: ΠΟΛΕΜΟΣ ΚΑΙΣΑΡΑ ΚΑΙ ΠΟΜΠΗΙΟΥ ΣΤΗΝ ΗΠΕΙΡΟ ΚΑΙ ΤΗΝ ΙΛΛΥΡΙΑ
     3: (49-48Π.Χ)
-    4: 938.21 ΣΙΩ
+    4: 938.21ΣΙΩ
     5: '2244'
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1981'
     11: 91Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΚΑΙΣΑΡΑΣ
@@ -56915,15 +56910,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1115
     1: ΣΚΑΛΤΣΑΡΗ,ΣΤΕΛΛΑ
     2: ΣΤΑ ΒΟΥΝΑ ΚΑΙ ΣΤΑ ΛΑΓΚΑΔΙΑ ΤΗΣ ΣΑΧΑΡΑΣ
-    4: 916 ΣΚΑ
+    4: 916ΣΚΑ
     5: '416'
     8: Χ.Ε
     9: ΠΕΙΡΑΙΑΣ
     10: '1969'
     11: 93Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΣΑΧΑΡΑ
     13: ΤΑΞΙΔΙΑ-ΣΑΧΑΡΑ
@@ -56969,15 +56964,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1116
     1: ΣΚΑΝΔΑΛΗΣ,ΧΡΗΣΤΟΣ
     2: Ο ΣΚΥΛΟΣΟΦΟΣ
     3: ΙΣΤΟΡΙΚΟ ΔΡΑΜΑ
-    4: 886.2 ΣΚΑ
+    4: 886.2ΣΚΑ
     5: '1485'
     8: Χ.Ε
     9: ΓΙΑΝΝΙΝΑ
     10: '1985'
     11: 48Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -57017,15 +57012,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1117
     1: ΣΚΑΝΔΑΛΗΣ,ΧΡΗΣΤΟΣ
     2: ΣΤΗΝ ΑΡΧΑΙΑ ΑΜΒΡΑΚΙΑ
-    4: 938.21 ΣΚΑ
+    4: 938.21ΣΚΑ
     5: '284'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 109Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΑΜΒΡΑΚΙΑ
@@ -57068,15 +57063,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1118
     1: ΣΚΟΥΡΤΗΣ,ΓΙΩΡΓΟΣ
     2: Ο ΚΑΡΑΓΚΙΟΖΗΣ...ΚΑΡΑΓΚΙΟΖΗΣ
-    4: 886.2 ΣΚΟ
+    4: 886.2ΣΚΟ
     5: '1531'
     8: ΚΕΔΡΟΣ
     9: ΑΘΗΝΑ
     10: '1983'
     11: 183Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΑΡΑΓΚΙΟΖΗΣ
@@ -57119,15 +57114,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1119
     1: ΣΜΟΚΟΒΙΤΗΣ,ΓΙΩΡΓΟΣ ΒΑΣ
     2: ΑΝΘΡΩΠΕ ΑΚΟΥ ΤΗ ΜΟΥΣΙΚΗ ΣΟΥ ΠΑΙΞΕ ΣΤΟ ΡΥΘΜΟ ΣΟΥ
-    4: 886.2 ΣΜΟ
+    4: 886.2ΣΜΟ
     5: '1496'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 48Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -57221,15 +57216,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1121
     1: ΣΜΥΡΝΙΑΔΟΣ,ΒΙΩΝΟΣ
     2: Η ΔΗΜΑΓΩΓΙΑ ΕΝ ΑΘΗΝΑΙΣ ΚΑΤΑ ΤΗΝ ΑΡΧΑΙΟΤΗΤΑ
-    4: 938.1 ΣΜΥ
+    4: 938.1ΣΜΥ
     5: '1757'
     8: ΚΛΕΙΣΙΟΥΝΗΣ
     9: ΑΘΗΝΑ
     10: '1945'
     11: 87Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΑΘΗΝΑ-ΑΡΧΑΙΑ ΔΗΜΑΓΩΓΙΑ
@@ -57426,15 +57421,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1125
     1: ΣΟΛΩΜΟΣ,ΑΛΕΞΗΣ
     2: ΘΕΑΤΡΙΚΟ ΤΕΤΡΑΔΙΟ
-    4: 886.2 ΣΟΛ
+    4: 886.2ΣΟΛ
     5: '1410'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 179Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΘΕΑΤΡΙΚΑ ΤΕΤΡΑΔΙΑ
@@ -57533,15 +57528,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1127
     1: ΣΟΛΩΜΟΣ,Δ
     2: ΑΠΑΝΤΑ
-    4: 889.15 ΣΟΛ
+    4: 889.15ΣΟΛ
     5: 46-44-45
     8: ΓΡΗΓΟΡΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 267Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
@@ -57634,15 +57629,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1129
     1: ΣΟΥΛΗΣ,ΧΡΗΣΤΟΣ
     2: ΑΦΙΕΡΩΜΑ ΕΙΣ ΤΗΝ ΗΠΕΙΡΟΝ
-    4: 938.93 ΣΟΥ
+    4: 938.93ΣΟΥ
     5: 2146-2383
     8: ΜΥΡΤΙΔΗ
     9: ΑΘΗΝΑ
     10: '1956'
     11: 253Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΑΦΙΕΡΩΜΑ
@@ -57682,15 +57677,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1130
     1: ΣΟΥΛΤΑΤΗΣ,ΝΙΚΟΛΑΟΣ
     2: Η ΠΑΤΡΙΣ ΜΑΣ
-    4: 938 ΣΟΥ
+    4: 938ΣΟΥ
     5: '1919'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1962'
     11: 79Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΤΡΙΔΑ
     13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -57734,15 +57729,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1131
     1: ΣΟΥΤΖΟΣ,ΔΗΜΗΤΡΙΟΣ
     2: ΑΓΩΝΕΣ ΓΙΑ ΤΗ ΛΕΥΤΕΡΙΑ
     3: ΤΡΕΙΣ ΙΣΤΟΡΙΚΟΙ ΣΤΑΘΜΟΙ ΤΟΥ ΝΕΩΤΕΡΟΥ ΕΛΛΗΝΙΣΜΟΥ 1854,1878,97
-    4: 938.65 ΣΟΥ
+    4: 938.65ΣΟΥ
     5: '2252'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 111Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
     13: ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
@@ -57997,15 +57992,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1136
     1: ΣΟΥΡΑΣ,ΑΘΑΝΑΣΙΟΣ Χ
     2: Η ΣΥΜΒΟΛΗ ΤΩΝ ΑΔΕΛΦΩΝ ΡΙΖΑΡΗ ΕΙΣ ΤΗΝ ΕΠΑΝΑΣΤΑΣΙΝ ΤΟΥ 1821
-    4: 938.5 ΣΟΥ
+    4: 938.5ΣΟΥ
     5: 2729-2730-9266
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1972'
     11: 35Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ 1821
     13: ΕΠΑΝΑΣΤΑΣΗ 1821
@@ -58048,15 +58043,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1137
     1: ΣΠΑΘΑΡΗΣ,ΣΙΜΟΣ
     2: ΤΑ ΤΡΑΓΟΥΔΙΑ ΤΟΥ ΑΙΧΜΑΛΩΤΟΥ (1941-1943)
-    4: 782.42 ΣΠΑ
+    4: 782.42ΣΠΑ
     5: '729'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1973'
     11: 77Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -58277,34 +58272,34 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1142
   authors:
-  - ΣΠΑΡΟΥΝΗΣ,ΑΘΑΝ.Ι
+  - ΣΜΠΑΡΟΥΝΗΣ,ΑΘΑΝ.Ι
   title: ΣΚΕΨΕΙΣ ΤΙΝΕΣ ΔΙΑ ΜΕΤΑΠΟΛΕΜΙΚΗΝ
-  dewey: 938 ΣΠΑ
+  dewey: 938 ΣΜΠ
   entry_numbers:
   - '1959'
   editor: None // ΑΘΗΝΑ
   edition_year: 1945
   pages: 180
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΕΤΑΠΟΛΙΤΕΥΣΗ
   - '1821'
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1142
-    1: ΣΠΑΡΟΥΝΗΣ,ΑΘΑΝ.Ι
+    1: ΣΜΠΑΡΟΥΝΗΣ,ΑΘΑΝ.Ι
     2: ΣΚΕΨΕΙΣ ΤΙΝΕΣ ΔΙΑ ΜΕΤΑΠΟΛΕΜΙΚΗΝ
-    4: 938 ΣΠΑ
+    4: 938ΣΜΠ
     5: '1959'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1945'
     11: 180Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΤΑΠΟΛΙΤΕΥΣΗ
     13: ΜΕΤΑΠΟΛΙΤΕΥΣΗ-1821
@@ -58348,15 +58343,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1143
     1: ΣΠΑΤΑΛΑΣ,ΓΕΡΑΣΙΜΟΣ
     2: ΣΥΓΧΡΟΝΗ ΙΤΑΛΙΚΗ ΠΟΙΗΣΗ
-    4: 851 ΣΠΑ
+    4: 851ΣΠΑ
     5: 230-231
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1959'
     11: 63Σ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΙΤΑΛΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
@@ -58400,15 +58395,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1144
     1: ΣΠΕΡΑΝΤΣΑΣ,ΣΤΕΛΙΟΣ
     2: ΟΙ ΕΛΛΗΝΕΣ ΓΙΑΤΡΟΙ-ΛΟΓΟΤΕΧΝΕΣ
     3: ΑΠΟ ΤΗΝ ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ ΩΣ ΣΤΑ ΣΗΜΕΡΑ
-    4: 880.3 ΣΠΕ
+    4: 880.3ΣΠΕ
     5: '196'
     8: ΠΕΧΛΙΒΑΝΙΔΗΣ
     9: ΑΘΗΝΑ
     10: '1961'
     11: 199Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΓΙΑΤΡΟΙ
@@ -58501,15 +58496,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1146
     1: ΣΤΑΘΑΚΗΣ,ΙΩΑΝΝΗΣ
     2: Η ΖΩΗ ΜΟΥ ΕΙΣ ΜΙΑΝ ΑΚΤΙΝΑ ΗΛΙΟΥ
-    4: 938.7 ΣΤΑ
+    4: 938.7ΣΤΑ
     5: '2108'
     8: ΓΕΩΡΓΙΑΔΗΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 247Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΦΗΓΗΣΕΙΣ
     13: ΠΟΛΙΤΙΚΕΣ-ΑΦΗΓΗΣΕΙΣ
@@ -58549,15 +58544,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1147
     1: ΣΤΑΘΑΚΗΣ,ΝΙΚΟΣ Α
     2: ΑΠΟ ΤΗ ΣΤΑΧΤΗ ΣΤΗ ΖΩΗ
-    4: 950 ΣΤΑ
+    4: 950ΣΤΑ
     5: '2638'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1982'
     11: 257Σ
     12: ΑΣΙΑΤΙΚΗ ΙΣΤΟΡΙΑ
     13: ΑΣΙΑ-ΙΣΤΟΡΙΑ
@@ -58599,15 +58594,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1148
     1: ΣΤΑΘΑΚΟΠΟΥΛΟΣ,ΛΟΥΚΑΣ
     2: ΑΝΘΟΛΟΓΙΑ ΠΟΙΗΤΩΝ ΑΡΓΟΛΙΔΟΣ
-    4: 880.08 ΣΤΑ
+    4: 880.08ΣΤΑ
     5: '640'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1958'
     11: 256Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΑΝΘΟΛΟΓΙΑ
@@ -58699,15 +58694,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1150
     1: ΣΤΑΘΗΣ,ΓΕΩΡΓΙΟΣ
     2: ΑΠΟ Τ'ΑΓΡΑΦΑ
-    4: 938.93 ΣΤΑ
+    4: 938.93ΣΤΑ
     5: '313'
     8: Χ.Ε
     9: Η.Π.Α
     10: '1957'
     11: 267Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΡΑΦΑ
     13: ΑΓΡΑΦΑ-ΙΣΤΟΡΙΑ
@@ -58799,15 +58794,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1152
     1: ΣΤΑΛΙΟΣ,Ζ
     2: ΙΑΠΩΝΙΑ
-    4: 915 ΣΤΑ
+    4: 915ΣΤΑ
     5: '452'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1962'
     11: 238Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΙΑΠΩΝΙΑ
     13: ΤΑΞΙΔΙΑ-ΙΑΠΩΝΙΑ
@@ -58850,15 +58845,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1153
     1: ΣΤΑΜΑΤΟΠΟΥΛΟΣ,ΤΑΚΗΣ Α
     2: Ο ΕΣΩΤΕΡΙΚΟΣ ΑΓΩΝΑΣ ΠΡΙΝ ΚΑΙ ΚΑΤΑ ΤΗΝ ΕΠΑΝΑΣΤΑΣΗ ΤΟΥ 1821
-    4: 938.41 ΣΤΑ
+    4: 938.41ΣΤΑ
     5: '1810'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1957'
     11: 422Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ 1821
     13: ΕΠΑΝΑΣΤΑΣΗ 1821-ΕΣΩΤΕΡΙΚΟΣ ΑΓΩΝΑΣ
@@ -59259,15 +59254,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1161
     1: ΣΤΑΣΙΝΟΠΟΥΛΟΣ,ΝΙΚΟΣ Α.
     2: ΤΡΑΓΟΥΔΙΑ ΣΤΑ ΚΑΛΑΒΡΥΤΑ
-    4: 782.42 ΣΤΑ
+    4: 782.42ΣΤΑ
     5: '747'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 30Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -59415,15 +59410,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1164
     1: ΣΤΑΥΡΙΔΟΥ,ΜΑΡΙΑ
     2: ΣΥΓΧΡΟΝΟ ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ
-    4: 886.2 ΣΤΑ
+    4: 886.2ΣΤΑ
     5: 1491-1490
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1976'
     11: 163Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΣΥΓΧΡΟΝΟ
@@ -59469,15 +59464,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1165
     1: ΣΤΑΥΡΙΔΟΥ,ΜΑΡΙΑ
     2: ΣΥΓΧΡΟΝΟ ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ
-    4: 886.2 ΣΤΑ
+    4: 886.2ΣΤΑ
     5: '1489'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1979'
     11: 207Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΣΥΓΧΡΟΝΟ
@@ -59521,15 +59516,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1166
     1: ΣΤΑΥΡΟΥ,ΤΑΤΙΑΝΑ
     2: ΤΕΤΡΑΔΙΑ ΜΝΗΜΗΣ
-    4: 880.3 ΣΤΑ
+    4: 880.3ΣΤΑ
     5: '1009'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1982'
     11: 110Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΜΥΡΙΒΗΛΗΣ
@@ -59622,15 +59617,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1168
     1: ΣΤΑΥΡΟΠΟΥΛΟΣ,ΧΑΡΑΛΑΜΠΟΣ Π
     2: Η ΖΩΗ ΤΟΥ ΕΛΛΗΝΟΣ ΣΤΗΝ ΑΜΕΡΙΚΗ
-    4: 938.99 ΣΤΑ
+    4: 938.99ΣΤΑ
     5: '2346'
     7: 2ΕΚΔ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1956'
     11: 95Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΔΙΑΣΠΟΡΑΣ
@@ -59771,15 +59766,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1171
     1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,ΚΩΝΣΤ.
     2: ΠΑΡΑΤΗΡΗΣΕΙΣ ΕΙΣ ΤΗΝ ΝΕΩΤΕΡΑΝ ΓΕΩΓΡΑΦΙΑΝ ΤΗΣ ΗΠΕΙΡΟΥ
-    4: 914.95 ΣΤΕ
+    4: 914.95ΣΤΕ
     5: '2544'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1937'
     11: 98Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΓΕΩΓΡΑΦΙΑ
@@ -59824,15 +59819,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1172
     1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ.
     2: ΟΙ ΥΠΕΥΘΥΝΟΙ ΠΟΛΕΜΟΥ ΚΑΤΑ ΤΟΥΣ ΑΡΧΑΙΟΥΣ ΧΡΟΝΟΥΣ
-    4: 938.1 ΣΤΕ
+    4: 938.1ΣΤΕ
     5: 2515-2586
     8: ΣΙΔΕΡΗ
     9: ΑΘΗΝΑ
     10: '1952'
     11: 192Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ-ΥΠΕΥΘΥΝΟΙ ΠΟΛΕΜΟΥ
@@ -59873,15 +59868,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1173
     1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ.
     2: ΤΑ ΒΟΡΕΙΑ ΣΥΝΟΡΑ ΤΗΣ ΗΠΕΙΡΟΥ
-    4: 938.93 ΣΤΕ
+    4: 938.93ΣΤΕ
     5: '2553'
     8: ΓΡΗΓΟΡΙΑΔΗ
     9: ΑΘΗΝΑ
     10: '1945'
     11: 79Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΣΥΝΟΡΑ
@@ -59924,15 +59919,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1174
     1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
     2: Η ΑΡΧΑΙΑ ΑΙΤΩΛΙΑ
-    4: 938.22 ΣΤΕ
+    4: 938.22ΣΤΕ
     5: 2215-2587
     8: ΔΗΜΗΤΡΑΚΟΥ
     9: ΑΘΗΝΑ
     10: '1939'
     11: 191Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΙΑ
@@ -59974,15 +59969,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1175
     1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
     2: Η ΙΣΤΟΡΙΚΗ ΜΝΗΜΗ
-    4: 938 ΣΤΕ
+    4: 938ΣΤΕ
     5: '2110'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1972'
     11: 21Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΝΗΜΗ
     13: ΜΝΗΜΗ ΙΣΤΟΡΙΚΗ
@@ -60232,15 +60227,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1180
     1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
     2: ΑΙ ΗΠΕΙΡΩΤΙΣΣΑΙ ΕΙΣ ΤΟΥΣ ΕΘΝΙΚΟΥΣ ΑΓΩΝΑΣ
-    4: 938 ΣΤΕ
+    4: 938ΣΤΕ
     5: 2030-2031-9268
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 32Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΙΣΣΕΣ
@@ -60739,15 +60734,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1190
     1: ΣΕΜΠΕΡ ΚΑΙ ΡΟΥΣΣΕΤ
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΓΑΛΛΟ-ΓΕΡΜΑΝΙΚΟΥ ΠΟΛΕΜΟΥ (1870-1871)
-    4: 940.2 ΣΕΜ
+    4: 940.2ΣΕΜ
     5: '2311'
     6: ΝΕΟΚΛΕΟΥΣ,Χ
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1898'
     11: 556Σ
     12: ΕΥΡΩΠΑΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
@@ -60791,15 +60786,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1191
     1: ΣΤΡΑΒΟΛΕΜΟΣ,ΔΙΟΝΥΣΙΟΣ Χ.
     2: ΕΝΑΣ ΗΡΩΙΣΜΟΣ-ΜΙΑ ΔΙΚΑΙΩΣΗ
     3: Η ΔΙΑΣΩΣΗ ΤΩΝ ΕΒΡΑΙΩΝ ΤΗΣ ΖΑΚΥΝΘΟΥ ΣΤΗ ΚΑΤΟΧΗ
-    4: 938.7 ΣΤΡ
+    4: 938.7ΣΤΡ
     5: '1985'
     8: Χ.Χ
     9: ΑΘΗΝΑ
     10: '1988'
     11: 124Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΖΑΚΥΝΘΟΣ
     13: ΖΑΚΥΝΘΟΣ-ΚΑΤΟΧΗ
@@ -60826,14 +60821,15 @@
   authors:
   - ΣΤΡΑΤΗΣ,ΚΩΝ
   title: ΧΡΟΝΙΚΟΝ ΑΡΤΗΣ
   dewey: 938.939 ΣΤΡ
   entry_numbers:
   - '2148'
   - '8014'
+  - '10001'
   editor: None // ΑΡΤΑ
   edition_year: 1969
   pages: 176
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΑΡΤΑ
   - ΧΡΟΝΙΚΟ
@@ -60842,15 +60838,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1192
     1: ΣΤΡΑΤΗΣ,ΚΩΝ
     2: ΧΡΟΝΙΚΟΝ ΑΡΤΗΣ
     4: 938.939ΣΤΡ
-    5: 2148-8014
+    5: 2148-8014-10001
     8: Χ.Ε
     9: ΑΡΤΑ
     10: '1969'
     11: 176Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
     13: ΑΡΤΑ-ΧΡΟΝΙΚΟ
     14: ΧΡΟΝΙΚΟ-ΑΡΤΑ
@@ -60890,15 +60886,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1193
     1: ΣΤΡΑΤΗΣ,ΚΩΝΑΝΤΩΝ
     2: ΑΜΒΡΑΚΙΑ-ΑΡΑΧΘΕΙΑ ΑΚΑΡΝΑΝΙΚΗ-ΑΡΤΑ
-    4: 938.21 ΣΤΡ
+    4: 938.21ΣΤΡ
     5: '2259'
     8: Χ.Ε
     9: ΑΡΤΑ
     10: '1976'
     11: 97Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΜΒΡΑΚΙΑ
     13: ΑΜΒΡΑΚΙΑ-ΙΣΤΟΡΙΑ
@@ -60989,15 +60985,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1195
     1: ΣΥΓΚΕΛΛΟΣ,ΓΕΩΡΓΙΟΣ
     2: ΕΚΛΟΓΗ ΧΡΟΝΟΓΡΑΦΙΑΣ
-    4: 938.31 ΣΥΓ
+    4: 938.31ΣΥΓ
     5: '2548'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 788Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
     13: ΒΥΖΑΝΤΙΟ-ΧΡΟΝΟΓΡΑΦΙΑ
@@ -61040,15 +61036,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1196
     1: ΣΥΝΑΔΙΝΟΣ,ΝΙΚ Θ
     2: ΔΑΝΙΑ
     3: Η ΧΩΡΑ ΤΟΥ ΑΝΤΕΡΣΕΝ
-    4: 914.49 ΣΥΝ
+    4: 914.49ΣΥΝ
     5: '401'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1964'
     11: 130Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΔΑΝΙΑ
     13: ΤΑΞΙΔΙΑ-ΔΑΝΙΑ
@@ -61087,15 +61083,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1197
     1: ΣΥΡΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
     2: Η ΑΜΕΡΙΚΗ ΧΩΡΙΣ ΦΑΝΤΑΣΙΑ
-    4: 970 ΣΥΡ
+    4: 970ΣΥΡ
     5: '437'
     8: ΑΕΤΟΣ
     9: ΑΘΗΝΑ
     10: '1954'
     11: 176Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ
     13: ΑΜΕΡΙΚΗ-ΙΣΤΟΡΙΑ
@@ -61291,15 +61287,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1201
     1: ΣΩ,ΜΠΕΡΝΑΡ
     2: Ο ΑΝΘΡΩΠΟΣ ΚΑΙ ΤΑ ΟΠΛΑ
-    4: 828.99 ΣΩ
+    4: 828.99ΣΩ
     5: '1369'
     6: ΜΠΕΛΛΟΥ,ΖΕΤΤΑ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 151Σ
     12: ΙΡΛΑΝΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -61397,15 +61393,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1203
     1: ΤΑΞΙΑΡΧΗΣ,ΝΤΙΝΟΣ
     2: ΕΝΑ ΔΡΑΜΑ ΤΙΜΗΣ
     3: ΜΟΝΟΠΡΑΚΤΟ
-    4: 886.2 ΤΑΞ
+    4: 886.2ΤΑΞ
     5: '1521'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1960'
     11: 46Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΜΟΝΟΠΡΑΚΤΟ
@@ -61546,15 +61542,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1206
     1: ΤΑΡΣΟΥΛΗ,ΓΕΩΡΓΙΑ
     2: ΜΩΡΑΙΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
-    4: 782.42 ΤΑΡ
+    4: 782.42ΤΑΡ
     5: '726'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 208Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -61601,15 +61597,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1207
     1: ΤΑΤΣΙΟΠΟΥΛΟΣ,ΛΑΜΠΡΟΣ ΑΠ
     2: ΝΙΚΟΛΑΟΣ ΣΚΟΥΦΑΣ
-    4: 886.2 ΤΑΤ
+    4: 886.2ΤΑΤ
     5: 1482-1483-9279Α
     8: Χ.Ε
     9: ΑΡΤΑ
     10: '1971'
     11: 40Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -61692,14 +61688,15 @@
   title: ΝΙΚΟΛΑΟΣ ΣΚΟΥΦΑΣ
   subtitle: Ο ΕΘΝΕΓΕΡΤΗΣ ΑΡΧΗΓΟΣ ΤΗΣ ΦΙΛΙΚΗΣ ΕΤΑΙΡΕΙΑΣ
   dewey: 938.487 ΤΑΤ
   entry_numbers:
   - '2256'
   - '1034'
   - '1661'
+  - '1482.'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1980
   pages: 73
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΣΚΟΥΦΑΣ
   - ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
@@ -61709,15 +61706,15 @@
   offprint: false
   original_entry:
     0: 1209
     1: ΤΑΤΣΙΟΠΟΥΛΟΣ,ΛΑΜΠΡΟΣ ΑΠ
     2: ΝΙΚΟΛΑΟΣ ΣΚΟΥΦΑΣ
     3: Ο ΕΘΝΕΓΕΡΤΗΣ ΑΡΧΗΓΟΣ ΤΗΣ ΦΙΛΙΚΗΣ ΕΤΑΙΡΕΙΑΣ
     4: 938.487ΤΑΤ
-    5: 2256-1034-1661
+    5: 2256-1034-1661-1482.
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1980'
     11: 73Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΟΥΦΑΣ
     13: ΣΚΟΥΦΑΣ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
     14: ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ-ΣΚΟΥΦΑΣ
@@ -61758,15 +61755,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1210
     1: ΤΑΤΣΙΟΠΟΥΛΟΣ,ΛΑΜΠΡΟΣ ΑΠ.
     2: ΕΥΣΤΑΘΙΟΣ ΓΕΡΟΣΤΑΘΗΣ
     3: Ο ΣΟΦΟΣ ΔΑΣΚΑΛΟΣ
-    4: 938.7 ΤΑΤ
+    4: 938.7ΤΑΤ
     5: '2405'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1982'
     11: 78Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ- ΓΕΡΟΣΤΑΘΗΣ
     13: ΓΕΡΟΣΤΑΘΗΣ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
@@ -61907,15 +61904,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1213
     1: ΤΕΝΕΚΙΔΟΣ,ΓΕΩΡΓΙΟΣ
     2: ΑΙ ΑΡΧΑΙΟΕΛΛΗΝΙΚΑΙ ΡΙΖΑΙ ΤΟΥ ΕΙΚΟΣΙΕΝΑ
-    4: 938.5 ΤΕΝ
+    4: 938.5ΤΕΝ
     5: '1879'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1962'
     11: 43Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821
     13: 1821-ΠΑΝΗΓΥΡΙΚΟΣ ΛΟΓΟΣ
@@ -62116,15 +62113,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1217
     1: ΤΕΡΖΑΚΗΣ,ΑΓΓΕΛΟΣ
     2: Ο ΣΤΑΥΡΟΣ ΚΑΙ ΤΟ ΣΠΑΘΙ
     3: ΤΡΑΓΩΔΙΑ
-    4: 886.2 ΤΕΡ
+    4: 886.2ΤΕΡ
     5: '1525'
     8: ΑΕΤΟΣ
     9: ΑΘΗΝΑ
     10: '1950'
     11: 125Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
@@ -62214,15 +62211,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1219
     1: ΤΕΡΖΑΚΗΣ,ΑΓΓΕΛΟΣ
     2: ΘΕΑΤΡΟ
-    4: 886.2 ΤΕΡ
+    4: 886.2ΤΕΡ
     5: '1568'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 238Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
@@ -62562,15 +62559,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1226
     1: ΤΖΙΑΚΟΖΑ,ΙΩΣΗΦ
     2: ΣΑΝ ΤΑ ΦΥΛΛΑ
     3: ΚΩΜΩΔΙΑ
-    4: 852 ΤΖΙ
+    4: 852ΤΖΙ
     5: '1392'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1916'
     11: 84Σ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΙΤΑΛΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
@@ -62612,15 +62609,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1227
     1: ΤΖΙΟΒΑΣ,ΔΗΜΗΤΡΙΟΣ
     2: Η ΠΕΖΟΓΡΑΦΙΑ ΤΟΥ ΔΗΜΗΤΡΗ ΧΑΤΖΗ
-    4: 880.5 ΤΖΙ
+    4: 880.5ΤΖΙ
     5: '2645'
     8: Χ.Ε
     9: ΓΙΑΝΝΙΝΑ
     10: '1980'
     11: 23Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -62763,15 +62760,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1230
     1: ΤΖΟΥΝΗΣ,ΤΡΙΑΝΤ
     2: ΜΕΤΑ 49 ΧΡΟΝΙΑ ΣΤΗΝ ΠΑΛΙΑ ΠΑΤΡΙΔΑ
     3: Η ΝΟΣΤΑΛΓΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΘΡΑΚΗΣ
-    4: 938 ΤΖΟ
+    4: 938ΤΖΟ
     5: '2140'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1966'
     11: 15Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
     13: ΘΡΑΚΗ-ΕΛΛΗΝΕΣ
@@ -62911,15 +62908,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1233
     1: ΔΙΑΜΑΝΤΟΠΟΥΛΟΣ,ΙΑΚΩΒΟΣ Γ.
     2: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΗΝ 15 ΙΟΥΛΙΟΥ 1965
-    4: 938.78 ΔΙΑ
+    4: 938.78ΔΙΑ
     5: '2781'
     8: Χ.Ε
     9: Χ.Τ
     10: '1972'
     11: 30Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΑΜΝΗΣΕΙΣ
     13: ΑΝΑΜΝΗΣΕΙΣ-1965
@@ -63012,15 +63009,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1235
     1: ΚΑΛΟΓΙΑΝΝΗΣ,ΒΑΣΟΣ
     2: Η ΧΡΥΣΗ ΒΙΒΛΟΣ ΤΟΥ ΔΗΜΟΥ-ΛΑΡΙΣΗΣ
     3: ΑΠΟ ΤΗΝ ΜΑΚΡΑΙΩΝΗ ΙΣΤΟΡΙΑ ΤΗΣ ΘΕΣΣΑΛΙΚΗΣ ΠΡΩΤΕΥΟΥΣΗΣ
-    4: 938.21 ΚΑΛ
+    4: 938.21ΚΑΛ
     5: '2374'
     8: ΔΗΜΗΤΡΑΚΟΠΟΥΛΟΥ
     9: ΛΑΡΙΣΑ
     10: '1963'
     11: 390Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΣΑΛΙΑ-ΛΑΡΙΣΑ
     13: ΘΕΣΣΑΛΙΑ-ΛΑΡΙΣΑ
@@ -63112,15 +63109,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1237
     1: ΠΕΤΣΑΣ,ΦΩΤΙΟΣ Μ.
     2: ΣΕΛΙΔΕΣ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΤΩΝ ΗΠΕΙΡΩΤΩΝ
     3: ΑΠΟ ΤΟΥΣ ΜΥΘΙΚΟΥΣ ΧΡΟΝΟΥΣ ΩΣ ΤΗΣ ΜΕΡΕΣ ΜΑΣ
-    4: 938.21 ΠΕΤ
+    4: 938.21ΠΕΤ
     5: '2815'
     8: ΙΑΙΑΧ
     9: ΙΩΑΝΝΙΝΑ
     10: '1993'
     11: 254Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ
@@ -63212,15 +63209,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1239
     1: ΛΑΖΑΡΙΔΗΣ,ΚΩΣΤΑΣ Π.
     2: ΑΠΟ ΤΑ ΛΑΟΓΡΑΦΙΚΑ ΤΟΥ ΧΩΡΙΟΥ ΜΟΥ ΚΟΥΚΟΥΛΙΟΥ-ΖΑΓΟΡΙΟΥ
-    4: 938.93 ΛΑΖ
+    4: 938.93ΛΑΖ
     5: '310'
     8: ΗΠ.ΕΣΤΙΑ
     9: ΓΙΑΝΝΙΝΑ
     10: '1980'
     11: 63Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΚΟΥΚΟΥΛΙΑ
@@ -63266,15 +63263,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1240
     1: ΣΑΛΑΜΑΓΚΑΣ,Δ
     2: ΕΛΕΝΗ ΑΓΓΕΛΙΝΑ ΔΟΥΚΑΙΝΑ
     3: Η ΤΡΑΓΙΚΗ ΜΟΡΦΗ ΜΙΑΣ ΗΠΕΙΡΩΤΟΠΟΥΛΑΣ ΠΡΙΓΚΗΠΕΣΣΑΣ
-    4: 938.4 ΣΑΛ
+    4: 938.4ΣΑΛ
     5: '2800'
     8: Χ.Ε
     9: ΓΙΑΝΝΙΝΑ
     10: '1961'
     11: 13Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΠΡΩΣΟΠΑ
@@ -63317,15 +63314,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1241
     1: ΣΟΥΡΑΣ,ΑΘΑΝΑΣΙΟΣ
     2: ΟΙ ΔΙΟΙΚΗΣΑΝΤΕΣ ΤΑ ΤΗΣ ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΚΑΤΑ ΤΗΝ ΑΠΟ ΤΗΣ
     3: ΑΝΑΣΥΣΤΑΣΕΩΣ ΤΗΣ ΤΕΣΣΑΡΑΚΟΝΤΑΕΤΗ ΠΕΡΙΟΔΟΝ 1934-1974
-    4: 938.93 ΣΟΥ
+    4: 938.93ΣΟΥ
     5: '2782'
     8: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
     9: ΑΘΗΝΑ
     10: '1977'
     11: 13Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
@@ -63364,15 +63361,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1242
     1: ΤΟΥΝΓΚ,ΜΑΟ ΤΣΕ
     2: ΤΟ ΚΟΚΚΙΝΟ ΒΙΒΛΙΟ
-    4: 952 ΤΟΥ
+    4: 952ΤΟΥ
     5: '2576'
     8: ΓΕΡΟΝΤΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 227Σ
     12: ΙΑΠΩΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΕΚΙΝΟ
     13: ΠΕΚΙΝΟ-ΙΣΤΟΡΙΑ
@@ -63464,15 +63461,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1244
     1: ΤΟΥΡΛΙΔΟΣ,ΓΕΩΡΓΙΟΣ ΑΘ
     2: Η ΘΡΑΚΗ ΕΝ ΤΗ ΠΟΙΗΣΕΙ ΤΟΥ ΕΝΝΙΟΥ
-    4: 880.1 ΤΟΥ
+    4: 880.1ΤΟΥ
     5: '2696'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 6Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΘΡΑΚΗ
@@ -63564,15 +63561,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1246
     1: ΤΟΥΡΛΙΔΟΣ,ΓΕΩΡΓΙΟΣ ΑΘ
     2: Η ΕΠΕΚΤΑΤΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΡΩΜΗΣ ΚΑΙ Ο ΟΡΑΤΙΟΣ
-    4: 938.19 ΤΟΥ
+    4: 938.19ΤΟΥ
     5: '2513'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1976'
     11: 95Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ
     13: ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ-ΟΡΑΤΙΟΣ
@@ -63716,15 +63713,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1249
     1: ΔΕΛΑΠΟΡΤΑΣ,ΠΑΥΛΟΣ Γ.
     2: ΜΝΗΜΗ ΓΕΩΡΓΙΟΥ ΓΚΑΛΚΟΥ
-    4: 938.7 ΔΕΛ
+    4: 938.7ΔΕΛ
     5: 2796-3695
     8: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
     9: ΑΘΗΝΑ
     10: '1977'
     11: 38Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΓΚΑΛΚΟΣ
@@ -63765,15 +63762,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1250
     1: ΒΙΤΤΗΣ,ΦΩΤΗΣ Σ.
     2: ΙΣΤΟΡΙΚΑ ΠΑΡΑΔΟΣΙΑΚΑ ΠΑΡΑΘΕΜΑΤΑ
-    4: 938.4 ΒΙΤ
+    4: 938.4ΒΙΤ
     5: '2766'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1984'
     11: 8Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΡΑΔΟΣΗ
     13: ΠΑΡΑΔΟΣΗ-1821
@@ -63870,15 +63867,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1252
     1: ΤΣΟΥΚΑΝΕΛΗΣ,ΑΛΕΞΑΝΔΡΟΣ Σ
     2: ΧΑΡΑΛΑΜΠΟΣ ΚΑΤΣΙΜΗΤΡΟΣ
     3: ΠΡΟΜΑΧΟΣ ΤΗΣ ΗΠΕΙΡΟΥ
-    4: 938.7 ΤΣΟ
+    4: 938.7ΤΣΟ
     5: 2765-9282
     8: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
     9: ΑΘΗΝΑ
     10: '1978'
     11: 93Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΚΑΤΣΙΜΗΤΡΟΣ
@@ -63996,18 +63993,17 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1255
-  authors:
-  - ΤΡΙΚΟΥΠΗΣ,ΧΑΡΙΛΑΟΣ
+  authors: []
   title: ΠΕΡΙ ΧΑΡΙΛΑΟΥ ΤΡΙΚΟΥΠΗ
-  dewey: 938.647 ΤΡΙ
+  dewey: 938.647 ΧΣ
   entry_numbers:
   - '1938'
   - '1937'
   - '1936'
   - '1935'
   - '1933'
   - '1870'
@@ -64026,17 +64022,17 @@
   - ΤΡΙΚΟΥΠΗΣ
   - ΑΝΑΛΕΚΤΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1255
-    1: ΤΡΙΚΟΥΠΗΣ,ΧΑΡΙΛΑΟΣ
+    1: Χ.Σ
     2: ΠΕΡΙ ΧΑΡΙΛΑΟΥ ΤΡΙΚΟΥΠΗ
-    4: 938.647ΤΡΙ
+    4: 938.647Χ.Σ
     5: 1938-1937-1936-1935-
     6: 1933-1870-1869-1866-
     7: '1932'
     8: ΣΑΚΕΛΛΑΡΙΟΥ
     9: ΑΘΗΝΑ
     10: '1907'
     11: 1064Σ
@@ -64127,15 +64123,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1257
     1: ΤΡΟΥΣΛΟ,ΑΝΤΑΜΣ
     2: Η ΕΠΟΠΟΙΙΑ ΤΗΣ ΑΜΕΡΙΚΗΣ
-    4: 970 TRU
+    4: 970TRU
     5: '433'
     8: ΑΕΤΟΣ
     9: ΑΘΗΝΑ
     10: '1952'
     11: 244Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΟΠΟΙΙΑ
     13: ΑΜΕΡΙΚΗ-ΕΠΟΠΟΙΙΑ
@@ -64279,15 +64275,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1260
     1: ΤΣΑΚΩΝΑΣ,ΔΗΜ Γ.
     2: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΟΝ ΝΕΟΝ ΕΛΛΗΝΙΣΜΟΝ
-    4: 938.7 ΤΣΑ
+    4: 938.7ΤΣΑ
     5: '1903'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1958'
     11: 191Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
     13: ΕΛΛΗΝΙΣΜΟΣ
@@ -64379,15 +64375,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1262
     1: ΤΣΑΠΑΛΗΣ,ΛΑΜΠΡΟΣ
     2: ΣΥΝΤΟΜΗ ΙΣΤΟΡΙΑ ΗΠΕΙΡΟΥ
-    4: 938.21 ΤΣΑ
+    4: 938.21ΤΣΑ
     5: '2265'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1988'
     11: 15Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
@@ -64481,15 +64477,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1264
     1: ΤΣΑΡΜΑΚΗΣ,ΑΘΑΝΑΣΙΟΣ Γ.
     2: ΛΑΜΙΑ-ΤΕΠΕΛΕΝΙ 1940
-    4: 938.75 ΤΣΑ
+    4: 938.75ΤΣΑ
     5: '2019'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1981'
     11: 87Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΛΑΜΙΑ
     13: ΛΑΜΙΑ-1940
@@ -64577,15 +64573,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1266
     1: ΤΣΑΤΣΟΣ,ΚΩΝ/ΝΟΣ
     2: ΑΙΣΘΗΤΙΚΑ ΔΟΚΙΜΙΑ
-    4: 880.4 ΤΣΑ
+    4: 880.4ΤΣΑ
     5: '1229'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1961'
     11: 214Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΟΚΙΜΙΑ
     13: ΔΟΚΙΜΙΑ-ΑΙΣΘΗΤΙΚΑ
@@ -64627,15 +64623,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1267
     1: ΤΣΑΤΣΟΣ,ΚΩΝ/ΝΟΣ
     2: ΑΙΣΘΗΤΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
-    4: 880.4 ΤΣΑ
+    4: 880.4ΤΣΑ
     5: '1230'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 283Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΕΛΕΤΗΜΑΤΑ
     13: ΜΕΛΕΤΗΜΑΤΑ-ΑΙΣΘΗΤΙΚΑ
@@ -65035,15 +65031,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1275
     1: ΤΣΕΧΩΦ,ΑΝΤΟΝ
     2: Ο ΓΛΑΡΟΣ-ΘΕΙΟΣ ΒΑΝΙΑΣ-ΠΡΟΤΑΣΗ ΓΑΜΟΥ-Η ΑΡΚΟΥΔΑ
-    4: 891.7 ΤΣΕ
+    4: 891.7ΤΣΕ
     5: 1563-1562-
     6: ΚΑΛΕΡΓΗΣ,ΛΥΚΟΥΡΓΟΣ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: '1986'
     11: 230Σ
     12: ΡΩΣΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -65084,15 +65080,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1276
     1: ΤΣΙΑΤΗΣ,ΒΑΣΙΛΗΣ Ε
     2: ΣΚΑΝΔΙΝΑΒΙΚΗ ΑΝΑΠΟΛΗΣΗ
-    4: 914.48 ΤΣΙ
+    4: 914.48ΤΣΙ
     5: '403'
     8: Χ.Ε
     9: ΠΕΙΡΑΙΑ
     10: '1985'
     11: 154Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΣΚΑΝΔΙΝΑΒΙΑ
     13: ΤΑΞΙΔΙΑ-ΣΚΑΝΔΙΝΑΒΙΑ
@@ -65133,15 +65129,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1277
     1: ΤΣΙΑΤΗΣ,ΒΑΣΙΛΗΣ
     2: ΗΛΙΟΛΟΥΣΤΗ ΚΑΙ ΘΑΛΑΣΣΟΦΙΛΗΤΗ ΧΩΡΑ
-    4: 889.21 ΤΣΙ
+    4: 889.21ΤΣΙ
     5: '377'
     8: Χ.Ε
     9: ΠΕΙΡΑΙΑ
     10: '1981'
     11: 170Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΥΠΡΟΣ
     13: ΤΑΞΙΔΙΑ-ΚΥΠΡΟΣ
@@ -65233,15 +65229,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1279
     1: ΤΣΙΜΑΝΗΣ,ΠΡΟΚΟΠΙΟΣ
     2: ΟΙ ΠΑΤΡΙΑΡΧΑΙ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ
-    4: 938.4 ΤΣΙ
+    4: 938.4ΤΣΙ
     5: 1811-1812-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1981'
     11: 384Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
     13: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΠΑΤΡΙΑΡΧΕΣ
@@ -65387,15 +65383,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1282
     1: ΤΣΙΡΟΠΟΥΛΟΣ,ΚΩΣΤΑΣ Ε.
     2: ΑΜΕΡΙΚΑΝΙΚΗ ΑΝΘΡΩΠΟΓΕΩΓΡΑΦΙΑ
-    4: 917 ΤΣΙ
+    4: 917ΤΣΙ
     5: 429-430
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1976'
     11: 153Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΑΜΕΡΙΚΗ
     13: ΑΜΕΡΙΚΗ-ΑΝΘΡΩΠΟΓΕΩΓΡΑΦΙΑ
@@ -65436,15 +65432,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1283
     1: ΤΣΙΡΠΑΝΛΗΣ,ΖΑΧ Ν.
     2: Η ΔΥΤΙΚΗ ΕΥΡΩΠΗ ΣΤΟΥΣ ΜΕΣΟΥΣ ΧΡΟΝΟΥΣ(5-15ΑΙ)
-    4: 940.1 ΤΣΙ
+    4: 940.1ΤΣΙ
     5: '2496'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1973'
     11: 289Σ
     12: ΕΥΡΩΠΑΙΚΗ ΙΣΤΟΡΙΑ-(5-15ΑΙ)
     13: ΕΥΡΩΠΗ-ΙΣΤΟΡΙΑ
@@ -65487,15 +65483,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1284
     1: ΤΣΙΤΣΑΣ,ΣΕΡΑΦΕΙΜ Κ.
     2: Ο ΤΡΑΓΟΥΔΙΣΤΗΣ ΤΟΥ ΒΟΥΝΟΥ ΚΑΙ ΤΟΥ ΔΑΣΟΥΣ
-    4: 782.42 ΤΣΙ
+    4: 782.42ΤΣΙ
     5: '715'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1980'
     11: 63Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -65535,15 +65531,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1285
     1: ΤΣΙΤΣΑΣ,ΣΕΡΑΦΕΙΜ Κ.
     2: Τ'ΑΓΡΑΦΑ ΤΗΣ ΠΙΝΔΟΥ
-    4: 938.93 ΤΣΙ
+    4: 938.93ΤΣΙ
     5: '314'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 95Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΡΑΦΑ
     13: ΑΓΡΑΦΑ-ΙΣΤΟΡΙΑ
@@ -65633,15 +65629,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1287
     1: ΤΣΟΚΟΠΟΥΛΟΣ,Γ.Β
     2: ΓΥΝΑΙΚΕΣ ΤΟΥ ΒΥΖΑΝΤΙΟΥ
-    4: 938.3 ΤΣΟ
+    4: 938.3ΤΣΟ
     5: '1983'
     8: ΣΙΔΕΡΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 162Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
     13: ΒΥΖΑΝΤΙΟ-ΓΥΝΑΙΚΕΣ
@@ -65733,15 +65729,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1289
     1: ΤΣΟΝΙΔΗΣ,ΤΑΚΗΣ ΧΡ.
     2: ΤΟ ΓΕΝΟΣ ΚΑΡΑΘΕΟΔΩΡΗ 1740-1950
-    4: 938.4 ΤΣΟ
+    4: 938.4ΤΣΟ
     5: 2447-2446
     8: Χ.Ε
     9: Ν.ΟΡΕΣΤΙΑ
     10: '1989'
     11: 352Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΚΑΡΑΘΕΟΔΩΡΗ-(1740-1950)
@@ -65833,15 +65829,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1291
     1: ΤΣΟΥΤΣΙΝΟΣ,ΓΙΑΝΝΗΣ
     2: ΠΕΝΤΕ ΑΡΤΙΝΑ ΜΕΛΕΤΗΜΑΤΑ
-    4: 938.21 ΤΣΟ
+    4: 938.21ΤΣΟ
     5: 2481-2482
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1982'
     11: 38Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
     13: ΑΡΤΑ-ΜΕΛΕΤΗΜΑΤΑ
@@ -65882,15 +65878,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1292
     1: ΤΣΟΥΤΣΙΝΟΣ,ΓΙΑΝΝΗΣ
     2: Ο ΕΝΤΙΜΟΣ ΘΑΝΑΤΟΣ ΤΗΣ ΑΜΒΡΑΚΙΑΣ
-    4: 938.21 ΤΣΟ
+    4: 938.21ΤΣΟ
     5: 2216-13251
     8: Χ.Ε
     9: ΓΙΑΝΝΙΝΑ
     10: '1967'
     11: 35Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΜΒΡΑΚΙΑ
     13: ΑΜΒΡΑΚΙΑ
@@ -65980,15 +65976,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1294
     1: ΤΩΜΑΔΑΚΗΣ,Ν.Β
     2: ΕΟΡΤΑΣΤΙΚΟΙ ΛΟΓΟΙ
-    4: 889.21 ΤΩΜ
+    4: 889.21ΤΩΜ
     5: '2529'
     8: ΓΡΗΓΟΡΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 116Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΟΡΤΑΣΤΙΚΟΙ ΛΟΓΟΙ
     13: ΕΟΡΤΑΣΤΙΚΟΙ ΛΟΓΟΙ
@@ -66080,15 +66076,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1296
     1: ΤΩΜΑΔΑΚΗΣ,ΝΙΚΟΛΑΟΣ Β.
     2: ΑΠΑΝΘΙΣΜΑΤΑ
     3: ΓΡΑΜΜΑΤΟΛΟΓΙΚΑΙ ΚΑΙ ΒΙΟΓΡΑΦΙΚΑ ΤΗΣ ΝΕΑΣ ΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑ
-    4: 886.2 ΤΩΜ
+    4: 886.2ΤΩΜ
     5: '2642'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 294Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΕΛΕΤΕΣ
     13: ΜΕΛΕΤΕΣ-ΛΟΓΟΤΕΧΝΙΑ
@@ -66210,15 +66206,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1299
   authors:
   - ΦΑΚΟΥ,ΠΑΝΤΕΛΗΣ Π.
   title: ΓΝΩΡΙΣΤΕ ΤΟ ΞΗΡΟΜΕΡΟ
-  dewey: 398 ΦΑΚ
+  dewey: 938.917 ΦΑΚ
   entry_numbers:
   - '320'
   editor: None // ΑΘΗΝΑ
   edition_year: 1978
   pages: 176
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -66226,15 +66222,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1299
     1: ΦΑΚΟΥ,ΠΑΝΤΕΛΗΣ Π.
     2: ΓΝΩΡΙΣΤΕ ΤΟ ΞΗΡΟΜΕΡΟ
-    4: 398 ΦΑΚ
+    4: 938.917ΦΑΚ
     5: '320'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 176Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΞΗΡΟΜΕΡΟ
     13: ΞΗΡΟΜΕΡΟ
@@ -66278,15 +66274,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1300
     1: ΦΑΝΑΡΙΩΤΟΥ-ΦΙΛΙΠΠΟΥ,ΑΘΗΝΑ Δ
     2: ΛΥΡΙΚΑ ΤΡΑΓΟΥΔΙΑ
-    4: 880.14 ΦΑΝ
+    4: 880.14ΦΑΝ
     5: 745-746
     8: Χ.Ε
     9: ΝΕΑ ΥΟΡΚΗ
     10: Χ.Χ
     11: 40Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -66378,15 +66374,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1302
     1: ΦΕΡΕΝΤΙΝΟΣ,ΓΕΩΡΓΙΟΣ Α.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΚΑΡΝΑΝΙΑΣ ΑΠΟ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ
     3: ΤΗΣ ΕΠΟΧΗΣ ΤΟΥ ΧΡΙΣΤΟΥ
-    4: 938.22 ΦΕΡ
+    4: 938.22ΦΕΡ
     5: 1720-1719-
     8: ΠΑΠΑΖΗΣΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 319Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΚΑΡΝΑΝΙΑ
     13: ΑΚΑΡΝΑΝΙΑ
@@ -66426,15 +66422,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1303
     1: ΦΕΡΤΑΚΗΣ,ΒΑΣΙΛΕΙΟΣ ΕΥΘ
     2: Η ΕΝ ΕΛΛΑΔΙ ΜΕΤΑΠΟΛΙΤΕΥΣΙΣ
-    4: 938.8 ΦΕΡ
+    4: 938.8ΦΕΡ
     5: '2486'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1976'
     11: 154Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΤΑΠΟΛΙΤΕΥΣΗ
     13: ΜΕΤΑΠΟΛΙΤΕΥΣΗ-ΕΛΛΑΔΑ
@@ -66584,15 +66580,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1306
     1: ΦΙΛΙΠΠΟΥ,ΕΝΤΟΥΑΡΝΤΟ ΝΤΕ
     2: ΦΙΛΟΥΜΕΝΑ ΜΑΡΤΟΥΡΑΝΟ
-    4: 852 ΦΙΛ
+    4: 852ΦΙΛ
     5: '1561'
     6: ΜΠΟΥΜΗ,ΡΙΤΑ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 106Σ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -66733,15 +66729,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1309
     1: ΦΙΣΕΡ,ΕΡΒΕΡΤΟΥ
     2: ΝΑΠΟΛΕΩΝ
-    4: 944 ΦΙΣ
+    4: 944ΦΙΣ
     5: '1267'
     6: ΣΤΑΥΡΙΝΙΔΟΣ,Δ.Θ.
     8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '1930'
     11: 173Σ
     12: ΓΑΛΛΙΚΗ ΙΣΤΟΡΙΑ-ΝΑΠΟΛΕΩΝ
@@ -66782,15 +66778,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1310
     1: ΦΛΑΜΙΝΙ,ΚΡΕΜΙΕ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΙΤΑΛΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-    4: 850 ΦΛΑ
+    4: 850ΦΛΑ
     5: '202'
     6: ΣΕΡΟΥΙΟΥ,Γ
     8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '1930'
     11: 239Σ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -66831,15 +66827,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1311
     1: FLEMING,G.DAVID
     2: JOHN CAPODISTRIAS AND THE CONFERERCE OF LONDON(1828-1831)
-    4: 938.57 FLE
+    4: 938.57FLE
     5: '1771'
     8: X.E
     9: THE/NIKI
     10: '1970'
     11: 398S
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
     13: ΚΑΠΟΔΙΣΤΡΙΑΣ-(1828-1831)
@@ -66879,15 +66875,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1312
     1: ΦΛΟΥΔΑΣ,ΝΙΚΟΛΑΟΣ Ι
     2: ΒΥΖΙΚΙΩΤΙΚΑ
-    4: 398 ΦΛΟ
+    4: 398ΦΛΟ
     5: '333'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1960'
     11: 144Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΙΚΙΩΤΙΚΑ
     13: ΒΥΖΙΚΙΩΤΙΚΑ
@@ -66930,15 +66926,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1313
     1: ΦΛΩΡΟΣ,ΠΑΥΛΟΣ
     2: ΕΛΛΗΝΙΚΟΙ ΔΡΟΜΟΙ
     3: ΤΑΞΙΔΙΑ
-    4: 914.95 ΦΛΩ
+    4: 914.95ΦΛΩ
     5: '2579'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 284Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
     13: ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
@@ -66978,15 +66974,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1314
     1: ΦΛΩΡΟΣ,ΠΑΥΛΟΣ
     2: ΣΤΑΥΡΟΔΡΟΜΙΑ ΤΗΣ ΕΥΡΩΠΗΣ
-    4: 914.4 ΦΛΩ
+    4: 914.4ΦΛΩ
     5: '394'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1964'
     11: 216Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
     13: ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
@@ -67031,15 +67027,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1315
     1: ΦΟΝΤΟΝ,ΧΟΥΑΝ
     2: Η ΧΙΛΗ ΘΑ ΝΙΚΗΣΗ
-    4: 819.7 ΦΟΝ
+    4: 819.7ΦΟΝ
     5: '1377'
     6: ΜΠΑΟΥΔΑΚΗ,ΕΛΠΙΔΑ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 75Σ
     12: ΧΙΛΙΑΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -67080,15 +67076,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1316
     1: ΦΟΥΡΙΩΤΗΣ,ΑΓΓΕΛΟΣ
     2: ΤΟ ΜΥΘΙΣΤΟΡΗΜΑ
-    4: 880.3 ΦΟΥ
+    4: 880.3ΦΟΥ
     5: '222'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1959'
     11: 368Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
@@ -67129,15 +67125,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1317
     1: FOSS,ARTHUR
     2: EPIRUS
-    4: 938.21 FOS
+    4: 938.21FOS
     5: 2181-2274
     8: FADER
     9: LONDON
     10: '1978'
     11: 223S
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
@@ -67180,15 +67176,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1318
     1: ΦΟΥΛΜΡΙΤΖ,ΤΖ
     2: Η ΑΛΑΖΟΝΕΙΑ ΤΗΣ ΔΥΝΑΜΕΩΣ
-    4: 970 ΦΟΥ
+    4: 970ΦΟΥ
     5: '2629'
     6: ΠΑΠΑΜΑΡΓΑΡΗ,Θ
     8: ΠΑΠΑΖΗΣΗ
     9: ΑΘΗΝΑ
     10: '1970'
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΥΝΑΜΕΙΣ
     13: ΑΜΕΡΙΚΗ-ΠΡΟΒΛΗΜΑΤΑ
@@ -67283,15 +67279,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1320
     1: ΦΡΑΓΚΟΠΟΥΛΟΣ,Θ.Δ
     2: ΚΑΡΤΕΡΙΑ
-    4: 886.2 ΦΡΑ
+    4: 886.2ΦΡΑ
     5: '1497'
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1957'
     11: 118Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -67336,15 +67332,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1321
     1: ΦΡΑΓΚΟΠΟΥΛΟΣ,Θ.Δ
     2: ΚΑΠΟΔΙΣΤΡΙΑΣ
     3: ΘΕΑΤΡΟ
-    4: 886.2 ΦΡΑ
+    4: 886.2ΦΡΑ
     5: '1498'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1959'
     11: 50Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -67386,15 +67382,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1322
     1: ΦΡΑΓΚΟΥ,ΚΩΝ/ΝΟΣ
     2: Η 21 ΦΕΒΡΟΥΑΡΙΟΥ 1913 ΩΣ ΜΙΑ ΤΩΝ ΕΚΒΟΛΩΝ ΤΗΣ ΑΓΩΓΗΣ ΚΑΙ
     3: ΤΟΥΗΘΟΥΣ ΤΩΝ ΠΡΟ ΑΥΤΗΣ ΕΛΛΗΝΙΚΩΝ ΓΕΝΕΩΝ
-    4: 938.68 ΦΡΑ
+    4: 938.68ΦΡΑ
     5: '2104'
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1967'
     11: 14Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1913
     13: 1913-21 ΦΕΒΡΟΥΑΡΙΟΥ
@@ -67484,15 +67480,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1324
     1: ΦΤΕΡΗΣ,Γ
     2: ΜΑΝΗ ΠΑΤΡΙΔΑ ΜΟΥ
-    4: 938.92 ΦΤΕ
+    4: 938.92ΦΤΕ
     5: '324'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1976'
     11: 178Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΝΗ
     13: ΜΑΝΗ-ΙΣΤΟΡΙΑ
@@ -67534,15 +67530,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1325
     1: ΦΤΕΡΗΣ,ΓΕΩΡΓΙΟΣ
     2: ΕΛΛΗΝΙΚΕΣ ΜΟΡΦΕΣ
-    4: 880.3 ΦΤΕ
+    4: 880.3ΦΤΕ
     5: '2652'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1979'
     11: 236Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΕΛΛΗΝΕΣ
@@ -67587,15 +67583,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1326
     1: ΦΩΤΙΑΔΟΥ,ΑΘΑΝΑΣΙΟΣ(ΛΟΓΙΟΣ)
     2: ΚΑΡΑΓΚΙΟΖΗΣ Ο ΠΡΟΣΦΥΓΑΣ
     3: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ ΣΚΙΩΝ
-    4: 886.2 ΦΩΤ
+    4: 886.2ΦΩΤ
     5: '1535'
     8: GYTENBERG
     9: ΑΘΗΝΑ
     10: '1977'
     11: 522Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΑΡΑΓΚΙΟΖΗΣ
@@ -67634,15 +67630,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1327
     1: ΦΩΤΙΑΔΟΥ,Φ.Δ
     2: ΠΑΡΙΣΙΟΙ
-    4: 914.44 ΦΩΤ
+    4: 914.44ΦΩΤ
     5: '402'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 147Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΠΑΡΙΣΙ
     13: ΤΑΞΙΔΙΑ-ΠΑΡΙΣΙ
@@ -67735,15 +67731,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1329
     1: ΦΩΤΙΑΔΟΥ,ΕΡΜΗΝΕΙΑ
     2: ΞΕΝΟΙ ΤΟΠΟΙ
-    4: 910 ΦΩΤ
+    4: 910ΦΩΤ
     5: '2603'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1972'
     11: 99Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΞΕΝΟΙ ΤΟΠΟΙ
     13: ΙΣΠΑΝΙΑ-ΤΑΞΙΔΙΑ
@@ -67791,15 +67787,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1330
     1: ΦΩΤΙΑΔΗΣ,ΕΥΑΓΓΕΛΟΣ Π.
     2: ΣΠΥΡΙΔΩΝ ΛΑΜΠΡΟΣ
     3: ΜΝΗΜΟΣΥΝΟΣ ΛΟΓΟΣ
-    4: 938 ΦΩΤ
+    4: 938ΦΩΤ
     5: 2023-2733-9254Α
     7: 2ΕΚΔ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 35Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
@@ -67887,15 +67883,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1332
     1: ΦΩΤΟΠΟΥΛΟΣ,Κ.Ι
     2: ΧΡΟΝΙΚΟ ΤΟΥ ΜΕΓΑΛΟΥ ΣΗΚΩΜΟΥ ΤΟΥ ΓΕΝΟΥΣ
-    4: 938.5 ΦΩΤ
+    4: 938.5ΦΩΤ
     5: '2142'
     8: Χ.Ε
     9: ΓΙΑΝΝΙΝΑ
     10: Χ.Χ
     11: 254Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΧΡΟΝΙΚΟ
     13: ΧΡΟΝΙΚΟ-ΞΕΣΗΚΩΜΟΣ
@@ -67935,15 +67931,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1333
     1: ΦΩΤΟΠΟΥΛΟΣ,ΑΘΑΝΑΣΙΟΣ Θ.
     2: ΙΣΤΟΡΙΚΑ ΤΩΝ ΠΕΤΙΜΕΖΑΙΩΝ
-    4: 938.5 ΦΩΤ
+    4: 938.5ΦΩΤ
     5: '2128'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1982'
     11: 105Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΕΤΙΜΕΖΑΙΟΙ
     13: ΠΕΤΙΜΕΖΑΙΟΙ
@@ -68093,15 +68089,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1336
     1: ΧΑΜΜΕΡ,Ι
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΟΘΩΜΑΝΙΚΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
-    4: 956.1 ΧΑΜ
+    4: 956.1ΧΑΜ
     5: 2302-2303-2304-2305-
     6: ΚΡ0ΚΙΔΑΣ,Κ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1870'
     11: 385Σ
     12: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-ΙΣΤΟΡΙΑ
@@ -68194,15 +68190,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1338
     1: ΧΑΜΟΝΤ,Ν
     2: ΗΠΕΙΡΟΣ
-    4: 938.21 ΧΑΜ
+    4: 938.21ΧΑΜ
     5: 2269-2270-2271-
     6: ΓΙΑΓΚΑΣ,ΑΘ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1971'
     11: 214Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
@@ -68247,15 +68243,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1339
     1: ΧΑΝΤΚΕ,ΠΕΤΕΡ
     2: ΚΑΣΠΑΡ
-    4: 832 ΧΑΝ
+    4: 832ΧΑΝ
     5: '1373'
     6: ΑΙΝΤΕΝΑΙΕΡ,ΝΙΚΗ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 111Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -68353,15 +68349,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1341
     1: ΧΑΡΗΣ,ΠΕΤΡΟΣ
     2: Η ΚΙΝΑ ΕΞΩ ΑΠΟ ΤΑ ΤΕΙΧΗ
-    4: 915.31 ΧΑΡ
+    4: 915.31ΧΑΡ
     5: 451-455-450
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1963'
     11: 246Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΙΝΑ
     13: ΤΑΞΙΔΙΑ-ΚΙΝΑ
@@ -68401,15 +68397,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1342
     1: ΧΑΡΗΣ,ΠΕΤΡΟΣ
     2: Η ΠΝΕΥΜΑΤΙΚΗ ΕΛΕΥΘΕΡΙΑ ΚΑΙ ΟΙ ΜΕΤΑΠΟΛΕΜΙΚΟΙ ΑΝΘΡΩΠΟΙ
-    4: 880.4 ΧΑΡ
+    4: 880.4ΧΑΡ
     5: '1003'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 243Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΣΥΓΓΡΑΦΕΙΣ-ΛΟΓΟΤΕΧΝΕΣ
@@ -68453,15 +68449,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1343
     1: ΧΑΤΖΗΣ,ΘΑΝΑΣΗΣ
     2: Η ΝΙΚΗΦΟΡΑ ΕΠΑΝΑΣΤΑΣΗ ΠΟΥ ΧΑΘΗΚΕ
-    4: 938.75 ΧΑΤ
+    4: 938.75ΧΑΤ
     5: 2290-2291-2292-
     8: ΠΑΠΑΖΗΣΗ
     9: ΑΘΗΝΑ
     10: '1977'
     11: 473Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
     13: 1940-ΕΠΑΝΑΣΤΑΣΗ
@@ -68606,15 +68602,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1346
     1: ΧΑΤΖΗΙΩΑΝΝΟΥ,ΓΙΑΝΝΗΣ
     2: ΠΕΖΟΓΡΑΦΗΜΑΤΑ (1989-1990)
     3: ΠΟΙΗΤΙΚΑ ΘΕΜΑΤΑ Β'(ΜΕΛΕΤΗΜΑ)
-    4: 880.3 ΧΑΤ
+    4: 880.3ΧΑΤ
     5: '1667'
     8: Χ.Ε
     9: ΘΕΣ/ΝΙΚΗ
     10: '1990'
     11: 137Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΠΕΖΟΓΡΑΦΗΜΑΤΑ
@@ -68959,15 +68955,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1353
     1: ΧΕΜΠΕΛ,ΦΡΕΙΔΕΡΙΚΗ
     2: ΙΟΥΔΗΘ
     3: ΤΡΑΓΩΔΙΑ
-    4: 832 ΧΕΜ
+    4: 832ΧΕΜ
     5: '1375'
     6: ΔΙΚΤΑΙΟΣ,ΑΡΗΣ
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 142Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -69005,36 +69001,37 @@
   - ΚΑΡΟΛΙΔΟΣ,Π.
   editor: ΣΑΚΕΛΛΑΡΙΟΥ // ΑΘΗΝΑ
   edition_year: 1906
   pages: 634
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΑΡΧΑΙΑ
+  - ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   copies: 2
   notes: '1752'
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1354
     1: ΧΕΡΤΣΒΕΡΓ,ΓΟΥΣΤΑΒΟΥ ΦΡΕΙΔΕΡΙΚΟΥ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΑΔΟΣ ΑΠΟ ΤΗΣ ΛΗΞΕΩΣ ΤΟΥ ΑΡΧΑΙΟΥ ΒΙΟΥ ΜΕΧΡΙ
     3: ΣΗΜΕΡΟΝ
-    4: 938 ΧΕΡ
+    4: 938ΧΕΡ
     5: 1752-1753-1855-2175-
     6: ΚΑΡΟΛΙΔΟΣ,Π
     8: ΣΑΚΕΛΛΑΡΙΟΥ
     9: ΑΘΗΝΑ
     10: '1906'
     11: 634Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
+    13: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
+    14: ΙΣΤΟΡΙΑ
     17: (1752-2 ΑΝΤΙΤΥΠΑ)
     7: null
-    13: null
-    14: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -69550,15 +69547,14 @@
     27: null
     28: null
     29: null
 - dbase_number: 1365
   authors:
   - ΧΟΦΜΑΝ,ΦΡΕΝΤ
   title: ΤΟ ΣΥΓΧΡΟΝΟ ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ(1900-1950)
-  dewey: 880.3 XOF
   entry_numbers:
   - '2655'
   editor: ΑΕΤΟΣ // ΑΘΗΝΑ
   edition_year: 1954
   pages: 167
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -69568,15 +69564,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1365
     1: ΧΟΦΜΑΝ,ΦΡΕΝΤ
     2: ΤΟ ΣΥΓΧΡΟΝΟ ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ(1900-1950)
-    4: 880.3XOF
+    4: 880.ΧΟΦ
     5: '2655'
     8: ΑΕΤΟΣ
     9: ΑΘΗΝΑ
     10: '1954'
     11: 167Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
@@ -69619,15 +69615,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1366
     1: ΧΟΥΡΜΟΥΖΙΑΔΗΣ,Γ.Δ.
     2: ΑΝΘΟΛΟΓΙΑ ΤΟΝ ΑΡΓΕΝΤΙΝΟΥ ΔΙΗΓΗΜΑΤΟΣ
-    4: 810 ΧΟΥ
+    4: 810ΧΟΥ
     5: '2640'
     8: ΒΑΚΩΝ
     9: ΑΘΗΝΑ
     10: '1967'
     11: 175Σ
     12: ΑΡΓΕΝΤΙΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΑΡΓΕΝΤΙΝΟ ΔΙΗΓΗΜΑ-ΑΝΘΟΛΟΓΙΑ
@@ -69670,15 +69666,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1367
     1: ΧΟΥΡΜΟΥΖΙΑΔΗΣ,Γ.Δ.
     2: EΠΟΠΤΕΙΕΣ
     3: ΒΙΩΜΑΤΑ ΚΑΙ ΔΟΚΙΜΙΑ
-    4: 880.4 ΧΟΥ
+    4: 880.4ΧΟΥ
     5: '2719'
     8: ΣΙΔΕΡΗΣ
     9: ΑΘΗΝΑ
     10: '1972'
     11: 174Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΟΚΙΜΙΑ
     13: ΔΟΚΙΜΙΑ-ΛΟΓΟΤΕΧΝΙΑ
@@ -69771,15 +69767,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1369
     1: ΧΟΦΜΑΝ,ΠΩΛ
     2: ΗΝΩΜΕΝΕΣ ΠΟΛΙΤΕΙΕΣ
     3: Η ΑΕΝΑΗ ΕΠΑΝΑΣΤΑΣΙΣ
-    4: 973 ΧΟΦ
+    4: 973ΧΟΦ
     5: '435'
     8: Χ.Ε
     9: ΝΕΑ ΥΟΡΚΗ
     10: '1951'
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΝΩΜΕΝΕΣ ΠΟΛΙΤΕΙΕΣ
     13: ΗΝΩΜΕΝΕΣ ΠΟΛΙΤΕΙΕΣ-ΙΣΤΟΡΙΑ
     14: ΑΕΝΑΗ-ΕΠΑΝΑΣΤΑΣΗ
@@ -69823,15 +69819,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1370
     1: ΧΟΧΟΥΤ,ΡΟΛΦ
     2: ΣΤΡΑΤΙΩΤΕΣ
     3: ΤΡΑΓΩΔΙΑ
-    4: 832 ΧΟΧ
+    4: 832ΧΟΧ
     5: '1367'
     8: ΔΩΔΩΝΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 222Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
@@ -69974,15 +69970,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1373
     1: ΨΑΘΑΣ,ΔΗΜΗΤΡΙΟΣ
     2: Ο ΦΟΝ ΔΗΜΗΤΡΑΚΗΣ
     3: ΚΩΜΩΔΙΑ
-    4: 880.2 ΨΑΘ
+    4: 880.2ΨΑΘ
     5: '1399'
     8: ΜΑΡΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 111Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
@@ -70023,15 +70019,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1374
     1: ΨΑΘΑΣ,Δ
     2: ΤΟ ΣΤΡΑΒΟΞΥΛΟ
-    4: 886.2 ΨΑΘ
+    4: 886.2ΨΑΘ
     5: '1574'
     8: ΜΑΡΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 132Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
@@ -70125,15 +70121,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1376
     1: ΓΟΥΕΛ,ΤΖΟΝ
     2: ΡΟΣΑΜΠΩ ΚΑΙ Ο ΠΟΛΕΜΟΣ ΤΗΣ ΒΟΡΕΙΟΑΜΕΡΙΚΑΝΙΚΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ
     3: 1725-1807
-    4: 970 ΓΟΥ
+    4: 970ΓΟΥ
     5: '2523'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1936'
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΕΞΑΡΤΗΣΙΑ
     13: ΡΟΣΑΜΠΩ-ΑΜΕΡΙΚΗ
     14: ΑΜΕΡΙΚΗ-ΒΟΡΕΙΟΑΜΕΡΙΚΑΝΙΚΗ ΑΝΕΞΑΡΤΗΣΙΑ
@@ -70224,15 +70220,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1378
     1: ΓΟΥΝΤΑΡ,ΒΑΝ
     2: ΣΥΓΚΡΙΤΙΚΑ ΔΟΚΙΜΙΑ ΓΥΡΩ ΑΠΟ ΤΗΝ ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ
-    4: 970 ΓΟΥ
+    4: 970ΓΟΥ
     5: '427'
     6: ΤΑΧΤΣΗΣ,Κ
     8: ΠΑΛΤΕΖΑΝΑΚΗ
     9: ΑΘΗΝΑ
     10: '1969'
     11: 518Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΟΚΙΜΙΑ
@@ -70327,15 +70323,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1380
     1: Χ.Σ
     2: ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ
     3: ΑΡΧΑΙΟΤΗΤΕΣ ΚΑΙ ΜΝΗΜΕΙΑ ΑΙΤΩΛΟΚΑΡΝΑΝΙΑΣ
-    4: 938.22 ΑΙΤ
+    4: 938.22ΑΙΤ
     5: '321'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 15Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ
     13: ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ-ΜΝΗΜΕΙΑ
@@ -70373,15 +70369,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1381
     1: Χ.Σ
     2: ΑΠΕΙΛΗ ΝΕΟΥ ΑΚΡΩΤΗΡΙΑΣΜΟΥ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ
-    4: 938.7 ΑΠΕ
+    4: 938.7ΑΠΕ
     5: '1975'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 125Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΠΕΙΛΗ ΑΚΡΩΤΗΡΙΑΣΜΟΥ
     13: ΑΠΕΙΛΗ ΑΚΡΩΤΗΡΙΑΣΜΟΥ
@@ -70404,15 +70400,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1382
   authors: []
   title: ΑΠΟΚΑΛΥΠΤΗΡΙΑ ΠΡΟΤΟΜΗΣ ΑΡΧΙΣΤΑΤΗΓΟΥ ΓΕΩΡΓΙΟΥ ΚΑΡΑΙΣΚΑΚΗ
-  dewey: 938.566 ΑΠΟ
+  dewey: 938.566 ΧΣ
   entry_numbers:
   - '1878'
   editor: None // ΑΡΤΑ
   edition_year: 1965
   pages: 44
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -70420,15 +70416,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1382
     1: Χ.Σ
     2: ΑΠΟΚΑΛΥΠΤΗΡΙΑ ΠΡΟΤΟΜΗΣ ΑΡΧΙΣΤΑΤΗΓΟΥ ΓΕΩΡΓΙΟΥ ΚΑΡΑΙΣΚΑΚΗ
-    4: 938.566ΑΠΟ
+    4: 938.566Χ.Σ
     5: '1878'
     8: Χ.Ε
     9: ΑΡΤΑ
     10: '1965'
     11: 44Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ
     13: ΚΑΡΑΙΣΚΑΚΗΣ
@@ -70452,15 +70448,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1383
   authors: []
   title: ΑΡΤΑ
   subtitle: ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
-  dewey: 938.939 ΑΡΤ
+  dewey: 938.939 ΧΣ
   entry_numbers:
   - '305'
   pages: 19
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΑΡΤΑ
   - ΜΝΗΜΕΙΑ
@@ -70468,15 +70464,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1383
     1: Χ.Σ
     2: ΑΡΤΑ
     3: ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
-    4: 938.939ΑΡΤ
+    4: 938.939Χ.Σ
     5: '305'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 19Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
     13: ΑΡΤΑ-ΜΝΗΜΕΙΑ
@@ -70547,15 +70543,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1385
   authors: []
   title: ΑΡΧΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΠΑΛΙΓΓΕΝΕΣΙΑΣ ΜΕΧΡΙ ΤΗΣ ΕΓΚΑΤΑΣΤΑΣΕΩΣ
   subtitle: ΤΗΣ ΒΑΣΙΛΕΙΑΣ
-  dewey: 938.501 ΑΡΧ
+  dewey: 938.501 ΧΣ
   entry_numbers:
   - '1907'
   - '1908'
   editor: None // ΑΘΗΝΑ
   edition_year: 1971
   pages: 572
   topics:
@@ -70568,15 +70564,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1385
     1: Χ.Σ
     2: ΑΡΧΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΠΑΛΙΓΓΕΝΕΣΙΑΣ ΜΕΧΡΙ ΤΗΣ ΕΓΚΑΤΑΣΤΑΣΕΩΣ
     3: ΤΗΣ ΒΑΣΙΛΕΙΑΣ
-    4: 938.501ΑΡΧ
+    4: 938.501Χ.Σ
     5: 1907-1908
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1971'
     11: 572Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΕΙΑ
     13: ΑΡΧΕΙΑ-ΠΑΛΙΓΓΕΝΕΣΙΑ
@@ -70749,15 +70745,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1389
   authors: []
   title: ΕΙΚΟΝΟΓΡΑΦΙΑ ΤΟΥ 21
-  dewey: 938.5 ΕΙΚ
+  dewey: 938.5 ΧΣ
   entry_numbers:
   - '2565'
   editor: None // ΑΘΗΝΑ
   edition_year: 1971
   pages: 86
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -70767,15 +70763,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1389
     1: Χ.Σ
     2: ΕΙΚΟΝΟΓΡΑΦΙΑ ΤΟΥ 21
-    4: 938.5 ΕΙΚ
+    4: 938.5Χ.Σ
     5: '2565'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1971'
     11: 86Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821-ΕΙΚΟΝΟΓΡΑΦΙΑ
     13: 1821-ΕΙΚΟΝΟΓΡΑΦΙΑ
@@ -70799,15 +70795,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1390
   authors: []
   title: ΤΟ ΕΙΚΟΣΙΕΝΑ
   subtitle: ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ
-  dewey: 938.5 ΕΙΚ
+  dewey: 938.5 ΧΣ
   entry_numbers:
   - '1883'
   editor: None // ΑΘΗΝΑ
   edition_year: 1977
   pages: 1024
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -70818,15 +70814,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1390
     1: Χ.Σ
     2: ΤΟ ΕΙΚΟΣΙΕΝΑ
     3: ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ
-    4: 938.5 ΕΙΚ
+    4: 938.5Χ.Σ
     5: '1883'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 1024Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821
     13: 1821-ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ
@@ -70849,15 +70845,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1391
   authors: []
   title: 28 ΟΚΤΩΒΡΙΟΥ 1940
   subtitle: Η ΕΛΛΑΔΑ ΣΤΟ ΧΑΡΑΚΩΜΑ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
-  dewey: 938.752 ΟΚΤ
+  dewey: 938.752 ΧΣ
   entry_numbers:
   - '2539'
   editor: ΕΥΘΥΝΗ // ΑΘΗΝΑ
   edition_year: 1980
   pages: 259
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -70867,15 +70863,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1391
     1: Χ.Σ
     2: 28 ΟΚΤΩΒΡΙΟΥ 1940
     3: Η ΕΛΛΑΔΑ ΣΤΟ ΧΑΡΑΚΩΜΑ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
-    4: 938.752ΟΚΤ
+    4: 938.752Χ.Σ
     5: '2539'
     8: ΕΥΘΥΝΗ
     9: ΑΘΗΝΑ
     10: '1980'
     11: 259Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
     13: 1940-28 ΟΚΤΩΒΡΙΟΥ
@@ -70916,15 +70912,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1392
     1: Χ.Σ
     2: ΕΙΣ ΜΝΗΜΗΝ Κ. ΑΜΑΝΤΟΥ(1874-1960)
-    4: 938.64 ΜΝΗ
+    4: 938.64ΜΝΗ
     5: 1881-2341
     8: ΜΥΡΤΙΔΗ
     9: ΑΘΗΝΑ
     10: '1960'
     11: 531Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΑΜΑΝΤΟΣ-ΜΝΗΜΗ
@@ -70948,15 +70944,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1393
   authors: []
   title: Η ΕΚΣΤΡΑΤΕΙΑ ΕΙΣ ΤΗΝ ΜΙΚΡΑΝ ΑΣΙΑΝ(1919-1922)
   subtitle: ΕΠΙΘΕΤΙΚΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ ΔΕΚΕΜΒΡΙΟΥ 1920 ΜΑΡΤΙΟΥ 1921
-  dewey: 938.721 ΕΚΣ
+  dewey: 938.721 ΧΣ
   entry_numbers:
   - '1793'
   - '1873'
   - '8192'
   editor: ΓΕΝ.ΕΠΙΤ.ΣΤΡΑΤΟΥ // ΑΘΗΝΑ
   edition_year: 1963
   topics:
@@ -70970,15 +70966,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1393
     1: Χ.Σ
     2: Η ΕΚΣΤΡΑΤΕΙΑ ΕΙΣ ΤΗΝ ΜΙΚΡΑΝ ΑΣΙΑΝ(1919-1922)
     3: ΕΠΙΘΕΤΙΚΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ ΔΕΚΕΜΒΡΙΟΥ 1920 ΜΑΡΤΙΟΥ 1921
-    4: 938.721ΕΚΣ
+    4: 938.721Χ.Σ
     5: 1793-1873-8192
     8: ΓΕΝ.ΕΠΙΤ.ΣΤΡΑΤΟΥ
     9: ΑΘΗΝΑ
     10: '1963'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
     13: ΜΙΚΡΑ ΑΣΙΑ-ΕΚΣΤΡΑΤΕΙΑ
     14: 1919-ΜΙΚΡΑ ΑΣΙΑ
@@ -71071,15 +71067,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1395
     1: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
     2: ΕΛΛΑΣ
-    4: 938 ΕΛΛ
+    4: 938ΕΛΛ
     5: 362-363-364-
     8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '1926'
     11: 156Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
     13: ΕΛΛΑΣ
@@ -71199,15 +71195,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1398
   authors: []
   title: ΕΛΛΗΝΙΚΑ ΔΙΠΛΩΜΑΤΙΚΑ ΕΓΓΡΑΦΑ 1940-41
-  dewey: 938.75 ΕΛΛ
+  dewey: 938.75 ΧΣ
   entry_numbers:
   - '2393'
   editor: None // ΑΘΗΝΑ
   edition_year: 1980
   pages: 244
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71218,15 +71214,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1398
     1: Χ.Σ
     2: ΕΛΛΗΝΙΚΑ ΔΙΠΛΩΜΑΤΙΚΑ ΕΓΓΡΑΦΑ 1940-41
-    4: 938.75ΕΛΛ
+    4: 938.75Χ.Σ
     5: '2393'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1980'
     11: 244Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΓΓΡΑΦΑ
     13: ΕΓΓΡΑΦΑ-ΔΙΠΛΩΜΑΤΙΚΑ
@@ -71250,15 +71246,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1399
   authors: []
   title: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ 1940-1941
   subtitle: Η ΙΤΑΛΙΚΗ ΕΙΣΒΟΛΗ
-  dewey: 938.752 ΕΛΛ
+  dewey: 938.752 ΧΣ
   entry_numbers:
   - '2136'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
   pages: 342
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71270,15 +71266,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1399
     1: Χ.Σ
     2: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ 1940-1941
     3: Η ΙΤΑΛΙΚΗ ΕΙΣΒΟΛΗ
-    4: 938.752ΕΛΛ
+    4: 938.752Χ.Σ
     5: '2136'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1960'
     11: 342Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
     13: ΠΟΛΕΜΟΣ-ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ
@@ -71301,15 +71297,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1400
   authors: []
   title: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ 1940-1941
   subtitle: ΧΕΙΜΕΡΙΝΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ-ΙΤΑΛΙΚΗ ΕΠΙΘΕΣΕΙΣ ΜΑΡΤΙΟΥ
-  dewey: 938.752 ΕΛΛ
+  dewey: 938.752 ΧΣ
   entry_numbers:
   - '2135'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
   pages: 250
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71321,15 +71317,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1400
     1: Χ.Σ
     2: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ 1940-1941
     3: ΧΕΙΜΕΡΙΝΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ-ΙΤΑΛΙΚΗ ΕΠΙΘΕΣΕΙΣ ΜΑΡΤΙΟΥ
-    4: 938.752ΕΛΛ
+    4: 938.752Χ.Σ
     5: '2135'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1966'
     11: 250Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
     13: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ
@@ -71351,15 +71347,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1401
   authors: []
   title: Η ΕΛΛΗΝΙΚΗ ΑΝΤΕΠΙΘΕΣΙΣ 1940-1941
-  dewey: 938.75 ΕΛΛ
+  dewey: 938.75 ΧΣ
   entry_numbers:
   - '2137'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - '1940'
@@ -71368,15 +71364,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1401
     1: Χ.Σ
     2: Η ΕΛΛΗΝΙΚΗ ΑΝΤΕΠΙΘΕΣΙΣ 1940-1941
-    4: 938.75ΕΛΛ
+    4: 938.75Χ.Σ
     5: '2137'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1966'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
     13: 1940-ΑΝΤΕΠΙΘΕΣΗ
     14: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
@@ -71399,15 +71395,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1402
   authors: []
   title: ΤΟ ΕΛΛΗΝΙΚΟΝ ΕΚΣΤΡΑΤΕΥΤΙΚΟΝ ΣΩΜΑ ΕΙΣ ΜΕΣΗΜΒΡΙΝΗΝ ΡΩΣΙΑΝ 1919
-  dewey: 938.72 ΕΛΛ
+  dewey: 938.72 ΧΣ
   entry_numbers:
   - '1877'
   editor: None // ΑΘΗΝΑ
   edition_year: 1955
   pages: 446
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71417,15 +71413,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1402
     1: Χ.Σ
     2: ΤΟ ΕΛΛΗΝΙΚΟΝ ΕΚΣΤΡΑΤΕΥΤΙΚΟΝ ΣΩΜΑ ΕΙΣ ΜΕΣΗΜΒΡΙΝΗΝ ΡΩΣΙΑΝ 1919
-    4: 938.72ΕΛΛ
+    4: 938.72Χ.Σ
     5: '1877'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1955'
     11: 446Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΣΙΑ
     13: ΡΩΣΙΑ-1919
@@ -71449,15 +71445,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1403
   authors: []
   title: Ο ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΠΡΩΤΟΝ ΠΑΓΚΟΣΜΙΟΝ ΠΟΛΕΜΟΝ
   subtitle: 1914-1918
-  dewey: 938.721 ΕΛΛ
+  dewey: 938.721 ΧΣ
   entry_numbers:
   - '1874'
   - '1875'
   editor: None // ΑΘΗΝΑ
   edition_year: 1958
   pages: 374
   topics:
@@ -71469,15 +71465,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1403
     1: Χ.Σ
     2: Ο ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΠΡΩΤΟΝ ΠΑΓΚΟΣΜΙΟΝ ΠΟΛΕΜΟΝ
     3: 1914-1918
-    4: 938.721ΕΛΛ
+    4: 938.721Χ.Σ
     5: 1874-1875-
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1958'
     11: 374Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
     13: ΠΟΛΕΜΟΣ-Α'ΠΑΓΚΟΣΜΙΟΣ
@@ -71500,15 +71496,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1404
   authors: []
   title: Ο ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΔΕΥΤΕΡΟ ΠΑΓΚΟΣΜΙΟ ΠΟΛΕΜΟΝ
   subtitle: ΑΙΤΙΑ ΚΑΙ ΑΦΟΡΜΑΙ ΕΛΛΗΝΟ-ΙΤΑΛΙΚΟΥ ΠΟΛΕΜΟΥ (1940-1941)
-  dewey: 938.75 ΕΛΛ
+  dewey: 938.75 ΧΣ
   entry_numbers:
   - '1876'
   editor: None // ΑΘΗΝΑ
   edition_year: 1959
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΠΟΛΕΜΟΣ
@@ -71518,15 +71514,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1404
     1: Χ.Σ
     2: Ο ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΔΕΥΤΕΡΟ ΠΑΓΚΟΣΜΙΟ ΠΟΛΕΜΟΝ
     3: ΑΙΤΙΑ ΚΑΙ ΑΦΟΡΜΑΙ ΕΛΛΗΝΟ-ΙΤΑΛΙΚΟΥ ΠΟΛΕΜΟΥ (1940-1941)
-    4: 938.75 ΕΛΛ
+    4: 938.75Χ.Σ
     5: '1876'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1959'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
     13: ΠΟΛΕΜΟΣ-Β'ΠΑΓΚΟΣΜΙΟΣ
     14: Β'ΠΑΓΚΟΣΜΙΟΣ ΠΟΛΕΜΟΣ
@@ -71548,15 +71544,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1405
   authors: []
   title: ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΑΝΤΙΣΥΜΜΟΡΙΑΚΟΥ ΑΓΩΝΑ (1946-1949)
-  dewey: 938.774 ΕΛΛ
+  dewey: 938.774 ΧΣ
   entry_numbers:
   - '2238'
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
   pages: 469
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71566,15 +71562,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1405
     1: Χ.Σ
     2: ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΑΝΤΙΣΥΜΜΟΡΙΑΚΟΥ ΑΓΩΝΑ (1946-1949)
-    4: 938.774ΕΛΛ
+    4: 938.774Χ.Σ
     5: '2238'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 469Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ
     13: ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ
@@ -71647,30 +71643,30 @@
     28: null
     29: null
     30: null
 - dbase_number: 1407
   authors: []
   title: Η ΕΞΕΛΙΞΙΣ ΤΟΥ ΚΥΠΡΙΑΚΟΥ ΚΑΙ ΟΙ ΘΕΣΕΙΣ ΤΗΣ ΝΕΑΣ ΔΗΜΟΚΡΑΤΙΚΗΣ
   subtitle: ΚΙΝΗΣΕΩΣ
-  dewey: 938.497 ΕΞΕ
+  dewey: 938.497 ΧΣ
   entry_numbers:
   - '2233'
   editor: None // ΑΘΗΝΑ
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΚΥΠΡΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1407
     1: Χ.Σ
     2: Η ΕΞΕΛΙΞΙΣ ΤΟΥ ΚΥΠΡΙΑΚΟΥ ΚΑΙ ΟΙ ΘΕΣΕΙΣ ΤΗΣ ΝΕΑΣ ΔΗΜΟΚΡΑΤΙΚΗΣ
     3: ΚΙΝΗΣΕΩΣ
-    4: 938.497ΕΞΕ
+    4: 938.497Χ.Σ
     5: '2233'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
     13: ΚΥΠΡΟΣ
     6: null
@@ -71693,33 +71689,33 @@
     28: null
     29: null
     30: null
 - dbase_number: 1408
   authors: []
   title: Ο ΕΟΡΤΑΣΜΟΣ ΤΗΣ 100ΕΤΗΡΙΔΟΣ
   subtitle: ΑΝΤΩΝΙΟΥ Δ.ΚΕΡΑΜΟΠΟΥΛΛΟΥ
-  dewey: 938 ΕΟΡ
+  dewey: 938 ΧΣ
   entry_numbers:
   - '2348'
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
   pages: 33
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΠΡΟΣΩΠΑ
   - ΚΕΡΑΜΟΠΟΥΛΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1408
-    1: Χ.Ε
+    1: Χ.Σ
     2: Ο ΕΟΡΤΑΣΜΟΣ ΤΗΣ 100ΕΤΗΡΙΔΟΣ
     3: ΑΝΤΩΝΙΟΥ Δ.ΚΕΡΑΜΟΠΟΥΛΛΟΥ
-    4: 938 ΕΟΡ
+    4: 938Χ.Σ
     5: '2348'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 33Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΚΕΡΑΜΟΠΟΥΛΟΣ-ΙΣΤΟΡΙΑ
@@ -71742,15 +71738,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1409
   authors: []
   title: Ο ΕΟΡΤΑΣΜΟΣ ΤΗΣ 100ΕΤΗΡΙΔΟΣ ΤΟΥ ΗΡΩΟΣ ΤΟΥ ΜΑΚΕΔΟΝΙΚΟΥ ΑΓΩΝΟΣ
   subtitle: ΠΑΥΛΟΥ ΜΕΛΑ
-  dewey: 938.667 ΕΟΡ
+  dewey: 938.667 ΧΣ
   entry_numbers:
   - '2347'
   editor: None // ΑΘΗΝΑ
   edition_year: 1972
   pages: 29
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71761,15 +71757,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1409
     1: Χ.Σ
     2: Ο ΕΟΡΤΑΣΜΟΣ ΤΗΣ 100ΕΤΗΡΙΔΟΣ ΤΟΥ ΗΡΩΟΣ ΤΟΥ ΜΑΚΕΔΟΝΙΚΟΥ ΑΓΩΝΟΣ
     3: ΠΑΥΛΟΥ ΜΕΛΑ
-    4: 938.667ΕΟΡ
+    4: 938.667Χ.Σ
     5: '2347'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1972'
     11: 29Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΑ-ΠΑΥΛΟΣ ΜΕΛΑΣ
@@ -71791,15 +71787,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1410
   authors: []
   title: ΕΠΙΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΕΙΣ ΜΙΚΡΑΝ ΑΣΙΑΝ ΕΚΣΤΡΑΤΕΙΑΣ (1919-1922
-  dewey: 938.72 ΕΠΙ
+  dewey: 938.72 ΧΣ
   entry_numbers:
   - '1793'
   - '8192'
   editor: None // ΑΘΗΝΑ
   edition_year: 1967
   pages: 495
   topics:
@@ -71810,15 +71806,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1410
     1: Χ.Σ
     2: ΕΠΙΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΕΙΣ ΜΙΚΡΑΝ ΑΣΙΑΝ ΕΚΣΤΡΑΤΕΙΑΣ (1919-1922
-    4: 938.72 ΕΠΙ
+    4: 938.72Χ.Σ
     5: 1793-8192
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 495Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
     13: ΜΙΚΡΑ ΑΣΙΑ-1919
@@ -71841,15 +71837,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1411
   authors: []
   title: ΕΠΙΧΕΙΡΗΣΕΙΣ ΕΙΣ ΘΡΑΚΗΝ(1919-1923)
-  dewey: 938.695 ΕΠΙ
+  dewey: 938.695 ΧΣ
   entry_numbers:
   - '2132'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
   pages: 221
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71860,15 +71856,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1411
     1: Χ.Σ
     2: ΕΠΙΧΕΙΡΗΣΕΙΣ ΕΙΣ ΘΡΑΚΗΝ(1919-1923)
-    4: 938.695ΕΠΙ
+    4: 938.695Χ.Σ
     5: '2132'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1969'
     11: 221Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
     13: ΘΡΑΚΗ-ΕΠΙΧΕΙΡΗΣΕΙΣ
@@ -71892,15 +71888,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1412
   authors: []
   title: Η ΕΥΡΩΠΑΙΚΗ ΟΛΟΚΛΗΡΩΣΗ
   subtitle: Η ΕΛΛΑΔΑ ΜΕΤΑ ΤΟ ΜΑΑΣΤΡΙΧΤ
-  dewey: 938.87 ΕΥΡ
+  dewey: 938.87 ΧΣ
   entry_numbers:
   - '2561'
   editor: None // ΑΘΗΝΑ
   edition_year: 1992
   pages: 377
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71911,15 +71907,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1412
     1: Χ.Σ
     2: Η ΕΥΡΩΠΑΙΚΗ ΟΛΟΚΛΗΡΩΣΗ
     3: Η ΕΛΛΑΔΑ ΜΕΤΑ ΤΟ ΜΑΑΣΤΡΙΧΤ
-    4: 938.87 ΕΥΡ
+    4: 938.87Χ.Σ
     5: '2561'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1992'
     11: 377Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
     13: ΕΥΡΩΠΗ-ΜΑΑΣΤΡΙΧΤ
@@ -71942,15 +71938,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1413
   authors: []
   title: ΗΠΕΙΡΟΣ
   subtitle: ΙΣΤΟΡΙΑ,ΓΕΩΓΡΑΦΙΑ,ΓΛΩΣΣΑ Κ.Λ.Π
-  dewey: 938.93 ΗΠΕ
+  dewey: 938.93 ΧΣ
   entry_numbers:
   - '2094'
   editor: ΗΠΕΙΡΩΤΙΚΗ ΕΣΤΙΑ // ΙΩΑΝΝΙΝΑ
   edition_year: 1952
   pages: 162
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -71959,15 +71955,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1413
     1: Χ.Σ
     2: ΗΠΕΙΡΟΣ
     3: ΙΣΤΟΡΙΑ,ΓΕΩΓΡΑΦΙΑ,ΓΛΩΣΣΑ Κ.Λ.Π
-    4: 938.93 ΗΠΕ
+    4: 938.93Χ.Σ
     5: '2094'
     8: ΗΠΕΙΡΩΤΙΚΗ ΕΣΤΙΑ
     9: ΙΩΑΝΝΙΝΑ
     10: '1952'
     11: 162Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
@@ -71990,15 +71986,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1414
   authors: []
   title: ΗΠΕΙΡΟΣ
   subtitle: Η ΕΤΑΙΡΕΙΑ ΗΠΕΙΡΩΤΙΚΩΝ ΜΕΛΕΤΩΝ
-  dewey: 938.93 ΗΠΕ
+  dewey: 938.93 ΧΣ
   entry_numbers:
   - '2089'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1989
   pages: 110
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -72007,15 +72003,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1414
     1: Χ.Σ
     2: ΗΠΕΙΡΟΣ
     3: Η ΕΤΑΙΡΕΙΑ ΗΠΕΙΡΩΤΙΚΩΝ ΜΕΛΕΤΩΝ
-    4: 938.93 ΗΠΕ
+    4: 938.93Χ.Σ
     5: '2089'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1989'
     11: 110Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
@@ -72037,15 +72033,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1415
   authors: []
   title: Ο ΙΠΠΟΤΗΣ ΙΩΑΝΝΗΣ ΓΑΒΡΙΗΛ
-  dewey: 938.545 ΙΠΠ
+  dewey: 938.545 ΧΣ
   entry_numbers:
   - '2425'
   editor: None // ΑΘΗΝΑ
   edition_year: 1963
   pages: 69
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -72055,15 +72051,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1415
     1: Χ.Σ
     2: Ο ΙΠΠΟΤΗΣ ΙΩΑΝΝΗΣ ΓΑΒΡΙΗΛ
-    4: 938.545ΙΠΠ
+    4: 938.545Χ.Σ
     5: '2425'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1963'
     11: 69Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΦΙΛΕΛΛΗΝΑΣ
     13: ΦΙΛΕΛΛΗΝΑΣ-ΓΑΒΡΙΗΛ
@@ -72087,15 +72083,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1416
   authors: []
   title: ΙΣΡΑΗΛ
   subtitle: ΓΕΓΟΝΟΤΑ ΚΑΙ ΑΡΙΘΜΟΙ
-  dewey: 950 ΙΣΡ
+  dewey: 950 ΧΣ
   entry_numbers:
   - '444'
   editor: None // ΑΘΗΝΑ
   edition_year: 1979
   pages: 247
   topics:
   - ΙΣΡΑΗΛΙΝΗ ΙΣΤΟΡΙΑ
@@ -72104,15 +72100,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1416
     1: Χ.Σ
     2: ΙΣΡΑΗΛ
     3: ΓΕΓΟΝΟΤΑ ΚΑΙ ΑΡΙΘΜΟΙ
-    4: 950 ΙΣΡ
+    4: 950Χ.Σ
     5: '444'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1979'
     11: 247Σ
     12: ΙΣΡΑΗΛΙΝΗ ΙΣΤΟΡΙΑ
     13: ΙΣΡΑΗΛ-ΙΣΤΟΡΙΑ
@@ -72134,15 +72130,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1417
   authors: []
   title: Η ΙΣΤΟΡΙΑ ΤΗΣ ΑΜΕΡΙΚΑΝΙΚΗΣ ΠΡΟΣΠΑΘΕΙΑΣ ΕΙΣ ΤΗΝ ΕΛΛΑΔΑ
-  dewey: 970 ΙΣΤ
+  dewey: 970 ΧΣ
   entry_numbers:
   - '1947'
   edition_year: 1952
   pages: 144
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΣΧΕΔΙΟ ΜΑΡΣΑΛ
@@ -72151,15 +72147,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1417
     1: Χ.Σ
     2: Η ΙΣΤΟΡΙΑ ΤΗΣ ΑΜΕΡΙΚΑΝΙΚΗΣ ΠΡΟΣΠΑΘΕΙΑΣ ΕΙΣ ΤΗΝ ΕΛΛΑΔΑ
-    4: 970 ΙΣΤ
+    4: 970Χ.Σ
     5: '1947'
     8: Χ.Ε
     9: Χ.Τ
     10: '1952'
     11: 144Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΧΕΔΙΟ ΜΑΡΣΑΛΛ
     13: ΣΧΕΔΙΟ ΜΑΡΣΑΛ
@@ -72198,15 +72194,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1418
     1: Χ.Σ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΑΔΑΣ
-    4: 938.1 Χ.Σ
+    4: 938.1Χ.Σ
     5: '1909'
     8: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ
     9: ΑΘΗΝΑ
     10: '1978'
     11: 600Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     3: null
@@ -72246,15 +72242,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1419
     1: Χ.Σ
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΛΑΟΥ ΤΟΥ ΙΣΡΑΗΛ ΜΕΧΡΙ ΤΟΥ 1880
-    4: 950 Χ.Σ
+    4: 950Χ.Σ
     5: 441-442
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1974'
     11: 360Σ
     12: ΙΣΡΑΗΛΙΝΗ ΙΣΤΟΡΙΑ
     13: ΙΣΡΑΗΛ-ΙΣΤΟΡΙΑ
@@ -72324,15 +72320,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1421
   authors: []
   title: ΚΥΠΡΟΣ '74 ΤΟ ΑΛΛΟ ΠΡΟΣΩΠΟ ΤΗΣ ΑΦΡΟΔΙΤΗΣ
-  dewey: 938.497 ΚΥΠ
+  dewey: 938.497 ΧΣ
   entry_numbers:
   - '380'
   editor: None // ΑΘΗΝΑ
   edition_year: 1975
   pages: 277
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -72341,15 +72337,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1421
     1: Χ.Σ
     2: ΚΥΠΡΟΣ '74 ΤΟ ΑΛΛΟ ΠΡΟΣΩΠΟ ΤΗΣ ΑΦΡΟΔΙΤΗΣ
-    4: 938.497ΚΥΠ
+    4: 938.497Χ.Σ
     5: '380'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 277Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
     13: ΚΥΠΡΟΣ-ΑΦΡΟΔΙΤΗ
@@ -72521,15 +72517,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1425
   authors: []
   title: ΜΕΓΑΛΕΣ ΜΟΡΦΕΣ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
-  dewey: 938 ΜΕΓ
+  dewey: 938 ΧΣ
   entry_numbers:
   - '1957'
   - '2355'
   editor: ΚΟΤΖΙΑ // ΑΘΗΝΑ
   pages: 10
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -72538,26 +72534,26 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1425
     1: Χ.Σ
     2: ΜΕΓΑΛΕΣ ΜΟΡΦΕΣ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
-    4: 938 ΜΕΓ
+    4: 938Χ.Σ
     5: 1957-2355
     8: ΚΟΤΖΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 10Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΟΡΦΕΣ
     13: ΜΟΡΦΕΣ ΤΗΣ ΙΣΤΟΡΙΑΣ
+    14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
     3: null
     6: null
     7: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -72638,15 +72634,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1427
     1: Χ.Σ
     2: ΜΩΣΑΒ ΚΑΙ ΚΙΜΠΟΥΤΖ
     3: ΤΡΟΠΟΙ ΑΓΡΟΤΙΚΗΣ ΖΩΗΣ ΣΤΟ ΙΣΡΑΗΛ
-    4: 915.35 ΜΩΣ
+    4: 915.35ΜΩΣ
     5: '440'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1979'
     11: 34Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΙΣΡΑΗΛ-ΑΓΡΟΤΙΚΗ
     13: ΙΣΡΑΗΛ-ΓΕΩΓΡΑΦΙΑ
@@ -72668,15 +72664,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1428
   authors: []
   title: ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ ΑΚΑΔΗΜΑΙΚΩΝ ΓΙΑ ΤΗΝ 28 ΟΚΤΩΒΡΙΟΥ 1940
-  dewey: 938.752 ΠΑΝ
+  dewey: 938.752 ΧΑΡ
   entry_numbers:
   - '2505'
   editor: None // ΑΘΗΝΑ
   edition_year: 1978
   pages: 608
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -72685,15 +72681,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1428
     1: Χ.Σ
     2: ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ ΑΚΑΔΗΜΑΙΚΩΝ ΓΙΑ ΤΗΝ 28 ΟΚΤΩΒΡΙΟΥ 1940
-    4: 938.752ΠΑΝ
+    4: 938.752ΧΑΡ
     5: '2505'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 608Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940-28 ΟΚΤΩΒΡΙΟΥ
     13: 1940-28 ΟΚΤΩΒΡΙΟΥ
@@ -72831,15 +72827,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1431
     1: Χ.Σ
     2: ΠΡΟΒΛΗΜΑΤΑ ΕΔΑΦΙΚΗΣ ΑΚΕΡΑΙΟΤΗΤΑΣ (ΑΙΓΑΙΟ)
-    4: 938.7 ΠΡΟ
+    4: 938.7ΠΡΟ
     5: '1977'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 32Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΔΑΦΙΚΗ ΑΚΕΡΑΙΟΤΗΤΑ
     13: ΕΔΑΦΙΚΗ ΑΚΕΡΑΙΟΤΗΤΑ
@@ -72862,15 +72858,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1432
   authors: []
   title: Η ΠΡΟΣ ΠΟΛΕΜΟΝ ΠΡΟΠΑΡΑΣΚΕΥΗ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΣΤΡΑΤΟΥ (1923-1940
-  dewey: 938.73 ΠΡΟ
+  dewey: 938.73 ΧΣ
   entry_numbers:
   - '2134'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
   pages: 171
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -72879,15 +72875,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1432
     1: Χ.Σ
     2: Η ΠΡΟΣ ΠΟΛΕΜΟΝ ΠΡΟΠΑΡΑΣΚΕΥΗ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΣΤΡΑΤΟΥ (1923-1940
-    4: 938.73ΠΡΟ
+    4: 938.73Χ.Σ
     5: '2134'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1969'
     11: 171Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ
     13: ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ-1940
@@ -72958,30 +72954,30 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1434
   authors: []
   title: ΤΟ ΡΟΥΜΑΝΙΚΟ ΒΙΒΛΙΟ
-  dewey: 949.8 ΡΟΥ
+  dewey: 949.8 ΧΣ
   entry_numbers:
   - '2563'
   editor: None // ΑΘΗΝΑ
   pages: 133
   topics:
   - ΡΟΥΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΡΟΥΜΑΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1434
     1: Χ.Σ
     2: ΤΟ ΡΟΥΜΑΝΙΚΟ ΒΙΒΛΙΟ
-    4: 949.8 ΡΟΥ
+    4: 949.8Χ.Σ
     5: '2563'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Τ
     11: 133Σ
     12: ΡΟΥΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
     13: ΡΟΥΜΑΝΙΑ-ΙΣΤΟΡΙΑ
@@ -73004,30 +73000,30 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1435
   authors: []
   title: ΣΥΝΤΟΜΗ ΙΣΤΟΡΙΑ ΤΩΝ Η.Π.Α
-  dewey: 973 ΣΥΝ
+  dewey: 973 ΧΣ
   entry_numbers:
   - '428'
   pages: 199
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ
   - Η.Π.Α.
   - ΑΜΕΡΙΚΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1435
     1: Χ.Σ
     2: ΣΥΝΤΟΜΗ ΙΣΤΟΡΙΑ ΤΩΝ Η.Π.Α
-    4: 973 ΣΥΝ
+    4: 973Χ.Σ
     5: '428'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 199Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-Η.Π.Α
     13: ΑΜΕΡΙΚΗ-ΙΣΤΟΡΙΑ
@@ -73050,29 +73046,29 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1436
   authors: []
   title: ΣΥΝΟΨΗ ΤΗΣ ΓΕΩΓΡΑΦΙΑΣ ΤΗΣ ΑΜΕΡΙΚΗΣ
-  dewey: 917 ΣΥΝ
+  dewey: 917 ΧΣ
   entry_numbers:
   - '2324'
   pages: 205
   topics:
   - ΓΕΩΓΡΑΦΙΑ
   - ΑΜΕΡΙΚΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1436
     1: Χ.Σ
     2: ΣΥΝΟΨΗ ΤΗΣ ΓΕΩΓΡΑΦΙΑΣ ΤΗΣ ΑΜΕΡΙΚΗΣ
-    4: 917 ΣΥΝ
+    4: 917Χ.Σ
     5: '2324'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 205Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΑΜΕΡΙΚΗ
     13: ΑΜΕΡΙΚΗ-ΓΕΩΓΡΑΦΙΑ
@@ -73096,30 +73092,30 @@
     28: null
     29: null
     30: null
 - dbase_number: 1437
   authors: []
   title: ΣΤΡΑΤΗΓΟΥ ΜΑΚΡΥΓΙΑΝΝΗ
   subtitle: ΠΡΑΓΜΑΤΑ ΚΑΙ ΟΡΑΜΑΤΑ
-  dewey: 938.478 ΣΤΡ
+  dewey: 938.478 ΧΣ
   entry_numbers:
   - '1694'
   pages: 211
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΑΚΡΥΓΙΑΝΝΗΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1437
     1: Χ.Σ
     2: ΣΤΡΑΤΗΓΟΥ ΜΑΚΡΥΓΙΑΝΝΗ
     3: ΠΡΑΓΜΑΤΑ ΚΑΙ ΟΡΑΜΑΤΑ
-    4: 938.478ΣΤΡ
+    4: 938.478Χ.Σ
     5: '1694'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 211Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΡΥΓΙΑΝΝΗΣ
     13: ΜΑΚΡΥΓΙΑΝΝΗΣ
@@ -73142,30 +73138,30 @@
     28: null
     29: null
     30: null
 - dbase_number: 1438
   authors: []
   title: ΣΤΕΡΕΑ ΕΛΛΑΣ
   subtitle: ΕΙΚΟΝΟΓΡΑΦΗΜΕΝΗ ΕΠΙΘΕΩΡΗΣΙΣ ΤΗΣ ΡΟΥΜΕΛΗΣ
-  dewey: 938.91 ΣΤΕ
+  dewey: 938.91 ΧΣ
   entry_numbers:
   - '336'
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΣΤΕΡΕΑ ΕΛΛΑΔΑ
   - ΡΟΥΜΕΛΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1438
     1: Χ.Σ
     2: ΣΤΕΡΕΑ ΕΛΛΑΣ
     3: ΕΙΚΟΝΟΓΡΑΦΗΜΕΝΗ ΕΠΙΘΕΩΡΗΣΙΣ ΤΗΣ ΡΟΥΜΕΛΗΣ
-    4: 938.91 ΣΤΕ
+    4: 938.91Χ.Σ
     5: '336'
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΤΕΡΕΑ ΕΛΛΑΣ
     13: ΣΤΕΡΕΑ ΕΛΛΑΣ
     14: ΡΟΥΜΕΛΗ
@@ -73187,15 +73183,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1439
   authors: []
   title: ΤΡΙΑ ΕΤΗ ΔΙΑΚΥΒΕΡΝΗΣΕΩΣ ΤΟΥ Κ.ΙΩΑΝΝΟΥ ΜΕΤΑΞΑ (1936-1939)
-  dewey: 938.714 ΤΡΙ
+  dewey: 938.714 ΧΣ
   entry_numbers:
   - '2557'
   editor: ΠΥΡΣΟΣ // ΑΘΗΝΑ
   edition_year: 1939
   pages: 323
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -73203,15 +73199,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1439
     1: Χ.Σ
     2: ΤΡΙΑ ΕΤΗ ΔΙΑΚΥΒΕΡΝΗΣΕΩΣ ΤΟΥ Κ.ΙΩΑΝΝΟΥ ΜΕΤΑΞΑ (1936-1939)
-    4: 938.714ΤΡΙ
+    4: 938.714Χ.Σ
     5: '2557'
     8: ΠΥΡΣΟΣ
     9: ΑΘΗΝΑ
     10: '1939'
     11: 323Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΤΑΞΑΣ
     13: ΜΕΤΑΞΑΣ
@@ -73234,15 +73230,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1440
   authors: []
   title: ΦΑΚΕΛΛΟΣ ΑΙΓΑΙΟ
-  dewey: 938.7 ΦΑΚ
+  dewey: 938.7 ΧΣ
   entry_numbers:
   - '1976'
   editor: None // ΑΘΗΝΑ
   edition_year: 1978
   pages: 78
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -73252,15 +73248,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1440
     1: Χ.Σ
     2: ΦΑΚΕΛΛΟΣ ΑΙΓΑΙΟ
-    4: 938.7 ΦΑΚ
+    4: 938.7Χ.Σ
     5: '1976'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 78Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΦΑΚΕΛΛΟΣ ΑΙΓΑΙΟΥ
     13: ΑΙΓΑΙΟ-ΦΑΚΕΛΛΟΣ
@@ -73284,15 +73280,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1441
   authors: []
   title: ΧΡΟΝΙΚΟΝ 1940-1944
   subtitle: ΕΜΠΡΟΣ ΤΗΣ ΕΛΛΑΔΟΣ ΠΑΙΔΙΑ
-  dewey: 938.75 ΧΡΟ
+  dewey: 938.75 ΧΣ
   entry_numbers:
   - '2295'
   editor: None // ΑΘΗΝΑ
   edition_year: 1978
   pages: 375
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -73303,15 +73299,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1441
     1: Χ.Σ
     2: ΧΡΟΝΙΚΟΝ 1940-1944
     3: ΕΜΠΡΟΣ ΤΗΣ ΕΛΛΑΔΟΣ ΠΑΙΔΙΑ
-    4: 938.75 ΧΡΟ
+    4: 938.75Χ.Σ
     5: '2295'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 375Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
     13: 1940-ΧΡΟΝΙΚΟ
@@ -73331,34 +73327,35 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1442
-  authors: []
+  authors:
+  - ΜΟΔΗ,ΓΕΩΡΓΙΟΥ
   title: ΧΩΡΙΑ-ΦΡΟΥΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
-  dewey: 938.664 ΧΩΡ
+  dewey: 938.664 ΜΟΔ
   entry_numbers:
   - '349'
   editor: None // ΑΘΗΝΑ
   edition_year: 1964
   pages: 16
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΑΚΕΔΟΝΙΑ
   - ΧΩΡΙΑ ΦΡΟΥΡΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1442
-    1: Χ.Σ
+    1: ΜΟΔΗ,ΓΕΩΡΓΙΟΥ
     2: ΧΩΡΙΑ-ΦΡΟΥΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
-    4: 938.664ΧΩΡ
+    4: 938.664ΜΟΔ
     5: '349'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1964'
     11: 16Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΑ-ΧΩΡΙΑ ΦΡΟΥΡΙΑ
@@ -74995,15 +74992,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1475
   authors: []
   title: ΕΛΕΥΘΕΡΙΟΣ ΒΕΝΙΖΕΛΟΣ
   subtitle: Η ΖΩΗ ΚΑΙ ΤΟ ΕΡΓΟΝ ΤΟΥ
-  dewey: 938.672 ΕΛΕ
+  dewey: 938.672 ΧΣ
   entry_numbers:
   - '2585'
   editor: None // ΑΘΗΝΑ
   edition_year: 1936
   pages: 175
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -75013,15 +75010,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1475
     1: Χ.Σ
     2: ΕΛΕΥΘΕΡΙΟΣ ΒΕΝΙΖΕΛΟΣ
     3: Η ΖΩΗ ΚΑΙ ΤΟ ΕΡΓΟΝ ΤΟΥ
-    4: 938.672ΕΛΕ
+    4: 938.672Χ.Σ
     5: '2585'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1936'
     11: 175Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ
     13: ΒΕΝΙΖΕΛΟΣ-ΖΩΗ ΚΑΙ ΕΡΓΟ
@@ -75184,15 +75181,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1479
   authors: []
   title: ΜΝΗΜΗ ΔΗΜΗΤΡΙΟΥ ΑΙΓΝΗΤΟΥ (1862-1934)
-  dewey: 938.729 ΜΝΗ
+  dewey: 938.729 ΧΣ
   entry_numbers:
   - '2378'
   editor: None // ΑΘΗΝΑ
   edition_year: 1975
   pages: 469
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -75202,15 +75199,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1479
     1: Χ.Σ
     2: ΜΝΗΜΗ ΔΗΜΗΤΡΙΟΥ ΑΙΓΝΗΤΟΥ (1862-1934)
-    4: 938.729ΜΝΗ
+    4: 938.729Χ.Σ
     5: '2378'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1975'
     11: 469Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΑΙΓΙΝΗΤΗΣ-(1862-1934)
@@ -75234,15 +75231,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1480
   authors: []
   title: ΓΕΩΡΓΙΟΥ ΠΑΠΑΝΔΡΕΟΥ
   subtitle: ΚΕΙΜΕΝΑ (1913-1942)
-  dewey: 938.791 ΓΕΩ
+  dewey: 938.791 ΧΣ
   entry_numbers:
   - '2379'
   editor: ΜΠΙΡΗΣ // ΑΘΗΝΑ
   pages: 318
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΓΕΤΕΣ
@@ -75252,15 +75249,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1480
     1: Χ.Σ
     2: ΓΕΩΡΓΙΟΥ ΠΑΠΑΝΔΡΕΟΥ
     3: ΚΕΙΜΕΝΑ (1913-1942)
-    4: 938.791ΓΕΩ
+    4: 938.791Χ.Σ
     5: '2379'
     8: ΜΠΙΡΗΣ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 318Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΓΕΤΕΣ
     13: ΗΓΕΤΕΣ-ΠΑΠΑΝΔΡΕΟΥ ΓΕΩΓΡΙΟΣ
@@ -75734,45 +75731,43 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1490
   authors:
-  - ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΤΕΦΑΝΟΣ Π.
-  title: ΤΟ ΧΕΡΣΑΙΟ ΔΙΚΤΥΟ ΕΠΙΚΟΙΝΩΝΙΑΣ ΣΤΟ ΚΡΑΤΟΣ ΤΟΥ ΑΛΗ ΠΑΣΑ
-  subtitle: ΤΕΠΕΛΕΝΛΗ
-  dewey: 938.484 ΜΑΚ
+  - ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ,ΘΩΜΑΣ
+  title: ΤΟ ΠΡΟΕΠΑΝΑΣΤΑΤΙΚΟ ΚΙΝΗΜΑ ΤΟΥ ΠΑΠΑ ΕΥΘΥΜΙΟΥ ΒΛΑΧΑΒΑ ΣΤΗ
+  subtitle: ΘΕΣΣΑΛΑΙ (1807-1809) ΚΑΙ ΟΙ ΞΕΝΟΙ ΙΣΤΟΡΙΚΟΙ-ΠΕΡΙΗΓΗΤΕΣ
+  dewey: 938.485 ΠΑΠ
   entry_numbers:
-  - '1708'
-  - '4160'
-  editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
-  edition_year: 1990
-  pages: 240
+  - '5194'
+  editor: ΟΛΥΜΠΟΣ // ΑΘΗΝΑ
+  edition_year: 1998
+  pages: 91
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
-  - ΤΕΠΕΛΕΝΛΗ
-  - ΑΛΗ ΠΑΣΑΣ
+  - ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1490
-    1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΤΕΦΑΝΟΣ Π.
-    2: ΤΟ ΧΕΡΣΑΙΟ ΔΙΚΤΥΟ ΕΠΙΚΟΙΝΩΝΙΑΣ ΣΤΟ ΚΡΑΤΟΣ ΤΟΥ ΑΛΗ ΠΑΣΑ
-    3: ΤΕΠΕΛΕΝΛΗ
-    4: 938.484ΜΑΚ
-    5: 1708-4160
-    8: ΠΑΠΑΖΗΣΗ
+    1: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ,ΘΩΜΑΣ
+    2: ΤΟ ΠΡΟΕΠΑΝΑΣΤΑΤΙΚΟ ΚΙΝΗΜΑ ΤΟΥ ΠΑΠΑ ΕΥΘΥΜΙΟΥ ΒΛΑΧΑΒΑ ΣΤΗ
+    3: ΘΕΣΣΑΛΑΙ (1807-1809) ΚΑΙ ΟΙ ΞΕΝΟΙ ΙΣΤΟΡΙΚΟΙ-ΠΕΡΙΗΓΗΤΕΣ
+    4: 938.485ΠΑΠ
+    5: '5194'
+    8: ΟΛΥΜΠΟΣ
     9: ΑΘΗΝΑ
-    10: '1990'
-    11: 240Σ
-    12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΕΠΕΛΕΝΛΗ
-    13: ΤΕΠΕΛΕΝΛΗ-ΑΛΗ ΠΑΣΑΣ
-    14: ΑΛΗ ΠΑΣΑΣ-ΤΕΠΕΛΕΝΛΗ
+    10: '1998'
+    11: '91'
+    12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ
+    13: ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ-ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
+    14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -76795,15 +76790,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1511
   authors: []
   title: ΜΟΥΣΕΙΟ "ΕΛΕΥΘΕΡΙΟΣ Κ.ΒΕΝΙΖΕΛΟΣ"
-  dewey: 938.672 ΜΟΥ
+  dewey: 938.672 ΧΣ
   entry_numbers:
   - '2884'
   editor: None // ΑΘΗΝΑ
   edition_year: 1992
   pages: 154
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -76812,15 +76807,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1511
     1: Χ.Σ
     2: ΜΟΥΣΕΙΟ "ΕΛΕΥΘΕΡΙΟΣ Κ.ΒΕΝΙΖΕΛΟΣ"
-    4: 938.672ΜΟΥ
+    4: 938.672Χ.Σ
     5: '2884'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1992'
     11: 154Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ
     13: ΒΕΝΙΖΕΛΟΣ-ΜΟΥΣΕΙΟ
@@ -76865,15 +76860,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1512
     1: ΨΑΘΑΣ,ΔΗΜΗΤΡΗΣ
     2: ΖΗΤΕΙΤΑΙ ΨΕΥΤΗΣ
     3: ΚΩΜΩΔΙΑ
-    4: 886.2 ΨΑΘ
+    4: 886.2ΨΑΘ
     5: '2888'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1993'
     11: 107Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
@@ -77095,15 +77090,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1517
   authors:
   - ΤΖΙΟΒΑΣ,ΠΑΝΟΣ ΔΗΜ
   title: ΗΠΕΙΡΩΤΙΚΑ ΑΝΕΚΔΟΤΑ
-  dewey: 398 ΤΖΙ
+  dewey: 938.93 ΤΖΙ
   entry_numbers:
   - '2883'
   - '10439'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1992
   pages: 93
   topics:
@@ -77113,15 +77108,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1517
     1: ΤΖΙΟΒΑΣ,ΠΑΝΟΣ ΔΗΜ
     2: ΗΠΕΙΡΩΤΙΚΑ ΑΝΕΚΔΟΤΑ
-    4: 398 ΤΖΙ
+    4: 938.93ΤΖΙ
     5: 2883-10439
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1992'
     11: 93Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΑΝΕΚΔΟΤΑ
@@ -77144,15 +77139,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1518
   authors:
   - ΑΘΗΝΑΙΟΣ,ΑΝΔΡΕΑΣ
-  title: 7ΕΛΛΗΝΙΚΑ ΘΕΜΑΤΑ
+  title: ΕΛΛΗΝΙΚΑ ΘΕΜΑΤΑ
   dewey: 938 ΑΘΗ
   entry_numbers:
   - '2882'
   editor: None // ΑΘΗΝΑ
   edition_year: 1976
   pages: 46
   topics:
@@ -77161,16 +77156,16 @@
   - ΕΛΛΑΔΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1518
     1: ΑΘΗΝΑΙΟΣ,ΑΝΔΡΕΑΣ
-    2: 7ΕΛΛΗΝΙΚΑ ΘΕΜΑΤΑ
-    4: 938 ΑΘΗ
+    2: ΕΛΛΗΝΙΚΑ ΘΕΜΑΤΑ
+    4: 938ΑΘΗ
     5: '2882'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1976'
     11: 46Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΜΑΤΑ
     13: ΘΕΜΑΤΑ-ΕΛΛΑΔΑ
@@ -77268,15 +77263,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1520
     1: ΠΑΠΑΚΩΣΤΑΣ,ΝΙΚ
     2: ΗΠΕΙΡΩΤΙΚΑ
     3: ΑΘΑΝΑΝΙΚΑ
-    4: 938.93 ΠΑΠ
+    4: 938.93ΠΑΠ
     5: 1380-3016
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 646Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΙΚΑ
@@ -77755,35 +77750,36 @@
     28: null
     29: null
     30: null
 - dbase_number: 1530
   authors:
   - ΠΑΠΑΒΑΣΙΛΕΙΟΥ,ΙΩΑΝΝΗΣ
   title: Ο ΣΥΓΧΡΟΝΟΣ ΤΡΑΓΙΚΟΣ ΑΝΘΡΩΠΟΣ ΚΑΙ ΤΟ ΛΥΤΡΩΤΙΚΟΝ  ΡΟΔΟΧΑΡΑΜΑ
-  dewey: 938.009 ΠΑΠ
+  dewey: 938 ΠΑΠ
   entry_numbers:
   - '5771'
   - '2875'
   - '2876'
+  - '12496'
   editor: None // ΑΘΗΝΑ
   edition_year: 1976
   pages: 85
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΑΝΘΡΩΠΟΣ
   copies: 4
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1530
     1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ,ΙΩΑΝΝΗΣ
     2: Ο ΣΥΓΧΡΟΝΟΣ ΤΡΑΓΙΚΟΣ ΑΝΘΡΩΠΟΣ ΚΑΙ ΤΟ ΛΥΤΡΩΤΙΚΟΝ  ΡΟΔΟΧΑΡΑΜΑ
-    4: 938.009ΠΑΠ
-    5: 5771-2875-2876
+    4: 938ΠΑΠ
+    5: 5771-2875-2876-12496
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1976'
     11: 85Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΘΡΩΠΟΣ
     13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΘΡΩΠΟΣ
     14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -78622,15 +78618,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1547
     1: ΛΟΥΚΑΤΟΣ,ΔΗΜΗΤΡΙΟΣ Σ
     2: Ο ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ ΤΩΝ ΗΠΕΙΡΩΤΩΝ
-    4: 938.93 ΛΟΥ
+    4: 938.93ΛΟΥ
     5: 2768-2887
     8: ΑΘΗΝΑ
     9: Χ.Ε
     10: '1976'
     11: 36Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ
@@ -79568,18 +79564,18 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1566
   authors:
-  - ΜΥΡΣΙΝΗ-ΜΑΝΘΟΥ,ΑΛΚΗ
+  - ΜΑΝΘΟΥ,ΜΥΡΣΙΝΗ-ΑΛΚΗ
   title: ΗΠΕΙΡΩΤΑΙ ΔΗΜΟΣΙΟΓΡΑΦΟΙ ΣΤΗ ΡΟΥΜΑΝΙΑ
   subtitle: Ζ.ΣΑΡΔΕΛΛΗΣ Κ ΥΙΟΙ,ΣΠ.ΣΙΜΟΣ,Ι.ΟΙΚΟΝΟΜΟΥ,Κ.ΒΕΛΕΝΤΖΑΣ Κ.Α
-  dewey: 938.93 ΜΥΡ
+  dewey: 938.93 ΜΑΝ
   entry_numbers:
   - '2828'
   - '2827'
   - '9248'
   editor: None // ΑΘΗΝΑ
   edition_year: 1973
   pages: 31
@@ -79590,18 +79586,18 @@
   - ΔΗΜΟΣΙΟΓΡΑΦΟΙ
   - ΗΠΕΙΡΩΤΕΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1566
-    1: ΜΥΡΣΙΝΗ-ΜΑΝΘΟΥ,ΑΛΚΗ
+    1: ΜΑΝΘΟΥ,ΜΥΡΣΙΝΗ-ΑΛΚΗ
     2: ΗΠΕΙΡΩΤΑΙ ΔΗΜΟΣΙΟΓΡΑΦΟΙ ΣΤΗ ΡΟΥΜΑΝΙΑ
     3: Ζ.ΣΑΡΔΕΛΛΗΣ Κ ΥΙΟΙ,ΣΠ.ΣΙΜΟΣ,Ι.ΟΙΚΟΝΟΜΟΥ,Κ.ΒΕΛΕΝΤΖΑΣ Κ.Α
-    4: 938.93 ΜΥΡ
+    4: 938.93ΜΑΝ
     5: 2828-2827-9248
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1973'
     11: 31Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΩΤΕΣ ΔΗΜΟΣΙΟΓΡΑΦΟΙ
     13: ΗΠΕΙΡΟΣ-ΔΗΜΟΣΙΟΓΡΑΦΟΙ
@@ -79647,15 +79643,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1567
     1: ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ ΑΧ
     2: ΓΕΩΡΓΙΟΣ ΧΑΤΖΗΣ-ΠΕΛΛΕΡΕΝ
     3: Ο ΗΠΕΙΡΩΤΗΣ ΑΓΩΝΙΣΤΗΣ,Ο ΔΗΜΟΣΙΟΓΡΑΦΟΣ,Ο ΠΟΙΗΤΗΣ
-    4: 938.93 ΒΑΒ
+    4: 938.93ΒΑΒ
     5: '2773'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1963'
     11: 31Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΧΑΤΖΗΣ
@@ -79699,15 +79695,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1568
     1: ΛΑΜΠΡΙΔΗΣ,ΣΤΑΘΗΣ Δ
     2: ΚΩΣΤΑΣ ΓΚΡΑΤΖΙΟΣ
     3: Ο ΜΕΓΑΛΟΣ ΗΠΕΙΡΩΤΗΣ ΕΚΠΑΙΔΕΥΤΗΣ
-    4: 938.93 ΛΑΜ
+    4: 938.93ΛΑΜ
     5: '2829'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1983'
     11: 48Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΓΚΡΑΤΖΙΟΣ
@@ -79783,15 +79779,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1570
   authors:
   - ΣΦΑΕΛΛΟΣ,ΔΗΜ Κ
   title: ΕΘΝΙΚΗ ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΚΑΙ ΕΘΝΙΚΑ ΙΔΑΝΙΚΑ
-  dewey: 938.032 ΣΦΑ
+  dewey: 938.05 ΣΦΑ
   entry_numbers:
   - '2747'
   - '2748'
   editor: None // ΑΘΗΝΑ
   edition_year: 1978
   pages: 56
   topics:
@@ -79804,15 +79800,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1570
     1: ΣΦΑΕΛΛΟΣ,ΔΗΜ Κ
     2: ΕΘΝΙΚΗ ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΚΑΙ ΕΘΝΙΚΑ ΙΔΑΝΙΚΑ
-    4: 938.032ΣΦΑ
+    4: 938.05ΣΦΑ
     5: 2747-2748
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 56Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ
     13: ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ-ΕΛΛΑΣ
@@ -80102,17 +80098,19 @@
     28: null
     29: null
     30: null
 - dbase_number: 1576
   authors:
   - ΚΑΡΑΤΖΕΝΗΣ,ΔΗΜΗΤΡΙΟΣ ΦΩΤΙΟΣ
   title: Η ΕΚΑΤΟΝΤΑΕΤΗΡΙΣ ΤΗΣ ΑΡΤΑΣ(1881-1981)
-  dewey: 938.65 ΚΑΡ
+  dewey: 938.939 ΚΑΡ
   entry_numbers:
   - '2807'
+  - '15812'
+  - '16445'
   editor: ΣΚΟΥΦΑΣ // ΑΘΗΝΑ
   edition_year: 1982
   pages: 62
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΑΡΤΑ
@@ -80120,16 +80118,16 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1576
     1: ΚΑΡΑΤΖΕΝΗΣ,ΔΗΜΗΤΡΙΟΣ ΦΩΤΙΟΣ
     2: Η ΕΚΑΤΟΝΤΑΕΤΗΡΙΣ ΤΗΣ ΑΡΤΑΣ(1881-1981)
-    4: 938.65 ΚΑΡ
-    5: '2807'
+    4: 938.939ΚΑΡ
+    5: 2807-15812-16445
     8: ΣΚΟΥΦΑΣ
     9: ΑΘΗΝΑ
     10: '1982'
     11: 62Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΑΡΤΑ
     14: ΑΡΤΑ-(1881-1981)
@@ -80374,15 +80372,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1581
     1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞ Χ
     2: ΛΑΙΚΗ ΑΡΧΙΤΕΚΤΟΝΙΚΗ
     3: ΗΠΕΙΡΩΤΕΣ ΜΑΣΤΟΡΟΙ ΚΑΙ ΓΕΦΥΡΙΑ
-    4: 938.93 ΜΑΜ
+    4: 938.93ΜΑΜ
     5: 2898-2899
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1973'
     11: 48Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΑΡΧΙΤΕΚΤΟΝΙΚΗ
@@ -80502,17 +80500,18 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1584
-  authors: []
+  authors:
+  - ΕΜΜΑΝΟΥΗΛ,ΦΙΛΙΠΠΟΣ
   title: Η ΕΝΝΟΙΑ ΤΗΣ ΠΑΡΑΔΟΣΕΩΣ ΚΑΙ Η ΗΠΕΙΡΟΣ
-  dewey: 398 ΧΣ
+  dewey: 938.93 ΕΜΜ
   entry_numbers:
   - '2902'
   editor: None // ΑΘΗΝΑ
   edition_year: 1980
   pages: 28
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -80520,17 +80519,17 @@
   - ΠΑΡΑΔΟΣΗ
   notes: ΔΙΑΛΕΞΗ ΚΑΘΗΓΗΤΟΥ ΦΙΛΙΠΠΟΥ Δ. ΕΜΜΑΝΟΥΗΛ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1584
-    1: Χ.Σ
+    1: ΕΜΜΑΝΟΥΗΛ,ΦΙΛΙΠΠΟΣ
     2: Η ΕΝΝΟΙΑ ΤΗΣ ΠΑΡΑΔΟΣΕΩΣ ΚΑΙ Η ΗΠΕΙΡΟΣ
-    4: 398 Χ.Σ.
+    4: 938.93ΕΜΜ
     5: '2902'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1980'
     11: 28Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΠΑΡΑΔΟΣΗ
@@ -86883,15 +86882,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1709
   authors: []
   title: ΤΡΑΝΣΤΕΚΟΜ
   subtitle: ΛΕΥΚΩΜΑ
-  dewey: 938.5 ΤΡΑ
+  dewey: 938.5 ΧΣ
   entry_numbers:
   - '3164'
   editor: None // ΑΘΗΝΑ
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - '1821'
   - ΛΕΥΚΩΜΑ
@@ -86899,15 +86898,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1709
     1: Χ.Σ
     2: ΤΡΑΝΣΤΕΚΟΜ
     3: ΛΕΥΚΩΜΑ
-    4: 938.5 ΤΡΑ
+    4: 938.5Χ.Σ
     5: '3164'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821
     13: 1821-ΛΕΥΚΩΜΑ
     14: ΛΕΥΚΩΜΑ-1821
@@ -87644,15 +87643,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 1724
   authors: []
   title: ΚΑΣΣΩΠΗ-ΖΑΛΟΓΓΟ
   subtitle: ΑΠΟ ΤΟ ΟΔΟΙΠΟΡΙΚΟ ΣΤΟΝ ΕΛΛΗΝΙΚΟ ΧΩΡΟ
-  dewey: 938.93 ΚΑΣ
+  dewey: 938.93 ΧΣ
   entry_numbers:
   - '291'
   edition_year: 1973
   pages: 61
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
@@ -87663,15 +87662,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1724
     1: Χ.Σ
     2: ΚΑΣΣΩΠΗ-ΖΑΛΟΓΓΟ
     3: ΑΠΟ ΤΟ ΟΔΟΙΠΟΡΙΚΟ ΣΤΟΝ ΕΛΛΗΝΙΚΟ ΧΩΡΟ
-    4: 938.93 ΚΑΣ
+    4: 938.93Χ.Σ
     5: '291'
     8: Χ.Ε
     9: Χ.Τ
     10: '1973'
     11: 61Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΚΑΣΣΩΠΗ
@@ -88170,15 +88169,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1734
     1: ΑΡΑΒΑΝΤΙΝΟΣ,Π
     2: ΗΠΕΙΡΩΤΙΚΟΝ ΓΛΩΣΣΑΡΙΟΝ
-    4: 938.93 ΑΡΑ
+    4: 938.93ΑΡΑ
     5: '3021'
     8: ΠΕΤΡΑΚΟΥ
     9: ΑΘΗΝΑ
     10: '1909'
     11: 102Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΓΛΩΣΣΑΡΙΟ
@@ -117637,15 +117636,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 2316
   authors: []
   title: ΤΟ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟΝ ΖΗΤΗΜΑ
   subtitle: ΠΑΡΕΛΘΟΝ-ΠΑΡΟΝ-ΜΕΛΛΟΝ ΠΡΑΚΤΙΚΑ
-  dewey: 938.694 ΒΟΡ
+  dewey: 938.694 ΧΣ
   entry_numbers:
   - '3653'
   editor: None // ΑΘΗΝΑ
   edition_year: 1992
   pages: 623
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -117658,15 +117657,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2316
     1: Χ.Σ
     2: ΤΟ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟΝ ΖΗΤΗΜΑ
     3: ΠΑΡΕΛΘΟΝ-ΠΑΡΟΝ-ΜΕΛΛΟΝ ΠΡΑΚΤΙΚΑ
-    4: 938.694ΒΟΡ
+    4: 938.694Χ.Σ
     5: '3653'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1992'
     11: 623Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
     13: ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ-ΠΡΑΚΤΙΚΑ
@@ -117705,15 +117704,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2317
     1: Χ.Σ
     2: Η ΑΡΧΑΙΑ ΕΛΛΑΣ
-    4: 938.1 ΑΡΧ
+    4: 938.1ΑΡΧ
     5: '256'
     8: ΚΑΔΜΟΣ
     9: ΑΘΗΝΑ
     10: '1957'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΑΡΧΑΙΟΤΗΤΑ-ΦΙΛΟΣΟΦΙΑ
     14: ΦΙΛΟΣΟΦΙΑ-ΑΡΧΑΙΑ
@@ -117945,15 +117944,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 2322
   authors: []
   title: ΕΝΑΣ ΕΛΛΗΝΑΣ ΤΟΥ 20 ΑΙΩΝΟΣ
   subtitle: ΕΜΜΑΝΟΥΗΛ ΜΠΕΝΑΚΗΣ
-  dewey: 938.8 ΕΛΛ
+  dewey: 938.8 ΧΣ
   entry_numbers:
   - '3677'
   editor: None // ΑΘΗΝΑ
   edition_year: 1931
   pages: 27
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -117963,15 +117962,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2322
     1: Χ.Σ
     2: ΕΝΑΣ ΕΛΛΗΝΑΣ ΤΟΥ 20 ΑΙΩΝΟΣ
     3: ΕΜΜΑΝΟΥΗΛ ΜΠΕΝΑΚΗΣ
-    4: 938.8 ΕΛΛ
+    4: 938.8Χ.Σ
     5: '3677'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1931'
     11: 27Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-20 ΑΙΩΝΑΣ
     13: 20 ΑΙΩΝΑΣ-ΜΠΕΝΑΚΗΣ
@@ -117992,15 +117991,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2323
   authors:
-  - ΧΙΩΤΑΚΗ, ΑΜΑΛΙΑ
+  - ΧΙΩΤΑΚΗ,ΑΜΑΛΙΑ
   title: Η ΣΥΜΠΕΡΙΦΟΡΑ ΤΟΥ ΤΡΑΠΕΖΙΚΟΥ ΚΕΦΑΛΑΙΟΥ ΣΕ ΜΙΑ ΑΓΡΟΤΙΚΗ ΚΟΙΝ
   subtitle: Η ΠΕΡΙΠΤΩΣΗ ΤΗΣ ΤΡΑΠΕΖΑΣ ΗΠΕΙΡΟΘΕΣΣΑΛΙΑΣ ΣΤΗΝ ΑΡΤΑ
   dewey: 938.6 ΧΙΩ
   entry_numbers:
   - '3674'
   editor: None // ΑΘΗΝΑ
   edition_year: 1994
@@ -118012,18 +118011,18 @@
   - ΚΕΦΑΛΑΙΟ
   - ΤΡΑΠΕΖΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2323
-    1: ΧΙΩΤΑΚΗ, ΑΜΑΛΙΑ
+    1: ΧΙΩΤΑΚΗ,ΑΜΑΛΙΑ
     2: Η ΣΥΜΠΕΡΙΦΟΡΑ ΤΟΥ ΤΡΑΠΕΖΙΚΟΥ ΚΕΦΑΛΑΙΟΥ ΣΕ ΜΙΑ ΑΓΡΟΤΙΚΗ ΚΟΙΝ
     3: Η ΠΕΡΙΠΤΩΣΗ ΤΗΣ ΤΡΑΠΕΖΑΣ ΗΠΕΙΡΟΘΕΣΣΑΛΙΑΣ ΣΤΗΝ ΑΡΤΑ
-    4: 938.6 ΧΙΩ
+    4: 938.6ΧΙΩ
     5: '3674'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1994'
     11: 509Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΡΟΤΙΚΗ ΚΟΙΝΩΝΙΑ
     13: ΑΓΡΟΤΙΚΗ ΚΟΙΝΩΝΙΑ-ΑΡΤΑ
@@ -119066,15 +119065,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2344
     1: ΑΘΑΝΑΣΙΑΔΗ-ΝΟΒΑ,ΘΕΜ
     2: ΣΤΗΝ ΤΟΥΡΚΙΑ ΜΕ ΔΗΜΟΣΙΑΓΡΑΦΙΚΟ ΦΑΚΟ(1925-1926)
-    4: 938.73 ΑΘΑ
+    4: 938.73ΑΘΑ
     5: '2540'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΙΑ
     13: ΤΟΥΡΚΙΑ-ΔΗΜΟΣΙΟΓΡΑΦΙΑ(1925-1926)
     14: ΔΗΜΟΣΙΟΓΡΑΦΙΑ(1925-1926)
@@ -139702,15 +139701,15 @@
     29: null
     30: null
 - dbase_number: 2755
   authors:
   - ΛΟΙΖΙΔΗΣ,ΣΑΒΒΑΣ
   title: ΑΤΥΧΗ ΚΥΠΡΟΣ
   subtitle: ΠΩΣ ΕΖΗΣΑ ΤΟΥΣ ΠΟΘΟΥΣ ΚΑΙ ΤΟΥΣ ΚΑΗΜΟΥΣ ΤΗΣ 1910-1980
-  dewey: 938.799 ΛΟΙ
+  dewey: 938.497 ΛΟΙ
   entry_numbers:
   - '4084'
   editor: ΜΠΕΡΓΑΔΗ // ΑΘΗΝΑ
   edition_year: 1980
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΚΥΠΡΟΣ
@@ -139718,15 +139717,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2755
     1: ΛΟΙΖΙΔΗΣ,ΣΑΒΒΑΣ
     2: ΑΤΥΧΗ ΚΥΠΡΟΣ
     3: ΠΩΣ ΕΖΗΣΑ ΤΟΥΣ ΠΟΘΟΥΣ ΚΑΙ ΤΟΥΣ ΚΑΗΜΟΥΣ ΤΗΣ 1910-1980
-    4: 938.799ΛΟΙ
+    4: 938.497ΛΟΙ
     5: '4084'
     8: ΜΠΕΡΓΑΔΗ
     9: ΑΘΗΝΑ
     10: '1980'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
     13: ΚΥΠΡΟΣ
     6: null
@@ -139902,15 +139901,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 2759
   authors: []
   title: Η ΕΠΕΚΤΑΤΙΚΗ ΠΟΛΙΤΙΚΗ ΤΩΝ ΣΚΟΠΙΩΝ
   subtitle: ΣΥΛΛΟΓΗ ΕΓΓΡΑΦΩΝ (1934-1992)
-  dewey: 938.692 ΕΠΕ
+  dewey: 938.692 ΧΣ
   entry_numbers:
   - '3033'
   editor: Ι.Μ.Χ.Α // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1993
   pages: 72
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -139921,15 +139920,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2759
     1: Χ.Σ
     2: Η ΕΠΕΚΤΑΤΙΚΗ ΠΟΛΙΤΙΚΗ ΤΩΝ ΣΚΟΠΙΩΝ
     3: ΣΥΛΛΟΓΗ ΕΓΓΡΑΦΩΝ (1934-1992)
-    4: 938.692ΕΠΕ
+    4: 938.692Χ.Σ
     5: '3033'
     8: Ι.Μ.Χ.Α
     9: ΘΕΣ/ΝΙΚΗ
     10: '1993'
     11: 72Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΟΠΙΑ
     13: ΣΚΟΠΙΑ-ΠΟΛΙΤΙΚΗ
@@ -140311,15 +140310,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2767
   authors: []
   title: ΗΠΕΙΡΟΣ ΚΟΙΝΩΝΙΑ-ΟΙΚΟΝΟΜΙΑ 15ΟΣ-20ΟΣ ΑΙΩΝΑΣ
-  dewey: 938.408 ΔΙΕ
+  dewey: 938.408 ΧΣ
   entry_numbers:
   - '2158'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1987
   pages: 370
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -140329,15 +140328,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2767
     1: Χ.Σ
     2: ΗΠΕΙΡΟΣ ΚΟΙΝΩΝΙΑ-ΟΙΚΟΝΟΜΙΑ 15ΟΣ-20ΟΣ ΑΙΩΝΑΣ
-    4: 938.408ΔΙΕ
+    4: 938.408Χ.Σ
     5: '2158'
     9: ΓΙΑΝΝΙΝΑ
     10: '1987'
     11: 370Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΠΡΑΚΤΙΚΑ
     13: ΗΠΕΙΡΟΣ-ΠΡΑΚΤΙΚΑ
     14: ΠΡΑΚΤΙΚΑ ΔΙΕΘΝΟΥΣ ΣΥΝΕΔΡΙΟΥ
@@ -147232,15 +147231,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2905
     1: ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜ
     2: Η ΚΑΤΑ ΤΩΝ ΡΩΜΑΙΩΝ ΕΚΣΤΡΑΤΕΙΑ ΤΟΥ ΑΝΤΙΟΧΟΥ ΤΟΥ Γ'ΕΙΣ ΤΗΝ
     3: ΕΛΛΑΔΑ
-    4: 938.19 ΒΡΑ
+    4: 938.19ΒΡΑ
     5: '4174'
     8: ΣΠΑΝΟΠΟΥΛΟΥ
     9: ΑΘΗΝΑ
     10: '1974'
     11: 107Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΜΑΙΟΙ
     13: ΡΡΩΜΑΙΟΙ-ΑΝΤΙΟΧΙΟΣ Γ'
@@ -232547,17 +232546,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4653
   authors:
-  - ΡΙΤΣΙ,ΡΙΤΑ
+  - RITCHIE,RITA
   title: ΤΑ ΧΡΥΣΑ ΓΕΡΑΚΙΑ ΤΟΥ ΤΖΕΝΓΚΙΣ ΧΑΝ
-  dewey: 808.899 ΡΙΤ
+  dewey: 808.899 RIT
   entry_numbers:
   - '4792'
   translators:
   - ΜΠΑΡΤΖΙΝΟΠΟΥΛΟΣ,ΕΡΡ.
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 1993
   pages: 187
@@ -232565,17 +232564,17 @@
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4653
-    1: ΡΙΤΣΙ,ΡΙΤΑ
+    1: RITCHIE,RITA
     2: ΤΑ ΧΡΥΣΑ ΓΕΡΑΚΙΑ ΤΟΥ ΤΖΕΝΓΚΙΣ ΧΑΝ
-    4: 808.899ΡΙΤ
+    4: 808.899RIT
     5: '4792'
     6: ΕΡΡ.ΜΠΑΡΤΖΙΝΟΠΟΥΛΟΣ
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '1993'
     11: 187Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -233090,50 +233089,47 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4664
   authors:
-  - ΝΤΑΓΛΑΣ,Λ.
-  title: Ο ΧΙΤΩΝ
-  dewey: 808.899 ΝΤΑ
+  - ΠΕΛΩ,ΠΙΕΡ
+  title: ΤΟ ΠΑΙΔΙ ΚΑΙ ΤΟ ΑΣΤΕΡΙ
+  dewey: 808.899 ΠΕΛ
   entry_numbers:
-  - '6665'
-  translators:
-  - ΨΑΡΡΑ,ΜΑΡ.
-  editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
-  edition_year: 1971
-  pages: 189
+  - '20651'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 1979
+  pages: 160
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
-  copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4664
-    1: ΝΤΑΓΛΑΣ,Λ.
-    2: Ο ΧΙΤΩΝ
-    4: 808.899ΝΤΑ
-    5: '6665'
-    6: ΜΑΡ.ΨΑΡΡΑ
-    8: ΑΓΚΥΡΑ
+    1: ΠΕΛΩ,ΠΙΕΡ
+    2: ΤΟ ΠΑΙΔΙ ΚΑΙ ΤΟ ΑΣΤΕΡΙ
+    4: 808.899ΠΕΛ
+    5: '20651'
+    8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
-    10: '1971'
-    11: 189Σ
+    10: '1979'
+    11: '160'
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
-    17: 2 ΑΝΤΙΤΥΠΑ
     3: null
+    6: null
     7: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
@@ -233143,15 +233139,14 @@
     28: null
     29: null
     30: null
 - dbase_number: 4665
   authors:
   - ΚΡΟΝΙΝ,Α
   title: ΤΑ ΑΓΟΥΡΑ ΧΡΟΝΙΑ
-  dewey: 823 ΚΡΟ
   entry_numbers:
   - '6666'
   - '9596'
   - '20585'
   translators:
   - ΜΑΥΡΟΕΙΔΗ-ΠΑΠΑΔΑΚΗ,ΣΟΦΙΑ
   editor: ΑΣΤΗΡ // ΑΘΗΝΑ
@@ -233163,15 +233158,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4665
     1: ΚΡΟΝΙΝ,Α
     2: ΤΑ ΑΓΟΥΡΑ ΧΡΟΝΙΑ
-    4: 823ΚΡΟ
+    4: 8Ο8.899ΚΡΟ
     5: 6666,9596,20585
     6: ΠΑΠΑΔΑΚΗ-ΜΑΥΡΟΕΙΔΗ,Σ
     8: ΑΣΤΗΡ
     9: ΑΘΗΝΑ
     10: '1978'
     11: 320Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
@@ -276336,29 +276331,29 @@
     28: null
     29: null
     30: null
 - dbase_number: 5571
   authors:
   - ΝΙΚΟΡΕΤΖΟΣ,ΔΗΜΗΤΡΗΣ
   title: ΛΟΓΙΑ ΤΗΣ ΚΑΡΔΙΑΣ
-  dewey: 880.09 ΝΙΚ
+  dewey: 808.899 ΝΙΚ
   entry_numbers:
   - '6690'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   pages: 60
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 5571
     1: ΝΙΚΟΡΕΤΖΟΣ,ΔΗΜΗΤΡΗΣ
     2: ΛΟΓΙΑ ΤΗΣ ΚΑΡΔΙΑΣ
-    4: 880.09ΝΙΚ
+    4: 808.899ΝΙΚ
     5: '6690'
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     11: 60Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -280740,47 +280735,47 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5659
   authors:
-  - DOUGLAS,L.
+  - ΝΤΑΓΚΛΑΣ,ΛΟΥΔ
   title: Ο ΧΙΤΩΝ
-  dewey: 889 DOU
+  dewey: 808.899 ΝΤΑ
   entry_numbers:
-  - '6999'
+  - 6999,6665
   translators:
   - ΛΑΜΨΑΣ,ΓΙΑΝΝΗΣ
   edition: '2'
   editor: ΔΑΜΑΣΚΟΣ // ΑΘΗΝΑ
   edition_year: 1950
   pages: 438
   topics:
-  - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   donors:
   - ΓΩΓΟΣ,
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 5659
-    1: DOUGLAS,L.
+    1: ΝΤΑΓΚΛΑΣ,ΛΟΥΔ
     2: Ο ΧΙΤΩΝ
-    4: 889DOU
-    5: '6999'
+    4: 808.899ΝΤΑ
+    5: 6999,6665
     6: ΓΙΑΝΝΗ ΛΑΜΨΑ
     7: 2η
     8: ΔΑΜΑΣΚΟΣ
     9: ΑΘΗΝΑ
     10: '1950'
     11: 438Σ
-    12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
-    13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
-    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΓΩΓΟΥ
     3: null
     15: null
     16: null
     18: null
     19: null
     20: null
@@ -307870,15 +307865,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6209
   authors: []
   title: ΘΡΑΚΗ 80 ΧΡΟΝΙΑ ΑΠΟ ΤΗΝ ΕΝΣΩΜΑΤΩΣΗ
-  dewey: 938.695 ΘΡΑ
+  dewey: 938.695 ΧΣ
   entry_numbers:
   - '8078'
   - '6857'
   editor: ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 24
   topics:
@@ -307889,15 +307884,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6209
     1: Χ.Σ
     2: ΘΡΑΚΗ 80 ΧΡΟΝΙΑ ΑΠΟ ΤΗΝ ΕΝΣΩΜΑΤΩΣΗ
-    4: 938.695ΘΡΑ
+    4: 938.695Χ.Σ
     5: 8078-6857-
     8: ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 24Σ
     12: ΘΡΑΚΗ-ΕΝΣΩΜΑΤΩΣΗ
     13: ΕΝΣΩΜΑΤΩΣΗ-ΘΡΑΚΗ
@@ -310145,15 +310140,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6256
   authors: []
   title: ΓΙΑΝΝΙΝΑ-ΗΠΕΙΡΟΣ 19ος-20ος ΑΙΩΝΑΣ
-  dewey: '938.939'
+  dewey: 938.939 ΧΣ
   entry_numbers:
   - '8164'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1993
   pages: 341
   topics:
   - ΓΙΑΝΝΕΝΑ
@@ -310162,15 +310157,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6256
     1: Χ.Σ
     2: ΓΙΑΝΝΙΝΑ-ΗΠΕΙΡΟΣ 19ος-20ος ΑΙΩΝΑΣ
-    4: '938.939'
+    4: 938.939Χ.Σ
     5: '8164'
     9: ΓΙΑΝΝΙΝΑ
     10: '1993'
     11: 341Σ
     12: ΓΙΑΝΝΙΝΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΠΟΛΙΤΙΣΜΟΣ
     14: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
@@ -322637,15 +322632,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6515
     1: ΜΠΟΡΟΒΣΚΙ,ΤΑΝΤΕΟΥΣ
     2: ΑΠΟ ΔΩ ΓΙΑ ΤΑ ΑΕΡΙΑ ΚΥΡΙΕΣ ΚΑΙ ΚΥΡΙΟΙ
-    4: 938.87ΜΠΟ8
+    4: 938.87ΜΠΟ
     5: '8645'
     8: ΣΤΟΧΑΣΤΗΣ
     9: ΑΘΗΝΑ
     10: '1981'
     11: 149Σ
     12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -325684,34 +325679,34 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6579
   authors:
-  - ΤΟΥΡΑΤΣΟΓΛΟΥ ΙΩΑΝΝΗΣ
+  - ΤΟΥΡΑΤΣΟΓΛΟΥ,ΙΩΑΝΝΗΣ
   title: ΜΑΚΕΔΟΝΙΑ
   subtitle: ΙΣΤΟΡΙΑ ΜΝΗΜΕΙΑ ΜΟΥΣΕΙΑ
-  dewey: 398.666 ΤΟΥ
+  dewey: 938.666 ΤΟΥ
   entry_numbers:
   - 9298Α
   editor: ΕΚΔΟΤΙΚΗ ΑΘΗΝΩΝ // ΑΘΗΝΑ
   edition_year: 1996
   pages: 459
   topics:
   - ΜΑΚΕΔΟΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6579
-    1: ΤΟΥΡΑΤΣΟΓΛΟΥ ΙΩΑΝΝΗΣ
+    1: ΤΟΥΡΑΤΣΟΓΛΟΥ,ΙΩΑΝΝΗΣ
     2: ΜΑΚΕΔΟΝΙΑ
     3: ΙΣΤΟΡΙΑ ΜΝΗΜΕΙΑ ΜΟΥΣΕΙΑ
-    4: 398.666ΤΟΥ
+    4: 938.666ΤΟΥ
     5: 9298Α
     8: ΕΚΔΟΤΙΚΗ ΑΘΗΝΩΝ
     9: ΑΘΗΝΑ
     10: '1996'
     11: 459Σ
     12: ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΑ
@@ -326478,44 +326473,46 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6596
   authors: []
-  title: ΠΕΡΙ ΠΕΤΡΟΓΕΦΥΡΩΝ...
+  title: ΟΠΛΑΡΧΗΓΟΥ ΑΠΟΣΤΟΛΟΥ Γ. ΠΑΠΑΚΩΣΤΑ
+  subtitle: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
+  dewey: 938.764 ΠΑΠ
   entry_numbers:
-  - '8656'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 2003
-  pages: 229
-  topics: []
-  notes: ΠΡΑΚΤΙΚΑ
+  - '7863'
+  pages: 474
+  topics:
+  - ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
+  - ΠΑΠΑΚΩΣΤΑΣ ΑΠΟΣΤΟΛΟΣ
+  - ΟΠΛΑΡΧΗΓΟΙ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6596
     1: Χ.Σ
-    2: ΠΕΡΙ ΠΕΤΡΟΓΕΦΥΡΩΝ...
-    5: '8656'
-    9: ΑΘΗΝΑ
-    10: '2003'
-    11: 229Σ
-    17: ΠΡΑΚΤΙΚΑ
-    3: null
-    4: null
+    2: ΟΠΛΑΡΧΗΓΟΥ ΑΠΟΣΤΟΛΟΥ Γ. ΠΑΠΑΚΩΣΤΑ
+    3: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
+    4: 938.764ΠΑΠ
+    5: '7863'
+    11: '474'
+    12: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
+    13: ΠΑΠΑΚΩΣΤΑΣ ΑΠΟΣΤΟΛΟΣ
+    14: ΟΠΛΑΡΧΗΓΟΣ
     6: null
     7: null
     8: null
-    12: null
-    13: null
-    14: null
+    9: null
+    10: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
@@ -332951,15 +332948,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6730
   authors: []
   title: ΡΗΓΑΣ ΓΙΑ ΜΙΑ ΝΕΑ ΕΡΕΥΝΗΤΙΚΗ ΣΥΓΚΟΜΙΔΗ
-  dewey: 949.483 ΡΗΓ
+  dewey: 938.483 ΧΣ
   entry_numbers:
   - '6822'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1998
   pages: 92
   topics:
   - ΣΥΝΕΔΡΙΟ
@@ -332970,15 +332967,15 @@
   has_cd: false
   has_dvd: false
   offprint: true
   original_entry:
     0: 6730
     1: Χ.Σ.
     2: ΡΗΓΑΣ ΓΙΑ ΜΙΑ ΝΕΑ ΕΡΕΥΝΗΤΙΚΗ ΣΥΓΚΟΜΙΔΗ
-    4: 949.483ΡΗΓ
+    4: 938.483Χ.Σ
     5: '6822'
     9: ΙΩΑΝΝΙΝΑ
     10: '1998'
     11: 92Σ
     12: ΣΥΝΕΔΡΙΟ-ΡΗΓΑΣ
     13: ΣΥΝΕΔΡΙΟ-ΡΗΓΑΣ
     14: ΣΥΝΕΔΡΙΟ-ΡΗΓΑΣ
@@ -333049,30 +333046,30 @@
     28: null
     29: null
     30: null
 - dbase_number: 6732
   authors:
   - ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΛΗΣ
   title: ΦΥΣΙΚΗΣ ΑΠΑΝΘΙΣΜΑ
-  dewey: 949.483 ΒΕΛ
+  dewey: 938.483 ΧΣ
   entry_numbers:
   - '6828'
   editor: ΦΕΡΡΩΝ-ΒΕΛΕΣΤΙΝΟΥ-ΡΗ // ΑΘΗΝΑ
   edition_year: 1991
   pages: 200
   topics:
   - ΕΘΝΙΚΟ ΔΙΑΦΩΤΙΣΤΙΚΟ ΕΡΓΟ ΡΗΓΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6732
     1: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΛΗΣ
     2: ΦΥΣΙΚΗΣ ΑΠΑΝΘΙΣΜΑ
-    4: 949.483ΒΕΛ
+    4: 938.483Χ.Σ
     5: '6828'
     8: ΦΕΡΡΩΝ-ΒΕΛΕΣΤΙΝΟΥ-ΡΗ
     9: ΑΘΗΝΑ
     10: '1991'
     11: 200Σ
     12: ΕΘΝΙΚΟ ΔΙΑΦΩΤΙΣΤΙΚΟ ΕΡΓΟ ΡΗΓΑ
     13: ΕΘΝΙΚΟ ΔΙΑΦΩΤΙΣΤΙΚΟ ΕΡΓΟ ΡΗΓΑ
@@ -333096,15 +333093,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 6733
   authors: []
   title: ΡΗΓΑ ΒΕΛΕΣΤΙΝΛΗ
   subtitle: ΑΠΑΝΘΙΣΜΑ ΚΕΙΜΕΝΩΝ
-  dewey: 949.483 ΡΗΓ
+  dewey: 938.483 ΧΣ
   entry_numbers:
   - '6860'
   editor: None // ΑΘΗΝΑ
   edition_year: 1998
   pages: 158
   topics:
   - ΕΠΙΛΟΓΗ ΚΕΙΜΕΝΩΝ ΡΗΓΑ
@@ -333112,15 +333109,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 6733
     1: Χ.Σ.
     2: ΡΗΓΑ ΒΕΛΕΣΤΙΝΛΗ
     3: ΑΠΑΝΘΙΣΜΑ ΚΕΙΜΕΝΩΝ
-    4: 949.483ΡΗΓ
+    4: 938.483Χ.Σ
     5: '6860'
     9: ΑΘΗΝΑ
     10: '1998'
     11: 158Σ
     12: ΕΠΙΛΟΓΗ ΚΕΙΜΕΝΩΝ ΡΗΓΑ
     13: ΕΠΙΛΟΓΗ ΚΕΙΜΕΝΩΝ ΡΗΓΑ
     14: ΕΠΙΛΟΓΗ ΚΕΙΜΕΝΩΝ ΡΗΓΑ
@@ -334094,15 +334091,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 6754
   authors:
   - ΒΟΥΡΝΑΣ,ΤΑΣΟΣ
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΩΤΕΡΗΣ ΚΑΙ ΣΥΓΧΡΟΝΗΣ ΕΛΛΑΔΑΣ
-  dewey: 949.597 ΒΟΥ
+  dewey: 949.7 ΒΟΥ
   entry_numbers:
   - '8884'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 1999
   pages: 621
   topics:
   - ΝΕΩΤΕΡΗ
@@ -334112,15 +334109,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6754
     1: ΒΟΥΡΝΑΣ,ΤΑΣΟΣ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΩΤΕΡΗΣ ΚΑΙ ΣΥΓΧΡΟΝΗΣ ΕΛΛΑΔΑΣ
-    4: 949.597ΒΟΥ
+    4: 949.7ΒΟΥ
     5: '8884'
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '1999'
     11: 621Σ
     12: ΙΣΤΟΡΙΑ-ΝΕΩΤΕΡΗ-ΣΥΓΧΡΟΝΗ ΕΛΛΑΔΑ
     13: ΙΣΤΟΡΙΑ-ΝΕΩΤΕΡΗ ΣΥΓΧΡΟΝΗ ΕΛΛΑΔΑ
@@ -335345,15 +335342,15 @@
     29: null
     30: null
 - dbase_number: 6780
   authors:
   - ΑΘΑΝΑΣΙΟΥ,ΘΕΟΦΙΛΟΣ
   title: ΗΜΟΥΝΑ ΚΙ ΕΓΩ ΕΚΕΙ
   subtitle: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
-  dewey: 938.764 ΑΘΑ
+  dewey: 920 ΑΘΑ
   entry_numbers:
   - '8804'
   editor: None // ΑΘΗΝΑ
   edition_year: 2005
   pages: 286
   topics:
   - ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
@@ -335361,15 +335358,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 6780
     1: ΑΘΑΝΑΣΙΟΥ,ΘΕΟΦΙΛΟΣ
     2: ΗΜΟΥΝΑ ΚΙ ΕΓΩ ΕΚΕΙ
     3: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
-    4: 938.764ΑΘΑ
+    4: 920ΑΘΑ
     5: '8804'
     9: ΑΘΗΝΑ
     10: '2005'
     11: 286Σ
     12: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
     13: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
     14: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
@@ -336679,15 +336676,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 6808
   authors:
   - NICOL,DONALD
   title: ΒΙΟΓΡΑΦΙΚΟ ΛΕΞΙΚΟ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
-  dewey: 998.301 NIC
+  dewey: 938.301 NIC
   entry_numbers:
   - '8951'
   editor: ΕΛΛΗΝΙΚΗ ΕΥΡΩΕΚΔΟΤΙΚ // ΑΘΗΝΑ
   edition_year: 1993
   pages: 350
   topics:
   - ΒΙΟΓΡΑΦΙΚΟ ΛΕΞΙΚΟ
@@ -336695,15 +336692,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6808
     1: NICOL,DONALD
     2: ΒΙΟΓΡΑΦΙΚΟ ΛΕΞΙΚΟ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
-    4: 998.301NIC
+    4: 938.301NIC
     5: '8951'
     8: ΕΛΛΗΝΙΚΗ ΕΥΡΩΕΚΔΟΤΙΚ
     9: ΑΘΗΝΑ
     10: '1993'
     11: 350Σ
     12: ΒΙΟΓΡΑΦΙΚΟ ΛΕΞΙΚΟ-ΒΥΖΑΝΤΙΝΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
     13: ΒΥΖΑΝΤΙΝΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΚΟ ΛΕΞΙΚΟ
@@ -337156,32 +337153,33 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6818
   authors: []
   title: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ ΜΑΚΡΥΓΙΑΝΝΗ
-  dewey: 920.008 ΜΑΚ
+  dewey: 938.478 ΧΣ
   entry_numbers:
   - '8936'
+  - '98'
   editor: None // ΑΘΗΝΑ
   edition_year: 1995
   pages: 221
   topics:
   - ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
   - ΜΑΚΡΥΓΙΑΝΝΗΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6818
     1: Χ.Σ
     2: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ ΜΑΚΡΥΓΙΑΝΝΗ
-    4: 920.008ΜΑΚ
-    5: '8936'
+    4: 938.478Χ.Σ
+    5: 8936-98
     9: ΑΘΗΝΑ
     10: '1995'
     11: 221Σ
     12: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ-ΜΑΚΡΥΓΙΑΝΝΗΣ
     13: ΜΑΚΡΥΓΙΑΝΝΗΣ-ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
     14: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
     15: ΜΑΚΡΥΓΙΑΝΝΗΣ
@@ -337348,49 +337346,49 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6822
   authors:
-  - ΚΑΡΑΤΖΕΝΗΣ,ΔΗΜΗΤΡΙΟΣ
-  title: ΠΟΛΙΤΙΚΕΣ ΠΡΟΣΩΠΙΚΟΤΗΤΕΣ ΝΟΜΟΥ ΑΡΤΗΑΣ
-  subtitle: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ ΔΗΜΑΡΧΟΣ-ΒΟΥΛΕΥΤΗΣ
-  dewey: 920 ΚΑΡ
+  - ΤΟΥΝΤΑ ΧΑΤΖΟΥΔΗ,ΕΛΕΝΗ
+  title: ΤΑΞΙΔΕΥΟΝΤΑΣ ΑΠΟ ΤΗΝ ΑΘΗΝΑ ΣΤΟ ΜΠΙΖΑΝΙ
+  dewey: 938.93 ΤΟΥ
   entry_numbers:
-  - '8942'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1983
-  pages: 125
+  - '22935'
+  editor: None // ΙΩΑΝΝΙΝΑ
+  edition_year: 2012
+  pages: 345
   topics:
-  - ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ
+  - ΜΠΙΖΑΝΙ
   has_cd: false
   has_dvd: false
   offprint: false
+  ean: '9789609897693'
   original_entry:
     0: 6822
-    1: ΚΑΡΑΤΖΕΝΗΣ,ΔΗΜΗΤΡΙΟΣ
-    2: ΠΟΛΙΤΙΚΕΣ ΠΡΟΣΩΠΙΚΟΤΗΤΕΣ ΝΟΜΟΥ ΑΡΤΗΑΣ
-    3: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ ΔΗΜΑΡΧΟΣ-ΒΟΥΛΕΥΤΗΣ
-    4: 920ΚΑΡ
-    5: '8942'
-    9: ΑΘΗΝΑ
-    10: '1983'
-    11: 125Σ
-    12: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ
-    13: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ
-    14: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ
+    1: ΤΟΥΝΤΑ ΧΑΤΖΟΥΔΗ,ΕΛΕΝΗ
+    2: ΤΑΞΙΔΕΥΟΝΤΑΣ ΑΠΟ ΤΗΝ ΑΘΗΝΑ ΣΤΟ ΜΠΙΖΑΝΙ
+    4: 938.93ΤΟΥ
+    5: '22935'
+    9: ΙΩΑΝΝΙΝΑ
+    10: '2012'
+    11: 345Σ
+    12: ΙΣΤΟΡΙΑ-ΜΠΙΖΑΝΙ
+    13: ΜΠΙΖΑΝΙ
+    14: ΙΣΤΟΡΙΑ
+    18: '9789609897'
+    19: '693'
+    3: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
-    18: null
-    19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
@@ -341408,30 +341406,30 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6906
   authors: []
   title: ΚΥΠΡΟΣ Η ΛΕΗΛΑΣΙΑ ΕΝΟΣ ΠΟΛΙΤΙΣΜΟΥ
-  dewey: 938.497 ΚΥΠ
+  dewey: 938.497 ΧΣ
   entry_numbers:
   - '6879'
   editor: ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 237
   topics:
   - ΚΥΠΡΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6906
     1: Χ.Σ.
     2: ΚΥΠΡΟΣ Η ΛΕΗΛΑΣΙΑ ΕΝΟΣ ΠΟΛΙΤΙΣΜΟΥ
-    4: 938.497ΚΥΠ
+    4: 938.497Χ.Σ
     5: '6879'
     8: ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 237Σ
     12: ΚΥΠΡΟΣ
     13: ΚΥΠΡΟΣ
@@ -342193,30 +342191,30 @@
     28: null
     29: null
     30: null
 - dbase_number: 6922
   authors:
   - ΚΑΡΑΘΑΝΑΣΗ,ΑΘΑΝΑΣΙΟ
   title: ΚΑΠΠΑΔΟΚΙΑΣ ΤΥΧΑΙ
-  dewey: 938.498 ΚΑΡ
+  dewey: 938.392 ΚΑΡ
   entry_numbers:
   - '6823'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2000
   pages: 109
   topics:
   - ΚΑΠΠΑΔΟΚΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6922
     1: ΚΑΡΑΘΑΝΑΣΗ,ΑΘΑΝΑΣΙΟ
     2: ΚΑΠΠΑΔΟΚΙΑΣ ΤΥΧΑΙ
-    4: 938.498ΚΑΡ
+    4: 938.392ΚΑΡ
     5: '6823'
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2000'
     11: 109Σ
     12: ΚΑΠΠΑΔΟΚΙΑ
     13: ΚΑΠΠΑΔΟΚΙΑ
     14: ΚΑΠΠΑΔΟΚΙΑ
@@ -342244,15 +342242,14 @@
   authors:
   - MURAT,JOHN
   title: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
   subtitle: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
   dewey: 938.498 ΜΟΥ
   entry_numbers:
   - '5363'
-  - '1950'
   editor: None // ΑΘΗΝΑ
   edition_year: 1982
   pages: 542
   topics:
   - ΕΛΛΗΝΙΣΜΟΣ
   copies: 2
   has_cd: false
@@ -342260,15 +342257,15 @@
   offprint: false
   original_entry:
     0: 6923
     1: MURAT,JOHN
     2: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
     3: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
     4: 938.498ΜΟΥ
-    5: 5363-1950
+    5: '5363'
     9: ΑΘΗΝΑ
     10: '1982'
     11: 542Σ
     12: ΕΛΛΗΝΙΣΜΟΣ
     13: ΕΛΛΗΝΙΣΜΟΣ
     14: ΕΛΛΗΝΙΣΜΟΣ
     17: 2 ANTITYΠΑ
@@ -344456,14 +344453,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 6969
   authors:
   - ΣΤΑΜΑΤΗΣ,ΕΛΕΥΘΕΡΙΟΣ
   title: ΚΥΡΙΟΙ, ΠΑΤΕ ΓΙΑ ΥΠΝΟ
+  dewey: 938.799 ΣΤΑ
   entry_numbers:
   - '9011'
   editor: ΔΟΥΡΕΙΟΣ ΙΠΠΟΣ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 298
   topics:
   - ΤΡΑΓΩΔΙΑ ΚΥΠΡΟΥ
@@ -344472,24 +344470,24 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6969
     1: ΣΤΑΜΑΤΗΣ,ΕΛΕΥΘΕΡΙΟΣ
     2: ΚΥΡΙΟΙ, ΠΑΤΕ ΓΙΑ ΥΠΝΟ
+    4: 938.799ΣΤΑ
     5: '9011'
     8: ΔΟΥΡΕΙΟΣ ΙΠΠΟΣ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 298Σ
     12: ΤΡΑΓΩΔΙΑΚΥΠΡΟΥ
     13: ΤΡΑΓΩΔΙΑ-ΚΥΠΡΟΣ
     14: ΚΥΠΡΟΣ
     3: null
-    4: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -345877,15 +345875,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 6998
   authors:
   - ΛΑΜΠΡΗ,Π.ΠΑΝΑΓΙΩΤΑ
   title: ΡΟΔΑΥΓΗ
-  subtitle: ΤΟ ΡΟΔΟ ΤΗΣ ΑΥΓΗΣ
+  subtitle: ΤΟ ΡΟΔΟ ΤΗΣ ΑΥΓΗΣ                                          Τ
   dewey: 938.939 ΛΑΜ
   entry_numbers:
   - '9037'
   editor: ΤΑΧΥΤΥΠΟ // None
   edition_year: 2006
   pages: 495
   topics:
@@ -345895,16 +345893,16 @@
   has_dvd: false
   offprint: false
   isbn: '9606311821'
   original_entry:
     0: 6998
     1: ΛΑΜΠΡΗ,Π.ΠΑΝΑΓΙΩΤΑ
     2: ΡΟΔΑΥΓΗ
-    3: ΤΟ ΡΟΔΟ ΤΗΣ ΑΥΓΗΣ
-    4: ' 938939ΛΑΜ'
+    3: ΤΟ ΡΟΔΟ ΤΗΣ ΑΥΓΗΣ                                          Τ
+    4: 938.939ΛΑΜ
     5: '9037'
     8: ΤΑΧΥΤΥΠΟ
     10: '2006'
     11: 495Σ
     12: ΛΑΟΓΡΑΦΙΑ-ΡΟΔΑΥΓΗ
     13: ΡΟΔΑΥΓΗ-ΛΑΟΓΡΑΦΙΑ
     14: ΡΟΔΑΥΓΗ
@@ -355720,14 +355718,15 @@
     29: null
     30: null
 - dbase_number: 7197
   authors:
   - MANFREDI,VALERIO MASSIMO
   title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   subtitle: Ο ΓΙΟΣ ΤΟΥ ΟΝΕΙΡΟΥ
+  dewey: 938.174 MAN
   entry_numbers:
   - '9255'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 1999
   pages: 224
   topics:
   - ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
@@ -355737,26 +355736,26 @@
   offprint: false
   isbn: 960-14-0056-7
   original_entry:
     0: 7197
     1: MANFREDI,VALERIO MASSIMO
     2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     3: Ο ΓΙΟΣ ΤΟΥ ΟΝΕΙΡΟΥ
+    4: 938.174MAN
     5: '9255'
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '1999'
     11: 224Σ
     12: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     14: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     17: 2 ΤΟΜΟΙ
     18: 960-14-005
     19: 6-7
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -355769,14 +355768,15 @@
     29: null
     30: null
 - dbase_number: 7198
   authors:
   - MANFREDI,VALERIO MASSIMO
   title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   subtitle: Η ΑΜΜΟΣ ΤΟΥ ΑΜΜΩΝΑ
+  dewey: 938.174 MAN
   entry_numbers:
   - '9256'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 1999
   pages: 439
   topics:
   - ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
@@ -355785,26 +355785,26 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7198
     1: MANFREDI,VALERIO MASSIMO
     2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     3: Η ΑΜΜΟΣ ΤΟΥ ΑΜΜΩΝΑ
+    4: 938.174MAN
     5: '9256'
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '1999'
     11: 439Σ
     12: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     14: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     17: 2 ΤΟΜΟΙ
     18: 960-14-012
     19: 7-Χ
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -355817,14 +355817,15 @@
     29: null
     30: null
 - dbase_number: 7199
   authors:
   - MANFREDI,VALERIO MASSIMO
   title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   subtitle: ΤΑ ΠΕΡΑΤΑ ΤΟΥ ΚΟΣΜΟΥ
+  dewey: 938.174 MAN
   entry_numbers:
   - '9257'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 515
   topics:
   - ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
@@ -355834,26 +355835,26 @@
   offprint: false
   isbn: 960-14-0177-6
   original_entry:
     0: 7199
     1: MANFREDI,VALERIO MASSIMO
     2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     3: ΤΑ ΠΕΡΑΤΑ ΤΟΥ ΚΟΣΜΟΥ
+    4: 938.174MAN
     5: '9257'
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 515Σ
     12: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     14: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     17: 2 ΤΟΜΟΙ
     18: 960-14-017
     19: 7-6
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -356404,14 +356405,15 @@
     29: null
     30: null
 - dbase_number: 7211
   authors:
   - IRVING,DAVID
   title: Ο ΠΟΛΕΜΟΣ ΤΩΝ ΣΤΡΑΤΗΓΩΝ
   subtitle: ΣΤΑ ΕΝΔΟΤΕΡΑ ΤΩΝ ΣΥΜΜΑΧΙΚΩΝ ΔΥΝΑΜΕΩΝ 1944-1945
+  dewey: 938.764 IRV
   entry_numbers:
   - '9169'
   translators:
   - ΧΟΥΡΜΟΥΖΙΑΔΗΣ,ΣΤΕΛΙΟΣ
   editor: ΙΩΛΚΟΣ // ΑΘΗΝΑ
   edition_year: 2005
   pages: 655
@@ -356425,27 +356427,27 @@
   offprint: false
   isbn: 960-426-390-0
   original_entry:
     0: 7211
     1: IRVING,DAVID
     2: Ο ΠΟΛΕΜΟΣ ΤΩΝ ΣΤΡΑΤΗΓΩΝ
     3: ΣΤΑ ΕΝΔΟΤΕΡΑ ΤΩΝ ΣΥΜΜΑΧΙΚΩΝ ΔΥΝΑΜΕΩΝ 1944-1945
+    4: 938.764IRV
     5: '9169'
     6: ΣΤΕΛΙΟΣ ΧΟΥΡΜΟΥΖΙΑΔΗ
     8: ΙΩΛΚΟΣ
     9: ΑΘΗΝΑ
     10: '2005'
     11: 655Σ
     12: ΠΟΛΕΜΟΣ ΣΤΡΑΤΗΓΩΝ
     13: ΣΤΡΑΤΗΓΩΝ ΠΟΛΕΜΟΣ
     14: ΠΟΛΕΜΟΣ
     15: ΣΤΡΑΤΗΓΟΙ
     18: 960-426-39
     19: 0-0
-    4: null
     7: null
     16: null
     17: null
     20: null
     21: null
     22: null
     23: null
@@ -357584,14 +357586,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 7235
   authors:
   - ΧΟΥΤΑ,ΣΤΥΛΙΑΝΟΥ
   title: Η ΜΑΧΗ ΤΟΥ ΜΑΚΡΥΝΟΡΟΥΣ (14-22 ΙΟΥΛΙΟΥ 1943)
+  dewey: 938.765 ΧΟΥ
   entry_numbers:
   - '9183'
   editor: ΣΙΔΕΡΗΣ // ΑΘΗΝΑ
   edition_year: 1983
   pages: 83
   topics:
   - ΜΑΚΡΥΝΟΡΟΣ
@@ -357599,24 +357602,24 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7235
     1: ΧΟΥΤΑ,ΣΤΥΛΙΑΝΟΥ
     2: Η ΜΑΧΗ ΤΟΥ ΜΑΚΡΥΝΟΡΟΥΣ (14-22 ΙΟΥΛΙΟΥ 1943)
+    4: 938.765ΧΟΥ
     5: '9183'
     8: ΣΙΔΕΡΗΣ
     9: ΑΘΗΝΑ
     10: '1983'
     11: 83Σ
     12: ΜΑΚΡΥΝΟΡΟΣ
     13: ΜΑΧΗ ΜΑΚΡΥΝΟΡΟΣ
     14: ΜΑΚΡΥΝΟΡΟΣ
     3: null
-    4: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -357646,15 +357649,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7236
     1: ΣΑΡΑΝΤΗ,ΘΕΟΔΩΡΟΥ
     2: Η ΣΥΝΟΜΩΣΙΑ ΚΑΤΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
-    4: 938,695ΣΑΡ
+    4: 938.695ΣΑΡ
     5: '9182'
     9: ΑΘΗΝΑ
     10: '1984'
     11: 207Σ
     12: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΑ-ΙΣΤΟΡΙΑ
     14: ΜΑΚΕΔΟΝΙΑ
@@ -359184,15 +359187,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 7268
   authors:
   - ΚΑΜΠΦ,ΜΑΙΝ
   title: Α.ΧΙΤΛΕΡ Ο ΑΓΩΝ ΜΟΥ
-  dewey: 938.87 ΧΙΤ
+  dewey: 938.87 ΚΑΜ
   entry_numbers:
   - '9178'
   translators:
   - ΚΩΣΤΕΛΕΝΟΣ,ΔΗΜΗΤΡΗΣ
   editor: Δ.ΔΑΡΕΜΑ // ΑΘΗΝΑ
   pages: 450
   topics:
@@ -359201,15 +359204,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7268
     1: ΚΑΜΠΦ,ΜΑΙΝ
     2: Α.ΧΙΤΛΕΡ Ο ΑΓΩΝ ΜΟΥ
-    4: 938.87ΧΙΤ
+    4: 938.87ΚΑΜ
     5: '9178'
     6: ΔΗΜΗΤΡΗΣ ΚΩΣΤΕΛΕΝΟΣ
     8: Δ.ΔΑΡΕΜΑ
     9: ΑΘΗΝΑ
     11: 450Σ
     12: ΧΙΤΛΕΡ
     13: ΧΙΤΛΕΡ
@@ -359529,14 +359532,15 @@
     29: null
     30: null
 - dbase_number: 7275
   authors:
   - ΣΕΡΒΕΤΑ,ΘΕΟΦΙΛΟΥ
   title: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
   subtitle: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
+  dewey: 938 ΣΕΡ
   entry_numbers:
   - '9274'
   editor: None // ΑΘΗΝΑ
   edition_year: 2002
   pages: 137
   topics:
   - ΑΡΧΑΙΑ ΕΛΛΑΔΑ
@@ -359544,22 +359548,22 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7275
     1: ΣΕΡΒΕΤΑ,ΘΕΟΦΙΛΟΥ
     2: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
     3: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
+    4: 938ΣΕΡ
     5: '9274'
     9: ΑΘΗΝΑ
     10: '2002'
     11: 137Σ
     12: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
     13: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
     14: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
-    4: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -359576,14 +359580,15 @@
     29: null
     30: null
 - dbase_number: 7276
   authors:
   - ΣΕΡΒΕΤΑΣ,ΘΕΟΦΙΛΟΣ
   title: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
   subtitle: ΑΡΧΑΙΑ ΡΩΜΗ
+  dewey: 938 ΣΕΡ
   entry_numbers:
   - '9275'
   editor: None // ΑΘΗΝΑ
   edition_year: 2003
   pages: 130
   topics:
   - ΑΡΧΑΙΑ ΡΩΜΗ
@@ -359591,22 +359596,22 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7276
     1: ΣΕΡΒΕΤΑΣ,ΘΕΟΦΙΛΟΣ
     2: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
     3: ΑΡΧΑΙΑ ΡΩΜΗ
+    4: 938ΣΕΡ
     5: '9275'
     9: ΑΘΗΝΑ
     10: '2003'
     11: 130Σ
     12: ΑΡΧΑΙΑ ΡΩΜΗ
     13: ΑΡΧΑΙΑ ΡΩΜΗ
     14: ΑΡΧΑΙΑ ΡΩΜΗ
-    4: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -359623,14 +359628,15 @@
     29: null
     30: null
 - dbase_number: 7277
   authors:
   - ΣΕΡΒΕΤΑ,ΘΕΟΦΙΛΟΥ
   title: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
   subtitle: ΒΥΖΑΝΤΙΟ
+  dewey: 938 ΣΕΡ
   entry_numbers:
   - '9276'
   editor: None // ΑΘΗΝΑ
   edition_year: 2004
   pages: 154
   topics:
   - ΒΥΖΑΝΤΙΟ
@@ -359638,22 +359644,22 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7277
     1: ΣΕΡΒΕΤΑ,ΘΕΟΦΙΛΟΥ
     2: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
     3: ΒΥΖΑΝΤΙΟ
+    4: 938ΣΕΡ
     5: '9276'
     9: ΑΘΗΝΑ
     10: '2004'
     11: 154Σ
     12: ΒΥΖΑΝΤΙΟ
     13: ΒΥΖΑΝΤΙΟ
     14: ΒΥΖΑΝΤΙΟ
-    4: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -360593,38 +360599,40 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7297
   authors: []
   title: 1453 Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
+  dewey: 938.498 ΧΣ
   entry_numbers:
   - '9293'
+  - '12662'
   editor: NATIONAL GEOGRAPHIC // None
   pages: 127
   topics:
   - ΑΛΩΣΗ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-469-076-3
   original_entry:
     0: 7297
     1: Χ.Σ.
     2: 1453 Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
-    5: '9293'
+    4: 938.498Χ.Σ
+    5: 9293-12662
     8: NATIONAL GEOGRAPHIC
     11: 127Σ
     12: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
     13: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
     14: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
     18: 978-960-46
     19: 9-076-3
     3: null
-    4: null
     6: null
     7: null
     9: null
     10: null
     15: null
     16: null
     17: null
@@ -365741,30 +365749,30 @@
     28: null
     29: null
     30: null
 - dbase_number: 7403
   authors:
   - ΚΑΣΤΡΙΤΗ,ΝΑΤΑΣΑ
   title: Η ΕΛΛΑΔΑ ΤΟΥ 21 ΜΕ ΤΗ ΜΑΤΙΑ ΤΩΝ ΦΙΛΕΛΛΗΝΩΝ
-  dewey: 949.506 ΚΑΣ
+  dewey: 938.5 ΚΑΣ
   entry_numbers:
   - '9420'
   editor: ΙΣΤ.ΕΘΝ.ΕΤΑΙΡ.ΕΛΛΑΔΟ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 145
   topics:
   - ΦΙΛΕΛΛΗΝΕΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7403
     1: ΚΑΣΤΡΙΤΗ,ΝΑΤΑΣΑ
     2: Η ΕΛΛΑΔΑ ΤΟΥ 21 ΜΕ ΤΗ ΜΑΤΙΑ ΤΩΝ ΦΙΛΕΛΛΗΝΩΝ
-    4: 949.506ΚΑΣ
+    4: 938.5ΚΑΣ
     5: '9420'
     8: ΙΣΤ.ΕΘΝ.ΕΤΑΙΡ.ΕΛΛΑΔΟ
     9: ΑΘΗΝΑ
     10: '2006'
     11: 145ΣΕΛ
     12: ΙΣΤΟΡΙΑ-ΦΙΛΕΛΛΗΝΕΣ
     13: ΦΙΛΕΛΛΗΝΕΣ-ΙΣΤΟΡΙΑ
@@ -365982,44 +365990,45 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7408
-  authors: []
-  title: ΕΜΠΡΟΣ ΤΗΣ ΕΛΛΑΔΟΣ ΤΑ ΠΑΙΔΙΑ
-  subtitle: ΧΡΟΝΙΚΟΝ 1940-1944
-  dewey: 938.752 ΧΣ
+  authors:
+  - ΒΙΔΑΛΗΣ,ΟΡΕΣΤΗΣ
+  title: ΙΣΤΟΡΙΚΟ ΗΜΕΡΟΛΟΓΙΟ
+  subtitle: ΧΡΟΝΙΑ ΕΚΠΑΤΡΙΣΜΟΥ 1968-1975
+  dewey: 938.790 ΒΙΔ
   entry_numbers:
-  - 9295Α
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1978
-  pages: 376
+  - 4288,4292
+  editor: LIBRO // ΑΘΗΝΑ
+  edition_year: 1997
+  pages: 570
   topics:
   - ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7408
-    1: Χ.Σ.
-    2: ΕΜΠΡΟΣ ΤΗΣ ΕΛΛΑΔΟΣ ΤΑ ΠΑΙΔΙΑ
-    3: ΧΡΟΝΙΚΟΝ 1940-1944
-    4: 938.752Χ.Σ
-    5: 9295Α
+    1: ΒΙΔΑΛΗΣ,ΟΡΕΣΤΗΣ
+    2: ΙΣΤΟΡΙΚΟ ΗΜΕΡΟΛΟΓΙΟ
+    3: ΧΡΟΝΙΑ ΕΚΠΑΤΡΙΣΜΟΥ 1968-1975
+    4: 938.790ΒΙΔ
+    5: 4288,4292
+    8: LIBRO
     9: ΑΘΗΝΑ
-    10: '1978'
-    11: 376Σ
+    10: '1997'
+    11: '570'
     12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
     13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
     14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
     6: null
     7: null
-    8: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -366420,15 +366429,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 7417
   authors: []
   title: ΤΟ ΕΠΟΣ ΤΟΥ 40
   subtitle: ΛΑΙΚΗ ΕΙΚΟΝΟΓΡΑΦΙΑ
-  dewey: 938.752 Σ
+  dewey: 938.752 ΧΣ
   entry_numbers:
   - '9416'
   editor: ΙΣΤ.ΕΘΝ.ΕΤ.ΕΛΛΑΔΟΣ // ΑΘΗΝΑ
   edition_year: 1987
   pages: 217
   topics:
   - ΕΠΟΣ 40
@@ -366436,15 +366445,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7417
     1: Χ.Σ.
     2: ΤΟ ΕΠΟΣ ΤΟΥ 40
     3: ΛΑΙΚΗ ΕΙΚΟΝΟΓΡΑΦΙΑ
-    4: 938.752Σ
+    4: 938.752Χ.Σ
     5: '9416'
     8: ΙΣΤ.ΕΘΝ.ΕΤ.ΕΛΛΑΔΟΣ
     9: ΑΘΗΝΑ
     10: '1987'
     11: 217Σ
     12: ΙΣΤΟΡΙΑ-ΕΠΟΣ 40
     13: ΕΠΟΣ 40-ΙΣΤΟΡΙΑ
@@ -369693,15 +369702,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7482
   authors: []
   title: ΑΥΤΟΒΙΟΓΡΑΦΙΑ ΙΩΑΝΝΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
-  dewey: 889 ΧΣ
+  dewey: 938.571 ΧΣ
   entry_numbers:
   - '9953'
   edition: '3'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
   edition_year: 1971
   pages: 172
   topics:
@@ -369712,15 +369721,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7482
     1: Χ.Σ
     2: ΑΥΤΟΒΙΟΓΡΑΦΙΑ ΙΩΑΝΝΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
-    4: 889Χ.Σ
+    4: 938.571Χ.Σ
     5: '9953'
     7: 3Η
     8: ΓΑΛΑΞΙΑΣ
     9: ΑΘΗΝΑ
     10: '1971'
     11: 172Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΥΤΟΒΙΟΓΡΑΦΙΑ
@@ -372202,14 +372211,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 7533
   authors: []
   title: ΤΟ ΑΙΩΝΙΟΝ ΖΗΤΗΜΑ
   subtitle: ΤΟ ΑΝΑΤΟΛΙΚΟΝ ΖΗΤΗΜΑ
+  dewey: 938.652 ΧΣ
   entry_numbers:
   - '10077'
   editor: ΕΚΔΟΣΕΙΣ ΜΠΕΡΓΑΔΗ // ΑΘΗΝΑ
   pages: 262
   topics: []
   donors:
   - ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
@@ -372217,20 +372227,20 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7533
     1: Χ.Σ
     2: ΤΟ ΑΙΩΝΙΟΝ ΖΗΤΗΜΑ
     3: ΤΟ ΑΝΑΤΟΛΙΚΟΝ ΖΗΤΗΜΑ
+    4: 938.652Χ.Σ
     5: '10077'
     8: ΕΚΔΟΣΕΙΣ ΜΠΕΡΓΑΔΗ
     9: ΑΘΗΝΑ
     11: 262Σ
     17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
-    4: null
     6: null
     7: null
     10: null
     12: null
     13: null
     14: null
     15: null
@@ -376384,45 +376394,48 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7622
   authors:
-  - ΚΑΣΙΜΑΤΗΣ ΓΡΗΓΟΡΗΣ
-  title: ΠΑΙΔΕΣ ΕΛΛΗΝΩΝ ΙΤΕ
+  - ΨΗΜΜΕΝΟΥ,ΝΙΚΟΥ
+  title: ΕΡΜΗΝΕΥΤΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ
+  dewey: 199.495 ΨΗΜ
   entry_numbers:
-  - '10043'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1972
-  topics: []
-  donors:
-  - ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
+  - '21494'
+  editor: ΔΩΤΙΟΝ // ΙΩΑΝΝΙΝΑ
+  edition_year: 2019
+  pages: 100
+  topics:
+  - ΠΟΙΗΣΗ
+  - ΙΣΤΟΡΙΚΑ ΚΑΙ ΚΡΙΤΙΚΗ
+  - ΔΙΑΤΡΙΒΕΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7622
-    1: ΚΑΣΙΜΑΤΗΣ ΓΡΗΓΟΡΗΣ
-    2: ΠΑΙΔΕΣ ΕΛΛΗΝΩΝ ΙΤΕ
-    5: '10043'
-    9: ΑΘΗΝΑ
-    10: '1972'
-    17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
+    1: ΨΗΜΜΕΝΟΥ,ΝΙΚΟΥ
+    2: ΕΡΜΗΝΕΥΤΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ
+    4: 199.495ΨΗΜ
+    5: '21494'
+    8: ΔΩΤΙΟΝ
+    9: ΙΩΑΝΝΙΝΑ
+    10: '2019'
+    11: '100'
+    12: ΠΟΙΗΣΗ
+    13: ΙΣΤΟΡΙΚΑ ΚΑΙ ΚΡΙΤΙΚΗ
+    14: ΔΙΑΤΡΙΒΗ
     3: null
-    4: null
     6: null
     7: null
-    8: null
-    11: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
@@ -377226,48 +377239,49 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7640
   authors:
-  - ΡΗΓΑΣ.ΓΙΩΡΓΟΣ. ΣΚΟΥΤΕΛΑΣ
+  - ΣΚΟΥΤΕΛΑΣ,ΡΗΓΑΣ
   title: ΘΕΟΔΩΡΙΑΝΑ ΑΡΤΑΣ
-  dewey: '938.939'
+  dewey: 938.939 ΣΚΟ
   entry_numbers:
   - '10129'
   editor: None // ΑΘΗΝΑ
   edition_year: 1994
   pages: 638
   topics:
-  - ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
+  - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
+  - ΘΕΟΔΩΡΙΑΝΑ
   copies: 2
   donors:
   - ΛΙΟΝΤΟΣ,Ν.
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7640
-    1: ΡΗΓΑΣ.ΓΙΩΡΓΟΣ. ΣΚΟΥΤΕΛΑΣ
+    1: ΣΚΟΥΤΕΛΑΣ,ΡΗΓΑΣ
     2: ΘΕΟΔΩΡΙΑΝΑ ΑΡΤΑΣ
-    4: '938.939'
+    4: 938.939ΣΚΟ
     5: '10129'
     9: ΑΘΗΝΑ
     10: '1994'
     11: 638Σ
-    12: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
-    13: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
+    12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
+    13: ΘΕΟΔΩΡΙΑΝΑ
+    14: ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
     30: 2 ΑΝΤΙΤΥΠΑ
     3: null
     6: null
     7: null
     8: null
-    14: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -377376,42 +377390,42 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7643
   authors: []
   title: ΑΚΡΙΤΙΚΟΣ ΑΛΥΤΡΩΤΟΣ ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
-  dewey: 398 ΧΣ
+  dewey: 938.695 ΧΣ
   entry_numbers:
   - '8053'
   - '10128'
   editor: ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1996
   pages: 234
   topics:
-  - ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
+  - ΕΛΛΗΝΙΣΜΟΣ
   copies: 3
   donors:
   - ΛΙΟΝΤΟΣ,Ν.
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7643
     1: Χ.Σ
     2: ΑΚΡΙΤΙΚΟΣ ΑΛΥΤΡΩΤΟΣ ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
-    4: 398Χ.Σ.
+    4: 938.695Χ.Σ
     5: 8053-10128
     8: ΚΥΡΙΑΚΙΔΗΣ
     9: ΒΕΡΟΙΑ
     10: '1996'
     11: 234Σ
-    12: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
-    13: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
-    14: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
+    12: ΕΛΛΗΝΙΣΜΟΣ
+    13: ΕΛΛΗΝΙΣΜΟΣ
+    14: ΕΛΛΗΝΙΣΜΟΣ
     17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
     30: 3 ΑΝΤΙΤΥΠΑ
     3: null
     6: null
     7: null
     15: null
     16: null
@@ -377956,15 +377970,15 @@
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 7655
   authors:
   - ΜΕΛΙΚΗΣ. ΓΙΩΡΓΗΣ
-  title: ΤΑ ΛΑΟΓΡΑΦΙΚΣ ΤΗΣ ΜΕΛΙΚΗΣ
+  title: ΤΑ ΛΑΟΓΡΑΦΙΚΑ ΤΗΣ ΜΕΛΙΚΗΣ
   dewey: 398 ΜΕΛ
   entry_numbers:
   - '10151'
   - '8079'
   editor: None // ΜΕΛΙΚΗ
   pages: 220
   topics:
@@ -377974,15 +377988,15 @@
   volume: ΤΟΜΟΣ Δ- 2 ΑΝΤΙΤΥΠΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7655
     1: ΜΕΛΙΚΗΣ. ΓΙΩΡΓΗΣ
-    2: ΤΑ ΛΑΟΓΡΑΦΙΚΣ ΤΗΣ ΜΕΛΙΚΗΣ
+    2: ΤΑ ΛΑΟΓΡΑΦΙΚΑ ΤΗΣ ΜΕΛΙΚΗΣ
     4: 398ΜΕΛ
     5: 10151-8079
     9: ΜΕΛΙΚΗ
     11: 220Σ
     12: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
     17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
@@ -378440,15 +378454,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7665
   authors: []
-  title: ΠΟΙΗΤΙΚΗ ΑΝΘΟΛΟΓΙΑΔΙΟΝΥΣΙΟΣ ΣΟΛΩΜΟΣ
+  title: ΠΟΙΗΤΙΚΗ ΑΝΘΟΛΟΓΙΑ ΔΙΟΝΥΣΙΟΣ ΣΟΛΩΜΟΣ
   dewey: 880.08 ΧΣ
   entry_numbers:
   - '8519'
   editor: ΜΑΛΛΙΑΡΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1976
   pages: 300
   topics:
@@ -378457,15 +378471,15 @@
   volume: 3 ΤΟΜΟΙ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7665
     1: Χ.Σ
-    2: ΠΟΙΗΤΙΚΗ ΑΝΘΟΛΟΓΙΑΔΙΟΝΥΣΙΟΣ ΣΟΛΩΜΟΣ
+    2: ΠΟΙΗΤΙΚΗ ΑΝΘΟΛΟΓΙΑ ΔΙΟΝΥΣΙΟΣ ΣΟΛΩΜΟΣ
     4: 880.08Χ.Σ
     5: '8519'
     8: ΜΑΛΛΙΑΡΗΣ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1976'
     11: 300Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
@@ -380824,46 +380838,48 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7713
   authors:
-  - ΤΟΥΤΣΙΝΟΣ ΓΙΑΝΝΗΣ
+  - ΤΣΟΥΤΣΙΝΟΣ ΓΙΑΝΝΗΣ
   title: ΑΡΤΙΝΑ ΙΣΤΟΡΙΚΑ ΘΕΜΑΤΑ
   dewey: 938.939 ΤΟΥ
   entry_numbers:
   - '4420'
   editor: None // ΑΡΤΑ
   edition_year: 2001
   pages: 265
   topics:
+  - ΑΡΤΙΝΑ ΘΕΜΑΤΑ
   - ΙΣΤΟΡΙΚΑ
+  - ΑΡΤΑ
   donors:
   - ΨΩΜΑΣ,ΓΙΩΡΓΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7713
-    1: ΤΟΥΤΣΙΝΟΣ ΓΙΑΝΝΗΣ
+    1: ΤΣΟΥΤΣΙΝΟΣ ΓΙΑΝΝΗΣ
     2: ΑΡΤΙΝΑ ΙΣΤΟΡΙΚΑ ΘΕΜΑΤΑ
     4: 938.939ΤΟΥ
     5: '4420'
     9: ΑΡΤΑ
     10: '2001'
     11: 265Σ
-    12: ΙΣΤΟΡΙΚΑ
+    12: ΑΡΤΙΝΑ ΘΕΜΑΤΑ
     13: ΙΣΤΟΡΙΚΑ
+    14: ΑΡΤΑ
     17: ΔΩΡΕΑ ΓΙΩΡΓΟΥ ΨΩΜΑ
     3: null
     6: null
     7: null
     8: null
-    14: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -381464,15 +381480,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7726
   authors:
-  - ΕΛΕΝΗ ΚΑΡΙΤΑ
+  - ΚΑΡΙΤΑ,ΕΛΕΝΗ
   title: Η ΜΟΡΦΗ ΜΙΑΣ ΑΓΙΑΣ
   dewey: 230 ΚΑΡ
   entry_numbers:
   - '10251'
   editor: Ι. ΜΗΤΡ.ΧΑΛΚΙΔΟΣ // None
   edition_year: 1973
   pages: 219
@@ -381481,15 +381497,15 @@
   donors:
   - ΜΑΝΙΚΑ,ΕΛΕΝΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7726
-    1: ΕΛΕΝΗ ΚΑΡΙΤΑ
+    1: ΚΑΡΙΤΑ,ΕΛΕΝΗ
     2: Η ΜΟΡΦΗ ΜΙΑΣ ΑΓΙΑΣ
     4: 230ΚΑΡ
     5: '10251'
     8: Ι. ΜΗΤΡ.ΧΑΛΚΙΔΟΣ
     10: '1973'
     11: 219Σ
     12: ΘΡΗΣΚΕΥΤΙΚΑ
@@ -381901,15 +381917,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7735
   authors:
-  - ΧΑΡΑΛΑΜΠΙΔΗΣ ΓΡΗΓΟΡΙΟΣ
+  - ΧΑΡΑΛΑΜΠΙΔΗΣ,ΓΡΗΓΟΡΙΟΣ
   title: ΤΟ ΣΑΡΑΚΙ ΤΗΣ ΨΥΧΗΣ
   dewey: 230 ΧΑΡ
   entry_numbers:
   - '10241'
   edition: '9'
   editor: Ο ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 2003
@@ -381919,15 +381935,15 @@
   donors:
   - ΜΑΝΙΚΑ,ΕΛΕΝΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7735
-    1: ΧΑΡΑΛΑΜΠΙΔΗΣ ΓΡΗΓΟΡΙΟΣ
+    1: ΧΑΡΑΛΑΜΠΙΔΗΣ,ΓΡΗΓΟΡΙΟΣ
     2: ΤΟ ΣΑΡΑΚΙ ΤΗΣ ΨΥΧΗΣ
     4: 230ΧΑΡ
     5: '10241'
     7: 9Η
     8: Ο ΣΩΤΗΡ
     9: ΑΘΗΝΑ
     10: '2003'
@@ -408568,32 +408584,33 @@
     28: null
     29: null
     30: null
 - dbase_number: 8285
   authors:
   - ΣΧΙΣΜΕΝΟΣ ΑΡΙΣΤΕΙΔΗΣ
   title: ΜΥΘΟΙ ΚΑΙ ΠΑΡΑΔΟΣΕΙΣ ΜΝΗΜΕΙΩΝ ΚΑΙ ΤΟΠΟΘΕΣΙΩΝ ΤΟΥ ΝΟΜΟΥ ΑΡΤΑΣ
-  dewey: 398 ΣΧΙ
+  dewey: 938.939 ΣΧΙ
   entry_numbers:
   - '9589'
+  - '16177'
   editor: ΥΔΡΟΓΕΙΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2009
   pages: 369
   topics:
   - ΛΑΟΓΡΑΦΙΑ
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8285
     1: ΣΧΙΣΜΕΝΟΣ ΑΡΙΣΤΕΙΔΗΣ
     2: ΜΥΘΟΙ ΚΑΙ ΠΑΡΑΔΟΣΕΙΣ ΜΝΗΜΕΙΩΝ ΚΑΙ ΤΟΠΟΘΕΣΙΩΝ ΤΟΥ ΝΟΜΟΥ ΑΡΤΑΣ
-    4: 398 ΣΧΙ
-    5: '9589'
+    4: 938.939ΣΧΙ
+    5: 9589-16177
     8: ΥΔΡΟΓΕΙΟΣ
     9: ΘΕΣ\ΝΙΚΗ
     10: '2009'
     11: 369Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
     14: ΛΑΟΓΡΑΦΙΑ
@@ -415959,29 +415976,29 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8438
   authors: []
   title: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΗΣ
-  dewey: 398.483 ΡΗΓ
+  dewey: 938.483 ΡΗΓ
   entry_numbers:
   - '9422'
   editor: None // ΑΘΗΝΑ
   edition_year: 1998
   pages: 141
   topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8438
     1: Χ.Σ
     2: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΗΣ
-    4: 398.483ΡΗΓ
+    4: 938.483ΡΗΓ
     5: '9422'
     9: ΑΘΗΝΑ
     10: '1998'
     11: 141Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
     3: null
@@ -416013,34 +416030,35 @@
   entry_numbers:
   - '9889'
   translators:
   - ΚΟΥΝΕΖΗ,
   editor: ΜΕΤΑΙΧΜΙΟ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 318
-  topics: []
+  topics:
+  - ΣΜΥΡΝΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8439
     1: ΚΑΡΜΕΝ ΣΜΥΡΝΕΛΗ ΜΑΡΙΑ
     2: ΣΜΥΡΝΗ, Η ΛΗΣΜΟΝΗΜΕΝΗ ΠΟΛΗ?
     4: 938.498ΚΑΡ
     5: '9889'
     6: ΚΟΥΝΕΖΗ
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2006'
     11: 318Σ
+    12: ΙΣΤΟΡΙΑ-ΣΜΥΡΝΗ
+    13: ΙΣΤΟΡΙΑ-ΣΜΥΡΝΗ
+    14: ΣΜΥΡΝΗ-ΙΣΤΟΡΙΑ
     3: null
     7: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -416059,35 +416077,37 @@
   title: ΣΤΟ ΟΝΟΜΑ ΤΗΣ ΠΡΟΣΦΥΓΙΑΣ
   dewey: 938.498 ΤΖΑ
   entry_numbers:
   - '9890'
   editor: ΜΕΤΑΙΧΜΙΟ // ΑΘΗΝΑ
   edition_year: 2009
   pages: 575
-  topics: []
+  topics:
+  - ΠΟΝΤΟΣ
+  - ΣΜΥΡΝΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8440
     1: ΤΖΑΝΑΚΑΡΗΣ ΒΑΣΙΛΗΣ
     2: ΣΤΟ ΟΝΟΜΑ ΤΗΣ ΠΡΟΣΦΥΓΙΑΣ
     4: 938.498ΤΖΑ
     5: '9890'
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2009'
     11: 575Σ
+    12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+    13: ΙΣΤΟΡΙΑ-ΣΜΥΡΝΗ
+    14: ΙΣΤΟΡΙΑ
+    15: ΠΟΝΤΟΣ-ΣΜΥΡΝΗ
     3: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
-    15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -416143,33 +416163,33 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8442
   authors:
-  - ΑΘΑΝΑΣΑΚΗ ΑΝΤΩΝΙΟΥ
+  - ΑΘΑΝΑΣΑΚΗ,ΑΝΤΩΝΙΟΥ
   title: ΠΕΡΙΛΗΠΤΙΚΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ
   subtitle: ΑΠΟ ΤΟ 1897 ΜΕΧΡΙ ΤΟ 1940-41
-  dewey: '938.764'
+  dewey: 938.764 ΑΘΑ
   entry_numbers:
   - '9659'
   editor: ΠΕΤΡΑ // ΑΘΗΝΑ
   edition_year: 2010
   pages: 141
   topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8442
-    1: ΑΘΑΝΑΣΑΚΗ ΑΝΤΩΝΙΟΥ
+    1: ΑΘΑΝΑΣΑΚΗ,ΑΝΤΩΝΙΟΥ
     2: ΠΕΡΙΛΗΠΤΙΚΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ
     3: ΑΠΟ ΤΟ 1897 ΜΕΧΡΙ ΤΟ 1940-41
-    4: '938.764'
+    4: 938.764ΑΘΑ
     5: '9659'
     8: ΠΕΤΡΑ
     9: ΑΘΗΝΑ
     10: '2010'
     11: 141Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -416437,21 +416457,21 @@
     1: ΑΡΚΑΔΙΝΟΣ ΠΟΛΙΒΙΟΣ
     2: Η ΕΣΩΤΕΡΙΚΗ ΚΡΙΣΙΣ ΤΟΥ Κ.Κ.Ε
     4: 938.8ΑΡΚ
     5: '9839'
     9: ΑΘΗΝΑ
     10: '1954'
     11: 136Σ
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
     3: null
     6: null
     7: null
     8: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -416464,40 +416484,40 @@
     28: null
     29: null
     30: null
 - dbase_number: 8449
   authors:
   - ΔΗΜΟΣ ΤΑΣΟΣ
   title: ΕΝΑ ΓΑΡΥΦΑΛΛΟ ΠΟΥ ΔΕΝ Τ ΑΦΗΝΟΥΝ Ν ΑΝΘΙΣΕΙ
-  dewey: '938.8'
+  dewey: 938.8 ΔΗΜ
   entry_numbers:
   - '4350'
   editor: ΓΛΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1982
   pages: 98
   topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8449
     1: ΔΗΜΟΣ ΤΑΣΟΣ
     2: ΕΝΑ ΓΑΡΥΦΑΛΛΟ ΠΟΥ ΔΕΝ Τ ΑΦΗΝΟΥΝ Ν ΑΝΘΙΣΕΙ
-    4: '938.8'
+    4: 938.8ΔΗΜ
     5: '4350'
     8: ΓΛΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1982'
     11: 98Σ
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
     3: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -416510,40 +416530,41 @@
     28: null
     29: null
     30: null
 - dbase_number: 8450
   authors:
   - ΛΑΜΠΡΙΝΙΔΗΣ ΜΗΝΑΣ
   title: Η ΑΛΒΑΝΙΑ ΣΗΜΕΡΑ
-  dewey: '941.2'
+  dewey: 941.2 ΛΑΜ
   entry_numbers:
   - '5372'
   editor: None // ΑΘΗΝΑ
   edition_year: 1987
   pages: 173
-  topics: []
+  topics:
+  - ΑΛΒΑΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8450
     1: ΛΑΜΠΡΙΝΙΔΗΣ ΜΗΝΑΣ
     2: Η ΑΛΒΑΝΙΑ ΣΗΜΕΡΑ
-    4: '941.2'
+    4: 941.2ΛΑΜ
     5: '5372'
     9: ΑΘΗΝΑ
     10: '1987'
     11: 173Σ
+    12: ΑΛΒΑΝΙΑ
+    13: ΑΛΒΑΝΙΑ
+    14: ΑΛΒΑΝΙΑ
     3: null
     6: null
     7: null
     8: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -416983,15 +417004,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8460
     1: ΛΙΧΤΧΑΙΜ ΤΖΩΡΤΖ
     2: ΣΥΝΤΟΜΗ ΠΑΓΚΟΣΜΙΑ ΙΣΤΟΡΙΑ ΤΟΥ ΣΟΣΙΑΛΙΣΜΟΥ
-    4: 938.8 ΛΙΧ
+    4: 938.8ΛΙΧ
     5: '10662'
     6: ΚΩΣΤΕΛΕΝΙΟΣ
     8: ΓΛΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1976'
     11: 409Σ
     12: ΙΣΤΟΡΙΑ
@@ -417424,31 +417445,31 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8470
   authors:
-  - ΚΕΛΑΙΔΗ ΠΑΡΙ
+  - ΚΕΛΑΙΔΗ,ΠΑΡΙ
   title: ΚΡΗΤΙΚΟΙ ΕΘΕΛΟΝΤΕΣ ΣΤΟΥΣ ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΥΣ ΠΟΛΕΜΟΥΣ 1912-13
-  dewey: '938.655'
+  dewey: 938.655 ΚΕΛ
   entry_numbers:
   - '10686'
   editor: ΚΑΡΑΒΙ ΚΑΙ ΤΟΞΟ // ΑΘΗΝΑ
   edition_year: 1995
   pages: 295
   topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8470
-    1: ΚΕΛΑΙΔΗ ΠΑΡΙ
+    1: ΚΕΛΑΙΔΗ,ΠΑΡΙ
     2: ΚΡΗΤΙΚΟΙ ΕΘΕΛΟΝΤΕΣ ΣΤΟΥΣ ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΥΣ ΠΟΛΕΜΟΥΣ 1912-13
-    4: '938.655'
+    4: 938.655ΚΕΛ
     5: '10686'
     8: ΚΑΡΑΒΙ ΚΑΙ ΤΟΞΟ
     9: ΑΘΗΝΑ
     10: '1995'
     11: 295Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -417486,15 +417507,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8471
     1: ΤΟΚΒΙΛ ΑΛΕΞΗΣ
     2: Η ΔΗΜΟΚΡΑΤΙΑ ΣΤΗΝ ΑΜΕΡΙΚΗ
-    4: 970 ΤΟΚ
+    4: 970ΤΟΚ
     5: '9303'
     8: ΣΤΟΧΑΣΤΗΣ
     9: ΑΘΗΝΑ
     10: '1997'
     11: 722Σ
     3: null
     6: null
@@ -417661,42 +417682,44 @@
     28: null
     29: null
     30: null
 - dbase_number: 8475
   authors:
   - ΣΠΗΛΙΟΣ ΑΠΟΣΤΟΛΟΣ
   title: ΠΕΛΑΣΓΙΚΗ ΗΠΕΙΡΟΣ ΚΑΙ ΑΡΑΧΘΟΣ Ο ΠΕΛΑΣΓΙΚΟΣ
-  subtitle: '9'
   dewey: 938.21 ΣΠΗ
   entry_numbers:
   - '9335'
+  - '17184'
   editor: ΘΕΣΙΣ // ΑΘΗΝΑ
   edition_year: 2002
   pages: 135
-  topics: []
+  topics:
+  - ΗΠΕΙΡΟΣ
+  - ΑΡΑΧΘΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8475
     1: ΣΠΗΛΙΟΣ ΑΠΟΣΤΟΛΟΣ
     2: ΠΕΛΑΣΓΙΚΗ ΗΠΕΙΡΟΣ ΚΑΙ ΑΡΑΧΘΟΣ Ο ΠΕΛΑΣΓΙΚΟΣ
-    3: '                                                           9'
     4: 938.21ΣΠΗ
-    5: '9335'
+    5: 9335-17184
     8: ΘΕΣΙΣ
     9: ΑΘΗΝΑ
     10: '2002'
     11: 135Σ
+    12: ΗΠΕΙΡΟΣ-ΑΡΑΧΘΟΣ
+    13: ΙΣΤΟΡΙΑ
+    14: ΑΡΑΧΘΟΣ
+    15: ΗΠΕΙΡΟΣ
+    3: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
-    15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -417714,35 +417737,37 @@
   title: ΙΣΤΟΡΙΑ ΤΟΥ ΒΟΡΕΙΟΥ ΕΛΛΗΝΙΣΜΟΥ ΘΡΑΚΗ
   dewey: 938.695 ΒΑΚ
   entry_numbers:
   - '9305'
   editor: ΚΥΡΙΑΚΙΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1993
   pages: 567
-  topics: []
+  topics:
+  - ΘΡΑΚΗ
+  - ΒΟΡΕΙΟΣ ΕΛΛΗΝΙΣΜΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8476
     1: ΒΑΚΑΛΟΠΟΥΛΟΣ ΚΩΝΣΤΑΝΤΙΝΟΣ
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΒΟΡΕΙΟΥ ΕΛΛΗΝΙΣΜΟΥ ΘΡΑΚΗ
     4: 938.695ΒΑΚ
     5: '9305'
     8: ΚΥΡΙΑΚΙΗΣ
     9: ΘΕΣ\ΝΙΚΗ
     10: '1993'
     11: 567Σ
+    12: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
+    13: ΘΡΑΚΗ
+    14: ΙΣΤΟΡΙΑ
+    15: ΒΟΡΕΙΟΣ ΕΛΛΗΝΙΣΜΟΣ
     3: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
-    15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -420706,17 +420731,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8537
   authors:
-  - ΕΝΙΝΤ,ΜΠΛΑΙΤΟΝ
+  - ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
   title: ΤΟ ΒΙΒΛΙΟ ΜΕ ΤΙΣ ΝΕΡΑΙΔΕΣ
-  dewey: 808.899 ΕΝΙ
+  dewey: 808.899 ΜΠΛ
   entry_numbers:
   - '10818'
   translators:
   - ΚΟΝΔΑΚΗ,ΜΙΡΚΑ
   edition: '2'
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 1996
@@ -420725,17 +420750,17 @@
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8537
-    1: ΕΝΙΝΤ,ΜΠΛΑΙΤΟΝ
+    1: ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
     2: ΤΟ ΒΙΒΛΙΟ ΜΕ ΤΙΣ ΝΕΡΑΙΔΕΣ
-    4: 808.899ΕΝΙ
+    4: 808.899ΜΠΛ
     5: '10818'
     6: ΜΙΡΚΑ ΚΟΝΔΑΚΗ
     7: 2η εκδ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '1996'
     11: '216'
@@ -452199,16 +452224,16 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9157
   authors:
   - SCHMINCK-GUSTAVUS CHRISTOPH U.
-  title: ΕΛΛΗΝΕΣ ΚΡΑΤΟΥΜΕΝΟΙ ΚΙΑ Ο ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
-  dewey: 938.764 CUS
+  title: ΕΛΛΗΝΕΣ ΚΡΑΤΟΥΜΕΝΟΙ ΚAI Ο ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
+  dewey: 938.764 GUS
   entry_numbers:
   - '11528'
   editor: ΦΙΛΙΣΤΩΡ // ΑΘΗΝΑ
   edition_year: 2004
   pages: 203
   topics:
   - ΙΣΤΟΡΙΚΑ
@@ -452217,16 +452242,16 @@
   - ΜΠΑΝΙΑΣ,ΓΙΑΝΝΗΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 9157
     1: SCHMINCK-GUSTAVUS CHRISTOPH U.
-    2: ΕΛΛΗΝΕΣ ΚΡΑΤΟΥΜΕΝΟΙ ΚΙΑ Ο ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
-    4: 938.764CUS
+    2: ΕΛΛΗΝΕΣ ΚΡΑΤΟΥΜΕΝΟΙ ΚAI Ο ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
+    4: 938.764GUS
     5: '11528'
     8: ΦΙΛΙΣΤΩΡ
     9: ΑΘΗΝΑ
     10: '2004'
     11: '203'
     12: ΙΣΤΟΡΙΚΑ-ΚΑΤΟΧΗ
     13: ΙΣΤΟΡΙΚΑ-ΚΑΤΟΧΗ
@@ -454562,15 +454587,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9204
   authors:
-  - ΑΒΔΟΥΛΟΣ,ΣΤΑΥΡΟΑ
+  - ΑΒΔΟΥΛΟΣ,ΣΤΑΥΡΟΣ
   title: ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
   subtitle: ΜΥΘΟΣ ΚΑΙ ΠΡΑΓΜΑΤΙΚΟΤΗΤΑ
   dewey: 938.764 ΑΒΔ
   entry_numbers:
   - '11490'
   editor: ΠΑΡΑΣΚΗΝΙΟ // ΑΘΗΝΑ
   edition_year: 2009
@@ -454581,15 +454606,15 @@
   - ΜΠΑΝΙΑΣ,ΓΙΑΝΝΗΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-8342-72-9
   original_entry:
     0: 9204
-    1: ΑΒΔΟΥΛΟΣ,ΣΤΑΥΡΟΑ
+    1: ΑΒΔΟΥΛΟΣ,ΣΤΑΥΡΟΣ
     2: ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
     3: ΜΥΘΟΣ ΚΑΙ ΠΡΑΓΜΑΤΙΚΟΤΗΤΑ
     4: 938.764ΑΒΔ
     5: '11490'
     8: ΠΑΡΑΣΚΗΝΙΟ
     9: ΑΘΗΝΑ
     10: '2009'
@@ -468857,54 +468882,53 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9488
   authors:
-  - ΜΠΑΣΤΑΝΗΣ,ΠΑΝΑΓΙΩΤΗΣ
-  title: ΤΟ ΤΡΕΝΟ ΤΟΥ ΦΩΤΟΣ
-  dewey: 889.21 ΜΠΑ
+  - ΛΑΡΣΟΝ,ΟΣΑ
+  title: PAX ΤΟ ΦΑΝΤΑΣΜΑ
+  dewey: 808.899 ΛΑΡ
   entry_numbers:
-  - '11773'
-  editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
-  edition_year: 1991
-  pages: 724
+  - '22602'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2018
+  pages: 215
   topics:
-  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-  - ΛΟΓΟΤΕΧΝΙΑ
-  donors:
-  - ΜΠΑΝΙΑΣ,ΓΙΑΝΝΗΣ
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  - 095
   has_cd: false
   has_dvd: false
   offprint: false
+  ean: '9786180124095'
   original_entry:
     0: 9488
-    1: ΜΠΑΣΤΑΝΗΣ,ΠΑΝΑΓΙΩΤΗΣ
-    2: ΤΟ ΤΡΕΝΟ ΤΟΥ ΦΩΤΟΣ
-    4: 889.21ΜΠΑ
-    5: '11773'
-    8: ΔΩΔΩΝΗ
+    1: ΛΑΡΣΟΝ,ΟΣΑ
+    2: PAX ΤΟ ΦΑΝΤΑΣΜΑ
+    4: 808.899ΛΑΡ
+    5: '22602'
+    8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
-    10: '1991'
-    11: 724Σ
-    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-    14: ΛΟΓΟΤΕΧΝΙΑ
-    17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
+    10: '2018'
+    11: '215'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    19: '9786180124'
+    22: 095
     3: null
     6: null
     7: null
     15: null
     16: null
+    17: null
     18: null
-    19: null
     20: null
     21: null
-    22: null
     23: null
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
@@ -473161,15 +473185,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 9574
   authors:
   - ΠΡΙΑΜΟΣ
   title: ΜΕ ΤΟ 7ο ΣΥΝΤΑΓΜΑ ΤΟΥ ΕΛΑΣ ΣΤΑ ΒΟΥΝΑ ΤΗΣ ΕΥΒΟΙΑΣ
-  dewey: 938.764 ΠΡΙ
+  dewey: 938.764 ΧΣ
   entry_numbers:
   - '11817'
   editor: None // ΑΘΗΝΑ
   pages: 136
   topics:
   - ΕΜΦΥΛΙΟΣ
   donors:
@@ -473177,15 +473201,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 9574
     1: ΠΡΙΑΜΟΣ
     2: ΜΕ ΤΟ 7ο ΣΥΝΤΑΓΜΑ ΤΟΥ ΕΛΑΣ ΣΤΑ ΒΟΥΝΑ ΤΗΣ ΕΥΒΟΙΑΣ
-    4: 938.764ΠΡΙ
+    4: 938.764Χ.Σ
     5: '11817'
     9: ΑΘΗΝΑ
     11: 136Σ
     12: ΙΣΤΟΡΙΑ-ΕΜΦΥΛΙΟΣ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
@@ -474398,15 +474422,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 9599
   authors:
   - ΠΑΠΑΙΩΑΝΝΟΥ,ΑΧΙΛΛΕΑΣ
   title: Η ΑΠΑΓΟΡΕΥΜΕΝΗ ΕΙΚΟΝΑ
-  dewey: 938.77 ΠΑΠ
+  dewey: 938.764 ΠΑΠ
   entry_numbers:
   - '11891'
   editor: ΦΙΛΙΣΤΩΡ // ΑΘΗΝΑ
   edition_year: 2001
   pages: 208
   topics: []
   donors:
@@ -474414,15 +474438,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 9599
     1: ΠΑΠΑΙΩΑΝΝΟΥ,ΑΧΙΛΛΕΑΣ
     2: Η ΑΠΑΓΟΡΕΥΜΕΝΗ ΕΙΚΟΝΑ
-    4: 938.77ΠΑΠ
+    4: 938.764ΠΑΠ
     5: '11891'
     8: ΦΙΛΙΣΤΩΡ
     9: ΑΘΗΝΑ
     10: '2001'
     11: 208Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -476969,17 +476993,18 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9649
   authors: []
   title: ΠΕΡΙ ΠΕΤΡΟΓΕΦΥΡΩΝ..
-  dewey: 624.609 ΠΡΑ
+  dewey: 938.939 ΧΣ
   entry_numbers:
   - '11920'
+  - '8656'
   editor: ΚΕ.ΜΕ.ΠΕ.Γ // ΑΘΗΝΑ
   edition_year: 2005
   pages: 414
   topics:
   - ΓΕΦΥΡΕΣ
   - ΠΕΤΡΙΝΕΣ
   - ΗΠΕΙΡΟΣ
@@ -476989,16 +477014,16 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 9649
     1: Χ.Σ.
     2: ΠΕΡΙ ΠΕΤΡΟΓΕΦΥΡΩΝ..
-    4: 624.609ΠΡΑ
-    5: '11920'
+    4: 938.939Χ.Σ
+    5: 11920-8656
     8: ΚΕ.ΜΕ.ΠΕ.Γ
     9: ΑΘΗΝΑ
     10: '2005'
     11: 414Σ
     12: ΓΕΦΥΡΕΣ-ΠΕΤΡΙΝΕΣ-ΗΠΕΙΡΟΣ
     13: ΓΕΦΥΡΕΣ-ΤΟΞΟΕΙΔΕΣ-ΗΠΕΙΡΟΣ
     14: ΓΕΦΥΡΕΣ-ΗΠΕΙΡΟΣ
@@ -477219,33 +477244,32 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9654
-  authors:
-  - ΠΡΑΚΤΙΚΑ
+  authors: []
   title: ΟΙ ΔΙΚΕΣ ΤΗΣ ΧΟΥΝΤΑΣ
-  dewey: 938.79 ΠΡΑ
+  dewey: 938.79 ΧΣ
   entry_numbers:
   - '11916'
   pages: 210
   topics:
   - ΧΟΥΝΤΑ
   donors:
   - ΜΠΑΝΙΑΣ,ΓΙΑΝΝΗΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 9654
-    1: ΠΡΑΚΤΙΚΑ
+    1: Χ.Σ
     2: ΟΙ ΔΙΚΕΣ ΤΗΣ ΧΟΥΝΤΑΣ
-    4: 938.79ΠΡΑ
+    4: 938.79Χ.Σ
     5: '11916'
     11: 210Σ
     12: ΙΣΤΟΡΙΑ-ΧΟΥΝΤΑ
     13: ΧΟΥΝΤΑ
     14: ΧΟΥΝΤΑ
     17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
     3: null
@@ -481382,14 +481406,15 @@
 - dbase_number: 9738
   authors: []
   title: ΠΟΛΗ 1955
   subtitle: Η ΤΕΛΕΥΤΑΙΑ ΑΛΩΣΗ
   dewey: 938.498 ΧΣ
   entry_numbers:
   - '12047'
+  - '14151'
   editor: ΤΕΓΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   pages: 192
   topics:
   - ΑΛΩΣΗ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗΣ
   - ΑΛΩΣΗ
   donors:
   - ΜΠΑΝΙΑΣ,ΓΙΑΝΝΗΣ
@@ -481398,15 +481423,15 @@
   offprint: false
   original_entry:
     0: 9738
     1: Χ.Σ
     2: ΠΟΛΗ 1955
     3: Η ΤΕΛΕΥΤΑΙΑ ΑΛΩΣΗ
     4: 938.498Χ.Σ
-    5: '12047'
+    5: 12047-14151
     8: ΤΕΓΟΠΟΥΛΟΣ
     9: ΑΘΗΝΑ
     11: 192Σ
     12: ΙΣΤΟΡΙΑ-ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
     13: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
     14: ΑΛΩΣΗ
     17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
@@ -481428,15 +481453,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 9739
   authors: []
   title: ΔΕΚΕΜΒΡΗΣ 44
   subtitle: ΟΙ ΜΑΧΕΣ ΣΤΙΣ ΓΕΙΤΟΝΙΕΣ ΤΗΣ ΑΘΗΝΑΣ
-  dewey: 938.771 ΧΣ
+  dewey: 938.764 ΧΣ
   entry_numbers:
   - '12046'
   editor: ΤΕΓΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   pages: 192
   topics:
   - ΔΕΚΕΜΒΡΙΑΝΑ
   donors:
@@ -481445,15 +481470,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 9739
     1: Χ.Σ
     2: ΔΕΚΕΜΒΡΗΣ 44
     3: ΟΙ ΜΑΧΕΣ ΣΤΙΣ ΓΕΙΤΟΝΙΕΣ ΤΗΣ ΑΘΗΝΑΣ
-    4: 938.771Χ.Σ
+    4: 938.764Χ.Σ
     5: '12046'
     8: ΤΕΓΟΠΟΥΛΟΣ
     9: ΑΘΗΝΑ
     11: 192Σ
     12: ΙΣΤΟΡΙΑ-ΔΕΚΕΜΒΡΙΑΝΑ
     13: ΙΣΤΟΡΙΑ-ΔΕΚΕΜΒΡΙΑΝΑ
     14: ΔΕΚΕΜΒΡΙΑΝΑ
@@ -482206,18 +482231,17 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9755
-  authors:
-  - ΜΠΕΛΟΓΙΑΝΝΗ
+  authors: []
   title: ΟΙ ΜΕΓΑΛΕΣ ΔΙΚΕΣ
-  dewey: 938.764 ΜΠΕ
+  dewey: 938.764 ΧΣ
   entry_numbers:
   - '12033'
   editor: ΦΩΤΟΕΚΔΟΤΙΚΗ // ΑΘΗΝΑ
   edition_year: 2011
   pages: 207
   topics:
   - ΜΠΕΛΟΓΙΑΝΝΗΣ
@@ -482225,17 +482249,17 @@
   donors:
   - ΜΠΑΝΙΑΣ,ΓΙΑΝΝΗΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 9755
-    1: ΜΠΕΛΟΓΙΑΝΝΗ
+    1: Χ.Σ
     2: ΟΙ ΜΕΓΑΛΕΣ ΔΙΚΕΣ
-    4: 938.764ΜΠΕ
+    4: 938.764Χ.Σ
     5: '12033'
     8: ΦΩΤΟΕΚΔΟΤΙΚΗ
     9: ΑΘΗΝΑ
     10: '2011'
     11: 207Σ
     12: ΙΣΤΟΡΙΑ-ΜΠΕΛΟΓΙΑΝΝΗΣ
     13: ΜΠΕΛΟΓΙΑΝΝΗΣ-ΔΙΚΗ
@@ -485491,18 +485515,17 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9822
-  authors:
-  - ΑΝΤΥΠΑΣ,ΣΤΑΥΡΟΣ
+  authors: []
   title: ΝΟΕΜΒΡΗΣ ΗΤΑΝ,ΟΙ ΧΡΟΝΙΕΣ..1973-2003
-  dewey: 938.79 ΑΝΤ
+  dewey: 938.79 ΧΣ
   entry_numbers:
   - '12123'
   editor: ΓΡΑΦΕΣ // ΑΘΗΝΑ
   edition_year: 2003
   pages: 173
   topics:
   - ΠΟΛΥΤΕΧΝΕΙΟ
@@ -485510,17 +485533,17 @@
   - ΜΠΑΝΙΑΣ,ΓΙΑΝΝΗΣ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-8281-28-8
   original_entry:
     0: 9822
-    1: ΑΝΤΥΠΑΣ,ΣΤΑΥΡΟΣ
+    1: Χ.Σ
     2: ΝΟΕΜΒΡΗΣ ΗΤΑΝ,ΟΙ ΧΡΟΝΙΕΣ..1973-2003
-    4: 938.79ΑΝΤ
+    4: 938.79Χ.Σ
     5: '12123'
     8: ΓΡΑΦΕΣ
     9: ΑΘΗΝΑ
     10: '2003'
     11: 173Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΛΥΤΕΧΝΕΙΟ
     13: ΠΟΛΥΤΕΧΝΕΙΟ
@@ -485982,15 +486005,15 @@
     29: null
     30: null
 - dbase_number: 9832
   authors:
   - ΠΡΑΚΤΙΚΑ ΕΚΔΗΛΩΣΗΣ
   title: 40 ΧΡΟΝΙΑ
   subtitle: ΜΑΗΣ 68
-  dewey: 938.79 ΠΡΑ
+  dewey: 938.79 ΧΣ
   entry_numbers:
   - '12096'
   editor: ΜΙΛΗΤΟΣ // ΑΘΗΝΑ
   pages: 331
   topics:
   - ΠΡΑΞΙΚΟΠΗΜΑ
   donors:
@@ -485999,15 +486022,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 9832
     1: ΠΡΑΚΤΙΚΑ ΕΚΔΗΛΩΣΗΣ
     2: 40 ΧΡΟΝΙΑ
     3: ΜΑΗΣ 68
-    4: 938.79ΠΡΑ
+    4: 938.79Χ.Σ
     5: '12096'
     8: ΜΙΛΗΤΟΣ
     9: ΑΘΗΝΑ
     11: 331Σ
     12: ΙΣΤΟΡΙΑ-ΠΡΑΞΙΚΟΠΗΜΑ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
@@ -504703,37 +504726,36 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10227
-  authors:
-  - ΔΑΡΔΑΒΕΣΗΣ,ΘΕΟΔΩΡΟΥ
+  authors: []
   title: ΓΕΡΜΑΝΙΚΗ ΚΑΤΟΧΗ
   subtitle: ΙΣΤΟΡΙΕΣ ΑΠΟ ΤΑ ΣΥΣΣΙΤΙΑ ΣΤΗ ΦΙΛΟΠΤΩΧΟ ΑΔΕΛΦΟΤΗΤΑ ΑΝΔΡΩΝ ΘΕΣ
-  dewey: 938.764 ΔΑΡ
+  dewey: 938.764 ΧΣ
   entry_numbers:
   - '12511'
   editor: ΦΑΑΘ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2012
   pages: 150
   topics:
   - ΚΑΤΟΧΗ
   - ΓΕΡΜΑΝΙΚΗ ΚΑΤΟΧΗ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-9694-06-3
   original_entry:
     0: 10227
-    1: ΔΑΡΔΑΒΕΣΗΣ,ΘΕΟΔΩΡΟΥ
+    1: Χ.Σ
     2: ΓΕΡΜΑΝΙΚΗ ΚΑΤΟΧΗ
     3: ΙΣΤΟΡΙΕΣ ΑΠΟ ΤΑ ΣΥΣΣΙΤΙΑ ΣΤΗ ΦΙΛΟΠΤΩΧΟ ΑΔΕΛΦΟΤΗΤΑ ΑΝΔΡΩΝ ΘΕΣ
-    4: 938.764ΔΑΡ
+    4: 938.764Χ.Σ
     5: '12511'
     8: ΦΑΑΘ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2012'
     11: 150Σ
     12: ΙΣΤΟΡΙΑ-ΚΑΤΟΧΗ
     13: ΙΣΤΟΡΙΑ-ΚΑΤΟΧΗ
@@ -504757,15 +504779,17 @@
     29: null
     30: null
 - dbase_number: 10228
   authors:
   - ΒΑΣΙΛΑΚΗΣ,ΧΡΗΣΤΟΣ
   title: ΤΟ ΑΙΜΑ ΤΩΝ ΜΑΡΤΥΡΩΝ
   subtitle: ΤΟ ΚΟΜΜΕΝΟ ΣΤΑ ΧΡΟΝΙΑ ΤΗΣ ΓΕΡΜΑΝΙΚΗΣ ΚΑΤΟΧΗΣ
-  entry_numbers: []
+  dewey: 938.939 ΒΑΣ
+  entry_numbers:
+  - '12512'
   editor: ΓΡΗΓΟΡΗ // ΑΘΗΝΑ
   edition_year: 2012
   pages: 327
   topics:
   - ΚΟΜΜΕΝΟ
   - ΚΑΤΟΧΗ
   has_cd: false
@@ -504773,25 +504797,25 @@
   offprint: false
   ean: 978-960-333-693-8
   original_entry:
     0: 10228
     1: ΒΑΣΙΛΑΚΗΣ,ΧΡΗΣΤΟΣ
     2: ΤΟ ΑΙΜΑ ΤΩΝ ΜΑΡΤΥΡΩΝ
     3: ΤΟ ΚΟΜΜΕΝΟ ΣΤΑ ΧΡΟΝΙΑ ΤΗΣ ΓΕΡΜΑΝΙΚΗΣ ΚΑΤΟΧΗΣ
+    4: 938.939ΒΑΣ
+    5: '12512'
     8: ΓΡΗΓΟΡΗ
     9: ΑΘΗΝΑ
     10: '2012'
     11: 327Σ
     12: ΙΣΤΟΡΙΑ-ΚΟΜΜΕΝΟ
     13: ΚΟΜΜΕΝΟ-ΚΑΤΟΧΗ
     14: ΙΣΤΟΡΙΑ
     18: 978-960-33
     19: 3-693-8
-    4: null
-    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     20: null
     21: null
@@ -507000,15 +507024,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10274
   authors: []
   title: ΜΙΚΡΑΣΙΑΤΙΚΗ ΚΑΤΑΣΤΡΟΦΗ
-  subtitle: ΤΙ ΕΦΤΕΙΞΕ
+  subtitle: ΤΙ ΕΦΤΑΙΞΕ
   dewey: 938.498 ΧΣ
   entry_numbers:
   - '12629'
   editor: ΕΛΕΥΘΕΡΟΣ ΤΥΠΟΣ // ΑΘΗΝΑ
   pages: 160
   topics:
   - ΜΙΚΡΑ ΑΣΙΑ
@@ -507017,15 +507041,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-285-118-0
   original_entry:
     0: 10274
     1: Χ.Σ.
     2: ΜΙΚΡΑΣΙΑΤΙΚΗ ΚΑΤΑΣΤΡΟΦΗ
-    3: ΤΙ ΕΦΤΕΙΞΕ
+    3: ΤΙ ΕΦΤΑΙΞΕ
     4: 938.498Χ.Σ
     5: '12629'
     8: ΕΛΕΥΘΕΡΟΣ ΤΥΠΟΣ
     9: ΑΘΗΝΑ
     11: 160Σ
     12: ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
     13: ΜΙΚΡΑΣΙΑΤΙΚΗ ΚΑΤΑΣΤΡΟΦΗ
@@ -515987,15 +516011,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10451
   authors:
   - ΣΑΜΟΥΗΛΙΔΗΣ,ΧΡΗΣΤΟΣ
   title: ΑΜΙΣΟΣ (ΣΑΜΨΟΥΝΤΑ) ΚΑΙ Η ΠΕΡΙΦΕΡΕΙΑ ΤΗΣ
-  dewey: 938.993 ΣΑΜ
+  dewey: 938.498 ΣΑΜ
   entry_numbers:
   - '13033'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2004
   pages: 187
   topics:
   - ΠΟΝΤΟΣ
@@ -516007,15 +516031,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-778-6
   original_entry:
     0: 10451
     1: ΣΑΜΟΥΗΛΙΔΗΣ,ΧΡΗΣΤΟΣ
     2: ΑΜΙΣΟΣ (ΣΑΜΨΟΥΝΤΑ) ΚΑΙ Η ΠΕΡΙΦΕΡΕΙΑ ΤΗΣ
-    4: 938.993ΣΑΜ
+    4: 938.498ΣΑΜ
     5: '13033'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2004'
     11: 187Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516039,15 +516063,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10452
   authors:
   - ΤΣΙΡΟΖΗΣ-ΤΣΙΡΟΖΙΔΗΣ,ΣΤΑΥΡΟΣ
   title: ΤΟ ΧΩΡΙΟ ΜΟΥ ΤΣΙΤΑ ΣΤΑ ΣΟΥΡΜΕΝΑ ΤΟΥ ΠΟΝΤΟΥ
-  dewey: 938.993 ΤΣΙ
+  dewey: 938.498 ΤΣΙ
   entry_numbers:
   - '13032'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2000
   pages: 176
   topics:
   - ΠΟΝΤΟΣ
@@ -516059,15 +516083,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-560-0
   original_entry:
     0: 10452
     1: ΤΣΙΡΟΖΗΣ-ΤΣΙΡΟΖΙΔΗΣ,ΣΤΑΥΡΟΣ
     2: ΤΟ ΧΩΡΙΟ ΜΟΥ ΤΣΙΤΑ ΣΤΑ ΣΟΥΡΜΕΝΑ ΤΟΥ ΠΟΝΤΟΥ
-    4: 938.993ΤΣΙ
+    4: 938.498ΤΣΙ
     5: '13032'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2000'
     11: 176Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516091,15 +516115,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10453
   authors:
   - ΜΠΑΚΑΛΑΚΗ-ΕΜΠΕΟΓΛΟΥ,ΕΥΔΟΚΙΑ
   title: Η ΑΜΑΣΕΙΑ
-  dewey: 938.993 ΜΠΑ
+  dewey: 938.498 ΜΠΑ
   entry_numbers:
   - '13031'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1988
   pages: 176
   topics:
   - ΠΟΝΤΟΣ
@@ -516110,15 +516134,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10453
     1: ΜΠΑΚΑΛΑΚΗ-ΕΜΠΕΟΓΛΟΥ,ΕΥΔΟΚΙΑ
     2: Η ΑΜΑΣΕΙΑ
-    4: 938.993ΜΠΑ
+    4: 938.498ΜΠΑ
     5: '13031'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1988'
     11: 176Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516193,15 +516217,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10455
   authors:
   - ΚΥΝΗΓΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ
   title: ΠΑΦΡΑ ΤΟΥ ΠΟΝΤΟΥ Η ΧΩΡΑ ΤΩΝ ΓΕΝΝΑΙΩΝ
-  dewey: 938.993 ΚΥΝ
+  dewey: 938.498 ΚΥΝ
   entry_numbers:
   - '13029'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2012
   pages: 308
   topics:
   - ΠΟΝΤΟΣ
@@ -516213,15 +516237,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-467-363-6
   original_entry:
     0: 10455
     1: ΚΥΝΗΓΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ
     2: ΠΑΦΡΑ ΤΟΥ ΠΟΝΤΟΥ Η ΧΩΡΑ ΤΩΝ ΓΕΝΝΑΙΩΝ
-    4: 938.993ΚΥΝ
+    4: 938.498ΚΥΝ
     5: '13029'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2012'
     11: 308Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516297,15 +516321,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10457
   authors:
   - ΧΑΡΗΣ,ΘΕΟΧΑΡΗΣ
   title: ΤΟ ΚΑΡΑΟΥΡΓΑΝ ΤΟΥ ΚΑΡΣ ΚΑΙ Η ΖΩΗ ΜΟΥ
-  dewey: 938.993 ΧΑΡ
+  dewey: 938.498 ΧΑΡ
   entry_numbers:
   - '13027'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 235
   topics:
   - ΠΟΝΤΟΣ
@@ -516317,15 +516341,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-596-1
   original_entry:
     0: 10457
     1: ΧΑΡΗΣ,ΘΕΟΧΑΡΗΣ
     2: ΤΟ ΚΑΡΑΟΥΡΓΑΝ ΤΟΥ ΚΑΡΣ ΚΑΙ Η ΖΩΗ ΜΟΥ
-    4: 938.993ΧΑΡ
+    4: 938.498ΧΑΡ
     5: '13027'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2001'
     11: 235Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516349,15 +516373,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10458
   authors:
   - ΧΑΤΖΗΚΥΡΙΑΚΙΔΗ,ΚΥΡΙΑΚΟ
   title: ΤΟ ΜΕΤΑΛΛΕΙΟ ΤΑΥΡΟΥ (ΜΠΟΥΓΑ ΜΑΝΤΕΝ)1826-1924
-  dewey: 938.993 ΧΑΤ
+  dewey: 938.498 ΧΑΤ
   entry_numbers:
   - '13026'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2004
   pages: 280
   topics:
   - ΠΟΝΤΟΣ
@@ -516369,15 +516393,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-473-6
   original_entry:
     0: 10458
     1: ΧΑΤΖΗΚΥΡΙΑΚΙΔΗ,ΚΥΡΙΑΚΟ
     2: ΤΟ ΜΕΤΑΛΛΕΙΟ ΤΑΥΡΟΥ (ΜΠΟΥΓΑ ΜΑΝΤΕΝ)1826-1924
-    4: 938.993ΧΑΤ
+    4: 938.498ΧΑΤ
     5: '13026'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2004'
     11: 280Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516506,15 +516530,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10461
   authors:
   - ΛΑΠΑΡΙΔΗΣ,ΝΙΚΟΣ
   title: Η ΖΑΒΕΡΑ ΤΗΣ ΜΑΤΣΟΥΚΑΣ ΤΟΥ ΠΟΝΤΟΥ
-  dewey: 938.993 ΛΑΠ
+  dewey: 938.498 ΛΑΠ
   entry_numbers:
   - '13042'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2003
   pages: 118
   topics:
   - ΠΟΝΤΟΣ
@@ -516526,15 +516550,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-725-5
   original_entry:
     0: 10461
     1: ΛΑΠΑΡΙΔΗΣ,ΝΙΚΟΣ
     2: Η ΖΑΒΕΡΑ ΤΗΣ ΜΑΤΣΟΥΚΑΣ ΤΟΥ ΠΟΝΤΟΥ
-    4: 938.993ΛΑΠ
+    4: 938.498ΛΑΠ
     5: '13042'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2003'
     11: 118Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516559,15 +516583,15 @@
     28: null
     29: null
 - dbase_number: 10462
   authors:
   - ΣΠΥΡΑΝΤΗ,ΑΝΔΡΕΑ
   title: ΤΡΑΠΕΖΟΥΣ ΚΑΙ Η ΜΟΝΗ ΣΟΥΜΕΛΑ ΤΟΥ ΠΟΝΤΟΥ
   subtitle: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΑ ΧΡΟΝΙΑ 1910-1922
-  dewey: 938.993 ΣΠΥ
+  dewey: 938.498 ΣΠΥ
   entry_numbers:
   - '13041'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1991
   pages: 110
   topics:
   - ΠΟΝΤΟΣ
@@ -516580,15 +516604,15 @@
   offprint: false
   isbn: 960-343-144-3
   original_entry:
     0: 10462
     1: ΣΠΥΡΑΝΤΗ,ΑΝΔΡΕΑ
     2: ΤΡΑΠΕΖΟΥΣ ΚΑΙ Η ΜΟΝΗ ΣΟΥΜΕΛΑ ΤΟΥ ΠΟΝΤΟΥ
     3: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΑ ΧΡΟΝΙΑ 1910-1922
-    4: 938.993ΣΠΥ
+    4: 938.498ΣΠΥ
     5: '13041'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1991'
     11: 110Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516715,15 +516739,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 10465
   authors:
   - ΛΑΠΑΡΙΔΗ,ΝΙΚΟΥ
   title: Η ΜΑΤΣΟΥΚΑ ΤΟΥ ΠΟΝΤΟΥ
-  dewey: 938.993 ΛΑΠ
+  dewey: 938.498 ΛΑΠ
   entry_numbers:
   - '13039'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1996
   pages: 181
   topics:
   - ΠΟΝΤΟΣ
@@ -516735,15 +516759,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-378-0
   original_entry:
     0: 10465
     1: ΛΑΠΑΡΙΔΗ,ΝΙΚΟΥ
     2: Η ΜΑΤΣΟΥΚΑ ΤΟΥ ΠΟΝΤΟΥ
-    4: 938.993ΛΑΠ
+    4: 938.498ΛΑΠ
     5: '13039'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1996'
     11: 181Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -516767,15 +516791,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10466
   authors:
   - ΠΑΠΑΔΟΠΟΥΛΟΣ,ΓΙΩΡΓΟΣ
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΑΥΛΗΑΝΝΑΣ
-  dewey: 938.993 ΠΑΠ
+  dewey: 938.498 ΠΑΠ
   entry_numbers:
   - '13037'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2000
   pages: 175
   topics:
   - ΠΟΝΤΟΣ
@@ -516787,15 +516811,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-520-1
   original_entry:
     0: 10466
     1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΓΙΩΡΓΟΣ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΥΛΗΑΝΝΑΣ
-    4: 938.993ΠΑΠ
+    4: 938.498ΠΑΠ
     5: '13037'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2000'
     11: 175Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -517233,15 +517257,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10475
   authors:
   - ΚΟΥΛΟΧΕΡΗ,ΙΑΚΩΒΟΣ
   title: Η ΑΜΙΣΟΣ ΚΑΙ ΤΑ ΠΑΘΗ ΤΗΣ
-  dewey: 938.993 ΚΟΥ
+  dewey: 938.498 ΚΟΥ
   entry_numbers:
   - '13047'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1991
   pages: 151
   topics:
   - ΠΟΝΤΟΣ
@@ -517253,15 +517277,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-088-9
   original_entry:
     0: 10475
     1: ΚΟΥΛΟΧΕΡΗ,ΙΑΚΩΒΟΣ
     2: Η ΑΜΙΣΟΣ ΚΑΙ ΤΑ ΠΑΘΗ ΤΗΣ
-    4: 938.993ΚΟΥ
+    4: 938.498ΚΟΥ
     5: '13047'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1991'
     11: 151Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -517285,15 +517309,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10476
   authors:
   - ΤΣΑΡΤΙΛΙΔΗ,ΧΡΗΣΤΟΥ
   title: Η ΚΡΩΜΝΗ
-  dewey: 938.993 ΤΣΑ
+  dewey: 938.498 ΤΣΑ
   entry_numbers:
   - '13046'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 192
   topics:
   - ΠΟΝΤΟΣ
@@ -517305,15 +517329,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-343-954-7
   original_entry:
     0: 10476
     1: ΤΣΑΡΤΙΛΙΔΗ,ΧΡΗΣΤΟΥ
     2: Η ΚΡΩΜΝΗ
-    4: 938.993ΤΣΑ
+    4: 938.498ΤΣΑ
     5: '13046'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2007'
     11: 192Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -517390,15 +517414,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10478
   authors:
   - ΤΣΑΝΙΚΛΙΔΗ,ΚΩΝ/ΝΟ
   title: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΟΝ ΠΟΝΤΟ
-  dewey: 938.993 ΤΣΑ
+  dewey: 938.498 ΤΣΑ
   entry_numbers:
   - '13044'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2002
   pages: 167
   topics:
   - ΠΟΝΤΟΣ
@@ -517410,15 +517434,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-625-9
   original_entry:
     0: 10478
     1: ΤΣΑΝΙΚΛΙΔΗ,ΚΩΝ/ΝΟ
     2: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΟΝ ΠΟΝΤΟ
-    4: 938.993ΤΣΑ
+    4: 938.498ΤΣΑ
     5: '13044'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2002'
     11: 167Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -517442,15 +517466,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10479
   authors:
   - ΤΑΞΙΔΗ,ΕΥΣΤΑΘΙΟΥ
   title: ΑΠΟ ΤΗΝ ΤΣΙΜΕΡΑ ΤΟΥ ΠΟΝΤΟΥ ΣΤΗΝ ΕΛΛΑΔΑ
-  dewey: 938.993 ΤΑΞ
+  dewey: 938.498 ΤΑΞ
   entry_numbers:
   - '13061'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 448
   topics:
   - ΠΟΝΤΟΣ
@@ -517462,15 +517486,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-343-909-7
   original_entry:
     0: 10479
     1: ΤΑΞΙΔΗ,ΕΥΣΤΑΘΙΟΥ
     2: ΑΠΟ ΤΗΝ ΤΣΙΜΕΡΑ ΤΟΥ ΠΟΝΤΟΥ ΣΤΗΝ ΕΛΛΑΔΑ
-    4: 938.993ΤΑΞ
+    4: 938.498ΤΑΞ
     5: '13061'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2007'
     11: 448Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -517754,15 +517778,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10485
   authors:
   - ΚΑΙΚΟΥΝΙΔΗΣ,ΜΙΧΑΗΛ
   title: ΣΑΜΨΟΥΝΤΑ ΠΟΛΗ ΤΗΣ ΦΩΤΙΑΣ
-  dewey: 938.993 ΚΑΙ
+  dewey: 938.498 ΚΑΙ
   entry_numbers:
   - '13053'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2009
   pages: 218
   topics:
   - ΠΟΝΤΟΣ
@@ -517774,15 +517798,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-467-118-2
   original_entry:
     0: 10485
     1: ΚΑΙΚΟΥΝΙΔΗΣ,ΜΙΧΑΗΛ
     2: ΣΑΜΨΟΥΝΤΑ ΠΟΛΗ ΤΗΣ ΦΩΤΙΑΣ
-    4: 938.993ΚΑΙ
+    4: 938.498ΚΑΙ
     5: '13053'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2009'
     11: 218Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -520485,15 +520509,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10538
   authors:
   - ΚΑΝΕΩΣ-ΚΑΝΔΗΛΑΤΟΥ,ΓΕΩΡΓΙΟΥ
   title: ΠΟΝΤΙΑΚΑΙ ΑΝΑΜΝΗΣΕΙΣ
-  dewey: 938.498 ΚΑΝ
+  dewey: 938.4 ΚΑΝ
   entry_numbers:
   - '13115'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1965
   pages: 72
   topics:
   - ΠΟΝΤΟΣ
@@ -520503,15 +520527,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10538
     1: ΚΑΝΕΩΣ-ΚΑΝΔΗΛΑΤΟΥ,ΓΕΩΡΓΙΟΥ
     2: ΠΟΝΤΙΑΚΑΙ ΑΝΑΜΝΗΣΕΙΣ
-    4: 938.498ΚΑΝ
+    4: 938.4ΚΑΝ
     5: '13115'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1965'
     11: 72Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -520535,15 +520559,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10539
   authors:
   - ΚΑΝΕΩΣ-ΚΑΝΔΗΛΑΤΟΥ,ΓΕΩΡΓΙΟΥ
   title: Ο ΕΛΛΗΝΟΜΗΜΩΝ ΤΟΥ ΠΟΝΤΟΥ
-  dewey: 938.498 ΚΑΝ
+  dewey: 938.4 ΚΑΝ
   entry_numbers:
   - '13116'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2006
   pages: 256
   topics:
   - ΠΟΝΤΟΣ
@@ -520554,15 +520578,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-908-8
   original_entry:
     0: 10539
     1: ΚΑΝΕΩΣ-ΚΑΝΔΗΛΑΤΟΥ,ΓΕΩΡΓΙΟΥ
     2: Ο ΕΛΛΗΝΟΜΗΜΩΝ ΤΟΥ ΠΟΝΤΟΥ
-    4: 938.498ΚΑΝ
+    4: 938.4ΚΑΝ
     5: '13116'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2006'
     11: 256Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -521654,17 +521678,17 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10561
   authors:
-  - BENESEVIC,V.N
+  - USPENSKIJ,F.I-BENESEVIC,V.N
   title: ΤΑ ACTA ΤΗΣ ΜΟΝΗΣ ΒΑΖΕΛΩΝΟΣ
-  dewey: 938.498 BEN
+  dewey: 938.498 USP
   entry_numbers:
   - '13109'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 391
   topics:
   - ΠΟΝΤΟΣ
@@ -521673,17 +521697,17 @@
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-343-958-5
   original_entry:
     0: 10561
-    1: BENESEVIC,V.N
+    1: USPENSKIJ,F.I-BENESEVIC,V.N
     2: ΤΑ ACTA ΤΗΣ ΜΟΝΗΣ ΒΑΖΕΛΩΝΟΣ
-    4: 938.498BEN
+    4: 938.498USP
     5: '13109'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2007'
     11: 391Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -521862,46 +521886,45 @@
     28: null
     29: null
 - dbase_number: 10565
   authors:
   - ΑΠΟΣΤΟΛΙΔΗ,ΠΑΥΛΟΥ
   title: Η ΜΗΤΡΟΠΟΛΙΣ ΡΟΔΟΠΟΛΕΩΣ
   subtitle: ΤΟ ΖΗΤΗΜΑ ΤΩΝ ΕΞΑΡΧΙΩΝ ΤΟΥ ΠΟΝΤΟΥ
-  dewey: 956.5 ΑΠΟ
+  dewey: 938.498 ΑΠΟ
   entry_numbers:
   - '12958'
   - '16967'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 480
   topics:
   - ΠΟΝΤΟΣ
-  - ΘΡΗΣΚΕΙΑ
   copies: 4
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   - ΣΩΜΑΤΕΙΟ ΠΑΝΑΓΙΑΣ ΣΟΥΜΕΛΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-343-968-4
   original_entry:
     0: 10565
     1: ΑΠΟΣΤΟΛΙΔΗ,ΠΑΥΛΟΥ
     2: Η ΜΗΤΡΟΠΟΛΙΣ ΡΟΔΟΠΟΛΕΩΣ
     3: ΤΟ ΖΗΤΗΜΑ ΤΩΝ ΕΞΑΡΧΙΩΝ ΤΟΥ ΠΟΝΤΟΥ
-    4: 956.5ΑΠ0
+    4: 938.498ΑΠΟ
     5: 12958-16967
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2007'
     11: 480Σ
-    12: ΠΟΝΤΟΣ-ΘΡΗΣΚΕΙΑ
-    13: ΠΟΝΤΟΣ-ΘΡΗΣΚΕΙΑ
-    14: ΠΟΝΤΟΣ-ΘΡΗΣΚΕΙΑ
+    12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ ΔΩΡΕΑ ΣΩΜΑΤΕΙΟΥ ΠΑΝΑΓΙΑΣ ΣΟΥΜΕΛΑ
     18: 978-960-34
     19: 3-968-4
     30: 2 ΑΝΤΙΤΥΠΑ  &  2 ΑΝΤΙΤΥΠΑ
     6: null
     7: null
     15: null
@@ -522594,43 +522617,42 @@
     28: null
     29: null
     30: null
 - dbase_number: 10579
   authors:
   - ΒΗΣΣΑΡΙΩΝΟΣ
   title: ΕΓΚΩΜΙΟΝ ΕΙΣ ΤΡΑΠΕΖΟΥΝΤΑ
-  dewey: 230 ΒΗΣ
+  dewey: 938.498 ΒΗΣ
   entry_numbers:
   - '12950'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2000
   pages: 62
   topics:
   - ΠΟΝΤΟΣ
-  - ΕΓΚΩΜΙΑ
   copies: 2
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-343-556-2
   original_entry:
     0: 10579
     1: ΒΗΣΣΑΡΙΩΝΟΣ
     2: ΕΓΚΩΜΙΟΝ ΕΙΣ ΤΡΑΠΕΖΟΥΝΤΑ
-    4: 230ΒΗΣ
+    4: 938.498ΒΗΣ
     5: '12950'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2000'
     11: 62Σ
-    12: ΠΟΝΤΟΣ-ΕΓΚΩΜΙΑ
-    13: ΠΟΝΤΟΣ-ΕΓΚΩΜΙΑ
-    14: ΠΟΝΤΟΣ-ΕΓΚΩΜΙΑ
+    12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     18: 960-343-55
     19: 6-2
     30: 2 ΑΝΤΙΤΥΠΑ
     3: null
     6: null
     7: null
@@ -525421,15 +525443,15 @@
     28: null
     29: null
 - dbase_number: 10634
   authors:
   - ΟΡΦΑΝΙΔΟΥ,ΕΛΕΝΗ
   title: ΤΟ ΧΩΡΙΟ ΜΟΥ ΤΑΧΤΑΡΓΑΝ (ΚΑΡΣ-ΚΑΥΚΑΣΟΥ)
   subtitle: ΒΙΟΓΡΑΦΙΑ ΠΑΥΛΟΥ ΟΡΦΑΝΙΔΗ
-  dewey: 938.993 ΟΡΦ
+  dewey: 938.498 ΟΡΦ
   entry_numbers:
   - '13063'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2006
   pages: 80
   topics:
   - ΠΟΝΤΟΣ
@@ -525442,15 +525464,15 @@
   offprint: false
   isbn: 960-343-911-8
   original_entry:
     0: 10634
     1: ΟΡΦΑΝΙΔΟΥ,ΕΛΕΝΗ
     2: ΤΟ ΧΩΡΙΟ ΜΟΥ ΤΑΧΤΑΡΓΑΝ (ΚΑΡΣ-ΚΑΥΚΑΣΟΥ)
     3: ΒΙΟΓΡΑΦΙΑ ΠΑΥΛΟΥ ΟΡΦΑΝΙΔΗ
-    4: 938.993ΟΡΦ
+    4: 938.498ΟΡΦ
     5: '13063'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2006'
     11: 80Σ
     12: ΠΟΝΤΟΣ-ΑΥΤΟΒΙΟΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΑΥΤΟΒΙΟΓΡΑΦΙΑ
@@ -526302,15 +526324,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10651
   authors:
   - ΒΑΛΑΒΑΝΗ,ΓΕΩΡΓΙΟΥ
   title: ΣΥΓΧΡΟΝΟΣ ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ
-  dewey: 938.498 ΒΑΛ
+  dewey: 938.4 ΒΑΛ
   entry_numbers:
   - '13088'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1986
   pages: 317
   topics:
   - ΠΟΝΤΟΣ
@@ -526321,15 +526343,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-343-281-4
   original_entry:
     0: 10651
     1: ΒΑΛΑΒΑΝΗ,ΓΕΩΡΓΙΟΥ
     2: ΣΥΓΧΡΟΝΟΣ ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ
-    4: 938.498ΒΑΛ
+    4: 938.4ΒΑΛ
     5: '13088'
     8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1986'
     11: 317Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -527681,15 +527703,15 @@
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10677
   authors:
   - ΛΑΥΡΕΝΤΙΔΗ,ΙΣΑΑΚ
-  title: ΟΙ ΕΚ ΣΟΒΙΕΤΙΚΗΕ ΕΝΩΣΕΩΣ ΕΛΛΗΝΕΣ ΠΟΝΤΙΑΚΗΣ ΚΑΤΑΓΩΓΗΣ ΚΑΙ ΤΑ
+  title: ΟΙ ΕΚ ΣΟΒΙΕΤΙΚΗΣ ΕΝΩΣΕΩΣ ΕΛΛΗΝΕΣ ΠΟΝΤΙΑΚΗΣ ΚΑΤΑΓΩΓΗΣ ΚΑΙ ΤΑ
   subtitle: ΕΚ ΤΗΣ ΣΥΝΘΗΚΗΣ ΤΗΣ ΛΩΖΑΝΗΣ ΔΙΚΑΙΩΜΑΤΑ ΤΩΝ
   dewey: 938.498 ΛΑΥ
   entry_numbers:
   - '12536'
   editor: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ // ΑΘΗΝΑ
   edition_year: 1986
   pages: 168
@@ -527702,15 +527724,15 @@
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10677
     1: ΛΑΥΡΕΝΤΙΔΗ,ΙΣΑΑΚ
-    2: ΟΙ ΕΚ ΣΟΒΙΕΤΙΚΗΕ ΕΝΩΣΕΩΣ ΕΛΛΗΝΕΣ ΠΟΝΤΙΑΚΗΣ ΚΑΤΑΓΩΓΗΣ ΚΑΙ ΤΑ
+    2: ΟΙ ΕΚ ΣΟΒΙΕΤΙΚΗΣ ΕΝΩΣΕΩΣ ΕΛΛΗΝΕΣ ΠΟΝΤΙΑΚΗΣ ΚΑΤΑΓΩΓΗΣ ΚΑΙ ΤΑ
     3: ΕΚ ΤΗΣ ΣΥΝΘΗΚΗΣ ΤΗΣ ΛΩΖΑΝΗΣ ΔΙΚΑΙΩΜΑΤΑ ΤΩΝ
     4: 938.498ΛΑΥ
     5: '12536'
     8: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ
     9: ΑΘΗΝΑ
     10: '1986'
     11: 168Σ
@@ -527947,15 +527969,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10682
   authors:
   - ΚΩΝΣΤΑΝΤΙΝΙΔΟΥ-ΒΑΡΒΕΡΗ,ΔΕΣΠΟΙΝΑ
   title: ΤΑ ΣΩΖΟΜΕΝΑ ΕΓΓΡΑΦΑ ΤΗΣ ΕΠΙΤΡΟΠΕΙΑΣ ΠΟΝΤΙΩΝ ΕΛΛΗΝΩΝ ΚΩΝ/ΠΟΛΕ
-  dewey: 938.498 ΚΩΝ
+  dewey: 938.498 ΒΑΡ
   entry_numbers:
   - '12592'
   editor: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ // ΑΘΗΝΑ
   edition_year: 2012
   pages: 702
   topics:
   - ΠΟΝΤΟΣ
@@ -527967,15 +527989,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10682
     1: ΚΩΝΣΤΑΝΤΙΝΙΔΟΥ-ΒΑΡΒΕΡΗ,ΔΕΣΠΟΙΝΑ
     2: ΤΑ ΣΩΖΟΜΕΝΑ ΕΓΓΡΑΦΑ ΤΗΣ ΕΠΙΤΡΟΠΕΙΑΣ ΠΟΝΤΙΩΝ ΕΛΛΗΝΩΝ ΚΩΝ/ΠΟΛΕ
-    4: 938.498ΚΩΝ
+    4: 938.498ΒΑΡ
     5: '12592'
     8: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ
     9: ΑΘΗΝΑ
     10: '2012'
     11: 702Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -527999,15 +528021,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10683
   authors:
   - ΛΑΜΨΙΔΟΥ,ΟΔ.
   title: ΑΝΔΡΕΟΥ ΛΙΒΑΔΗΝΟΥ ΒΙΟΣ ΚΑΙ ΕΡΓΑ
-  dewey: 938.993 ΛΑΜ
+  dewey: 938.498 ΛΑΜ
   entry_numbers:
   - '12524'
   editor: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ // ΑΘΗΝΑ
   edition_year: 1975
   pages: 296
   topics:
   - ΠΟΝΤΟΣ
@@ -528020,15 +528042,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10683
     1: ΛΑΜΨΙΔΟΥ,ΟΔ.
     2: ΑΝΔΡΕΟΥ ΛΙΒΑΔΗΝΟΥ ΒΙΟΣ ΚΑΙ ΕΡΓΑ
-    4: 938.993ΛΑΜ
+    4: 938.498ΛΑΜ
     5: '12524'
     8: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ
     9: ΑΘΗΝΑ
     10: '1975'
     11: 296Σ
     12: ΠΟΝΤΟΣ-ΒΙΟΓΡΑΦΙΑ
     13: ΠΟΝΤΟΣ-ΒΙΟΓΡΑΦΙΑ
@@ -528907,15 +528929,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 10701
   authors:
   - ΝΑΝΑΚΗΣ,ΑΝΔΡΕΑΣ
   title: ΜΙΚΡΑ ΑΣΙΑ ΠΡΟΣΦΥΓΙΚΑ ΑΤΕΛΕΥΤΗΤΑ
-  dewey: 938.498 ΝΑΝ
+  dewey: 938.499 ΝΑΝ
   entry_numbers:
   - '13149'
   - '19961'
   editor: ΑΝΤ.ΣΤΑΜΟΥΛΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2012
   pages: 248
   topics:
@@ -528927,15 +528949,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-9533-41-6
   original_entry:
     0: 10701
     1: ΝΑΝΑΚΗΣ,ΑΝΔΡΕΑΣ
     2: ΜΙΚΡΑ ΑΣΙΑ ΠΡΟΣΦΥΓΙΚΑ ΑΤΕΛΕΥΤΗΤΑ
-    4: 938.498ΝΑΝ
+    4: 938.499ΝΑΝ
     5: 13149-19961
     8: ΑΝΤ.ΣΤΑΜΟΥΛΗΣ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2012'
     11: 248Σ
     12: ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
     13: ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
@@ -529204,38 +529226,39 @@
     28: null
     29: null
     30: null
 - dbase_number: 10707
   authors:
   - ΛΥΤ,ΧΡΙΣΤΙΑΝΑ
   title: ΜΙΑ ΔΑΝΕΖΑ ΣΤΗΝ ΑΥΛΗ ΤΟΥ ΟΘΩΝΑ
-  dewey: 889.21 ΛΥΤ
+  dewey: 938.009 ΛΥΤ
   entry_numbers:
   - '12425'
   editor: ΕΡΜΗΣ // ΑΘΗΝΑ
   edition_year: 1988
   pages: 366
   topics:
-  - ΛΟΓΟΤΕΧΝΙΑ
+  - ΜΑΡΤΥΡΙΑ
+  - ΙΣΤΟΡΙΚΗ ΜΑΡΤΥΡΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10707
     1: ΛΥΤ,ΧΡΙΣΤΙΑΝΑ
     2: ΜΙΑ ΔΑΝΕΖΑ ΣΤΗΝ ΑΥΛΗ ΤΟΥ ΟΘΩΝΑ
-    4: 889.21ΛΥΤ
+    4: 938.009ΛΥΤ
     5: '12425'
     8: ΕΡΜΗΣ
     9: ΑΘΗΝΑ
     10: '1988'
     11: 366Σ
-    12: ΛΟΓΟΤΕΧΝΙΑ
-    13: ΛΟΓΟΤΕΧΝΙΑ
-    14: ΛΟΓΟΤΕΧΝΙΑ
+    12: ΙΣΤΟΡΙΑ-ΜΑΡΤΥΡΙΑ
+    13: ΜΑΡΤΥΡΙΑ
+    14: ΙΣΤΟΡΙΚΗ ΜΑΡΤΥΡΙΑ
     3: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
@@ -530115,41 +530138,40 @@
     27: null
     28: null
     29: null
 - dbase_number: 10725
   authors:
   - ΑΝΔΡΕΑΔΗ,ΓΕΩΡΓΙΟΥ
   title: ΤΟ ΤΣΑΓΡΑΚ ΤΗΣ ΚΕΡΑΣΟΥΝΤΑΣ ΤΟΥ ΠΟΝΤΟΥ
-  dewey: 398 ΑΝΔ
+  dewey: 938.498 ΑΝΔ
   entry_numbers:
   - '13182'
   editor: None // ΑΘΗΝΑ
   edition_year: 1999
   pages: 214
   topics:
   - ΠΟΝΤΟΣ
-  - ΛΑΟΓΡΑΦΙΑ
   copies: 2
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10725
     1: ΑΝΔΡΕΑΔΗ,ΓΕΩΡΓΙΟΥ
     2: ΤΟ ΤΣΑΓΡΑΚ ΤΗΣ ΚΕΡΑΣΟΥΝΤΑΣ ΤΟΥ ΠΟΝΤΟΥ
-    4: 398ΑΝΔ
+    4: 938.498ΑΝΔ
     5: '13182'
     9: ΑΘΗΝΑ
     10: '1999'
     11: 214Σ
-    12: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
-    13: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
-    14: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
+    12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     30: 2 ΑΝΤΙΤΥΠΑ
     3: null
     6: null
     7: null
     8: null
     15: null
@@ -530526,14 +530548,15 @@
 - dbase_number: 10733
   authors: []
   title: Ο ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΜΑΥΡΗΣ ΘΑΛΑΣΣΑΣ
   subtitle: ΠΟΝΤΟΣ-ΡΩΣΙΑ
   dewey: 938.498 ΧΣ
   entry_numbers:
   - '13203'
+  - '21362'
   editor: None // ΑΘΗΝΑ
   edition_year: 1996
   pages: 188
   topics:
   - ΠΟΝΤΟΣ
   copies: 2
   donors:
@@ -530543,15 +530566,15 @@
   offprint: false
   original_entry:
     0: 10733
     1: Χ.Σ.
     2: Ο ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΜΑΥΡΗΣ ΘΑΛΑΣΣΑΣ
     3: ΠΟΝΤΟΣ-ΡΩΣΙΑ
     4: 938.498Χ.Σ
-    5: '13203'
+    5: 13203-21362
     9: ΑΘΗΝΑ
     10: '1996'
     11: 188Σ
     12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
@@ -530880,15 +530903,15 @@
     29: null
 - dbase_number: 10740
   authors:
   - ΑΡΓΥΡΟΣ,ΑΝΤΩΝΗΣ
   title: ΤΟ ΝΟΜΙΚΟ ΚΑΘΕΣΤΩΣ ΤΩΝ ΠΑΛΙΝΝΟΥΣΤΟΥΝΤΩΝ
   dewey: 938.498 ΑΡΓ
   entry_numbers:
-  - '13989'
+  - '13189'
   editor: None // ΑΘΗΝΑ
   edition_year: 1996
   pages: 415
   topics:
   - ΠΟΝΤΟΣ
   - ΠΡΟΣΦΥΓΕΣ
   donors:
@@ -530897,15 +530920,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 10740
     1: ΑΡΓΥΡΟΣ,ΑΝΤΩΝΗΣ
     2: ΤΟ ΝΟΜΙΚΟ ΚΑΘΕΣΤΩΣ ΤΩΝ ΠΑΛΙΝΝΟΥΣΤΟΥΝΤΩΝ
     4: 938.498ΑΡΓ
-    5: '13989'
+    5: '13189'
     9: ΑΘΗΝΑ
     10: '1996'
     11: 415Σ
     12: ΠΟΝΤΟΣ-ΠΡΟΣΦΥΓΕΣ
     13: ΠΟΝΤΟΣ-ΠΡΟΣΦΥΓΕΣ
     14: ΠΟΝΤΟΣ-ΠΡΟΣΦΥΓΕΣ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
@@ -531078,42 +531101,41 @@
     28: null
     29: null
     30: null
 - dbase_number: 10744
   authors:
   - ΠΑΥΛΙΔΗΣ,ΑΝΤΩΝΗΣ
   title: Ο ΓΚΙΟΥΛΜΠΑΞΕΣ ΕΡΥΘΡΑΙΑΣ
-  dewey: 398 ΠΑΥ
+  dewey: 938.498 ΠΑΥ
   entry_numbers:
   - '13185'
   editor: None // ΑΘΗΝΑ
   edition_year: 2010
   pages: 187
   topics:
   - ΠΟΝΤΟΣ
-  - ΛΑΟΓΡΑΦΙΑ
   copies: 2
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-99299-0-5
   original_entry:
     0: 10744
     1: ΠΑΥΛΙΔΗΣ,ΑΝΤΩΝΗΣ
     2: Ο ΓΚΙΟΥΛΜΠΑΞΕΣ ΕΡΥΘΡΑΙΑΣ
-    4: 398ΠΑΥ
+    4: 938.498ΠΑΥ
     5: '13185'
     9: ΑΘΗΝΑ
     10: '2010'
     11: 187Σ
-    12: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
-    13: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
-    14: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
+    12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     18: 978-960-99
     19: 299-0-5
     30: 2 ΑΝΤΙΤΥΠΑ
     3: null
     6: null
     7: null
@@ -535753,15 +535775,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10837
   authors: []
   title: Η ΓΕΝΟΚΤΟΝΙΑ ΤΟΥ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  dewey: 938.993 ΧΣ
+  dewey: 938.498 ΧΣ
   entry_numbers:
   - '13404'
   - '13945'
   editor: Ο.Π.Σ.Ν.Ε // ΑΘΗΝΑ
   edition_year: 1996
   pages: 16
   topics:
@@ -535772,15 +535794,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10837
     1: Χ.Σ.
     2: Η ΓΕΝΟΚΤΟΝΙΑ ΤΟΥ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
-    4: 938.993Χ.Σ
+    4: 938.498Χ.Σ
     5: 13404-13945
     8: Ο.Π.Σ.Ν.Ε
     9: ΑΘΗΝΑ
     10: '1996'
     11: 16Σ
     12: ΙΣΤΟΡΙΑ-ΓΕΝΟΚΤΟΝΙΑ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
     13: ΙΣΤΟΡΙΑ-ΓΕΝΟΚΤΟΝΙΑ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
@@ -536611,15 +536633,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 10854
   authors:
   - ΜΙΧΑΗΛΙΔΗΣ,ΧΡΗΣΤΟΣ-ΑΘΑΝΑΣΙΑΔΗΣ,ΑΝΔΡΕΑΣ
   title: ΓΕΝΝΗΘΕΙΣ ΕΙΣ ΚΑΥΚΑΣΟΝ ΡΩΣΙΑΣ
-  dewey: 938.498 ΜΙΧ
+  dewey: 938.498 ΑΘΑ
   entry_numbers:
   - '13451'
   editor: ΙΝΦΟΓΝΩΜΩΝ // ΑΘΗΝΑ
   edition_year: 2010
   pages: 384
   topics:
   - ΠΟΝΤΟΣ
@@ -536630,15 +536652,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-836-240-7
   original_entry:
     0: 10854
     1: ΜΙΧΑΗΛΙΔΗΣ,ΧΡΗΣΤΟΣ-ΑΘΑΝΑΣΙΑΔΗΣ,ΑΝΔΡΕΑΣ
     2: ΓΕΝΝΗΘΕΙΣ ΕΙΣ ΚΑΥΚΑΣΟΝ ΡΩΣΙΑΣ
-    4: 938.498ΜΙΧ
+    4: 938.498ΑΘΑ
     5: '13451'
     8: ΙΝΦΟΓΝΩΜΩΝ
     9: ΑΘΗΝΑ
     10: '2010'
     11: 384Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -536816,17 +536838,17 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10858
   authors:
-  - ΚΥΠΑΡΛΗ-ΑΚΡΙΤΙΔΟΥ,ΕΛΙΣΑΒΕΤ
+  - ΑΚΡΙΤΙΔΟΥ-ΚΥΠΑΡΛΗ,ΕΛΙΣΑΒΕΤ
   title: Η ΧΡΥΣΑΝΝΑ ΤΟΥ ΠΟΝΤΟΥ
-  dewey: 938.498 ΚΥΠ
+  dewey: 938.498 ΑΚΡ
   entry_numbers:
   - '13444'
   editor: ΙΝΦΟΓΝΩΜΩΝ // ΑΘΗΝΑ
   edition_year: 2012
   pages: 84
   topics:
   - ΠΟΝΤΟΣ
@@ -536835,17 +536857,17 @@
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-836-250-4
   original_entry:
     0: 10858
-    1: ΚΥΠΑΡΛΗ-ΑΚΡΙΤΙΔΟΥ,ΕΛΙΣΑΒΕΤ
+    1: ΑΚΡΙΤΙΔΟΥ-ΚΥΠΑΡΛΗ,ΕΛΙΣΑΒΕΤ
     2: Η ΧΡΥΣΑΝΝΑ ΤΟΥ ΠΟΝΤΟΥ
-    4: 938.498ΚΥΠ
+    4: 938.498ΑΚΡ
     5: '13444'
     8: ΙΝΦΟΓΝΩΜΩΝ
     9: ΑΘΗΝΑ
     10: '2012'
     11: 84Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -537731,15 +537753,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 10876
   authors:
   - ΓΑΛΑΝΙΔΟΥ-ΜΠΑΛΦΟΥΣΙΑ,ΕΛΣΑ
   title: ΕΞΟΧΕΣ ΚΑΙ ΠΑΡΧΑΡΙΑ ΤΗΣ ΤΡΑΠΕΖΟΥΝΤΑΣ
-  dewey: 938.498 ΓΑΛ
+  dewey: 938.498 ΜΠΑ
   entry_numbers:
   - '13434'
   editor: ΕΝ.ΠΟΝ.ΜΕΛΙΣΣΙΩΝ ΑΤΤ // ΑΘΗΝΑ
   edition_year: 1982
   pages: 20
   topics:
   - ΠΟΝΤΟΣ
@@ -537749,15 +537771,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10876
     1: ΓΑΛΑΝΙΔΟΥ-ΜΠΑΛΦΟΥΣΙΑ,ΕΛΣΑ
     2: ΕΞΟΧΕΣ ΚΑΙ ΠΑΡΧΑΡΙΑ ΤΗΣ ΤΡΑΠΕΖΟΥΝΤΑΣ
-    4: 938.498ΓΑΛ
+    4: 938.498ΜΠΑ
     5: '13434'
     8: ΕΝ.ΠΟΝ.ΜΕΛΙΣΣΙΩΝ ΑΤΤ
     9: ΑΘΗΝΑ
     10: '1982'
     11: 20Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -537781,15 +537803,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 10877
   authors:
   - ΓΑΛΑΝΙΔΟΥ-ΜΠΑΛΦΟΥΣΙΑ,ΕΛΣΑ
   title: ΟΙ ΕΛΛΗΝΕΣ ΤΟΥ ΠΟΝΤΟΥ ΚΙ Η ΠΑΝΑΓΙΑ ΣΟΥΜΕΛΑ
-  dewey: 938.498 ΓΑΛ
+  dewey: 938.498 ΜΠΑ
   entry_numbers:
   - '13433'
   editor: ΕΝ.ΠΟΝ.ΜΕΛΙΣΣΙΩΝ ΑΤΤ // ΑΘΗΝΑ
   edition_year: 1997
   pages: 29
   topics:
   - ΠΟΝΤΟΣ
@@ -537798,15 +537820,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10877
     1: ΓΑΛΑΝΙΔΟΥ-ΜΠΑΛΦΟΥΣΙΑ,ΕΛΣΑ
     2: ΟΙ ΕΛΛΗΝΕΣ ΤΟΥ ΠΟΝΤΟΥ ΚΙ Η ΠΑΝΑΓΙΑ ΣΟΥΜΕΛΑ
-    4: 938.498ΓΑΛ
+    4: 938.498ΜΠΑ
     5: '13433'
     8: ΕΝ.ΠΟΝ.ΜΕΛΙΣΣΙΩΝ ΑΤΤ
     9: ΑΘΗΝΑ
     10: '1997'
     11: 29Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -539919,15 +539941,15 @@
     28: null
     29: null
 - dbase_number: 10920
   authors:
   - ΡΟΔΑΚΗΣ,ΠΕΡΙΚΛΗΣ
   title: Η ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ Α)ΑΠΟ ΤΑ ΜΥΘΙΚΑ ΧΡΟΝΙΑ ΩΣ ΤΗΝ ΤΟΥΡΚΙΚΗ
   subtitle: ΚΑΤΑΚΤΗΣΗ Β)ΑΠΟ ΤΗΝ ΤΟΥΡΚΙΚΗ ΚΑΤΑΚΤΗΣΗ ΩΣ ΤΗ ΓΕΝΟΚΤΟΝΙΑ
-  dewey: 938.498 ΡΟΔ
+  dewey: 938.4 ΡΟΔ
   entry_numbers:
   - '13486'
   editor: ΓΟΡΔΙΟΣ // ΑΘΗΝΑ
   edition_year: 2004
   pages: 415
   topics:
   - ΠΟΝΤΟΣ
@@ -539939,15 +539961,15 @@
   offprint: false
   isbn: 960-7083-55-5
   original_entry:
     0: 10920
     1: ΡΟΔΑΚΗΣ,ΠΕΡΙΚΛΗΣ
     2: Η ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ Α)ΑΠΟ ΤΑ ΜΥΘΙΚΑ ΧΡΟΝΙΑ ΩΣ ΤΗΝ ΤΟΥΡΚΙΚΗ
     3: ΚΑΤΑΚΤΗΣΗ Β)ΑΠΟ ΤΗΝ ΤΟΥΡΚΙΚΗ ΚΑΤΑΚΤΗΣΗ ΩΣ ΤΗ ΓΕΝΟΚΤΟΝΙΑ
-    4: 938.498ΡΟΔ
+    4: 938.4ΡΟΔ
     5: '13486'
     8: ΓΟΡΔΙΟΣ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 415Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -540996,43 +541018,42 @@
     28: null
     29: null
 - dbase_number: 10941
   authors:
   - ΤΣΙΛΙΜΑΓΚΟΥ-ΕΥΣΤΑΘΙΑΔΟΥ,ΣΟΥΛΑ
   title: ΚΙ ΥΣΤΕΡΑ Ο ΞΕΡΙΖΩΜΟΣ
   subtitle: ΕΛΛΗΝΕΣ ΤΗΣ ΚΑΠΠΑΔΟΚΙΑΣ
-  dewey: 889.21 ΤΣΙ
+  dewey: 938.498 ΤΣΙ
   entry_numbers:
   - '13481'
   editor: ΓΟΡΔΙΟΣ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 238
-  topics:
-  - ΛΟΓΟΤΕΧΝΙΑ
+  topics: []
   copies: 2
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-7083-93-7
   original_entry:
     0: 10941
     1: ΤΣΙΛΙΜΑΓΚΟΥ-ΕΥΣΤΑΘΙΑΔΟΥ,ΣΟΥΛΑ
     2: ΚΙ ΥΣΤΕΡΑ Ο ΞΕΡΙΖΩΜΟΣ
     3: ΕΛΛΗΝΕΣ ΤΗΣ ΚΑΠΠΑΔΟΚΙΑΣ
-    4: 889.21ΤΣΙ
+    4: 938.498ΤΣΙ
     5: '13481'
     8: ΓΟΡΔΙΟΣ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 238Σ
-    12: ΛΟΓΟΤΕΧΝΙΑ
-    13: ΛΟΓΟΤΕΧΝΙΑ
-    14: ΛΟΓΟΤΕΧΝΙΑ
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     18: 978-960-70
     19: 83-93-7
     30: 2 ΑΝΤΙΤΥΠΑ
     6: null
     7: null
     15: null
@@ -543892,15 +543913,15 @@
 - dbase_number: 10998
   authors:
   - ΠΑΠΑΤΡΙΑΝΤΑΦΥΛΛΟΥ,ΑΘΑΝΑΣΙΟΣ
   title: ΘΡΑΚΗ ΙΣΤΟΡΙΕΣ ΖΩΗΣ
   subtitle: ΟΔΟΙΠΟΡΙΚΟ ΤΡΙΩΝ ΑΙΩΝΩΝ
   dewey: 938.498 ΠΑΠ
   entry_numbers:
-  - '13623'
+  - '13627'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΑΘΗΝΑ
   edition_year: 2008
   pages: 304
   topics:
   - ΘΡΑΚΗ
   copies: 2
   donors:
@@ -543911,15 +543932,15 @@
   ean: 978-960-467-060-4
   original_entry:
     0: 10998
     1: ΠΑΠΑΤΡΙΑΝΤΑΦΥΛΛΟΥ,ΑΘΑΝΑΣΙΟΣ
     2: ΘΡΑΚΗ ΙΣΤΟΡΙΕΣ ΖΩΗΣ
     3: ΟΔΟΙΠΟΡΙΚΟ ΤΡΙΩΝ ΑΙΩΝΩΝ
     4: 938.498ΠΑΠ
-    5: '13623'
+    5: '13627'
     8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 304Σ
     12: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
     13: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
     14: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
@@ -547961,15 +547982,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 11078
   authors:
   - ΓΙΑΝΝΟΥΛΑΤΣΟΥ-ΔΕΣΤΟΥΝΗ,ΜΑΡΙΑ-ΧΡΙΣΤΙΝΑ
   title: ΠΟΝΤΟΣ ΚΑΙ ΑΣΗΜΙ
-  dewey: 398 ΓΙΑ
+  dewey: 938.498 ΔΕΣ
   entry_numbers:
   - '13687'
   pages: 13
   topics:
   - ΜΟΥΣΕΙΟ ΜΠΕΝΑΚΗ
   copies: 2
   donors:
@@ -547978,15 +547999,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-8347-14-9
   original_entry:
     0: 11078
     1: ΓΙΑΝΝΟΥΛΑΤΣΟΥ-ΔΕΣΤΟΥΝΗ,ΜΑΡΙΑ-ΧΡΙΣΤΙΝΑ
     2: ΠΟΝΤΟΣ ΚΑΙ ΑΣΗΜΙ
-    4: 398ΓΙΑ
+    4: 938.498ΔΕΣ
     5: '13687'
     11: 13Σ
     12: ΜΟΥΣΕΙΟ ΜΠΕΝΑΚΗ
     13: ΜΟΥΣΕΙΟ ΜΠΕΝΑΚΗ
     14: ΜΟΥΣΕΙΟ ΜΠΕΝΑΚΗ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     18: 960-8347-1
@@ -550668,15 +550689,15 @@
     29: null
     30: null
 - dbase_number: 11132
   authors:
   - ΤΟΙΛΟΣ ΧΡΗΣΤΟΣ ΥΠΟΣΤΡΑΤΗΓΟΣ
   title: Η ΠΟΡΕΙΑ ΤΟΥ ΒΕΛΛΗΝΙΣΜΟΥ ΠΡΟΣ ΤΗΝ ΕΠΑΝΑΣΤΑΣΗ ΤΟΥ 1821
   subtitle: (ΣΥΝΟΔΕΥΕΤΑΙ ΑΠΟ 155 ΣΛΑΙΤΣ
-  dewey: '938.498'
+  dewey: 938.498 ΧΣ
   entry_numbers:
   - '13813'
   editor: None // ΜΕΛΙΣΣΙΑ
   edition_year: 2000
   pages: 56
   topics:
   - ΔΙΑΛΕΞΕΙΣ
@@ -550686,15 +550707,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 11132
     1: ΤΟΙΛΟΣ ΧΡΗΣΤΟΣ ΥΠΟΣΤΡΑΤΗΓΟΣ
     2: Η ΠΟΡΕΙΑ ΤΟΥ ΒΕΛΛΗΝΙΣΜΟΥ ΠΡΟΣ ΤΗΝ ΕΠΑΝΑΣΤΑΣΗ ΤΟΥ 1821
     3: (ΣΥΝΟΔΕΥΕΤΑΙ ΑΠΟ 155 ΣΛΑΙΤΣ
-    4: '938.498'
+    4: 938.498Χ.Σ
     5: '13813'
     9: ΜΕΛΙΣΣΙΑ
     10: '2000'
     11: 56Σ
     12: ΔΙΑΛΕΞΗ
     13: ΔΙΑΛΕΞΗ
     14: ΔΙΑΛΕΞΗ
@@ -551930,43 +551951,44 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11158
   authors:
-  - GRIECHISCHES PARLAMENT
+  - ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ
   title: ΠΕΡΙΚΛΕΟΥΣ ΕΠΙΤΑΦΙΟΣ
-  dewey: 938.498 GRI
+  dewey: 881 ΘΟΥ
   entry_numbers:
   - '13790'
+  pages: 25
   topics:
   - ΙΣΤΟΡΙΚΟ
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11158
-    1: GRIECHISCHES PARLAMENT
+    1: ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ
     2: ΠΕΡΙΚΛΕΟΥΣ ΕΠΙΤΑΦΙΟΣ
-    4: 938.498GRI
+    4: 881ΘΟΥ
     5: '13790'
+    11: '25'
     12: ΙΣΤΟΡΙΚΟ
     13: ΙΣΤΟΡΙΚΟ
     14: ΙΣΤΟΡΙΚΟ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     3: null
     6: null
     7: null
     8: null
     9: null
     10: null
-    11: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -558728,35 +558750,35 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11297
   authors:
-  - ΕΥΑΓΓΕΛΙΑ ΓΙΑΜΑΛΗ- ΧΑΖΤΗΙΩΑΝΝΟΥ
+  - ΧΑΤΖΗΙΩΑΝΝΟΥ-ΓΙΑΜΜΑΛΗ,ΕΥΑΓΓΕΛΙΑ
   title: ΜΙΚΡΑΣΙΑΤΙΚΟΣ ΕΛΛΗΝΙΣΜΟΣ
-  subtitle: ΟΔΟΙΠΟΡΙΚΟΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
-  dewey: 938.488 ΧΑΤ
+  subtitle: ΟΔΟΙΠΟΡΙΚΟ  ΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
+  dewey: 938.498 ΧΑΤ
   entry_numbers:
   - '14086'
   editor: None // ΝΙΚΑΙΑ
   edition_year: 2001
   pages: 55
   topics: []
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11297
-    1: ΕΥΑΓΓΕΛΙΑ ΓΙΑΜΑΛΗ- ΧΑΖΤΗΙΩΑΝΝΟΥ
+    1: ΧΑΤΖΗΙΩΑΝΝΟΥ-ΓΙΑΜΜΑΛΗ,ΕΥΑΓΓΕΛΙΑ
     2: ΜΙΚΡΑΣΙΑΤΙΚΟΣ ΕΛΛΗΝΙΣΜΟΣ
-    3: ΟΔΟΙΠΟΡΙΚΟΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
-    4: 938.488ΧΑΤ
+    3: ΟΔΟΙΠΟΡΙΚΟ  ΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
+    4: 938.498ΧΑΤ
     5: '14086'
     9: ΝΙΚΑΙΑ
     10: '2001'
     11: 55Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
@@ -559160,49 +559182,50 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11306
   authors:
-  - ΕΥΑΓΓΕΛΙΑ ΓΙΑΜΑΛΗ-ΧΑΤΖΗΙΩΑΝΝΟΥ
-  title: ΜΙΚΡΑΣΙΑΤΙΚΟΣ ΕΛΛΗΝΙΣΜΟΣ ΟΔΟΙΠΟΡΙΚΟΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
-  dewey: 938.498 ΧΑΤ
+  - ΚΑΛΠΟΥΖΟΣ,ΓΙΑΝΝΗΣ
+  title: ΚΑΛΝΤΕΡΙΜΙ 99ΧΡΟΝΙΑ ΣΤΗ ΣΑΛΟΝΙΚΗ
+  dewey: 889.21 ΚΑΛ
   entry_numbers:
-  - '14086'
-  editor: ΔΗΜΟΣ ΝΙΚΑΙΑΣ // None
-  edition_year: 2001
-  pages: 56
-  topics: []
-  donors:
-  - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
+  - '22886'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2023
+  pages: 576
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
+  ean: '9786180149234'
   original_entry:
     0: 11306
-    1: ΕΥΑΓΓΕΛΙΑ ΓΙΑΜΑΛΗ-ΧΑΤΖΗΙΩΑΝΝΟΥ
-    2: ΜΙΚΡΑΣΙΑΤΙΚΟΣ ΕΛΛΗΝΙΣΜΟΣ ΟΔΟΙΠΟΡΙΚΟΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
-    4: 938.498ΧΑΤ
-    5: '14086'
-    8: ΔΗΜΟΣ ΝΙΚΑΙΑΣ
-    10: '2001'
-    11: 56Σ
-    12: ΙΣΤΟΡΙΑ
-    13: ΙΣΤΟΡΙΑ
-    14: ΙΣΤΟΡΙΑ
-    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
+    1: ΚΑΛΠΟΥΖΟΣ,ΓΙΑΝΝΗΣ
+    2: ΚΑΛΝΤΕΡΙΜΙ 99ΧΡΟΝΙΑ ΣΤΗ ΣΑΛΟΝΙΚΗ
+    4: 889.21ΚΑΛ
+    5: '22886'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2023'
+    11: '576'
+    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+    18: '9786180149'
+    19: '234'
     3: null
     6: null
     7: null
-    9: null
     15: null
     16: null
-    18: null
-    19: null
+    17: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
@@ -559351,15 +559374,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11310
   authors: []
-  title: ΝΑΥΠΗΓΙΚΗΓ ΚΑΙ ΠΛΟΙΑ ΤΗΑ ΑΝΑΤΟΛΙΚΗΣ ΜΕΣΟΓΕΙΟΥ ΚΑΙ ΜΑΥΡ ΘΑΛΑΣ
+  title: ΝΑΥΠΗΓΙΚΗ ΚΑΙ ΠΛΟΙΑ ΤΗΑ ΑΝΑΤΟΛΙΚΗΣ ΜΕΣΟΓΕΙΟΥ ΚΑΙ ΜΑΥΡ ΘΑΛΑΣ
   subtitle: ΣΑΣ ΚΑΤΑ ΤΟΝ 18 ΚΑΙ 19 ΑΙΩΝΑ
   dewey: 938.498 ΧΣ
   entry_numbers:
   - '13989'
   editor: ΠΝΕΥΜΑΤΙΚΟΚΕΝ ΑΘΗΝΩΝ // None
   pages: 146
   topics:
@@ -559368,15 +559391,15 @@
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11310
     1: Χ. Σ.
-    2: ΝΑΥΠΗΓΙΚΗΓ ΚΑΙ ΠΛΟΙΑ ΤΗΑ ΑΝΑΤΟΛΙΚΗΣ ΜΕΣΟΓΕΙΟΥ ΚΑΙ ΜΑΥΡ ΘΑΛΑΣ
+    2: ΝΑΥΠΗΓΙΚΗ ΚΑΙ ΠΛΟΙΑ ΤΗΑ ΑΝΑΤΟΛΙΚΗΣ ΜΕΣΟΓΕΙΟΥ ΚΑΙ ΜΑΥΡ ΘΑΛΑΣ
     3: ΣΑΣ ΚΑΤΑ ΤΟΝ 18 ΚΑΙ 19 ΑΙΩΝΑ
     4: 938.498Χ.Σ
     5: '13989'
     8: ΠΝΕΥΜΑΤΙΚΟΚΕΝ ΑΘΗΝΩΝ
     11: 146Σ
     12: ΝΑΥΠΗΓΙΚΗ ΤΕΧΝΗ
     13: ΝΑΥΠΗΓΙΚΗ ΤΕΧΝΗ
@@ -559826,15 +559849,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11320
   authors:
-  - ΑΧΙΛΛΕΑΣ ΙΩΑΝΝΟΥ ΛΑΜΤΖΙΔΗΣ
+  - ΛΑΜΤΖΙΔΗΣ,ΑΧΙΛΛΕΑΣ
   title: ΣΥΜΒΟΛΗ ΣΤΗ ΔΗΜΟΓΡΑΦΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΕΝΟΡΙΑΣ ΥΠΑΠΑΝΤΗΣ ΤΗΣ
   subtitle: ΤΡΑΠΕΖΟΥΝΤΑΣ (1920-1923)
   dewey: 938.498 ΛΑΜ
   entry_numbers:
   - '13990'
   editor: None // ΑΘΗΝΑ
   edition_year: 1997
@@ -559845,15 +559868,15 @@
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11320
-    1: ΑΧΙΛΛΕΑΣ ΙΩΑΝΝΟΥ ΛΑΜΤΖΙΔΗΣ
+    1: ΛΑΜΤΖΙΔΗΣ,ΑΧΙΛΛΕΑΣ
     2: ΣΥΜΒΟΛΗ ΣΤΗ ΔΗΜΟΓΡΑΦΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΕΝΟΡΙΑΣ ΥΠΑΠΑΝΤΗΣ ΤΗΣ
     3: ' ΤΡΑΠΕΖΟΥΝΤΑΣ (1920-1923)'
     4: 938.498ΛΑΜ
     5: '13990'
     9: ΑΘΗΝΑ
     10: '1997'
     11: 251Σ
@@ -560318,15 +560341,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11330
   authors:
-  - ΜΑΡΙΑ ΝΥΣΤΑΖΟΠΟΥΛΟΠΥ-ΠΕΛΕΚΙΔΟΥ
+  - ΠΕΛΕΚΙΔΟΥ-ΝΥΣΤΑΖΟΠΟΥΛΟΥ,ΜΑΡΙΑ
   title: ΤΟ ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ
   subtitle: ΙΣΤΟΡΙΚΗ ΘΕΩΡΗΣΗ ΤΟΥ ΠΡΟΒΛΗΜΑΤΟΣ
   dewey: 938.498 ΠΕΛ
   entry_numbers:
   - '14113'
   editor: ΚΕΝΤΡΟ ΣΠΟΥΔΩΝ ΝΑ.ΕΥ // ΑΘΗΝΑ
   edition_year: 1998
@@ -560335,15 +560358,15 @@
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11330
-    1: ΜΑΡΙΑ ΝΥΣΤΑΖΟΠΟΥΛΟΠΥ-ΠΕΛΕΚΙΔΟΥ
+    1: ΠΕΛΕΚΙΔΟΥ-ΝΥΣΤΑΖΟΠΟΥΛΟΥ,ΜΑΡΙΑ
     2: ΤΟ ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ
     3: ΙΣΤΟΡΙΚΗ ΘΕΩΡΗΣΗ ΤΟΥ ΠΡΟΒΛΗΜΑΤΟΣ
     4: 938.498ΠΕΛ
     5: '14113'
     8: ΚΕΝΤΡΟ ΣΠΟΥΔΩΝ ΝΑ.ΕΥ
     9: ΑΘΗΝΑ
     10: '1998'
@@ -560421,15 +560444,15 @@
 - dbase_number: 11332
   authors:
   - ΓΕΩΡΓΙΟΣ ΧΑΡ. ΠΑΠΑΔΟΠΟΥΛΟΣ
   title: Η ΕΘΝΙΚΗ ΕΛΛΗΝΙΚΗ ΜΕΙΟΝΟΤΗΣ ΕΙΣ ΤΗΝ ΑΛΒΑΝΙΑΝ ΚΑΙ ΤΟ ΣΧΟΛΙΚΟΝ
   subtitle: ΑΥΤΗΣ ΖΗΤΗΜΑ
   dewey: 938.498 ΠΑΠ
   entry_numbers:
-  - '14022'
+  - '14092'
   editor: ΙΔΡΥΜΑ ΒΟΡ/ΚΩΝ ΕΡΕΥΝ // ΙΩΑΝΝΙΝΑ
   edition_year: 1981
   pages: 296
   topics:
   - ΙΣΤΟΡΙΑ ΑΛΒΑΝΙΑ
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
@@ -560438,15 +560461,15 @@
   offprint: false
   original_entry:
     0: 11332
     1: ΓΕΩΡΓΙΟΣ ΧΑΡ. ΠΑΠΑΔΟΠΟΥΛΟΣ
     2: Η ΕΘΝΙΚΗ ΕΛΛΗΝΙΚΗ ΜΕΙΟΝΟΤΗΣ ΕΙΣ ΤΗΝ ΑΛΒΑΝΙΑΝ ΚΑΙ ΤΟ ΣΧΟΛΙΚΟΝ
     3: ' ΑΥΤΗΣ ΖΗΤΗΜΑ'
     4: 938.498ΠΑΠ
-    5: '14022'
+    5: '14092'
     8: ΙΔΡΥΜΑ ΒΟΡ/ΚΩΝ ΕΡΕΥΝ
     9: ΙΩΑΝΝΙΝΑ
     10: '1981'
     11: 296Σ
     12: ΙΣΤΟΡΙΑ ΑΛΒΑΝΙΑ
     13: ΙΣΤΟΡΙΑ ΑΛΒΑΝΙΑ
     14: ΙΣΤΟΡΙΑ ΑΛΒΑΝΙΑ
@@ -566028,15 +566051,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11446
   authors:
-  - ΓΕΡΑΣΙΜΟΣ Μ. ΒΛΑΧΟΣ
+  - ΒΛΑΧΟΣ,ΓΕΡΑΣΙΜΟΣ
   title: ΤΟ ΑΡΧΕΙΟΝ ΤΗΣ ΙΟΝΙΚΗΣ ΤΡΑΠΕΖΗΣ
   subtitle: ΕΓΓΡΑΦΑ ΤΗΣ ΠΕΡΙΟΔΟΥ 1833-1920
   dewey: 938.498 ΒΛΑ
   entry_numbers:
   - '13530'
   editor: ΕΤΑΙΡ ΜΕΛ ΕΛΛΗΝ ΙΣΤ // ΑΘΗΝΑ
   edition_year: 2000
@@ -566046,15 +566069,15 @@
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11446
-    1: ΓΕΡΑΣΙΜΟΣ Μ. ΒΛΑΧΟΣ
+    1: ΒΛΑΧΟΣ,ΓΕΡΑΣΙΜΟΣ
     2: ΤΟ ΑΡΧΕΙΟΝ ΤΗΣ ΙΟΝΙΚΗΣ ΤΡΑΠΕΖΗΣ
     3: ΕΓΓΡΑΦΑ ΤΗΣ ΠΕΡΙΟΔΟΥ 1833-1920
     4: 938.498ΒΛΑ
     5: '13530'
     8: ΕΤΑΙΡ ΜΕΛ ΕΛΛΗΝ ΙΣΤ
     9: ΑΘΗΝΑ
     10: '2000'
@@ -566078,15 +566101,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11447
   authors:
-  - ΣΠΥΡΟΣ ΔΗΜ. ΛΟΥΚΑΤΟΣ
+  - ΛΟΥΚΑΤΟΣ,ΣΠΥΡΟΣ
   title: ΠΟΛΙΤΕΙΟΓΡΑΦΙΑ ΤΗΣ ΝΟΜΑΡΧΙΑΚΗΣ ΠΕΡΙΕΦΕΡΕΙΑΣ ΤΗΣ ΘΕΣΣΑΛΟΝΙΚΗΣ
   dewey: 304.60 ΛΟΥ
   entry_numbers:
   - '14104'
   editor: ΚΕΝΤ ΣΠ ΝΑ ΕΥΡΩΠΗΣ // ΑΘΗΝΑ
   edition_year: 1987
   pages: 139
@@ -566095,15 +566118,15 @@
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11447
-    1: ΣΠΥΡΟΣ ΔΗΜ. ΛΟΥΚΑΤΟΣ
+    1: ΛΟΥΚΑΤΟΣ,ΣΠΥΡΟΣ
     2: ΠΟΛΙΤΕΙΟΓΡΑΦΙΑ ΤΗΣ ΝΟΜΑΡΧΙΑΚΗΣ ΠΕΡΙΕΦΕΡΕΙΑΣ ΤΗΣ ΘΕΣΣΑΛΟΝΙΚΗΣ
     4: 304.60ΛΟΥ
     5: '14104'
     8: ΚΕΝΤ ΣΠ ΝΑ ΕΥΡΩΠΗΣ
     9: ΑΘΗΝΑ
     10: '1987'
     11: 139Σ
@@ -567192,46 +567215,51 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11470
   authors:
-  - ΣΑΡΑΝΤΟΣ Ι. ΚΑΡΓΑΛΟΣ
+  - ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
   title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   subtitle: Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
   dewey: 938.498 ΚΑΡ
   entry_numbers:
   - '14148'
+  - '17352'
+  editor: REAL NEWS // ΑΘΗΝΑ
+  edition_year: 2014
+  pages: 224
   topics:
-  - ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
+  - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+  - ΜΕΓΑ ΑΛΕΞΑΝΔΡΟΣ
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
-  volume: ΤΟΜΟΙ 3
+  volume: ΤΟΜΟΙ 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11470
-    1: ΣΑΡΑΝΤΟΣ Ι. ΚΑΡΓΑΛΟΣ
+    1: ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
     2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     3: Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
     4: 938.498ΚΑΡ
-    5: '14148'
-    12: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
-    13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
-    14: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
+    5: 14148-17352
+    8: REAL NEWS
+    9: ΑΘΗΝΑ
+    10: '2014'
+    11: '224'
+    12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+    13: ΜΕΓΑ ΑΛΕΞΑΝΔΡΟΣ
+    14: ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
-    30: ΤΟΜΟΙ 3
+    30: ΤΟΜΟΙ 2
     6: null
     7: null
-    8: null
-    9: null
-    10: null
-    11: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -567289,46 +567317,47 @@
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11472
-  authors:
-  - ΠΕΡΙΟΔΙΚΟ
+  authors: []
   title: ΕΛΛΗΝΩΝ ΙΣΤΟΡΙΚΑ
-  dewey: 938.498 ΠΕΡ
+  dewey: 938.498 ΧΣ
   entry_numbers:
   - '14149'
+  editor: None // ΑΘΗΝΑ
+  pages: 155
   topics:
   - ΠΕΡΙΟΔΙΚΟ
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   volume: 12 ΤΕΥΧΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11472
-    1: ΠΕΡΙΟΔΙΚΟ
+    1: Χ.Σ
     2: ΕΛΛΗΝΩΝ ΙΣΤΟΡΙΚΑ
-    4: 938.498ΠΕΡ
+    4: 938.498Χ.Σ
     5: '14149'
+    9: ΑΘΗΝΑ
+    11: '155'
     12: ΠΕΡΙΟΔΙΚΟ
     13: ΠΕΡΙΟΔΙΚΟ
     14: ΠΕΡΙΟΔΙΚΟ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
     30: 12 ΤΕΥΧΗ
     3: null
     6: null
     7: null
     8: null
-    9: null
     10: null
-    11: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -567436,30 +567465,30 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11475
   authors:
-  - ΒΑΣΙΛΙΚΗ ΛΑΖΟΥ
+  - ΛΑΖΟΥ,ΒΑΣΙΛΙΚΗ
   title: ΠΟΛΗ 1955 Η ΤΕΛΕΥΤΑΙΑ ΑΛΩΣΗ
   dewey: 938.498 ΛΑΖ
   entry_numbers: []
   editor: ΕΛΕΥΘΕΡΟΤΥΠΙΑ // ΑΘΗΝΑ
   edition_year: 2010
   pages: 192
   topics: []
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11475
-    1: ΒΑΣΙΛΙΚΗ ΛΑΖΟΥ
+    1: ΛΑΖΟΥ,ΒΑΣΙΛΙΚΗ
     2: ΠΟΛΗ 1955 Η ΤΕΛΕΥΤΑΙΑ ΑΛΩΣΗ
     4: 938.498ΛΑΖ
     8: ΕΛΕΥΘΕΡΟΤΥΠΙΑ
     9: ΑΘΗΝΑ
     10: '2010'
     11: 192Σ
     12: ΙΣΤΟΡΙΑ
@@ -567529,30 +567558,30 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11477
   authors:
-  - ΓΙΩΡΓΟΣ ΞΕΠΑΠΑΔΑΚΟΣ
+  - ΞΕΠΑΠΑΔΑΚΟΣ,ΓΙΩΡΓΟΣ
   title: ΘΡΑΚΕΣ ΤΣΑΚΩΝΕΣ ΜΑΚΕΔΟΝΕΣ ΑΡΒΑΝΙΤΕΣ ΜΙΚΡΑΣΙΑΤΕΣ
   dewey: 910 ΞΕΠ
   entry_numbers:
   - '14153'
   topics:
   - ΡΙΖΕΣ ΕΛΛΗΝΩΝ
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   volume: 5 ΤΟΜΟΙ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11477
-    1: ΓΙΩΡΓΟΣ ΞΕΠΑΠΑΔΑΚΟΣ
+    1: ΞΕΠΑΠΑΔΑΚΟΣ,ΓΙΩΡΓΟΣ
     2: ΘΡΑΚΕΣ ΤΣΑΚΩΝΕΣ ΜΑΚΕΔΟΝΕΣ ΑΡΒΑΝΙΤΕΣ ΜΙΚΡΑΣΙΑΤΕΣ
     4: 910 ΞΕΠ
     5: '14153'
     12: ΡΙΖΕΣ ΕΛΛΗΝΩΝ
     13: ΡΙΖΕΣ ΕΛΛΗΝΩΝ
     14: ΡΙΖΕΣ ΕΛΛΗΝΩΝ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
@@ -567576,61 +567605,64 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11478
   authors:
-  - ΒΑΣΙΛΙΚΗ ΛΑΖΟΥ
-  title: ΚΙΝΗΜΑΤΑ ΠΡΑΞΙΚΟ[ΠΗΜΑΤΑ ΔΙΚΤΑΤΟΡΙΕΣ
+  - ΛΑΖΟΥ,ΒΑΣΙΛΙΚΗ
+  title: ΚΙΝΗΜΑΤΑ ΠΡΑΞΙΚΟΠΗΜΑΤΑ ΔΙΚΤΑΤΟΡΙΕΣ
   dewey: 938.498 ΛΑΖ
   entry_numbers:
   - '14152'
+  editor: ΕΛΕΥΘΕΡΟΤΥΠΙΑ // ΑΘΗΝΑ
+  edition_year: 2011
   pages: 193
   topics: []
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
+  ean: '9789609487733'
   original_entry:
     0: 11478
-    1: ΒΑΣΙΛΙΚΗ ΛΑΖΟΥ
-    2: ΚΙΝΗΜΑΤΑ ΠΡΑΞΙΚΟ[ΠΗΜΑΤΑ ΔΙΚΤΑΤΟΡΙΕΣ
+    1: ΛΑΖΟΥ,ΒΑΣΙΛΙΚΗ
+    2: ΚΙΝΗΜΑΤΑ ΠΡΑΞΙΚΟΠΗΜΑΤΑ ΔΙΚΤΑΤΟΡΙΕΣ
     4: 938.498ΛΑΖ
     5: '14152'
+    8: ΕΛΕΥΘΕΡΟΤΥΠΙΑ
+    9: ΑΘΗΝΑ
+    10: '2011'
     11: 193Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
+    18: '9789609487'
+    19: '733'
     3: null
     6: null
     7: null
-    8: null
-    9: null
-    10: null
     15: null
     16: null
-    18: null
-    19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11479
   authors:
-  - ΓΕΩΡΓΙΟΣ ΒΙΖΥΗΝΟΣ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
   title: ΑΤΘΙΔΕΣ ΑΥΡΑΙ
   dewey: 889.21 ΒΙΖ
   entry_numbers:
   - '14163'
   editor: ΛΑΜΠΡΑΚΗΣ // None
   edition_year: 2014
   pages: 330
@@ -567640,15 +567672,15 @@
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-503-471-9
   original_entry:
     0: 11479
-    1: ΓΕΩΡΓΙΟΣ ΒΙΖΥΗΝΟΣ
+    1: ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
     2: ΑΤΘΙΔΕΣ ΑΥΡΑΙ
     4: 889.21ΒΙΖ
     5: '14163'
     8: ΛΑΜΠΡΑΚΗΣ
     10: '2014'
     11: 330Σ
     12: ΠΟΙΗΣΗ
@@ -567672,15 +567704,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11480
   authors:
-  - ΚΩΣΤΗΣ ΠΑΛΑΜΑΣ
+  - ΠΑΛΑΜΑΣ,ΚΩΣΤΗΣ
   title: Ο ΔΩΔΕΚΑΛΟΓΟΣ ΤΟΥ ΓΥΦΤΟΥ
   dewey: 889.21 ΠΑΛ
   entry_numbers:
   - '14162'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 2014
   pages: 204
@@ -567690,15 +567722,15 @@
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-503-464-1
   original_entry:
     0: 11480
-    1: ΚΩΣΤΗΣ ΠΑΛΑΜΑΣ
+    1: ΠΑΛΑΜΑΣ,ΚΩΣΤΗΣ
     2: Ο ΔΩΔΕΚΑΛΟΓΟΣ ΤΟΥ ΓΥΦΤΟΥ
     4: 889.21ΠΑΛ
     5: '14162'
     8: ΤΟ ΒΗΜΑ
     9: ΑΘΗΝΑ
     10: '2014'
     11: 204Σ
@@ -567771,15 +567803,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11482
   authors:
-  - ΠΑΝΟΣ ΜΠΑΙΛΗΣ
+  - ΜΠΑΙΛΗΣ,ΠΑΝΟΣ
   title: ΤΟΥ ΛΟΓΟΥ ΜΟΥ Ο ΜΟΝΑΧΟΣ ΠΑΙΣΙΟΣ
   dewey: 938.993 ΜΠΑ
   entry_numbers:
   - '14159'
   editor: ΧΡΗΣΤΟΣ ΚΤΕΝΑΣ // None
   pages: 111
   topics:
@@ -567787,15 +567819,15 @@
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11482
-    1: ΠΑΝΟΣ ΜΠΑΙΛΗΣ
+    1: ΜΠΑΙΛΗΣ,ΠΑΝΟΣ
     2: ΤΟΥ ΛΟΓΟΥ ΜΟΥ Ο ΜΟΝΑΧΟΣ ΠΑΙΣΙΟΣ
     4: 938.993ΜΠΑ
     5: '14159'
     8: ΧΡΗΣΤΟΣ ΚΤΕΝΑΣ
     11: 111Σ
     12: ΘΡΗΣΚΕΙΑ
     13: ΘΡΗΣΚΕΙΑ
@@ -567819,15 +567851,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11483
   authors:
-  - ΘΕΟΦ. ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ
   title: ΠΟΛΙΤΙΚΗ ΑΓΩΓΗ
   dewey: 320.071 ΠΑΠ
   entry_numbers:
   - '14169'
   editor: KABANAS // ΑΘΗΝΑ
   edition_year: 1970
   topics:
@@ -567835,15 +567867,15 @@
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11483
-    1: ΘΕΟΦ. ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ
+    1: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ
     2: ΠΟΛΙΤΙΚΗ ΑΓΩΓΗ
     4: 320.071ΠΑΠ
     5: '14169'
     8: KABANAS
     9: ΑΘΗΝΑΙ
     10: '1970'
     12: ΠΟΛΙΤΙΚΗ ΑΓΩΓΗ
@@ -568064,15 +568096,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11488
   authors:
-  - ΛΕΝΑ ΛΟΥΚΙΔΟΥ
+  - ΔΟΥΚΙΔΟΥ,ΛΕΝΑ
   title: ΠΩΣ ΦΤΑΣΑΜΕ ΣΤΗ ΔΙΚΤΑΤΟΡΙΑ ΤΟΥ 67
   dewey: 938.498 ΔΟΥ
   entry_numbers:
   - '14168'
   editor: ΛΑΜΠΡΑΚΗ // None
   edition_year: 2012
   pages: 251
@@ -568081,15 +568113,15 @@
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-503-097-1
   original_entry:
     0: 11488
-    1: ΛΕΝΑ ΛΟΥΚΙΔΟΥ
+    1: ΔΟΥΚΙΔΟΥ,ΛΕΝΑ
     2: ΠΩΣ ΦΤΑΣΑΜΕ ΣΤΗ ΔΙΚΤΑΤΟΡΙΑ ΤΟΥ 67
     4: 938.498ΔΟΥ
     5: '14168'
     8: ΛΑΜΠΡΑΚΗ
     10: '2012'
     11: 251Σ
     12: ΙΣΤΟΡΙΑ
@@ -568405,15 +568437,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11495
   authors:
-  - ΣΤΑΥΡΟΣ ΨΥΧΑΡΗΣ
+  - ΨΥΧΑΡΗΣ,ΣΤΑΥΡΟΣ
   title: ΟΙ ΕΒΔΟΜΗΝΤΑ ΚΡΙΣΙΜΕΣ ΗΜΕΡΕΣ
   dewey: 938.498 ΨΥΧ
   entry_numbers:
   - '14189'
   editor: ΛΑΜΠΡΑΚΗ // None
   edition_year: 2013
   pages: 303
@@ -568422,15 +568454,15 @@
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-503-393-4
   original_entry:
     0: 11495
-    1: ΣΤΑΥΡΟΣ ΨΥΧΑΡΗΣ
+    1: ΨΥΧΑΡΗΣ,ΣΤΑΥΡΟΣ
     2: ΟΙ ΕΒΔΟΜΗΝΤΑ ΚΡΙΣΙΜΕΣ ΗΜΕΡΕΣ
     4: 938.498ΨΥΧ
     5: '14189'
     8: ΛΑΜΠΡΑΚΗ
     10: '2013'
     11: 303Σ
     12: ΙΣΤΟΡΙΑ
@@ -568792,48 +568824,48 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11503
   authors:
-  - ΣΤΕΦΑΝΟΣ, ΠΑΠΑΔΟΠΟΥΛΟΣ
-  title: ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
-  dewey: 938.498 ΠΑΠ
+  - ΗΛΙΟΠΟΥΛΟΣ,ΓΙΩΡΓΟΣ
+  title: Ο ΑΓΝΩΣΤΟΣ ΑΛΕΞΑΝΔΡΟΣ
+  dewey: 938.070 ΗΛΙ
   entry_numbers:
-  - '14176'
-  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
-  edition_year: 1969
-  pages: 62
-  topics: []
-  donors:
-  - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
+  - '17213'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2003
+  pages: 250
+  topics:
+  - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
+  isbn: '9607882229'
   original_entry:
     0: 11503
-    1: ΣΤΕΦΑΝΟΣ, ΠΑΠΑΔΟΠΟΥΛΟΣ
-    2: ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
-    4: 938.498ΠΑΠ
-    5: '14176'
-    9: ΘΕΣ/ΝΙΚΗ
-    10: '1969'
-    11: 62Σ
-    12: ΙΣΤΟΡΙΑ
-    13: ΙΣΤΟΡΙΑ
-    14: ΙΣΤΟΡΙΑ
-    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
+    1: ΗΛΙΟΠΟΥΛΟΣ,ΓΙΩΡΓΟΣ
+    2: Ο ΑΓΝΩΣΤΟΣ ΑΛΕΞΑΝΔΡΟΣ
+    4: 938.070ΗΛΙ
+    5: '17213'
+    9: ΑΘΗΝΑ
+    10: '2003'
+    11: '250'
+    12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+    13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+    14: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+    18: '9607882229'
     3: null
     6: null
     7: null
     8: null
     15: null
     16: null
-    18: null
+    17: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
@@ -568889,36 +568921,37 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11505
   authors:
-  - ΦΩΤΕΙΝΗ ΤΖΙΚΟΥ
+  - ΤΖΙΚΟΥ,ΦΩΤΕΙΝΗ
   title: Ο ΑΓΝΩΣΤΟΣ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  dewey: 938.498 ΤΖΙ
+  dewey: 938.174 ΤΖΙ
   entry_numbers:
   - '14172'
+  - '17408'
   edition: Β
   editor: ΑΡΧΕΤΥΠΟ // None
   edition_year: 2005
   pages: 254
   topics: []
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-421-030-0
   original_entry:
     0: 11505
-    1: ΦΩΤΕΙΝΗ ΤΖΙΚΟΥ
+    1: ΤΖΙΚΟΥ,ΦΩΤΕΙΝΗ
     2: Ο ΑΓΝΩΣΤΟΣ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    4: 938.498ΤΖΙ
-    5: '14172'
+    4: 938.174ΤΖΙ
+    5: 14172-17408
     7: Β
     8: ΑΡΧΕΤΥΠΟ
     10: '2005'
     11: 254Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
@@ -569929,15 +569962,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11526
   authors:
-  - ΚΑΡΛ ΜΕΝΤΕΛΣΟΝ -ΜΠΑΡΤΟΛΝΤΙ
+  - ΜΕΝΤΕΛΣΟΝ-ΜΠΑΡΤΟΛΝΤΙ,ΚΑΡΛ
   title: ΕΠΙΤΟΜΗ ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
   dewey: 938.498 ΜΕΝ
   entry_numbers:
   - '15029'
   editor: ΤΕΓΟΠΟΥΛΟΣ // None
   edition_year: 2011
   pages: 235
@@ -569947,15 +569980,15 @@
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-9487-68-9
   original_entry:
     0: 11526
-    1: ΚΑΡΛ ΜΕΝΤΕΛΣΟΝ -ΜΠΑΡΤΟΛΝΤΙ
+    1: ΜΕΝΤΕΛΣΟΝ-ΜΠΑΡΤΟΛΝΤΙ,ΚΑΡΛ
     2: ΕΠΙΤΟΜΗ ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
     4: 938.498ΜΕΝ
     5: '15029'
     8: ΤΕΓΟΠΟΥΛΟΣ
     10: '2011'
     11: 235Σ
     12: ΕΠΙΤΟΜΗ ΙΣΤΟΡΙΑ
@@ -570660,15 +570693,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11541
   authors:
-  - ΘΑΒΩΡΗΣ,Α.
+  - ΘΑΒΩΡΗΣ,Α
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΓΛΩΣΣΑΣ
   dewey: 938.498 ΘΑΒ
   entry_numbers:
   - '15001'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1971
   pages: 153
@@ -570676,25 +570709,25 @@
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11541
-    1: Α. ΘΑΒΩΡΗΣ
+    1: ΘΑΒΩΡΗΣ,Α
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΓΛΩΣΣΑΣ
     4: 938.498ΘΑΒ
     5: '15001'
     9: ΙΩΑΝΝΙΝΑ
     10: '1971'
     11: 153Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
-    17: ΔΩΡΕΑΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
     3: null
     6: null
     7: null
     8: null
     15: null
     16: null
     18: null
@@ -570708,15 +570741,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11542
   authors:
-  - ΓΕΩΡΓΙΟΥ Ι. ΘΕΟΧΑΡΙΔΟΥ
+  - ΘΕΟΧΑΡΙΔΟΥ,ΓΕΩΡΓΙΟΥ
   title: ΙΣΤΟΡΙΑ ΜΕΣΩΝ ΧΡΟΝΩΝ
   dewey: 938.498 ΘΕΟ
   entry_numbers:
   - '14197'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1970
   topics: []
@@ -570724,15 +570757,15 @@
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   volume: ΠΕΝΤΕ ΤΟΜΟΙ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11542
-    1: ΓΕΩΡΓΙΟΥ Ι. ΘΕΟΧΑΡΙΔΟΥ
+    1: ΘΕΟΧΑΡΙΔΟΥ,ΓΕΩΡΓΙΟΥ
     2: ΙΣΤΟΡΙΑ ΜΕΣΩΝ ΧΡΟΝΩΝ
     4: 938.498ΘΕΟ
     5: '14197'
     9: ΘΕΣ/ΝΙΚΗ
     10: '1970'
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -571359,15 +571392,15 @@
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 144
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
-  volume: 5 ΤΟΜΟΙ
+  volume: 7 ΤΟΜΟΙ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-475-151-8
   original_entry:
     0: 11555
     1: Χ.Σ
@@ -571381,15 +571414,15 @@
     11: 144Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
     13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
     14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
     18: 978-960-47
     19: 5-151-8
-    30: 5 ΤΟΜΟΙ
+    30: 7 ΤΟΜΟΙ
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -572624,15 +572657,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11581
   authors:
-  - ΜΠΑΙΡΟΝ
+  - ΠΡΟΚΟΣ,ΦΡΕΝΤΕΡΙΚ
   title: ΤΑ ΧΕΙΡΟΓΡΑΦΑ ΤΟΥ ΜΕΣΟΛΟΓΓΙΟΥ
   dewey: 938.483 ΜΠΑ
   entry_numbers:
   - '15049'
   translators:
   - ΣΚΟΝΔΡΑΣ,ΠΑΝΑΓΙΩΤΗΣ
   editor: ΤΕΓΟΠΟΥΛΟΣ // None
@@ -572644,15 +572677,15 @@
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-9487-66-5
   original_entry:
     0: 11581
-    1: ΜΠΑΙΡΟΝ
+    1: ΠΡΟΚΟΣ,ΦΡΕΝΤΕΡΙΚ
     2: ΤΑ ΧΕΙΡΟΓΡΑΦΑ ΤΟΥ ΜΕΣΟΛΟΓΓΙΟΥ
     4: 938.483ΜΠΑ
     5: '15049'
     6: ΠΑΝΑΓΙΩΤΗΣ ΣΚΟΝΔΡΑΣ
     8: ΤΕΓΟΠΟΥΛΟΣ
     10: '2011'
     11: 301Σ
@@ -573057,15 +573090,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11590
   authors:
-  - Ν. ΤΣΙΦΟΡΟΥ
+  - ΤΣΙΦΟΡΟΥ,Ν.
   title: ΙΑΣΟΝΑΣ
   dewey: 808.899 ΤΣΙ
   entry_numbers:
   - '15072'
   edition_year: 2013
   pages: 49
   topics:
@@ -573074,15 +573107,15 @@
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-503-411-5
   original_entry:
     0: 11590
-    1: Ν. ΤΣΙΦΟΡΟΥ
+    1: ΤΣΙΦΟΡΟΥ,Ν.
     2: ΙΑΣΟΝΑΣ
     4: 808.899ΤΣΙ
     5: '15072'
     10: '2013'
     11: 49Σ
     12: ΜΥΘΟΛΟΓΙΑ
     13: ΜΥΘΟΛΟΓΙΑ
@@ -581158,30 +581191,30 @@
     29: null
     30: null
 - dbase_number: 11754
   authors: []
   title: ΟΙ 100 ΜΕΓΑΛΥΤΕΡΕΣ ΜΑΧΕΣ ΤΗΣ ΙΣΤΟΡΙΑ
   dewey: 938.498 ΧΣ
   entry_numbers:
-  - '15234'
+  - '15237'
   editor: ΕΘΝΟΣ // ΑΘΗΝΑ
   edition_year: 2008
   pages: 79
   topics: []
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11754
     1: Χ.Σ.
     2: ΟΙ 100 ΜΕΓΑΛΥΤΕΡΕΣ ΜΑΧΕΣ ΤΗΣ ΙΣΤΟΡΙΑ
     4: 938.498Χ.Σ
-    5: '15234'
+    5: '15237'
     8: ΕΘΝΟΣ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 79Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
@@ -588620,15 +588653,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11905
   authors: []
   title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  dewey: 938.498 ΧΣ
+  dewey: 938.174 ΧΣ
   entry_numbers:
   - '15350'
   editor: ΤΕΓΟΠΟΥΛΟΣ // None
   pages: 194
   topics:
   - ΙΣΤΟΡΙΑ
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -588637,15 +588670,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11905
     1: Χ.Σ.
     2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    4: 938.498Χ.Σ
+    4: 938.174Χ.Σ
     5: '15350'
     8: ΤΕΓΟΠΟΥΛΟΣ
     11: 194Σ
     12: ΙΣΤΙΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     14: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
@@ -603603,37 +603636,36 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12210
-  authors:
-  - THOMPSON HOMER
+  authors: []
   title: Η ΑΓΟΡΑ ΤΗΣ ΑΡΧΑΙΑΣ ΑΘΗΝΑ
   subtitle: ΣΥΝΤΟΜΟΣ ΟΔΗΓΟΣ
-  dewey: 938.498 THO
+  dewey: 938.498 ΧΣ
   entry_numbers:
   - '15612'
   editor: ΑΜΕΡ ΣΧ ΚΛΑΣΣΙΚ ΣΠ // ΑΘΗΝΑ
   edition_year: 1985
   pages: 32
   topics:
   - ΙΣΤΟΡΙΑ ΑΡΧΑΙΑΣ ΑΘΗΝΑΣ
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12210
-    1: THOMPSON HOMER
+    1: Χ.Σ
     2: Η ΑΓΟΡΑ ΤΗΣ ΑΡΧΑΙΑΣ ΑΘΗΝΑ
     3: ΣΥΝΤΟΜΟΣ ΟΔΗΓΟΣ
-    4: 938.498THO
+    4: 938.498Χ.Σ
     5: '15612'
     8: ΑΜΕΡ ΣΧ ΚΛΑΣΣΙΚ ΣΠ
     9: ΑΘΗΝΑ
     10: '1985'
     11: 32Σ
     12: ΙΣΤΟΡΙΑ ΑΡΧΑΙΑ ΑΘΗΝΑ
     13: ΙΣΤΟΡΙΑ ΑΡΧΑΙΑ ΑΘΗΝΑ
@@ -607155,15 +607187,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 12282
   authors:
   - ΓΟΡΓΩ-ΑΛΕΞΙΟΥ,ΓΕΩΡΓΙΑ
   title: ΤΟ ΟΙΚΟΥΜΕΝΙΚΟ ΟΡΑΜΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
-  dewey: 938.498 ΓΟΡ
+  dewey: 938.07 ΓΟΡ
   entry_numbers:
   - '15710'
   editor: ΕΡΩΔΙΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2010
   pages: 48
   topics:
   - ΑΛΕΞΑΝΔΡΟΣ
@@ -607173,15 +607205,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-454-106-5
   original_entry:
     0: 12282
     1: ΓΟΡΓΩ-ΑΛΕΞΙΟΥ,ΓΕΩΡΓΙΑ
     2: ΤΟ ΟΙΚΟΥΜΕΝΙΚΟ ΟΡΑΜΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
-    4: 938.498ΓΟΡ
+    4: 938.07ΓΟΡ
     5: '15710'
     8: ΕΡΩΔΙΟΣ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2010'
     11: 48Σ
     12: ΙΣΤΟΡΙΑ-ΑΛΕΞΑΝΔΡΟΣ
     13: ΙΣΤΟΡΙΑ-ΑΛΕΞΑΝΔΡΟΣ
@@ -607301,15 +607333,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12285
   authors: []
   title: ΤΟ ΣΥΜΒΟΥΛΙΟ ΤΗΣ ΕΠΙΚΡΑΤΕΙΑΣ ΣΤΗΝ ΕΛΛΑΔΑ
-  dewey: 938.498 ΙΣΤ
+  dewey: 938.498 ΧΣ
   entry_numbers:
   - '15518'
   editor: ΑΡΜΕΝΟΠΟΥΛΟ // ΑΘΗΝΑ
   edition_year: 1979
   pages: 167
   topics: []
   donors:
@@ -607317,15 +607349,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12285
     1: Χ.Σ.
     2: ΤΟ ΣΥΜΒΟΥΛΙΟ ΤΗΣ ΕΠΙΚΡΑΤΕΙΑΣ ΣΤΗΝ ΕΛΛΑΔΑ
-    4: 938.498ΙΣΤ
+    4: 938.498Χ.Σ
     5: '15518'
     8: ΑΡΜΕΝΟΠΟΥΛΟ
     9: ΑΘΗΝΑ
     10: '1979'
     11: 167Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -607397,15 +607429,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 12287
   authors:
-  - ΓΚΑΡΟΥΦ,Β-ΤΣΙΜΠΟΥΚΙΔΗΣ,ΔΗΜ
+  - ΓΚΑΦΟΥΡΟΦ,Β-ΤΣΙΜΠΟΥΚΙΔΗΣ,ΔΗΜ
   title: ΑΛΕΞΑΝΔΡΟΣ Ο ΜΑΚΕΔΩΝ ΚΑΙ Η ΑΝΑΤΟΛΗ
   dewey: 938.498 ΓΚΑ
   entry_numbers:
   - '15714'
   editor: ΠΑΠΑΔΗΜΑ // ΑΘΗΝΑ
   edition_year: 1982
   pages: 735
@@ -607414,15 +607446,15 @@
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12287
-    1: ΓΚΑΡΟΥΦ,Β-ΤΣΙΜΠΟΥΚΙΔΗΣ,ΔΗΜ
+    1: ΓΚΑΦΟΥΡΟΦ,Β-ΤΣΙΜΠΟΥΚΙΔΗΣ,ΔΗΜ
     2: ΑΛΕΞΑΝΔΡΟΣ Ο ΜΑΚΕΔΩΝ ΚΑΙ Η ΑΝΑΤΟΛΗ
     4: 938.498ΓΚΑ
     5: '15714'
     8: ΠΑΠΑΔΗΜΑ
     9: ΑΘΗΝΑ
     10: '1982'
     11: 735Σ
@@ -611924,15 +611956,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 12379
   authors:
   - RICE,E.E
   title: ΑΛΕΞΑΝΔΡΟΣ Ο ΜΕΓΑΣ
-  dewey: 938.07 RIC
+  dewey: 938.174 RIC
   entry_numbers:
   - '15873'
   editor: ΝΕΦΕΛΗ // ΑΘΗΝΑ
   edition_year: 2003
   pages: 87
   topics:
   - ΒΙΟΓΡΑΦΙΑ
@@ -611941,15 +611973,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12379
     1: RICE,E.E
     2: ΑΛΕΞΑΝΔΡΟΣ Ο ΜΕΓΑΣ
-    4: 938.07RIC
+    4: 938.174RIC
     5: '15873'
     8: ΝΕΦΕΛΗ
     9: ΑΘΗΝΑ
     10: '2003'
     11: 87Σ
     12: ΒΙΟΓΡΑΦΙΑ
     13: ΒΙΟΓΡΑΦΙΑ
@@ -613941,15 +613973,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 12420
   authors:
   - ΠΑΒΑΓΙΩΤΙΔΟΥ,ΙΑΚΩΒΟΥ
   title: ΑΛΕΞΑΝΔΡΟΣ Ο ΠΑΜΜΕΓΙΣΤΟΣ
-  dewey: 938.07 ΠΑΝ
+  dewey: 938.174 ΠΑΝ
   entry_numbers:
   - '15829'
   editor: ΓΕΩΡΓΙΑΔΗΣ // ΑΘΗΝΑ
   edition_year: 1998
   pages: 261
   topics:
   - ΑΛΕΞΑΝΔΡΟΣ
@@ -613958,15 +613990,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12420
     1: ΠΑΒΑΓΙΩΤΙΔΟΥ,ΙΑΚΩΒΟΥ
     2: ΑΛΕΞΑΝΔΡΟΣ Ο ΠΑΜΜΕΓΙΣΤΟΣ
-    4: 938.07ΠΑΝ
+    4: 938.174ΠΑΝ
     5: '15829'
     8: ΓΕΩΡΓΙΑΔΗΣ
     9: ΑΘΗΝΑ
     10: '1998'
     11: 261Σ
     12: ΙΣΤΟΡΙΑ-ΑΛΕΞΑΝΔΡΟΣ
     13: ΙΣΤΟΡΙΑ-ΑΛΕΞΑΝΔΡΟΣ
@@ -617253,15 +617285,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 12487
   authors:
   - ΧΡΗΣΤΟΥ,ΠΑΝΑΓΙΩΤΗ
   title: ΕΚΘΕΣΙΣ ΠΕΠΡΑΓΜΕΝΩΝ
-  dewey: 949.565 ΧΡΗ
+  dewey: 949.498 ΧΡΗ
   entry_numbers:
   - '15852'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1968
   pages: 83
   topics:
   - ΠΕΠΡΑΓΜΕΝΑ ΑΡΙΣΤΟΤΕΛΕΙΟΥ
@@ -617270,15 +617302,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12487
     1: ΧΡΗΣΤΟΥ,ΠΑΝΑΓΙΩΤΗ
     2: ΕΚΘΕΣΙΣ ΠΕΠΡΑΓΜΕΝΩΝ
-    4: 949.565ΧΡΗ
+    4: 949.498ΧΡΗ
     5: '15852'
     9: ΘΕΣ/ΝΙΚΗ
     10: '1968'
     11: 83Σ
     12: ΠΕΠΡΑΓΜΕΝΑ ΑΡΙΣΤΟΤΕΛΕΙΟΥ
     13: ΠΕΠΡΑΓΜΕΝΑ ΑΡΙΣΤΟΤΕΛΕΙΟΥ
     14: ΠΕΠΡΑΓΜΕΝΑ ΑΡΙΣΤΟΤΕΛΕΙΟΥ
@@ -622303,42 +622335,44 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12590
   authors:
-  - ΖΩΙΔΗ,Γ.
+  - ΚΟΛΟΜΠΟΒΑ,Κ.Μ
   title: Η ΖΩΗ ΣΤΗΝ ΑΡΧΑΙΑ ΕΛΛΑΔΑ
-  dewey: 938.498 ΖΩΙ
+  dewey: 938.498 ΚΟΛ
   entry_numbers:
   - '16064'
+  translators:
+  - ΖΩΙΔΗ,Γ
   editor: ΔΡΑΚΟΠΟΥΛΟΥ // None
   pages: 223
   topics:
   - ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12590
-    1: ΖΩΙΔΗ,Γ.
+    1: ΚΟΛΟΜΠΟΒΑ,Κ.Μ
     2: Η ΖΩΗ ΣΤΗΝ ΑΡΧΑΙΑ ΕΛΛΑΔΑ
-    4: 938.498ΖΩΙ
+    4: 938.498ΚΟΛ
     5: '16064'
+    6: ΖΩΙΔΗ,Γ
     8: ΔΡΑΚΟΠΟΥΛΟΥ
     11: 223Σ
     12: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ ΕΛΛΑΔΑ
     13: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ ΕΛΛΑΔΑ
     14: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ ΕΛΛΑΔΑ
     17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
     3: null
-    6: null
     7: null
     9: null
     10: null
     15: null
     16: null
     18: null
     19: null
@@ -623089,33 +623123,33 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12606
   authors:
-  - ΣΤΥΛΙΑΝΟΣ ΧΡΑΠΗΣ
+  - ΧΡΑΠΗΣ,ΣΤΥΛΙΑΝΟΣ
   title: Ο ΔΡΟΜΟΣ ΤΟΥ ΗΓΕΤΗ
-  dewey: 938.498 ΣΤΥ
+  dewey: 938.07 ΧΡΑ
   entry_numbers:
   - '16085'
   editor: ΔΗΛΙΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   pages: 191
   topics:
   - ΙΣΤΟΡΙΑ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12606
-    1: ΣΤΥΛΙΑΝΟΣ ΧΡΑΠΗΣ
+    1: ΧΡΑΠΗΣ,ΣΤΥΛΙΑΝΟΣ
     2: Ο ΔΡΟΜΟΣ ΤΟΥ ΗΓΕΤΗ
-    4: 938.498ΣΤΥ
+    4: 938.07ΧΡΑ
     5: '16085'
     8: ΔΗΛΙΟΣ
     9: ΘΕΣ/ΚΗ
     11: 191Σ
     12: ΙΣΤΟΡΙΑ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΙΣΤΟΡΙΑ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     14: ΙΣΤΟΡΙΑ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -624461,17 +624495,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12634
   authors:
-  - ΖΩΓΡΑΦΙΚΗ,ΓΕΩΡΓΙΟΥ
+  - ΖΩΓΡΑΦΑΚΗ,ΓΕΩΡΓΙΟΥ
   title: ΘΕΣΣΑΛΟΝΙΚΗ
-  subtitle: ΠΕΡΙΠΑΤΟΣ ΑΝΑ ΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΚΑΙ ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
+  subtitle: ΠΕΡΙΠΑΤΟΣ ΑΝΑΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΚΑΙ ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
   dewey: 949.565 ΖΩΓ
   entry_numbers:
   - '16070'
   editor: ΜΑΣΤΟΡΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1967
   pages: 50
   topics:
@@ -624479,17 +624513,17 @@
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12634
-    1: ΖΩΓΡΑΦΙΚΗ,ΓΕΩΡΓΙΟΥ
+    1: ΖΩΓΡΑΦΑΚΗ,ΓΕΩΡΓΙΟΥ
     2: ΘΕΣΣΑΛΟΝΙΚΗ
-    3: ΠΕΡΙΠΑΤΟΣ ΑΝΑ ΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΚΑΙ ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
+    3: ΠΕΡΙΠΑΤΟΣ ΑΝΑΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΚΑΙ ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
     4: 949.565ΖΩΓ
     5: '16070'
     8: ΜΑΣΤΟΡΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1967'
     11: 50Σ
     12: ΙΣΤΟΡΙΑ-ΘΕΣ/ΝΙΚΗ
@@ -630450,46 +630484,47 @@
 - dbase_number: 12756
   authors:
   - FINLAY,GEORGE
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
   dewey: 938.6 ΦΙΝ
   entry_numbers:
   - '16201'
+  - '19214'
   translators:
   - ΚΟΡΔΑΤΟΣ,ΓΙΑΝΝΗΣ
   editor: Ο ΚΟΣΜΟΑ // ΑΘΗΝΑ
   pages: 423
   topics:
   - ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
-  donors:
-  - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  volume: ΤΟΜΟΙ 2
   has_cd: false
   has_dvd: false
   offprint: false
+  ean: '9789606757051'
   original_entry:
     0: 12756
     1: ΦΙΝΛΕΥ,ΓΕΩΡΓΙΟΥ
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
     4: 938.6ΦΙΝ
-    5: '16201'
+    5: 16201-19214
     6: ΓΙΑΝΝΗ ΚΟΡΔΑΤΟΥ
     8: Ο ΚΟΣΜΟΑ
     9: ΑΘΗΝΑ
     11: 423Σ
     12: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
     13: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
     14: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
-    17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
+    17: ΤΟΜΟΙ 2
+    18: '9789606757'
+    19: '051'
     3: null
     7: null
     10: null
     15: null
     16: null
-    18: null
-    19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
@@ -632361,15 +632396,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 12795
   authors:
   - ΠΕΤΡΑΚΑΚΟΥ.ΔΗΜΗΤΡΙΟΥ
   title: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  dewey: 938.07 ΠΕΤ
+  dewey: 938.174 ΠΕΤ
   entry_numbers:
   - '16269'
   editor: None // ΑΘΗΝΑ
   edition_year: 1944
   pages: 103
   topics:
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -632378,15 +632413,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12795
     1: ΠΕΤΡΑΚΑΚΟΥ.ΔΗΜΗΤΡΙΟΥ
     2: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    4: 938.07ΠΕΤ
+    4: 938.174ΠΕΤ
     5: '16269'
     9: ΑΘΗΝΑ
     10: '1944'
     11: 103Σ
     12: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     14: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -639056,14 +639091,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12932
   authors: []
   title: ΟΔΗΓΟΣ ΤΗΣ ΘΑΣΟΥ
+  dewey: 914.009 ΧΣ
   entry_numbers:
   - '16411'
   editor: ΓΑΛΛΙΚΗ ΑΡΧΣΙΟΛΟΓΙΚΗ // ΑΘΗΝΑ
   edition_year: 1974
   pages: 202
   topics:
   - ΑΡΧΑΙΟΤΗΤΑ
@@ -639072,25 +639108,25 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12932
     1: Χ.Σ.
     2: ΟΔΗΓΟΣ ΤΗΣ ΘΑΣΟΥ
+    4: 914.009Χ.Σ
     5: '16411'
     8: ΓΑΛΛΙΚΗ ΑΡΧΣΙΟΛΟΓΙΚΗ
     9: ΑΘΗΝΑ
     10: '1974'
     11: 202Σ
     12: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΟΤΗΤΕΣ
     13: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΟΤΗΤΕΣ
     14: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΟΤΗΤΕΣ
     17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
     3: null
-    4: null
     6: null
     7: null
     15: null
     16: null
     18: null
     19: null
     20: null
@@ -640769,18 +640805,18 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12967
   authors:
-  - ΚΑΛΛΙΝΑΚΗ,ΜΑΡΙΑ-ΓΟΥΔΗΣ,ΧΡΙΣΤΟΣ
+  - ΓΟΥΔΗΣ,ΧΡΙΣΤΟΣ-ΚΑΛΛΙΝΑΚΗ ΜΑΡΙΑ
   title: 1821 Η ΕΙΚΟΝΟΓΡΑΦΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
   subtitle: Α.Η ΕΠΟΧΗ ΤΗΑ ΑΥΤΟΓΝΩΣΙΑΣ Β.Η ΜΕΓΑΛΗ ΕΚΡΗΞΗ Γ. Η ΔΙΚΑΙΩΣΗ
-  dewey: 938 ΚΑΛ
+  dewey: 938 ΓΟΥ
   entry_numbers:
   - '16460'
   editor: ΚΑΔΜΟΣ // ΑΘΗΝΑ
   edition_year: 2012
   pages: 295
   topics:
   - ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
@@ -640789,18 +640825,18 @@
   volume: ΤΟΜΟΙ Α.Β.Γ.
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-6851-35-3
   original_entry:
     0: 12967
-    1: ΚΑΛΛΙΝΑΚΗ,ΜΑΡΙΑ-ΓΟΥΔΗΣ,ΧΡΙΣΤΟΣ
+    1: ΓΟΥΔΗΣ,ΧΡΙΣΤΟΣ-ΚΑΛΛΙΝΑΚΗ ΜΑΡΙΑ
     2: 1821 Η ΕΙΚΟΝΟΓΡΑΦΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
     3: Α.Η ΕΠΟΧΗ ΤΗΑ ΑΥΤΟΓΝΩΣΙΑΣ Β.Η ΜΕΓΑΛΗ ΕΚΡΗΞΗ Γ. Η ΔΙΚΑΙΩΣΗ
-    4: 938ΚΑΛ
+    4: 938ΓΟΥ
     5: '16460'
     8: ΚΑΔΜΟΣ
     9: ΑΘΗΝΑ
     10: '2012'
     11: 295Σ
     12: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
     13: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
@@ -641907,35 +641943,36 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12990
   authors:
-  - ΤΕΡΖΟΠΟΥΛΟΥ,ΛΟΛΑ,ΠΑΤΣΑΛΙΑ,ΚΑΤΕΡΙΝΑ
+  - ΠΑΤΣΑΛΙΑ,ΚΑΤΕΡΙΝΑ,ΤΕΡΖΟΠΟΥΛΟΥ,ΛΟΛΑ
   title: ΝΟΜΟΛΟΓΙΑ ΤΟΥ ΠΡΩΤΟΔΙΚΕΙΟΥ ΑΡΤΗΣ ΕΠΙ ΤΟΥ ΑΓΡΟΤΙΚΟΥ ΖΗΤΗΜΑΤΟΣ
-  dewey: 938.65 ΤΕΡ
+  dewey: 938.65 ΠΑΤ
   entry_numbers:
   - '16456'
+  - '17229'
   editor: Μ/Φ ΣΥΛΛΟΓΟΣ ΣΚΟΥΦΑΣ // ΑΡΤΑ
   edition_year: 1981
   pages: 31
   topics:
   - ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 12990
-    1: ΤΕΡΖΟΠΟΥΛΟΥ,ΛΟΛΑ,ΠΑΤΣΑΛΙΑ,ΚΑΤΕΡΙΝΑ
+    1: ΠΑΤΣΑΛΙΑ,ΚΑΤΕΡΙΝΑ,ΤΕΡΖΟΠΟΥΛΟΥ,ΛΟΛΑ
     2: ΝΟΜΟΛΟΓΙΑ ΤΟΥ ΠΡΩΤΟΔΙΚΕΙΟΥ ΑΡΤΗΣ ΕΠΙ ΤΟΥ ΑΓΡΟΤΙΚΟΥ ΖΗΤΗΜΑΤΟΣ
-    4: 938.65ΤΕΡ
-    5: '16456'
+    4: 938.65ΠΑΤ
+    5: 16456-17229
     8: Μ/Φ ΣΥΛΛΟΓΟΣ ΣΚΟΥΦΑΣ
     9: ΑΡΤΑ
     10: '1981'
     11: 31Σ
     12: ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
     13: ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
     14: ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
@@ -641960,14 +641997,15 @@
     30: null
 - dbase_number: 12991
   authors: []
   title: ΠΑΙΔΕΣ ΕΛΛΗΝΩΝ ΙΤΕ
   dewey: 938 ΚΑΣ
   entry_numbers:
   - '16506'
+  - '10043'
   editor: ΑΚΑΔΗΜΙΑ ΑΘΗΝΩΝ // ΑΘΗΝΑ
   edition_year: 1972
   pages: 18
   topics:
   - ΠΑΝΗΓΥΡΙΚΗ ΣΥΝΕΔΡΙΑ
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
@@ -641975,15 +642013,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 12991
     1: Χ.Σ.
     2: ΠΑΙΔΕΣ ΕΛΛΗΝΩΝ ΙΤΕ
     4: 938ΚΑΣ
-    5: '16506'
+    5: 16506-10043
     8: ΑΚΑΔΗΜΙΑ ΑΘΗΝΩΝ
     9: ΑΘΗΝΑ
     10: '1972'
     11: 18Σ
     12: ΠΑΝΗΓΥΡΙΚΗ ΣΥΝΕΔΡΙΑ
     13: ΠΑΝΗΓΥΡΙΚΗ ΣΥΝΕΔΡΙΑ
     14: ΠΑΝΗΓΥΡΙΚΗ ΣΥΝΕΔΡΙΑ
@@ -643917,31 +643955,32 @@
     28: null
     29: null
     30: null
 - dbase_number: 13031
   authors:
   - NATIONAL GEOGRAPHIC
   title: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ 1453
-  dewey: 949.504 ΧΣ
+  dewey: 938.389 ΧΣ
   entry_numbers:
   - '16502'
+  - '12662'
   pages: 159
   topics:
   - ΑΛΩΣΗ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗΣ
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13031
     1: NATIONAL GEOGRAPHIC
     2: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ 1453
-    4: 949.504Χ.Σ
-    5: '16502'
+    4: 938.389Χ.Σ
+    5: 16502-12662
     11: 159Σ
     12: ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
     13: ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
     14: ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
     17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
     3: null
     6: null
@@ -645783,15 +645822,15 @@
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 13069
   authors: []
   title: ΘΗΣΑΥΡΟΙ ΤΗΣ ΑΡΜΕΝΙΑΣ
-  dewey: 938 ΑΡΜ
+  dewey: 938 ΧΣ
   entry_numbers:
   - '16558'
   editor: ΙΟΝΙΚΗ ΤΡΑΠΕΖΑ // ΑΘΗΝΑ
   edition_year: 1998
   pages: 240
   topics:
   - ΠΟΛΙΤΙΣΜΟΣ
@@ -645801,15 +645840,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13069
     1: Χ.Σ
     2: ΘΗΣΑΥΡΟΙ ΤΗΣ ΑΡΜΕΝΙΑΣ
-    4: 938ΑΡΜ
+    4: 938Χ.Σ
     5: '16558'
     8: ΙΟΝΙΚΗ ΤΡΑΠΕΖΑ
     9: ΑΘΗΝΑ
     10: '1998'
     11: 240Σ
     12: ΠΟΛΙΤΙΣΜΟΣ-ΑΡΜΕΝΙΑ
     13: ΠΟΛΙΤΙΣΜΟΣ-ΑΡΜΕΝΙΑ
@@ -652707,15 +652746,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 13207
   authors:
   - ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
   title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
-  dewey: 938.07 ΚΑΡ
+  dewey: 938.174 ΚΑΡ
   entry_numbers:
   - '16650'
   editor: REAL MEDIA // ΑΘΗΝΑ
   edition_year: 2014
   pages: 271
   topics:
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -652725,15 +652764,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13207
     1: ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
     2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
-    4: 938.07ΚΑΡ
+    4: 938.174ΚΑΡ
     5: '16650'
     8: REAL MEDIA
     9: ΑΘΗΝΑ
     10: '2014'
     11: 271Σ
     12: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -653370,15 +653409,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 13220
   authors:
   - ΕΥΑΓΓΕΛΙΔΗΣ,ΜΑΡΓΑΡΙΤΗΣ
   title: Η ΜΗΧΑΝΙΩΝΑ ΤΗΣ ΚΥΖΙΚΟΥ ΙΣΤΟΡΙΑ ΚΑΙ ΠΑΡΑΔΟΣΙΣ
-  dewey: 938.498 ΕΥΑ
+  dewey: 938.494 ΕΥΑ
   entry_numbers:
   - '16704'
   editor: ΕΤ.ΜΕΛ.ΑΝΑΤΟΛΗΣ // ΑΘΗΝΑ
   edition_year: 2005
   pages: 311
   topics: []
   copies: 2
@@ -653388,15 +653427,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-88703-0-5
   original_entry:
     0: 13220
     1: ΕΥΑΓΓΕΛΙΔΗΣ,ΜΑΡΓΑΡΙΤΗΣ
     2: Η ΜΗΧΑΝΙΩΝΑ ΤΗΣ ΚΥΖΙΚΟΥ ΙΣΤΟΡΙΑ ΚΑΙ ΠΑΡΑΔΟΣΙΣ
-    4: 938.498ΕΥΑ
+    4: 938.494ΕΥΑ
     5: '16704'
     8: ΕΤ.ΜΕΛ.ΑΝΑΤΟΛΗΣ
     9: ΑΘΗΝΑ
     10: '2005'
     11: 311Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -663930,43 +663969,42 @@
     29: null
     30: null
 - dbase_number: 13432
   authors:
   - ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
   title: Η ΕΠΙΣΤΡΟΦΗ
   subtitle: Η ΑΛΗΘΙΝΗ ΙΣΤΟΡΙΑ ΤΟΥ ΜΙΧΑΗΛ ΘΕΟΔΟΡΟΒΙΤΣ ΚΥΡΙΑΚΟΒ
-  dewey: 889.21 ΠΑΠ
+  dewey: 938.498 ΠΑΠ
   entry_numbers:
   - '16946'
   editor: ΔΙΟΠΤΡΑ // ΑΘΗΝΑ
   edition_year: 2012
   pages: 528
-  topics:
-  - ΛΟΓΟΤΕΧΝΙΑ
+  topics: []
   copies: 2
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-364-469-9
   original_entry:
     0: 13432
     1: ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
     2: Η ΕΠΙΣΤΡΟΦΗ
     3: Η ΑΛΗΘΙΝΗ ΙΣΤΟΡΙΑ ΤΟΥ ΜΙΧΑΗΛ ΘΕΟΔΟΡΟΒΙΤΣ ΚΥΡΙΑΚΟΒ
-    4: 889.21ΠΑΠ
+    4: 938.498ΠΑΠ
     5: '16946'
     8: ΔΙΟΠΤΡΑ
     9: ΑΘΗΝΑ
     10: '2012'
     11: 528Σ
-    12: ΛΟΓΟΤΕΧΝΙΑ
-    13: ΛΟΓΟΤΕΧΝΙΑ
-    14: ΛΟΓΟΤΕΧΝΙΑ
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     18: 978-960-36
     19: 4-469-9
     30: 2 ΑΝΤΙΤΥΠΑ
     6: null
     7: null
     15: null
@@ -664032,15 +664070,15 @@
     29: null
     30: null
 - dbase_number: 13434
   authors:
   - ΦΕΣΤΕΡΙΔΗΣ,ΤΑΣΟΣ
   title: Η ΕΛΛΗΝΙΚΗ ΠΟΝΤΙΑΚΗ ΚΟΙΝΟΤΗΤΑ ΤΟΥ ΜΕΤΑΛΛΕΙΟΥ ΤΑΥΡΟΥ (ΜΠΟΥΓΑ
   subtitle: ΜΑΝΤΕΝ) ΤΗΣ ΜΙΚΡΑΣ ΑΣΙΑΣ
-  dewey: 938.993 ΦΕΣ
+  dewey: 938.498 ΦΕΣ
   entry_numbers:
   - '16947'
   editor: ΜΕΛΙΣΣΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1999
   pages: 271
   topics:
   - ΛΑΟΓΡΑΦΙΑ
@@ -664051,15 +664089,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 13434
     1: ΦΕΣΤΕΡΙΔΗΣ,ΤΑΣΟΣ
     2: Η ΕΛΛΗΝΙΚΗ ΠΟΝΤΙΑΚΗ ΚΟΙΝΟΤΗΤΑ ΤΟΥ ΜΕΤΑΛΛΕΙΟΥ ΤΑΥΡΟΥ (ΜΠΟΥΓΑ
     3: ΜΑΝΤΕΝ) ΤΗΣ ΜΙΚΡΑΣ ΑΣΙΑΣ
-    4: 938.993ΦΕΣ
+    4: 938.498ΦΕΣ
     5: '16947'
     8: ΜΕΛΙΣΣΑ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1999'
     11: 271Σ
     12: ΙΣΤΟΡΙΑ-ΛΑΟΓΡΑΦΙΑ
     13: ΙΣΤΟΡΙΑ-ΛΑΟΓΡΑΦΙΑ
@@ -672379,15 +672417,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 13604
   authors:
   - ΟΙΚΟΝΟΜΙΔΗ,ΦΟΙΒΟΥ
   title: ΟΙ ΠΡΟΣΤΑΤΕΣ Η ΑΛΗΘΙΝΗ ΙΣΤΟΡΙΑ ΤΗΣ ΑΝΤΙΣΤΑΣΗΣ
-  dewey: 320 ΟΙΚ
+  dewey: 938.760 ΟΙΚ
   entry_numbers:
   - '17106'
   editor: ΟΡΦΕΑΣ // ΑΘΗΝΑ
   edition_year: 1990
   pages: 431
   topics:
   - ΠΟΛΙΤΙΚΗ
@@ -672396,15 +672434,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13604
     1: ΟΙΚΟΝΟΜΙΔΗ,ΦΟΙΒΟΥ
     2: ΟΙ ΠΡΟΣΤΑΤΕΣ Η ΑΛΗΘΙΝΗ ΙΣΤΟΡΙΑ ΤΗΣ ΑΝΤΙΣΤΑΣΗΣ
-    4: 320ΟΙΚ
+    4: 938.760ΟΙΚ
     5: '17106'
     8: ΟΡΦΕΑΣ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 431Σ
     12: ΠΟΛΙΤΙΚΗ
     13: ΠΟΛΙΤΙΚΗ
@@ -673774,53 +673812,50 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13632
-  authors:
-  - ΣΠΗΛΙΟΣ,ΑΠΟΣΤΟΛΟΣ
-  title: ΠΕΛΑΣΓΙΚΗ ΗΠΕΙΡΟΣ ΚΑΙ ΑΡΑΧΘΟΣ Ο ΠΕΛΑΣΓΙΚΟΣ
-  dewey: 938.939 ΣΠΗ
+  authors: []
+  title: 28 ΟΚΤΩΒΡΙΟΥ 1940
+  subtitle: 70 ΧΡΟΝΙΑ ΜΕΤΑ
+  dewey: 938.752 ΧΣ
   entry_numbers:
-  - '17184'
-  editor: ΝΕΑ ΘΕΣΙΣ // ΑΘΗΝΑ
-  edition_year: 2002
-  pages: 151
+  - '21620'
+  editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
+  edition_year: 2010
+  pages: 78
   topics:
-  - ΗΠΕΙΡΟΣ
-  - ΑΡΑΧΘΟΣ
-  donors:
-  - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - 28 ΟΚΤΩΒΡΙΟΥ
   has_cd: false
   has_dvd: false
   offprint: false
-  isbn: 960-7076-09-5
+  ean: '9789604751662'
   original_entry:
     0: 13632
-    1: ΣΠΗΛΙΟΣ,ΑΠΟΣΤΟΛΟΣ
-    2: ΠΕΛΑΣΓΙΚΗ ΗΠΕΙΡΟΣ ΚΑΙ ΑΡΑΧΘΟΣ Ο ΠΕΛΑΣΓΙΚΟΣ
-    4: 938.939ΣΠΗ
-    5: '17184'
-    8: ΝΕΑ ΘΕΣΙΣ
+    1: Χ.Σ
+    2: 28 ΟΚΤΩΒΡΙΟΥ 1940
+    3: 70 ΧΡΟΝΙΑ ΜΕΤΑ
+    4: 938.752Χ.Σ
+    5: '21620'
+    8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
-    10: '2002'
-    11: 151Σ
-    12: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΑΡΑΧΘΟΣ
-    13: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΑΡΑΧΘΟΣ
-    14: ΗΠΕΙΡΟΣ-ΑΡΑΧΘΟΣ
-    17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
-    18: 960-7076-0
-    19: 9-5
-    3: null
+    10: '2010'
+    11: '78'
+    12: ΙΣΤΟΡΙΑ-28 ΟΚΤΩΒΡΙΟΥ
+    13: ΙΣΤΟΡΙΑ-28 ΟΚΤΩΒΡΙΟΥ
+    14: 28 ΟΚΤΩΒΡΙΟΥ
+    18: '9789604751'
+    19: '662'
     6: null
     7: null
     15: null
     16: null
+    17: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
@@ -674228,15 +674263,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 13641
   authors:
   - ΣΔΡΑΚΑ,ΕΥΑΓΓΕΛΟΥ
   title: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΩΣ ΥΙΟΣ ΤΟΥ ΘΕΟΥ ΑΜΜΩΝΟΣ-ΔΙΟΣ
-  dewey: 938.070 ΣΔΡ
+  dewey: 938.174 ΣΔΡ
   entry_numbers:
   - '17182'
   editor: ΚΥΡΟΜΑΝΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1995
   pages: 170
   topics:
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -674245,15 +674280,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13641
     1: ΣΔΡΑΚΑ,ΕΥΑΓΓΕΛΟΥ
     2: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΩΣ ΥΙΟΣ ΤΟΥ ΘΕΟΥ ΑΜΜΩΝΟΣ-ΔΙΟΣ
-    4: 938.070ΣΔΡ
+    4: 938.174ΣΔΡ
     5: '17182'
     8: ΚΥΡΟΜΑΝΟΣ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1995'
     11: 170Σ
     12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -675315,15 +675350,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 13663
   authors:
   - FAURE,PAUL
   title: Η ΚΑΘΗΜΕΡΙΝΗ ΖΩΗ ΤΗΝ ΕΠΟΧΗ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
-  dewey: 938.070 FAU
+  dewey: 938.174 FAU
   entry_numbers:
   - '17158'
   editor: ΠΑΠΑΔΗΜΑ // ΑΘΗΝΑ
   edition_year: 1977
   pages: 400
   topics:
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -675333,15 +675368,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-206-159-6
   original_entry:
     0: 13663
     1: FAURE,PAUL
     2: Η ΚΑΘΗΜΕΡΙΝΗ ΖΩΗ ΤΗΝ ΕΠΟΧΗ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
-    4: 938.070FAU
+    4: 938.174FAU
     5: '17158'
     8: ΠΑΠΑΔΗΜΑ
     9: ΑΘΗΝΑ
     10: '1977'
     11: 400Σ
     12: ΙΣΤΟΡΙΑ-ΜΕΓΑΛΟΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΙΣΤΟΡΙΑ-ΜΕΓΑΛΟΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -675365,15 +675400,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 13664
   authors:
   - STONEMAN,RICHARD
   title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΘΡΥΛΟΣ-ΜΥΘΟΣ-ΙΣΤΟΡΙΑ
-  dewey: 938.070 STO
+  dewey: 938.174 STO
   entry_numbers:
   - '17159'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 1993
   pages: 279
   topics:
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -675383,15 +675418,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-236-312-6
   original_entry:
     0: 13664
     1: STONEMAN,RICHARD
     2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΘΡΥΛΟΣ-ΜΥΘΟΣ-ΙΣΤΟΡΙΑ
-    4: 938.070STO
+    4: 938.174STO
     5: '17159'
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '1993'
     11: 279Σ
     12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΚΑΝΔΡΟΣ
@@ -676753,15 +676788,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 13692
   authors:
   - ΧΡΥΣΑΝΘΟΠΟΥΛΟΥ,ΦΩΤΙΟΥ
   title: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ ΠΕΡΙ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
-  dewey: 938.509 ΦΩΤ
+  dewey: 938.509 ΧΡΥ
   entry_numbers:
   - '17188'
   editor: None // ΑΘΗΝΑ
   edition_year: 1899
   pages: 470
   topics:
   - ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
@@ -676770,15 +676805,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13692
     1: ΧΡΥΣΑΝΘΟΠΟΥΛΟΥ,ΦΩΤΙΟΥ
     2: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ ΠΕΡΙ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
-    4: 938.509ΦΩΤ
+    4: 938.509ΧΡΥ
     5: '17188'
     9: ΑΘΗΝΑ
     10: '1899'
     11: 470Σ
     12: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
     13: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
     14: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
@@ -683398,15 +683433,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13828
   authors:
   - ΝΤΑΛΑ,ΧΡΗΣΤΟΥ
-  title: ΤΟ ΔΙΑΣΤΡΑΤΟ ΠΟΥ ΑΓΑΠΗΣΑΜΕ
+  title: ΤΟ ΔΙΣΤΡΑΤΟ ΠΟΥ ΑΓΑΠΗΣΑΜΕ
   dewey: 938.939 ΝΤΑ
   entry_numbers:
   - '17329'
   editor: None // ΑΘΗΝΑ
   edition_year: 2008
   pages: 191
   topics:
@@ -683415,15 +683450,15 @@
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13828
     1: ΝΤΑΛΑ,ΧΡΗΣΤΟΥ
-    2: ΤΟ ΔΙΑΣΤΡΑΤΟ ΠΟΥ ΑΓΑΠΗΣΑΜΕ
+    2: ΤΟ ΔΙΣΤΡΑΤΟ ΠΟΥ ΑΓΑΠΗΣΑΜΕ
     4: 938.939ΝΤΑ
     5: '17329'
     9: ΑΘΗΝΑ
     10: '2008'
     11: 191Σ
     12: ΙΣΤΟΡΙΑ-ΔΙΣΤΡΑΤΟ
     13: ΙΣΤΟΡΙΑ-ΔΙΣΤΡΑΤΟ
@@ -684868,63 +684903,58 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13858
   authors:
-  - ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
-  title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
-  dewey: 938.070 ΚΑΡ
+  - ΤΕΛΩΝΑ,ΝΙΚΟΛΑΟΥ
+  title: ΤΑ ΕΝ ΚΑΡΒΑΣΑΡΑ ΑΠΟ ΤΗΣ ΕΝΑΡΞΕΩΣ ΤΟΥ ΙΕΡΟΥ ΑΓΩΝΟΣ
+  dewey: 938.22 ΤΕΛ
   entry_numbers:
-  - '17352'
-  editor: REAL NEWS // ΑΘΗΝΑ
-  edition_year: 2014
-  pages: 224
+  - '13207'
+  editor: ΒΙΒΛΙΟΘΗΚΗ ΑΜΦΙΛΟΧΙΑ // None
+  pages: 238
   topics:
-  - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  - ΙΣΤΟΡΙΑ
-  donors:
-  - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
-  volume: ΤΟΜΟ Β-Γ
+  - ΚΑΡΒΑΣΑΡΑΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13858
-    1: ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
-    2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
-    4: 938.070ΚΑΡ
-    5: '17352'
-    8: REAL NEWS
-    9: ΑΘΗΝΑ
-    10: '2014'
-    11: 224Σ
-    12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    14: ΙΣΤΟΡΙΑ -ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
-    30: ΤΟΜΟ Β-Γ
+    1: ΤΕΛΩΝΑ,ΝΙΚΟΛΑΟΥ
+    2: ΤΑ ΕΝ ΚΑΡΒΑΣΑΡΑ ΑΠΟ ΤΗΣ ΕΝΑΡΞΕΩΣ ΤΟΥ ΙΕΡΟΥ ΑΓΩΝΟΣ
+    4: 938.22ΤΕΛ
+    5: '13207'
+    8: ΒΙΒΛΙΟΘΗΚΗ ΑΜΦΙΛΟΧΙΑ
+    11: '238'
+    12: ΙΣΤΟΡΙΑ-ΚΑΡΒΑΣΑΡΑΣ
+    13: ΙΣΤΟΡΙΑ-ΚΑΡΒΑΣΑΡΑΣ
+    14: ΙΣΤΟΡΙΑ-ΚΑΡΒΑΣΑΡΑΣ
     3: null
     6: null
     7: null
+    9: null
+    10: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
+    30: null
 - dbase_number: 13859
   authors:
   - ΣΦΕΝΔΟΝΗ,Ν.
   title: ΜΑΚΕΔΟΝΙΚΟΝ ΗΜΕΡΟΛΟΓΙΟΝ
   dewey: 889.21 ΣΦΕ
   entry_numbers:
   - '17370'
@@ -686487,15 +686517,16 @@
     29: null
     30: null
 - dbase_number: 13891
   authors:
   - FASSO,GUIDO
   title: Η ΔΗΜΟΚΡΑΤΙΑ ΣΤΗΝ ΕΛΛΑΔΑ
   dewey: 938 FAS
-  entry_numbers: []
+  entry_numbers:
+  - '17420'
   editor: ΠΟΣΕΙΔΩΝΑΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1971
   pages: 176
   topics:
   - ΠΟΛΙΤΙΚΗ
   donors:
   - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
@@ -686503,24 +686534,24 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 13891
     1: FASSO,GUIDO
     2: Η ΔΗΜΟΚΡΑΤΙΑ ΣΤΗΝ ΕΛΛΑΔΑ
     4: 938FAS
+    5: '17420'
     8: ΠΟΣΕΙΔΩΝΑΣ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1971'
     11: 176Σ
     12: ΠΟΛΙΤΙΚΗ
     13: ΠΟΛΙΤΙΚΗ
     14: ΠΟΛΙΤΙΚΗ
     17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
     3: null
-    5: null
     6: null
     7: null
     15: null
     16: null
     18: null
     19: null
     20: null
@@ -686629,51 +686660,48 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13894
   authors:
-  - ΤΖΙΚΟΥ,ΦΩΤΕΙΝΗ
-  title: Ο ΑΓΝΩΣΤΟΣ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  dewey: 938.07 ΤΖΙ
+  - ΨΗΜΜΕΝΟΥ,ΝΙΚΟΥ
+  title: ΑΙΤΩΛΟΑΚΑΡΝΑΝΕΣ ΛΟΓΙΟΙ
+  dewey: 938.22 ΨΗΜ
   entry_numbers:
-  - '17408'
-  editor: ΑΡΧΕΤΥΠΟ // ΑΘΗΝΑ
-  edition_year: 2004
-  pages: 254
+  - '21490'
+  editor: ΔΩΤΙΟΝ // ΙΩΑΝΝΙΝΑ
+  edition_year: 2021
+  pages: 95
   topics:
-  - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  donors:
-  - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - ΛΟΓΙΟΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
   has_cd: false
   has_dvd: false
   offprint: false
-  isbn: 960-421-030-0
   original_entry:
     0: 13894
-    1: ΤΖΙΚΟΥ,ΦΩΤΕΙΝΗ
-    2: Ο ΑΓΝΩΣΤΟΣ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    4: 938.07ΤΖΙ
-    5: '17408'
-    8: ΑΡΧΕΤΥΠΟ
-    9: ΑΘΗΝΑ
-    10: '2004'
-    11: 254Σ
-    12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    14: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
-    18: 960-421-03
-    19: 0-0
+    1: ΨΗΜΜΕΝΟΥ,ΝΙΚΟΥ
+    2: ΑΙΤΩΛΟΑΚΑΡΝΑΝΕΣ ΛΟΓΙΟΙ
+    4: 938.22ΨΗΜ
+    5: '21490'
+    8: ΔΩΤΙΟΝ
+    9: ΙΩΑΝΝΙΝΑ
+    10: '2021'
+    11: '95'
+    12: ΛΟΓΙΟΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
+    13: ΛΟΓΙΟΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
+    14: ΛΟΓΙΟΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
     3: null
     6: null
     7: null
     15: null
     16: null
+    17: null
+    18: null
+    19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
@@ -688313,46 +688341,45 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13928
   authors:
-  - ΣΔΡΑΚΑ,ΕΥΑΓΓΕΛΟΥ
-  title: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΩΣ ΥΙΟΣ ΤΟΥ ΘΕΟΥ ΑΜΜΩΝΟΣ-ΔΙΟΣ
-  entry_numbers: []
-  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
-  edition_year: 1971
-  pages: 110
+  - ΓΡΗΓΟΡΟΓΙΑΝΝΗ,Α.
+  title: Ο ΜΕΙΖΩΝ ΕΛΛΗΝΙΣΜΟΣ
+  dewey: 938.1 ΓΡΗ
+  entry_numbers:
+  - '21549'
+  editor: ΕΚΔΟΣΕΙΣ ΑΣΕ Α.Ε // None
+  pages: 235
   topics:
-  - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  donors:
-  - ΤΣΙΛΙΓΙΑΝΝΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - ΕΛΛΗΝΙΣΜΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 13928
-    1: ΣΔΡΑΚΑ,ΕΥΑΓΓΕΛΟΥ
-    2: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΩΣ ΥΙΟΣ ΤΟΥ ΘΕΟΥ ΑΜΜΩΝΟΣ-ΔΙΟΣ
-    9: ΘΕΣ/ΝΙΚΗ
-    10: '1971'
-    11: 110Σ
-    12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    14: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-    17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
+    1: ΓΡΗΓΟΡΟΓΙΑΝΝΗ,Α.
+    2: Ο ΜΕΙΖΩΝ ΕΛΛΗΝΙΣΜΟΣ
+    4: 938.1ΓΡΗ
+    5: '21549'
+    8: ΕΚΔΟΣΕΙΣ ΑΣΕ Α.Ε
+    11: '235'
+    12: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
+    13: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
+    14: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
     3: null
-    4: null
-    5: null
     6: null
     7: null
-    8: null
+    9: null
+    10: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
@@ -692234,15 +692261,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 14008
   authors: []
   title: ΕΚΘΕΣΙΣ ΤΩΝ ΓΕΝΟΜΕΝΩΝ ΖΗΜΙΩΝ ΕΝ ΓΕΝΕΙ ΗΠΕΙΡΟΥ ΑΠΟ ΤΗΣ ΚΗΡΥΞΕ
   subtitle: ΤΟΥ ΕΛΛΗΝΟΙΤΑΛΙΚΟΥ ΜΕΧΡΙ ΤΗΣ ΑΠΕΛΕΥΘΕΡΩΣΕΩΣ ΤΗΣ ΟΚΤΩΒΡΙΟΣ 44
-  dewey: 938.752 ΕΚΘ
+  dewey: 938.752 ΧΣ
   entry_numbers:
   - '17525'
   editor: None // ΑΘΗΝΑ
   edition_year: 1987
   pages: 175
   topics:
   - ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ
@@ -692254,15 +692281,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 14008
     1: Χ.Σ.
     2: ΕΚΘΕΣΙΣ ΤΩΝ ΓΕΝΟΜΕΝΩΝ ΖΗΜΙΩΝ ΕΝ ΓΕΝΕΙ ΗΠΕΙΡΟΥ ΑΠΟ ΤΗΣ ΚΗΡΥΞΕ
     3: ΤΟΥ ΕΛΛΗΝΟΙΤΑΛΙΚΟΥ ΜΕΧΡΙ ΤΗΣ ΑΠΕΛΕΥΘΕΡΩΣΕΩΣ ΤΗΣ ΟΚΤΩΒΡΙΟΣ 44
-    4: 938.752ΕΚΘ
+    4: 938.752Χ.Σ
     5: '17525'
     9: ΑΘΗΝΑ
     10: '1987'
     11: 175Σ
     12: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ-ΗΠΕΙΡΟΣ
     13: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ-ΑΡΤΑ
     14: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ-ΙΣΤΟΡΙΑ
@@ -694045,15 +694072,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 14045
   authors:
   - ΟΙΚΟΝΟΜΟΥ,ΜΑΝΘΟΥ
   title: ΜΑΝΘΟΣ ΟΙΚΟΝΟΜΟΥ Ο ΠΡΩΘΥΠΟΥΡΓΟΣ ΤΟΥ ΑΛΗ ΠΑΣΑ
-  dewey: 938.484 ΟΙΚ
+  dewey: 938.494 ΟΙΚ
   entry_numbers:
   - '17568'
   editor: ΗΠΕΙΡΩΤΙΚΗ ΕΣΤΙΑ // ΙΩΑΝΝΙΝΑ
   edition_year: 1959
   pages: 16
   topics:
   - ΑΛΗ ΠΑΣΑΣ
@@ -694062,15 +694089,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 14045
     1: ΟΙΚΟΝΟΜΟΥ,ΜΑΝΘΟΥ
     2: ΜΑΝΘΟΣ ΟΙΚΟΝΟΜΟΥ Ο ΠΡΩΘΥΠΟΥΡΓΟΣ ΤΟΥ ΑΛΗ ΠΑΣΑ
-    4: 938.484ΟΙΚ
+    4: 938.494ΟΙΚ
     5: '17568'
     8: ΗΠΕΙΡΩΤΙΚΗ ΕΣΤΙΑ
     9: ΙΩΑΝΝΙΝΑ
     10: '1959'
     11: 16Σ
     12: ΙΣΤΟΡΙΑ-ΑΛΗ ΠΑΣΑ
     13: ΙΣΤΟΡΙΑ-ΑΛΗ ΠΑΣΑ
@@ -697540,15 +697567,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 14116
   authors: []
   title: ΣΚΟΤΕΙΝΗ ΕΠΤΑΕΤΙΑ
   subtitle: 1967-1974 Η ΔΙΚΤΑΤΟΡΙΑ ΤΩΝ ΣΥΝΤΑΓΜΑΤΑΡΧΩΝ
-  dewey: 938.79 ΣΚΟ
+  dewey: 938.79 ΧΣ
   entry_numbers:
   - '1707'
   editor: ΙΔΡΥΜΑ ΒΟΥΛΗ ΕΛΛΗΝΩΝ // ΑΘΗΝΑ
   edition_year: 2014
   pages: 167
   topics:
   - ΔΙΚΤΑΤΟΡΙΑ
@@ -697557,15 +697584,15 @@
   offprint: false
   ean: 978-960-6757-89-1
   original_entry:
     0: 14116
     1: Χ.Σ.
     2: ΣΚΟΤΕΙΝΗ ΕΠΤΑΕΤΙΑ
     3: 1967-1974 Η ΔΙΚΤΑΤΟΡΙΑ ΤΩΝ ΣΥΝΤΑΓΜΑΤΑΡΧΩΝ
-    4: 938.79ΣΚΟ
+    4: 938.79Χ.Σ
     5: '1707'
     8: ΙΔΡΥΜΑ ΒΟΥΛΗ ΕΛΛΗΝΩΝ
     9: ΑΘΗΝΑ
     10: '2014'
     11: 167Σ
     12: ΙΣΤΟΡΙΑ-ΔΙΚΤΑΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ-ΔΙΚΤΑΤΟΡΙΑ
@@ -704386,15 +704413,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 14255
   authors:
   - ΑΜΠΑΤΖΗ,ΕΥΡΙΔΙΚΗ
   title: Η ΑΤΤΙΚΗ ΓΗ ΥΠΟΔΕΧΕΤΑΙ ΤΟΥΣ ΠΡΟΣΦΥΓΕΣ ΤΟΥ 22
-  dewey: 362.870 ΑΜΠ
+  dewey: 938.498 ΑΜΠ
   entry_numbers:
   - '17720'
   editor: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ // ΑΘΗΝΑ
   edition_year: 2016
   pages: 193
   topics:
   - ΠΡΟΣΦΥΓΕΣ 22
@@ -704404,15 +704431,15 @@
   has_dvd: false
   offprint: false
   isbn: 960-89284-1-9
   original_entry:
     0: 14255
     1: ΑΜΠΑΤΖΗ,ΕΥΡΙΔΙΚΗ
     2: Η ΑΤΤΙΚΗ ΓΗ ΥΠΟΔΕΧΕΤΑΙ ΤΟΥΣ ΠΡΟΣΦΥΓΕΣ ΤΟΥ 22
-    4: 362.870ΑΜΠ
+    4: 938.498ΑΜΠ
     5: '17720'
     8: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ
     9: ΑΘΗΝΑ
     10: '2016'
     11: 193Σ
     12: ΠΡΟΣΦΥΓΕΣ 22
     13: ΠΡΟΣΦΥΓΕΣ 22
@@ -704634,19 +704661,18 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14260
-  authors:
-  - ΓΟΥΝΑΡΗΣ,ΒΑΣΙΛΗΣ
+  authors: []
   title: ΤΟ ΑΓΝΩΣΤΟ ΜΕΤΩΠΟ ΤΩΝ ΒΑΛΚΑΝΙΚΩΝ ΠΟΛΕΜΩΝ
   subtitle: Η ΔΙΟΙΚΗΤΙΚΗ ΕΝΣΩΜΑΤΩΣΗ ΤΩΝ ΝΕΩΝ ΧΩΡΩΝ
-  dewey: 938.683 ΓΟΥ
+  dewey: 938.683 ΧΣ
   entry_numbers:
   - '17721'
   editor: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ // ΑΘΗΝΑ
   edition_year: 2012
   pages: 190
   topics:
   - ΒΑΛΚΑΝΙΚΟΣ ΠΟΛΕΜΟΣ
@@ -704655,18 +704681,18 @@
   - ΙΔΡΥΜΑ ΒΟΥΛΗΣ ΤΩΝ ΕΛΛΗΝΩΝ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-6757-62-4
   original_entry:
     0: 14260
-    1: ΓΟΥΝΑΡΗΣ,ΒΑΣΙΛΗΣ
+    1: Χ.Σ
     2: ΤΟ ΑΓΝΩΣΤΟ ΜΕΤΩΠΟ ΤΩΝ ΒΑΛΚΑΝΙΚΩΝ ΠΟΛΕΜΩΝ
     3: Η ΔΙΟΙΚΗΤΙΚΗ ΕΝΣΩΜΑΤΩΣΗ ΤΩΝ ΝΕΩΝ ΧΩΡΩΝ
-    4: 938.683ΓΟΥ
+    4: 938.683Χ.Σ
     5: '17721'
     8: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ
     9: ΑΘΗΝΑ
     10: '2012'
     11: 190Σ
     12: ΒΑΛΚΑΝΙΚΟΣ ΠΟΛΕΜΟΣ-ΕΝΣΩΜΑΤΩΣΗ
     13: ΒΑΛΚΑΝΙΚΟΣ ΠΟΛΕΜΟΣ-ΕΝΣΩΜΑΤΩΣΗ
@@ -705548,14 +705574,15 @@
     29: null
     30: null
 - dbase_number: 14278
   authors:
   - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
   title: ΠΡΩΙΜΟΙ ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΤΑ ΤΗΝ ΟΘΩΜΑΝΟΚ
   subtitle: ΡΑΤΙΑ (1453-1669) ΠΟΛΕΜΙΚΑ,ΠΟΛΙΤΙΚΑ ΚΑΙ ΘΡΗΣΚΕΥΤΙΚΑ ΓΕΓΟΝΟΤΑ
+  dewey: 938.498 ΒΑΚ
   entry_numbers:
   - '17772'
   editor: ΑΝΤ.ΣΤΑΜΟΥΛΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2000
   pages: 642
   topics:
   - ΟΘΩΜΑΝΟΚΡΑΤΙΑ
@@ -705566,26 +705593,26 @@
   offprint: false
   ean: 978-960-6741-48-7
   original_entry:
     0: 14278
     1: ΒΑΚΑΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
     2: ΠΡΩΙΜΟΙ ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΤΑ ΤΗΝ ΟΘΩΜΑΝΟΚ
     3: ΡΑΤΙΑ (1453-1669) ΠΟΛΕΜΙΚΑ,ΠΟΛΙΤΙΚΑ ΚΑΙ ΘΡΗΣΚΕΥΤΙΚΑ ΓΕΓΟΝΟΤΑ
+    4: 938.498ΒΑΚ
     5: '17772'
     8: ΑΝΤ.ΣΤΑΜΟΥΛΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2000'
     11: 642Σ
     12: ΟΘΩΜΑΝΟΚΡΑΤΙΑ
     13: ΟΘΩΜΑΝΟΚΡΤΑΙΑ
     14: ΟΘΩΜΑΝΟΚΡΑΤΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     18: 978-960-67
     19: 41-48-7
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -706596,15 +706623,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 14299
   authors:
   - ΖΟΥΡΑΒΛΙΟΒΑ-ΠΑΠΠΟΥ,ΑΙΚΑΤΕΡΙΝΗ
   title: ΓΛΩΣΣΑ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΑΖΟΦΙΚΗΣ
-  dewey: 956.5 ΖΟΥ
+  dewey: 983.498 ΖΟΥ
   entry_numbers:
   - '17777'
   editor: ΑΝΤ.ΣΤΑΜΟΥΛΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2009
   pages: 477
   topics:
   - ΠΑΙΔΕΙΑ
@@ -706614,15 +706641,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-6887-06-2
   original_entry:
     0: 14299
     1: ΖΟΥΡΑΒΛΙΟΒΑ-ΠΑΠΠΟΥ,ΑΙΚΑΤΕΡΙΝΗ
     2: ΓΛΩΣΣΑ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΑΖΟΦΙΚΗΣ
-    4: 956,5ΖΟΥ
+    4: 983.498ΖΟΥ
     5: '17777'
     8: ΑΝΤ.ΣΤΑΜΟΥΛΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2009'
     11: 477Σ
     12: ΠΑΙΔΕΙΑ
     13: ΠΑΙΔΕΙΑ
@@ -708300,15 +708327,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14333
   authors: []
   title: ΣΥΝΤΑΓΜΑΤΙΚΑ ΚΕΙΜΕΝΑ ΤΗΣ ΗΓΕΜΟΝΙΑΣ ΣΑΜΟΥ
-  dewey: 938.75 ΣΥΝ
+  dewey: 938.75 ΧΣ
   entry_numbers:
   - '17803'
   editor: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ // ΑΘΗΝΑ
   edition_year: 2013
   pages: 534
   topics:
   - ΣΥΝΤΑΓΜΑΤΙΚΑ ΚΕΙΜΕΝΑ
@@ -708319,15 +708346,15 @@
   has_dvd: false
   offprint: false
   ean: 978-960-6757-83-9
   original_entry:
     0: 14333
     1: Χ.Σ.
     2: ΣΥΝΤΑΓΜΑΤΙΚΑ ΚΕΙΜΕΝΑ ΤΗΣ ΗΓΕΜΟΝΙΑΣ ΣΑΜΟΥ
-    4: 938.75ΣΥΝ
+    4: 938.75Χ.Σ
     5: '17803'
     8: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ
     9: ΑΘΗΝΑ
     10: '2013'
     11: 534Σ
     12: ΣΥΝΤΑΓΜΑΤΙΚΑ ΚΕΙΜΕΝΑ-ΣΑΜΟΣ
     13: ΣΥΝΤΑΓΜΑΤΙΚΑ ΚΕΙΜΕΝΑ-ΣΑΜΟΣ
@@ -712803,15 +712830,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 14427
   authors:
   - ΤΣΙΡΚΙΝΙΔΗ,ΧΑΡΗ
   title: ΑΓΩΝΕΣ ΧΩΡΙΣ ΔΙΚΑΙΩΣΗ
-  dewey: 938.498 ΤΣΙ
+  dewey: 938.473 ΤΣΙ
   entry_numbers:
   - '17855'
   editor: ΕΡΩΔΙΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2002
   pages: 361
   topics: []
   donors:
@@ -712820,15 +712847,15 @@
   has_dvd: false
   offprint: false
   isbn: '9607942027'
   original_entry:
     0: 14427
     1: ΤΣΙΡΚΙΝΙΔΗ,ΧΑΡΗ
     2: ΑΓΩΝΕΣ ΧΩΡΙΣ ΔΙΚΑΙΩΣΗ
-    4: 938.498ΤΣΙ
+    4: 938.473ΤΣΙ
     5: '17855'
     8: ΕΡΩΔΙΟΣ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2002'
     11: 361Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -713052,15 +713079,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 14432
   authors:
   - ΣΥΜΕΩΝΙΔΟΥ-ΠΑΠΑΔΟΠΟΥΛΟΥ,ΠΑΡΥΣΑΤΙΣ
   title: ΤΡΑΠΕΖΟΥΣ Η ΠΟΛΗ ΣΤΟ ΦΩΣ ΤΟΥ ΠΟΛΙΤΙΣΜΟΥ ΤΗΣ
-  dewey: 938.498 SYM
+  dewey: 938.498 ΣΥΜ
   entry_numbers:
   - '17848'
   editor: UNIVERSITY STUDIO // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2011
   pages: 415
   topics:
   - '691'
@@ -713070,15 +713097,15 @@
   has_dvd: false
   offprint: false
   ean: '9789601219691'
   original_entry:
     0: 14432
     1: ΣΥΜΕΩΝΙΔΟΥ-ΠΑΠΑΔΟΠΟΥΛΟΥ,ΠΑΡΥΣΑΤΙΣ
     2: ΤΡΑΠΕΖΟΥΣ Η ΠΟΛΗ ΣΤΟ ΦΩΣ ΤΟΥ ΠΟΛΙΤΙΣΜΟΥ ΤΗΣ
-    4: 938.498SYM
+    4: 938.498ΣΥΜ
     5: '17848'
     8: UNIVERSITY STUDIO
     9: ΘΕΣ/ΝΙΚΗ
     10: '2011'
     11: 415Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -713102,15 +713129,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 14433
   authors:
   - ΧΡΗΣΤΟΥ,ΣΤΑΥΡΟΣ
   title: ΟΙ ΕΛΛΗΝΕΣ ΣΤΗ ΝΟΤΙΑ ΡΩΣΙΑ
-  dewey: 938.993 ΣΤΑ
+  dewey: 938.498 ΧΡΗ
   entry_numbers:
   - '17847'
   editor: UNIVERSITY STUDIO // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2009
   pages: 169
   topics: []
   donors:
@@ -713119,15 +713146,15 @@
   has_dvd: false
   offprint: false
   ean: '9789601218700'
   original_entry:
     0: 14433
     1: ΧΡΗΣΤΟΥ,ΣΤΑΥΡΟΣ
     2: ΟΙ ΕΛΛΗΝΕΣ ΣΤΗ ΝΟΤΙΑ ΡΩΣΙΑ
-    4: 938.993ΣΤΑ
+    4: 938.498ΧΡΗ
     5: '17847'
     8: UNIVERSITY STUDIO
     9: ΘΕΣ/ΝΙΚΗ
     10: '2009'
     11: 169Σ
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
@@ -713292,15 +713319,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14437
   authors: []
-  title: ΜΟΝΟΓΡΑΦΙΕΣ Η ΠΡΩΤΗ ΝΙΚΞΗ 1940-1941
+  title: ΜΟΝΟΓΡΑΦΙΕΣ Η ΠΡΩΤΗ ΝΙΚΗ 1940-1941
   dewey: 938.498 ΜΟΝ
   entry_numbers:
   - '17868'
   editor: NATONAL GEOGRAPHIC // ΑΘΗΝΑ
   edition_year: 2010
   pages: 158
   topics:
@@ -713310,15 +713337,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604880935'
   original_entry:
     0: 14437
     1: Χ.Σ.
-    2: ΜΟΝΟΓΡΑΦΙΕΣ Η ΠΡΩΤΗ ΝΙΚΞΗ 1940-1941
+    2: ΜΟΝΟΓΡΑΦΙΕΣ Η ΠΡΩΤΗ ΝΙΚΗ 1940-1941
     4: 938.498ΜΟΝ
     5: '17868'
     8: NATONAL GEOGRAPHIC
     9: ΑΘΗΝΑ
     10: '2010'
     11: 158Σ
     12: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ
@@ -713751,15 +713778,16 @@
     28: null
     29: null
 - dbase_number: 14446
   authors:
   - ΜΠΑΕΤΕΝ.ΛΙΒΕ-ΜΠΕΝΚΕ-ΚΟΥΝΤΣΛΕΡ,ΡΟΖΜΑΡΙ
   title: ΑΛΛΟΣ ΓΙΑ ΤΟ ΝΗΠΙΑΓΩΓΕΙΟ
   dewey: 808.899 ΜΠΑ
-  entry_numbers: []
+  entry_numbers:
+  - '17880'
   translators:
   - ΑΓΓΕΛΙΔΟΥ,ΜΑΡΙΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 20
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -713770,26 +713798,26 @@
   offprint: false
   isbn: '9602744561'
   original_entry:
     0: 14446
     1: ΜΠΑΕΤΕΝ.ΛΙΒΕ-ΜΠΕΝΚΕ-ΚΟΥΝΤΣΛΕΡ,ΡΟΖΜΑΡΙ
     2: ΑΛΛΟΣ ΓΙΑ ΤΟ ΝΗΠΙΑΓΩΓΕΙΟ
     4: 808.899ΜΠΑ
+    5: '17880'
     6: ΜΑΡΙΑ ΑΓΓΕΛΙΔΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 20Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΑΦΡΟΔΙΤΗΣ ΚΑΤΣΑΟΥΝΟΥ
     18: '9602744561'
     3: null
-    5: null
     7: null
     15: null
     16: null
     19: null
     20: null
     21: null
     22: null
@@ -714000,15 +714028,16 @@
     29: null
     30: null
 - dbase_number: 14451
   authors:
   - CARMI,EUGENIO-ECO,UMBERTO
   title: ΟΙ ΝΑΝΟΙ ΤΟΥ ΓΚΝΟΥ
   dewey: 808.899 ECO
-  entry_numbers: []
+  entry_numbers:
+  - '17873'
   translators:
   - ΚΑΛΛΙΦΑΤΙΔΗ,ΕΦΗ
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2004
   pages: 36
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -714019,26 +714048,26 @@
   offprint: false
   isbn: '9604069012'
   original_entry:
     0: 14451
     1: CARMI,EUGENIO-ECO,UMBERTO
     2: ΟΙ ΝΑΝΟΙ ΤΟΥ ΓΚΝΟΥ
     4: 808.899ECO
+    5: '17873'
     6: ΕΦΗ ΚΑΛΛΙΦΑΤΙΔΗ
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 36Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΑΦΡΟΔΙΤΗΣ ΚΑΤΣΑΟΥΝΟΥ
     18: '9604069012'
     3: null
-    5: null
     7: null
     15: null
     16: null
     19: null
     20: null
     21: null
     22: null
@@ -718185,17 +718214,17 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 14536
   authors:
-  - ΚΥΡΙΑΚΟΥ-ΞΑΝΘΟΠΟΥΛΟΥ,ΑΡΤΕΜΙΣ
+  - ΧΑΤΖΗΚΥΡΙΑΚΙΔΗΣ,ΚΥΡΙΑΚΟΣ-ΚΥΡΙΑΚΟΥ ΑΡΤΕΜΙ
   title: ΟΙ ΕΛΛΗΝΕΣ ΤΟΥ ΠΟΝΤΟΥ ΚΑΙ Η ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ 1461-1923
-  dewey: 938.498 ΚΥΡ
+  dewey: 938.4 ΧΑΤ
   entry_numbers:
   - '17960'
   editor: None // ΑΘΗΝΑ
   edition_year: 2015
   pages: 436
   topics:
   - ΠΟΝΤΟΣ
@@ -718203,17 +718232,17 @@
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 14536
-    1: ΚΥΡΙΑΚΟΥ-ΞΑΝΘΟΠΟΥΛΟΥ,ΑΡΤΕΜΙΣ
+    1: ΧΑΤΖΗΚΥΡΙΑΚΙΔΗΣ,ΚΥΡΙΑΚΟΣ-ΚΥΡΙΑΚΟΥ ΑΡΤΕΜΙ
     2: ΟΙ ΕΛΛΗΝΕΣ ΤΟΥ ΠΟΝΤΟΥ ΚΑΙ Η ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ 1461-1923
-    4: 938.498ΚΥΡ
+    4: 938.4ΧΑΤ
     5: '17960'
     9: ΑΘΗΝΑ
     10: '2015'
     11: 436Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -732449,17 +732478,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14829
   authors:
-  - ΤΖΟΡΙ,ΤΖΟΝ-ΜΠΑΡΝΕΤ,ΜΑΚ
+  - ΜΠΑΡΝΕΤ,ΜΑΚ-ΤΖΟΡΙ,ΤΖΟΝ
   title: ΤΟ ΤΡΟΜΕΡΟ ΔΙΔΥΜΟ
-  dewey: 808.899 ΤΖΟ
+  dewey: 808.899 ΜΠΑ
   entry_numbers:
   - '19656'
   translators:
   - ΚΟΛΥΔΑ,ΕΥΓΕΝΙΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2015
   pages: 227
@@ -732467,17 +732496,17 @@
   - ΝΕΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9786180110074'
   original_entry:
     0: 14829
-    1: ΤΖΟΡΙ,ΤΖΟΝ-ΜΠΑΡΝΕΤ,ΜΑΚ
+    1: ΜΠΑΡΝΕΤ,ΜΑΚ-ΤΖΟΡΙ,ΤΖΟΝ
     2: ΤΟ ΤΡΟΜΕΡΟ ΔΙΔΥΜΟ
-    4: 808.899ΤΖΟ
+    4: 808.899ΜΠΑ
     5: '19656'
     6: ΕΥΓΕΝΙΑ ΚΟΛΥΔΑ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2015'
     11: 227Σ
     12: ΝΕΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -737283,15 +737312,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14928
   authors:
-  - ΝΙΚΟΛΑΟΠΟΥΛΟΥ,ΑΓΓΕΛΙΚΗ
+  - ΝΙΚΟΛΟΠΟΥΛΟΥ,ΑΓΓΕΛΙΚΗ
   title: ΟΤΑΝ ΟΙ ΠΕΡΣΕΣ
   dewey: 808.899 ΝΙΚ
   entry_numbers:
   - '19902'
   editor: ΑΣΤΕΡΟΣ // ΑΘΗΝΑ
   edition_year: 1994
   pages: 225
@@ -737299,15 +737328,15 @@
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: '9602032979'
   original_entry:
     0: 14928
-    1: ΝΙΚΟΛΑΟΠΟΥΛΟΥ,ΑΓΓΕΛΙΚΗ
+    1: ΝΙΚΟΛΟΠΟΥΛΟΥ,ΑΓΓΕΛΙΚΗ
     2: ΟΤΑΝ ΟΙ ΠΕΡΣΕΣ
     4: 808.899ΝΙΚ
     5: '19902'
     8: ΑΣΤΕΡΟΣ
     9: ΑΘΗΝΑ
     10: '1994'
     11: 225Σ
@@ -739915,15 +739944,17 @@
     28: null
     29: null
     30: null
 - dbase_number: 14982
   authors:
   - ΚΟΝΤΑΡΑΣ,ΘΟΔΩΡΗΣ
   title: ΟΙ ΤΕΛΕΥΤΑΙΕΣ ΣΤΙΓΜΕΣ ΤΩΝ ΕΛΛΗΝΙΚΩΝ ΒΟΥΡΛΩΝ
-  entry_numbers: []
+  dewey: 938.498 ΚΟΝ
+  entry_numbers:
+  - '22885'
   editor: ΜΠΑΛΤΑ // ΑΘΗΝΑ
   edition_year: 2018
   pages: 79
   topics:
   - ΠΟΝΤΟΣ
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
@@ -739931,27 +739962,27 @@
   has_dvd: false
   offprint: false
   ean: '9786188287914'
   original_entry:
     0: 14982
     1: ΚΟΝΤΑΡΑΣ,ΘΟΔΩΡΗΣ
     2: ΟΙ ΤΕΛΕΥΤΑΙΕΣ ΣΤΙΓΜΕΣ ΤΩΝ ΕΛΛΗΝΙΚΩΝ ΒΟΥΡΛΩΝ
+    4: 938.498ΚΟΝ
+    5: '22885'
     8: ΜΠΑΛΤΑ
     9: ΑΘΗΝΑ
     10: '2018'
     11: 79Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     18: '9786188287'
     19: '914'
     3: null
-    4: null
-    5: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -741238,14 +741269,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 15008
   authors:
   - ΣΥΜΕΩΝΙΔΟΥ-ΠΑΠΑΔΟΠΟΥΛΟΥ,ΠΑΡΥΣΑΤΙΣ
   title: ΠΛΗΘΥΣΜΙΑΚΟΙ ΣΤΡΟΒΙΛΟΙ ΣΤΟΝ 21 ΑΙΩΝΑ
+  dewey: 938.43 ΣΥΜ
   entry_numbers:
   - '19968'
   editor: ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2016
   pages: 205
   topics:
   - ΠΛΗΘΥΣΜΟΣ
@@ -741257,28 +741289,28 @@
   has_dvd: false
   offprint: false
   ean: '9789605991692'
   original_entry:
     0: 15008
     1: ΣΥΜΕΩΝΙΔΟΥ-ΠΑΠΑΔΟΠΟΥΛΟΥ,ΠΑΡΥΣΑΤΙΣ
     2: ΠΛΗΘΥΣΜΙΑΚΟΙ ΣΤΡΟΒΙΛΟΙ ΣΤΟΝ 21 ΑΙΩΝΑ
+    4: 938.43ΣΥΜ
     5: '19968'
     8: ΚΥΡΙΑΚΙΔΗ
     9: ΘΕΣ/ΝΙΚΗ
     10: '2016'
     11: 205ΣΙΣ
     12: ΙΣΤΟΡΙΑ-ΠΛΗΘΥΣΜΟΣ
     13: ΣΥΡΙΑ-ΕΛΛΑΔΑ
     14: ΙΣΤΟΡΙΑ
     15: ΠΛΗΘΥΣΜΟΣ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
     18: '9789605991'
     19: '692'
     3: null
-    4: null
     6: null
     7: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -745234,38 +745266,39 @@
     29: null
     30: null
 - dbase_number: 15089
   authors:
   - BLYTON,ENID
   title: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΟΥ ΣΚΟΤΕΙΝΟΥ ΣΠΙΤΙΟΥ
   dewey: 808.899 BLY
-  entry_numbers: []
+  entry_numbers:
+  - '20080'
   translators:
   - ΓΙΟΥΡΓΟΣ,ΚΩΣΤΑΣ
   editor: GUTENBERG // ΑΘΗΝΑ
   pages: 181
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15089
     1: BLYTON,ENID
     2: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΟΥ ΣΚΟΤΕΙΝΟΥ ΣΠΙΤΙΟΥ
     4: 808.899BLY
+    5: '20080'
     6: ΚΩΣΤΑΣ ΓΙΟΥΡΓΟΣ
     8: GUTENBERG
     9: ΑΘΗΝΑ
     11: 181Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     3: null
-    5: null
     7: null
     10: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -750476,15 +750509,15 @@
     30: null
 - dbase_number: 15196
   authors:
   - ΤΣΕΧΩΦ,ΑΝΤΟΝ
   title: ΤΑ ΠΑΙΔΙΚΑ ΔΙΓΗΜΑΤΑ
   dewey: 808.899 ΤΣΕ
   entry_numbers:
-  - '20164'
+  - '20161'
   translators:
   - ΠΟΛΙΤΟΠΟΥΛΟΣ,ΓΙΩΡΓΗΣ
   editor: ΓΛΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1981
   pages: 117
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -750494,15 +750527,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 15196
     1: ΤΣΕΧΩΦ,ΑΝΤΟΝ
     2: ΤΑ ΠΑΙΔΙΚΑ ΔΙΓΗΜΑΤΑ
     4: 808.899ΤΣΕ
-    5: '20164'
+    5: '20161'
     6: ΓΙΩΡΓΗΣ ΠΟΛΙΤΟΠΟΥΛΟΣ
     8: ΓΛΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1981'
     11: 117Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -752413,38 +752446,39 @@
     29: null
     30: null
 - dbase_number: 15235
   authors:
   - ΧΑΤΟΓΛΟΥ,ΦΡΟΣΩ
   title: ΚΑΛΗΜΕΡΑ ΕΙΡΗΝΗ
   dewey: 808.899 ΧΑΤ
-  entry_numbers: []
+  entry_numbers:
+  - '20414'
   editor: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ // ΑΘΗΝΑ
   pages: 46
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   donors:
   - ΤΣΩΝΟΥ,ΒΑΣΙΛΙΚΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15235
     1: ΧΑΤΟΓΛΟΥ,ΦΡΟΣΩ
     2: ΚΑΛΗΜΕΡΑ ΕΙΡΗΝΗ
     4: 808.899ΧΑΤ
+    5: '20414'
     8: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ
     9: ΑΘΗΝΑ
     11: 46Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΒΑΣΙΛΙΚΗΣ ΤΣΩΝΟΥ
     3: null
-    5: null
     6: null
     7: null
     10: null
     15: null
     16: null
     18: null
     19: null
@@ -758045,40 +758079,41 @@
     29: null
     30: null
 - dbase_number: 15349
   authors:
   - ΖΑΙΡΗ-ΡΩΣΣΗ,ΡΕΝΑ
   title: ΔΥΟ ΦΙΛΙΑ ΓΙΑ ΤΗΝ ΑΜΕΛΙΑ
   dewey: 889.21 ΖΑΙ
-  entry_numbers: []
+  entry_numbers:
+  - '22779'
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2016
   pages: 562
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9786180114850'
   original_entry:
     0: 15349
     1: ΖΑΙΡΗ-ΡΩΣΣΗ,ΡΕΝΑ
     2: ΔΥΟ ΦΙΛΙΑ ΓΙΑ ΤΗΝ ΑΜΕΛΙΑ
     4: 889.21ΖΑΙ
+    5: '22779'
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2016'
     11: 562Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     18: '9786180114'
     19: '850'
     3: null
-    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     20: null
     21: null
@@ -766761,15 +766796,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15527
   authors:
   - GRISHAM,JOHN
-  title: ΤΟ ΝΗΣΙΣ ΚΑΜΙΝΟ
+  title: ΤΟ ΝΗΣΙ ΚΑΜΙΝΟ
   dewey: 810.11 GRI
   entry_numbers:
   - '20382'
   translators:
   - ΜΠΑΡΟΥΞΗΣ,ΓΙΩΡΓΟΣ
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2021
@@ -766779,15 +766814,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789601908373'
   original_entry:
     0: 15527
     1: GRISHAM,JOHN
-    2: ΤΟ ΝΗΣΙΣ ΚΑΜΙΝΟ
+    2: ΤΟ ΝΗΣΙ ΚΑΜΙΝΟ
     4: 810.11GRI
     5: '20382'
     6: ΓΙΩΡΓΟΣ ΜΠΑΡΟΥΞΗΣ
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '2021'
     11: 380Σ
@@ -768071,33 +768106,33 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15554
   authors:
-  - ΓΕΩΡΓΙΑΔΗ-ΤΣΟΡΩΝΗ,ΓΙΟΛΑΝΤΑ
+  - ΤΣΟΡΩΝΗ-ΓΕΩΡΓΙΑΔΗ,ΓΙΟΛΑΝΤΑ
   title: ΕΝΑ ΠΑΡΑΞΕΝΟ ΧΡΙΣΤΟΥΓΕΝΝΙΑΤΙΚΟ ΔΕΝΤΡΟ
-  dewey: 808.899 ΓΕΩ
+  dewey: 808.899 ΤΣΟ
   entry_numbers:
   - '20663'
   editor: ΣΑΒΒΑΛΑΣ // ΑΘΗΝΑ
   edition_year: 2020
   pages: 29
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604938100'
   original_entry:
     0: 15554
-    1: ΓΕΩΡΓΙΑΔΗ-ΤΣΟΡΩΝΗ,ΓΙΟΛΑΝΤΑ
+    1: ΤΣΟΡΩΝΗ-ΓΕΩΡΓΙΑΔΗ,ΓΙΟΛΑΝΤΑ
     2: ΕΝΑ ΠΑΡΑΞΕΝΟ ΧΡΙΣΤΟΥΓΕΝΝΙΑΤΙΚΟ ΔΕΝΤΡΟ
-    4: 808.899ΓΕΩ
+    4: 808.899ΤΣΟ
     5: '20663'
     8: ΣΑΒΒΑΛΑΣ
     9: ΑΘΗΝΑ
     10: '2020'
     11: 29Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -768119,15 +768154,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15555
   authors:
-  - ΓΕΩΡΓΙΑΔΗ-ΤΣΟΡΩΝΗ,ΓΙΟΛΑΝΤΑ
+  - ΤΣΟΡΩΝΗ-ΓΕΩΡΓΙΑΔΗ,ΓΙΟΛΑΝΤΑ
   title: Ο ΜΕΓΑΣ ΜΕΛΟΜΑΚΑΡΩΝ ΠΟΥ ΜΕΛΟΜΑΚΑΡΩΝΕ
   dewey: 808.899 ΓΕΩ
   entry_numbers:
   - '20664'
   editor: ΣΑΒΒΑΛΑΣ // ΑΘΗΝΑ
   edition_year: 2018
   pages: 28
@@ -768135,15 +768170,15 @@
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604935628'
   original_entry:
     0: 15555
-    1: ΓΕΩΡΓΙΑΔΗ-ΤΣΟΡΩΝΗ,ΓΙΟΛΑΝΤΑ
+    1: ΤΣΟΡΩΝΗ-ΓΕΩΡΓΙΑΔΗ,ΓΙΟΛΑΝΤΑ
     2: Ο ΜΕΓΑΣ ΜΕΛΟΜΑΚΑΡΩΝ ΠΟΥ ΜΕΛΟΜΑΚΑΡΩΝΕ
     4: 808.899ΓΕΩ
     5: '20664'
     8: ΣΑΒΒΑΛΑΣ
     9: ΑΘΗΝΑ
     10: '2018'
     11: 28Σ
@@ -771310,32 +771345,32 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15620
   authors:
-  - DRIAULT,E.
+  - ΝΤΡΙΟΤ,Ε.
   title: Ο ΒΑΣΙΛΕΥΣ ΚΩΝΣΤΑΝΤΙΝΟΣ
-  dewey: 938.687 DRI
+  dewey: 938.687 ΝΤΡ
   entry_numbers:
   - '16049'
   editor: ΠΡΩΙΑΣ // ΑΘΗΝΑ
   edition_year: 1930
   pages: 237
   topics:
   - ΒΙΟΓΡΑΦΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15620
-    1: DRIAULT,E.
+    1: ΝΤΡΙΟΤ,Ε.
     2: Ο ΒΑΣΙΛΕΥΣ ΚΩΝΣΤΑΝΤΙΝΟΣ
-    4: 938.687DRI
+    4: 938.687ΝΤΡ
     5: '16049'
     8: ΠΡΩΙΑΣ
     9: ΑΘΗΝΑ
     10: '1930'
     11: 237Σ
     12: ΙΣΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΑ
     13: ΙΣΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΑ
@@ -777058,44 +777093,46 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15741
   authors:
-  - ΣΤΑΜΑΤΗΣ, ΕΛΕΥΘΕΡΙΟΣ
-  title: ΚΥΡΙΟΙ, ΠΑΤΕ ΓΙΑ ΥΠΝΟ
+  - ΒΟΥΛΤΣΙΑΔΗ,ΓΕΩΡΓΙΟΥ
+  title: Η ΠΡΟΣΩΤΣΑΝΗ ΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ
+  dewey: 938.764 ΒΟΥ
   entry_numbers:
-  - '21078'
-  editor: ΔΟΥΡΕΙΟΣ ΙΠΠΟΣ // ΑΘΗΝΑ
-  edition_year: 2007
-  pages: 298
-  topics: []
+  - '12423'
+  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1995
+  pages: 437
+  topics:
+  - ΠΡΟΣΩΤΣΑΝΗ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789608835535'
   original_entry:
     0: 15741
-    1: ΣΤΑΜΑΤΗΣ, ΕΛΕΥΘΕΡΙΟΣ
-    2: ΚΥΡΙΟΙ, ΠΑΤΕ ΓΙΑ ΥΠΝΟ
-    5: '21078'
-    8: ΔΟΥΡΕΙΟΣ ΙΠΠΟΣ
-    9: ΑΘΗΝΑ
-    10: '2007'
-    11: '298'
+    1: ΒΟΥΛΤΣΙΑΔΗ,ΓΕΩΡΓΙΟΥ
+    2: Η ΠΡΟΣΩΤΣΑΝΗ ΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ
+    4: 938.764ΒΟΥ
+    5: '12423'
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1995'
+    11: '437'
+    12: ΠΡΟΣΩΤΣΑΝΗ
+    13: ΙΣΤΟΡΙΑ
+    14: ΠΡΟΣΩΤΣΑΝΗ
     18: '9789608835'
     19: '535'
     3: null
-    4: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
+    8: null
     15: null
     16: null
     17: null
     20: null
     21: null
     22: null
     23: null
@@ -778065,39 +778102,41 @@
     28: null
     29: null
     30: null
 - dbase_number: 15763
   authors:
   - ΘΕΟΔΩΡΑΚΟΠΟΥΛΟΥ,Ι.Ν.
   title: ΤΟ ΕΙΚΟΣΙΕΝΑ ΚΑΙ Ο ΣΥΓΧΡΟΝΟΣ ΕΛΛΗΝΙΣΜΟΣ
+  dewey: 938.5 ΘΕΟ
   entry_numbers:
   - '21098'
   editor: ΕΚΔ.ΤΩΝ ΦΙΛΩΝ // ΑΘΗΝΑ
   edition_year: 1972
   pages: 92
-  topics: []
+  topics:
+  - ΕΙΚΟΣΙΕΝΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15763
     1: ΘΕΟΔΩΡΑΚΟΠΟΥΛΟΥ,Ι.Ν.
     2: ΤΟ ΕΙΚΟΣΙΕΝΑ ΚΑΙ Ο ΣΥΓΧΡΟΝΟΣ ΕΛΛΗΝΙΣΜΟΣ
+    4: 938.5ΘΕΟ
     5: '21098'
     8: ΕΚΔ.ΤΩΝ ΦΙΛΩΝ
     9: ΑΘΗΝΑ
     10: '1972'
     11: '92'
+    12: ΙΣΤΟΡΙΑ-ΕΙΚΟΣΙΕΝΑ
+    13: ΕΙΚΟΣΙΕΝΑ
+    14: ΙΣΤΟΡΙΑ
     3: null
-    4: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -778287,45 +778326,46 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15768
-  authors:
-  - ΤΟΛΙΑΣ,Γ.
+  authors: []
   title: ΣΥΛΛΟΓΙΚΟ, Ο ΠΥΡΕΤΟΣ ΤΩΝ ΜΑΡΜΑΡΩΝ
+  dewey: 930.1 ΧΣ
   entry_numbers:
   - '21104'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 1996
   pages: 329
-  topics: []
+  topics:
+  - ΠΟΛΙΤΙΣΜΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604697861'
   original_entry:
     0: 15768
-    1: ΤΟΛΙΑΣ,Γ.
+    1: Χ.Σ
     2: ΣΥΛΛΟΓΙΚΟ, Ο ΠΥΡΕΤΟΣ ΤΩΝ ΜΑΡΜΑΡΩΝ
+    4: 930.1Χ.Σ
     5: '21104'
     8: ΤΟ ΒΗΜΑ
     9: ΑΘΗΝΑ
     10: '1996'
     11: '329'
+    12: ΙΣΤΟΡΙΑ-ΠΟΛΙΤΙΣΜΟΣ
+    13: ΠΟΛΙΤΙΣΜΟΣ
+    14: ΙΣΤΟΡΙΑ
     18: '9789604697'
     19: '861'
     3: null
-    4: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     20: null
     21: null
     22: null
     23: null
@@ -778607,39 +778647,41 @@
     28: null
     29: null
     30: null
 - dbase_number: 15775
   authors:
   - CASSIRER,ERNST
   title: ΔΟΚΙΜΙΟ ΓΙΑ ΤΟΝ ΑΝΘΡΩΠΟ
+  dewey: 901 CAS
   entry_numbers:
   - '21111'
   editor: ΚΑΛΒΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1972
   pages: 358
-  topics: []
+  topics:
+  - ΦΙΛΟΣΟΦΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15775
     1: CASSIRER,ERNST
     2: ΔΟΚΙΜΙΟ ΓΙΑ ΤΟΝ ΑΝΘΡΩΠΟ
+    4: 901CAS
     5: '21111'
     8: ΚΑΛΒΟΣ
     9: ΘΕΣ/ΝΙΚΗ
     10: '1972'
     11: '358'
+    12: ΦΙΛΟΣΟΦΙΑ
+    13: ΦΙΛΟΣΟΦΙΑ
+    14: ΦΙΛΟΣΟΦΙΑ
     3: null
-    4: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -778695,42 +778737,43 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15777
   authors:
-  - ΣΤΑΥΡΙΔΟΥ-ΖΑΦΡΑΚΑ ΑΛΚΜΙΝΗ
+  - ΖΑΦΡΑΚΑ-ΣΤΑΥΡΙΔΟΥ,ΑΛΚΜΗΝΗ
   title: ΙΓ ΠΑΝΕΛΛΗΝΙΟ ΙΣΤΟΡΙΚΟ ΣΥΝΕΔΡΙΟ
-  dewey: 938.498 ΣΤΑ
+  dewey: 938.498 ΖΑΦ
   entry_numbers:
   - '21113'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1993
   pages: 178
-  topics: []
+  topics:
+  - ΠΡΑΚΤΙΚΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15777
-    1: ΣΤΑΥΡΙΔΟΥ-ΖΑΦΡΑΚΑ ΑΛΚΜΙΝΗ
+    1: ΖΑΦΡΑΚΑ-ΣΤΑΥΡΙΔΟΥ,ΑΛΚΜΗΝΗ
     2: ΙΓ ΠΑΝΕΛΛΗΝΙΟ ΙΣΤΟΡΙΚΟ ΣΥΝΕΔΡΙΟ
-    4: 938.498ΣΤΑ
+    4: 938.498ΖΑΦ
     5: '21113'
     9: ΘΕΣ/ΝΙΚΗ
     10: '1993'
     11: '178'
+    12: ΠΡΑΚΤΙΚΑ
+    13: ΠΡΑΚΤΙΚΑ
+    14: ΠΡΑΚΤΙΚΑ
     3: null
     6: null
     7: null
     8: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -779017,38 +779060,39 @@
     29: null
     30: null
 - dbase_number: 15784
   authors: []
   title: ΙΣΤΟΡΙΚΗ ΠΟΡΕΙΑ ΤΗΣ ΘΕΣΣΑΛΟΝΙΚΗΣ
   dewey: 938.498 ΧΣ
   entry_numbers:
-  - '1120'
+  - '21120'
   editor: None // ΑΘΗΝΑ
   edition_year: 1988
   pages: 62
-  topics: []
+  topics:
+  - ΘΕΣΣΑΛΟΝΙΚΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15784
     1: Χ.Σ.
     2: ΙΣΤΟΡΙΚΗ ΠΟΡΕΙΑ ΤΗΣ ΘΕΣΣΑΛΟΝΙΚΗΣ
     4: 938.498Χ.Σ
-    5: '1120'
+    5: '21120'
     9: ΑΘΗΝΑ
     10: '1988'
     11: '62'
+    12: ΙΣΤΟΡΙΑ-ΘΕΣΣΑΛΟΝΙΚΗ
+    13: ΘΕΣΣΑΛΟΝΙΚΗ
+    14: ΙΣΤΟΡΙΑ
     3: null
     6: null
     7: null
     8: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -779698,39 +779742,41 @@
     28: null
     29: null
     30: null
 - dbase_number: 15799
   authors:
   - ΧΡΙΣΤΟΠΟΥΛΟΣ,Κ.Π.
   title: ΤΟ ΕΛΛΗΝΙΚΟΝ ΠΡΟΒΛΗΜΑ
+  dewey: 938.764 ΧΡΙ
   entry_numbers:
   - '21135'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1945
   pages: 123
-  topics: []
+  topics:
+  - '1940'
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15799
     1: ΧΡΙΣΤΟΠΟΥΛΟΣ,Κ.Π.
     2: ΤΟ ΕΛΛΗΝΙΚΟΝ ΠΡΟΒΛΗΜΑ
+    4: 938.764ΧΡΙ
     5: '21135'
     9: ΘΕΣ/ΝΙΚΗ
     10: '1945'
     11: '123'
+    12: ΙΣΤΟΡΙΑ-1940
+    13: ΙΣΤΟΡΙΑ
+    14: '1940'
     3: null
-    4: null
     6: null
     7: null
     8: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -779740,40 +779786,41 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15800
-  authors:
-  - Π.Ο.Α.Ε.Α
+  authors: []
   title: Η ΕΠΟΠΟΙΙΑ ΤΗΣ ΕΘΝΙΚΗΣ ΜΑΣ ΑΝΤΙΣΤΑΣΗΣ (1941-1945)
+  dewey: 938.764 ΧΣ
   entry_numbers:
   - '21136'
   pages: 133
-  topics: []
+  topics:
+  - ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15800
-    1: Π.Ο.Α.Ε.Α
+    1: Χ.Σ
     2: Η ΕΠΟΠΟΙΙΑ ΤΗΣ ΕΘΝΙΚΗΣ ΜΑΣ ΑΝΤΙΣΤΑΣΗΣ (1941-1945)
+    4: 938.764Χ.Σ
     5: '21136'
     11: '133'
+    12: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
+    13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
+    14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
     3: null
-    4: null
     6: null
     7: null
     8: null
     9: null
     10: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -779830,41 +779877,44 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15802
   authors:
-  - ΧΡΗΣΤΟΣ,ΚΩΣΤΑΣ
+  - ΧΡΗΣΤΟΥ,ΚΩΣΤΑΣ
   title: ΖΥΓΟΣ ΛΕΒΙΤΣΙΚΟ ΙΣΤΟΡΙΑ ΚΑΙ ΠΑΡΑΔΟΣΗ
+  dewey: 938.939 ΧΡΗ
   entry_numbers:
   - '21138'
   editor: None // ΑΘΗΝΑ
   edition_year: 2000
   pages: 317
-  topics: []
+  topics:
+  - ΙΤΟΡΙΑ
+  - ΖΥΓΟΣ ΛΕΒΙΝΣΙΚΟ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15802
-    1: ΧΡΗΣΤΟΣ,ΚΩΣΤΑΣ
+    1: ΧΡΗΣΤΟΥ,ΚΩΣΤΑΣ
     2: ΖΥΓΟΣ ΛΕΒΙΤΣΙΚΟ ΙΣΤΟΡΙΑ ΚΑΙ ΠΑΡΑΔΟΣΗ
+    4: 938.939ΧΡΗ
     5: '21138'
     9: ΑΘΗΝΑ
     10: '2000'
     11: '317'
+    12: ΙΤΟΡΙΑ
+    13: ΖΥΓΟΣ ΛΕΒΙΝΣΙΚΟ
+    14: ΙΣΤΟΡΙΑ
     3: null
-    4: null
     6: null
     7: null
     8: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -787995,14 +788045,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15968
   authors: []
   title: 70 ΕΠΙΣΤΗΜΟΝΕΣ ΠΟΥ ΑΛΛΑΞΑΝ ΤΟΝ ΚΟΣΜΟ
+  dewey: 920 ΧΣ
   entry_numbers:
   - '20986'
   editor: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
   edition_year: 2017
   pages: 127
   topics:
   - ΕΠΙΣΤΗΜΗ
@@ -788012,27 +788063,27 @@
   has_dvd: false
   offprint: false
   ean: '9789605038540'
   original_entry:
     0: 15968
     1: Χ.Σ.
     2: 70 ΕΠΙΣΤΗΜΟΝΕΣ ΠΟΥ ΑΛΛΑΞΑΝ ΤΟΝ ΚΟΣΜΟ
+    4: 920Χ.Σ
     5: '20986'
     8: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ
     9: ΑΘΗΝΑ
     10: '2017'
     11: '127'
     12: ΕΠΙΣΤΗΜΗ
     13: ΕΠΙΣΤΗΜΗ
     14: ΕΠΙΣΤΗΜΗ
     17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
     18: '9789605038'
     19: '540'
     3: null
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -788095,14 +788146,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 15970
   authors: []
   title: 1955 ΣΕΠΤΕΜΒΡΙΑΝΑ
   subtitle: ΟΙ ΜΑΥΡΕΣ ΜΕΡΕΣ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ ΤΗΣ ΠΟΛΗΣ
+  dewey: 938.498 ΧΣ
   entry_numbers:
   - '20977'
   editor: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
   edition_year: 2018
   pages: 299
   topics:
   - ΙΣΤΟΡΙΚΟ ΑΡΧΕΙΟ
@@ -788113,26 +788165,26 @@
   offprint: false
   ean: '9789605039646'
   original_entry:
     0: 15970
     1: Χ.Σ.
     2: 1955 ΣΕΠΤΕΜΒΡΙΑΝΑ
     3: ΟΙ ΜΑΥΡΕΣ ΜΕΡΕΣ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ ΤΗΣ ΠΟΛΗΣ
+    4: 938.498Χ.Σ
     5: '20977'
     8: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ
     9: ΑΘΗΝΑ
     10: '2018'
     11: '299'
     12: ΙΣΤΟΡΙΚΟ ΑΡΧΕΙΟ
     13: ΙΣΤΟΡΙΚΟ ΑΡΧΕΙΟ
     14: ΙΣΤΟΡΙΚΟ ΑΡΧΕΙΟ
     17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
     18: '9789605039'
     19: '646'
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -788144,14 +788196,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 15971
   authors:
   - ΑΝΤΩΝΙΑΔΗΣ,ΑΝΤΩΝΗΣ
   title: ΤΑ 100 ΓΕΓΟΝΟΤΑ ΠΟΥ ΣΗΜΑΔΕΨΑΝ ΤΗΝ ΕΛΛΑΔΑ ΑΠ ΤΟ 1821 ΕΩΣ ΣΗΜΕ
+  dewey: 938.498 ΑΝΤ
   entry_numbers:
   - '20984'
   editor: ΤΟ ΒΗΜΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 263
   topics:
   - ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
@@ -788162,28 +788215,28 @@
   has_dvd: false
   offprint: false
   ean: '9789604367450'
   original_entry:
     0: 15971
     1: ΑΝΤΩΝΙΑΔΗΣ,ΑΝΤΩΝΗΣ
     2: ΤΑ 100 ΓΕΓΟΝΟΤΑ ΠΟΥ ΣΗΜΑΔΕΨΑΝ ΤΗΝ ΕΛΛΑΔΑ ΑΠ ΤΟ 1821 ΕΩΣ ΣΗΜΕ
+    4: 938.498ΑΝΤ
     5: '20984'
     8: ΤΟ ΒΗΜΑ ΑΛΤΕΡ ΕΓΚΟ
     9: ΑΘΗΝΑ
     10: '2021'
     11: '263'
     12: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
     13: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
     14: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
     16: ΑΝΤΩΝΙΑΔΗΣ
     17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
     18: '9789604367'
     19: '450'
     3: null
-    4: null
     6: null
     7: null
     15: null
     20: null
     21: null
     22: null
     23: null
@@ -788194,14 +788247,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 15972
   authors: []
   title: 1922 ΠΩΣ ΧΑΣΑΜΕ ΤΗ ΣΜΥΡΝΗ
   subtitle: ΒΑΣΙΣΜΕΝΟ ΣΕ ΑΓΝΩΣΤΑ ΚΑΙ ΑΠΟΚΑΛΥΠΤΙΚΑ ΕΓΓΡΑΦΑ
+  dewey: 938.498 ΧΣ
   entry_numbers:
   - '20987'
   editor: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
   edition_year: 2018
   pages: 267
   topics:
   - ΣΜΥΡΝΗ
@@ -788213,27 +788267,27 @@
   offprint: false
   ean: '9789605039592'
   original_entry:
     0: 15972
     1: Χ.Σ.
     2: 1922 ΠΩΣ ΧΑΣΑΜΕ ΤΗ ΣΜΥΡΝΗ
     3: ΒΑΣΙΣΜΕΝΟ ΣΕ ΑΓΝΩΣΤΑ ΚΑΙ ΑΠΟΚΑΛΥΠΤΙΚΑ ΕΓΓΡΑΦΑ
+    4: 938.498Χ.Σ
     5: '20987'
     8: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ
     9: ΑΘΗΝΑ
     10: '2018'
     11: '267'
     12: ΣΜΥΡΝΗ
     13: ΣΜΥΡΝΗ
     14: ΣΜΥΡΝΗ
     16: ΜΑΛΟΥΧΟΣ,Γ.
     17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
     18: '9789605039'
     19: '592'
-    4: null
     6: null
     7: null
     15: null
     20: null
     21: null
     22: null
     23: null
@@ -788292,14 +788346,15 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15974
   authors: []
   title: 70 ΦΙΛΟΣΟΦΟΙ ΠΟΥ ΑΛΛΑΞΑΝ ΤΟΝ ΚΟΣΜΟ
+  dewey: 920 ΧΣ
   entry_numbers:
   - '20986'
   editor: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
   edition_year: 2017
   pages: 127
   topics:
   - ΦΙΛΟΣΟΦΟΙ
@@ -788309,27 +788364,27 @@
   has_dvd: false
   offprint: false
   ean: '9789605038533'
   original_entry:
     0: 15974
     1: Χ.Σ.
     2: 70 ΦΙΛΟΣΟΦΟΙ ΠΟΥ ΑΛΛΑΞΑΝ ΤΟΝ ΚΟΣΜΟ
+    4: 920Χ.Σ
     5: '20986'
     8: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ
     9: ΑΘΗΝΑ
     10: '2017'
     11: '127'
     12: ΦΙΛΟΣΟΦΟΙ
     13: ΦΙΛΟΣΟΦΟΙ
     14: ΦΙΛΟΣΟΦΟΙ
     17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
     18: '9789605038'
     19: '533'
     3: null
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -788928,30 +788983,30 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15987
   authors:
   - ΤΣΟΥΤΣΙΝΟΣ,ΓΙΑΝΝΗΣ
-  title: ΑΡΤΙΝΑ ΙΣΤΟΡΙΜΑΤΑ
+  title: ΑΡΤΙΝΑ ΙΣΤΟΡΗΜΑΤΑ
   dewey: 938.939 ΤΣΟ
   entry_numbers:
   - '21196'
   editor: ΠΕΡΙΟΔΙΚΟ ΣΚΟΥΦΑΣ // ΑΡΤΑ
   edition_year: 1975
   pages: 36
   topics:
   - ΑΡΤΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 15987
     1: ΤΣΟΥΤΣΙΝΟΣ,ΓΙΑΝΝΗΣ
-    2: ΑΡΤΙΝΑ ΙΣΤΟΡΙΜΑΤΑ
+    2: ΑΡΤΙΝΑ ΙΣΤΟΡΗΜΑΤΑ
     4: 938.939ΤΣΟ
     5: '21196'
     8: ΠΕΡΙΟΔΙΚΟ ΣΚΟΥΦΑΣ
     9: ΑΡΤΑ
     10: '1975'
     11: '36'
     12: ΑΡΤΑ
@@ -788977,15 +789032,15 @@
     29: null
     30: null
 - dbase_number: 15988
   authors:
   - NICOL,DONALD
   title: ΗΠΕΙΡΩΤΙΚΑ ΧΡΟΝΙΚΑ
   subtitle: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
-  dewey: 938.939 DON
+  dewey: 938.384 NIC
   entry_numbers:
   - '21197'
   editor: ΑΠΕΙΡΩΤΑΝ // ΙΩΑΝΝΙΝΑ
   edition_year: 1992
   pages: 59
   topics:
   - ΗΠΕΙΡΟΣ
@@ -788993,15 +789048,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 15988
     1: NICOL,DONALD
     2: ΗΠΕΙΡΩΤΙΚΑ ΧΡΟΝΙΚΑ
     3: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
-    4: 938.939DON
+    4: 938.384NIC
     5: '21197'
     8: ΑΠΕΙΡΩΤΑΝ
     9: ΙΩΑΝΝΙΝΑ
     10: '1992'
     11: '59'
     12: ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ
@@ -789069,33 +789124,33 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15990
   authors:
-  - NICOL, M. DONALD
+  - NICOL,DONALD
   title: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ 1267-1479
-  dewey: 938.939 DON
+  dewey: 938.375 NIC
   entry_numbers:
   - '21199'
   editor: ΕΛ.ΕΥΡΩΕΚΔΟΤΙΚΗ ΕΠΕ // ΑΘΗΝΑ
   edition_year: 1991
   pages: 327
   topics:
   - ΗΠΕΙΡΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: '9602410191'
   original_entry:
     0: 15990
-    1: NICOL, M. DONALD
+    1: NICOL,DONALD
     2: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ 1267-1479
-    4: 938.939DON
+    4: 938.375NIC
     5: '21199'
     8: ΕΛ.ΕΥΡΩΕΚΔΟΤΙΚΗ ΕΠΕ
     9: ΑΘΗΝΑ
     10: '1991'
     11: '327'
     12: ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ
@@ -790230,36 +790285,36 @@
 - dbase_number: 16014
   authors: []
   title: ΜΝΗΜΗ ΣΟΥΛΙΟΥ
   dewey: 938.526 ΧΣ
   entry_numbers:
   - '21252'
   editor: ΟΙ ΦΙΛΟΙ ΤΟΥ ΣΟΥΛΙΟΥ // ΑΘΗΝΑ
-  edition_year: 2007
+  edition_year: 2016
   pages: 343
   topics:
   - ΣΟΥΛΙ
-  volume: ΤΟΜΟΣ ΠΡΩΤΟΣ
+  volume: ΤΟΜΟΙ 4
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 16014
     1: Χ.Σ.
     2: ΜΝΗΜΗ ΣΟΥΛΙΟΥ
     4: 938.526Χ.Σ
     5: '21252'
     8: ΟΙ ΦΙΛΟΙ ΤΟΥ ΣΟΥΛΙΟΥ
     9: ΑΘΗΝΑ
-    10: '2007'
+    10: '2016'
     11: '343'
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
-    17: ΤΟΜΟΣ ΠΡΩΤΟΣ
+    17: ΤΟΜΟΙ 4
     22: ΣΟΥΛΙ
     23: ΣΟΥΛΙ
     24: ΣΟΥΛΙ
     3: null
     6: null
     7: null
     15: null
@@ -790272,48 +790327,49 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16015
   authors: []
-  title: ΜΝΗΜΗ ΣΟΥΛΙΟΥ ΔΕΥΤΕΡΟΣ ΤΟΜΟΣ
+  title: ΜΝΗΜΗ ΣΟΥΛΙΟΥ
   dewey: 938.526 ΧΣ
   entry_numbers:
   - '21253'
   editor: ΟΙ ΦΙΛΟΙ ΤΟΥ ΣΟΥΛΙΟΥ // ΑΘΗΝΑ
   edition_year: 1973
   pages: 365
   topics:
   - ΣΟΥΛΙ
+  volume: ΤΟΜΟΙ 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 16015
     1: Χ.Σ.
-    2: ΜΝΗΜΗ ΣΟΥΛΙΟΥ ΔΕΥΤΕΡΟΣ ΤΟΜΟΣ
+    2: ΜΝΗΜΗ ΣΟΥΛΙΟΥ
     4: 938.526Χ.Σ
     5: '21253'
     8: ΟΙ ΦΙΛΟΙ ΤΟΥ ΣΟΥΛΙΟΥ
     9: ΑΘΗΝΑ
     10: '1973'
     11: '365'
     12: ΙΣΤΟΡΙΑ
     13: ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
+    17: ΤΟΜΟΙ 2
     22: ΣΟΥΛΙ
     23: ΣΟΥΛΙ
     24: ΣΟΥΛΙ
     3: null
     6: null
     7: null
     15: null
     16: null
-    17: null
     18: null
     19: null
     20: null
     21: null
     25: null
     26: null
     27: null
@@ -790374,15 +790430,15 @@
     27: null
     28: null
     29: null
 - dbase_number: 16017
   authors:
   - HELLER,ROBERT
   title: ΣΥΜΒΟΥΛΟΣ ΜΑΝΑΤΖΕΡ
-  subtitle: ΕΠΙΚΟΙΝΩΝΙΣΤΕ ΑΠΟΤΕΛΕΣΜΑΤΙΚΑ
+  subtitle: ΕΠΙΚΟΙΝΩΝΗΣΤΕ ΑΠΟΤΕΛΕΣΜΑΤΙΚΑ
   dewey: 658.4 HEL
   entry_numbers:
   - '21295'
   translators:
   - ΠΕΡΑΝΤΑΚΟΥ,ΜΑΙΡΗ
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2001
@@ -790396,15 +790452,15 @@
   has_dvd: false
   offprint: false
   isbn: '9603936782'
   original_entry:
     0: 16017
     1: HELLER,ROBERT
     2: ΣΥΜΒΟΥΛΟΣ ΜΑΝΑΤΖΕΡ
-    3: ΕΠΙΚΟΙΝΩΝΙΣΤΕ ΑΠΟΤΕΛΕΣΜΑΤΙΚΑ
+    3: ΕΠΙΚΟΙΝΩΝΗΣΤΕ ΑΠΟΤΕΛΕΣΜΑΤΙΚΑ
     4: 658.4HEL
     5: '21295'
     6: ΠΕΡΑΝΤΑΚΟΥ,ΜΑΙΡΗ
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '2001'
     11: '72'
@@ -790691,15 +790747,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16023
   authors: []
-  title: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  title: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   subtitle: ΑΛΕΞΑΝΔΡΕΙΑ
   dewey: 909.048 ΧΣ
   entry_numbers:
   - '21232'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 128
   topics:
@@ -790709,15 +790765,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604751761'
   original_entry:
     0: 16023
     1: Χ.Σ.
-    2: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+    2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
     3: ΑΛΕΞΑΝΔΡΕΙΑ
     4: 909.048Χ.Σ
     5: '21232'
     8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
     11: '128'
     12: ΕΛΛΗΝΙΣΜΟΣ
@@ -790740,15 +790796,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16024
   authors: []
-  title: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  title: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   subtitle: ΟΔΗΣΣΟΣ
   dewey: 909.048 ΧΣ
   entry_numbers:
   - '21233'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 96
   topics:
@@ -790758,15 +790814,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604751778'
   original_entry:
     0: 16024
     1: Χ.Σ.
-    2: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+    2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
     3: ΟΔΗΣΣΟΣ
     4: 909.048Χ.Σ
     5: '21233'
     8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
     11: '96'
     12: ΕΛΛΗΝΙΣΜΟΣ
@@ -790789,15 +790845,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16025
   authors: []
-  title: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  title: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   subtitle: ΣΜΥΡΝΗ
   dewey: 909.048 ΧΣ
   entry_numbers:
   - '21234'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 101
   topics:
@@ -790807,15 +790863,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604751785'
   original_entry:
     0: 16025
     1: Χ.Σ.
-    2: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+    2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
     3: ΣΜΥΡΝΗ
     4: 909.048Χ.Σ
     5: '21234'
     8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
     11: '101'
     12: ΕΛΛΗΝΙΣΜΟΣ
@@ -790838,15 +790894,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16026
   authors: []
-  title: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  title: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   subtitle: ΜΙΛΗΤΟΣ
   dewey: 909.048 ΧΣ
   entry_numbers:
   - '21235'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 96
   topics:
@@ -790856,15 +790912,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604751792'
   original_entry:
     0: 16026
     1: Χ.Σ.
-    2: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+    2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
     3: ΜΙΛΗΤΟΣ
     4: 909.048Χ.Σ
     5: '21235'
     8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
     11: '96'
     12: ΕΛΛΗΝΙΣΜΟΣ
@@ -790985,15 +791041,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16029
   authors: []
-  title: ΚΟΙΤΙΔΕΣ ΠΟΛΙΤΙΣΜΟΥ
+  title: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   subtitle: ΠΕΡΓΑΜΟΣ
   dewey: 909.048 ΧΣ
   entry_numbers:
   - '21238'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 88
   topics:
@@ -791003,15 +791059,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604751822'
   original_entry:
     0: 16029
     1: Χ.Σ.
-    2: ΚΟΙΤΙΔΕΣ ΠΟΛΙΤΙΣΜΟΥ
+    2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
     3: ΠΕΡΓΑΜΟΣ
     4: 909.048Χ.Σ
     5: '21238'
     8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
     11: '88'
     12: ΕΛΛΗΝΙΣΜΟΣ
@@ -791043,15 +791099,14 @@
   dewey: 909.048 ΧΣ
   entry_numbers:
   - '21239'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 102
   topics:
   - ΕΛΛΗΝΙΣΜΟΣ
-  - ΕΛΛΗΝΙΣΜΟ
   donors:
   - ΠΝΕΥΜΑΤΙΚΟΣ,Ι.
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604751839'
   original_entry:
@@ -791061,15 +791116,15 @@
     3: ΒΕΝΕΤΙΑ
     4: 909.048Χ.Σ
     5: '21239'
     8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
     11: '102'
     12: ΕΛΛΗΝΙΣΜΟΣ
-    13: ΕΛΛΗΝΙΣΜΟ
+    13: ΕΛΛΗΝΙΣΜΟΣ
     14: ΕΛΛΗΝΙΣΜΟΣ
     18: '9789604751'
     19: '839'
     30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
     6: null
     7: null
     10: null
@@ -791281,15 +791336,15 @@
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16035
   authors: []
   title: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
-  subtitle: ΑΛΛΟΧΩΣΤΟΣ
+  subtitle: ΑΜΜΟΧΩΣΤΟΣ
   dewey: 909.048 ΧΣ
   entry_numbers:
   - '21244'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 96
   topics:
   - ΕΛΛΗΝΙΣΜΟΣ
@@ -791299,15 +791354,15 @@
   has_dvd: false
   offprint: false
   ean: '9789604751921'
   original_entry:
     0: 16035
     1: Χ.Σ.
     2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
-    3: ΑΛΛΟΧΩΣΤΟΣ
+    3: ΑΜΜΟΧΩΣΤΟΣ
     4: 909.048Χ.Σ
     5: '21244'
     8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
     11: '96'
     12: ΕΛΛΗΝΙΣΜΟΣ
     13: ΕΛΛΗΝΙΣΜΟΣ
@@ -791476,15 +791531,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16039
   authors: []
-  title: ΚΟΙΤΟΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  title: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   subtitle: ΚΑΜΠΑΝΙΑ ΚΑΙ ΑΠΟΥΛΙΑ
   dewey: 909.048 ΧΣ
   entry_numbers:
   - '21248'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 88
   topics:
@@ -791494,15 +791549,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789604751938'
   original_entry:
     0: 16039
     1: Χ.Σ.
-    2: ΚΟΙΤΟΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+    2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
     3: ΚΑΜΠΑΝΙΑ ΚΑΙ ΑΠΟΥΛΙΑ
     4: 909.048Χ.Σ
     5: '21248'
     8: ΚΑΘΗΜΕΡΙΝΗ
     9: ΑΘΗΝΑ
     11: '88'
     12: ΕΛΛΗΝΙΣΜΟΣ
@@ -793268,15 +793323,15 @@
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16075
   authors: []
   title: ΟΔΗΓΟΙ ΤΟΥ ΚΟΣΜΟΥ
-  subtitle: ΑΙΓΗΠΤΟΣ
+  subtitle: ΑΙΓΥΠΤΟΣ
   dewey: 910.202 ΧΣ
   entry_numbers:
   - '21286'
   editor: GALLIMARD // ΑΘΗΝΑ
   edition_year: 2000
   pages: 479
   topics:
@@ -793287,15 +793342,15 @@
   has_dvd: false
   offprint: false
   isbn: '9603682136'
   original_entry:
     0: 16075
     1: Χ.Σ.
     2: ΟΔΗΓΟΙ ΤΟΥ ΚΟΣΜΟΥ
-    3: ΑΙΓΗΠΤΟΣ
+    3: ΑΙΓΥΠΤΟΣ
     4: 910.202Χ.Σ
     5: '21286'
     8: GALLIMARD
     9: ΑΘΗΝΑ
     10: '2000'
     11: '479'
     12: ΤΑΞΙΔΙΩΤΙΚΟΙ ΟΔΗΓΟΙ
@@ -803150,39 +803205,39 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16276
   authors:
-  - MARK TWAIN
+  - TWAIN,MARK
   title: ΤΟΜ ΣΟΓΕΡ
   dewey: 808.899 TWA
   entry_numbers:
   - '21741'
   editor: ΠΑΠΑΔΟΠΟΥΛΟΣ // None
   pages: 156
   topics:
-  - ΤΟΜ ΣΟΓΕΡ
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   donors:
   - ΚΟΛΙΟΥ,ΜΑΡΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 16276
-    1: MARK TWAIN
+    1: TWAIN,MARK
     2: ΤΟΜ ΣΟΓΕΡ
     4: 808.899TWA
     5: '21741'
     8: ΠΑΠΑΔΟΠΟΥΛΟΣ
     11: '156'
-    12: ΤΟΜ ΣΟΓΕΡ
-    13: ΤΟΜ ΣΟΓΕΡ
-    14: ΤΟΜ ΣΟΓΕΡ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΜΑΡΙΑΣ ΚΟΛΙΟΥ
     3: null
     6: null
     7: null
     9: null
     10: null
     15: null
@@ -843741,15 +843796,15 @@
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2022'
     11: 438Σ
     12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
-    17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΑΣ
+    17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180143'
     19: '003'
     4: null
     5: null
     7: null
     15: null
     16: null
@@ -844027,15 +844082,16 @@
     29: null
 - dbase_number: 17129
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   subtitle: ΤΟ ΠΟΤΗΡΙ ΞΕΧΕΙΛΙΣΕ
   dewey: 808.899 ΚΙΝ
-  entry_numbers: []
+  entry_numbers:
+  - '22580'
   translators:
   - ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ,ΧΑΡΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 225
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844048,27 +844104,27 @@
   ean: '9789604536665'
   original_entry:
     0: 17129
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
     3: ΤΟ ΠΟΤΗΡΙ ΞΕΧΕΙΛΙΣΕ
     4: 808.899ΚΙΝ
+    5: '22580'
     6: ΧΑΡΑ ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2021'
     11: 225Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9789604536'
     19: '665'
     30: ΤΟΜΟΣ 3
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844080,15 +844136,16 @@
     29: null
 - dbase_number: 17130
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   subtitle: Ο ΡΟΝΤΡΙΚ ΔΕΝ ΠΑΙΖΕΤΑΙ
   dewey: 808.899 ΚΙΝ
-  entry_numbers: []
+  entry_numbers:
+  - '22579'
   translators:
   - ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ,ΧΑΡΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2022
   pages: 225
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844101,27 +844158,27 @@
   ean: '9789604535248'
   original_entry:
     0: 17130
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
     3: Ο ΡΟΝΤΡΙΚ ΔΕΝ ΠΑΙΖΕΤΑΙ
     4: 808.899ΚΙΝ
+    5: '22579'
     6: ΧΑΡΑ ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2022'
     11: 225Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9789604535'
     19: '248'
     30: ΤΟΜΟΣ 2
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844133,15 +844190,16 @@
     29: null
 - dbase_number: 17131
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   subtitle: ΣΚΥΛΙΣΙΑ ΖΩΗ
   dewey: 808.899 ΚΙΝ
-  entry_numbers: []
+  entry_numbers:
+  - '22581'
   translators:
   - ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ,ΧΑΡΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2022
   pages: 224
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844154,27 +844212,27 @@
   ean: '9789604537716'
   original_entry:
     0: 17131
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
     3: ΣΚΥΛΙΣΙΑ ΖΩΗ
     4: 808.899ΚΙΝ
+    5: '22581'
     6: ΧΑΡΑ ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2022'
     11: 224Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9789604537'
     19: '716'
     30: ΤΟΜΟΣ 4
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844186,15 +844244,16 @@
     29: null
 - dbase_number: 17132
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   subtitle: ΘΑ ΠΑΕΙ ΜΑΚΡΙΑ Η ΒΑΛΙΤΣΑ
   dewey: 808.899 ΚΙΝ
-  entry_numbers: []
+  entry_numbers:
+  - '22584'
   translators:
   - ΓΑΒΡΙΗΛΙΔΟΥ,ΠΕΤΡΟΥΛΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 225
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844207,27 +844266,27 @@
   ean: '9786180108262'
   original_entry:
     0: 17132
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
     3: ΘΑ ΠΑΕΙ ΜΑΚΡΙΑ Η ΒΑΛΙΤΣΑ
     4: 808.899ΚΙΝ
+    5: '22584'
     6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2021'
     11: 225Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180108'
     19: '262'
     30: ΤΟΜΟΣ 9
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844239,15 +844298,16 @@
     29: null
 - dbase_number: 17133
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   subtitle: Η ΑΠΟΔΡΑΣΗ
   dewey: 808.899 ΚΙΝ
-  entry_numbers: []
+  entry_numbers:
+  - '22585'
   translators:
   - ΓΑΒΡΙΗΛΙΔΟΥ,ΠΕΤΡΟΥΛΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2022
   pages: 225
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844260,27 +844320,27 @@
   ean: '9786180122381'
   original_entry:
     0: 17133
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
     3: Η ΑΠΟΔΡΑΣΗ
     4: 808.899ΚΙΝ
+    5: '22585'
     6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2022'
     11: 225Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180122'
     19: '381'
     30: ΤΟΜΟΣ 12
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844292,15 +844352,16 @@
     29: null
 - dbase_number: 17134
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   subtitle: Η ΣΚΛΗΡΗ ΑΛΗΘΕΙΑ
   dewey: 808.899 ΚΙΝ
-  entry_numbers: []
+  entry_numbers:
+  - '22582'
   translators:
   - ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ,ΧΑΡΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2022
   pages: 225
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844313,27 +844374,27 @@
   ean: '9789604960071'
   original_entry:
     0: 17134
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
     3: Η ΣΚΛΗΡΗ ΑΛΗΘΕΙΑ
     4: 808.899ΚΙΝ
+    5: '22582'
     6: ΧΑΡΑ ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2022'
     11: 225Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9789604960'
     19: '071'
     30: ΤΟΜΟΣ 5
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844345,15 +844406,16 @@
     29: null
 - dbase_number: 17135
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   subtitle: ΣΤΟΥΣ ΔΥΟ ΤΡΙΤΟΣ ΔΕ ΧΩΡΕΙ
   dewey: 808.899 ΚΙΝ
-  entry_numbers: []
+  entry_numbers:
+  - '22583'
   translators:
   - ΓΑΒΡΙΗΛΙΔΟΥ,ΠΕΤΡΟΥΛΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2022
   pages: 226
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844366,27 +844428,27 @@
   ean: '9786180100136'
   original_entry:
     0: 17135
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
     3: ΣΤΟΥΣ ΔΥΟ ΤΡΙΤΟΣ ΔΕ ΧΩΡΕΙ
     4: 808.899ΚΙΝ
+    5: '22583'
     6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2022'
     11: 226Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180100'
     19: '136'
     30: ΤΟΜΟΣ 7
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844394,19 +844456,20 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 17136
   authors:
-  - ΛΑΖΑΡ,ΡΑΛΦ-ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ
+  - ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ-ΛΑΖΑΡ,ΡΑΛΦ
   title: Ο ΝΤΕΤΕΚΤΙΒ ΡΟΝΙ
   subtitle: ΒΑΖΕΙ ΤΑ ΓΕΛΙΑ ΜΠΡΟΣΤΑ ΣΤΟΝ ΚΙΝΔΥΝΟ
-  dewey: 808.899 ΛΑΖ
-  entry_numbers: []
+  dewey: 808.899 ΚΛΟ
+  entry_numbers:
+  - '22604'
   translators:
   - ΚΟΛΥΔΑ,ΕΥΓΕΝΙΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2019
   pages: 350
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844415,31 +844478,31 @@
   volume: ΤΟΜΟΣ 2
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9786180129342'
   original_entry:
     0: 17136
-    1: ΛΑΖΑΡ,ΡΑΛΦ-ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ
+    1: ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ-ΛΑΖΑΡ,ΡΑΛΦ
     2: Ο ΝΤΕΤΕΚΤΙΒ ΡΟΝΙ
     3: ΒΑΖΕΙ ΤΑ ΓΕΛΙΑ ΜΠΡΟΣΤΑ ΣΤΟΝ ΚΙΝΔΥΝΟ
-    4: 808.899ΛΑΖ
+    4: 808.899ΚΛΟ
+    5: '22604'
     6: ΕΥΓΕΝΙΑ ΚΟΛΥΔΑ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2019'
     11: 350Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180129'
     19: '342'
     30: ΤΟΜΟΣ 2
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844447,18 +844510,20 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 17137
   authors:
-  - ΛΑΖΑΡ,ΡΑΛΦ-ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ
+  - ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ-ΛΑΖΑΡ,ΡΑΛΦ
   title: Ο ΝΤΕΤΕΚΤΙΒ ΡΟΝΙ
   subtitle: ΠΑΤΑΕΙ ΣΤΟ ΚΕΦΑΛΙ ΤΟΥΣ ΚΑΚΟΥΣ
-  entry_numbers: []
+  dewey: 808.899 ΚΛΟ
+  entry_numbers:
+  - '22605'
   translators:
   - ΚΟΛΥΔΑ,ΕΥΓΕΝΙΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2020
   pages: 282
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844467,31 +844532,31 @@
   volume: ΤΟΜΟΣ 4
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9786180131154'
   original_entry:
     0: 17137
-    1: ΛΑΖΑΡ,ΡΑΛΦ-ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ
+    1: ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ-ΛΑΖΑΡ,ΡΑΛΦ
     2: Ο ΝΤΕΤΕΚΤΙΒ ΡΟΝΙ
     3: ΠΑΤΑΕΙ ΣΤΟ ΚΕΦΑΛΙ ΤΟΥΣ ΚΑΚΟΥΣ
+    4: 808.899ΚΛΟ
+    5: '22605'
     6: ΕΥΓΕΝΙΑ ΚΟΛΥΔΑ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2020'
     11: 282Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180131'
     19: '154'
     30: ΤΟΜΟΣ 4
-    4: null
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -844660,15 +844725,16 @@
     28: null
     29: null
 - dbase_number: 17141
   authors:
   - ΜΟΥΡΙΚΗ,ΚΑΤΕΡΙΝΑ
   title: ΠΑΥΛΟΣ Ο ΑΠΟΣΤΟΛΟΣ ΤΩΝ ΕΘΝΩΝ
   dewey: 808.899 ΜΟΥ
-  entry_numbers: []
+  entry_numbers:
+  - '22594'
   editor: ΟΥΡΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 2020
   pages: 50
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   donors:
   - ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
@@ -844677,26 +844743,26 @@
   offprint: false
   ean: '9789605590413'
   original_entry:
     0: 17141
     1: ΜΟΥΡΙΚΗ,ΚΑΤΕΡΙΝΑ
     2: ΠΑΥΛΟΣ Ο ΑΠΟΣΤΟΛΟΣ ΤΩΝ ΕΘΝΩΝ
     4: 808.899ΜΟΥ
+    5: '22594'
     8: ΟΥΡΑΝΟΣ
     9: ΑΘΗΝΑ
     10: '2020'
     11: 50Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9789605590'
     19: '413'
     3: null
-    5: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -844806,15 +844872,16 @@
     29: null
     30: null
 - dbase_number: 17144
   authors:
   - ΓΕΩΡΓΟΣΤΑΘΗ,ΕΛΕΝΗ
   title: ΧΑΘΗΚΕ Η ΜΠΑΛΑ
   dewey: 808.899 ΓΕΩ
-  entry_numbers: []
+  entry_numbers:
+  - '22597'
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2017
   pages: 93
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   donors:
   - ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
@@ -844822,26 +844889,26 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 17144
     1: ΓΕΩΡΓΟΣΤΑΘΗ,ΕΛΕΝΗ
     2: ΧΑΘΗΚΕ Η ΜΠΑΛΑ
     4: 808.899ΓΕΩ
+    5: '22597'
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2017'
     11: 93Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180118'
     19: '75'
     3: null
-    5: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -844854,15 +844921,16 @@
     29: null
     30: null
 - dbase_number: 17145
   authors:
   - ΔΗΜΟΠΟΥΛΟΣ,ΧΡΗΣΤΟΣ
   title: ΤΟ ΠΡΩΤΟ ΣΥΝΤΑΓΜΑ ΤΗΣ ΕΛΛΑΔΑΣ ΓΙΑ ΠΑΙΔΙΑ
   dewey: 808.899 ΔΗΜ
-  entry_numbers: []
+  entry_numbers:
+  - '22593'
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2020
   pages: 39
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   donors:
   - ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
@@ -844871,26 +844939,26 @@
   offprint: false
   ean: '9786180136067'
   original_entry:
     0: 17145
     1: ΔΗΜΟΠΟΥΛΟΣ,ΧΡΗΣΤΟΣ
     2: ΤΟ ΠΡΩΤΟ ΣΥΝΤΑΓΜΑ ΤΗΣ ΕΛΛΑΔΑΣ ΓΙΑ ΠΑΙΔΙΑ
     4: 808.899ΔΗΜ
+    5: '22593'
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2020'
     11: 39Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180136'
     19: '067'
     3: null
-    5: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -844954,15 +845022,16 @@
     29: null
     30: null
 - dbase_number: 17147
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΑΠΙΣΤΕΥΤΑ ΚΑΛΟΥ ΠΑΙΔΙΟΥ
   dewey: 808.899 ΚΙΝ
-  entry_numbers: []
+  entry_numbers:
+  - '22599'
   translators:
   - ΓΑΒΡΙΗΛΙΔΟΥ,ΠΕΤΡΟΥΛΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2019
   pages: 226
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -844973,27 +845042,27 @@
   offprint: false
   ean: '9786180131093'
   original_entry:
     0: 17147
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΑΠΙΣΤΕΥΤΑ ΚΑΛΟΥ ΠΑΙΔΙΟΥ
     4: 808.899ΚΙΝ
+    5: '22599'
     6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2019'
     11: 226Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180131'
     19: 093
     3: null
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -845004,16 +845073,17 @@
     28: null
     29: null
     30: null
 - dbase_number: 17148
   authors:
   - ΚΙΝΙ,ΤΖΕΦ
   title: ΟΙ ΑΠΙΣΤΕΥΤΑ ΚΑΛΕΣ ΙΣΤΟΡΙΕΣ ΤΡΟΜΟΥ
-  dewey: 808.899 ΝΙΚ
-  entry_numbers: []
+  dewey: 808.899 ΚΙΝ
+  entry_numbers:
+  - '22600'
   translators:
   - ΓΑΒΡΙΗΛΙΔΟΥ,ΠΕΤΡΟΥΛΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 226
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -845023,28 +845093,28 @@
   has_dvd: false
   offprint: false
   ean: '9786180140224'
   original_entry:
     0: 17148
     1: ΚΙΝΙ,ΤΖΕΦ
     2: ΟΙ ΑΠΙΣΤΕΥΤΑ ΚΑΛΕΣ ΙΣΤΟΡΙΕΣ ΤΡΟΜΟΥ
-    4: 808.899ΝΙΚ
+    4: 808.899ΚΙΝ
+    5: '22600'
     6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2021'
     11: 226Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180140'
     19: '224'
     3: null
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -845210,17 +845280,18 @@
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 17152
   authors:
   - ΠΙΛΚΙ,ΝΤΕΙΒ
-  title: Ο ΚΑΠΕΤΑ ΒΡΑΚΑΣ ΚΑΙ Η ΜΕΓΑΛΗ ΜΑΝΙΑΣΜΕΝΗ ΜΑΧΗ
+  title: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΜΕΓΑΛΗ ΜΑΝΙΑΣΜΕΝΗ ΜΑΧΗ
   dewey: 808.899 ΠΙΛ
-  entry_numbers: []
+  entry_numbers:
+  - '22611'
   translators:
   - ΓΡΗΓΟΡΙΟΥ,ΣΟΦΙΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 177
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -845230,30 +845301,30 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '978618012435'
   original_entry:
     0: 17152
     1: ΠΙΛΚΙ,ΝΤΕΙΒ
-    2: Ο ΚΑΠΕΤΑ ΒΡΑΚΑΣ ΚΑΙ Η ΜΕΓΑΛΗ ΜΑΝΙΑΣΜΕΝΗ ΜΑΧΗ
+    2: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΜΕΓΑΛΗ ΜΑΝΙΑΣΜΕΝΗ ΜΑΧΗ
     4: 808.899ΠΙΛ
+    5: '22611'
     6: ΣΟΦΙΑ ΓΡΗΓΟΡΙΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2021'
     11: 177Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180124'
     19: '35'
     30: ΤΟΜΟΣ 6
     3: null
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -845264,15 +845335,16 @@
     28: null
     29: null
 - dbase_number: 17153
   authors:
   - ΠΙΛΚΙ,ΝΤΕΙΒ
   title: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΠΡΟΣΜΕΝΗ ΕΠΙΣΤΡΟΦΗ
   dewey: 808.899 ΠΙΛ
-  entry_numbers: []
+  entry_numbers:
+  - '22612'
   translators:
   - ΓΡΗΓΟΡΙΟΥ,ΣΟΦΙΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2019
   pages: 298
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -845283,28 +845355,28 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 17153
     1: ΠΙΛΚΙ,ΝΤΕΙΒ
     2: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΠΡΟΣΜΕΝΗ ΕΠΙΣΤΡΟΦΗ
     4: 808.899ΠΙΛ
+    5: '22612'
     6: ΣΟΦΙΑ ΓΡΗΓΟΡΙΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2019'
     11: 298Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180130'
     19: '22'
     30: ΤΟΜΟΣ 9
     3: null
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -845315,15 +845387,16 @@
     28: null
     29: null
 - dbase_number: 17154
   authors:
   - ΠΙΛΚΙ,ΝΤΕΙΒ
   title: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΝΕΚΔΙΗΓΗΤΗ ΕΚΔΙΚΗΣΗ
   dewey: 808.899 ΠΙΛ
-  entry_numbers: []
+  entry_numbers:
+  - '22613'
   translators:
   - ΓΡΗΓΟΡΙΟΥ,ΣΟΦΙΑ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2020
   pages: 224
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -845335,28 +845408,28 @@
   offprint: false
   ean: '9786180134551'
   original_entry:
     0: 17154
     1: ΠΙΛΚΙ,ΝΤΕΙΒ
     2: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΝΕΚΔΙΗΓΗΤΗ ΕΚΔΙΚΗΣΗ
     4: 808.899ΠΙΛ
+    5: '22613'
     6: ΣΟΦΙΑ ΓΡΗΓΟΡΙΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2020'
     11: 224Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180134'
     19: '551'
     30: ΤΟΜΟΣ 10
     3: null
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -845367,15 +845440,16 @@
     28: null
     29: null
 - dbase_number: 17155
   authors:
   - ΠΙΛΚΙ,ΝΤΕΙΒ
   title: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΒΑΣΤΑΧΤΗ ΒΑΡΒΑΡΟΤΗΤΑ
   dewey: 808.899 ΠΙΛ
-  entry_numbers: []
+  entry_numbers:
+  - '22610'
   translators:
   - ΓΡΑΜΜΕΝΟΥ,ΜΑΙΡΗ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2022
   pages: 170
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -845387,28 +845461,28 @@
   offprint: false
   ean: '9786180118513'
   original_entry:
     0: 17155
     1: ΠΙΛΚΙ,ΝΤΕΙΒ
     2: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΒΑΣΤΑΧΤΗ ΒΑΡΒΑΡΟΤΗΤΑ
     4: 808.899ΠΙΛ
+    5: '22610'
     6: ΜΑΙΡΗ ΓΡΑΜΜΕΝΟΥ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2022'
     11: 170Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
     18: '9786180118'
     19: '513'
     30: ΤΟΜΟΣ 5
     3: null
-    5: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -850201,36 +850275,37 @@
   title: ΣΠΑΣΤΕ ΤΑ ΔΕΣΜΑ ΤΗΣ ΧΑΜΗΛΗΣ ΑΥΤΟΕΚΤΙΜΗΣΗΣ
   dewey: 306.7 SOR
   entry_numbers:
   - '22522'
   editor: ΦΥΤΡΑΚΗΣ // ΑΘΗΝΑ
   edition_year: 1998
   pages: 418
-  topics: []
+  topics:
+  - ΑΥΤΟΕΚΤΙΜΗΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: '9605354896'
   original_entry:
     0: 17255
     1: SORENSEN,MERILYN
     2: ΣΠΑΣΤΕ ΤΑ ΔΕΣΜΑ ΤΗΣ ΧΑΜΗΛΗΣ ΑΥΤΟΕΚΤΙΜΗΣΗΣ
     4: 306.7SOR
     5: '22522'
     8: ΦΥΤΡΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '1998'
     11: '418'
+    12: ΑΥΤΟΕΚΤΙΜΗΣΗ
+    13: ΑΥΤΟΕΚΤΙΜΗΣΗ
+    14: ΑΥΤΟΕΚΤΙΜΗΣΗ
     18: '9605354896'
     3: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     19: null
     20: null
     21: null
     22: null
@@ -850248,34 +850323,35 @@
   title: ΤΑ ΠΡΩΤΑ 6 ΧΡΟΝΙΑ ΤΗΣ ΖΩΗΣ ΤΟΥ ΠΑΙΔΙΟΥ
   dewey: 305.231 ΠΑΠ
   entry_numbers:
   - '22548'
   editor: NESTLE // ΑΘΗΝΑ
   edition_year: 1996
   pages: 76
-  topics: []
+  topics:
+  - ΠΡΟΣΧΟΛΙΚΗ ΗΛΙΚΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 17256
     1: ΠΑΠΑΔΑΤΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
     2: ΤΑ ΠΡΩΤΑ 6 ΧΡΟΝΙΑ ΤΗΣ ΖΩΗΣ ΤΟΥ ΠΑΙΔΙΟΥ
     4: 305.231ΠΑΠ
     5: '22548'
     8: NESTLE
     9: ΑΘΗΝΑ
     10: '1996'
     11: '76'
+    12: ΠΡΟΣΧΟΛΙΚΗ ΗΛΙΚΙΑ
+    13: ΠΡΟΣΧΟΛΙΚΗ ΗΛΙΚΙΑ
+    14: ΠΡΟΣΧΟΛΙΚΗ ΗΛΙΚΙΑ
     3: null
     6: null
     7: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -851625,15 +851701,14 @@
   - ΠΑΓΚΑΛΙΑΣ,ΞΕΝΟΦΩΝ
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 436
   topics:
   - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΑΣΤΥΝΟΜΙΚΟ
-  - ΑΣΤΥΝΟΜΙΚΟ ΜΥΘΙΣΤΟΡΙΜΑ
   notes: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789600451825'
   original_entry:
     0: 17284
@@ -851644,15 +851719,15 @@
     6: ΠΑΓΚΑΛΙΑΣ ΞΕΝ.
     8: ΚΕΔΡΟΣ
     9: ΑΘΗΝΑ
     10: '2021'
     11: '436'
     12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
     13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
-    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ ΜΥΘΙΣΤΟΡΙΜΑ
+    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
     18: '9789600451'
     19: '825'
     3: null
     7: null
     15: null
     16: null
@@ -851782,15 +851857,15 @@
   - ΚΑΝΕΛΟΠΟΥΛΟΥ,ΔΕΣ.
   edition: '1'
   editor: ΚΑΣΤΑΝΙΟΤΗΣ NOIR // ΑΘΗΝΑ
   edition_year: 2020
   pages: 564
   topics:
   - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
-  - ΜΥΘΙΣΤΟΡΙΜΑ
+  - ΜΥΘΙΣΤΟΡΗΜΑ
   - ΞΕΝΗ ΛΟΗΟΤΕΧΝΙΑ
   notes: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789600367546'
   original_entry:
@@ -851801,17 +851876,17 @@
     5: '22684'
     6: ΚΑΝΕΛΟΠΟΥΛΟΥ ΔΕΣ.
     7: 1Η
     8: ΚΑΣΤΑΝΙΟΤΗΣ NOIR
     9: ΑΘΗΝΑ
     10: '2020'
     11: '564'
-    12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
-    13: ΞΕΝΗ ΛΟΗΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
-    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
+    12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+    13: ΞΕΝΗ ΛΟΗΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
     18: '9789600367'
     19: '546'
     3: null
     15: null
     16: null
     20: null
@@ -851884,15 +851959,15 @@
   translators:
   - ΟΙΚΟΝΟΜΙΔΟΥ,ΜΑΡΙΑ
   editor: ΠΑΤΑΚΗΣ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 652
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-  - ΜΥΘΙΣΤΟΡΙΜΑ
+  - ΜΥΘΙΣΤΟΡΗΜΑ
   notes: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789601692715'
   original_entry:
     0: 17289
@@ -851901,17 +851976,17 @@
     4: 850.11ΜΑΣ
     5: '22682'
     6: ΟΙΚΟΝΟΜΙΔΟΥ ΜΑΡΙΑ
     8: ΠΑΤΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '2021'
     11: '652'
-    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
-    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
-    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
+    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
     18: '9789601692'
     19: '715'
     3: null
     7: null
     15: null
     16: null
@@ -852274,17 +852349,18 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17297
   authors:
-  - ΜΕΓΕΡ,ΜΑΡΙΣΣΑ
+  - MEYER,MARISSA
   title: ΣΙΝΤΕΡ
   subtitle: Η ΤΕΤΡΑΛΟΓΙΑ ΤΗΣ ΣΕΛΗΝΗΣ
+  dewey: 823 MEY
   entry_numbers:
   - '22678'
   translators:
   - ΚΑΛΟΦΟΛΙΑΣ
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2012
   pages: 486
@@ -852294,30 +852370,30 @@
   notes: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: '9789601648248'
   original_entry:
     0: 17297
-    1: ΜΕΓΕΡ,ΜΑΡΙΣΣΑ
+    1: MEYER,MARISSA
     2: ΣΙΝΤΕΡ
     3: Η ΤΕΤΡΑΛΟΓΙΑ ΤΗΣ ΣΕΛΗΝΗΣ
+    4: 823MEY
     5: '22678'
     6: ΚΑΛΟΦΟΛΙΑΣ
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2012'
     11: '486'
     12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
     13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
     14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
     17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
     18: '9789601648'
     19: '248'
-    4: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -852337,15 +852413,15 @@
   - '22677'
   translators:
   - ΚΟΚΚΙΝΟΥ,ΒΑΣΙΛΙΚΗ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2005
   pages: 390
   topics:
-  - ΜΥΘΙΣΤΟΡΙΜΑ
+  - ΜΥΘΙΣΤΟΡΗΜΑ
   notes: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 17298
     1: ΣΙΝΟΥΕ,ΖΙΛΜΠΕΡ
@@ -852353,17 +852429,17 @@
     4: 843ΣΙΝ
     5: '22677'
     6: ΚΟΚΚΙΝΟΥ ΒΑΣΙΛΙΚΗ
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2005'
     11: '390'
-    12: ΜΥΘΙΣΤΟΡΙΜΑ
-    13: ΜΥΘΙΣΤΟΡΙΜΑ
-    14: ΜΥΘΙΣΤΟΡΙΜΑ
+    12: ΜΥΘΙΣΤΟΡΗΜΑ
+    13: ΜΥΘΙΣΤΟΡΗΜΑ
+    14: ΜΥΘΙΣΤΟΡΗΜΑ
     17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
     3: null
     7: null
     15: null
     16: null
     18: null
     19: null
@@ -853348,11 +853424,10178 @@
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17319
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  title: ΜΙΑ ΠΛΩΤΗ ΠΟΛΙΤΕΙΑ
+  subtitle: ΝΑΥΤΙΚΟΣ ΑΠΟΚΛΕΙΣΜΟΣ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - '22777'
+  translators:
+  - Κ.ΜΠΟΥΛΟΥΚΟΥ
+  editor: ΤΕΣΣΕΡΑ ΠΙ // ΑΘΗΝΑ
+  edition_year: 2011
+  pages: 254
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604883264'
+  original_entry:
+    0: 17319
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
+    2: ΜΙΑ ΠΛΩΤΗ ΠΟΛΙΤΕΙΑ
+    3: ΝΑΥΤΙΚΟΣ ΑΠΟΚΛΕΙΣΜΟΣ
+    4: 808.899ΒΕΡ
+    5: '22777'
+    6: Κ.ΜΠΟΥΛΟΥΚΟΥ
+    8: ΤΕΣΣΕΡΑ ΠΙ
+    9: ΑΘΗΝΑ
+    10: '2011'
+    11: '254'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789604883'
+    19: '264'
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17320
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  title: ΡΟΒΗΡΟΣ Ο ΚΑΤΑΚΤΗΤΗΣ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - '20776'
+  translators:
+  - Χ.ΤΡΑΙΤΟΡΑΚΗ
+  editor: ΤΕΣΣΕΡΑ ΠΙ // ΑΘΗΝΑ
+  edition_year: 2011
+  pages: 230
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604883097'
+  original_entry:
+    0: 17320
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
+    2: ΡΟΒΗΡΟΣ Ο ΚΑΤΑΚΤΗΤΗΣ
+    4: 808.899ΒΕΡ
+    5: '20776'
+    6: Χ.ΤΡΑΙΤΟΡΑΚΗ
+    8: ΤΕΣΣΕΡΑ ΠΙ
+    9: ΑΘΗΝΑ
+    10: '2011'
+    11: '230'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789604883'
+    19: 097
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17321
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  title: ΒΟΡΡΑΣ ΕΝΑΝΤΙΟΝ ΝΟΤΟΥ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - '22775'
+  translators:
+  - Μ.ΜΑΥΡΟΜΑΤΑΚΗ
+  editor: ΤΕΣΣΕΡΑ ΠΙ // ΑΘΗΝΑ
+  edition_year: 2011
+  pages: 393
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604883509'
+  original_entry:
+    0: 17321
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
+    2: ΒΟΡΡΑΣ ΕΝΑΝΤΙΟΝ ΝΟΤΟΥ
+    4: 808.899ΒΕΡ
+    5: '22775'
+    6: Μ.ΜΑΥΡΟΜΑΤΑΚΗ
+    8: ΤΕΣΣΕΡΑ ΠΙ
+    9: ΑΘΗΝΑ
+    10: '2011'
+    11: '393'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789604883'
+    19: '509'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17322
+  authors:
+  - SMITH,WILBOUR
+  title: ΚΥΝΗΓΟΙ ΔΙΑΜΑΝΤΩΝ
+  dewey: 823 SMI
+  entry_numbers:
+  - '22766'
+  translators:
+  - ΜΑΝΩΛΙΔΗΣ,ΑΛΕΚΟΣ
+  editor: BELL // ΑΘΗΝΑ
+  edition_year: 2021
+  pages: 317
+  topics:
+  - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604502752'
+  original_entry:
+    0: 17322
+    1: SMITH,WILBOUR
+    2: ΚΥΝΗΓΟΙ ΔΙΑΜΑΝΤΩΝ
+    4: 823SMI
+    5: '22766'
+    6: ΑΛΕΚΟΣ ΜΑΝΩΛΙΔΗΣ
+    8: BELL
+    9: ΑΘΗΝΑ
+    10: '2021'
+    11: '317'
+    12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789604502'
+    19: '752'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17323
+  authors:
+  - ΚΑΡΑΦΥΛΛΗ,ΙΡΕΝΑ
+  title: Η ΑΣΥΜΒΙΒΑΣΤΗ ΜΟΥΣΑ
+  dewey: 889.21 ΚΑΡ
+  entry_numbers:
+  - '22768'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2008
+  pages: 540
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604534289'
+  original_entry:
+    0: 17323
+    1: ΚΑΡΑΦΥΛΛΗ,ΙΡΕΝΑ
+    2: Η ΑΣΥΜΒΙΒΑΣΤΗ ΜΟΥΣΑ
+    4: 889.21ΚΑΡ
+    5: '22768'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2008'
+    11: '540'
+    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789604534'
+    19: '289'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17324
+  authors:
+  - ΑΚΡΙΤΑ,ΕΛΕΝΑ
+  title: ΧΤΥΠΟΚΑΡΔΙΑ ΣΤΟ ΚΡΑΝΙΟ
+  dewey: 889.21 ΑΚΡ
+  entry_numbers:
+  - '22768'
+  editor: ΚΑΣΤΑΝΙΩΤΗΣ // ΑΘΗΝΑ
+  edition_year: 2011
+  pages: 181
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789600353723'
+  original_entry:
+    0: 17324
+    1: ΑΚΡΙΤΑ,ΕΛΕΝΑ
+    2: ΧΤΥΠΟΚΑΡΔΙΑ ΣΤΟ ΚΡΑΝΙΟ
+    4: 889.21ΑΚΡ
+    5: '22768'
+    8: ΚΑΣΤΑΝΙΩΤΗΣ
+    9: ΑΘΗΝΑ
+    10: '2011'
+    11: 181Σ
+    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789600353'
+    19: '723'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17325
+  authors:
+  - ΚΑΡΙΖΩΝΗ,ΚΑΤΕΡΙΝΑ
+  title: ΜΕΓΑΛΟ ΑΛΓΕΡΙ
+  entry_numbers:
+  - '2770'
+  editor: ΚΑΣΤΑΝΙΩΤΗΣ // ΑΘΗΝΑ
+  edition_year: 2006
+  pages: 272
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9600342547'
+  original_entry:
+    0: 17325
+    1: ΚΑΡΙΖΩΝΗ,ΚΑΤΕΡΙΝΑ
+    2: ΜΕΓΑΛΟ ΑΛΓΕΡΙ
+    4: 889.21ΚΑΡ2
+    5: '2770'
+    8: ΚΑΣΤΑΝΙΩΤΗΣ
+    9: ΑΘΗΝΑ
+    10: '2006'
+    11: '272'
+    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9600342547'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17326
+  authors:
+  - KOONTZ,DEAN
+  title: ΟΣΑ ΞΕΡΕΙ Η ΝΥΧΤΑ
+  dewey: 823 ΚΟΟ
+  entry_numbers:
+  - '22769'
+  translators:
+  - ΙΣΜΥΡΙΔΟΥ,ΠΑΛΜΥΡΑ
+  editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
+  edition_year: 2010
+  pages: 426
+  topics:
+  - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606354304'
+  original_entry:
+    0: 17326
+    1: KOONTZ,DEAN
+    2: ΟΣΑ ΞΕΡΕΙ Η ΝΥΧΤΑ
+    4: 823ΚΟΟ
+    5: '22769'
+    6: ΠΑΛΜΥΡΑ ΙΣΜΥΡΙΔΟΥ
+    8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
+    9: ΑΘΗΝΑ
+    10: '2010'
+    11: 426Σ
+    12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789606354'
+    19: '304'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17327
+  authors:
+  - ΘΕΟΤΟΚΑΣ,ΓΙΩΡΓΟΣ
+  title: ΑΡΓΩ
+  subtitle: ΙΣΤΟΡΙΑ ΣΤΗ ΛΟΓΟΤΕΧΝΙΑ
+  dewey: 889.21 ΘΕΟ
+  entry_numbers:
+  - '22771'
+  editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
+  edition_year: 2015
+  pages: 378
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789605036010'
+  original_entry:
+    0: 17327
+    1: ΘΕΟΤΟΚΑΣ,ΓΙΩΡΓΟΣ
+    2: ΑΡΓΩ
+    3: ΙΣΤΟΡΙΑ ΣΤΗ ΛΟΓΟΤΕΧΝΙΑ
+    4: 889.21ΘΕΟ
+    5: '22771'
+    8: ΤΟ ΒΗΜΑ
+    9: ΑΘΗΝΑ
+    10: '2015'
+    11: '378'
+    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789605036'
+    19: '010'
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17328
+  authors:
+  - BARKS,CARL
+  title: ΤΟ ΔΑΧΤΥΛΙΔΙ ΤΗΣ ΜΟΥΜΙΑΣ
+  dewey: 808.899 BAR
+  entry_numbers:
+  - '22774'
+  editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
+  edition_year: 2016
+  pages: 191
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789605850425'
+  original_entry:
+    0: 17328
+    1: BARKS,CARL
+    2: ΤΟ ΔΑΧΤΥΛΙΔΙ ΤΗΣ ΜΟΥΜΙΑΣ
+    4: 808.899BAR
+    5: '22774'
+    8: ΚΑΘΗΜΕΡΙΝΗ
+    9: ΑΘΗΝΑ
+    10: '2016'
+    11: '191'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789605850'
+    19: '425'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17329
+  authors:
+  - STRANDBERG,MATS
+  title: Η ΚΡΟΥΑΖΙΕΡΑ ΤΟΥ ΤΡΟΜΟΥ
+  dewey: 839.72 STR
+  entry_numbers:
+  - '22773'
+  translators:
+  - ΓΙΩΡΓΟΣ ΜΑΘΟΠΟΥΛΟΣ
+  editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
+  edition_year: 2019
+  pages: 576
+  topics:
+  - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789600449570'
+  original_entry:
+    0: 17329
+    1: STRANDBERG,MATS
+    2: Η ΚΡΟΥΑΖΙΕΡΑ ΤΟΥ ΤΡΟΜΟΥ
+    4: 839.72STR
+    5: '22773'
+    6: ΓΙΩΡΓΟΣ ΜΑΘΟΠΟΥΛΟΣ
+    8: ΚΕΔΡΟΣ
+    9: ΑΘΗΝΑ
+    10: '2019'
+    11: '576'
+    12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789600449'
+    19: '570'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17330
+  authors:
+  - MASTERTON,GRAHAM
+  title: ΠΛΗΓΩΜΕΝΟΙ ΑΓΓΕΛΟΙ
+  dewey: 823 MAS
+  entry_numbers:
+  - '22772'
+  translators:
+  - ΜΑΡΙΑ ΜΟΥΝΤΟΚΑΛΑΚΗ
+  editor: ΟΞΥ // ΑΘΗΝΑ
+  edition_year: 2017
+  pages: 432
+  topics:
+  - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604363544'
+  original_entry:
+    0: 17330
+    1: MASTERTON,GRAHAM
+    2: ΠΛΗΓΩΜΕΝΟΙ ΑΓΓΕΛΟΙ
+    4: 823MAS
+    5: '22772'
+    6: ΜΑΡΙΑ ΜΟΥΝΤΟΚΑΛΑΚΗ
+    8: ΟΞΥ
+    9: ΑΘΗΝΑ
+    10: '2017'
+    11: '432'
+    12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+    18: '9789604363'
+    19: '544'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17331
+  authors:
+  - ΒΡΑΚΑΣ,ΦΩΤΗΣ
+  title: ΦΙΛΙΠΠΙΑΔΑ Ο ΧΩΡΟΣ Ο ΟΙΚΙΣΜΟΣ Ο ΚΑΖΑΣ
+  dewey: 938.937 ΒΡΑ
+  entry_numbers:
+  - '22781'
+  editor: 24 ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
+  edition_year: 2022
+  pages: 359
+  topics:
+  - ΦΙΛΙΠΠΙΑΔΑ
+  - ΟΙΚΙΣΜΟΣ
+  notes: ΔΩΡΕΑ ΦΩΤΗ ΒΡΑΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786182015032'
+  original_entry:
+    0: 17331
+    1: ΒΡΑΚΑΣ,ΦΩΤΗΣ
+    2: ΦΙΛΙΠΠΙΑΔΑ Ο ΧΩΡΟΣ Ο ΟΙΚΙΣΜΟΣ Ο ΚΑΖΑΣ
+    4: 938.937ΒΡΑ
+    5: '22781'
+    8: 24 ΓΡΑΜΜΑΤΑ
+    9: ΑΘΗΝΑ
+    10: '2022'
+    11: 359Σ
+    12: ΙΣΤΟΡΙΑ-ΦΙΛΙΠΠΙΑΔΑ
+    13: ΟΙΚΙΣΜΟΣ
+    14: ΦΙΛΙΠΠΙΑΔΑ
+    15: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΦΩΤΗ ΒΡΑΚΑ
+    18: '9786182015'
+    19: '032'
+    3: null
+    6: null
+    7: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17332
+  authors:
+  - ΣΤΑΥΡΟΣ,ΧΡΗΣΤΟΣ
+  title: ΡΟΔΑΥΓΗ ΕΝΑ ΤΑΞΙΔΙ ΣΤΟ ΧΤΕΣ
+  dewey: 938.939 ΣΤΑ
+  entry_numbers:
+  - '22780'
+  editor: ΕΝΤΥΠΩΣΙΣ // ΑΡΤΑ
+  edition_year: 2020
+  pages: 199
+  topics:
+  - ΡΟΔΑΥΓΗ
+  - ΦΩΤΟΓΡΑΦΙΚΟ ΛΕΥΚΩΜΑ
+  notes: ΔΩΡΕΑ ΧΡΗΣΤΟΣ ΣΤΑΥΡΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180021097'
+  original_entry:
+    0: 17332
+    1: ΣΤΑΥΡΟΣ,ΧΡΗΣΤΟΣ
+    2: ΡΟΔΑΥΓΗ ΕΝΑ ΤΑΞΙΔΙ ΣΤΟ ΧΤΕΣ
+    4: 938.939ΣΤΑ
+    5: '22780'
+    8: ΕΝΤΥΠΩΣΙΣ
+    9: ΑΡΤΑ
+    10: '2020'
+    11: '199'
+    12: ΙΣΤΟΡΙΑ-ΡΟΔΑΥΓΗ
+    13: ΦΩΤΟΓΡΑΦΙΚΟ ΛΕΥΚΩΜΑ
+    14: ΡΟΔΑΥΓΗ
+    15: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΧΡΗΣΤΟΣ ΣΤΑΥΡΟΣ
+    18: '9786180021'
+    19: 097
+    3: null
+    6: null
+    7: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17333
+  authors:
+  - ΓΟΥΒΕΛΗ,ΓΙΩΤΑ
+  title: ΤΟ ΔΑΚΡΥ ΤΗΣ ΜΑΝΤΙΣΣΑΣ
+  dewey: 889.21 ΓΟΥ
+  entry_numbers:
+  - '22778'
+  editor: ΔΙΟΠΤΡΑ // ΑΘΗΝΑ
+  edition_year: 2022
+  pages: 501
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606539152'
+  original_entry:
+    0: 17333
+    1: ΓΟΥΒΕΛΗ,ΓΙΩΤΑ
+    2: ΤΟ ΔΑΚΡΥ ΤΗΣ ΜΑΝΤΙΣΣΑΣ
+    4: 889.21ΓΟΥ
+    5: '22778'
+    8: ΔΙΟΠΤΡΑ
+    9: ΑΘΗΝΑ
+    10: '2022'
+    11: '501'
+    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789606539'
+    19: '152'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17334
+  authors:
+  - ΣΚΛΑΒΕΝΙΤΗΣ,ΔΗΜΗΤΡΗΣ
+  title: 1922 ΜΕ ΞΙΦΟΛΟΓΧΗ ΚΑΙ ΓΡΑΦΙΔΑ ΣΤΟ ΜΙΚΡΑΣΙΑΤΙΚΟ ΜΕΤΩΠΟ
+  entry_numbers:
+  - '22782'
+  editor: ΜΟΡΦΩΤ.ΙΔΡΥΜΑ ΕΣΗΕΑ // ΑΘΗΝΑ
+  edition_year: 2022
+  pages: 301
+  topics:
+  - ΑΡΧΕΙΑΚΕΣ ΣΥΛΛΟΓΕΣ
+  - ΜΙΚΡΑΣΙΑΤΙΚΟ ΜΕΤΩΠΟ
+  - ΕΦΗΜΕΡΙΔΕΣ ΕΛΛΗΝΩΝ ΣΤΡΑΤΙΩΤΩΝ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17334
+    1: ΣΚΛΑΒΕΝΙΤΗΣ,ΔΗΜΗΤΡΗΣ
+    2: 1922 ΜΕ ΞΙΦΟΛΟΓΧΗ ΚΑΙ ΓΡΑΦΙΔΑ ΣΤΟ ΜΙΚΡΑΣΙΑΤΙΚΟ ΜΕΤΩΠΟ
+    5: '22782'
+    8: ΜΟΡΦΩΤ.ΙΔΡΥΜΑ ΕΣΗΕΑ
+    9: ΑΘΗΝΑ
+    10: '2022'
+    11: '301'
+    12: ΑΡΧΕΙΑΚΕΣ ΣΥΛΛΟΓΕΣ
+    13: ΜΙΚΡΑΣΙΑΤΙΚΟ ΜΕΤΩΠΟ
+    14: ΕΦΗΜΕΡΙΔΕΣ ΕΛΛΗΝΩΝ ΣΤΡΑΤΙΩΤΩΝ
+    18: '9789960888'
+    19: '9545'
+    3: null
+    4: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17335
+  authors:
+  - ΚΟΜΖΙΑΣ,ΓΕΩΡΓΙΟΣ
+  title: ΤΟ ΑΡΤΙΝΟ ΛΑΙΚΟ ΧΟΡΟΣΤΑΣΙ
+  dewey: 938.939 ΚΟΜ
+  entry_numbers:
+  - '22783'
+  editor: SOUL TWINKLES // ΑΘΗΝΑ
+  edition_year: 2021
+  pages: 406
+  topics:
+  - ΑΡΤΑ
+  - ΧΟΡΟΣΤΑΣΙ
+  - ΛΑΟΓΡΑΦΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786188389731'
+  original_entry:
+    0: 17335
+    1: ΚΟΜΖΙΑΣ,ΓΕΩΡΓΙΟΣ
+    2: ΤΟ ΑΡΤΙΝΟ ΛΑΙΚΟ ΧΟΡΟΣΤΑΣΙ
+    4: 938.939ΚΟΜ
+    5: '22783'
+    8: SOUL TWINKLES
+    9: ΑΘΗΝΑ
+    10: '2021'
+    11: '406'
+    12: ΙΣΤΟΡΙΑ-ΑΡΤΑ
+    13: ΧΟΡΟΣΤΑΣΙ
+    14: ΑΡΤΑ
+    15: ΛΑΟΓΡΑΦΙΑ
+    18: '9786188389'
+    19: '731'
+    3: null
+    6: null
+    7: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17336
+  authors:
+  - ΓΑΙΤΑΝΙΔΗΣ,ΠΑΥΛΟΣ
+  title: ΜΟΥΣΙΚΗ ΤΩΝ ΕΛΛΗΝΩΝ ΤΟΥ ΠΟΝΤΟΥ
+  dewey: 781.62 ΓΑΙ
+  entry_numbers:
+  - '22786'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2022
+  pages: 150
+  topics:
+  - ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606022586'
+  original_entry:
+    0: 17336
+    1: ΓΑΙΤΑΝΙΔΗΣ,ΠΑΥΛΟΣ
+    2: ΜΟΥΣΙΚΗ ΤΩΝ ΕΛΛΗΝΩΝ ΤΟΥ ΠΟΝΤΟΥ
+    4: 781.62ΓΑΙ
+    5: '22786'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2022'
+    11: '150'
+    12: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+    13: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+    14: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606022'
+    19: '586'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17337
+  authors:
+  - ΓΑΙΤΑΝΙΔΗΣ,ΠΑΥΛΟΣ
+  title: Η ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ ΩΣ ΕΠΕΚΤΑΣΗ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΜΟΥΣΙΚΗΣ
+  dewey: 781.62 ΓΑΙ
+  entry_numbers:
+  - '22787'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2022
+  pages: 268
+  topics:
+  - ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606023361'
+  original_entry:
+    0: 17337
+    1: ΓΑΙΤΑΝΙΔΗΣ,ΠΑΥΛΟΣ
+    2: Η ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ ΩΣ ΕΠΕΚΤΑΣΗ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΜΟΥΣΙΚΗΣ
+    4: 781.62ΓΑΙ
+    5: '22787'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2022'
+    11: '268'
+    12: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+    13: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+    14: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606023'
+    19: '361'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17338
+  authors:
+  - ΤΣΙΝΑΛΗΣ,ΚΟΣΜΑΣ
+  title: ΕΝΑΝ ΖΑΝΤΟΝ ΑΡΚΟΥΔΟΠΟΝ
+  dewey: 889.3 ΤΣΙ
+  entry_numbers:
+  - '22790'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2022
+  pages: 70
+  topics:
+  - ΠΟΝΤΙΑΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
+  - ΠΟΝΤΙΑΚΟ ΠΑΡΑΜΥΘΙ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606023613'
+  original_entry:
+    0: 17338
+    1: ΤΣΙΝΑΛΗΣ,ΚΟΣΜΑΣ
+    2: ΕΝΑΝ ΖΑΝΤΟΝ ΑΡΚΟΥΔΟΠΟΝ
+    4: 889.3ΤΣΙ
+    5: '22790'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2022'
+    11: '70'
+    12: ΠΟΝΤΙΑΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
+    13: ΠΟΝΤΙΑΚΟ ΠΑΡΑΜΥΘΙ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606023'
+    19: '613'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17339
+  authors:
+  - ΝΤΕ ΣΑΙΝΤ-ΕΞΥΠΕΡΥ,ΑΝΤΟΥΑΝ
+  title: Ο ΜΙΚΡΟΣ Ο ΠΡΙΓΚΙΠΑΣ
+  dewey: 889.3 ΝΤΕ
+  entry_numbers:
+  - '22798'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2022
+  pages: 150
+  topics:
+  - ΠΟΝΤΙΑΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
+  - ΠΟΝΤΙΑΚΟ ΠΑΡΑΜΥΘΙ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606022678'
+  original_entry:
+    0: 17339
+    1: ΝΤΕ ΣΑΙΝΤ-ΕΞΥΠΕΡΥ,ΑΝΤΟΥΑΝ
+    2: Ο ΜΙΚΡΟΣ Ο ΠΡΙΓΚΙΠΑΣ
+    4: 889.3ΝΤΕ
+    5: '22798'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2022'
+    11: '150'
+    12: ΠΟΝΤΙΑΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
+    13: ΠΟΝΤΙΑΚΟ ΠΑΡΑΜΥΘΙ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606022'
+    19: '678'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17340
+  authors:
+  - ΜΑΥΡΙΔΟΥ,ΜΑΡΙΑ
+  title: ΤΗ ΦΤΕΧΟΥ ΤΟ ΚΑΜΙΣ ΚΑΙ ΤΟ ΞΕΦΤΙΛΕΡ
+  dewey: 887 ΜΑΥ
+  entry_numbers:
+  - '22799'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2021
+  pages: 144
+  topics:
+  - ΠΟΝΤΙΑΚΟ ΘΕΑΤΡΟ
+  - ΘΕΑΤΡΙΚΑ ΕΡΓΑ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606023057'
+  original_entry:
+    0: 17340
+    1: ΜΑΥΡΙΔΟΥ,ΜΑΡΙΑ
+    2: ΤΗ ΦΤΕΧΟΥ ΤΟ ΚΑΜΙΣ ΚΑΙ ΤΟ ΞΕΦΤΙΛΕΡ
+    4: 887ΜΑΥ
+    5: '22799'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2021'
+    11: '144'
+    12: ΠΟΝΤΙΑΚΟ ΘΕΑΤΡΟ
+    13: ΘΕΑΤΡΙΚΟ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606023'
+    19: '057'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17341
+  authors:
+  - ΦΥΛΑΧΤΟΣ,ΧΡΗΣΤΟΣ
+  title: ΑΠ ΤΟ ΧΟΛΟΜΩΝΤΑ ΣΤΟ ΣΑΓΓΑΡΙΟ
+  dewey: 887 ΦΥΛ
+  entry_numbers:
+  - '22785'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2017
+  pages: 111
+  topics:
+  - ΠΟΝΤΙΑΚΟ ΘΕΑΤΡΟ
+  - ΘΕΑΤΡΙΚΑ ΕΡΓΑ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606023200'
+  original_entry:
+    0: 17341
+    1: ΦΥΛΑΧΤΟΣ,ΧΡΗΣΤΟΣ
+    2: ΑΠ ΤΟ ΧΟΛΟΜΩΝΤΑ ΣΤΟ ΣΑΓΓΑΡΙΟ
+    4: 887ΦΥΛ
+    5: '22785'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2017'
+    11: '111'
+    12: ΠΟΝΤΙΑΚΟ ΘΕΑΤΡΟ
+    13: ΘΕΑΤΡΙΚΟ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606023'
+    19: '200'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17342
+  authors:
+  - ΛΑΖΙΟΥ,ΓΙΟΥΛΗ
+  title: ΑΣ ΣΗΝ ΛΑΛΙΑΝ Σ ΣΟ ΓΡΑΨΙΜΟΝ
+  dewey: 889.3 ΛΑΖ
+  entry_numbers:
+  - '22791'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2022
+  pages: 157
+  topics:
+  - ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+  - ΛΟΓΟΤΕΧΝΙΑ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17342
+    1: ΛΑΖΙΟΥ,ΓΙΟΥΛΗ
+    2: ΑΣ ΣΗΝ ΛΑΛΙΑΝ Σ ΣΟ ΓΡΑΨΙΜΟΝ
+    4: 889.3ΛΑΖ
+    5: '22791'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2022'
+    11: '157'
+    12: ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+    13: ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606023'
+    19: '533545'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17343
+  authors:
+  - ΧΑΤΖΗΘΕΟΔΩΡΙΔΗΣ,ΒΑΣΙΛΗΣ
+  title: ΨΗΓΜΑΤΑ ΠΟΝΤΙΑΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
+  dewey: 889.3 ΧΑΤ
+  entry_numbers:
+  - '22784'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2021
+  pages: 144
+  topics:
+  - ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+  - ΛΟΓΟΤΕΧΝΙΑ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606023323'
+  original_entry:
+    0: 17343
+    1: ΧΑΤΖΗΘΕΟΔΩΡΙΔΗΣ,ΒΑΣΙΛΗΣ
+    2: ΨΗΓΜΑΤΑ ΠΟΝΤΙΑΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
+    4: 889.3ΧΑΤ
+    5: '22784'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2021'
+    11: '144'
+    12: ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+    13: ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606023'
+    19: '323'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17344
+  authors:
+  - ΧΑΤΖΗΘΕΟΔΩΡΙΔΗΣ,ΒΑΣΙΛΗΣ
+  title: ΣΑΝ ΤΑ ΠΟΥΛΙΑ ΣΤΗΝ ΜΠΟΡΑ
+  dewey: 920.7 ΧΑΤ
+  entry_numbers:
+  - '22800'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2019
+  pages: 445
+  topics:
+  - ΑΥΤΟΒΙΟΓΡΑΦΙΑ
+  - ΒΙΟΓΡΑΦΙΕΣ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606022494'
+  original_entry:
+    0: 17344
+    1: ΧΑΤΖΗΘΕΟΔΩΡΙΔΗΣ,ΒΑΣΙΛΗΣ
+    2: ΣΑΝ ΤΑ ΠΟΥΛΙΑ ΣΤΗΝ ΜΠΟΡΑ
+    4: 920.7ΧΑΤ
+    5: '22800'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2019'
+    11: '445'
+    12: ΑΥΤΟΒΙΟΓΡΑΦΙΕΣ
+    13: ΒΙΟΓΡΑΦΙΕΣ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606022'
+    19: '494'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17345
+  authors:
+  - ΙΩΑΝΝΙΔΟΥ,ΓΙΩΤΑ
+  title: ΙΣΚΙΛΙ
+  dewey: 889.3 ΙΩΑ
+  entry_numbers:
+  - '22797'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2020
+  pages: 348
+  topics:
+  - ΠΟΝΤΙΑΚΗ ΠΕΖΟΓΡΑΦΙΑ
+  - ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606022487'
+  original_entry:
+    0: 17345
+    1: ΙΩΑΝΝΙΔΟΥ,ΓΙΩΤΑ
+    2: ΙΣΚΙΛΙ
+    4: 889.3ΙΩΑ
+    5: '22797'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2020'
+    11: '348'
+    12: ΠΟΝΤΙΑΚΗ ΠΕΖΟΓΡΑΦΙΑ
+    13: ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606022'
+    19: '487'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17346
+  authors:
+  - ΑΛΕΞΙΑΔΗΣ,ΘΩΜΑΣ
+  title: Ο ΠΟΛΕΜΑΡΧΟΣ ΤΗΣ ΕΥΠΑΤΟΡΙΑΣ ΑΝΑΣΤΑΣΙΟΣ ΠΑΠΑΔΟΠΟΥΛΟΣ
+  dewey: 938.71 ΑΛΕ
+  entry_numbers:
+  - '22796'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2020
+  pages: 324
+  topics:
+  - ΠΟΝΤΟΣ
+  - ΑΝΤΑΡΤΙΚΟ ΤΟΥ ΠΟΝΤΟΥ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606022906'
+  original_entry:
+    0: 17346
+    1: ΑΛΕΞΙΑΔΗΣ,ΘΩΜΑΣ
+    2: Ο ΠΟΛΕΜΑΡΧΟΣ ΤΗΣ ΕΥΠΑΤΟΡΙΑΣ ΑΝΑΣΤΑΣΙΟΣ ΠΑΠΑΔΟΠΟΥΛΟΣ
+    4: 938.71ΑΛΕ
+    5: '22796'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2020'
+    11: '324'
+    12: ΠΟΝΤΟΣ
+    13: ΙΣΤΟΡΙΑ
+    14: ΑΝΤΑΡΤΙΚΟ ΤΟΥ ΠΟΝΤΟΥ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606022'
+    19: '906'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17347
+  authors:
+  - ΚΑΡΙΠΙΔΟΥ,ΑΝΝΥ
+  title: ΙΛΙΑΔΑ
+  dewey: 881 ΚΑΡ
+  entry_numbers:
+  - '22794'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2020
+  pages: 205
+  topics:
+  - ΠΟΝΤΙΑΚΗ ΔΙΑΛΕΚΤΟΣ
+  - ΕΠΙΚΗ ΠΟΙΗΣΗ
+  - ΟΜΗΡΟΥ ΙΛΙΑΔΑ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606022739'
+  original_entry:
+    0: 17347
+    1: ΚΑΡΙΠΙΔΟΥ,ΑΝΝΥ
+    2: ΙΛΙΑΔΑ
+    4: 881ΚΑΡ
+    5: '22794'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2020'
+    11: '205'
+    12: ΠΟΝΤΙΑΚΗ ΔΙΑΛΕΚΤΟΣ
+    13: ΕΠΙΚΗ ΠΟΙΗΣΗ
+    14: ΟΜΗΡΟΥ ΙΛΙΑΔΑ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606022'
+    19: '739'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17348
+  authors:
+  - ΠΕΤΡΟΠΟΥΛΟΥ,ΙΩΑΝΝΑ
+  title: Η ΣΜΥΡΝΗ ΤΩΝ ΒΙΒΛΙΩΝ
+  dewey: 070.509 ΠΕΤ
+  entry_numbers:
+  - '22792'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 204
+  topics:
+  - ΕΚΔΟΤΕΣ ΚΑΙ ΕΚΔΟΣΕΙΣ ΣΤΗ ΣΜΥΡΝΗ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789609586023'
+  original_entry:
+    0: 17348
+    1: ΠΕΤΡΟΠΟΥΛΟΥ,ΙΩΑΝΝΑ
+    2: Η ΣΜΥΡΝΗ ΤΩΝ ΒΙΒΛΙΩΝ
+    4: 070.509ΠΕΤ
+    5: '22792'
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '204'
+    12: ΕΚΔΟΤΕΣ ΚΑΙ ΕΚΔΟΣΕΙΣ ΣΤΗ ΣΜΥΡΝΗ
+    13: ΕΚΔΟΤΕΣ ΚΑΙ ΕΚΔΟΣΕΙΣ ΣΤΗ ΣΜΥΡΝΗ
+    14: ΕΚΔΟΤΕΣ ΚΑΙ ΕΚΔΟΣΕΙΣ ΣΤΗ ΣΜΥΡΝΗ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789609586'
+    19: '023'
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17349
+  authors:
+  - ΕΛΕΥΘΕΡΙΑΔΟΥ,ΡΟΖΑΛΙΑ
+  title: ΤΑΞΙΔΙ ΣΤΟΝ ΠΑΡΑΔΕΙΣΟ
+  dewey: 889.3 ΕΛΕ
+  entry_numbers:
+  - '22793'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2021
+  pages: 15
+  topics:
+  - ΠΟΝΤΙΑΚΗ ΠΕΖΟΓΡΑΦΙΑ
+  - ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606022500'
+  original_entry:
+    0: 17349
+    1: ΕΛΕΥΘΕΡΙΑΔΟΥ,ΡΟΖΑΛΙΑ
+    2: ΤΑΞΙΔΙ ΣΤΟΝ ΠΑΡΑΔΕΙΣΟ
+    4: 889.3ΕΛΕ
+    5: '22793'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2021'
+    11: '15'
+    12: ΠΟΝΤΙΑΚΗ ΠΕΖΟΓΡΑΦΙΑ
+    13: ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+    14: ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606022'
+    19: '500'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17350
+  authors:
+  - ΒΕΝΕΖΗΣ,ΗΛΙΑΣ
+  title: Η ΚΙΒΩΤΟΣ ΤΟΥ ΜΙΚΡΑΣΙΑΤΙΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
+  entry_numbers:
+  - '22789'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2021
+  pages: 180
+  topics: []
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789609586030'
+  original_entry:
+    0: 17350
+    1: ΒΕΝΕΖΗΣ,ΗΛΙΑΣ
+    2: Η ΚΙΒΩΤΟΣ ΤΟΥ ΜΙΚΡΑΣΙΑΤΙΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
+    5: '22789'
+    9: ΑΘΗΝΑ
+    10: '2021'
+    11: '180'
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789609586'
+    19: '030'
+    3: null
+    4: null
+    6: null
+    7: null
+    8: null
+    12: null
+    13: null
+    14: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17351
+  authors:
+  - ΛΙΑΖΟΣ,ΝΙΚΟΛΑΟΣ
+  title: ΤΑ ΤΟΥΡΚΙΚΑ ΑΝΑΓΝΩΣΤΙΚΑ ΕΓΧΕΙΡΙΔΙΑ ΤΗΣ ΠΡΩΤΟΒΑΘΜΙΑΣ ΕΚΠΑΙΔ
+  dewey: 956.5 ΛΙΑ
+  entry_numbers:
+  - '22788'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2022
+  pages: 192
+  topics:
+  - ΕΚΠΑΙΔΕΥΣΗ
+  - ΠΟΝΤΟΣ
+  - ΔΥΤΙΚΗ ΘΡΑΚΗ
+  - ΕΚΠΑΙΔΕΥΣΗ ΜΕΙΟΝΟΤΙΚΗ ΔΥΤΙΚΗ ΘΡΑΚΗ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606023729'
+  original_entry:
+    0: 17351
+    1: ΛΙΑΖΟΣ,ΝΙΚΟΛΑΟΣ
+    2: ΤΑ ΤΟΥΡΚΙΚΑ ΑΝΑΓΝΩΣΤΙΚΑ ΕΓΧΕΙΡΙΔΙΑ ΤΗΣ ΠΡΩΤΟΒΑΘΜΙΑΣ ΕΚΠΑΙΔ
+    4: 956.5ΛΙΑ
+    5: '22788'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2022'
+    11: '192'
+    12: ΕΚΠΑΙΔΕΥΣΗ-ΠΟΝΤΟΣ-ΔΥΤΙΚΗ ΘΡΑΚΗ
+    13: ΠΟΝΤΟΣ-ΕΚΠΑΙΔΕΥΣΗ
+    14: ΕΚΠΑΙΔΕΥΣΗ ΜΕΙΟΝΟΤΙΚΗ ΔΥΤΙΚΗ ΘΡΑΚΗ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606023'
+    19: '729'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17352
+  authors:
+  - ΕΛΕΥΘΕΡΙΑΔΟΥ,ΡΟΖΑΛΙΑ
+  title: ΤΑ ΧΡΩΜΑΤΑ ΤΗΣ ΘΑΛΑΣΣΑΣ
+  dewey: 889.11 ΕΛΕ
+  entry_numbers:
+  - '22795'
+  editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2022
+  pages: 16
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
+  - ΠΟΙΗΜΑΤΑ
+  - ΠΟΝΤΟΣ
+  notes: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606023484'
+  original_entry:
+    0: 17352
+    1: ΕΛΕΥΘΕΡΙΑΔΟΥ,ΡΟΖΑΛΙΑ
+    2: ΤΑ ΧΡΩΜΑΤΑ ΤΗΣ ΘΑΛΑΣΣΑΣ
+    4: 889.11ΕΛΕ
+    5: '22795'
+    8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2022'
+    11: '16'
+    12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
+    13: ΠΟΝΤΟΣ-ΠΟΙΗΜΑΤΑ
+    14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
+    15: ΠΟΙΗΜΑΤΑ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+    18: '9789606023'
+    19: '484'
+    3: null
+    6: null
+    7: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17353
+  authors:
+  - ΔΑΡΛΑΣΗ,ΑΓΓΕΛΙΚΗ
+  title: ΟΙ ΟΝΕΙΡΟΦΥΛΑΚΕΣ ΚΑΙ Ο ΦΑΡΟΣ ΤΩΝ ΟΝΕΙΡΩΝ
+  dewey: 808.899 ΔΑΡ
+  entry_numbers:
+  - '19459'
+  editor: ΠΑΤΑΚΗΣ // ΑΘΗΝΑ
+  edition_year: 2013
+  pages: 266
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601648552'
+  original_entry:
+    0: 17353
+    1: ΔΑΡΛΑΣΗ,ΑΓΓΕΛΙΚΗ
+    2: ΟΙ ΟΝΕΙΡΟΦΥΛΑΚΕΣ ΚΑΙ Ο ΦΑΡΟΣ ΤΩΝ ΟΝΕΙΡΩΝ
+    4: 808.899ΔΑΡ
+    5: '19459'
+    8: ΠΑΤΑΚΗΣ
+    9: ΑΘΗΝΑ
+    10: '2013'
+    11: 266Σ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789601648'
+    19: '552'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17354
+  authors:
+  - ΖΕΗ,ΑΛΚΗ
+  title: Ο ΜΕΓΑΛΟΣ ΠΕΡΙΠΑΤΟΣ ΤΟΥ ΠΕΤΡΟΥ
+  dewey: 808.899 ΖΕΗ
+  entry_numbers:
+  - '19462'
+  editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
+  edition_year: 1987
+  pages: 260
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9600400695'
+  original_entry:
+    0: 17354
+    1: ΖΕΗ,ΑΛΚΗ
+    2: Ο ΜΕΓΑΛΟΣ ΠΕΡΙΠΑΤΟΣ ΤΟΥ ΠΕΤΡΟΥ
+    4: 808.899ΖΕΗ
+    5: '19462'
+    8: ΚΕΔΡΟΣ
+    9: ΑΘΗΝΑ
+    10: '1987'
+    11: 260Σ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9600400695'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17355
+  authors:
+  - ΙΩΑΝΝΙΔΗΣ,Ι.Δ
+  title: ΚΑΒΑΛΑ ΣΤΟ ΧΡΟΝΟΔΙΑΒΙΤΗ
+  dewey: 808.899 ΙΩΑ
+  entry_numbers:
+  - '22801'
+  editor: ΚΑΣΤΑΝΙΩΤΗΣ // ΑΘΗΝΑ
+  edition_year: 1989
+  pages: 151
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9600303525'
+  original_entry:
+    0: 17355
+    1: ΙΩΑΝΝΙΔΗΣ,Ι.Δ
+    2: ΚΑΒΑΛΑ ΣΤΟ ΧΡΟΝΟΔΙΑΒΙΤΗ
+    4: 808.899ΙΩΑ
+    5: '22801'
+    8: ΚΑΣΤΑΝΙΩΤΗΣ
+    9: ΑΘΗΝΑ
+    10: '1989'
+    11: '151'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9600303525'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17356
+  authors:
+  - ΙΩΑΝΝΟΥ,ΓΙΩΡΓΟΣ
+  title: ΠΑΡΑΜΥΘΙΑ ΤΟΥ ΛΑΟΥ ΜΑΣ
+  dewey: 808.899 ΙΩΑ
+  entry_numbers:
+  - '20638'
+  editor: ΕΡΜΗΣ // ΑΘΗΝΑ
+  edition_year: 2008
+  pages: 375
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17356
+    1: ΙΩΑΝΝΟΥ,ΓΙΩΡΓΟΣ
+    2: ΠΑΡΑΜΥΘΙΑ ΤΟΥ ΛΑΟΥ ΜΑΣ
+    4: 808.899ΙΩΑ
+    5: '20638'
+    8: ΕΡΜΗΣ
+    9: ΑΘΗΝΑ
+    10: '2008'
+    11: 375Σ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17357
+  authors:
+  - ΚΩΖΙΝΣ,ΜΑΡΓΚΑΡΕΤ
+  title: ΒΕΝΙΑΜΙΝ ΦΡΑΓΚΛΙΝΟΣ
+  dewey: 808.899 ΚΩΖ
+  entry_numbers:
+  - '20413'
+  editor: ΑΤΛΑΝΤΙΣ // ΑΘΗΝΑ
+  pages: 159
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  donors:
+  - ΣΠΥΡΟΥ,ΣΠΥΡΙΔΩΝ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17357
+    1: ΚΩΖΙΝΣ,ΜΑΡΓΚΑΡΕΤ
+    2: ΒΕΝΙΑΜΙΝ ΦΡΑΓΚΛΙΝΟΣ
+    4: 808.899ΚΩΖ
+    5: '20413'
+    8: ΑΤΛΑΝΤΙΣ
+    9: ΑΘΗΝΑ
+    11: 159Σ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΣΠΥΡΙΔΩΝ ΣΠΥΡΟΥ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17358
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  title: Ο ΚΥΡΙΑΡΧΟΣ ΤΟΥ ΚΟΣΜΟΥ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - 9170Α
+  translators:
+  - Λ.ΟΛΥΜΠΙΟΥ
+  editor: ΑΤΤΙΚΟΣ // ΑΘΗΝΑ
+  pages: 212
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17358
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+    2: Ο ΚΥΡΙΑΡΧΟΣ ΤΟΥ ΚΟΣΜΟΥ
+    4: 808.899ΒΕΡ
+    5: 9170Α
+    6: Λ.ΟΛΥΜΠΙΟΥ
+    8: ΑΤΤΙΚΟΣ
+    9: ΑΘΗΝΑ
+    11: '212'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17359
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  title: ΚΟΥΡΣΑΡΟΙ ΤΟΥ ΑΙΓΑΙΟΥ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - 9175Α
+  translators:
+  - ΚΩΣΤΕΛΕΝΟΣ,Δ.Π.
+  editor: ΑΤΤΙΚΟΣ // ΑΘΗΝΑ
+  pages: 206
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17359
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+    2: ΚΟΥΡΣΑΡΟΙ ΤΟΥ ΑΙΓΑΙΟΥ
+    4: 808.899ΒΕΡ
+    5: 9175Α
+    6: Δ.Π.ΚΩΣΤΕΛΕΝΟΣ
+    8: ΑΤΤΙΚΟΣ
+    9: ΑΘΗΝΑ
+    11: '206'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17360
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  title: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - '13461'
+  translators:
+  - Λ.ΟΛΥΜΠΙΟΥ
+  editor: ΑΤΤΙΚΟΣ // ΑΘΗΝΑ
+  pages: 260
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17360
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+    2: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
+    4: 808.899ΒΕΡ
+    5: '13461'
+    6: Λ.ΟΛΥΜΠΙΟΥ
+    8: ΑΤΤΙΚΟΣ
+    9: ΑΘΗΝΑ
+    11: '260'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17361
+  authors:
+  - ΑΝΤΕΡΣΕΝ,ΧΑΝΣ ΚΡΙΣΤΙΑΝ
+  title: ΑΠΑΝΤΑ Ε
+  dewey: 808.899 ΑΝΤ
+  entry_numbers: []
+  translators:
+  - Σ.ΠΡΩΤΟΠΑΠΑ
+  editor: ΑΡΣΕΝΙΔΗΣ // ΑΘΗΝΑ
+  pages: 188
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17361
+    1: ΑΝΤΕΡΣΕΝ,ΧΑΝΣ ΚΡΙΣΤΙΑΝ
+    2: ΑΠΑΝΤΑ Ε
+    4: 808.899ΑΝΤ
+    6: Σ.ΠΡΩΤΟΠΑΠΑ
+    8: ΑΡΣΕΝΙΔΗΣ
+    9: ΑΘΗΝΑ
+    11: '188'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    5: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17362
+  authors:
+  - ΑΝΤΡΙΟΥΣ,ΤΖΟΥΛΙ
+  title: ΜΑΝΤΥ
+  dewey: 808.899 ΑΝΤ
+  entry_numbers: []
+  translators:
+  - Κ.ΣΙΝΟΥ
+  editor: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ // ΑΘΗΝΑ
+  pages: 148
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17362
+    1: ΑΝΤΡΙΟΥΣ,ΤΖΟΥΛΙ
+    2: ΜΑΝΤΥ
+    4: 808.899ΑΝΤ
+    6: Κ.ΣΙΝΟΥ
+    8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
+    9: ΑΘΗΝΑ
+    11: '148'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    5: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17363
+  authors: []
+  title: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΚΟΥΣΤΩ
+  subtitle: ΟΑΣΗ ΣΤΟ ΔΙΑΣΤΗΜΑ
+  dewey: 808.899 ΚΟΥ
+  entry_numbers:
+  - '7402'
+  translators:
+  - ΑΒΡΑΜΙΔΗΣ,ΟΜΗΡΟΣ
+  editor: ΑΛΚΥΩΝ // ΑΘΗΝΑ
+  edition_year: 1973
+  pages: 141
+  topics:
+  - ΠΑΙΔΙΚΗ ΒΙΒΛΙΟΘΗΚΗ
+  - ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
+  volume: ΤΟΜΟΣ 1
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17363
+    1: Χ.Σ.
+    2: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΚΟΥΣΤΩ
+    3: ΟΑΣΗ ΣΤΟ ΔΙΑΣΤΗΜΑ
+    4: 808.899ΚΟΥ
+    5: '7402'
+    6: ΟΜΗΡΟΣ ΑΒΡΑΜΙΔΗΣ
+    8: ΑΛΚΥΩΝ
+    9: ΑΘΗΝΑ
+    10: '1973'
+    11: '141'
+    12: ΠΑΙΔΙΚΗ ΒΙΒΛΙΟΘΗΚΗ-ΕΓΚΥΚΛΟΑΠΙΔΕΙΑ
+    13: ΠΑΙΔΙΚΗ ΒΙΒΛΙΟΘΗΚΗ
+    14: ΕΓΚΥΚΛΟΑΠΙΔΕΙΑ
+    17: ΤΟΜΟΣ 1
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17364
+  authors:
+  - ΒΑΡΕΛΛΑ,ΑΓΓΕΛΙΚΗ
+  title: ΤΗΛΕΦΩΝΗΜΑΤΑ ΚΙ ΕΝΑΣ ΛΑΓΟΣ
+  dewey: 808.899 ΒΑΡ
+  entry_numbers:
+  - '20419'
+  editor: ΜΙΝΩΑΣ ΕΚΔΟΣΕΙΣ // ΑΘΗΝΑ
+  edition_year: 2003
+  pages: 77
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9605421038'
+  original_entry:
+    0: 17364
+    1: ΒΑΡΕΛΛΑ,ΑΓΓΕΛΙΚΗ
+    2: ΤΗΛΕΦΩΝΗΜΑΤΑ ΚΙ ΕΝΑΣ ΛΑΓΟΣ
+    4: 808.899ΒΑΡ
+    5: '20419'
+    8: ΜΙΝΩΑΣ ΕΚΔΟΣΕΙΣ
+    9: ΑΘΗΝΑ
+    10: '2003'
+    11: '77'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    19: '9605421038'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17365
+  authors:
+  - ΚΟΛΕΤ,ΒΙΒΙΕ
+  title: ΤΟ ΠΟΛΙΚΟ ΑΣΤΕΡΙ
+  dewey: 808.899 ΚΟΛ
+  entry_numbers:
+  - '20427'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 1990
+  pages: 210
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9607020030'
+  original_entry:
+    0: 17365
+    1: ΚΟΛΕΤ,ΒΙΒΙΕ
+    2: ΤΟ ΠΟΛΙΚΟ ΑΣΤΕΡΙ
+    4: 808.899ΚΟΛ
+    5: '20427'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '1990'
+    11: '210'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    19: '9607020030'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17366
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  title: ΜΠΡΟΣΤΑ ΣΤΗ ΣΗΜΑΙΑ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - '22804'
+  editor: ΑΣΤΗΡ // ΑΘΗΝΑ
+  edition_year: 1978
+  pages: 272
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17366
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+    2: ΜΠΡΟΣΤΑ ΣΤΗ ΣΗΜΑΙΑ
+    4: 808.899ΒΕΡ
+    5: '22804'
+    8: ΑΣΤΗΡ
+    9: ΑΘΗΝΑ
+    10: '1978'
+    11: '272'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17367
+  authors:
+  - ΓΚΟΡΚΙ,ΜΑΞΙΜ
+  title: Η ΦΛΟΓΕΡΗ ΚΑΡΔΙΑ ΤΟΥ ΝΤΑΝΚΟ
+  dewey: 808.899 ΓΚΟ
+  entry_numbers:
+  - '20152'
+  editor: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ // ΑΘΗΝΑ
+  edition_year: 1983
+  pages: 98
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17367
+    1: ΓΚΟΡΚΙ,ΜΑΞΙΜ
+    2: Η ΦΛΟΓΕΡΗ ΚΑΡΔΙΑ ΤΟΥ ΝΤΑΝΚΟ
+    4: 808.899ΓΚΟ
+    5: '20152'
+    8: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ
+    9: ΑΘΗΝΑ
+    10: '1983'
+    11: '98'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17368
+  authors:
+  - ΓΟΥΕΛΣ,ΡΕΝΑΤΕ
+  title: Η ΜΕΛΑΝΙ ΚΑΙ ΤΑ ΜΑΓΙΑ
+  dewey: 808.899 ΓΟΥ
+  entry_numbers:
+  - '19455'
+  editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
+  pages: 125
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9606000389'
+  original_entry:
+    0: 17368
+    1: ΓΟΥΕΛΣ,ΡΕΝΑΤΕ
+    2: Η ΜΕΛΑΝΙ ΚΑΙ ΤΑ ΜΑΓΙΑ
+    4: 808.899ΓΟΥ
+    5: '19455'
+    8: ΠΑΤΑΚΗ
+    9: ΑΘΗΝΑ
+    11: '125'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    19: '9606000389'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17369
+  authors:
+  - ΓΟΥΛΙΜΗ,ΑΛΚΗΣ
+  title: Η ΑΟΡΑΤΗ ΣΕΛΙΔΑ
+  dewey: 808.899 ΓΟΥ
+  entry_numbers:
+  - '22805'
+  editor: ΝΕΑΝΙΚΗ ΒΙΒΛΙΟΘΗΚΗ // ΑΘΗΝΑ
+  edition_year: 1989
+  pages: 385
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17369
+    1: ΓΟΥΛΙΜΗ,ΑΛΚΗΣ
+    2: Η ΑΟΡΑΤΗ ΣΕΛΙΔΑ
+    4: 808.899ΓΟΥ
+    5: '22805'
+    8: ΝΕΑΝΙΚΗ ΒΙΒΛΙΟΘΗΚΗ
+    9: ΑΘΗΝΑ
+    10: '1989'
+    11: '385'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    19: 960030260Χ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17370
+  authors:
+  - ΓΟΥΠΟΣ,ΘΕΟΔΩΡΟΣ
+  title: Η ΓΛΩΣΣΑ ΜΟΥ ΓΙΑ ΤΗΝ Α ΔΗΜΟΤΙΚΟΥ
+  dewey: 808.899 ΓΟΥ
+  entry_numbers:
+  - '20630'
+  editor: ΕΚΔΟΣΕΙΣ ΚΑΜΠΑΝΑ // ΑΘΗΝΑ
+  pages: 230
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9602572337'
+  original_entry:
+    0: 17370
+    1: ΓΟΥΠΟΣ,ΘΕΟΔΩΡΟΣ
+    2: Η ΓΛΩΣΣΑ ΜΟΥ ΓΙΑ ΤΗΝ Α ΔΗΜΟΤΙΚΟΥ
+    4: 808.899ΓΟΥ
+    5: '20630'
+    8: ΕΚΔΟΣΕΙΣ ΚΑΜΠΑΝΑ
+    9: ΑΘΗΝΑ
+    11: '230'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    19: '9602572337'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17371
+  authors:
+  - ΓΙΑΝΣΣΟΝ,ΤΟΥΒΕ
+  title: ΤΟ ΚΑΠΕΛΟ ΤΟΥ ΜΑΓΟΥ ΜΟΥΜΕΡΛΙΝ
+  dewey: 808.899 ΓΙΑ
+  entry_numbers:
+  - '22700'
+  editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
+  pages: 174
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601646992'
+  original_entry:
+    0: 17371
+    1: ΓΙΑΝΣΣΟΝ,ΤΟΥΒΕ
+    2: ΤΟ ΚΑΠΕΛΟ ΤΟΥ ΜΑΓΟΥ ΜΟΥΜΕΡΛΙΝ
+    4: 808.899ΓΙΑ
+    5: '22700'
+    8: ΠΑΤΑΚΗ
+    9: ΑΘΗΝΑ
+    11: '174'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789601646'
+    19: '992'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17372
+  authors:
+  - ΓΕΩΡΓΟΣΤΑΘΗ,ΕΛΕΝΗ
+  title: ΧΑΘΗΚΕ Η ΜΠΑΛΑ
+  dewey: 808.899 ΓΕΩ
+  entry_numbers:
+  - '22597'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2017
+  pages: 105
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180118759'
+  original_entry:
+    0: 17372
+    1: ΓΕΩΡΓΟΣΤΑΘΗ,ΕΛΕΝΗ
+    2: ΧΑΘΗΚΕ Η ΜΠΑΛΑ
+    4: 808.899ΓΕΩ
+    5: '22597'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2017'
+    11: '105'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180118'
+    19: '759'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17373
+  authors:
+  - ΓΚΑΛΚΙΝΑ,ΑΝΑΣΤΑΣΙΑ
+  title: ΜΙΑ ΥΠΕΡΟΧΗ ΜΕΡΑ
+  dewey: 808.899 ΓΚΑ
+  entry_numbers:
+  - '22615'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  pages: 30
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17373
+    1: ΓΚΑΛΚΙΝΑ,ΑΝΑΣΤΑΣΙΑ
+    2: ΜΙΑ ΥΠΕΡΟΧΗ ΜΕΡΑ
+    4: 808.899ΓΚΑ
+    5: '22615'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    11: '30'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17374
+  authors:
+  - ΛΑΡΣΟΝ,ΟΣΑ
+  title: PAX ΤΟ ΑΒΑΠΤΙΣΤΟ
+  dewey: 808.899 ΛΑΡ
+  entry_numbers:
+  - '22601'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  pages: 205
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180119510'
+  original_entry:
+    0: 17374
+    1: ΛΑΡΣΟΝ,ΟΣΑ
+    2: PAX ΤΟ ΑΒΑΠΤΙΣΤΟ
+    4: 808.899ΛΑΡ
+    5: '22601'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    11: '205'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180119'
+    19: '510'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17375
+  authors:
+  - ΛΑΡΙ,Χ.Ι
+  title: ΨΗΦΙΑΚΟΙ ΕΙΣΒΟΛΕΙΣ
+  dewey: 808.899 ΛΑΡ
+  entry_numbers:
+  - '22603'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2013
+  pages: 105
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180108224'
+  original_entry:
+    0: 17375
+    1: ΛΑΡΙ,Χ.Ι
+    2: ΨΗΦΙΑΚΟΙ ΕΙΣΒΟΛΕΙΣ
+    4: 808.899ΛΑΡ
+    5: '22603'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2013'
+    11: '105'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180108'
+    19: '224'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17376
+  authors:
+  - ΛΙΝΤΓΚΡΕΝ,ΑΣΤΡΙΝΤ
+  title: ΣΚΑΝΤΑΛΙΕΣ ΣΤΟ ΜΙΚΡΟ ΧΩΡΙΟ
+  dewey: 808.899 ΛΙΝ
+  entry_numbers:
+  - '20418'
+  editor: ΜΕΤΟΠΗ // None
+  pages: 125
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17376
+    1: ΛΙΝΤΓΚΡΕΝ,ΑΣΤΡΙΝΤ
+    2: ΣΚΑΝΤΑΛΙΕΣ ΣΤΟ ΜΙΚΡΟ ΧΩΡΙΟ
+    4: 808.899ΛΙΝ
+    5: '20418'
+    8: ΜΕΤΟΠΗ
+    11: '125'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    9: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17377
+  authors:
+  - ΛΙΝΤΓΚΡΕΝ,ΑΣΤΡΙΝΤ
+  title: Η ΠΙΠΗ ΦΑΚΙΔΟΜΥΤΗ ΣΤΙΣ ΝΟΤΙΕΣ ΘΑΛΑΣΣΕΣ
+  dewey: 808.899 ΛΙΝ
+  entry_numbers:
+  - '22608'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 160
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180138696'
+  original_entry:
+    0: 17377
+    1: ΛΙΝΤΓΚΡΕΝ,ΑΣΤΡΙΝΤ
+    2: Η ΠΙΠΗ ΦΑΚΙΔΟΜΥΤΗ ΣΤΙΣ ΝΟΤΙΕΣ ΘΑΛΑΣΣΕΣ
+    4: 808.899ΛΙΝ
+    5: '22608'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '160'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180138'
+    19: '696'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17378
+  authors:
+  - ΜΑΛΟ,ΕΚΤΟΡΑΣ
+  title: ΧΩΡΙΣ ΟΙΚΟΓΕΝΕΙΑ
+  dewey: 808.899 ΜΑΛ
+  entry_numbers:
+  - '20637'
+  editor: ΣΠ. ΔΑΡΕΜΑ // ΑΘΗΝΑ
+  pages: 483
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17378
+    1: ΜΑΛΟ,ΕΚΤΟΡΑΣ
+    2: ΧΩΡΙΣ ΟΙΚΟΓΕΝΕΙΑ
+    4: 808.899ΜΑΛ
+    5: '20637'
+    8: ΣΠ. ΔΑΡΕΜΑ
+    9: ΑΘΗΝΑ
+    11: '483'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17379
+  authors:
+  - ΜΑΝΔΗΛΑΡΑΣ,ΦΙΛΙΠΠΟΣ
+  title: Ο ΠΑΠΠΟΥΣ ΜΑΣ ΑΦΗΣΕ
+  dewey: 808.899 ΜΑΝ
+  entry_numbers:
+  - '22697'
+  editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
+  pages: 56
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601628622'
+  original_entry:
+    0: 17379
+    1: ΜΑΝΔΗΛΑΡΑΣ,ΦΙΛΙΠΠΟΣ
+    2: Ο ΠΑΠΠΟΥΣ ΜΑΣ ΑΦΗΣΕ
+    4: 808.899ΜΑΝ
+    5: '22697'
+    8: ΠΑΤΑΚΗ
+    9: ΑΘΗΝΑ
+    11: '56'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789601628'
+    19: '622'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17380
+  authors:
+  - ΜΑΥΡΟΜΑΤΗΣ,ΘΩΜΑΣ
+  title: ΑΛΗΘΙΝΟΙ ΗΡΩΕΣ - ΗΡΩΕΣ ΤΟΥ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
+  dewey: 808.899 ΜΑΥ
+  entry_numbers:
+  - '21511'
+  editor: ΕΚΔΟΣΕΙΣ ΕΑΡ ΠΑΙΔΙΚΑ // ΑΘΗΝΑ
+  edition_year: 2022
+  pages: 15
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786185368951'
+  original_entry:
+    0: 17380
+    1: ΜΑΥΡΟΜΑΤΗΣ,ΘΩΜΑΣ
+    2: ΑΛΗΘΙΝΟΙ ΗΡΩΕΣ - ΗΡΩΕΣ ΤΟΥ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
+    4: 808.899ΜΑΥ
+    5: '21511'
+    8: ΕΚΔΟΣΕΙΣ ΕΑΡ ΠΑΙΔΙΚΑ
+    9: ΑΘΗΝΑ
+    10: '2022'
+    11: '15'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786185368'
+    19: '951'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17381
+  authors:
+  - ΜΙΛΑΝΙ,ΜΙΝΟ
+  title: ΣΑΝΤΑ ΑΛΕΓΚΡΑΝΤΣΑ
+  dewey: 808.899 ΜΙΛ
+  entry_numbers:
+  - '20421'
+  translators:
+  - ΤΡΟΠΑΙΤΗΣ,ΑΛΚΗΣ
+  editor: ΧΑΡΗ ΠΑΤΣΗ // ΑΘΗΝΑ
+  pages: 212
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17381
+    1: ΜΙΛΑΝΙ,ΜΙΝΟ
+    2: ΣΑΝΤΑ ΑΛΕΓΚΡΑΝΤΣΑ
+    4: 808.899ΜΙΛ
+    5: '20421'
+    6: ΑΛΚΗ ΤΡΟΠΑΙΤΗ
+    8: ΧΑΡΗ ΠΑΤΣΗ
+    9: ΑΘΗΝΑ
+    11: '212'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17382
+  authors:
+  - ΟΥΓΚΩ,ΒΙΚΤΩΡ
+  title: ΟΙ ΑΘΛΙΟΙ
+  dewey: 808.899 ΟΥΓ
+  entry_numbers:
+  - '19892'
+  editor: ΕΚΔΟΣΕΙΣ ΑΣΤΗΡ // ΑΘΗΝΑ
+  pages: 215
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17382
+    1: ΟΥΓΚΩ,ΒΙΚΤΩΡ
+    2: ΟΙ ΑΘΛΙΟΙ
+    4: 808.899ΟΥΓ
+    5: '19892'
+    8: ΕΚΔΟΣΕΙΣ ΑΣΤΗΡ
+    9: ΑΘΗΝΑ
+    11: '215'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17383
+  authors:
+  - ΟΥΓΚΩ,ΒΙΚΤΩΡ
+  title: Η ΠΑΝΑΓΙΑ ΤΩΝ ΠΑΡΙΣΙΩΝ
+  dewey: 808.899 ΟΥΓ
+  entry_numbers:
+  - '22806'
+  editor: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ // ΑΘΗΝΑ
+  pages: 128
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17383
+    1: ΟΥΓΚΩ,ΒΙΚΤΩΡ
+    2: Η ΠΑΝΑΓΙΑ ΤΩΝ ΠΑΡΙΣΙΩΝ
+    4: 808.899ΟΥΓ
+    5: '22806'
+    8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
+    9: ΑΘΗΝΑ
+    11: '128'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17384
+  authors:
+  - NOZIERE,JEAN-PAUL
+  title: ΕΚΔΙΚΗΣΗ ΤΙΤΟΣ
+  dewey: 808.899 NOZ
+  entry_numbers:
+  - '22681'
+  editor: Χ.Ε ΔΑΡΔΑΝΟΣ // ΑΘΗΝΑ
+  edition_year: 1998
+  pages: 180
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9603800465'
+  original_entry:
+    0: 17384
+    1: NOZIERE,JEAN-PAUL
+    2: ΕΚΔΙΚΗΣΗ ΤΙΤΟΣ
+    4: 808.899NOZ
+    5: '22681'
+    8: Χ.Ε ΔΑΡΔΑΝΟΣ
+    9: ΑΘΗΝΑ
+    10: '1998'
+    11: '180'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    19: '9603800465'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17385
+  authors:
+  - ΝΟΡΘΦΙΛΝΤ,ΓΚΑΡΙ
+  title: ΙΟΥΛΙΟΣ ΖΕΒΡΑ ΒΙΒΛΙΟ 2
+  dewey: 808.899 ΝΟΡ
+  entry_numbers:
+  - '22606'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2017
+  pages: 250
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180118698'
+  original_entry:
+    0: 17385
+    1: ΝΟΡΘΦΙΛΝΤ,ΓΚΑΡΙ
+    2: ΙΟΥΛΙΟΣ ΖΕΒΡΑ ΒΙΒΛΙΟ 2
+    4: 808.899ΝΟΡ
+    5: '22606'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2017'
+    11: '250'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180118'
+    19: '698'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17386
+  authors:
+  - ΝΟΡΘΦΙΛΝΤ,ΓΚΑΡΙ
+  title: ΙΟΥΛΙΟΣ ΖΕΒΡΑ ΒΙΒΛΙΟ 3
+  dewey: 808.899 ΝΟΡ
+  entry_numbers:
+  - '22607'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2018
+  pages: 300
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180125177'
+  original_entry:
+    0: 17386
+    1: ΝΟΡΘΦΙΛΝΤ,ΓΚΑΡΙ
+    2: ΙΟΥΛΙΟΣ ΖΕΒΡΑ ΒΙΒΛΙΟ 3
+    4: 808.899ΝΟΡ
+    5: '22607'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2018'
+    11: '300'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180125'
+    19: '177'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17387
+  authors: []
+  title: Η ΜΑΓΕΜΕΝΗ ΒΑΣΙΛΟΠΟΥΛΑ
+  dewey: 808.899 ΧΣ
+  entry_numbers:
+  - '22808'
+  editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
+  pages: 20
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9602343060'
+  original_entry:
+    0: 17387
+    1: Χ.Σ
+    2: Η ΜΑΓΕΜΕΝΗ ΒΑΣΙΛΟΠΟΥΛΑ
+    4: 808.899Χ.Σ
+    5: '22808'
+    8: ΑΓΚΥΡΑ
+    9: ΑΘΗΝΑ
+    11: '20'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9602343060'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17388
+  authors:
+  - ΤΣΙΜΙΚΑΛΗ,ΠΙΠΙΝΑ
+  title: ΤΟ ΚΑΛΟΚΑΙΡΑΚΙ - ΠΑΙΖΩ ΚΑΙ ΜΑΘΑΙΝΩ
+  dewey: 808.899 ΤΣΙ
+  entry_numbers:
+  - '22807'
+  editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
+  pages: 20
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9602343052'
+  original_entry:
+    0: 17388
+    1: ΤΣΙΜΙΚΑΛΗ,ΠΙΠΙΝΑ
+    2: ΤΟ ΚΑΛΟΚΑΙΡΑΚΙ - ΠΑΙΖΩ ΚΑΙ ΜΑΘΑΙΝΩ
+    4: 808.899ΤΣΙ
+    5: '22807'
+    8: ΑΓΚΥΡΑ
+    9: ΑΘΗΝΑ
+    11: '20'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9602343052'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17389
+  authors:
+  - ΝΤΙΞΟΝ,ΦΡΑΝΚΛΙΝ
+  title: ΟΙ ΓΙΓΑΝΤΕΣ ΤΗΣ ΕΡΗΜΟΥ
+  dewey: 808.899 ΝΤΙ
+  entry_numbers:
+  - '22809'
+  editor: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ // ΑΘΗΝΑ
+  pages: 170
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17389
+    1: ΝΤΙΞΟΝ,ΦΡΑΝΚΛΙΝ
+    2: ΟΙ ΓΙΓΑΝΤΕΣ ΤΗΣ ΕΡΗΜΟΥ
+    4: 808.899ΝΤΙ
+    5: '22809'
+    8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
+    9: ΑΘΗΝΑ
+    11: '170'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17390
+  authors:
+  - ΟΥΑΛΙΑΜΣ,ΝΤΕΙΒΙΝΤ
+  title: Ο ΧΛΑΠΑΤΣΑ
+  dewey: 808.899 ΟΥΑ
+  entry_numbers:
+  - '22598'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2022
+  pages: 325
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180141986'
+  original_entry:
+    0: 17390
+    1: ΟΥΑΛΙΑΜΣ,ΝΤΕΙΒΙΝΤ
+    2: Ο ΧΛΑΠΑΤΣΑ
+    4: 808.899ΟΥΑ
+    5: '22598'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2022'
+    11: '325'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180141'
+    19: '986'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17391
+  authors:
+  - ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+  title: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΤΑΛΑΝΤΟΥΧΑ ΠΟΠ ΣΤΑΡ
+  dewey: 808.899 ΡΑΣ
+  entry_numbers:
+  - '22577'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2011
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604964079'
+  original_entry:
+    0: 17391
+    1: ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+    2: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΤΑΛΑΝΤΟΥΧΑ ΠΟΠ ΣΤΑΡ
+    4: 808.899ΡΑΣ
+    5: '22577'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2011'
+    11: 320ΠΑΙ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789604964'
+    19: 079
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17392
+  authors:
+  - ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+  title: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΧΑΡΟΥΜΕΝΗ ΚΑΡΔΙΟΚΑΤΑΚΤΗΤΡΙΑ
+  dewey: 808.899 ΡΑΣ
+  entry_numbers:
+  - '22578'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2013
+  pages: 350
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180103922'
+  original_entry:
+    0: 17392
+    1: ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+    2: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΧΑΡΟΥΜΕΝΗ ΚΑΡΔΙΟΚΑΤΑΚΤΗΤΡΙΑ
+    4: 808.899ΡΑΣ
+    5: '22578'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2013'
+    11: '350'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180103'
+    19: '922'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17393
+  authors:
+  - ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+  title: ΦΤΙΑΞΕ ΤΟ ΔΙΚΟ ΣΟΥ ΞΕΝΕΡΩΤΟ ΗΜΕΡΟΛΟΓΙΟ
+  dewey: 808.899 ΡΑΣ
+  entry_numbers:
+  - '22575'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2011
+  pages: 350
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604968930'
+  original_entry:
+    0: 17393
+    1: ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+    2: ΦΤΙΑΞΕ ΤΟ ΔΙΚΟ ΣΟΥ ΞΕΝΕΡΩΤΟ ΗΜΕΡΟΛΟΓΙΟ
+    4: 808.899ΡΑΣ
+    5: '22575'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2011'
+    11: '350'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789604968'
+    19: '930'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17394
+  authors:
+  - ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+  title: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΛΑΜΠΕΡΗ TV STAR
+  dewey: 808.899 ΡΑΣ
+  entry_numbers:
+  - '22576'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2014
+  pages: 350
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180108118'
+  original_entry:
+    0: 17394
+    1: ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+    2: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΛΑΜΠΕΡΗ TV STAR
+    4: 808.899ΡΑΣ
+    5: '22576'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2014'
+    11: '350'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180108'
+    19: '118'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17395
+  authors:
+  - ΕΞΥΠΕΡΥ,ΑΝΤΟΥΑΝ
+  title: Ο ΜΙΚΡΟΣ ΠΡΙΓΚΙΠΑΣ
+  dewey: 808.899 ΕΞΥ
+  entry_numbers:
+  - '22815'
+  editor: ΝΕΦΕΛΗ // ΑΘΗΝΑ
+  edition_year: 1984
+  pages: 97
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17395
+    1: ΕΞΥΠΕΡΥ,ΑΝΤΟΥΑΝ
+    2: Ο ΜΙΚΡΟΣ ΠΡΙΓΚΙΠΑΣ
+    4: 808.899ΕΞΥ
+    5: '22815'
+    8: ΝΕΦΕΛΗ
+    9: ΑΘΗΝΑ
+    10: '1984'
+    11: '97'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17396
+  authors:
+  - ΣΑΡΗ,ΖΩΡΖ
+  title: Ε.Π
+  dewey: 808.899 ΣΑΡ
+  entry_numbers:
+  - '22814'
+  editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
+  edition_year: 1995
+  pages: 254
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9603605115'
+  original_entry:
+    0: 17396
+    1: ΣΑΡΗ,ΖΩΡΖ
+    2: Ε.Π
+    4: 808.899ΣΑΡ
+    5: '22814'
+    8: ΠΑΤΑΚΗ
+    9: ΑΘΗΝΑ
+    10: '1995'
+    11: '254'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9603605115'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17397
+  authors:
+  - ΣΑΡΗ,ΖΩΡΖ
+  title: ΤΟ ΨΕΜΑ
+  dewey: 808.899 ΣΑΡ
+  entry_numbers:
+  - '22813'
+  editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
+  edition_year: 1987
+  pages: 144
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9600400660'
+  original_entry:
+    0: 17397
+    1: ΣΑΡΗ,ΖΩΡΖ
+    2: ΤΟ ΨΕΜΑ
+    4: 808.899ΣΑΡ
+    5: '22813'
+    8: ΚΕΔΡΟΣ
+    9: ΑΘΗΝΑ
+    10: '1987'
+    11: '144'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9600400660'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17398
+  authors:
+  - ΣΑΡΗ,ΖΩΡΖ
+  title: ΤΟ ΠΑΡΑΡΑΔΙΑΣΜΑ
+  dewey: 808.899 ΣΑΡ
+  entry_numbers:
+  - '22812'
+  editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
+  edition_year: 1989
+  pages: 205
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9602934778'
+  original_entry:
+    0: 17398
+    1: ΣΑΡΗ,ΖΩΡΖ
+    2: ΤΟ ΠΑΡΑΡΑΔΙΑΣΜΑ
+    4: 808.899ΣΑΡ
+    5: '22812'
+    8: ΠΑΤΑΚΗ
+    9: ΑΘΗΝΑ
+    10: '1989'
+    11: '205'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9602934778'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17399
+  authors:
+  - ΣΕΡΕΦΑΣ,ΣΑΚΗΣ
+  title: ΠΩΛΟΥΝΤΑΙ ΣΚΙΕΣ
+  dewey: 808.899 ΣΕΡ
+  entry_numbers:
+  - '22691'
+  editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
+  pages: 40
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601638478'
+  original_entry:
+    0: 17399
+    1: ΣΕΡΕΦΑΣ,ΣΑΚΗΣ
+    2: ΠΩΛΟΥΝΤΑΙ ΣΚΙΕΣ
+    4: 808.899ΣΕΡ
+    5: '22691'
+    8: ΠΑΤΑΚΗ
+    9: ΑΘΗΝΑ
+    11: '40'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789601638'
+    19: '478'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17400
+  authors:
+  - ΣΙΝΟΥ,ΚΙΡΑ
+  title: ΤΟ ΤΕΛΟΣ ΤΩΝ ΤΕΡΑΤΩΝ
+  dewey: 808.899 ΣΙΝ
+  entry_numbers:
+  - '22811'
+  editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
+  edition_year: 1987
+  pages: 160
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9600402868'
+  original_entry:
+    0: 17400
+    1: ΣΙΝΟΥ,ΚΙΡΑ
+    2: ΤΟ ΤΕΛΟΣ ΤΩΝ ΤΕΡΑΤΩΝ
+    4: 808.899ΣΙΝ
+    5: '22811'
+    8: ΚΕΔΡΟΣ
+    9: ΑΘΗΝΑ
+    10: '1987'
+    11: '160'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9600402868'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17401
+  authors:
+  - ΣΠΙΡΙ,ΓΙΟΧΑΝΑ
+  title: ΧΑΙΝΤΙ
+  dewey: 808.899 ΣΠΙ
+  entry_numbers:
+  - '22810'
+  editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
+  pages: 48
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604750788'
+  original_entry:
+    0: 17401
+    1: ΣΠΙΡΙ,ΓΙΟΧΑΝΑ
+    2: ΧΑΙΝΤΙ
+    4: 808.899ΣΠΙ
+    5: '22810'
+    8: ΚΑΘΗΜΕΡΙΝΗ
+    9: ΑΘΗΝΑ
+    11: '48'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789604750'
+    19: '788'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17402
+  authors:
+  - ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+  title: ΑΥΡΙΟ ΕΙΝΑΙ ΚΥΡΙΑΚΗ
+  dewey: 808.899 ΣΟΥ
+  entry_numbers:
+  - '17875'
+  editor: ΝΕΟΙ ΑΚΡΙΤΕΣ // ΑΘΗΝΑ
+  edition_year: 1999
+  pages: 56
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9607006933'
+  original_entry:
+    0: 17402
+    1: ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+    2: ΑΥΡΙΟ ΕΙΝΑΙ ΚΥΡΙΑΚΗ
+    4: 808.899ΣΟΥ
+    5: '17875'
+    8: ΝΕΟΙ ΑΚΡΙΤΕΣ
+    9: ΑΘΗΝΑ
+    10: '1999'
+    11: '56'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9607006933'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17403
+  authors:
+  - ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+  title: Ο ΜΕΓΑΛΟΣ ΑΠΟΧΑΙΡΕΤΙΣΜΟΣ
+  dewey: 808.899 ΣΟΥ
+  entry_numbers:
+  - '22596'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2021
+  pages: 190
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789607021854'
+  original_entry:
+    0: 17403
+    1: ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+    2: Ο ΜΕΓΑΛΟΣ ΑΠΟΧΑΙΡΕΤΙΣΜΟΣ
+    4: 808.899ΣΟΥ
+    5: '22596'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2021'
+    11: '190'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789607021'
+    19: '854'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17404
+  authors:
+  - ΣΟΦΟΚΛΗ
+  title: ΟΙΔΙΠΟΥΣ ΤΥΡΑΝΝΟΣ
+  dewey: 808.899 ΣΟΦ
+  entry_numbers:
+  - '19984'
+  editor: ΣΑΒΒΑΛΑΣ // ΑΘΗΝΑ
+  edition_year: 2012
+  pages: 55
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9604609734'
+  original_entry:
+    0: 17404
+    1: ΣΟΦΟΚΛΗ
+    2: ΟΙΔΙΠΟΥΣ ΤΥΡΑΝΝΟΣ
+    4: 808.899ΣΟΦ
+    5: '19984'
+    8: ΣΑΒΒΑΛΑΣ
+    9: ΑΘΗΝΑ
+    10: '2012'
+    11: '55'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9604609734'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17405
+  authors:
+  - ΣΤΑΝΤΛΕΡ,ΑΛΕΞΑΝΤΕΡ
+  title: ΤΖΟΥΛΙΑΝ ΡΟΝΤΡΙΓΚΕΖ
+  dewey: 808.899 ΣΤΑ
+  entry_numbers:
+  - '22690'
+  editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
+  pages: 140
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17405
+    1: ΣΤΑΝΤΛΕΡ,ΑΛΕΞΑΝΤΕΡ
+    2: ΤΖΟΥΛΙΑΝ ΡΟΝΤΡΙΓΚΕΖ
+    4: 808.899ΣΤΑ
+    5: '22690'
+    8: ΠΑΤΑΚΗ
+    9: ΑΘΗΝΑ
+    11: '140'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17406
+  authors:
+  - ΣΤΟΟΥ-ΜΠΙΤΣΕΡ,ΧΑΡΙΕΤ
+  title: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+  dewey: 808.899 ΣΤΟ
+  entry_numbers:
+  - '20973'
+  editor: ΤΑ ΝΕΑ // ΑΘΗΝΑ
+  edition_year: 2018
+  pages: 225
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789605039554'
+  original_entry:
+    0: 17406
+    1: ΣΤΟΟΥ-ΜΠΙΤΣΕΡ,ΧΑΡΙΕΤ
+    2: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+    4: 808.899ΣΤΟ
+    5: '20973'
+    8: ΤΑ ΝΕΑ
+    9: ΑΘΗΝΑ
+    10: '2018'
+    11: '225'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789605039'
+    19: '554'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17407
+  authors:
+  - ΣΤΟΟΥ,ΜΠΗΤΣΕΡ
+  title: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+  dewey: 808.899 ΣΤΟ
+  entry_numbers:
+  - '20640'
+  editor: ΠΑΓΚΟΣΜΙΑ ΛΟΓΟΤΕΧΝΙΑ // ΑΘΗΝΑ
+  pages: 125
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17407
+    1: ΣΤΟΟΥ,ΜΠΗΤΣΕΡ
+    2: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+    4: 808.899ΣΤΟ
+    5: '20640'
+    8: ΠΑΓΚΟΣΜΙΑ ΛΟΓΟΤΕΧΝΙΑ
+    9: ΑΘΗΝΑ
+    11: '125'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17408
+  authors:
+  - ΣΤΡΑΤΟΛΑΤΗ-ΝΙΚΗΤΑ,ΧΡ.
+  title: ΤΑ ΜΑΤΙΑ ΤΗΣ ΜΑΝΑΣ
+  dewey: 808.899 ΣΤΡ
+  entry_numbers:
+  - '16257'
+  editor: ΑΛΚΑΙΟΣ // ΑΘΗΝΑ
+  pages: 149
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17408
+    1: ΣΤΡΑΤΟΛΑΤΗ-ΝΙΚΗΤΑ,ΧΡ.
+    2: ΤΑ ΜΑΤΙΑ ΤΗΣ ΜΑΝΑΣ
+    4: 808.899ΣΤΡ
+    5: '16257'
+    8: ΑΛΚΑΙΟΣ
+    9: ΑΘΗΝΑ
+    11: 149Σ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17409
+  authors:
+  - ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+  title: ΦΟΥΡΦΟΥΡΗΣ Ο ΚΟΤΣΥΦΑΣ
+  dewey: 808.899 ΣΟΥ
+  entry_numbers:
+  - '22740'
+  edition: '9'
+  editor: ΠΑΤΑΚΗΣ // ΑΘΗΝΑ
+  edition_year: 1999
+  pages: 72
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  - ΠΙΑΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9603602051'
+  original_entry:
+    0: 17409
+    1: ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+    2: ΦΟΥΡΦΟΥΡΗΣ Ο ΚΟΤΣΥΦΑΣ
+    4: 808.899ΣΟΥ
+    5: '22740'
+    7: 9Η
+    8: ΠΑΤΑΚΗΣ
+    9: ΑΘΗΝΑ
+    10: '1999'
+    11: '72'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΙΑΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    19: '9603602051'
+    3: null
+    6: null
+    15: null
+    16: null
+    17: null
+    18: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17410
+  authors:
+  - ΤΡΙΑΝΤΑΦΥΛΛΟΥ,ΣΩΤΗ
+  title: Η ΜΙΛΕΝΑ ΚΑΙ ΤΟ ΦΡΙΚΤΟ ΨΑΡΙ
+  dewey: 808.899 ΤΡΙ
+  entry_numbers:
+  - '22702'
+  edition: '1'
+  editor: ΠΑΤΑΚΗΣ // ΑΘΗΝΑ
+  edition_year: 2011
+  pages: 25
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601640266'
+  original_entry:
+    0: 17410
+    1: ΤΡΙΑΝΤΑΦΥΛΛΟΥ,ΣΩΤΗ
+    2: Η ΜΙΛΕΝΑ ΚΑΙ ΤΟ ΦΡΙΚΤΟ ΨΑΡΙ
+    4: 808.899ΤΡΙ
+    5: '22702'
+    7: 1Η
+    8: ΠΑΤΑΚΗΣ
+    9: ΑΘΗΝΑ
+    10: '2011'
+    11: '25'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789601640'
+    19: '266'
+    3: null
+    6: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17411
+  authors:
+  - ΛΑΓΟΥ-ΠΑΠΑΚΟΥ,ΑΥΓΗ
+  title: ΟΙ ΘΑΥΜΑΣΙΕΣ ΗΛΙΑΧΤΙΔΕΣ
+  dewey: 808.899 ΛΑΓ
+  entry_numbers:
+  - '20645'
+  edition: '3'
+  editor: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ // ΑΘΗΝΑ
+  edition_year: 1983
+  pages: 47
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17411
+    1: ΛΑΓΟΥ-ΠΑΠΑΚΟΥ,ΑΥΓΗ
+    2: ΟΙ ΘΑΥΜΑΣΙΕΣ ΗΛΙΑΧΤΙΔΕΣ
+    4: 808.899ΛΑΓ
+    5: '20645'
+    7: 3Η
+    8: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ
+    9: ΑΘΗΝΑ
+    10: '1983'
+    11: '47'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17412
+  authors:
+  - ΠΑΠΑΔΙΑΜΑΝΤΗΣ
+  title: ΠΑΙΔΙΚΑ ΔΙΗΓΗΜΑΤΑ
+  dewey: 808.899 ΠΑΠ
+  entry_numbers:
+  - '20631'
+  translators:
+  - ΑΘΑΝ.ΘΕΟΔΩΡΑΚΗ
+  editor: ΖΑΝΑΚΗ // ΑΘΗΝΑ
+  pages: 188
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17412
+    1: ΠΑΠΑΔΙΑΜΑΝΤΗΣ
+    2: ΠΑΙΔΙΚΑ ΔΙΗΓΗΜΑΤΑ
+    4: 808.899ΠΑΠ
+    5: '20631'
+    6: ΑΘΑΝ.ΘΕΟΔΩΡΑΚΗ
+    8: ΖΑΝΑΚΗ
+    9: ΑΘΗΝΑ
+    11: '188'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17413
+  authors:
+  - ΠΑΣΧΟΥ,ΒΑΣΙΛΗ
+  title: ΠΡΩΤΟΠΟΡΟΙ ΣΤΟ ΔΙΑΣΤΗΜΑ
+  dewey: 808.899 ΠΑΣ
+  entry_numbers:
+  - '20424'
+  editor: ΦΙΛΟΛΟΓΙΚΗ // ΑΘΗΝΑ
+  pages: 196
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17413
+    1: ΠΑΣΧΟΥ,ΒΑΣΙΛΗ
+    2: ΠΡΩΤΟΠΟΡΟΙ ΣΤΟ ΔΙΑΣΤΗΜΑ
+    4: 808.899ΠΑΣ
+    5: '20424'
+    8: ΦΙΛΟΛΟΓΙΚΗ
+    9: ΑΘΗΝΑ
+    11: '196'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17414
+  authors:
+  - ΠΕΡΩ,ΣΟΥΖΑΝΑ
+  title: Η ΕΚΔΙΚΗΣΗ ΤΟΥ ΡΟΜΠΕΝ
+  dewey: 808.899 ΠΕΡ
+  entry_numbers:
+  - '20422'
+  translators:
+  - ΑΡΓΥΡΟΠΟΥΛΟΥ,ΟΘ.
+  editor: ΧΑΡΗ ΠΑΤΣΗ // ΑΘΗΝΑ
+  edition_year: 1967
+  pages: 199
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  donors:
+  - ΚΑΓΚΑΡΑΣ,ΕΥΣΤΑΘΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17414
+    1: ΠΕΡΩ,ΣΟΥΖΑΝΑ
+    2: Η ΕΚΔΙΚΗΣΗ ΤΟΥ ΡΟΜΠΕΝ
+    4: 808.899ΠΕΡ
+    5: '20422'
+    6: ΟΘ.ΑΡΓΥΡΟΠΟΥΛΟΥ
+    8: ΧΑΡΗ ΠΑΤΣΗ
+    9: ΑΘΗΝΑ
+    10: '1967'
+    11: '199'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΕΥΣΤΑΘΙΟΣ ΚΑΓΚΑΡΑΣ
+    3: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17415
+  authors: []
+  entry_numbers: []
+  topics: []
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17415
+    1: null
+    2: null
+    3: null
+    4: null
+    5: null
+    6: null
+    7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17416
+  authors:
+  - DAHL,ROALD
+  title: ΝΤΑΝΙ,Ο ΠΡΩΤΑΘΛΗΤΗΣ ΤΟΥ ΚΟΣΜΟΥ
+  dewey: 808.899 DAH
+  entry_numbers:
+  - '22592'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 250
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180137248'
+  original_entry:
+    0: 17416
+    1: DAHL,ROALD
+    2: ΝΤΑΝΙ,Ο ΠΡΩΤΑΘΛΗΤΗΣ ΤΟΥ ΚΟΣΜΟΥ
+    4: 808.899DAH
+    5: '22592'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '250'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180137'
+    19: '248'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17417
+  authors:
+  - DAHL,ROALD
+  title: Ο ΤΖΙΜΗΣ ΚΑΙ ΤΟ ΓΙΓΑΝΤΟΡΟΔΑΚΙΝΟ
+  dewey: 808.899 DAH
+  entry_numbers:
+  - '22591'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 200
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180137255'
+  original_entry:
+    0: 17417
+    1: DAHL,ROALD
+    2: Ο ΤΖΙΜΗΣ ΚΑΙ ΤΟ ΓΙΓΑΝΤΟΡΟΔΑΚΙΝΟ
+    4: 808.899DAH
+    5: '22591'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '200'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180137'
+    19: '255'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17418
+  authors:
+  - DAHL,ROALD
+  title: ΜΑΤΙΛΝΤΑ
+  dewey: 808.899 DAH
+  entry_numbers:
+  - '22590'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 280
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180137224'
+  original_entry:
+    0: 17418
+    1: DAHL,ROALD
+    2: ΜΑΤΙΛΝΤΑ
+    4: 808.899DAH
+    5: '22590'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '280'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180137'
+    19: '224'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17419
+  authors:
+  - DAHL,ROALD
+  title: Ο ΤΣΑΡΛΙ ΚΑΙ ΤΟ ΕΡΓΟΣΤΑΣΙΟ ΣΟΚΟΛΑΤΑΣ
+  dewey: 808.899 DAH
+  entry_numbers:
+  - '22589'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 210
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180137309'
+  original_entry:
+    0: 17419
+    1: DAHL,ROALD
+    2: Ο ΤΣΑΡΛΙ ΚΑΙ ΤΟ ΕΡΓΟΣΤΑΣΙΟ ΣΟΚΟΛΑΤΑΣ
+    4: 808.899DAH
+    5: '22589'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '210'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180137'
+    19: '309'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17420
+  authors:
+  - DAHL,ROALD
+  title: Ο ΑΠΙΘΑΝΟΣ ΚΥΡΙΟΣ ΦΟΞ
+  dewey: 808.899 DAH
+  entry_numbers:
+  - '22588'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 95
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180137231'
+  original_entry:
+    0: 17420
+    1: DAHL,ROALD
+    2: Ο ΑΠΙΘΑΝΟΣ ΚΥΡΙΟΣ ΦΟΞ
+    4: 808.899DAH
+    5: '22588'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '95'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180137'
+    19: '231'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17421
+  authors:
+  - DAHL,ROALD
+  title: ΟΙ ΜΑΓΙΣΣΕΣ
+  dewey: 808.899 DAH
+  entry_numbers:
+  - '22587'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 240
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180137262'
+  original_entry:
+    0: 17421
+    1: DAHL,ROALD
+    2: ΟΙ ΜΑΓΙΣΣΕΣ
+    4: 808.899DAH
+    5: '22587'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '240'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180137'
+    19: '262'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17422
+  authors:
+  - DAHL,ROALD
+  title: ΟΙ ΒΛΑΚΕΝΤΙΟΙ
+  dewey: 808.899 DAH
+  entry_numbers:
+  - '22586'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2020
+  pages: 115
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180137286'
+  original_entry:
+    0: 17422
+    1: DAHL,ROALD
+    2: ΟΙ ΒΛΑΚΕΝΤΙΟΙ
+    4: 808.899DAH
+    5: '22586'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2020'
+    11: '115'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180137'
+    19: '286'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17423
+  authors:
+  - ΤΣΙΑΛΤΑ,ΕΛΕΝΗ
+  title: ΕΝΑ ΚΟΥΒΑΡΙ ΜΥΣΤΙΚΑ
+  dewey: 808.899 ΤΣΙ
+  entry_numbers:
+  - '22595'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2015
+  pages: 75
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180109306'
+  original_entry:
+    0: 17423
+    1: ΤΣΙΑΛΤΑ,ΕΛΕΝΗ
+    2: ΕΝΑ ΚΟΥΒΑΡΙ ΜΥΣΤΙΚΑ
+    4: 808.899ΤΣΙ
+    5: '22595'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2015'
+    11: '75'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180109'
+    19: '306'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17424
+  authors:
+  - ΤΣΙΛΙΜΕΝΗ,ΤΑΣΟΥΛΑ
+  title: Η ΑΠΑΓΩΓΗ ΤΗΣ ΜΟΒ ΓΡΑΒΑΤΑΣ
+  dewey: 808.899 ΤΣΙ
+  entry_numbers:
+  - '19940'
+  editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
+  edition_year: 2006
+  pages: 50
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17424
+    1: ΤΣΙΛΙΜΕΝΗ,ΤΑΣΟΥΛΑ
+    2: Η ΑΠΑΓΩΓΗ ΤΗΣ ΜΟΒ ΓΡΑΒΑΤΑΣ
+    4: 808.899ΤΣΙ
+    5: '19940'
+    8: ΚΕΔΡΟΣ
+    9: ΑΘΗΝΑ
+    10: '2006'
+    11: '50'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: 960043333Χ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17425
+  authors:
+  - ΧΙΝΤΛΕΥ,ΚΕΙΤ
+  title: ΟΔΟΣ ΧΑΡΑΣ - Η ΜΠΟΥΓΑΤΣΑ ΠΟΥ ΠΕΤΑΕΙ!
+  dewey: 808.899 ΧΙΤ
+  entry_numbers:
+  - '22621'
+  editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
+  pages: 20
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601699790'
+  original_entry:
+    0: 17425
+    1: ΧΙΝΤΛΕΥ,ΚΕΙΤ
+    2: ΟΔΟΣ ΧΑΡΑΣ - Η ΜΠΟΥΓΑΤΣΑ ΠΟΥ ΠΕΤΑΕΙ!
+    4: 808.899ΧΙΤ
+    5: '22621'
+    8: ΠΑΤΑΚΗ
+    9: ΑΘΗΝΑ
+    11: '20'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789601699'
+    19: '790'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17426
+  authors:
+  - ΧΙΤΣΚΟΚ,ΑΛΦΡΕΝΤ
+  title: ΜΥΣΤΗΡΙΟ ΤΗΣ ΚΛΕΜΜΕΝΗΣ ΦΑΛΑΙΝΑΣ
+  dewey: 808.899 ΧΙΤ
+  entry_numbers:
+  - '20089'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 1992
+  pages: 190
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9602740272'
+  original_entry:
+    0: 17426
+    1: ΧΙΤΣΚΟΚ,ΑΛΦΡΕΝΤ
+    2: ΜΥΣΤΗΡΙΟ ΤΗΣ ΚΛΕΜΜΕΝΗΣ ΦΑΛΑΙΝΑΣ
+    4: 808.899ΧΙΤ
+    5: '20089'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '1992'
+    11: '190'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9602740272'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17427
+  authors:
+  - ΧΟΡΤΙΑΤΗ,ΘΕΤΗ
+  title: Ο ΚΟΚΚΙΝΟΣ ΚΑΚΤΟΣ
+  dewey: 808.899 ΧΟΡ
+  entry_numbers:
+  - '22818'
+  editor: ΠΕΡΙΠΛΟΥΣ // ΑΘΗΝΑ
+  edition_year: 2000
+  pages: 95
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9608151422'
+  original_entry:
+    0: 17427
+    1: ΧΟΡΤΙΑΤΗ,ΘΕΤΗ
+    2: Ο ΚΟΚΚΙΝΟΣ ΚΑΚΤΟΣ
+    4: 808.899ΧΟΡ
+    5: '22818'
+    8: ΠΕΡΙΠΛΟΥΣ
+    9: ΑΘΗΝΑ
+    10: '2000'
+    11: '95'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9608151422'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17428
+  authors:
+  - COLEMAN,MICHAEL
+  title: ΣΦΑΛΜΑ ΣΥΣΤΗΜΑΤΟΣ
+  dewey: 808.899 COL
+  entry_numbers:
+  - '22689'
+  editor: ΜΕΤΑΙΧΜΙΟ ΠΑΙΔΙΚΟ // ΑΘΗΝΑ
+  edition_year: 2002
+  pages: 152
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9603753548'
+  original_entry:
+    0: 17428
+    1: COLEMAN,MICHAEL
+    2: ΣΦΑΛΜΑ ΣΥΣΤΗΜΑΤΟΣ
+    4: 808.899COL
+    5: '22689'
+    8: ΜΕΤΑΙΧΜΙΟ ΠΑΙΔΙΚΟ
+    9: ΑΘΗΝΑ
+    10: '2002'
+    11: '152'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9603753548'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17429
+  authors:
+  - DETHISE,JEANNE
+  title: ΤΟ ΔΕΛΦΙΝΙ ΤΟΥ ΓΙΩΡΓΑΚΗ
+  dewey: 808.899 DET
+  entry_numbers:
+  - '17872'
+  editor: ΠΑΠΑΔΟΠΟΥΛΟΣ // ΑΘΗΝΑ
+  pages: 22
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17429
+    1: DETHISE,JEANNE
+    2: ΤΟ ΔΕΛΦΙΝΙ ΤΟΥ ΓΙΩΡΓΑΚΗ
+    4: 808.899DET
+    5: '17872'
+    8: ΠΑΠΑΔΟΠΟΥΛΟΣ
+    9: ΑΘΗΝΑ
+    11: '22'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17430
+  authors:
+  - LEGO
+  title: ΣΤΟΝ ΠΥΡΟΣΒΕΣΤΙΚΟ ΣΤΑΘΜΟ LEGO CITY
+  dewey: 808.899 LEG
+  entry_numbers:
+  - '22620'
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  pages: 10
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180141351'
+  original_entry:
+    0: 17430
+    1: LEGO
+    2: ΣΤΟΝ ΠΥΡΟΣΒΕΣΤΙΚΟ ΣΤΑΘΜΟ LEGO CITY
+    4: 808.899LEG
+    5: '22620'
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    11: '10'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9786180141'
+    19: '351'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17431
+  authors:
+  - MILLER,FRANK
+  title: BATMAN Ο ΣΚΟΤΕΙΝΟΣ ΙΠΠΟΤΗΣ ΕΠΙΣΤΡΕΦΕΙ
+  dewey: 808.899 MIL
+  entry_numbers:
+  - '22817'
+  editor: ANUBIS // ΑΘΗΝΑ
+  edition_year: 2008
+  pages: 200
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789603066729'
+  original_entry:
+    0: 17431
+    1: MILLER,FRANK
+    2: BATMAN Ο ΣΚΟΤΕΙΝΟΣ ΙΠΠΟΤΗΣ ΕΠΙΣΤΡΕΦΕΙ
+    4: 808.899MIL
+    5: '22817'
+    8: ANUBIS
+    9: ΑΘΗΝΑ
+    10: '2008'
+    11: '200'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789603066'
+    19: '729'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17432
+  authors:
+  - EXUPERY,ANTOINE
+  title: Ο ΜΙΚΡΟΣ ΠΡΙΓΚΙΠΑΣ
+  dewey: 808.899 EXU
+  entry_numbers:
+  - '19464'
+  editor: ΠΕΡΙΒΟΛΑΚΙ // ΑΘΗΝΑ
+  pages: 80
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9607412648'
+  original_entry:
+    0: 17432
+    1: EXUPERY,ANTOINE
+    2: Ο ΜΙΚΡΟΣ ΠΡΙΓΚΙΠΑΣ
+    4: 808.899EXU
+    5: '19464'
+    8: ΠΕΡΙΒΟΛΑΚΙ
+    9: ΑΘΗΝΑ
+    11: '80'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9607412648'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17433
+  authors:
+  - DUMAS,ALEXANDRE
+  title: ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+  dewey: 808.899 DUM
+  entry_numbers:
+  - '22816'
+  editor: ΑΛΚΥΩΝ // ΑΘΗΝΑ
+  edition_year: 2004
+  pages: 260
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9603260967'
+  original_entry:
+    0: 17433
+    1: DUMAS,ALEXANDRE
+    2: ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+    4: 808.899DUM
+    5: '22816'
+    8: ΑΛΚΥΩΝ
+    9: ΑΘΗΝΑ
+    10: '2004'
+    11: '260'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9603260967'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17434
+  authors:
+  - STAHL,P.G
+  title: ΤΑ ΑΣΗΜΕΝΙΑ ΠΑΓΟΠΕΔΙΛΑ
+  dewey: 808.899 STA
+  entry_numbers:
+  - '20688'
+  editor: ΑΓΚΥΡΑ ΠΑΙΔΙΚΑ // ΑΘΗΝΑ
+  pages: 120
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17434
+    1: STAHL,P.G
+    2: ΤΑ ΑΣΗΜΕΝΙΑ ΠΑΓΟΠΕΔΙΛΑ
+    4: 808.899STA
+    5: '20688'
+    8: ΑΓΚΥΡΑ ΠΑΙΔΙΚΑ
+    9: ΑΘΗΝΑ
+    11: '120'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17435
+  authors: []
+  entry_numbers: []
+  topics: []
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17435
+    1: null
+    2: null
+    3: null
+    4: null
+    5: null
+    6: null
+    7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17436
+  authors:
+  - ΚΑΛΑΤΖΟΠΟΥΛΟΣ,ΓΙΑΝΝΗΣ
+  title: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ ΚΑΙ ... ΕΞΥΠΝΟΥΣ ΜΕΓΑΛΟΥΣ
+  dewey: 886.2 ΚΑΛ
+  entry_numbers:
+  - 22839,22840
+  editor: ΦΙΛΝΤΙΣΙ // ΑΘΗΝΑ
+  edition_year: 2021
+  pages: 335
+  topics:
+  - ΘΕΑΤΡΟ
+  - ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ
+  - ΘΕΑΤΡΙΚΟ ΓΙΑ ΠΑΙΔΙΑ
+  volume: 2 ΤΟΜΟΙ
+  notes: ΔΩΡΕΑ ΕΛΠΙΔΟΦΟΡΟΣ ΙΝΤΖΕΜΠΕΛΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786185456481'
+  original_entry:
+    0: 17436
+    1: ΚΑΛΑΤΖΟΠΟΥΛΟΣ,ΓΙΑΝΝΗΣ
+    2: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ ΚΑΙ ... ΕΞΥΠΝΟΥΣ ΜΕΓΑΛΟΥΣ
+    4: 886.2ΚΑΛ
+    5: 22839,22840
+    8: ΦΙΛΝΤΙΣΙ
+    9: ΑΘΗΝΑ
+    10: '2021'
+    11: '335'
+    12: ΘΕΑΤΡΟ
+    13: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ
+    14: ΘΕΑΤΡΙΚΟ ΓΙΑ ΠΑΙΔΙΑ
+    17: ΔΩΡΕΑ ΕΛΠΙΔΟΦΟΡΟΣ ΙΝΤΖΕΜΠΕΛΗΣ
+    18: '9786185456'
+    19: '481'
+    30: 2 ΤΟΜΟΙ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+- dbase_number: 17437
+  authors:
+  - ΓΙΑΝΣΣΟΝ,ΤΟΥΒΕ
+  title: ΘΑΛΑΣΣΙΝΟ ΤΑΞΙΔΙ
+  dewey: 808.899 ΓΙΑ
+  entry_numbers:
+  - '22847'
+  translators:
+  - ΑΓΓΕΛΙΔΟΥ,ΜΑΡΙΑ
+  editor: ΠΑΤΑΚΗΣ // ΑΘΗΝΑ
+  edition_year: 2013
+  pages: 248
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601647012'
+  original_entry:
+    0: 17437
+    1: ΓΙΑΝΣΣΟΝ,ΤΟΥΒΕ
+    2: ΘΑΛΑΣΣΙΝΟ ΤΑΞΙΔΙ
+    4: 808.899ΓΙΑ
+    5: '22847'
+    6: ΜΑΡΙΑ ΑΓΓΕΛΙΔΟΥ
+    8: ΠΑΤΑΚΗΣ
+    9: ΑΘΗΝΑ
+    10: '2013'
+    11: '248'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789601647'
+    19: '012'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17438
+  authors:
+  - ΔΕΛΤΑ,Π.Σ
+  title: ΜΑΓΚΑΣ
+  dewey: 808.899 ΔΕΛ
+  entry_numbers:
+  - '22848'
+  editor: ΕΣΤΙΑ // ΑΘΗΝΑ
+  edition_year: 1975
+  pages: 305
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17438
+    1: ΔΕΛΤΑ,Π.Σ
+    2: ΜΑΓΚΑΣ
+    4: 808.899ΔΕΛ
+    5: '22848'
+    8: ΕΣΤΙΑ
+    9: ΑΘΗΝΑ
+    10: '1975'
+    11: '305'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17439
+  authors:
+  - ΔΟΥΜΑΣ,ΑΛΕΞΑΝΔΡΟΣ
+  title: ΟΙ ΤΡΕΙΣ ΣΩΜΑΤΟΦΥΛΑΚΕΣ
+  dewey: 808.899 ΔΟΥ
+  entry_numbers:
+  - '22851'
+  editor: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ // ΑΘΗΝΑ
+  pages: 234
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789606756382'
+  original_entry:
+    0: 17439
+    1: ΔΟΥΜΑΣ,ΑΛΕΞΑΝΔΡΟΣ
+    2: ΟΙ ΤΡΕΙΣ ΣΩΜΑΤΟΦΥΛΑΚΕΣ
+    4: 808.899ΔΟΥ
+    5: '22851'
+    8: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ
+    9: ΑΘΗΝΑ
+    11: '234'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789606756'
+    19: '382'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17440
+  authors:
+  - ΠΟΥΣΚΙΝ,ΑΛΕΞΑΝΤΡ
+  title: Η ΚΟΡΗ ΤΟΥ ΛΟΧΑΓΟΥ
+  dewey: 808.899 ΠΟΥ
+  entry_numbers:
+  - '22852'
+  editor: ΕΡΕΥΝΗΤΕΣ // ΑΘΗΝΑ
+  pages: 140
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789603684336'
+  original_entry:
+    0: 17440
+    1: ΠΟΥΣΚΙΝ,ΑΛΕΞΑΝΤΡ
+    2: Η ΚΟΡΗ ΤΟΥ ΛΟΧΑΓΟΥ
+    4: 808.899ΠΟΥ
+    5: '22852'
+    8: ΕΡΕΥΝΗΤΕΣ
+    9: ΑΘΗΝΑ
+    11: '140'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789603684'
+    19: '336'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17441
+  authors:
+  - ΝΤΕΦΟΕ,ΝΤΑΝΙΕΛ
+  title: ΡΟΒΙΝΣΩΝ ΚΡΟΥΣΟΣ
+  dewey: 808.899 ΝΤΕ
+  entry_numbers:
+  - '22853'
+  translators:
+  - ΓΙΑΝΝΗΣ ΚΟΤΣΙΚΑΣ
+  editor: ΠΑΠΑΔΗΜΗΤΡΙΟΥ // ΑΘΗΝΑ
+  edition_year: 2016
+  pages: 126
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789605851095'
+  original_entry:
+    0: 17441
+    1: ΝΤΕΦΟΕ,ΝΤΑΝΙΕΛ
+    2: ΡΟΒΙΝΣΩΝ ΚΡΟΥΣΟΣ
+    4: 808.899ΝΤΕ
+    5: '22853'
+    6: ΓΙΑΝΝΗΣ ΚΟΤΣΙΚΑΣ
+    8: ΠΑΠΑΔΗΜΗΤΡΙΟΥ
+    9: ΑΘΗΝΑ
+    10: '2016'
+    11: '126'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789605851'
+    19: 095
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17442
+  authors:
+  - ΝΤΙΚΕΝΣ,ΚΑΡΟΛ
+  title: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
+  dewey: 808.899 ΝΤΙ
+  entry_numbers:
+  - '22854'
+  translators:
+  - ΔΗΜΗΤΡΗΣ ΚΟΡΙΝΗΣ
+  editor: ΠΑΠΑΔΗΜΗΤΡΙΟΥ // ΑΘΗΝΑ
+  edition_year: 2016
+  pages: 319
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789605851071'
+  original_entry:
+    0: 17442
+    1: ΝΤΙΚΕΝΣ,ΚΑΡΟΛ
+    2: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
+    4: 808.899ΝΤΙ
+    5: '22854'
+    6: ΔΗΜΗΤΡΗΣ ΚΟΡΙΝΗΣ
+    8: ΠΑΠΑΔΗΜΗΤΡΙΟΥ
+    9: ΑΘΗΝΑ
+    10: '2016'
+    11: '319'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789605851'
+    19: '071'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17443
+  authors:
+  - ΤΟΥΕΙΝ,ΜΑΡΚ
+  title: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΤΟΜ ΣΟΓΙΕΡ
+  dewey: 808.899 ΤΟΥ
+  entry_numbers:
+  - '22855'
+  translators:
+  - ΑΘΑΝΑΣΙΑ ΜΠΙΡΗ
+  editor: ΚΑΛΟΚΑΘΗ // ΑΘΗΝΑ
+  edition_year: 2008
+  pages: 48
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789603963905'
+  original_entry:
+    0: 17443
+    1: ΤΟΥΕΙΝ,ΜΑΡΚ
+    2: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΤΟΜ ΣΟΓΙΕΡ
+    4: 808.899ΤΟΥ
+    5: '22855'
+    6: ΑΘΑΝΑΣΙΑ ΜΠΙΡΗ
+    8: ΚΑΛΟΚΑΘΗ
+    9: ΑΘΗΝΑ
+    10: '2008'
+    11: '48'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789603963'
+    19: '905'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17444
+  authors:
+  - ΠΑΠΑΝΤΩΝΙΟΥ,ΖΑΧΑΡΙΑΣ
+  title: ΤΑ ΨΗΛΑ ΒΟΥΝΑ
+  dewey: 808.899 ΠΑΠ
+  entry_numbers:
+  - '22856'
+  editor: ΠΕΡΙΒΟΛΑΚΗ // ΑΘΗΝΑ
+  edition_year: 1996
+  pages: 227
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9607412273'
+  original_entry:
+    0: 17444
+    1: ΠΑΠΑΝΤΩΝΙΟΥ,ΖΑΧΑΡΙΑΣ
+    2: ΤΑ ΨΗΛΑ ΒΟΥΝΑ
+    4: 808.899ΠΑΠ
+    5: '22856'
+    8: ΠΕΡΙΒΟΛΑΚΗ
+    9: ΑΘΗΝΑ
+    10: '1996'
+    11: '227'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9607412273'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17445
+  authors:
+  - ΝΤΙΚΕΝΣ,ΤΣΑΡΛΣ
+  title: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
+  dewey: 808.899 ΝΤΙ
+  entry_numbers:
+  - '22857'
+  translators:
+  - ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+  editor: ΜΙΝΩΑΣ // ΑΘΗΝΑ
+  edition_year: 2013
+  pages: 211
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604817429'
+  original_entry:
+    0: 17445
+    1: ΝΤΙΚΕΝΣ,ΤΣΑΡΛΣ
+    2: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
+    4: 808.899ΝΤΙ
+    5: '22857'
+    6: ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+    8: ΜΙΝΩΑΣ
+    9: ΑΘΗΝΑ
+    10: '2013'
+    11: '211'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789604817'
+    19: '429'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17446
+  authors:
+  - ΣΤΟΟΥ,ΧΑΡΙΕΤ-ΜΠΙΤΣΕΡ
+  title: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+  dewey: 808.899 ΣΤΟ
+  entry_numbers:
+  - '22858'
+  translators:
+  - ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+  editor: ΜΙΝΩΑΣ // ΑΘΗΝΑ
+  edition_year: 2013
+  pages: 219
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604816606'
+  original_entry:
+    0: 17446
+    1: ΣΤΟΟΥ,ΧΑΡΙΕΤ-ΜΠΙΤΣΕΡ
+    2: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+    4: 808.899ΣΤΟ
+    5: '22858'
+    6: ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+    8: ΜΙΝΩΑΣ
+    9: ΑΘΗΝΑ
+    10: '2013'
+    11: '219'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789604816'
+    19: '606'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17447
+  authors:
+  - ΡΟΟΥΛΙΝΓΚ,ΤΖ.Κ
+  title: Ο ΧΑΡΙ ΠΟΤΕΡ ΚΑΙ Η ΚΑΜΑΡΑ ΜΕ ΤΑ ΜΥΣΤΙΚΑ
+  dewey: 808.899 ΡΟΟ
+  entry_numbers:
+  - '22864'
+  translators:
+  - ΟΙΚΟΝΟΜΟΥ,ΚΑΙΤΗ
+  editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
+  edition_year: 2017
+  pages: 358
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789602744017'
+  original_entry:
+    0: 17447
+    1: ΡΟΟΥΛΙΝΓΚ,ΤΖ.Κ
+    2: Ο ΧΑΡΙ ΠΟΤΕΡ ΚΑΙ Η ΚΑΜΑΡΑ ΜΕ ΤΑ ΜΥΣΤΙΚΑ
+    4: 808.899ΡΟΟ
+    5: '22864'
+    6: ΚΑΙΤΗ ΟΙΚΟΝΟΜΟΥ
+    8: ΨΥΧΟΓΙΟΣ
+    9: ΑΘΗΝΑ
+    10: '2017'
+    11: 358Σ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789602744'
+    19: '017'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17448
+  authors:
+  - ΦΙΝΕΜΟΡ,ΤΖΟΝ
+  title: Ο ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+  dewey: 808.899 ΦΙΝ
+  entry_numbers:
+  - '22849'
+  translators:
+  - ΕΡ. ΜΠΑΡΤΖΙΝΟΠΟΥΛΟΣ
+  editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
+  edition_year: 2016
+  pages: 220
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789605851088'
+  original_entry:
+    0: 17448
+    1: ΦΙΝΕΜΟΡ,ΤΖΟΝ
+    2: Ο ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+    4: 808.899ΦΙΝ
+    5: '22849'
+    6: ΕΡ. ΜΠΑΡΤΖΙΝΟΠΟΥΛΟΣ
+    8: ΑΓΚΥΡΑ
+    9: ΑΘΗΝΑ
+    10: '2016'
+    11: '220'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789605851'
+    19: 088
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17449
+  authors:
+  - PYLE,HOWARD
+  title: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+  dewey: 808.899 PYL
+  entry_numbers:
+  - '22850'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2013
+  pages: 64
+  topics:
+  - ΑΙΔΙΚΗ ΠΛΟΓΟΤΕΧΝΙΑ
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17449
+    1: PYLE,HOWARD
+    2: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+    4: 808.899PYL
+    5: '22850'
+    9: ΑΘΗΝΑ
+    10: '2013'
+    11: '64'
+    12: ΑΙΔΙΚΗ ΠΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17450
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  title: ΜΙΧΑΗΛ ΣΤΡΟΓΚΟΦ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - '22859'
+  editor: ΣΜΥΡΝΙΩΤΑΚΗΣ // ΑΘΗΝΑ
+  pages: 254
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9602990678'
+  original_entry:
+    0: 17450
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+    2: ΜΙΧΑΗΛ ΣΤΡΟΓΚΟΦ
+    4: 808.899ΒΕΡ
+    5: '22859'
+    8: ΣΜΥΡΝΙΩΤΑΚΗΣ
+    9: ΑΘΗΝΑ
+    11: '254'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9602990678'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17451
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  title: Ο ΔΕΚΑΠΕΝΤΑΕΤΗΣ ΠΛΟΙΑΡΧΟΣ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - '22860'
+  editor: ΣΜΥΡΝΙΩΤΑΚΗΣ // ΑΘΗΝΑ
+  pages: 254
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9602990732'
+  original_entry:
+    0: 17451
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+    2: Ο ΔΕΚΑΠΕΝΤΑΕΤΗΣ ΠΛΟΙΑΡΧΟΣ
+    4: 808.899ΒΕΡ
+    5: '22860'
+    8: ΣΜΥΡΝΙΩΤΑΚΗΣ
+    9: ΑΘΗΝΑ
+    11: '254'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9602990732'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17452
+  authors:
+  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  title: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
+  dewey: 808.899 ΒΕΡ
+  entry_numbers:
+  - '22861'
+  translators:
+  - ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+  editor: ΜΙΝΩΑΣ // ΑΘΗΝΑ
+  pages: 251
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9786180201888'
+  original_entry:
+    0: 17452
+    1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+    2: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
+    4: 808.899ΒΕΡ
+    5: '22861'
+    6: ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+    8: ΜΙΝΩΑΣ
+    9: ΑΘΗΝΑ
+    11: '251'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9786180201'
+    19: '888'
+    3: null
+    7: null
+    10: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17453
+  authors:
+  - ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
+  title: ΠΑΡΑΜΥΘΙ ΧΩΡΙΣ ΟΝΟΜΑ
+  dewey: 808.899 ΔΕΛ
+  entry_numbers:
+  - '22862'
+  editor: ΜΙΝΩΑΣ // ΑΘΗΝΑ
+  edition_year: 2014
+  pages: 231
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604816439'
+  original_entry:
+    0: 17453
+    1: ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
+    2: ΠΑΡΑΜΥΘΙ ΧΩΡΙΣ ΟΝΟΜΑ
+    4: 808.899ΔΕΛ
+    5: '22862'
+    8: ΜΙΝΩΑΣ
+    9: ΑΘΗΝΑ
+    10: '2014'
+    11: '231'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789604816'
+    19: '439'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17454
+  authors:
+  - DOYLE,ARTHUR,CONAN
+  title: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΣΕΡΛΟΚ ΧΟΛΜΣ
+  dewey: 808.899 DOY
+  entry_numbers:
+  - '22863'
+  translators:
+  - ΠΙΠΙΝΗ,ΑΡΓΥΡΩ
+  editor: ΠΑΠΑΔΟΠΟΥΛΟΣ // ΑΘΗΝΑ
+  edition_year: 2005
+  pages: 109
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9604124242'
+  original_entry:
+    0: 17454
+    1: DOYLE,ARTHUR,CONAN
+    2: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΣΕΡΛΟΚ ΧΟΛΜΣ
+    4: 808.899DOY
+    5: '22863'
+    6: ΑΡΓΥΡΩ ΠΙΠΙΝΗ
+    8: ΠΑΠΑΔΟΠΟΥΛΟΣ
+    9: ΑΘΗΝΑ
+    10: '2005'
+    11: '109'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9604124242'
+    3: null
+    7: null
+    15: null
+    16: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17455
+  authors:
+  - ROWLING,J.K.
+  title: HARRY POTTER AND THE PHILOSOPHER'S STONE
+  dewey: 808.899 ROW
+  entry_numbers:
+  - '22865'
+  editor: BLOOMSBURY // LONDON
+  edition_year: 2014
+  pages: 332
+  topics:
+  - ΞΕΝΟΓΛΩΣΣΟ
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17455
+    1: ROWLING,J.K.
+    2: HARRY POTTER AND THE PHILOSOPHER'S STONE
+    4: 808.899ROW
+    5: '22865'
+    8: BLOOMSBURY
+    9: LONDON
+    10: '2014'
+    11: '332'
+    12: ΞΕΝΟΓΛΩΣΣΟ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΞΕΝΟΓΛΩΣΣΟ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΞΕΝΟΓΛΩΣΣΟ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9781488556'
+    19: '52'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17456
+  authors:
+  - BLYTON,ENID
+  title: ΟΙ ΠΕΝΤΕ ΦΙΛΟΙ ΠΑΛΙ ΣΤΟ ΝΗΣΙ ΤΟΥ ΚΙΡΡΙΝ
+  dewey: 808.899 BLY
+  entry_numbers:
+  - '22842'
+  translators:
+  - ΜΑΡΙΑ ΑΥΓΕΡΟΥ
+  editor: GUTENBERG // ΑΘΗΝΑ
+  edition_year: 1984
+  pages: 165
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17456
+    1: BLYTON,ENID
+    2: ΟΙ ΠΕΝΤΕ ΦΙΛΟΙ ΠΑΛΙ ΣΤΟ ΝΗΣΙ ΤΟΥ ΚΙΡΡΙΝ
+    4: 808.899BLY
+    5: '22842'
+    6: ΜΑΡΙΑ ΑΥΓΕΡΟΥ
+    8: GUTENBERG
+    9: ΑΘΗΝΑ
+    10: '1984'
+    11: '165'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17457
+  authors:
+  - BLYTON,ENID
+  title: ΟΙ ΠΕΝΤΕ ΦΙΛΟΙ ΠΕΦΤΟΥΝ ΣΕ ΠΕΡΙΠΕΤΕΙΑ
+  dewey: 808.899 BLY
+  entry_numbers:
+  - '22843'
+  translators:
+  - ΜΑΡΙΑ ΑΥΓΕΡΟΥ
+  editor: GUTENBERG // ΑΘΗΝΑ
+  edition_year: 1985
+  pages: 183
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17457
+    1: BLYTON,ENID
+    2: ΟΙ ΠΕΝΤΕ ΦΙΛΟΙ ΠΕΦΤΟΥΝ ΣΕ ΠΕΡΙΠΕΤΕΙΑ
+    4: 808.899BLY
+    5: '22843'
+    6: ΜΑΡΙΑ ΑΥΓΕΡΟΥ
+    8: GUTENBERG
+    9: ΑΘΗΝΑ
+    10: '1985'
+    11: '183'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17458
+  authors:
+  - BLYTON,ENID
+  title: ΟΙ ΜΥΣΤΙΚΟΙ 7 ΣΤΗΝ ΠΕΡΙΠΕΤΕΙΑ ΤΟΥ ΚΕΡΥ ΜΠΛΟΥ
+  dewey: 808.899 BLY
+  entry_numbers:
+  - '22846'
+  translators:
+  - ΜΑΡΙΑ ΤΣΑΟΥΣΗ
+  editor: GUTENBERG // ΑΘΗΝΑ
+  edition_year: 2012
+  pages: 106
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789600115079'
+  original_entry:
+    0: 17458
+    1: BLYTON,ENID
+    2: ΟΙ ΜΥΣΤΙΚΟΙ 7 ΣΤΗΝ ΠΕΡΙΠΕΤΕΙΑ ΤΟΥ ΚΕΡΥ ΜΠΛΟΥ
+    4: 808.899BLY
+    5: '22846'
+    6: ΜΑΡΙΑ ΤΣΑΟΥΣΗ
+    8: GUTENBERG
+    9: ΑΘΗΝΑ
+    10: '2012'
+    11: '106'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789600115'
+    19: 079
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17459
+  authors:
+  - ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+  title: ΣΩΣΤΕ ΤΟΝ ΣΚΑΜΠΕΡΜΥΣΤΙΚΟΙ ΕΦΤΑ
+  dewey: 808.899 ΜΠΛ
+  entry_numbers:
+  - '22845'
+  translators:
+  - ΑΛΕΞΑΝΔΡΑ ΒΑΣΙΛΕΙΟΥ
+  editor: GUTENBERG // ΑΘΗΝΑ
+  edition_year: 1985
+  pages: 134
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17459
+    1: ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+    2: ΣΩΣΤΕ ΤΟΝ ΣΚΑΜΠΕΡΜΥΣΤΙΚΟΙ ΕΦΤΑ
+    4: 808.899ΜΠΛ
+    5: '22845'
+    6: ΑΛΕΞΑΝΔΡΑ ΒΑΣΙΛΕΙΟΥ
+    8: GUTENBERG
+    9: ΑΘΗΝΑ
+    10: '1985'
+    11: 134Σ
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17460
+  authors:
+  - ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+  title: ΟΙ ΜΥΣΤΙΚΟΙ ΕΦΤΑ ΣΕ ΜΙΑ ΔΙΑΣΚΕΔΑΣΤΙΚΗ ΠΕΡΙΠΕΤΕΙΑ
+  dewey: 808.899 ΜΠΛ
+  entry_numbers:
+  - '22844'
+  translators:
+  - ΑΛΕΞΑΝΔΡΑ ΒΑΣΙΛΕΙΟΥ
+  editor: GUTENBERG // ΑΘΗΝΑ
+  edition_year: 1985
+  pages: 114
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17460
+    1: ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+    2: ΟΙ ΜΥΣΤΙΚΟΙ ΕΦΤΑ ΣΕ ΜΙΑ ΔΙΑΣΚΕΔΑΣΤΙΚΗ ΠΕΡΙΠΕΤΕΙΑ
+    4: 808.899ΜΠΛ
+    5: '22844'
+    6: ΑΛΕΞΑΝΔΡΑ ΒΑΣΙΛΕΙΟΥ
+    8: GUTENBERG
+    9: ΑΘΗΝΑ
+    10: '1985'
+    11: '114'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17461
+  authors: []
+  title: Η ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΓΙΑ ΤΟ ΔΗΜΟΤΙΚΟ
+  dewey: 808.899 ΧΣ
+  entry_numbers:
+  - '22869'
+  translators:
+  - ΠΛΑΚΟΥΛΑ,ΜΠΕΣΣΥ
+  editor: MODREN TIMES // ΑΘΗΝΑ
+  edition_year: 2004
+  pages: 174
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17461
+    1: Χ.Σ
+    2: Η ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΓΙΑ ΤΟ ΔΗΜΟΤΙΚΟ
+    4: 808.899Χ.Σ
+    5: '22869'
+    6: ΜΠΕΣΣΥ ΠΛΑΚΟΥΛΑ
+    8: MODREN TIMES
+    9: ΑΘΗΝΑ
+    10: '2004'
+    11: '174'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17462
+  authors:
+  - BOURNIER,ISABELLE
+  title: ΤΟ ΜΕΓΑΛΟ ΒΙΒΛΙΟ ΓΙΑ ΤΗΝ ΕΙΡΗΝΗ
+  dewey: 808.899 BOU
+  entry_numbers:
+  - '22870'
+  translators:
+  - ΜΑΡΙΑ ΜΠΑΣΤΑ
+  editor: ΕΡΕΥΝΗΤΕΣ // ΑΘΗΝΑ
+  edition_year: 2008
+  pages: 94
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789603684206'
+  original_entry:
+    0: 17462
+    1: BOURNIER,ISABELLE
+    2: ΤΟ ΜΕΓΑΛΟ ΒΙΒΛΙΟ ΓΙΑ ΤΗΝ ΕΙΡΗΝΗ
+    4: 808.899BOU
+    5: '22870'
+    6: ΜΑΡΙΑ ΜΠΑΣΤΑ
+    8: ΕΡΕΥΝΗΤΕΣ
+    9: ΑΘΗΝΑ
+    10: '2008'
+    11: '94'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789603684'
+    19: '206'
+    3: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17463
+  authors: []
+  title: Η ΓΗ
+  dewey: 808.899 ΧΣ
+  entry_numbers:
+  - '22868'
+  translators:
+  - ΣΩΤΗΡΙΑ ΟΡΦΑΝΙΔΟΥ
+  editor: ΣΑΒΒΑΛΑΣ // ΑΘΗΝΑ
+  edition_year: 2005
+  pages: 79
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17463
+    1: Χ.Σ.
+    2: Η ΓΗ
+    4: 808.899Χ.Σ
+    5: '22868'
+    6: ΣΩΤΗΡΙΑ ΟΡΦΑΝΙΔΟΥ
+    8: ΣΑΒΒΑΛΑΣ
+    9: ΑΘΗΝΑ
+    10: '2005'
+    11: '79'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17464
+  authors: []
+  title: ΑΦΡΙΚΗ 1
+  dewey: 808.899 ΧΣ
+  entry_numbers:
+  - '22866'
+  editor: DE AGOSTINI // ΑΘΗΝΑ
+  edition_year: 2008
+  pages: 57
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604166312'
+  original_entry:
+    0: 17464
+    1: Χ.Σ
+    2: ΑΦΡΙΚΗ 1
+    4: 808.899Χ.Σ
+    5: '22866'
+    8: DE AGOSTINI
+    9: ΑΘΗΝΑ
+    10: '2008'
+    11: '57'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789604166'
+    19: '312'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17465
+  authors: []
+  title: ΚΛΑΣΣΙΚΑ ΕΙΚΟΝΟΓΡΑΦΗΜΕΝΑ
+  dewey: 808.899 ΧΣ
+  entry_numbers:
+  - '22871'
+  editor: ΑΤΛΑΝΤΙΣ // ΑΘΗΝΑ
+  pages: 360
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: 'ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+
+    ΤΟΜΟΙ 3 - 4'
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17465
+    1: Χ.Σ.
+    2: ΚΛΑΣΣΙΚΑ ΕΙΚΟΝΟΓΡΑΦΗΜΕΝΑ
+    4: 808.899Χ.Σ
+    5: '22871'
+    8: ΑΤΛΑΝΤΙΣ
+    9: ΑΘΗΝΑ
+    11: '360'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    30: ΤΟΜΟΙ 3 - 4
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+- dbase_number: 17466
+  authors:
+  - DOOLEY,JENNY
+  title: EXCALIBUR- ACTIVITY BOOK
+  dewey: 808.899 DOO
+  entry_numbers:
+  - '22872'
+  editor: EXPRESS PUBLISHING // ENGLAND
+  edition_year: 2006
+  pages: 47
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  - ΞΕΝΟΓΛΩΣΣΟ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17466
+    1: DOOLEY,JENNY
+    2: EXCALIBUR- ACTIVITY BOOK
+    4: 808.899DOO
+    5: '22872'
+    8: EXPRESS PUBLISHING
+    9: ENGLAND
+    10: '2006'
+    11: '47'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΞΕΝΟΓΛΩΣΣΟ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΞΕΝΟΓΛΩΣΣΟ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΞΕΝΟΓΛΩΣΣΟ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17467
+  authors: []
+  title: FILOMATHIX
+  subtitle: ΕΠΙΣΤΗΜΕΣ ΤΗΣ ΓΗΣ
+  dewey: 808.899 ΧΣ
+  entry_numbers:
+  - '22867'
+  editor: ΠΕΔΙΟ // ΑΘΗΝΑ
+  edition_year: 2009
+  pages: 56
+  topics:
+  - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  notes: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604750887'
+  original_entry:
+    0: 17467
+    1: Χ.Σ.
+    2: FILOMATHIX
+    3: ΕΠΙΣΤΗΜΕΣ ΤΗΣ ΓΗΣ
+    4: 808.899Χ.Σ
+    5: '22867'
+    8: ΠΕΔΙΟ
+    9: ΑΘΗΝΑ
+    10: '2009'
+    11: '56'
+    12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+    18: '9789604750'
+    19: '887'
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17468
+  authors: []
+  title: ΕΛΛΑΔΑ ΙΣΤΟΡΙΑ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ
+  subtitle: ΤΟ ΝΕΟ ΕΛΛΗΝΙΚΟ ΚΡΑΤΟΣ Η ΟΙΚΟΝΟΜΙΑ
+  dewey: 938 ΧΣ
+  entry_numbers:
+  - '10666'
+  editor: ΜΑΛΛΙΑΡΗΣ // ΑΘΗΝΑ
+  edition_year: 1982
+  pages: 506
+  topics:
+  - ΠΟΛΙΤΙΣΜΟΣ
+  - ΕΛΛΑΔΑ
+  volume: ΤΟΜΟΣ 8
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9602392290'
+  original_entry:
+    0: 17468
+    1: Χ.Σ
+    2: ΕΛΛΑΔΑ ΙΣΤΟΡΙΑ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ
+    3: ΤΟ ΝΕΟ ΕΛΛΗΝΙΚΟ ΚΡΑΤΟΣ Η ΟΙΚΟΝΟΜΙΑ
+    4: 938Χ.Σ
+    5: '10666'
+    8: ΜΑΛΛΙΑΡΗΣ
+    9: ΑΘΗΝΑ
+    10: '1982'
+    11: '506'
+    12: ΙΣΤΟΡΙΑ-ΠΟΛΙΤΙΣΜΟΣ
+    13: ΕΛΛΑΔΑ
+    14: ΙΣΤΟΡΙΑ
+    15: ΠΟΛΙΤΙΣΜΟΣ
+    17: ΤΟΜΟΣ 8
+    18: '9602392290'
+    6: null
+    7: null
+    16: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17469
+  authors:
+  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  title: ΔΗΜΟΣΘΕΝΟΥΣ ΠΡΟΣ ΠΟΛΥΚΛΕΑ ΠΕΡΙ ΤΟΥ ΕΠΙΤΡΙΗΡΑΡΧΗΜΑΤΟΣ
+  subtitle: Η ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ ΚΑΤΑ ΤΟΝ 4ΟΝ ΑΙΩΝΑ Π.Χ
+  dewey: 938.02 ΒΕΤ
+  entry_numbers:
+  - '22873'
+  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2022
+  pages: 54
+  topics:
+  - ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ
+  - ΑΘΗΝΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17469
+    1: ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+    2: ΔΗΜΟΣΘΕΝΟΥΣ ΠΡΟΣ ΠΟΛΥΚΛΕΑ ΠΕΡΙ ΤΟΥ ΕΠΙΤΡΙΗΡΑΡΧΗΜΑΤΟΣ
+    3: Η ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ ΚΑΤΑ ΤΟΝ 4ΟΝ ΑΙΩΝΑ Π.Χ
+    4: 938.02ΒΕΤ
+    5: '22873'
+    9: ΘΕΣ/ΝΙΚΗ
+    10: '2022'
+    11: '54'
+    12: ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ
+    13: ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ
+    14: ΑΘΗΝΑ
+    18: '960920130'
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17470
+  authors:
+  - DROYSEN,JOHANN-GUSTAV
+  title: ΙΣΤΟΡΙΑ ΤΩΝ ΔΙΑΔΟΧΩΝ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+  dewey: 938.18 DRO
+  entry_numbers:
+  - '21528'
+  editor: ΕΛΕΥΘΕΡΟΤΥΠΙΑ // ΑΘΗΝΑ
+  edition_year: 1993
+  pages: 325
+  topics:
+  - ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+  - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
+  volume: 2 ΤΟΜΟΙ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17470
+    1: DROYSEN,JOHANN-GUSTAV
+    2: ΙΣΤΟΡΙΑ ΤΩΝ ΔΙΑΔΟΧΩΝ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+    4: 938.18DRO
+    5: '21528'
+    8: ΕΛΕΥΘΕΡΟΤΥΠΙΑ
+    9: ΑΘΗΝΑ
+    10: '1993'
+    11: '325'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+    14: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
+    17: 2 ΤΟΜΟΙ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17471
+  authors:
+  - ΜΕΤΑΛΛΗΝΟΥ,ΓΕΩΡΓΙΟΥ
+  title: ΤΟΥΡΚΟΚΡΑΤΙΑ
+  subtitle: ΟΙ ΕΛΛΗΝΕΣ ΣΤΗΝ ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
+  dewey: 938.4 ΜΕΤ
+  entry_numbers:
+  - '21576'
+  editor: ΑΚΡΙΤΑΣ // ΑΘΗΝΑ
+  edition_year: 1998
+  pages: 268
+  topics:
+  - ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  isbn: '9607006062'
+  original_entry:
+    0: 17471
+    1: ΜΕΤΑΛΛΗΝΟΥ,ΓΕΩΡΓΙΟΥ
+    2: ΤΟΥΡΚΟΚΡΑΤΙΑ
+    3: ΟΙ ΕΛΛΗΝΕΣ ΣΤΗΝ ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
+    4: 938.4ΜΕΤ
+    5: '21576'
+    8: ΑΚΡΙΤΑΣ
+    9: ΑΘΗΝΑ
+    10: '1998'
+    11: 268Σ
+    12: ΙΣΤΟΡΙΑ-ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
+    18: '9607006062'
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17472
+  authors:
+  - MOSSE,C.
+  title: ΤΟ ΤΕΛΟΣ ΤΗΣ ΑΘΗΝΑΙΚΗΣ ΔΗΜΟΚΡΑΤΙΑΣ
+  dewey: 938 MOS
+  entry_numbers:
+  - '17207'
+  translators:
+  - Γ.Κ. ΒΛΑΧΟΥ
+  editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
+  edition_year: 1978
+  pages: 639
+  topics:
+  - ΑΘΗΝΑΙΚΗ ΔΗΜΟΚΡΑΤΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17472
+    1: MOSSE,C.
+    2: ΤΟ ΤΕΛΟΣ ΤΗΣ ΑΘΗΝΑΙΚΗΣ ΔΗΜΟΚΡΑΤΙΑΣ
+    4: 938MOS
+    5: '17207'
+    6: Γ.Κ. ΒΛΑΧΟΥ
+    8: ΠΑΠΑΖΗΣΗ
+    9: ΑΘΗΝΑ
+    10: '1978'
+    11: '639'
+    12: ΙΣΤΟΡΙΑ-ΑΘΗΝΑΙΚΗ ΔΗΜΟΚΡΑΤΙΑ
+    13: ΑΘΗΝΑΙΚΗ ΔΗΜΟΚΡΑΤΙΑ
+    14: ΙΣΤΟΡΙΑ
+    3: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17473
+  authors:
+  - DROYSEN,JOHANN-GUSTAV
+  title: ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+  dewey: 938.174 DRO
+  entry_numbers:
+  - '22874'
+  editor: ΕΛΕΥΘΕΡΟΤΥΠΙΑ // ΑΘΗΝΑ
+  edition_year: 1993
+  pages: 390
+  topics:
+  - ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+  - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
+  notes: ΤΟΜΟΙ 1-2.
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17473
+    1: DROYSEN,JOHANN-GUSTAV
+    2: ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+    4: 938.174DRO
+    5: '22874'
+    8: ΕΛΕΥΘΕΡΟΤΥΠΙΑ
+    9: ΑΘΗΝΑ
+    10: '1993'
+    11: '390'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+    14: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
+    17: ΤΟΜΟΙ 1-2.
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17474
+  authors:
+  - ΠΛΟΥΜΙΔΗΣ,ΓΕΩΡΓΙΟΣ
+  title: ΚΑΝΟΝΙΣΜΟΙ ΤΗΣ ΝΗΣΟΥ ΚΥΠΡΟΥ (1507-1522)
+  dewey: 938.497 ΠΛΟ
+  entry_numbers:
+  - '7789'
+  editor: None // ΙΩΑΝΝΙΝΑ
+  edition_year: 1987
+  pages: 90
+  topics:
+  - ΚΥΠΡΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17474
+    1: ΠΛΟΥΜΙΔΗΣ,ΓΕΩΡΓΙΟΣ
+    2: ΚΑΝΟΝΙΣΜΟΙ ΤΗΣ ΝΗΣΟΥ ΚΥΠΡΟΥ (1507-1522)
+    4: 938.497ΠΛΟ
+    5: '7789'
+    9: ΙΩΑΝΝΙΝΑ
+    10: '1987'
+    11: '90'
+    12: ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
+    13: ΚΥΠΡΟΣ-ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    15: ΚΥΠΡΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17475
+  authors:
+  - ΝΙΑΡΧΟΣ,Θ.
+  title: ΚΥΠΡΟΣ ΝΗΣΙ ΤΟΥ ΠΑΘΟΥΣ ΚΑΙ ΤΩΝ ΜΑΡΤΥΡΙΩΝ
+  dewey: 938.497 ΝΙΑ
+  entry_numbers:
+  - '21225'
+  editor: ΛΑΜΠΡΑΚΗΣ // ΑΘΗΝΑ
+  edition_year: 2013
+  pages: 187
+  topics:
+  - ΚΥΠΡΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789605033958'
+  original_entry:
+    0: 17475
+    1: ΝΙΑΡΧΟΣ,Θ.
+    2: ΚΥΠΡΟΣ ΝΗΣΙ ΤΟΥ ΠΑΘΟΥΣ ΚΑΙ ΤΩΝ ΜΑΡΤΥΡΙΩΝ
+    4: 938.497ΝΙΑ
+    5: '21225'
+    8: ΛΑΜΠΡΑΚΗΣ
+    9: ΑΘΗΝΑ
+    10: '2013'
+    11: '187'
+    12: ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
+    13: ΚΥΠΡΟΣ-ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    15: ΚΥΠΡΟΣ
+    18: '9789605033'
+    19: '958'
+    3: null
+    6: null
+    7: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17476
+  authors: []
+  title: Η ΠΡΩΤΗ ΝΙΚΗ 1940-1941
+  dewey: 949.507 ΧΣ
+  entry_numbers:
+  - '12668'
+  editor: NATIONAL GEOGRAPHIC // ΑΘΗΝΑ
+  pages: 158
+  topics: []
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789604880935'
+  original_entry:
+    0: 17476
+    1: Χ.Σ.
+    2: Η ΠΡΩΤΗ ΝΙΚΗ 1940-1941
+    4: 949.507Χ.Σ
+    5: '12668'
+    8: NATIONAL GEOGRAPHIC
+    9: ΑΘΗΝΑ
+    11: '158'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    18: '9789604880'
+    19: '935'
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17477
+  authors: []
+  title: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΠΑΙΔΕΙΑ
+  dewey: 039.89 ΜΑΛ
+  entry_numbers:
+  - '22882'
+  editor: ΜΑΛΛΙΑΡΗΣ // ΑΘΗΝΑ
+  edition_year: 1976
+  pages: 200
+  topics:
+  - ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
+  notes: ΤΟΜΟΙ 20
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17477
+    1: Χ.Σ.
+    2: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΠΑΙΔΕΙΑ
+    4: 039.89ΜΑΛ
+    5: '22882'
+    8: ΜΑΛΛΙΑΡΗΣ
+    9: ΑΘΗΝΑ
+    10: '1976'
+    11: '200'
+    12: ΕΓΚΥΚΛΟΑΠΙΔΕΙΑ
+    13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
+    14: ΕΓΚΥΚΛΟΑΠΙΔΕΙΑ
+    17: ΤΟΜΟΙ 20
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17478
+  authors:
+  - ΧΡΙΣΤΟΔΟΥΛΟΥ,ΑΝΑΣΤΑΣΙΑ
+  title: ΠΑΙΔΕΙΑ, ΕΚΠΑΙΔΕΥΣΗ, ΑΞΙΕΣ
+  subtitle: ΣΗΜΕΙΩΤΙΚΗ ΠΡΟΣΕΓΓΙΣΗ
+  dewey: 302.2 ΧΡΙ
+  entry_numbers:
+  - '22884'
+  editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2012
+  pages: 145
+  topics:
+  - ΕΚΠΑΙΔΕΥΣΗ
+  - ΠΑΙΔΕΙΑ
+  donors:
+  - ΙΝΤΖΕΜΠΕΛΗΣ,ΕΛΠΙΔΟΦΟΡΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601221281'
+  original_entry:
+    0: 17478
+    1: ΧΡΙΣΤΟΔΟΥΛΟΥ,ΑΝΑΣΤΑΣΙΑ
+    2: ΠΑΙΔΕΙΑ, ΕΚΠΑΙΔΕΥΣΗ, ΑΞΙΕΣ
+    3: ΣΗΜΕΙΩΤΙΚΗ ΠΡΟΣΕΓΓΙΣΗ
+    4: 302.2ΧΡΙ
+    5: '22884'
+    8: UNIVERSITY STUDIO PR
+    9: ΘΕΣ/ΝΙΚΗ
+    10: '2012'
+    11: '145'
+    12: ΕΚΠΑΙΔΕΥΣΗ-ΠΑΙΔΕΙΑ
+    13: ΠΑΙΔΕΙΑ-ΕΚΠΑΙΔΕΥΣΗ
+    14: ΕΚΠΑΙΔΕΥΣΗ
+    15: ΠΑΙΔΕΙΑ
+    17: ΔΩΡΕΑ ΕΛΠΙΔΟΦΟΡΟΥ ΙΝΤΖΕΜΠΕΛΗ
+    18: '9789601221'
+    19: '281'
+    6: null
+    7: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17479
+  authors:
+  - ΤΖΙΜΑΣ,ΔΗΜΗΤΡΗΣ
+  title: ΤΟ ΝΕΟΧΩΡΑΚΙ ΑΡΤΑΣ
+  dewey: 938.939 ΤΖΙ
+  entry_numbers:
+  - '22883'
+  editor: None // ΑΡΤΑ
+  pages: 239
+  topics:
+  - ΝΕΟΧΩΡΑΚΙ ΑΡΤΑ
+  - ΑΡΤΑ
+  - ΝΕΟΧΩΡΑΚΙΑ ΑΡΤΑΣ
+  donors:
+  - ΙΝΤΖΕΜΠΕΛΗΣ,ΕΛΠΙΔΟΦΟΡΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789609313308'
+  original_entry:
+    0: 17479
+    1: ΤΖΙΜΑΣ,ΔΗΜΗΤΡΗΣ
+    2: ΤΟ ΝΕΟΧΩΡΑΚΙ ΑΡΤΑΣ
+    4: 938.939ΤΖΙ
+    5: '22883'
+    9: ΑΡΤΑ
+    11: '239'
+    12: ΙΣΤΟΡΙΑ-ΝΕΟΧΩΡΑΚΙ ΑΡΤΑ
+    13: ΑΡΤΑ
+    14: ΙΣΤΟΡΙΑ
+    15: ΝΕΟΧΩΡΑΚΙΑ ΑΡΤΑΣ
+    17: ΔΩΡΕΑ ΕΛΠΙΔΟΦΟΡΟΥ ΙΝΤΖΕΜΠΕΛΗ
+    18: '9789609313'
+    19: '308'
+    3: null
+    6: null
+    7: null
+    8: null
+    10: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17480
+  authors:
+  - ΣΑΡΡΗΓΙΑΝΝΙΔΗΣ,ΚΩΝ.
+  title: Ο ΠΟΝΤΟΣ 28 ΑΙΩΝΕΣ ΔΟΞΗΣ ΚΑΙ ΘΡΥΛΟΥ
+  dewey: 938 ΣΑΡ
+  entry_numbers:
+  - '20915'
+  pages: 93
+  topics:
+  - ΠΟΝΤΟΣ
+  donors:
+  - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17480
+    1: ΣΑΡΡΗΓΙΑΝΝΙΔΗΣ,ΚΩΝ.
+    2: Ο ΠΟΝΤΟΣ 28 ΑΙΩΝΕΣ ΔΟΞΗΣ ΚΑΙ ΘΡΥΛΟΥ
+    4: 938ΣΑΡ
+    5: '20915'
+    11: 93Σ
+    12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+    14: ΠΟΝΤΟΣ
+    15: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
+    3: null
+    6: null
+    7: null
+    8: null
+    9: null
+    10: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17481
+  authors:
+  - ΘΕΟΔΩΡΙΔΗΣ,ΚΩΣΤΑΣ
+  title: ΜΝΗΜΕΣ ΠΟΥ ΑΝΤΙΣΤΕΚΟΝΤΑΙ ...
+  dewey: 938.498 ΘΕΟ
+  entry_numbers:
+  - '20393'
+  editor: ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2019
+  pages: 606
+  topics:
+  - ΠΟΝΤΟΣ
+  donors:
+  - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789605992835'
+  original_entry:
+    0: 17481
+    1: ΘΕΟΔΩΡΙΔΗΣ,ΚΩΣΤΑΣ
+    2: ΜΝΗΜΕΣ ΠΟΥ ΑΝΤΙΣΤΕΚΟΝΤΑΙ ...
+    4: 938.498ΘΕΟ
+    5: '20393'
+    8: ΚΥΡΙΑΚΙΔΗΣ
+    9: ΘΕΣ/ΝΙΚΗ
+    10: '2019'
+    11: '606'
+    12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+    13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+    14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
+    18: '9789605992'
+    19: '835'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17482
+  authors:
+  - ΚΑΛΑΜΒΡΕΖΟΣ,ΔΙΟΝΥΣΙΟΣ
+  title: Ο ΕΛΛΗΝΙΣΜΟΣ ΣΤΗ ΡΩΣΙΑ ΚΑΙ ΣΤΙΣ ΑΛΛΕΣ ΧΩΡΕΣ ΤΗΣ Τ. ΕΣΣΔ
+  dewey: 938.498 ΚΑΛ
+  entry_numbers:
+  - '20399'
+  editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
+  edition_year: 2017
+  pages: 909
+  topics:
+  - ΔΙΕΘΝΗ ΠΟΛΙΤΙΚΗ
+  donors:
+  - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789600232912'
+  original_entry:
+    0: 17482
+    1: ΚΑΛΑΜΒΡΕΖΟΣ,ΔΙΟΝΥΣΙΟΣ
+    2: Ο ΕΛΛΗΝΙΣΜΟΣ ΣΤΗ ΡΩΣΙΑ ΚΑΙ ΣΤΙΣ ΑΛΛΕΣ ΧΩΡΕΣ ΤΗΣ Τ. ΕΣΣΔ
+    4: 938.498ΚΑΛ
+    5: '20399'
+    8: ΠΑΠΑΖΗΣΗ
+    9: ΑΘΗΝΑ
+    10: '2017'
+    11: '909'
+    12: ΔΙΕΘΝΗ ΠΟΛΙΤΙΚΗ
+    13: ΔΙΕΘΝΗ ΠΟΛΙΤΙΚΗ
+    14: ΔΙΕΘΝΗ ΠΟΛΙΤΙΚΗ
+    17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
+    18: '9789600232'
+    19: '912'
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17483
+  authors: []
+  title: ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ
+  subtitle: 8ΟΣ ΑΙΩΝΑΣ Π.Χ -1922
+  dewey: 938.497 ΧΣ
+  entry_numbers:
+  - '12667'
+  - '15039'
+  editor: ΤΕΣΣΕΡΑ ΠΙ // ΑΘΗΝΑ
+  edition_year: 2012
+  pages: 126
+  topics:
+  - ΠΟΝΤΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17483
+    1: Χ.Σ.
+    2: ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ
+    3: 8ΟΣ ΑΙΩΝΑΣ Π.Χ -1922
+    4: 938.497Χ.Σ
+    5: 12667-15039
+    8: ΤΕΣΣΕΡΑ ΠΙ
+    9: ΑΘΗΝΑ
+    10: '2012'
+    11: '126'
+    12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+    13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+    14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+    6: null
+    7: null
+    15: null
+    16: null
+    17: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17484
+  authors:
+  - ΣΠΥΡΟΜΙΛΙΟΥ,ΜΙΛΤΟΥ
+  title: ΕΛΛΑΣ ΚΑΙ ΑΛΒΑΝΙΑ Ο ΓΚΙΟΛΕΚΑΣ
+  dewey: 941.2 ΣΠΥ
+  entry_numbers:
+  - '22898'
+  editor: Ν. ΚΟΥΒΑΡΑ // ΑΘΗΝΑ
+  edition_year: 1966
+  pages: 107
+  topics:
+  - ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΙΣΤΟΡΙΑ
+  notes: ΔΩΡΕΑ ΕΛ.ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17484
+    1: ΣΠΥΡΟΜΙΛΙΟΥ,ΜΙΛΤΟΥ
+    2: ΕΛΛΑΣ ΚΑΙ ΑΛΒΑΝΙΑ Ο ΓΚΙΟΛΕΚΑΣ
+    4: 941.2ΣΠΥ
+    5: '22898'
+    8: Ν. ΚΟΥΒΑΡΑ
+    9: ΑΘΗΝΑ
+    10: '1966'
+    11: '107'
+    12: ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΙΣΤΟΡΙΑ
+    13: ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΙΣΤΟΡΙΑ
+    14: ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ.ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17485
+  authors:
+  - ΚΟΥΚΚΟΥ,ΕΛΕΝΗ
+  title: ΙΣΤΟΡΙΑ ΤΩΝ ΕΠΤΑΝΗΣΩΝ
+  dewey: 938.481 ΚΟΥ
+  entry_numbers:
+  - '22899'
+  editor: ΠΑΠΑΔΗΜΑ // ΑΘΗΝΑ
+  edition_year: 1999
+  pages: 250
+  topics:
+  - ΙΣΤΟΡΙΑ
+  - ΕΠΤΑΝΗΣΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17485
+    1: ΚΟΥΚΚΟΥ,ΕΛΕΝΗ
+    2: ΙΣΤΟΡΙΑ ΤΩΝ ΕΠΤΑΝΗΣΩΝ
+    4: 938.481ΚΟΥ
+    5: '22899'
+    8: ΠΑΠΑΔΗΜΑ
+    9: ΑΘΗΝΑ
+    10: '1999'
+    11: '250'
+    12: ΙΣΤΟΡΙΑ - ΕΠΤΑΝΗΣΑ
+    13: ΙΣΤΟΡΙΑ - ΕΠΤΑΝΗΣΑ
+    14: ΙΣΤΟΡΙΑ - ΕΠΤΑΝΗΣΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17486
+  authors:
+  - ΚΑΡΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ
+  title: ΕΙΣΑΓΩΓΗ ΣΤΗΝ ΤΕΧΝΙΚΗ ΤΗΣ ΕΠΙΣΤΗΜΟΝΙΚΗΣ ΙΣΤΟΡΙΚΗΣ ΕΡΓΑΣΙΑΣ
+  dewey: 907.2 ΚΑΡ
+  entry_numbers: []
+  editor: ΒΑΝΙΑΣ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1988
+  pages: 110
+  topics:
+  - ΕΠΙΣΤΗΜΟΝΙΚΕΣ ΕΡΓΑΣΙΕΣ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17486
+    1: ΚΑΡΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ
+    2: ΕΙΣΑΓΩΓΗ ΣΤΗΝ ΤΕΧΝΙΚΗ ΤΗΣ ΕΠΙΣΤΗΜΟΝΙΚΗΣ ΙΣΤΟΡΙΚΗΣ ΕΡΓΑΣΙΑΣ
+    4: 907.2ΚΑΡ
+    8: ΒΑΝΙΑΣ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1988'
+    11: '110'
+    12: ΕΠΙΣΤΗΜΟΝΙΚΕΣ ΕΡΓΑΣΙΕΣ
+    13: ΕΠΙΣΤΗΜΟΝΙΚΕΣ ΕΡΓΑΣΙΕΣ
+    14: ΕΠΙΣΤΗΜΟΝΙΚΕΣ ΕΡΓΑΣΙΕΣ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    5: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17487
+  authors:
+  - ΣΤΑΛΙΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  title: ΟΙ ΣΥΝΤΕΧΝΙΕΣ ΚΑΙ ΤΑ ΕΠΑΓΓΕΛΜΑΤΑ ΣΤΗΝ ΕΔΕΣΣΑ
+  dewey: 938.492 ΣΤΑ
+  entry_numbers:
+  - '22897'
+  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1999
+  pages: 240
+  topics:
+  - ΙΣΤΟΡΙΑ
+  - ΕΠΑΓΓΕΛΜΑΤΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17487
+    1: ΣΤΑΛΙΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+    2: ΟΙ ΣΥΝΤΕΧΝΙΕΣ ΚΑΙ ΤΑ ΕΠΑΓΓΕΛΜΑΤΑ ΣΤΗΝ ΕΔΕΣΣΑ
+    4: 938.492ΣΤΑ
+    5: '22897'
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1999'
+    11: '240'
+    12: ΙΣΤΟΡΙΑ - ΕΠΑΓΓΕΛΜΑΤΑ
+    13: ΙΣΤΟΡΙΑ - ΕΠΑΓΓΕΛΜΑΤΑ
+    14: ΙΣΤΟΡΙΑ - ΕΠΑΓΓΕΛΜΑΤΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17488
+  authors:
+  - ΑΣΔΡΑΧΑΣ,ΣΠΥΡΟΣ
+  title: ΟΙΚΟΝΟΜΙΑ ΚΑΙ ΝΟΟΤΡΟΠΙΕΣ
+  dewey: 949.505 ΑΣΔ
+  entry_numbers:
+  - '22907'
+  editor: ΕΡΜΗΣ // ΑΘΗΝΑ
+  edition_year: 1988
+  pages: 260
+  topics:
+  - ΟΙΚΟΝΟΜΙΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17488
+    1: ΑΣΔΡΑΧΑΣ,ΣΠΥΡΟΣ
+    2: ΟΙΚΟΝΟΜΙΑ ΚΑΙ ΝΟΟΤΡΟΠΙΕΣ
+    4: 949.505ΑΣΔ
+    5: '22907'
+    8: ΕΡΜΗΣ
+    9: ΑΘΗΝΑ
+    10: '1988'
+    11: '260'
+    12: ΙΣΤΟΡΙΑ-ΟΙΚΟΝΟΜΙΑ
+    13: ΙΣΤΟΡΙΑ-ΟΙΚΟΝΟΜΙΑ
+    14: ΙΣΤΟΡΙΑ-ΟΙΚΟΝΟΜΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17489
+  authors:
+  - ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
+  title: ΡΩΣΣΑΓΓΛΟΓΑΛΛΟΣ
+  dewey: 949.505 ΠΑΠ
+  entry_numbers:
+  - '22910'
+  editor: ΡΕΚΟΣ // None
+  pages: 200
+  topics: []
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17489
+    1: ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
+    2: ΡΩΣΣΑΓΓΛΟΓΑΛΛΟΣ
+    4: 949.505ΠΑΠ
+    5: '22910'
+    8: ΡΕΚΟΣ
+    11: '200'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    9: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17490
+  authors:
+  - ΔΡΟΥΛΙΑ,ΛΟΥΚΙΑ
+  title: ΠΡΟΣΕΓΓΙΣΕΙΣ ΣΤΙΣ ΝΟΟΤΡΟΠΙΕΣ ΤΩΝ ΒΑΛΚΑΝΙΚΩΝ ΛΑΩΝ
+  dewey: 949.6 ΔΡΟ
+  entry_numbers:
+  - '22909'
+  editor: Ι.ΖΑΧΑΡΟΠΟΥΛΟΣ // ΑΘΗΝΑ
+  edition_year: 1988
+  pages: 170
+  topics: []
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17490
+    1: ΔΡΟΥΛΙΑ,ΛΟΥΚΙΑ
+    2: ΠΡΟΣΕΓΓΙΣΕΙΣ ΣΤΙΣ ΝΟΟΤΡΟΠΙΕΣ ΤΩΝ ΒΑΛΚΑΝΙΚΩΝ ΛΑΩΝ
+    4: 949.6ΔΡΟ
+    5: '22909'
+    8: Ι.ΖΑΧΑΡΟΠΟΥΛΟΣ
+    9: ΑΘΗΝΑ
+    10: '1988'
+    11: '170'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17491
+  authors:
+  - ΔΡΟΥΛΙΑ,ΛΟΥΚΙΑ
+  title: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ
+  dewey: 910.9 ΔΡΟ
+  entry_numbers:
+  - '22908'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 1993
+  pages: 550
+  topics:
+  - ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ
+  - ΒΑΛΚΑΝΙΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17491
+    1: ΔΡΟΥΛΙΑ,ΛΟΥΚΙΑ
+    2: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ
+    4: 910.9ΔΡΟ
+    5: '22908'
+    9: ΑΘΗΝΑ
+    10: '1993'
+    11: '550'
+    12: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ-ΒΑΛΚΑΝΙΑ
+    13: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ-ΒΑΛΚΑΝΙΑ
+    14: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ-ΒΑΛΚΑΝΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17492
+  authors:
+  - ΣΥΓΚΕΛΟΥ,ΕΥΣΤΡΑΤΙΑ
+  title: Ο ΠΟΛΕΜΟΣ ΣΤΟΝ ΔΥΤΙΚΟ ΕΛΛΑΔΙΚΟ ΧΩΡΟ ΚΑΤΑ ΤΟΝ ΔΕΥΤΕΡΟ ΜΕΣΑΙΩΝ
+  subtitle: Α
+  dewey: 938.375 ΣΥΓ
+  entry_numbers:
+  - '22906'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2008
+  pages: 450
+  topics:
+  - ΠΟΛΕΜΟΣ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17492
+    1: ΣΥΓΚΕΛΟΥ,ΕΥΣΤΡΑΤΙΑ
+    2: Ο ΠΟΛΕΜΟΣ ΣΤΟΝ ΔΥΤΙΚΟ ΕΛΛΑΔΙΚΟ ΧΩΡΟ ΚΑΤΑ ΤΟΝ ΔΕΥΤΕΡΟ ΜΕΣΑΙΩΝ
+    3: Α
+    4: 938.375ΣΥΓ
+    5: '22906'
+    9: ΑΘΗΝΑ
+    10: '2008'
+    11: '450'
+    12: ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
+    13: ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
+    14: ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17493
+  authors:
+  - NICOL,DONALD
+  title: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
+  dewey: 938.375 NIC
+  entry_numbers:
+  - '22905'
+  editor: ΕΛΛΗΝΙΚΗ ΕΥΕΩΕΚΔΟΤΙΚ // ΑΘΗΝΑ
+  edition_year: 1991
+  pages: 380
+  topics:
+  - ΗΠΕΙΡΟΣ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17493
+    1: NICOL,DONALD
+    2: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
+    4: 938.375NIC
+    5: '22905'
+    8: ΕΛΛΗΝΙΚΗ ΕΥΕΩΕΚΔΟΤΙΚ
+    9: ΑΘΗΝΑ
+    10: '1991'
+    11: '380'
+    12: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
+    13: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
+    14: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17494
+  authors:
+  - ΑΝΤΩΝΙΑΔΗΣ,ΞΕΝΟΦΩΝ
+  title: Η ΣΚΥΡΟΣ ΣΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑ
+  dewey: 938.495 ΑΝΤ
+  entry_numbers:
+  - '22904'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 1997
+  pages: 341
+  topics:
+  - ΣΚΥΡΟΣ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17494
+    1: ΑΝΤΩΝΙΑΔΗΣ,ΞΕΝΟΦΩΝ
+    2: Η ΣΚΥΡΟΣ ΣΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑ
+    4: 938.495ΑΝΤ
+    5: '22904'
+    9: ΑΘΗΝΑ
+    10: '1997'
+    11: '341'
+    12: ΙΣΤΟΡΙΑ-ΣΚΥΡΟΣ
+    13: ΙΣΤΟΡΙΑ-ΣΚΥΡΟΣ
+    14: ΙΣΤΟΡΙΑ-ΣΚΥΡΟΣ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17495
+  authors:
+  - ΣΙΑΤΡΑΣ,ΔΗΜΗΤΡΗΣ
+  title: ΟΙ ΑΓΟΡΑΠΩΛΗΣΙΕΣ ΑΚΙΝΗΤΩΝ ΣΤΗΝ ΤΟΥΡΚΟΚΡΑΤΟΥΜΕΝΗ ΕΛΛΑΔΑ
+  dewey: 938.76 ΣΙΑ
+  entry_numbers:
+  - '22903'
+  editor: ΓΝΩΣΗ // ΑΘΗΝΑ
+  edition_year: 1992
+  pages: 275
+  topics: []
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17495
+    1: ΣΙΑΤΡΑΣ,ΔΗΜΗΤΡΗΣ
+    2: ΟΙ ΑΓΟΡΑΠΩΛΗΣΙΕΣ ΑΚΙΝΗΤΩΝ ΣΤΗΝ ΤΟΥΡΚΟΚΡΑΤΟΥΜΕΝΗ ΕΛΛΑΔΑ
+    4: 938.76ΣΙΑ
+    5: '22903'
+    8: ΓΝΩΣΗ
+    9: ΑΘΗΝΑ
+    10: '1992'
+    11: '275'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17496
+  authors:
+  - ΤΣΙΡΠΑΝΛΗΣ,ΖΑΧΑΡΙΑΣ
+  title: ΕΙΣΑΓΩΓΗ ΣΤΗ ΜΕΣΑΙΩΝΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΔΥΤΙΚΗΣ ΕΥΡΩΠΗΣ
+  dewey: 940.1 ΤΣΙ
+  entry_numbers:
+  - '22902'
+  editor: ΖΗΤΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1996
+  pages: 325
+  topics: []
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17496
+    1: ΤΣΙΡΠΑΝΛΗΣ,ΖΑΧΑΡΙΑΣ
+    2: ΕΙΣΑΓΩΓΗ ΣΤΗ ΜΕΣΑΙΩΝΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΔΥΤΙΚΗΣ ΕΥΡΩΠΗΣ
+    4: 940.1ΤΣΙ
+    5: '22902'
+    8: ΖΗΤΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1996'
+    11: '325'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17497
+  authors:
+  - HERING-ΚΑΤΣΙΑΡΔΗ,ΟΛΓΑ
+  title: ΤΕΧΝΙΤΕΣ ΚΑΙ ΤΕΧΝΙΚΕΣ ΒΑΦΗΣ ΝΗΜΑΤΩΝ
+  dewey: 677.009 HER
+  entry_numbers:
+  - '22901'
+  editor: ΗΡΟΔΟΤΟΣ // None
+  pages: 381
+  topics:
+  - ΥΦΑΝΤΟΥΡΓΙΑ
+  - ΧΡΩΜΑΤΑ
+  - ΒΑΦΕΣ
+  - ΘΕΣΣΑΛΙΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17497
+    1: HERING-ΚΑΤΣΙΑΡΔΗ,ΟΛΓΑ
+    2: ΤΕΧΝΙΤΕΣ ΚΑΙ ΤΕΧΝΙΚΕΣ ΒΑΦΗΣ ΝΗΜΑΤΩΝ
+    4: 677.009HER
+    5: '22901'
+    8: ΗΡΟΔΟΤΟΣ
+    11: '381'
+    12: ΥΦΑΝΤΟΥΡΓΙΑ-ΧΡΩΜΑΤΑ-ΒΑΦΕΣ
+    13: ΥΦΑΝΤΟΥΡΓΙΑ-ΧΡΩΜΑΤΑ-ΒΑΦΕΣ
+    14: ΘΕΣΣΑΛΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    9: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17498
+  authors:
+  - ΚΥΡΙΑΚΟΥ,ΑΡΤΕΜΗ
+  title: Η ΕΛΛΗΝΙΚΗ ΚΟΙΝΟΤΗΤΑ ΤΗΣ ΒΕΝΕΤΙΑΣ
+  dewey: 938.499 ΚΥΡ
+  entry_numbers:
+  - '22896'
+  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1978
+  pages: 300
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΚΟΙΝΟΤΗΤΑ
+  - ΒΕΝΕΤΙΑ
+  - ΔΙΔΑΚΤΟΡΙΚΗ ΔΙΑΤΡΙΒΗ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17498
+    1: ΚΥΡΙΑΚΟΥ,ΑΡΤΕΜΗ
+    2: Η ΕΛΛΗΝΙΚΗ ΚΟΙΝΟΤΗΤΑ ΤΗΣ ΒΕΝΕΤΙΑΣ
+    4: 938.499ΚΥΡ
+    5: '22896'
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1978'
+    11: '300'
+    12: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΚΟΙΝΟΤΗΤΑ
+    13: ΕΛΛΗΝΙΚΗ ΚΟΙΝΟΤΗΤΑ-ΒΕΝΕΤΙΑ
+    14: ΔΙΔΑΚΤΟΡΙΚΗ ΔΙΑΤΡΙΒΗ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17499
+  authors:
+  - ΚΑΡΑΓΕΩΡΓΑΚΗ,ΜΑΡΙΑ
+  title: ΣΥΓΧΡΟΝΕΣ ΜΕΘΟΔΟΛΟΓΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ ΣΤΗ ΔΙΔΑΣΚΑΛΙΑ ΤΗΣ ΙΣΤΟ
+  subtitle: ΡΙΑΣ
+  dewey: 907 ΚΑΡ
+  entry_numbers:
+  - '22888'
+  editor: ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2007
+  pages: 370
+  topics:
+  - ΔΙΔΑΣΚΑΚΙΑ ΤΗΣ ΙΣΤΟΡΙΑΣ
+  - ΘΕΜΑΤΑ ΙΣΤΟΡΙΚΑ
+  - ΔΙΔΑΣΚΑΛΙΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17499
+    1: ΚΑΡΑΓΕΩΡΓΑΚΗ,ΜΑΡΙΑ
+    2: ΣΥΓΧΡΟΝΕΣ ΜΕΘΟΔΟΛΟΓΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ ΣΤΗ ΔΙΔΑΣΚΑΛΙΑ ΤΗΣ ΙΣΤΟ
+    3: ΡΙΑΣ
+    4: 907ΚΑΡ
+    5: '22888'
+    8: ΚΥΡΙΑΚΙΔΗ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2007'
+    11: '370'
+    12: ΔΙΔΑΣΚΑΚΙΑ ΤΗΣ ΙΣΤΟΡΙΑΣ
+    13: ΙΣΤΟΡΙΑ
+    14: ΘΕΜΑΤΑ ΙΣΤΟΡΙΚΑ- ΔΙΔΑΣΚΑΛΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17500
+  authors:
+  - ΓΛΑΒΙΝΑ,ΑΠΟΣΤΟΛΟΥ
+  title: ΕΓΓΡΑΦΑ ΠΕΡΙ ΤΗΣ ΠΡΑΞΙΚΟΠΗΜΑΤΙΚΗΣ ΣΥΓΚΡΟΤΗΣΕΩΣ ΤΗΣ ΣΥΝΟΔΟΥ Τ
+  subtitle: ΗΣ ΟΡΘΟΔΟΞΟΥ ΕΚΚΛΗΣΙΑΣ ΤΗΣ ΑΛΒΑΝΙΑΣ
+  dewey: 281.949 ΓΛΑ
+  entry_numbers:
+  - '22895'
+  editor: ΙΜΙΑΧ // ΙΩΑΝΝΙΝΑ
+  edition_year: 1981
+  pages: 80
+  topics:
+  - ΕΚΚΛΗΣΙΑ
+  - ΑΛΒΑΝΙΑ
+  - ΕΚΚΛΗΣΙΑ ΑΛΒΑΝΙΑΣ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17500
+    1: ΓΛΑΒΙΝΑ,ΑΠΟΣΤΟΛΟΥ
+    2: ΕΓΓΡΑΦΑ ΠΕΡΙ ΤΗΣ ΠΡΑΞΙΚΟΠΗΜΑΤΙΚΗΣ ΣΥΓΚΡΟΤΗΣΕΩΣ ΤΗΣ ΣΥΝΟΔΟΥ Τ
+    3: ΗΣ ΟΡΘΟΔΟΞΟΥ ΕΚΚΛΗΣΙΑΣ ΤΗΣ ΑΛΒΑΝΙΑΣ
+    4: 281.949ΓΛΑ
+    5: '22895'
+    8: ΙΜΙΑΧ
+    9: ΙΩΑΝΝΙΝΑ
+    10: '1981'
+    11: '80'
+    12: ΕΚΚΛΗΣΙΑ-ΑΛΒΑΝΙΑ
+    13: ΑΛΒΑΝΙΑ-ΕΚΚΛΗΣΙΑ
+    14: ΕΚΚΛΗΣΙΑ ΑΛΒΑΝΙΑΣ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17501
+  authors:
+  - ΕΝΕΠΕΚΙΔΗΣ,Π.Κ.
+  title: ΜΑΚΕΔΟΝΙΚΕΣ ΠΟΛΕΙΣ ΚΑΙ ΟΙΚΟΓΕΝΕΙΕΣ 1750-1930
+  dewey: 914.95 ΕΝΕ
+  entry_numbers:
+  - '22894'
+  editor: ΒΙΒΛΟΠΩΛΕΙΟΝ ΕΣΤΙΑΣ // ΑΘΗΝΑ
+  edition_year: 1984
+  pages: 324
+  topics:
+  - ΜΑΚΕΔΟΝΙΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17501
+    1: ΕΝΕΠΕΚΙΔΗΣ,Π.Κ.
+    2: ΜΑΚΕΔΟΝΙΚΕΣ ΠΟΛΕΙΣ ΚΑΙ ΟΙΚΟΓΕΝΕΙΕΣ 1750-1930
+    4: 914.95ΕΝΕ
+    5: '22894'
+    8: ΒΙΒΛΟΠΩΛΕΙΟΝ ΕΣΤΙΑΣ
+    9: ΑΘΗΝΑ
+    10: '1984'
+    11: '324'
+    12: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
+    13: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
+    14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17502
+  authors:
+  - ΒΑΚΑΛΟΠΟΥΛΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  title: ΟΙΚΟΝΟΜΙΚΗ ΛΕΙΤΟΥΡΓΙΑ ΤΟΥ ΜΑΚΕΔΟΝΙΚΟΥ ΚΑΙ ΘΡΑΚΙΚΟΥ ΧΩΡΟΥ ΣΤΑ
+  subtitle: ΜΕΣΑ ΤΟΥ 19ΟΥ ΑΙΩΝΑ ΣΤΑ ΠΛΑΙΣΙΑ ΤΟΥ ΔΙΕΘΝΟΥΣ ΕΜΠΟΡΙΟΥ
+  dewey: 330.949 ΒΑΚ
+  entry_numbers:
+  - '22891'
+  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1980
+  pages: 215
+  topics:
+  - ΟΙΚΟΝΟΜΙΑ
+  - ΟΙΚΟΝΟΜΙΚΑ
+  - ΟΙΚΟΝΟΜΙΚΑ ΘΕΜΑΤΑ ΜΑΚΕΔΟΝΙΑΣ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17502
+    1: ΒΑΚΑΛΟΠΟΥΛΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+    2: ΟΙΚΟΝΟΜΙΚΗ ΛΕΙΤΟΥΡΓΙΑ ΤΟΥ ΜΑΚΕΔΟΝΙΚΟΥ ΚΑΙ ΘΡΑΚΙΚΟΥ ΧΩΡΟΥ ΣΤΑ
+    3: ' ΜΕΣΑ ΤΟΥ 19ΟΥ ΑΙΩΝΑ ΣΤΑ ΠΛΑΙΣΙΑ ΤΟΥ ΔΙΕΘΝΟΥΣ ΕΜΠΟΡΙΟΥ'
+    4: 330.949ΒΑΚ
+    5: '22891'
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1980'
+    11: '215'
+    12: ΟΙΚΟΝΟΜΙΑ-ΙΣΤΟΡΙΑ
+    13: ΟΙΚΟΝΟΜΙΚΑ
+    14: ΟΙΚΟΝΟΜΙΚΑ ΘΕΜΑΤΑ ΜΑΚΕΔΟΝΙΑΣ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17503
+  authors:
+  - ΛΙΑΤΑ,ΕΥΤΥΧΙΑ
+  title: ΑΡΓΕΙΑ ΓΗ
+  dewey: 938.921 ΛΙΑ
+  entry_numbers:
+  - '22893'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2003
+  pages: 140
+  topics: []
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17503
+    1: ΛΙΑΤΑ,ΕΥΤΥΧΙΑ
+    2: ΑΡΓΕΙΑ ΓΗ
+    4: 938.921ΛΙΑ
+    5: '22893'
+    9: ΑΘΗΝΑ
+    10: '2003'
+    11: '140'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17504
+  authors:
+  - ΠΑΠΑΓΕΩΡΓΙΟΥ,ΓΕΩΡΓΙΟΣ
+  title: ΟΙ ΣΥΝΤΕΧΝΙΕΣ ΣΤΑ ΓΙΑΝΝΕΝΑ ΚΑΤΑ ΤΟΝ 19ο ΚΑΙ ΤΙΣ ΑΡΧΕΣ ΤΟΥ 20
+  subtitle: ου ΑΙΩΝΑ
+  dewey: 938.936 ΠΑΠ
+  entry_numbers:
+  - '22892'
+  editor: ΙΜΙΑΧ // ΙΩΑΝΝΙΝΑ
+  edition_year: 1988
+  pages: 363
+  topics:
+  - ΓΙΑΝΝΕΝΑ
+  - ΙΣΤΟΡΙΑ ΙΩΑΝΝΙΝΑ
+  - ΙΣΤΟΡΙΚΑ ΤΩΝ ΙΩΑΝΝΙΝΩΝ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17504
+    1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΓΕΩΡΓΙΟΣ
+    2: ΟΙ ΣΥΝΤΕΧΝΙΕΣ ΣΤΑ ΓΙΑΝΝΕΝΑ ΚΑΤΑ ΤΟΝ 19ο ΚΑΙ ΤΙΣ ΑΡΧΕΣ ΤΟΥ 20
+    3: ου ΑΙΩΝΑ
+    4: 938.936ΠΑΠ
+    5: '22892'
+    8: ΙΜΙΑΧ
+    9: ΙΩΑΝΝΙΝΑ
+    10: '1988'
+    11: '363'
+    12: ΙΣΤΟΡΙΑ-ΓΙΑΝΝΕΝΑ
+    13: ΙΣΤΟΡΙΑ ΙΩΑΝΝΙΝΑ
+    14: ΙΣΤΟΡΙΚΑ ΤΩΝ ΙΩΑΝΝΙΝΩΝ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17505
+  authors:
+  - ΚΟΝΤΟΓΙΑΝΝΗ,ΠΑΝΤΕΛΗ
+  title: ΟΙ ΕΛΛΗΝΕΣ
+  dewey: 938.471 ΚΟΝ
+  entry_numbers:
+  - '22890'
+  editor: Π.Δ. ΣΑΚΕΛΛΑΡΙΟΥ // ΑΘΗΝΑ
+  pages: 528
+  topics: []
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17505
+    1: ΚΟΝΤΟΓΙΑΝΝΗ,ΠΑΝΤΕΛΗ
+    2: ΟΙ ΕΛΛΗΝΕΣ
+    4: 938.471ΚΟΝ
+    5: '22890'
+    8: Π.Δ. ΣΑΚΕΛΛΑΡΙΟΥ
+    9: ΑΘΗΝΑ
+    11: '528'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17506
+  authors:
+  - ΠΑΝΑΓΟΠΟΥΛΟΣ,ΑΓΓΕΛΙΚΗ
+  title: ΟΙ ΔΙΠΛΩΜΑΤΙΚΟΙ ΓΑΜΟΙ ΣΤΟ ΒΥΖΑΝΤΙΟ
+  dewey: 949.503 ΠΑΝ
+  entry_numbers:
+  - '22889'
+  editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
+  edition_year: 2006
+  pages: 550
+  topics:
+  - ΒΥΖΑΝΤΙΟ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17506
+    1: ΠΑΝΑΓΟΠΟΥΛΟΣ,ΑΓΓΕΛΙΚΗ
+    2: ΟΙ ΔΙΠΛΩΜΑΤΙΚΟΙ ΓΑΜΟΙ ΣΤΟ ΒΥΖΑΝΤΙΟ
+    4: 949.503ΠΑΝ
+    5: '22889'
+    8: Α.Α. ΛΙΒΑΝΗ
+    10: '2006'
+    11: '550'
+    12: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+    13: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+    14: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    9: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17507
+  authors:
+  - ΣΒΟΡΩΝΟΣ,ΝΙΚΟΣ
+  title: ΕΠΙΣΚΟΠΗΣΗ ΤΗΣ ΝΕΟΕΛΛΗΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
+  dewey: 938.3 ΣΒΟ
+  entry_numbers:
+  - '22887'
+  editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
+  edition_year: 1985
+  pages: 339
+  topics: []
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17507
+    1: ΣΒΟΡΩΝΟΣ,ΝΙΚΟΣ
+    2: ΕΠΙΣΚΟΠΗΣΗ ΤΗΣ ΝΕΟΕΛΛΗΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
+    4: 938.3ΣΒΟ
+    5: '22887'
+    8: ΘΕΜΕΛΙΟ
+    9: ΑΘΗΝΑ
+    10: '1985'
+    11: '339'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17508
+  authors:
+  - MILLER,WILLIAM
+  title: Η ΦΡΑΓΚΟΚΡΑΤΙΑ ΣΤΗΝ ΕΛΛΑΔΑ 1204-1566
+  dewey: 938.37 MIL
+  entry_numbers:
+  - '22921'
+  editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
+  edition_year: 1997
+  pages: 742
+  topics:
+  - ΦΡΑΓΚΟΚΡΑΤΙΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17508
+    1: MILLER,WILLIAM
+    2: Η ΦΡΑΓΚΟΚΡΑΤΙΑ ΣΤΗΝ ΕΛΛΑΔΑ 1204-1566
+    4: 938.37MIL
+    5: '22921'
+    8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
+    9: ΑΘΗΝΑ
+    10: '1997'
+    11: '742'
+    12: ΙΣΤΟΡΙΑ-ΦΡΑΓΚΟΚΡΑΤΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17509
+  authors:
+  - ΚΡΕΜΜΥΔΑΣ,ΒΑΣΙΛΗΣ
+  title: ΕΛΛΗΝΙΚΗ ΝΑΥΤΙΛΙΑ 1776-1835
+  dewey: 387.51 ΚΡΕ
+  entry_numbers:
+  - '22913'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 1985
+  pages: 155
+  topics:
+  - ΝΑΥΤΙΛΙΑ
+  - ΕΛΛΗΝΙΚΗ ΝΑΥΤΙΛΙΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17509
+    1: ΚΡΕΜΜΥΔΑΣ,ΒΑΣΙΛΗΣ
+    2: ΕΛΛΗΝΙΚΗ ΝΑΥΤΙΛΙΑ 1776-1835
+    4: 387.51ΚΡΕ
+    5: '22913'
+    9: ΑΘΗΝΑ
+    10: '1985'
+    11: '155'
+    12: ΝΑΥΤΙΛΙΑ
+    13: ΕΛΛΗΝΙΚΗ ΝΑΥΤΙΛΙΑ
+    14: ΝΑΥΤΙΛΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17510
+  authors:
+  - ΠΕΛΕΚΙΔΟΥ,ΜΑΡΙΑ
+  title: ΟΙ ΒΑΛΚΑΝΙΚΟΙ ΛΑΟΙ
+  dewey: 949.6 ΠΕΛ
+  entry_numbers:
+  - '22914'
+  editor: ΒΑΝΙΑΣ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1991
+  pages: 380
+  topics:
+  - ΒΑΛΚΑΝΙΑ
+  - ΒΑΛΚΑΝΙΚΟΙ ΛΑΟΙ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17510
+    1: ΠΕΛΕΚΙΔΟΥ,ΜΑΡΙΑ
+    2: ΟΙ ΒΑΛΚΑΝΙΚΟΙ ΛΑΟΙ
+    4: 949.6ΠΕΛ
+    5: '22914'
+    8: ΒΑΝΙΑΣ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1991'
+    11: '380'
+    12: ΙΣΤΟΡΙΑ-ΒΑΛΚΑΝΙΑ
+    13: ΒΑΛΚΑΝΙΚΟΙ ΛΑΟΙ
+    14: ΒΑΛΚΑΝΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17511
+  authors:
+  - ΛΙΑΤΑ,ΕΥΤΥΧΙΑ
+  title: Η ΣΕΡΙΦΟΣ ΚΑΤΑ ΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑ
+  dewey: 938.496 ΛΙΑ
+  entry_numbers:
+  - '22915'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 1987
+  pages: 235
+  topics:
+  - ΣΕΡΙΦΟΣ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17511
+    1: ΛΙΑΤΑ,ΕΥΤΥΧΙΑ
+    2: Η ΣΕΡΙΦΟΣ ΚΑΤΑ ΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑ
+    4: 938.496ΛΙΑ
+    5: '22915'
+    9: ΑΘΗΝΑ
+    10: '1987'
+    11: '235'
+    12: ΙΣΤΟΡΙΑ-ΣΕΡΙΦΟΣ
+    13: ΙΣΤΟΡΙΑ-ΣΕΡΙΦΟΣ
+    14: ΙΣΤΟΡΙΑ-ΣΕΡΙΦΟΣ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17512
+  authors:
+  - ΣΑΒΒΙΔΗΣ,ΑΛΕΞΙΟΣ
+  title: ΔΟΚΙΜΙΑ ΟΘΩΜΑΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
+  dewey: 956.015 ΣΑΒ
+  entry_numbers:
+  - '22916'
+  editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
+  edition_year: 2004
+  pages: 300
+  topics:
+  - ΟΘΩΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
+  - ΔΟΚΙΜΙΑ ΙΣΤΟΡΙΚΑ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17512
+    1: ΣΑΒΒΙΔΗΣ,ΑΛΕΞΙΟΣ
+    2: ΔΟΚΙΜΙΑ ΟΘΩΜΑΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
+    4: 956.015ΣΑΒ
+    5: '22916'
+    8: ΠΑΠΑΖΗΣΗ
+    9: ΑΘΗΝΑ
+    10: '2004'
+    11: '300'
+    12: ΙΣΤΟΡΙΑ
+    13: ΟΘΩΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
+    14: ΔΟΚΙΜΙΑ ΙΣΤΟΡΙΚΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17513
+  authors:
+  - ΠΑΠΑΓΕΩΡΓΙΟΥ,ΓΕΩΡΓΙΟΣ
+  title: Ο ΕΚΣΥΧΡΟΝΙΣΜΟΣ ΤΟΥ ΕΛΛΗΝΑ ΠΡΑΓΜΑΤΕΥΤΗ ΣΥΜΦΩΝΑ ΜΕ ΤΑ ΕΥΡΩΠΑΙ
+  subtitle: ΚΑ ΠΡΟΤΥΠΑ
+  dewey: 938.501 ΠΑΠ
+  entry_numbers:
+  - '22917'
+  editor: ΑΦΟΙ ΤΟΛΙΔΗ // ΑΘΗΝΑ
+  pages: 201
+  topics: []
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17513
+    1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΓΕΩΡΓΙΟΣ
+    2: Ο ΕΚΣΥΧΡΟΝΙΣΜΟΣ ΤΟΥ ΕΛΛΗΝΑ ΠΡΑΓΜΑΤΕΥΤΗ ΣΥΜΦΩΝΑ ΜΕ ΤΑ ΕΥΡΩΠΑΙ
+    3: ΚΑ ΠΡΟΤΥΠΑ
+    4: 938.501ΠΑΠ
+    5: '22917'
+    8: ΑΦΟΙ ΤΟΛΙΔΗ
+    9: ΑΘΗΝΑ
+    11: '201'
+    12: ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17514
+  authors:
+  - ΤΣΙΛΗ,ΓΕΩΡΓΙΟΥ
+  title: ΣΟΥΛΙ-ΚΑΤΑΓΩΓΗ ΣΟΥΛΙΩΤΩΝ
+  dewey: 938.478 ΤΣΙ
+  entry_numbers:
+  - '22918'
+  editor: ΑΠΕΙΡΟΣ ΧΩΡΑ // ΑΘΗΝΑ
+  edition_year: 2008
+  pages: 193
+  topics:
+  - ΣΟΥΛΙ
+  - ΙΣΤΟΡΙΚΑ ΣΟΥΛΙΩΤΩΝ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17514
+    1: ΤΣΙΛΗ,ΓΕΩΡΓΙΟΥ
+    2: ΣΟΥΛΙ-ΚΑΤΑΓΩΓΗ ΣΟΥΛΙΩΤΩΝ
+    4: 938.478ΤΣΙ
+    5: '22918'
+    8: APIROS HORA
+    9: ΑΘΗΝΑ
+    10: '2008'
+    11: '193'
+    12: ΙΣΤΟΡΙΑ-ΣΟΥΛΙ
+    13: ΙΣΤΟΡΙΚΑ ΣΟΥΛΙΩΤΩΝ
+    14: ΙΣΤΟΡΙΑ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17515
+  authors:
+  - ΠΛΑΚΟΓΙΑΝΝΑΚΗΣ,ΚΙΜΩΝ-ΕΜΜΑΝΟΥΗΛ
+  title: ΤΙΜΗΤΙΚΟΙ ΤΙΤΛΟΙ ΚΑΙ ΕΝΕΡΓΑ ΑΞΙΩΜΑΤΑ ΣΤΟ ΒΥΖΑΝΤΙΟ
+  dewey: 938.3 ΠΛΑ
+  entry_numbers:
+  - '22919'
+  editor: ΙΑΝΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2001
+  pages: 400
+  topics:
+  - ΒΥΖΑΝΤΙΟ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17515
+    1: ΠΛΑΚΟΓΙΑΝΝΑΚΗΣ,ΚΙΜΩΝ-ΕΜΜΑΝΟΥΗΛ
+    2: ΤΙΜΗΤΙΚΟΙ ΤΙΤΛΟΙ ΚΑΙ ΕΝΕΡΓΑ ΑΞΙΩΜΑΤΑ ΣΤΟ ΒΥΖΑΝΤΙΟ
+    4: 938.3ΠΛΑ
+    5: '22919'
+    8: ΙΑΝΟΣ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2001'
+    11: '400'
+    12: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+    13: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+    14: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17516
+  authors:
+  - ΜΑΡΙΝΑΚΟΥ,ΕΛΕΝΗ
+  title: ΑΙ ΕΝ ΘΡΑΚΗ ΣΥΝΤΕΧΝΙΑΙ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΤΑ ΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑΝ
+  dewey: 938.416 ΜΑΡ
+  entry_numbers:
+  - '22920'
+  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1950
+  pages: 202
+  topics:
+  - ΘΡΑΚΗ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17516
+    1: ΜΑΡΙΝΑΚΟΥ,ΕΛΕΝΗ
+    2: ΑΙ ΕΝ ΘΡΑΚΗ ΣΥΝΤΕΧΝΙΑΙ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΤΑ ΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑΝ
+    4: 938.416ΜΑΡ
+    5: '22920'
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1950'
+    11: '202'
+    12: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
+    13: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
+    14: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17517
+  authors: []
+  title: ΕΩΑ ΚΑΙ ΕΣΠΕΡΙΑ
+  dewey: 025 ΧΣ
+  entry_numbers:
+  - '22932'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2006
+  pages: 310
+  topics:
+  - ΠΕΡΙΟΔΙΚΟ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ 1-6
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17517
+    1: Χ.Σ
+    2: ΕΩΑ ΚΑΙ ΕΣΠΕΡΙΑ
+    4: 025Χ.Σ
+    5: '22932'
+    9: ΑΘΗΝΑ
+    10: '2006'
+    11: '310'
+    12: ΠΕΡΙΟΔΙΚΟ
+    13: ΠΕΡΙΟΔΙΚΟ
+    14: ΠΕΡΙΟΔΙΚΟ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ 1-6
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17518
+  authors: []
+  title: Ο ΕΡΑΝΙΣΤΗΣ
+  dewey: 025 ΧΣ
+  entry_numbers:
+  - '22933'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 1993
+  pages: 380
+  topics:
+  - ΠΕΡΙΟΔΙΚΟ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17518
+    1: Χ.Σ
+    2: Ο ΕΡΑΝΙΣΤΗΣ
+    4: 025Χ.Σ
+    5: '22933'
+    9: ΑΘΗΝΑ
+    10: '1993'
+    11: '380'
+    12: ΠΕΡΙΟΔΙΚΟ
+    13: ΠΕΡΙΟΔΙΚΟ
+    14: ΠΕΡΙΟΔΙΚΟ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17519
+  authors: []
+  title: ΤΕΤΡΑΔΙΑ ΕΡΓΑΣΙΑΣ
+  dewey: 025 ΧΣ
+  entry_numbers:
+  - '22934'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2004
+  pages: 370
+  topics:
+  - ΠΕΡΙΟΔΙΚΟ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ 1-5
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17519
+    1: Χ.Σ
+    2: ΤΕΤΡΑΔΙΑ ΕΡΓΑΣΙΑΣ
+    4: 025Χ.Σ
+    5: '22934'
+    9: ΑΘΗΝΑ
+    10: '2004'
+    11: '370'
+    12: ΠΕΡΙΟΔΙΚΟ
+    13: ΠΕΡΙΟΔΙΚΟ
+    14: ΠΕΡΙΟΔΙΚΟ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ 1-5
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17520
+  authors: []
+  title: Ζ ΠΑΝΙΟΝΙΟ ΣΥΝΕΔΡΙΟ - ΠΡΑΚΤΙΚΑ
+  dewey: 938.26 ΧΣ
+  entry_numbers:
+  - '22923'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2004
+  pages: 760
+  topics:
+  - ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ Α ΚΑΙ Β
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17520
+    1: Χ.Σ
+    2: Ζ ΠΑΝΙΟΝΙΟ ΣΥΝΕΔΡΙΟ - ΠΡΑΚΤΙΚΑ
+    4: 938.26Χ.Σ
+    5: '22923'
+    9: ΑΘΗΝΑ
+    10: '2004'
+    11: '760'
+    12: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    13: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    14: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ Α ΚΑΙ Β
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17521
+  authors: []
+  title: ΣΤ ΔΙΕΘΝΕΣ ΠΑΝΙΟΝΙΟ ΣΥΝΕΔΡΙΟ - ΠΡΑΚΤΙΚΑ
+  dewey: 938.26 ΧΣ
+  entry_numbers:
+  - '22922'
+  editor: None // ΑΘΗΝΑ
+  edition_year: 2001
+  pages: 662
+  topics:
+  - ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17521
+    1: Χ.Σ
+    2: ΣΤ ΔΙΕΘΝΕΣ ΠΑΝΙΟΝΙΟ ΣΥΝΕΔΡΙΟ - ΠΡΑΚΤΙΚΑ
+    4: 938.26Χ.Σ
+    5: '22922'
+    9: ΑΘΗΝΑ
+    10: '2001'
+    11: '662'
+    12: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    13: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    14: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17522
+  authors: []
+  title: Β ΔΙΕΘΝΕΣ ΙΣΤΟΡΙΚΟ ΚΑΙ ΑΡΧΑΙΟΛΟΓΙΚΟ ΣΥΝΕΔΡΙΟ ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ
+  dewey: 938.106 ΧΣ
+  entry_numbers:
+  - '22912'
+  editor: None // ΑΓΡΙΝΙΟ
+  edition_year: 2004
+  pages: 1150
+  topics:
+  - ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  notes: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ Α ΚΑΙ Β
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17522
+    1: Χ.Σ
+    2: Β ΔΙΕΘΝΕΣ ΙΣΤΟΡΙΚΟ ΚΑΙ ΑΡΧΑΙΟΛΟΓΙΚΟ ΣΥΝΕΔΡΙΟ ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ
+    4: 938.106Χ.Σ
+    5: '22912'
+    9: ΑΓΡΙΝΙΟ
+    10: '2004'
+    11: '1150'
+    12: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    13: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    14: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+    17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ Α ΚΑΙ Β
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17523
+  authors:
+  - ΣΑΙΞΠΗΡ
+  title: ΟΝΕΙΡΟ ΚΑΛΟΚΑΙΡΙΝΗΣ ΝΥΧΤΑΣ
+  dewey: 822.33 ΣΑΙ
+  entry_numbers:
+  - '22926'
+  pages: 30
+  topics:
+  - ΘΕΑΤΡΟ
+  notes: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗΣ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17523
+    1: ΣΑΙΞΠΗΡ
+    2: ΟΝΕΙΡΟ ΚΑΛΟΚΑΙΡΙΝΗΣ ΝΥΧΤΑΣ
+    4: 822.33ΣΑΙ
+    5: '22926'
+    11: '30'
+    12: ΘΕΑΤΡΟ
+    13: ΘΕΑΤΡΟ
+    14: ΘΕΑΤΡΟ
+    17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗΣ
+    3: null
+    6: null
+    7: null
+    8: null
+    9: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17524
+  authors:
+  - ΙΨΕΝ
+  title: ΜΝΗΣΤΗΡΕΣ ΤΟΥ ΘΡΟΝΟΥ
+  dewey: 839.82 ΙΨΕ
+  entry_numbers:
+  - '22927'
+  editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
+  edition_year: 1975
+  pages: 192
+  topics:
+  - ΘΕΑΤΡΟ
+  notes: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17524
+    1: ΙΨΕΝ
+    2: ΜΝΗΣΤΗΡΕΣ ΤΟΥ ΘΡΟΝΟΥ
+    4: 839.82ΙΨΕ
+    5: '22927'
+    8: ΔΩΔΩΝΗ
+    9: ΑΘΗΝΑ
+    10: '1975'
+    11: '192'
+    12: ΘΕΑΤΡΟ
+    13: ΘΕΑΤΡΟ
+    14: ΘΕΑΤΡΟ
+    17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17525
+  authors:
+  - ΛΥΠΟΥΡΛΗΣ,ΔΗΜΗΤΡΙΟΣ
+  title: ΙΠΠΟΚΡΑΤΗΣ - ΙΑΤΡΙΚΗ ΔΕΟΝΤΟΛΟΓΙΑ ΚΑΙ ΝΟΣΟΛΟΓΙΑ
+  dewey: 887.3 ΛΥΠ
+  entry_numbers:
+  - '22928'
+  editor: ΖΗΤΡΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 2001
+  pages: 496
+  topics:
+  - ΑΡΧΑΙΟ ΚΕΙΜΕΝΟ
+  notes: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17525
+    1: ΛΥΠΟΥΡΛΗΣ,ΔΗΜΗΤΡΙΟΣ
+    2: ΙΠΠΟΚΡΑΤΗΣ - ΙΑΤΡΙΚΗ ΔΕΟΝΤΟΛΟΓΙΑ ΚΑΙ ΝΟΣΟΛΟΓΙΑ
+    4: 887.3ΛΥΠ
+    5: '22928'
+    8: ΖΗΤΡΟΣ
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '2001'
+    11: '496'
+    12: ΑΡΧΑΙΟ ΚΕΙΜΕΝΟ
+    13: ΑΡΧΑΙΟ ΚΕΙΜΕΝΟ
+    14: ΑΡΧΑΙΟ ΚΕΙΜΕΝΟ
+    17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+    3: null
+    6: null
+    7: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17526
+  authors:
+  - ΚΟΛΛΑΤΟΥ,ΔΗΜΗΤΡΗ
+  title: Ο ΑΓΙΟΣ ΠΡΕΒΕΖΗΣ
+  dewey: 889.23 ΚΟΛ
+  entry_numbers:
+  - '22931'
+  editor: ΠΕΜΠΤΗ ΕΠΟΧΗ // ΠΡΕΒΕΖΑ
+  pages: 175
+  topics:
+  - ΘΕΑΤΡΟ
+  notes: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17526
+    1: ΚΟΛΛΑΤΟΥ,ΔΗΜΗΤΡΗ
+    2: Ο ΑΓΙΟΣ ΠΡΕΒΕΖΗΣ
+    4: 889.23ΚΟΛ
+    5: '22931'
+    8: ΠΕΜΠΤΗ ΕΠΟΧΗ
+    9: ΠΡΕΒΕΖΑ
+    11: '175'
+    12: ΘΕΑΤΡΟ
+    13: ΘΕΑΤΡΟ
+    14: ΘΕΑΤΡΟ
+    17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+    3: null
+    6: null
+    7: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17527
+  authors:
+  - ΡΩΤΑ,ΒΑΣΙΛΗ
+  title: ΘΕΑΤΡΟ
+  dewey: 889.23 ΡΩΤ
+  entry_numbers:
+  - '22929'
+  editor: ΙΚΑΡΟΣ // None
+  pages: 285
+  topics:
+  - ΘΕΑΤΡΟ
+  notes: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ - 2 ΒΙΒΛΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17527
+    1: ΡΩΤΑ,ΒΑΣΙΛΗ
+    2: ΘΕΑΤΡΟ
+    4: 889.23ΡΩΤ
+    5: '22929'
+    8: ΙΚΑΡΟΣ
+    11: '285'
+    12: ΘΕΑΤΡΟ
+    13: ΘΕΑΤΡΟ
+    14: ΘΕΑΤΡΟ
+    17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ - 2 ΒΙΒΛΙΑ
+    3: null
+    6: null
+    7: null
+    9: null
+    10: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17528
+  authors:
+  - ΦΩΤΙΑΔΟΥ,ΜΑΡΙΑ
+  title: ΟΜΑΔΕΣ ΑΙΜΑΤΟΣ-RH-ΑΙΜΟΛΥΤΙΚΗ ΑΝΑΙΜΙΑ ΤΩΝ ΝΕΟΓΝΩΝ
+  entry_numbers:
+  - '22930'
+  editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
+  edition_year: 1980
+  pages: 38
+  topics:
+  - ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
+  notes: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  original_entry:
+    0: 17528
+    1: ΦΩΤΙΑΔΟΥ,ΜΑΡΙΑ
+    2: ΟΜΑΔΕΣ ΑΙΜΑΤΟΣ-RH-ΑΙΜΟΛΥΤΙΚΗ ΑΝΑΙΜΙΑ ΤΩΝ ΝΕΟΓΝΩΝ
+    4: 610.73ΦΩΤ0
+    5: '22930'
+    9: ΘΕΣΣΑΛΟΝΙΚ
+    10: '1980'
+    11: '38'
+    12: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
+    13: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
+    14: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
+    17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+    3: null
+    6: null
+    7: null
+    8: null
+    15: null
+    16: null
+    18: null
+    19: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
     27: null
     28: null
     29: null
     30: null
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/editor_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/editor_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/entries.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/entries.yml`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
   13: ΜΑΚΡΥΓΙΑΝΝΗΣ-ΣΕΦΕΡΗΣ
   14: ΣΕΦΕΡΗΣ-ΜΑΚΡΥΓΙΑΝΝΗΣ
   17: 2 ΑΝΤΙΤΥΠΑ
   22: ΣΥΝΑΝΤΗΣΗ
 - 0: 16
   1: ΑΛΕΞΙΟΥ,ΑΘΑΝΑΣΙΟΣ
   2: ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ
-  4: 938 ΑΛΕ
+  4: 938ΑΛΕ
   5: '2055'
   7: 15ΕΚΔ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 806Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΕΝΙΚΗ
@@ -269,15 +269,15 @@
   13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   14: ΒΥΖΑΝΤΙΝΗ ΑΥΤΟΡΑΤΟΡΙΑ-395Μ.Χ-867Μ.Χ
   15: ΒΥΖΑΝΤΙΟ-ΙΣΤΟΡΙΑ
 - 0: 21
   1: ΑΜΑΝΤΟΣ,Ι.ΚΩΝΣΤΑΝΤΙΝΟΣ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΑΔΟΣ
   3: ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΤΟΥ 1071Μ.Χ
-  4: 938 ΑΜΑ
+  4: 938ΑΜΑ
   5: '1916'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 29ΙΣ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΟΤΗΤΑ-ΙΟ71Μ.Χ
@@ -308,17 +308,17 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΛΑΣΣΙΚΟΙ ΧΡΟΝΟΙ-ΜΥΡΙΟΙ
   13: ΚΛΑΣΙΚΟΙ ΧΡΟΝΟΙ-ΚΑΘΟΔΟΣ ΜΥΡΙΩΝ
   14: ΚΑΘΟΔΟΣ ΜΥΡΙΩΝ
   15: ΜΥΡΙΟΙ
   18: ΕΙΚ.ΧΑΡΤΕΣ
   22: ΚΑΘΟΔΟΣ
 - 0: 24
-  1: ΑΝΑΓΝΩΣΤΑΚΗΣ,ΗΛΙΑΣ    .
+  1: ΙΕΡΟΜΟΝΑΧΟΥ,ΕΥΘΥΜΙΟΥ
   2: ΧΡΟΝΙΚΟ ΓΑΛΑΞΕΙΔΙΟΥ
-  4: 938.91 ΑΝΑ
+  4: 938.91ΙΕΡ
   5: '1725'
   8: ΑΚΡΙΤΑ
   9: ΑΘΗΝΑ
   10: '1985'
   11: 93Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΑΛΑΞΕΙΔΙ
   13: ΓΑΛΑΞΕΙΔΙ-ΧΡΟΝΙΚΟ
@@ -423,30 +423,30 @@
   12: ΠΑΓΚΟΣΜΙΑ ΛΟΓΟΤΕΧΝΙΑ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   13: ΠΑΓΚΟΣΜΙΟΣ-ΚΙΝΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   14: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   15: ΜΙΚΕΛΑΝΤΖΕΛΟ
 - 0: 32
   1: ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ ΕΜΜ
   2: ΕΛΛΗΝΙΣΜΟΣ ΚΑΙ ΔΗΜΟΚΡΑΤΙΑ
-  4: 938 ΑΝΤ
+  4: 938ΑΝΤ
   5: '2533'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1971'
   11: 607Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΗΜΟΚΡΑΤΙΑ
   13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ ΚΑΙ ΔΗΜΟΚΡΑΤΙΑ
   15: ΔΗΜΟΚΡΑΤΙΑ-ΕΛΛΗΝΙΣΜΟΣ
   22: ΕΛΛΗΝΙΣΜΟΣ
 - 0: 33
   1: ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ ΕΜΜ
   2: Η ΕΠΑΡΧΙΑ
   3: ΕΛΛΑΔΑ ΔΕΝ ΕΙΝΑΙ ΜΟΝΑΧΑ Η ΑΘΗΝΑ
-  4: 938 ΑΝΤ
+  4: 938ΑΝΤ
   5: '2522'
   7: 2ΕΚΔ
   8: ΗΠΕΙΡΩΤΙΚΗ ΕΣΤΙΑ
   9: ΙΩΑΝΝΙΝΑ
   10: '1953'
   11: 184Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΡΧΙΑ
@@ -650,15 +650,15 @@
   14: ΛΟΓΙΟΙ-ΤΟΥΡΚΟΚΡΑΤΙΑ-ΒΙΟΓΡΑΦΙΚΗ ΣΥΛΛΟΓΗ
   15: ΒΙΟΓΡΑΦΙΚΗ ΣΥΛΛΟΓΗ-ΛΟΓΙΟΙ
   22: ΛΟΓΙΩΝ
   23: ΒΙΟΓΡΑΦΙΚΗ
 - 0: 48
   1: ΑΡΓΥΡΟΣ,ΣΠΥΡΙΔΩΝΟΣ
   2: Η ΠΕΙΡΑΤΕΙΑ ΑΠΟ ΤΟ 1500 Π.Χ ΕΩΣ ΤΟ 1860
-  4: 938 ΑΡΓ
+  4: 938ΑΡΓ
   5: '2319'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1956'
   11: 192Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΕΙΡΑΤΕΙΑ-1550Π.Χ-1860
   13: ΠΕΙΡΑΤΕΙΑ-1550Π.Χ-1860
@@ -777,30 +777,30 @@
   11: 67Σ
   12: ΠΑΓΚΟΣΜΙΑ ΙΣΤΟΡΙΑ-ΓΗ
   13: ΓΗ-ΙΣΤΟΡΙΑ
   22: ΣΤΡΟΓΓΥΛΗ
 - 0: 57
   1: ΑΣΤΡΙΝΟΣ,ΘΕΜΗΣ
   2: Η ΜΕΓΑΛΗ ΙΔΕΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  4: 938 ΑΣΤ
+  4: 938ΑΣΤ
   5: '2484'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1945'
   11: 230Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΛΗ ΙΔΕΑ
   13: ΕΛΛΗΝΙΣΜΟΣ-ΜΕΛΑΛΗ ΙΔΕΑ
   14: ΜΕΓΑΛΗ ΙΔΕΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
   22: ΙΔΕΑ
   23: ΜΕΓΑΛΗ
   24: ΕΛΛΗΝΙΣΜΟΥ
 - 0: 58
   1: ΑΣΩΠΙΟΣ,ΕΙΡΗΝΑΙΟΣ Κ
   2: ΠΑΛΑΙΑ ΚΑΙ ΝΕΑ
-  4: 938 ΑΣΩ
+  4: 938ΑΣΩ
   5: '2102'
   8: ΣΑΚΕΛΛΑΡΙΟΥ
   9: ΑΘΗΝΑ
   10: '1903'
   11: 672Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΑΜΝΗΣΕΙΣ-1845
   13: ΙΤΑΛΙΑ-ΑΝΑΜΝΗΣΕΙΣ-1845
@@ -961,15 +961,15 @@
   10: '1940'
   11: 395Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   13: ΠΑΠΑΔΙΑΜΑΝΤΗΣ-ΖΩΗ ΚΑΙ ΕΡΓΟ
 - 0: 70
   1: ΒΑΛΕΤΑΣ,Γ
   2: ΤΟ ΠΡΟΔΟΜΕΝΟ ΕΙΚΟΣΙΕΝΑ
-  4: 938.5 ΒΑΛ
+  4: 938.5ΒΑΛ
   5: '1845'
   7: 2ΕΚΔ
   8: ΦΙΛΙΠΠΟΤΗ
   9: ΑΘΗΝΑ
   10: '1979'
   11: 195Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΙΚΟΣΙΕΝΑ
@@ -1528,28 +1528,28 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΒΕΝΕΖΗΣ
   14: ΒΕΝΕΖΗΣ-ΜΥΘΙΣΤΟΡΗΜΑ
   15: ΜΥΘΙΣΤΟΡΗΜΑ-ΒΕΝΕΖΗΣ
 - 0: 111
   1: ΒΕΝΙΖΕΛΟΣ,ΕΛΕΥΘΕΡΙΟΣ
   2: ΙΔΙΟΓΡΑΦΟΝ ΗΜΕΡΟΛΟΓΙΟ
-  4: 938.672ΒΕΝ
+  4: 938.672Χ.Σ
   5: '2115'
   8: Χ.Ε
   9: ΧΑΝΙΑ
   10: '1979'
   11: 57Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ-ΗΜΕΡΟΛΟΓΙΟ
   13: ΒΕΝΙΖΕΛΟΣ-ΗΜΕΡΟΛΟΓΙΟ
   14: ΗΜΕΡΟΛΟΓΙΟ-ΒΕΝΙΖΕΛΟΣ
   22: ΙΔΙΟΓΡΑΦΟΝ
 - 0: 112
-  1: ΒΕΝΙΖΕΛΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  1: ΣΤΕΦΑΝΟΥ,Σ.Ι.
   2: ΠΟΛΙΤΙΚΑΙ ΥΠΟΘΗΚΑΙ
-  4: 938.672ΒΕΝ
+  4: 938.672ΣΤΕ
   5: 2391-2784-2785
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1965'
   11: 306Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ-ΠΟΛΙΤΙΚΑΙ ΥΠΟΘΗΚΑΙ
   13: ΒΕΝΙΖΕΛΟΣ-ΠΟΛΙΤΙΚΑΙ ΥΠΟΘΗΚΑΙ
@@ -1567,15 +1567,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΡΗΤΗ-ΕΠΑΝΑΣΤΑΣΗ 1889
   13: ΚΡΗΤΗ-ΕΠΑΝΑΣΤΑΣΗ 1889
   14: ΕΠΑΝΑΣΤΑΣΗ 1889-ΚΡΗΤΗ
   15: ΚΡΗΤΙΚΗ ΕΠΑΝΑΣΤΑΣΗ 1889
 - 0: 114
   1: ΒΕΡΕΜΗΣ,ΘΑΝΟΣ
   2: ΟΙ ΕΠΕΜΒΑΣΕΙΣ ΤΟΥ ΣΤΡΑΤΟΥ ΣΤΗΝ ΕΛΛΗΝΙΚΗ ΠΟΛΙΤΙΚΗ 1916-1936
-  4: 938.7 ΒΕΡ
+  4: 938.7ΒΕΡ
   5: '2010'
   8: ΕΞΑΝΤΑΣ
   9: ΑΘΗΝΑ
   10: '1977'
   11: 467Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΤΡΑΤΟΣ-(1916-1936)
   13: ΣΤΡΑΤΟΣ-(1916-1936)-ΕΠΕΜΒΑΣΕΙΣ
@@ -1674,27 +1674,22 @@
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 199Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ-ΒΙΟΓΡΑΦΙΑ
   13: ΚΑΡΑΙΣΚΑΚΗΣ-ΒΙΟΓΡΑΦΙΑ
   14: ΒΙΟΓΡΑΦΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ
 - 0: 122
-  1: ΒΟΓΑΣ,ΙΩΑΝΝΗΣ
-  2: Η ΘΕΣΙΣ ΤΟΥ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟΥ ΖΗΤΗΜΑΤΟΣ
-  4: 938.751ΒΟΓ
-  5: 2024-2762-2739
-  8: Χ.Ε
-  9: ΑΘΗΝΑ
-  10: '1970'
-  11: 26Σ
-  12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
-  13: ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
-  14: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ-ΘΕΣΕΙΣ
-  21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ 30
-  22: ΘΕΣΙΣ
+  1: ΔΙΑΜΑΝΤΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  2: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ ΚΑΙ ΧΕΙΡΟΓΡΑΦΑ
+  4: 938.915ΔΙΑ
+  5: '22924'
+  11: '32'
+  12: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ-ΧΕΙΡΟΓΡΑΦΑ
+  13: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ-ΧΕΙΡΟΓΡΑΦΑ
+  14: ΕΥΒΟΙΚΑ ΕΓΓΡΑΦΑ-ΧΕΙΡΟΓΡΑΦΑ
 - 0: 123
   1: ΒΟΓΑΣΑΡΗΣ,ΑΓΓΕΛΟΣ
   2: ΑΝΔΡΕΑΣ ΚΑΛΒΟΣ
   4: 889.23 ΒΟΓ
   5: '1212'
   8: ΒΑΚΩΝ
   9: ΑΘΗΝΑ
@@ -1825,15 +1820,15 @@
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΑΛΗ ΠΑΣΑΣ
   14: ΑΛΗ ΠΑΣΑΣ-ΤΕΠΕΛΕΝΛΗΣ
   22: ΤΕΠΕΛΕΝΛΗΣ
 - 0: 133
   1: ΒΟΥΡΝΑΣ,ΤΑΣΟΣ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΩΤΕΡΗΣ ΕΛΛΑΔΑΣ
   3: ΑΠΟ ΤΗΝ ΕΠΑΝΑΣΤΑΣΗ ΤΟΥ 1821 ΩΣ ΤΟ ΚΙΝΗΜΑ ΤΟΥ ΓΟΥΔΙ(1909)
-  4: 938.5 ΒΟΥ
+  4: 938.7ΒΟΥ
   5: '1846'
   8: ΤΟΛΙΔΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 620Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-(1821-1909)
   13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΟΥΔΙ-ΚΙΝΗΜΑ-1909
@@ -3273,15 +3268,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
   13: ΠΟΛΕΜΟΣ-ΚΙΝΔΥΝΟΙ-ΑΜΥΝΑ
   14: ΑΜΥΝΑ-ΠΟΛΕΜΟΣ
   15: ΚΙΝΔΥΝΟΙ ΠΟΛΕΜΟΥ
 - 0: 243
   1: ΔΙΑΚΟΓΙΑΝΝΗΣ,ΚΥΡΙΑΚΟΣ Ι
   2: ΟΙ ΣΑΡΚΟΦΑΓΟΙ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  4: 938.8 ΔΙΑ
+  4: 938.8ΔΙΑ
   5: '2314'
   8: ΛΑΔΙΑ
   9: ΑΘΗΝΑ
   10: '1979'
   11: 557Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΗΜΟΚΡΑΤΙΑ
   13: ΔΗΜΟΚΡΑΤΙΑ-ΙΣΤΟΡΙΑ
@@ -3444,54 +3439,54 @@
   13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   14: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   15: ΠΑΠΑΙΩΑΝΝΟΥ-ΔΙΑΜΑΝΤΗ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 256
   1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
   2: ΤΟ ΝΗΣΙ ΤΟΥ ΗΛΙΟΥ
-  4: 889.1 ΔΙΑ
+  4: 889.1ΔΙΑ
   5: '346'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1982'
   11: 69Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΥΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   14: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   15: ΤΑΞΙΔΙΩΤΙΚΟ
 - 0: 257
   1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
   2: ΦΩΝΕΣ ΣΤΟ ΧΑΟΣ
-  4: 889.1 ΔΙΑ
+  4: 889.1ΔΙΑ
   5: '1198'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1986'
   11: 46Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   14: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   15: ΠΑΠΑΙΩΑΝΝΟΥ-ΔΙΑΜΑΝΤΗ
 - 0: 258
   1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
   2: Η ΤΕΛΕΥΤΑΙΑ ΦΛΟΓΑ
-  4: 889.1 ΔΙΑ
+  4: 889.1ΔΙΑ
   5: '1201'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1983'
   11: 119Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ
   14: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   15: ΠΑΠΑΙΩΑΝΝΟΥ-ΔΙΑΜΑΝΤΗ
 - 0: 259
   1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
   2: ΑΝΕΜΩΝΕΣ ΣΤΗ ΘΥΕΛΛΑ
-  4: 889.1 ΔΙΑ
+  4: 889.1ΔΙΑ
   5: 1200-1199
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 58Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΝΝΟΥ
@@ -3669,15 +3664,15 @@
   11: 110Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
   13: ΕΥΡΩΠΗ-ΙΣΤΟΡΙΑ
   14: ΠΟΛΕΜΟΣ-ΕΥΡΩΠΗ
 - 0: 273
   1: ΔΡΟΣΟΠΟΥΛΟΣ,Κ Η
   2: ΟΙ ΑΘΗΝΑΙΟΙ ΩΣ ΠΟΛΕΜΙΣΤΑΙ
-  4: 938.13 ΔΡΟ
+  4: 938.13ΔΡΟ
   5: '2321'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1944'
   11: 15Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ-ΑΘΗΝΑΙΟΙ
   13: ΑΘΗΝΑ-ΑΡΧΑΙΑ
@@ -3705,17 +3700,17 @@
   9: ΑΘΗΝΑ
   10: '1962'
   11: 304Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΙΣΤΟΡΙΑ
   14: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
 - 0: 276
-  1: ΕΙΣΙΤΑΛ,ΚΟΥΣΤΑΒ
+  1: EICHTHAL,GUSTAVE
   2: Η ΕΛΛΑΣ ΤΟΥ 1833-1835
-  4: 938.62 ΕΙΣ
+  4: 938.62EIC
   5: '2501'
   6: ΒΙΚΕΛΑ,Δ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1968'
   11: 120Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
@@ -4294,15 +4289,15 @@
   11: 268Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΜΑΚΕΔΟΝΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   14: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
 - 0: 321
   1: ΖΑΝΑΝΤΡΙΣ,ΚΑΣ
   2: ΕΛΛΗΝΕΣ ΑΔΕΡΦΟΙ ΜΟΥ ΑΣ ΠΟΛΕΜΗΣΩΜΕΝ
-  4: 938 ΖΑΝ
+  4: 938ΖΑΝ
   5: '2558'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1948'
   11: 88Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ ΤΗΣ ΠΕΝΝΑΣ
   13: ΠΟΛΕΜΟΣ ΤΗΣ ΠΕΝΝΑΣ
@@ -4330,15 +4325,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΕΚΕΜΒΡΙΑΝΑ
   13: ΔΕΚΕΜΒΡΙΑΝΑ-ΙΣΤΟΡΙΑ
   14: ΛΑΙΚΗ ΑΝΤΙΣΤΑΣΗ
   15: 1944-ΔΕΚΕΜΒΡΙΑΝΑ
 - 0: 324
   1: ΖΕΝΕΒΟΥΑ,ΜΩΡΙΣ
   2: Η ΕΛΛΑΣ ΤΟΥ ΚΑΡΑΜΑΝΛΗ Ή Η ΔΗΜΟΚΡΑΤΙΑ ΔΥΣΧΕΡΗΣ
-  4: 938.792ΖΕΝ
+  4: 938.497ΖΕΝ
   5: '2575'
   8: ΣΙΔΕΡΗΣ
   9: ΑΘΗΝΑ
   10: '1972'
   11: 270Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΗΜΟΚΡΑΤΙΑ
   13: ΔΗΜΟΚΡΑΤΙΑ-ΚΑΡΑΜΑΝΛΗΣ
@@ -4591,28 +4586,28 @@
   13: ΟΘΩΝΑΣ-ΜΑΥΡΟΚΟΡΔΑΤΟΣ-ΠΟΤΙΚΕΣ ΔΙΑΦΩΝΙΕΣ
   14: ΜΑΥΡΟΚΟΡΔΑΤΟΣ-ΟΘΩΝΑΣ-ΠΟΛΙΤΙΚΕΣ ΔΙΑΦΩΝΙΕΣ
   15: 1821-ΠΟΛΙΤΙΚΕΣ ΔΙΑΦΩΝΙΕΣ
   22: ΔΙΑΣΤΑΣΗ
 - 0: 344
   1: ΘΕΟΔΩΡΑΚΟΠΟΥΛΟΣ,Ι.Ν
   2: ΤΟ ΠΝΕΥΜΑ ΤΟΥ ΝΕΟΕΛΛΗΝΙΣΜΟΥ ΚΑΙ Η ΤΡΟΠΗ ΤΩΝ ΚΑΙΡΩΝ
-  4: 938 ΘΕΟ
+  4: 938ΘΕΟ
   5: '2506'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1945'
   11: 64Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΕΟΕΛΛΗΝΙΣΜΟΣ
   13: ΝΕΟΕΛΛΗΝΙΣΜΟΣ
   14: ΠΝΕΥΜΑ ΝΕΟΕΛΛΗΝΙΣΜΟΥ
   15: ΠΡΟΒΛΗΜΑΤΑ ΚΑΙΡΩΝ
 - 0: 345
   1: ΘΕΟΔΩΡΟΠΟΥΛΟΥ-ΛΙΒΑΔΑ,ΒΑΡΒΑΡΑ
   2: Ο ΕΓΚΑΙΝΙΣΤΗΣ ΚΑΙ ΠΡΩΤΟΣ ΣΠΟΡΕΥΣ ΤΟΥ ΡΙΖΟΣΠΑΣΤΙΣΜΟΥ
-  4: 938 ΘΕΟ
+  4: 938ΘΕΟ
   5: '1970'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1966'
   11: 99Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΙΖΟΣΠΑΣΤΙΣΜΟΣ
   13: ΡΙΖΟΣΠΑΣΤΙΣΜΟΣ-ΛΙΒΑΔΑΣ
@@ -4820,42 +4815,42 @@
   9: ΑΘΗΝΑ
   10: '1962'
   11: 254Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ
   13: ΤΑΞΙΔΙΑ-ΕΚΔΡΟΜΕΣ
   14: ΕΚΔΡΟΜΕΣ
 - 0: 362
-  1: ΘΥΕΡ,ΑΜΕΝΤ
+  1: THIERRY,AMEDEE
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΑΤΤΙΛΑ ΚΑΙ ΤΩΝ ΔΙΑΔΟΧΩΝ ΑΥΤΟΥ
-  4: 938.322ΘΥΕ
+  4: 938.322THI
   5: 1764-1982-1984
   6: ΒΟΥΤΥΡΑΣ,Σ.Ι
   8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '1903'
   11: 603Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΕΠΙΔΡΟΜΕΣ
   14: ΑΤΤΙΛΑΣ-ΕΠΙΔΡΟΜΕΣ
 - 0: 363
   1: ΘΡΥΛΟΣ,ΑΛΚΗΣ
   2: ΤΟ ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ
-  4: 886.2 ΘΡΥ
+  4: 886.2ΘΡΥ
   5: 1414-1415-1416-1417-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 491Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-(1927-1955)
   14: ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
 - 0: 364
   1: ΘΡΥΛΟΣ,ΑΛΚΗΣ
   2: ΜΟΡΦΕΣ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΠΕΖΟΓΡΑΦΙΑΣ
-  4: 880.3 ΘΡΥ
+  4: 880.3ΘΡΥ
   5: '210'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 242Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -4873,15 +4868,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΣΟΛΩΜΟΣ
   15: ΣΟΛΩΜΟΣ
 - 0: 366
   1: ΘΡΥΛΟΣ,ΑΛΚΗΣ
   2: ΜΟΡΦΕΣ ΚΑΙ ΘΕΜΑΤΑ ΤΟΥ ΘΕΑΤΡΟΥ
-  4: 886.2 ΘΡΥ
+  4: 886.2ΘΡΥ
   5: 1413-1412
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1961'
   11: 271Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΜΟΡΦΕΣ ΚΑΙ ΘΕΜΑΤΑ
@@ -4926,15 +4921,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   15: ΠΑΛΑΜΑΣ
 - 0: 370
   1: ΙΑΚΩΒΙΔΗ,ΛΙΛΗ
   2: ΘΕΑΤΡΟ
-  4: 886.2 ΙΑΚ
+  4: 886.2ΙΑΚ
   5: '1500'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 344Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
@@ -4950,29 +4945,29 @@
   11: 160Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
   13: ΚΑΠΟΔΙΣΤΡΙΑΣ
   14: ΚΥΒΕΡΝΗΤΗΣ ΤΗΣ ΕΛΛΑΔΟΣ
 - 0: 372
   1: ΙΨΕΝ,ΕΡΡΙΚΟΣ
   2: ΟΙ ΜΝΗΣΤΗΡΕΣ ΤΟΥ ΘΡΟΝΟΥ
-  4: 832 ΙΨΕ
+  4: 832ΙΨΕ
   5: '1371'
   6: ΚΑΣΤΡΟ,ΚΑΙΤΗ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: '1975'
   11: 192Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΓΕΡΜΑΝΙΑ
 - 0: 373
   1: ΙΨΕΝ,ΕΡΡΙΚΟΣ
   2: ΕΝΤΑ ΓΚΑΜΛΕΡ
   3: ΔΡΑΜΑ
-  4: 832 ΙΨΕ
+  4: 832ΙΨΕ
   5: 1398-8112
   6: ΚΟΥΚΟΥΛΑ,Λ
   8: ΓΚΟΒΟΣΤΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 142Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -4980,15 +4975,15 @@
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΓΕΡΜΑΝΙΑ
   15: ΔΡΑΜΑ-ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 374
   1: ΙΨΕΝ,ΕΡΡΙΚΟΣ
   2: Η ΓΙΟΡΤΗ ΣΤΟ ΣΟΛΧΑΟΥΓΚ
   3: ΔΡΑΜΑ
-  4: 832 ΙΨΕ
+  4: 832ΙΨΕ
   5: '1397'
   6: ΚΟΥΚΟΥΛΑ,Λ
   8: ΓΚΟΒΟΣΤΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 72Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -5007,15 +5002,15 @@
   11: 196Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΓΕΤΕΣ-ΚΑΡΑΜΑΝΛΗΣ
   13: ΗΓΕΤΕΣ-ΚΑΡΑΜΑΝΛΗΣ
   14: ΚΑΡΑΜΑΝΛΗΣ-ΗΓΕΤΕΣ
 - 0: 376
   1: ΙΩΑΝΝΙΔΗΣ,ΑΛΚΙΒΙΑΔΗΣ
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ
-  4: 938 ΙΩΑ
+  4: 938ΙΩΑ
   5: '2408'
   8: ΚΟΛΛΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1904'
   11: 112Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΘΝΟΣ
   13: ΕΘΝΟΣ-ΙΣΤΟΡΙΑ
@@ -5059,28 +5054,28 @@
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΠΟΙΗΜΑΤΑ-ΚΑΒΑΦΗΣ
   15: ΚΑΒΑΦΗΣ-ΠΟΙΗΜΑΤΑ
 - 0: 380
   1: ΚΑΒΒΑΘΑΣ,ΒΑΣΙΛΗΣ
   2: ΑΙΘΙΟΠΙΑ
   3: 13 ΜΗΝΕΣ ΗΛΙΑΣ 13 ΜΗΝΕΣ ΘΑΝΑΤΟΣ
-  4: 915.39 ΚΑΒ
+  4: 915.39ΚΑΒ
   5: 418-419
   8: ΑΛΚΥΩΝ
   9: ΑΘΗΝΑ
   10: '1984'
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΑΙΘΙΟΠΙΑ
   13: ΤΑΞΙΔΙΑ-ΑΙΘΙΟΠΙΑ
   14: ΑΙΘΙΟΠΙΑ-ΤΑΞΙΔΙΑ
   15: ΛΕΥΚΩΜΑ-ΑΙΘΙΟΠΙΑ
 - 0: 381
   1: ΚΑΒΑΝΕΣ,ΠΙΕΡ
   2: L'EPIRE DE LA MORT DE PYRROS
   3: A LA CONGUTE ROMAINE(272-167M.X)
-  4: 938.21 CAB
+  4: 938.21CAB
   5: '2177'
   8: X.E
   9: PARIS
   10: '1976'
   11: 644S
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-(272-167Μ.Χ)
   13: ΗΠΕΙΡΟΣ-(272-167Μ.Χ)
@@ -5617,29 +5612,29 @@
   11: 310Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
   14: ΘΕΑΤΡΙΚΑ ΕΡΓΑ-ΕΛΛΗΝΙΚΑ
 - 0: 422
   1: ΚΑΝΑΤΣΟΥΛΗΣ,ΔΗΜ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ ΜΕΧΡΙ ΤΟΥ ΜΕΓΑΛΟΥ ΚΩΝΣΑΝΤΙΝΟΥ
-  4: 938.21 ΚΑΝ
+  4: 938.21ΚΑΝ
   5: '2199'
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1964'
   11: 188Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΚΩΝΣΤΑΝΤΙΚΟΣ
   14: ΚΩΝΣΤΑΝΤΙΝΟΣ-ΜΑΚΕΔΟΝΙΑ
   18: ΧΑΡΤΕΣ
 - 0: 423
   1: ΚΑΝΑΤΣΟΥΛΗΣ,ΔΗΜ
   2: Η ΜΑΚΕΔΟΝΙΑ ΑΠΟ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ
   3: ΜΕΧΡΙ ΤΗΣ ΑΝΟΔΟΥ ΤΟΥ ΦΙΛΙΠΠΟΥ Β'
-  4: 938.21 ΚΑΝ
+  4: 938.21ΚΑΝ
   5: 2202-2203
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1976'
   11: 134Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΦΙΛΙΠΠΟΣ Β'
@@ -5670,15 +5665,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΙΣΤΟΡΙΑ
   14: ΕΠΟΠΟΙΙΑ-ΒΥΖΑΝΤΙΟ
   15: ΒΥΖΑΝΤΙΝΗ ΕΠΟΠΟΙΙΑ
 - 0: 426
   1: ΚΑΠΟΔΙΣΤΡΙΑΣ,ΙΩΑΝΝΗΣ
   2: ΑΡΧΕΙΟΝ ΙΩΑΝΝΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
-  4: 938.571ΚΑΠ
+  4: 938.571Χ.Σ
   5: 1779-1780-1781-1782-
   8: Χ.Ε
   9: ΚΕΡΚΥΡΑ
   10: '1976'
   11: 320Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
   13: ΚΑΠΟΔΙΣΤΡΙΑΣ-ΑΡΧΕΙΟ
@@ -6285,27 +6280,27 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΙΣΤΟΡΙΑ ΚΑΙ ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ-ΑΡΤΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 474
   1: ΚΑΣΙΜΑΤΗΣ,ΓΡΗΓ Π
   2: Η ΕΛΛΑΣ ΚΑΙ Ο ΚΟΣΜΟΣ
-  4: 938 ΚΑΣ
+  4: 938ΚΑΣ
   5: '2490'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1961'
   11: 422Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΟΣΜΟΣ
   13: ΕΛΛΑΣ-ΚΟΣΜΟΣ
   14: ΚΟΣΜΟΣ-ΕΛΛΑΣ
 - 0: 475
   1: ΚΑΣΙΜΑΤΗΣ,ΓΡΗΓ.Π
   2: ΤΟ ΜΗΝΥΜΑ ΤΟΥ ΓΚΑΝΤΙ
-  4: 938.001ΚΑΣ
+  4: 938ΚΑΣ
   5: '2339'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1969'
   11: 39Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΗΝΥΜΑ ΓΚΑΝΤΙ
   13: ΓΚΑΝΤΙ-ΜΗΝΥΜΑ
@@ -6345,15 +6340,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΦΩΚΙΔΑ-ΑΜΦΙΣΣΑ
   13: ΦΩΚΙΔΑ-ΑΜΦΙΣΣΑ-ΠΡΟΣΗΛΙΟ
   14: ΑΜΦΙΣΣΑ-ΠΡΟΣΗΛΙΟ
   15: ΠΡΟΣΗΛΙΟ
 - 0: 479
   1: ΚΑΣΤΟΡΙΑΔΗΣ,ΚΟΡΝΗΛΙΟΣ
   2: ΜΠΡΟΣΤΑ ΣΤΟΝ ΠΟΛΕΜΟ
-  4: 938.ΚΑΣ
+  4: 938ΚΑΣ
   5: '2503'
   6: ΧΡΙΣΤΟΦΙΔΗ-ΚΑΣΤΟΡΙΑΔ
   8: Χ.Ε
   9: ΠΑΡΙΣΙ
   10: '1981'
   11: 338Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
@@ -6566,15 +6561,15 @@
   13: ΓΕΩΓΡΑΦΟΙ-ΠΕΡΙΗΓΗΤΕΣ
   14: ΕΛΛΑΔΑ-ΤΑΞΙΔΙΑ
   15: ΠΕΡΙΗΓΗΤΕΣ-ΓΕΩΓΡΑΦΟΙ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 496
   1: ΚΟΚΚΙΝΗΣ,ΔΙΟΝΥΣΙΟΣ
   2: ΟΙ ΔΥΟ ΠΟΛΕΜΟΙ 1940-1941
-  4: 938.75 ΚΟΚ
+  4: 938.75ΚΟΚ
   5: '2404'
   8: Ο ΠΛΑΤΩΝ
   9: ΑΘΗΝΑ
   10: '1945'
   11: 310Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΙ-(1940-1941)
   13: ΠΟΛΕΜΟΙ-(1940-1941)
@@ -6661,15 +6656,15 @@
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΝΕΩΤΕΡΟ
   14: ΤΡΑΓΩΔΙΑ-ΑΡΧΑΙΑ
   15: ΑΡΧΑΙΑ ΤΡΑΓΩΔΙΑ-ΑΝΑΒΙΩΣΗ
 - 0: 503
   1: ΚΟΛΙΑΤΣΟΣ,ΧΡΗΣΤΟΣ
   2: ΣΕΛΙΔΕΣ ΔΟΞΗΣ
   3: ΓΡΑΜΜΕΝΕΣ ΜΕ ΤΟ ΑΙΜΑ ΤΩΝ ΠΑΙΔΙΩΝ ΤΗΣ ΕΛΛΑΔΟΣ ΕΙΣ ΤΑ Β.ΗΠΕΙΡΩ
-  4: 938.75 ΚΟΛ
+  4: 938.75ΚΟΛ
   5: 1958-2632
   7: 2ΕΚΔ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1948'
   11: 321Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ-1940
@@ -6728,15 +6723,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΓΕΤΕΣ
   13: ΗΓΕΤΕΣ-ΠΑΠΑΝΔΡΕΟΥ ΓΕΩΡΓΙΟΣ
   14: ΠΑΠΑΝΔΡΕΟΥ ΓΕΩΡΓΙΟΣ-ΒΙΟΓΡΑΦΙΑ
   15: ΒΙΟΓΡΑΦΙΑ-ΠΑΠΑΝΡΕΟΥ ΓΕΩΡΓΙΟΣ
 - 0: 508
   1: ΚΟΜΠΟΡΡΟΖΟΣ,ΙΩΑΝΝΗΣ
   2: ΕΛΛΑΔΑ ΚΑΙ ΜΟΝΟΝ ΕΛΛΑΔΑ
-  4: 938.75 ΚΟΜ
+  4: 938.75ΚΟΜ
   5: '2514'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1952'
   11: 120Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
   13: 1940-ΕΛΛΑΔΑ
@@ -6794,15 +6789,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΞΟΔΟΣ ΜΕΣΟΛΟΓΓΙΟΥ
   13: ΕΞΟΔΟΣ ΜΕΣΟΛΟΓΓΙΟΥ
   14: ΜΕΣΣΟΛΟΓΓΙ-ΕΛΕΥΘΕΡΟΙ ΠΟΛΙΟΡΚΗΜΕΝΟΙ
   15: ΠΑΠΑΔΙΑΜΑΝΤΟΠΟΥΛΟΣ-ΕΞΟΔΟΣ ΜΕΣΣΟΛΟΓΙΟΥ
 - 0: 513
   1: ΚΟΝΟΜΟΣ,ΝΤΙΝΟΣ
   2: ΗΠΕΙΡΩΤΕΣ ΣΤΗ ΖΑΚΥΝΘΟ
-  4: 938.93 ΚΟΝ
+  4: 938.93ΚΟΝ
   5: 2165-5257
   8: ΕΤΑΙΡ.ΗΠΕΙΡ.ΜΕΛΕΤΩΝ
   9: ΙΩΑΝΝΙΝΑ
   10: '1964'
   11: 72Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΕΣ
   13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΕΣ
@@ -6857,78 +6852,78 @@
   11: 303Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΙΑ-ΤΟΥΡΚΟΙ
   13: ΤΟΥΡΚΙΑ-ΤΟΥΡΚΟΙ
   14: ΤΟΥΡΚΟΙ-ΤΟΥΡΚΙΑ
 - 0: 518
   1: ΚΟΝΤΟΓΕΩΡΓΗΣ,ΓΕΩΡΓΙΟΣ Λ
   2: Η ΕΛΛΑΔΑ ΣΤΗΝ ΕΥΡΩΠΗ
-  4: 938.8 ΚΟΝ
+  4: 938.8ΚΟΝ
   5: '923'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 311Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
   13: ΕΥΡΩΠΗ-ΕΛΛΑΔΑ
   14: ΕΛΛΑΔΑ-ΕΥΡΩΠΗ
   15: ΚΑΡΑΜΑΝΛΗΣ-ΠΟΛΙΤΙΚΗ
 - 0: 519
   1: ΚΟΝΤΟΜΙΧΗΣ,ΠΑΝΤΑΖΗΣ
   2: ΤΟ ΝΕΟΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ ΣΤΗ ΛΕΥΚΑΔΑ (1800-1964)
-  4: 886.2 ΚΟΝ
+  4: 886.2ΚΟΝ
   5: 1428-1429
   8: ΜΕΛΙΣΣΑ
   9: ΑΘΗΝΑ
   10: '1964'
   11: 108Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΛΕΥΚΑΔΑ (1800-1964)
   14: ΛΕΥΚΑΔΑ-ΘΕΑΤΡΟ
   15: ΝΕΟΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΛΕΥΚΑΔΑ
 - 0: 520
   1: ΚΟΝΤΥΛΑΚΗΣ.Ι
   2: Ο ΠΑΤΟΥΧΑΣ
-  4: 889.38 ΚΟΝ
+  4: 889.38ΚΟΝ
   5: '1178'
   8: ΓΡΗΓΟΡΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 190Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΚΟΝΤΥΛΑΚΗΣ
   15: ΚΟΝΤΥΛΑΚΗΣ
 - 0: 521
   1: ΚΟΝΤΥΛΑΚΗΣ,Ι
   2: ΟΤΑΝ ΗΜΟΥΝ ΔΑΣΚΑΛΟΣ
-  4: 889.38 ΚΟΝ
+  4: 889.38ΚΟΝ
   5: '1179'
   8: ΓΡΗΓΟΡΗ
   9: ΑΘΗΝΑ
   10: '1972'
   11: 134Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΚΟΝΤΥΛΑΚΗΣ
   15: ΚΟΝΤΥΛΑΚΗΣ
 - 0: 522
   1: ΚΟΡΑΗΣ,Α
   2: ΠΡΟΔΡΟΜΟΣ ΕΛΛΗΝΙΚΗΣ ΒΙΒΛΙΟΘΗΚΗΣ
-  4: 880.08 ΚΟΡ
+  4: 880.08ΚΟΡ
   5: '1220'
   8: ΔΙΔΟΤΟΥ
   9: ΠΑΡΙΣΙ
   11: 425Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΚΟΡΑΗΣ
   14: ΚΟΡΑΗΣ
 - 0: 523
   1: ΚΟΡΑΗΣ,Α
   2: ΕΠΙΣΤΟΛΑΙ ΑΔΑΜΑΝΤΙΟΥ ΚΟΡΑΗ
-  4: 880.08 ΚΟΡ
+  4: 880.08ΚΟΡ
   5: 2683-2682-
   8: ΠΕΡΡΗ
   9: ΑΘΗΝΑ
   10: '1885'
   11: 1007Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΚΟΡΑΗΣ
@@ -7116,15 +7111,15 @@
   12: ΤΣΕΧΟΣΛΟΒΑΚΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΤΣΕΧΟΣΛΟΒΑΚΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΣΕΧΟΣΛΟΒΑΚΙΑ
   15: ΤΣΕΧΟΣΛΟΒΑΚΙΑ-ΘΕΑΤΡΟ
 - 0: 538
   1: ΚΟΥΡΟΥΚΛΗΣ,Γ
   2: ΤΟ ΠΟΛΕΜΙΚΟΝ ΗΜΕΡΟΛΟΓΙΟΝ ΤΗΣ Δ'ΜΟΙΡΑΣ ΠΥΡΟΒΟΛΙΚΟΥ
-  4: 938.75 ΚΟΥ
+  4: 938.75ΚΟΥ
   5: '2390'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1973'
   11: 185Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΙΚΟ ΗΜΕΡΟΛΟΓΙΟ 1941
   13: ΗΜΕΡΟΛΟΓΙΟ-ΠΟΛΕΜΙΚΟ-1941
@@ -7226,15 +7221,15 @@
   10: '1977'
   11: 58Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΟΞΑ ΣΟΥΛΙΟΥ
   13: ΔΟΞΑ ΣΟΥΛΙΟΥ-ΙΣΤΟΡΙΑ
   14: ΣΟΥΛΙ-ΔΟΞΑ
 - 0: 547
   1: ΚΡΑΨΙΤΗΣ,ΒΑΣΙΛΗΣ
-  2: ΟΙ ΜΟΥΣΑΛΜΑΝΟΙ ΤΣΑΜΗΔΕΣ ΤΗΣ ΘΕΣΠΡΩΤΙΑΣ
+  2: Η ΙΣΤΟΡΙΚΟΙ ΑΛΗΘΕΙΑ ΓΙΑ ΤΟΥΣ ΜΟΥΣΑΛΜΑΝΟΥΣ ΤΣΑΜΗΔΕΣ
   4: 938.492ΚΡΑ
   5: 2253-8783
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 236Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΠΡΩΤΙΑ
@@ -7555,15 +7550,15 @@
   11: 214Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΟΚΙΜΙΑ
   13: ΔΟΚΙΜΙΑ
 - 0: 572
   1: ΚΥΡΙΑΚΟΠΟΥΛΟΣ,ΚΩΣΤΑΣ
   2: ΣΕΛΙΔΕΣ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΤΩΝ ΕΛΛΗΝΩΝ
   3: ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΚΑΙ ΤΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ ΤΟΥ 21
-  4: 938 ΚΥΡ
+  4: 938ΚΥΡ
   5: '1911'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 453Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ ΕΩΣ 1821
   13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ
@@ -7607,15 +7602,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-Κ.Κ.Ε-ΠΟΛΕΜΟΣ (1940-1941)
   13: Κ.Κ.Ε-ΠΟΛΕΜΟΣ(1940-1941)
   14: 1940-Κ.Κ.Ε
   15: ΠΟΛΕΜΟΣ 194-1941
 - 0: 576
   1: ΚΩΝΣΤΑΝΤΟΠΟΥΛΟΣ,ΣΑΒΒΑΣ
   2: ΣΟΒΙΕΤΙΚΗ ΡΩΣΙΑ ΚΑΙ ΕΛΛΑΣ
-  4: 938 ΚΩΝ
+  4: 938ΚΩΝ
   5: '1683'
   8: ΕΛΕΥΘΕΡΟΣ ΚΟΣΜΟΣ
   9: ΑΘΗΝΑ
   10: '1968'
   11: 164Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΣΙΑ
   13: ΡΩΣΙΑ-ΕΛΛΑΣ
@@ -7674,27 +7669,27 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΛΒΑΝΙΑ
   13: ΑΛΒΑΝΙΑ-ΑΛΒΑΝΟΙ
   14: ΑΛΒΑΝΟΙ-ΑΛΒΑΝΙΚΗ ΠΡΟΠΑΓΑΝΔΑ
   15: ΠΡΟΠΑΓΑΝΔΑ-ΑΛΒΑΝΙΚΗ
 - 0: 581
   1: ΛΑΖΑΡΟΥ,ΑΝΑΣΤ
   2: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗ
-  4: 938 ΛΑΖ
+  4: 938ΛΑΖ
   5: '2407'
   8: ΟΕΣΒ
   9: ΑΘΗΝΑ
   10: '1940'
   11: 263Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   13: ΕΛΛΑΣ-ΙΣΤΟΡΙΑ
 - 0: 582
   1: ΛΑΖΑΡΙΔΗΣ,ΚΩΣΤΑΣ
   2: ΤΟ ΧΩΡΙΟ ΜΟΥ
   3: ΤΟ ΚΟΥΚΟΥΛΙ
-  4: 938.93 ΛΑΖ
+  4: 938.93ΛΑΖ
   5: '312'
   8: Χ.Ε
   9: ΓΙΑΝΝΙΝΑ
   10: '1977'
   11: 51Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΚΟΥΚΟΥΛΙ
@@ -7916,15 +7911,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΠΑΙΔΙΚΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΑΙΔΙΚΟ
   14: ΠΑΙΔΙΚΟ ΘΕΑΤΡΟ-ΚΟΥΚΛΟΘΕΑΤΡΟ
   15: ΚΟΥΚΛΟΘΕΑΤΡΟ
 - 0: 600
   1: ΛΑΠΠΑΣ,ΤΑΚΗΣ
   2: ΘΕΑΤΡΙΚΕΣ ΕΙΚΟΝΕΣ ΑΠ'ΤΟ ΕΙΚΟΣΙΕΝΑ
-  4: 886.2 ΛΑΠ
+  4: 886.2ΛΑΠ
   5: '2672'
   8: ΠΕΧΛΙΒΑΝΙΔΗΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 161Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΙΚΟΣΙΕΝΑ
@@ -7952,15 +7947,15 @@
   11: 148Σ
   12: ΕΛΛΗΝΙΚΗ  ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΛΑΣΚΑΡΑΤΟΣ
   14: ΛΑΣΚΑΡΑΤΟΣ
 - 0: 603
   1: ΛΑΣΚΑΡΙΣ,ΘΕΟΔΟΣΙΟΣ
   2: Ο ΔΙΑΚΟΣ ΣΤΟ ΜΟΝΑΣΤΗΡΙ ΚΑΙ ΚΡΥΣΤΑΛΛΩ
-  4: 886.2 ΛΑΣ
+  4: 886.2ΛΑΣ
   5: '1464'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 85Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
@@ -7993,66 +7988,66 @@
   13: ΘΕΣΣΑΛΙΑ-(1805-1810)
   14: 1805-ΘΕΣΣΑΛΙΑ
   15: '1810'
   16: ΘΕΣΣΑΛΙΑ
 - 0: 606
   1: ΛΕΣΚΥ,ΑΛΠΙΝ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-  4: 881.09 LES
+  4: 881.09ΛΕΣ
   5: '2563'
   8: ΚΥΡΙΑΚΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1978'
   11: 1271Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΑΡΧΑΙΑ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
 - 0: 607
   1: ΛΙΑΠΗΣ,ΚΩΣΤΑΣ
   2: ΣΕΛΙΔΕΣ ΑΠ'ΤΗΝ ΙΣΤΟΡΙΑ ΤΟΥ ΑΝΑΤΟΛΙΚΟΥ ΠΗΛΙΟΥ
-  4: 938.931ΛΙΑ
+  4: 931ΛΙΑ
   5: '2325'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1969'
   11: 56Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΣΑΛΙΑ
   13: ΘΕΣΣΑΛΙΑ-ΜΑΓΝΗΣΙΑ-ΠΗΛΙΟ
   14: ΜΑΓΝΗΣΙΑ-ΠΗΛΙΟ
   15: ΠΗΛΙΟ
 - 0: 608
   1: ΛΙΑΤΣΟΣ,ΔΗΜΗΤΡΙΟΣ Π
   2: Η ΒΑΥΑΡΟΚΡΑΤΙΑ ΚΑΙ ΟΙ ΑΓΩΝΙΣΤΕΣ ΤΟΥ '21
-  4: 938.5 ΛΙΑ
+  4: 938.5ΛΙΑ
   5: '1808'
   8: ΕΛΛΗΝΙΚΟ ΒΙΒΛΙΟ
   9: ΑΘΗΝΑ
   10: '1976'
   11: 119Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821-ΑΓΩΝΙΣΤΕΣ
   13: 1821-ΑΓΩΝΙΣΤΕΣ
   14: ΑΓΩΝΙΣΤΕΣ-1821
   15: ΒΑΥΑΡΟΚΡΑΤΙΑ
 - 0: 609
   1: ΛΙΔΩΡΙΚΗΣ,ΑΛΕΚΟΣ
   2: ΟΙ ΞΕΡΡΙΖΩΜΕΝΟΙ
-  4: 886.2 ΛΙΔ
+  4: 886.2ΛΙΔ
   5: '1588'
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: '1979'
   11: 119Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
   18: ΦΩΤ
 - 0: 610
   1: ΛΙΔΩΡΙΚΗΣ ΑΛΕΚΟΣ
   2: ΧΩΡΙΣ ΓΑΝΤΙ
   3: ΣΑΤΙΡΙΚΗ ΚΩΜΩΔΙΑ
-  4: 886.2 ΛΙΔ
+  4: 886.2ΛΙΔ
   5: '1362'
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 132Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΑΤΥΡΑ
   13: ΕΛΛΗΝΙΚΗ ΣΑΤΥΡΑ-ΕΡΓΟ
@@ -8069,29 +8064,29 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
   13: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ-ΛΙΟΥΝΤΖΗ
   14: ΛΙΟΥΝΤΖΗ-Β.ΗΠΕΙΡΟΣ
   15: Β.ΗΠΕΙΡΟΣ
 - 0: 612
   1: ΚΟΥΡΕΤΑΣ,Δ
   2: ΑΝΩΜΑΛΟΙ ΧΑΡΑΚΤΗΡΕΣ ΕΙΣ ΤΟ ΑΡΧΑΙΟΝ ΔΡΑΜΑ
-  4: 881.2 ΚΟΥ
+  4: 881.2ΚΟΥ
   5: '1445'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1951'
   11: 325Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
   14: ΔΡΑΜΑ-ΑΡΧΑΙΟ
   15: ΑΝΩΜΑΛΟΙ ΧΑΡΑΚΤΗΡΕΣ-ΔΡΑΜΑ
 - 0: 613
   1: ΛΑΔΙΑ,ΕΛΕΝΗ
   2: ΠΟΙΗΤΕΣ ΚΑΙ ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   3: ΣΙΚΕΛΙΑΝΟΣ-ΣΕΦΕΡΗΣ-ΠΑΠΑΔΙΤΣΑΣ
-  4: 881.2 ΛΑΔ
+  4: 881.2ΛΑΔ
   5: '225'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1983'
   11: 146Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΠΑΠΑΔΙΤΣΑΣ
@@ -8121,15 +8116,15 @@
   11: 55Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΚΡΥΣΤΑΛΛΗΣ
   14: ΚΡΥΣΤΑΛΛΗΣ
 - 0: 616
   1: ΛΑΣΚΑΡΗΣ,ΝΙΚΟΛΑΟΣ
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΝΕΟΕΛΛΗΝΙΚΟΥ ΘΕΑΤΡΟΥ
-  4: 886.2 ΛΑΣ
+  4: 886.2ΛΑΣ
   5: 1423-1424-1422-
   8: ΒΑΣΙΛΕΙΟΥ
   9: ΑΘΗΝΑ
   10: '1938'
   11: 333Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
@@ -8173,28 +8168,28 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΣΙΚΕΛΙΑΝΟΣ
   15: ΣΙΚΕΛΙΑΝΟΣ-ΚΡΙΤΙΚΗ ΜΕΛΕΤΗ
 - 0: 620
   1: ΛΟΓΟΘΕΤΗΣ,ΚΩΝΣΤ
   2: ΕΘΝΙΚΑ ΚΑΙ ΕΠΙΣΤΗΜΟΝΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
-  4: 938.04 ΛΟΓ
+  4: 938.04ΛΟΓ
   5: '2535'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1971'
   11: 563Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΛΕΤΗΜΑΤΑ
   13: ΜΕΛΕΤΗΜΑΤΑ-ΕΘΝΙΚΑ
   14: ΕΘΝΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
   15: ΕΠΙΣΤΗΜΟΝΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
 - 0: 621
   1: ΛΟΓΟΘΕΤΗΣ,ΚΩΝΣΤ.Ι.
   2: ΚΡΙΤΙΚΑ ΚΑΙ ΕΡΜΗΝΕΥΤΙΚΑ ΕΙΣ ΕΛΛΗΝΑΣ ΣΥΓΓΡΑΦΕΙΣ
-  4: 880.3 ΛΟΓ
+  4: 880.3ΛΟΓ
   5: 2699-2700
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 171Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΚΡΙΤΙΚΑ
@@ -8212,41 +8207,41 @@
   13: ΤΑΞΙΔΙΑ-ΡΟΔΟΣ
   14: ΡΟΔΟΣ-ΤΑΞΙΔΙΑ
   15: ΤΟΥΡΙΣΜΟΣ-ΡΟΔΟΣ
 - 0: 623
   1: ΛΥΓΙΖΟΣ,ΜΗΤΣΟΣ
   2: ΘΕΜΑΤΑ ΚΑΙ ΠΟΙΗΤΕΣ
   3: ΔΟΚΙΜΙΑ ΚΑΙ ΜΕΛΕΤΕΣ
-  4: 880.4 ΛΥΓ
+  4: 880.4ΛΥΓ
   5: '1007'
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: '1977'
   11: 396Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΔΟΚΙΜΙΑ
   15: ΔΟΚΙΜΙΑ-ΣΥΓΓΡΑΦΕΙΣ
 - 0: 624
   1: ΛΥΓΙΖΟΣ,ΜΗΤΣΟΣ
   2: ΤΟ ΝΕΟΕΛΛΗΝΙΚΟ ΠΛΑΙ ΣΤΟ ΠΑΓΚΟΣΜΙΟ ΘΕΑΤΡΟ
-  4: 886.2 ΛΥΓ
+  4: 886.2ΛΥΓ
   5: '1427'
   8: ΣΑΛΙΒΕΡΟΥ
   9: ΑΘΗΝΑ
   10: '1958'
   11: 672Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΑΓΚΟΣΜΙΟ
   14: ΠΑΓΚΟΣΜΙΟ ΘΕΑΤΡΟ-ΝΕΟΕΛΛΗΝΙΚΟ
   15: ΝΕΟΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΑΓΚΟΣΜΙΟ
 - 0: 625
   1: ΛΥΓΙΖΟΣ,ΜΗΤΣΟΣ
   2: ΤΟΜΗ ΣΤΟ ΣΥΓΧΡΟΝΟ ΘΕΑΤΡΟ
-  4: 886.2 ΛΥΓ
+  4: 886.2ΛΥΓ
   5: '1430'
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: '1975'
   11: 205Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΣΥΓΧΡΟΝΟ
@@ -8264,15 +8259,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΕΝΕΥΗ-ΣΥΜΒΑΣΕΙΣ
   13: ΓΕΝΕΥΗ-ΣΥΜΒΑΣΕΙΣ
   14: ΣΥΜΒΑΣΕΙΣ ΓΕΝΕΥΗΣ
   15: 1949-ΣΥΜΒΑΣΕΙΣ ΓΕΝΕΥΗΣ
 - 0: 627
   1: ΛΩΛΗΣ,ΝΙΚΟΛΑΟΣ Β.
   2: ΤΟΠΟΙ ΚΑΙ ΘΡΥΛΟΙ ΤΗΣ ΗΠΕΙΡΟΥ
-  4: 398 ΛΩΛ
+  4: 398ΛΩΛ
   5: '271'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1961'
   11: 76Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΗΠΕΙΡΟΣ
   13: ΤΑΞΙΔΙΑ-ΗΠΕΙΡΟΣ
@@ -8303,15 +8298,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΤΙΣΤΑΣΗ
   13: ΑΝΤΙΣΤΑΣΗ-(1941-1944)
   14: 1944-ΑΝΤΙΣΤΑΣΗ
   15: ΣΥΜΜΑΧΟΙ-1944
 - 0: 630
   1: ΜΑΚΡΗΣ,ΕΥΡΙΠΙΔΗΣ
   2: ΖΩΗ ΚΑΙ ΠΑΡΑΔΟΣΗ ΤΩΝ ΣΑΡΑΚΑΤΣΑΙΩΝ
-  4: 398 ΚΑΜ
+  4: 398ΚΑΜ
   5: '304'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1990'
   11: 350Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΙΩΑΝΝΙΝΑ
   13: ΗΠΕΙΡΟΣ-ΙΩΑΝΝΙΝΑ
@@ -8329,44 +8324,44 @@
   11: 295Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΡΥΓΙΑΝΝΗΣ
   13: ΜΑΚΡΥΓΙΑΝΝΗΣ-ΧΕΙΡΟΓΡΑΦΑ
   14: ΕΠΙΣΤΟΛΕΣ-ΜΑΚΡΥΓΙΑΝΝΗΣ
 - 0: 632
   1: ΜΑΛΑΜΑΣ,ΛΑΜΠΡΟΣ
   2: ΤΟΥΡΙΣΤΙΚΗ ΗΠΕΙΡΟΣ
-  4: 914.95 ΜΑΛ
+  4: 914.95ΜΑΛ
   5: 273-274-275
   8: Χ.Ε
   9: ΓΙΑΝΝΙΝΑ
   10: Χ.Ε
   11: '1971'
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΗΠΕΙΡΟΣ
   13: ΤΑΞΙΔΙΑ-ΗΠΕΙΡΟΣ
   14: ΗΠΕΙΡΟΣ-ΤΑΞΙΔΙΑ
   15: ΤΟΥΡΙΣΜΟΣ-ΗΠΕΙΡΟΣ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 633
   1: ΜΑΛΑΜΑΣ,ΛΑΜΠΡΟΣ
   2: ΤΟ ΚΟΜΠΟΛΟΙ ΤΟΥ ΑΛΗ
   3: ΘΕΑΤΡΙΚΟ ΙΣΤΟΡΙΚΟ ΔΡΑΜΑ
-  4: 883.2 ΜΑΛ
+  4: 883.2ΜΑΛ
   5: 1523-5370
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1972'
   11: 90Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
   17: 4 ΑΝΤΙΤΥΠΑ
 - 0: 634
   1: ΜΑΛΑΜΑΣ,ΛΑΜΠΡΟΣ
   2: ΕΛΛΑΔΑ
   3: ΠΕΡΙΗΓΗΣΗ (1967-1974)
-  4: 914.95 ΜΑΛ
+  4: 914.95ΜΑΛ
   5: 360-361
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1974'
   11: 512Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
   13: ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
@@ -8413,15 +8408,15 @@
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΚΑΒΑΦΗΣ
   15: ΚΑΒΑΦΗΣ
 - 0: 638
   1: ΜΑΛΑΝΟΣ,ΤΙΜΟΣ
   2: ΔΕΙΓΜΑΤΟΛΟΓΙΟ
   3: ΚΡΙΤΙΚΑ ΔΙΑΦΟΡΑ
-  4: 880.3 ΜΑΛ
+  4: 880.3ΜΑΛ
   5: '2660'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 237Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΚΡΙΤΙΚΗ
@@ -8441,83 +8436,83 @@
   13: ΑΛΒΑΝΙΑ-ΑΝΑΞΑΡΤΗΣΙΑ
   14: ΑΝΕΞΑΡΤΗΣΙΑ ΤΗΣ ΕΛΛΑΔΑΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;5
 - 0: 640
   1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞΑΝΔΡΟΣ
   2: ΓΕΩΡΓΙΟΣ ΚΑΣΤΡΙΩΤΗΣ
   3: ΣΚΕΝΤΕΡΜΠΕΗΣ
-  4: 938.4 ΜΑΜ
+  4: 938.4ΜΑΜ
   5: 2026-2027-9247
   8: X.E
   9: ΑΘΗΝΑ
   10: '1968'
   11: 34Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΟΠΛΑΡΧΗΓΟΣ
   13: ΟΠΛΑΡΧΗΓΟΣ-ΚΑΣΤΡΙΩΤΗΣ
   14: ΚΑΣΤΡΙΩΤΗΣ-ΣΚΕΝΤΕΡΜΠΕΗΣ
   15: ΣΚΕΝΤΕΡΜΠΕΗΣ-ΚΑΣΤΡΙΩΤΗΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;20
 - 0: 641
   1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞ Χ.
   2: ΣΧΟΛΕΙΑ ΚΑΙ ΔΙΔΑΣΚΑΛΟΙ ΤΟΥ ΑΛΥΤΡΩΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  4: 938.5 ΜΑΜ
+  4: 938.5ΜΑΜ
   5: 2040-2041-9271
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 38Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΙΔΕΙΑ
   13: ΠΑΙΔΕΙΑ-ΔΙΔΑΣΚΑΛΟΙ
   14: ΔΑΣΚΑΛΟΙ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;18
 - 0: 642
   1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞ Χ.
   2: Ο ΑΠΟΣΤΟΛΟΣ ΑΡΣΑΚΗΣ ΚΑΙ Η ΦΙΛΕΚΠΑΙΔΕΥΤΙΚΗ ΕΤΑΙΡΕΙΑ
-  4: 938 ΜΑΜ
+  4: 938ΜΑΜ
   5: 2044-2045-9262
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 53Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΣΑΚΗΣ
   13: ΑΡΣΑΚΗΣ-ΦΙΛΕΚΠΑΙΔΕΥΤΙΚΗ ΕΤΑΙΡΕΙΑ
   14: ΦΙΛΕΚΠΑΙΔΕΥΤΙΚΗ ΕΤΑΙΡΕΙΑ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;31
 - 0: 643
   1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞΑΝΔΡΟΣ Χ.
   2: ΗΠΕΙΡΟΣ ΚΑΙ ΛΑΚΩΝΙΑ ΑΠΟ ΤΗΝ ΣΠΛΑΝΤΖΑ
   3: ΕΩΣ ΤΟΝ ΑΥΤΟΝΟΜΙΑΚΟΝ ΑΓΩΝΑ 1914
-  4: 938.68 ΜΑΜ
+  4: 938.68ΜΑΜ
   5: 2042-2043-9250Α
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1968'
   11: 38Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΛΑΚΩΝΙΑ
   14: ΛΑΚΩΝΙΑ-ΗΠΕΙΡΟΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;21
 - 0: 644
   1: ΜΑΝΘΟΣ,ΑΛΚΗΣ
   2: ΘΩΜΑΣ ΠΑΣΧΙΔΗΣ
   3: ΗΠΕΙΡΩΤΑΙ ΔΗΜΟΣΙΟΓΡΑΦΟΙ ΣΤΗ ΡΟΥΜΑΝΙΑ
-  4: 938 ΜΑΝ
+  4: 938ΜΑΝ
   5: 2032-2033-9261
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 56Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΔΗΜΟΣΙΟΓΡΑΦΟΙ
   13: ΗΠΕΙΡΟΣ-ΔΗΜΟΣΙΟΓΡΑΦΟΙ
   14: ΠΑΣΧΙΔΗΣ-ΔΗΜΟΣΙΟΓΡΑΦΟΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;31
 - 0: 645
   1: ΜΑΝΘΟΣ,ΑΛΚΗΣ
   2: ΗΠΕΙΡΩΤΑΙ ΕΙΣ ΤΗΝ ΡΟΥΜΑΝΙΑΝ
-  4: 938 ΜΑΝ
+  4: 938ΜΑΝ
   5: 2034-2035-9249
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 51Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΕΣ
@@ -8546,15 +8541,15 @@
   10: Χ.Χ
   11: 78Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ
   13: ΚΑΡΑΙΣΚΑΚΗΣ-ΙΣΤΟΡΙΑ
 - 0: 648
   1: ΜΑΝΟΣ,ΜΙΧΑΗΛ ΧΑΡ
   2: ΗΠΕΙΡΩΤΙΚΗ ΑΝΘΟΛΟΓΙΑ
-  4: 938.93 ΜΑΝ
+  4: 938.93ΜΑΝ
   5: '2154'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1955'
   11: 224Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΝΘΟΛΟΓΙΑ
@@ -8573,55 +8568,55 @@
   13: ΠΑΙΔΟΜΑΖΩΜΑ
   14: ΠΑΙΔΙ-ΠΑΙΔΟΜΑΖΩΜΑ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 650
   1: ΜΑΝΟΥΣΑΚΑΣ,Μ.Ι
   2: Η ΕΝ ΚΡΗΤΗ ΣΥΝΩΜΟΣΙΑ ΤΟΥ ΣΗΦΗ ΒΛΑΣΤΟΥ (1453-1454)
   3: ΚΑΙ Η ΝΕΑ ΣΥΝΩΜΟΤΙΚΗ ΚΙΝΗΣΙΣ ΤΟΥ (1460-1462)
-  4: 938.42 ΜΑΝ
+  4: 938.42ΜΑΝ
   5: '1906'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1960'
   11: 168Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ-ΚΡΗΤΗ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΚΡΗΤΗ
   14: ΚΡΗΤΗ-ΣΥΝΩΜΟΣΙΕΣ
   15: ΣΥΝΩΜΟΣΙΕΣ-ΚΡΗΤΗ
 - 0: 651
   1: ΜΑΡΑΖΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   2: Ο ΗΠΕΙΡΩΤΗΣ ΕΘΝΑΠΟΣΤΟΛΟΣ ΠΕΤΡΟΣ ΗΠΙΤΗΣ
-  4: 938.5 ΜΑΡ
+  4: 938.5ΜΑΡ
   5: 2061-2760-9258
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1973'
   11: 50Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΕΘΝΑΠΟΣΤΟΛΟΣ
   13: ΗΠΕΙΡΟΣ-ΗΠΙΤΗΣ
   14: ΗΠΙΤΗΣ-ΕΘΝΑΠΟΣΤΟΛΟΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;38
 - 0: 652
   1: ΜΑΡΙΔΑΚΗΣ,ΓΕΩΡΓΙΟΣ
   2: Η ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΙΣ ΩΣ ΕΚΦΡΑΣΙΣ ΤΟΥ ΕΥΡΩΠΑΙΚΟΥ ΠΝΕΥΜΑΤΟΣ
-  4: 938.5 ΜΑΡ
+  4: 938.5ΜΑΡ
   5: '2126'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1951'
   11: 21Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ
   13: ΕΠΑΝΑΣΤΑΣΗ-ΕΛΛΗΝΙΚΗ
   14: ΕΥΡΩΠΑΙΚΟ ΠΝΕΥΜΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   15: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
 - 0: 653
   1: ΜΑΡΚΑΝΤΩΝΑΤΟΣ,ΔΙΟΝΥΣΙΟΣ
   2: ΑΛΕΞΑΝΔΡΟΣ
   3: ΤΡΑΓΩΔΙΑ
-  4: 886.2 ΜΑΡ
+  4: 886.2ΜΑΡ
   5: '1526'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 73Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
@@ -8639,15 +8634,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΠΕΤΑ
   14: ΠΕΤΑ-ΦΙΛΕΛΛΗΝΕΣ
   15: ΦΙΛΛΕΛΗΝΕΣ-ΠΕΤΑ
 - 0: 655
   1: ΜΑΡΚΟΓΙΑΝΝΗΣ,ΧΡΗΣΤΟΣ
   2: ΕΘΝΙΚΑΙ ΑΝΑΞΙΟΤΗΤΕΣ
-  4: 938.8 ΜΑΡ
+  4: 938.8ΜΑΡ
   5: '2230'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1981'
   11: 55Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΘΝΙΚΑ
   13: ΕΘΝΙΚΕΣ ΑΝΑΞΙΟΤΗΤΕΣ
@@ -8677,39 +8672,39 @@
   12: ΕΛΛΗΝΙΚΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΦΙΛΜΣ
   13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΦΙΛΜΣ
   14: ΦΙΛΜΣ-ΤΕΧΝΙΚΗ
   15: ΤΕΧΝΙΚΗ ΤΩΝ ΦΙΛΜΣ
 - 0: 658
   1: ΜΑΤΕΣΙ,ΑΝΤΩΝΙΟΣ
   2: Ο ΒΑΣΙΛΙΚΟΣ
-  4: 886.2 ΜΑΤ
+  4: 886.2ΜΑΤ
   5: '1477'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1964'
   11: 182Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
   14: ΔΡΑΜΑ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΔΡΑΜΑ
 - 0: 659
   1: ΜΑΥΡΟΕΙΔΗΣ,ΦΑΝΗΣ
   2: ΣΥΜΒΟΛΗ ΣΤΗΝ ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΑΔΕΛΦΟΤΗΤΑΣ ΒΕΝΕΤΙΑΣ
   3: ΣΤΟ ΙΣΤ' ΑΙΩΝΑ
-  4: 938.4 ΜΑΥ
+  4: 938.4ΜΑΥ
   5: '2077'
   8: ΚΑΡΑΒΙΑ
   9: ΑΘΗΝΑ
   11: 372Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΔΕΛΦΟΤΗΤΑ ΒΕΝΕΤΙΑΣ
   13: ΑΔΕΛΦΟΤΗΤΑ ΒΕΝΕΤΙΑΣ
 - 0: 660
   1: ΜΑΥΡΟΧΑΛΥΒΙΔΗΣ,ΓΕΩΡΓΙΟΣ
   2: Η ΑΞΟ ΚΑΠΑΔΟΚΙΑΣ
-  4: 938.99 ΜΑΥ
+  4: 938.99ΜΑΥ
   5: 2442-2443-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1990'
   11: 338Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΠΑΔΟΚΙΑ-ΑΞΟ
   13: ΚΑΠΠΑΔΟΚΙΑ-ΑΞΟ
@@ -8737,28 +8732,28 @@
   11: 239Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΜΑΤΑ
   13: ΘΕΜΑΤΑ-ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΙΔΙΚΑ ΘΕΜΑΤΑ
 - 0: 663
   1: ΜΑΤΕΣΙΣ,ΠΑΥΛΟΣ
   2: ΒΙΟΧΗΜΕΙΑ ΚΑΙ Ο ΣΤΑΘΜΟΣ
-  4: 880.2 ΜΑΤ
+  4: 880.2ΜΑΤ
   5: '1361'
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 103Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
   14: ΘΕΑΤΡΙΚΑ ΕΡΓΑ
 - 0: 664
   1: ΜΑΤΣΑΣ,ΑΛΕΞΑΝΔΡΟΣ
   2: ΚΡΟΙΣΟΣ
   3: ΕΜΜΕΤΡΟΝ ΔΡΑΜΑ ΕΙΣ ΠΡΑΞΕΙΣ ΤΡΕΙΣ
-  4: 881.2 ΜΑΤ
+  4: 881.2ΜΑΤ
   5: '1495'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1959'
   11: 84Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -8798,15 +8793,15 @@
   11: 204S
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΡΤΑ
   14: ΑΡΤΑ
 - 0: 668
   1: ΜΕΛΑΣ,ΛΕΟΝΤΟΣ
   2: ΣΕΛΙΔΕΣ ΤΗΣ ΗΠΕΙΡΟΥ
-  4: 938.21 ΜΕΛ
+  4: 938.21ΜΕΛ
   5: '2179'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1963'
   11: 243Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ
@@ -8821,28 +8816,28 @@
   11: 382Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ 1909
   13: ΕΠΑΝΑΣΤΑΣΗ 1909
   14: 1909-ΕΠΑΝΑΣΤΑΣΗ
 - 0: 670
   1: ΜΕΛΑΣ,ΣΠΥΡΟΣ
   2: ΟΙ ΠΟΛΕΜΟΙ 1912-1913
-  4: 938.68 ΜΕΛ
+  4: 938.68ΜΕΛ
   5: '1988'
   8: ΜΠΙΡΗΣ
   9: ΑΘΗΝΑ
   10: '1958'
   11: 546Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΙ-(1912-1913)
   13: ΠΟΛΕΜΟΙ-(1912-1913)
   14: 1912-ΠΟΛΕΜΟΣ
   15: 1913-ΠΟΛΕΜΟΣ
 - 0: 671
   1: ΜΕΛΑΣ,ΣΠΥΡΟΣ
   2: ΝΕΟΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-  4: 880.09 ΜΕΛ
+  4: 880.09ΜΕΛ
   5: '186'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 507Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΝΕΩΤΕΡΗ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΝΕΩΤΕΡΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -8920,28 +8915,28 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΔΙΧΑΣΜΟΣ
   14: ΔΙΧΑΣΜΟΣ-ΠΟΙΗΣΗ
   15: ΜΕΤΑΙΧΜΙΟ-ΠΟΙΗΣΗ
 - 0: 678
   1: ΜΕΡΑΝΑΙΟΣ,Κ.Λ
   2: ΜΕΛΕΤΗΜΑΤΑ
-  4: 880.4 ΜΕΡ
+  4: 880.4ΜΕΡ
   5: '492'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1957'
   11: 127Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΜΕΛΕΤΗΜΑΤΑ
   14: ΜΕΛΕΤΗΜΑΤΑ-ΣΥΓΓΡΑΦΕΙΣ
 - 0: 679
   1: ΜΕΡΕΝΤΙΤΟΣ,ΙΩΑΝΝΗΣ ΚΩΝΣΤ
   2: ΣΥΓΚΡΙΣΙΣ ΤΟΥ "ΒΙΟΥ ΚΑΙΣΑΡΟΣ" ΠΑΡΑ ΣΟΥΗΤΩΝΙΩ ΠΡΟΣ ΤΟΝ
   3: '''ΒΙΟΝ ΚΑΙΣΑΡΟΣ"ΠΑΡΑ ΠΛΟΥΤΑΡΧΩ'
-  4: 920 ΜΕΡ
+  4: 920ΜΕΡ
   5: '2413'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1982'
   12: ΕΛΛΗΝΙΚΗ ΒΙΟΓΡΑΦΙΑ-ΠΛΟΥΤΑΡΧΟΣ
   13: ΠΛΟΥΤΑΡΧΟΣ-ΒΙΟΓΡΑΦΙΑ
   14: ΒΙΟΓΡΑΦΙΑ-ΠΛΟΥΤΑΡΧΟΣ
@@ -8959,15 +8954,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ-ΚΑΤΩ ΙΤΑΛΙΑ
   13: ΕΛΛΗΝΙΣΜΟΣ-ΚΑΤΩ ΙΤΑΛΙΑ
   14: ΚΑΤΩ ΙΤΑΛΙΑ-ΕΛΛΗΝΙΣΜΟΣ
   15: ΙΤΑΛΙΑ-ΕΛΛΗΝΙΣΜΟΣ
 - 0: 681
   1: ΜΕΡΚΟΥΡΗΣ,ΣΤΑΜΑΤΗΣ Σ
   2: ΓΕΩΡΓΙΟΣ ΚΟΝΔΥΛΗΣ (1879-1936)
-  4: 938.6 ΜΕΡ
+  4: 938.6ΜΕΡ
   5: '1917'
   8: ΜΑΥΡΙΔΗΣ
   9: Χ.Τ
   10: '1954'
   11: 258Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΠΡΟΣΩΠΑ-ΚΟΝΔΥΛΗΣ
@@ -8984,42 +8979,42 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
   13: ΜΙΚΡΑ ΑΣΙΑ-ΙΣΤΟΡΙΚΑ
   14: ΙΣΤΟΡΙΚΑ-ΜΙΚΡΑ ΑΣΙΑ
 - 0: 683
   1: ΜΗΤΣΑΚΗΣ,Κ
   2: ΝΕΟΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
   3: Η ΓΕΝΙΑ ΤΟΥ '30
-  4: 880.3 ΜΗΤ
+  4: 880.3ΜΗΤ
   5: 212-213
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 161Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-Η ΓΕΝΙΑ ΤΟΥ '30
   14: ΠΕΖΟΓΡΑΦΙΑ-1930
   15: ΣΥΓΓΡΑΦΕΙΣ-ΠΕΖΟΓΡΑΦΟΙ
 - 0: 684
   1: ΜΗΤΣΟΠΟΥΛΟΣ,ΦΑΝΗΣ Γ
   2: Ο ΡΟΒΑΣ
   3: ΤΡΑΓΩΔΙΑ
-  4: 881.2 ΜΗΤ
+  4: 881.2ΜΗΤ
   5: '2677'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 142Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
   15: ΤΡΑΓΩΔΙΑ-ΕΡΓΟ
 - 0: 685
   1: ΜΗΤΣΟΤΑΚΗΣ,ΚΥΡΙΑΚΟΣ
   2: ΠΡΟΣΩΠΑ ΚΑΙ ΤΟΠΟΙ
-  4: 889.21 ΜΗΤ
+  4: 889.21ΜΗΤ
   5: '2533'
   8: ΑΙΓΑΓΡΟΣ
   9: ΑΘΗΝΑ
   10: '1966'
   11: 116Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΠΡΟΣΩΠΑ-ΕΛΛΑΔΑ
@@ -9048,15 +9043,15 @@
   11: 288Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΜΕΡΙΚΑΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
   14: ΘΕΑΤΡΙΚΑ ΕΡΓΑ-ΑΜΕΡΙΚΗ
 - 0: 688
   1: ΜΙΛΛΕΡ,ΟΥΙΛΛΙΑΜ
   2: Η ΤΟΥΡΚΙΑ ΚΑΤΑΡΡΕΟΥΣΑ ΙΣΤΟΡΙΑ ΤΗΣ ΟΘΩΜΑΝΙΚΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
-  4: 956.1 ΜΙΛ
+  4: 956.1ΜΙΛ
   5: '2301'
   6: ΛΑΜΠΡΟΥ,ΣΠΥΡ.
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1914'
   11: 704Σ
   12: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-(1801-1913)
@@ -9074,53 +9069,53 @@
   11: 172Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ
   14: ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ
 - 0: 690
   1: ΜΙΣΑΗΛΙΔΗΣ,ΧΑΡΙΤΩΝΟΣ
   2: ΤΟ ΘΕΑΤΡΟ ΤΗΣ ΠΟΛΗΣ (1800-1900)
-  4: 886.2 ΜΙΣ
+  4: 886.2ΜΙΣ
   5: '1421'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1960'
   11: 12Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΟΛΗ(1800-1900)
   14: ΤΟ ΘΕΑΤΡΟ ΣΤΗΝ ΠΟΛΗ
 - 0: 691
   1: ΜΙΤΑΚΗΣ,ΔΙΟΝΥΣΗΣ
   2: ΓΙΑΝΝΑΚΗΣ ΣΟΥΛΤΑΝΗΣ
-  4: 938.4 ΜΙΤ
+  4: 938.4ΜΙΤ
   5: '2605'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1971'
   11: 21Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΠΡΟΣΩΠΑ-ΣΟΥΛΤΑΝΗΣ
   14: ΣΟΥΛΤΑΝΗΣ-ΠΡΟΣΩΠΑ
 - 0: 692
   1: ΜΙΤΣΟΥ,ΜΑΡΚΕΛΟΥ Θ
   2: Η ΕΚΣΤΡΑΤΕΙΑ ΤΟΥ ΚΛΕΥΜΕΝΟΥΣ ΚΑΤΑ ΤΟΥ ΑΡΓΟΥΣ
-  4: 938.15 ΜΙΤ
+  4: 938.15ΜΙΤ
   5: '2320'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1979'
   11: 6Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΚΣΤΡΑΤΕΙΑ-ΚΛΕΟΜΕΝΟΥΣ
   13: ΕΚΣΤΡΑΤΕΙΑ-ΚΛΕΟΜΕΝΟΥΣ
   14: ΑΡΓΟΣ-ΕΚΣΤΡΑΤΕΙΑ
   15: ΚΛΕΟΜΕΝΟΣ-ΕΚΣΤΡΑΤΕΙΑ
 - 0: 693
   1: ΜΙΧΑΗΛΙΔΗΣ-ΚΡΙΝΑΙΟΣ,ΜΠΑΜΠΗΣ
   2: Η ΜΕΤΑΒΟΛΗ ΤΗΣ ΔΟΜΗΣ ΤΟΥ ΜΕΤΑΠΟΛΕΜΙΚΟΥ ΜΥΘΙΣΤΟΡΗΜΑΤΟΣ ΚΑΙ
   3: Η ΝΕΟΕΛΛΗΝΙΚΗ ΚΟΙΝΩΝΙΑ
-  4: 880.3 ΜΙΧ
+  4: 880.3ΜΙΧ
   5: '219'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΜΕΤΑΒΟΛΗ
   14: ΜΥΘΙΣΤΟΡΗΜΑ-ΔΟΜΗ
@@ -9136,75 +9131,75 @@
   11: 29Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
   13: ΚΑΠΟΔΙΣΤΡΙΑΣ-ΔΙΑΛΕΞΕΙΣ
   14: ΔΙΑΛΕΞΕΙΣ-ΚΑΠΟΔΙΣΤΡΙΑΣ
 - 0: 695
   1: ΜΟΛΙΕΡΟΥ
   2: ΝΤΟΝ ΖΟΥΑΝ
-  4: 842 ΜΟΛ
+  4: 842ΜΟΛ
   5: '1439'
   6: ΠΡΕΒΕΛΑΚΗΣ,ΠΑΝΤΕΛΗΣ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1973'
   12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΑΛΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΓΑΛΛΙΑ
 - 0: 696
   1: ΜΟΛΟΣΣΟΣ,ΖΩΤΟΣ
   2: ΗΠΕΙΡΩΤΙΚΑΙ ΜΕΛΕΤΑΙ
-  4: 938.21 ΜΟΛ
+  4: 938.21ΜΟΛ
   5: '2178'
   8: ΑΝΤΩΝΙΑΔΗ
   9: ΑΘΗΝΑ
   10: '1875'
   11: 144Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΜΕΛΕΤΕΣ
   14: ΜΕΛΕΤΕΣ-ΗΠΕΙΡΟΣ
 - 0: 697
   1: ΜΟΣΤΡΑΤΟΥ,ΣΜΑΡΑΓΔΑ
   2: ΚΑΡΓΚΕΖΕ
   3: ΤΟ ΕΛΛΗΝΙΚΟ ΧΩΡΙΟ
-  4: 914 ΜΟΣ
+  4: 914ΜΟΣ
   5: '425'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 105Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΑΡΓΚΕΖΕ
   13: ΤΑΞΙΔΙΑ-ΚΑΡΓΚΕΖΕ
   14: ΚΑΡΓΚΕΖΕ-ΤΑΞΙΔΙΑ
 - 0: 698
   1: ΜΟΥΓΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
   2: Ο ΒΟΛΙΩΤΙΚΟΣ ΠΟΛΙΤΙΣΜΟΣ ΤΟΥ ΜΕΣΟΠΟΛΕΜΟΥ
-  4: 938.7 ΜΟΥ
+  4: 938.7ΜΟΥ
   5: '1653'
   8: ΠΥΛΗ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 110Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΛΟΣ
   13: ΒΟΛΟΣ-ΠΟΛΙΤΙΣΜΟΣ
   14: ΜΕΣΟΠΟΛΕΜΟΣ-ΒΟΛΟΣ
 - 0: 699
   1: ΜΟΥΓΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
   2: ΜΟΝΟΠΑΤΙΑ ΤΟΥ ΒΙΟΥ
-  4: 910 ΜΟΥ
+  4: 910ΜΟΥ
   5: '1669'
   8: ΠΥΛΗ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 126Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΩΤΙΚΑ
   13: ΤΑΞΙΩΤΙΚΑ-ΓΕΩΓΡΑΦΙΑ
 - 0: 700
   1: ΜΟΥΓΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
   2: ΠΤΥΧΕΣ ΤΟΥ ΒΟΛΙΩΤΙΚΟΥ ΠΟΛΙΤΙΣΜΟΥ
-  4: 938.7 ΜΟΥ
+  4: 938.7ΜΟΥ
   5: '1691'
   8: Χ.Ε
   9: ΒΟΛΟΣ
   10: '1992'
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΛΟΣ
   13: ΒΟΛΟΣ-ΠΟΛΙΤΙΣΜΟΣ (1940-1990)
@@ -9255,18 +9250,18 @@
   9: ΑΘΗΝΑ
   10: '1962'
   11: 180Σ
   12: ΚΙΝΕΖΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΚΙΝΕΖΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
   14: ΚΙΝΑ-ΘΕΑΤΡΟ
 - 0: 705
-  1: ΜΟΥΡΑΤ,ΤΖΟΝ
+  1: MURAT,JOHN
   2: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
   3: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  4: 938 MUR
+  4: 938.ΟΟ1MUR
   5: 2082-1950
   8: Χ.Ε
   9: Χ.Τ
   10: '1982'
   11: 542Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ-ΞΕΚΛΗΡΙΣΜΑ
@@ -9318,28 +9313,28 @@
   10: '1976'
   11: 131Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΠΟΤΣΑΡΗΣ
   13: ΜΠΟΤΣΑΡΗΣ
 - 0: 710
   1: ΜΟΥΣΕΛΙΜΗΣ,ΣΠΥΡΟΣ Γ.
   2: ΑΡΧΑΙΟΤΗΤΕΣ ΤΗΣ ΘΕΣΠΡΩΤΙΑΣ
-  4: 938.21 ΜΟΥ
+  4: 938.21ΜΟΥ
   5: '2349'
   8: Χ.Ε
   9: ΓΙΑΝΝΙΝΑ
   10: '1980'
   11: 319Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΠΡΩΤΙΑ
   13: ΘΕΣΠΡΩΤΙΑ-ΑΡΧΑΙΟΤΗΤΕΣ
   14: ΑΡΧΑΙΟΤΗΤΕΣ-ΘΕΣΠΡΩΤΙΑ
 - 0: 711
   1: ΜΟΥΣΤΑΚΗΣ,ΒΑΣ
   2: ΠΝΕΥΜΑ ΚΑΙ ΠΗΛΟΣ
   3: ΚΡΙΤΙΚΑ ΚΕΙΜΕΝΑ
-  4: 880.4 ΜΟΥ
+  4: 880.4ΜΟΥ
   5: '2705'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1980'
   11: 79Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΗΛΟΣ
   13: ΠΗΛΟΣ-ΛΟΓΟΤΕΧΝΙΑ
@@ -9366,15 +9361,15 @@
   10: '1977'
   11: 53Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ
   13: ΚΑΡΑΙΣΚΑΚΗΣ-ΚΑΤΑΓΩΓΗ
 - 0: 714
   1: ΜΠΑΚΟΓΙΑΝΝΗΣ,ΣΤΕΦΑΝΟΣ
   2: ΕΝΤΥΠΩΣΕΙΣ ΣΚΕΨΕΙΣ ΣΥΜΠΕΡΑΣΜΑΤΑ ΑΠΟ ΤΟ ΙΣΡΑΗΛ
-  4: 950 ΜΠΑ
+  4: 950ΜΠΑ
   5: 2526-2556
   8: Χ.Ε
   9: ΑΡΤΑ
   10: '1965'
   11: 51Σ
   12: ΙΣΡΑΗΛΙΝΗ ΙΣΤΟΡΙΑ
   13: ΙΣΡΑΗΛ-ΙΣΤΟΡΙΑ
@@ -9427,28 +9422,28 @@
   11: 277Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   14: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
 - 0: 719
   1: ΜΠΕΡΤΩ,ΣΙΜΟΝ
   2: ΕΝΤΙΘ ΠΙΑΦ
-  4: 840 ΜΠΕ
+  4: 840ΜΠΕ
   5: '2631'
   6: ΑΞΙΩΤΗ,ΜΕΛΠΩ
   8: ΡΑΠΠΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 504Σ
   12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΒΙΟΓΡΑΦΙΑ
   13: ΒΙΟΓΡΑΦΙΑ-ΓΑΛΛΙΚΗ
   14: ΕΝΤΙΘ ΠΙΑΦ-ΒΙΟΓΡΑΦΙΑ
 - 0: 720
   1: ΜΠΙΝΙΑΡΗΣ,ΓΚΙΚΑΣ
   2: ΕΚΑΤΟ ΧΡΟΝΙΑ ΘΕΑΤΡΙΚΗΣ ΠΕΙΡΑΙΚΗΣ ΖΩΗΣ
-  4: 886.2 ΜΠΙ
+  4: 886.2ΜΠΙ
   5: '2720'
   8: Χ.Ε
   9: ΠΕΙΡΑΙΑΣ
   10: '1976'
   11: 35Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΕΙΡΑΙΑΣ
@@ -9500,15 +9495,15 @@
   11: 95Σ
   12: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   14: ΑΡΧΕΙΟ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
 - 0: 725
   1: ΜΠΟΥΡΑΝΤΑΣ,ΛΑΜΠΡΟΣ Κ
   2: Ο ΑΜΒΡΑΚΙΚΟΣ ΚΟΛΠΟΣ ΚΑΙ ΑΙ ΓΥΡΩΘΕΝ ΑΥΤΟΥ ΛΙΜΝΟΘΑΛΑΣΣΑ
-  4: 938 ΜΠΟ
+  4: 938ΜΠΟ
   5: 2487-2524
   8: Χ.Ε
   9: ΑΡΤΑ
   10: '1982'
   11: 24Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΑΜΒΡΑΚΙΚΟΣ ΚΟΛΠΟΣ
@@ -9527,96 +9522,96 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΧΙΤΛΕΡ
   13: ΧΙΤΛΕΡ-ΓΕΡΜΑΝΙΑ
   14: ΓΕΡΜΑΝΙΑ-ΧΙΤΛΕΡ
 - 0: 727
   1: ΜΠΡΕΔΗΜΑΣ,ΠΙΝΔΑΡΟΣ
   2: ΜΑΡΤΙΝΟΣ ΛΟΥΘΗΡΟΣ
   3: ΙΣΤΟΡΙΚΟ ΔΡΑΜΑ
-  4: 886.2 ΜΠΡ
+  4: 886.2ΜΠΡ
   5: '1501'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1958'
   11: 95Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
   14: ΔΡΑΜΑ-ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
 - 0: 728
   1: ΜΠΡΕΔΗΜΑΣ,ΠΙΝΔΑΡΟΣ
   2: ΠΕΛΟΠΟΝΝΗΣΙΑΚΟΣ ΠΟΛΕΜΟΣ
   3: ΙΣΤΟΡΙΚΟ ΔΡΑΜΑ
-  4: 881.2 ΜΠΡ
+  4: 881.2ΜΠΡ
   5: '1502'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1959'
   11: 83Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΗ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ-ΔΡΑΜΑ
   14: ΔΡΑΜΑ-ΘΕΑΤΡΙΚΟ ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΔΡΑΜΑ
 - 0: 729
   1: ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
   2: Η ΜΑΝΑ ΚΟΥΡΑΓΙΟ ΚΑΙ ΤΑ ΠΑΙΔΙΑ ΤΗΣ
-  4: 832 ΜΠΡ
+  4: 832ΜΠΡ
   5: '1558'
   6: ΑΡΖΟΓΛΟΥ,ΙΟΡΔΑΝΗΣ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Ε
   11: 162Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΓΕΡΜΑΝΙΑ
 - 0: 730
   1: ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
   2: ΤΡΟΜΟΣ ΚΑΙ ΑΘΛΙΟΤΗΤΑ ΤΟΥ ΤΡΙΤΟΥ ΡΑΙΧ
-  4: 832 ΜΠΡ
+  4: 832ΜΠΡ
   5: '1575'
   6: ΒΕΡΥΚΟΚΑΚΗ,ΑΓΓΕΛΑ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 145Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΓΕΡΜΑΝΙΑ
 - 0: 731
   1: ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΝΤ
   2: Ο ΚΑΛΟΣ ΑΝΘΡΩΠΟΣ ΤΟΥ ΣΕΤΣΟΥΑΝ
-  4: 832 ΜΠΡ
+  4: 832ΜΠΡ
   5: '1572'
   6: ΠΛΩΡΙΤΗΣ,ΜΑΡΙΟΣ
   8: ΙΘΑΚΗ
   9: ΑΘΗΝΑ
   10: '1980'
   11: 135Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΓΕΡΜΑΝΙΑ
 - 0: 732
   1: ΜΠΡΕΧΤ,ΜΠΕΡΤΟΛΤ
   2: Ο ΚΑΥΚΑΣΙΑΝΟΣ ΚΥΚΛΟΣ ΜΕ ΤΗ ΚΙΜΩΛΙΑ
-  4: 832 ΜΠΡ
+  4: 832ΜΠΡ
   5: '1573'
   6: ΒΑΜΒΑΛΗΣ,ΓΙΩΡΓΟΣ
   7: 4ΕΚΔ
   8: ΜΟΥΚΟΥΜΑΝΗ
   9: ΑΘΗΝΑ
   10: '1970'
   11: 164Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΓΕΡΜΑΝΙΑ
 - 0: 733
   1: ΜΥΛΩΝΑΣ,ΠΟΛΥΣ
   2: ΠΟΛΩΝΙΑ,ΣΥΡΙΑ
   3: ΤΑΞΙΔΕΥΟΝΤΑΣ
-  4: 914.49 ΜΥΛ
+  4: 914.49ΜΥΛ
   5: '426'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1982'
   11: 131Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΠΟΛΩΝΙΑ
   13: ΤΑΞΙΔΙΑ-ΠΟΛΩΝΙΑ
@@ -9752,27 +9747,27 @@
   10: '1956'
   11: 356Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
 - 0: 745
   1: ΜΥΡΤΙΩΤΙΣΣΑ
   2: ΤΡΑΓΟΥΔΙΑ
-  4: 782.42 ΜΥΡ
+  4: 782.42ΜΥΡ
   5: '2626'
   8: ΤΥΠΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 31Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
   14: ΤΡΑΓΟΥΔΙΑ
 - 0: 746
   1: ΜΩΥΣΕΙΔΗΣ,ΣΤΥΛ Μ
   2: '"ΑΥΤΟΚΡΑΤΩΡ ΘΕΣΣΑΛΟΝΙΚΗΣ"'
-  4: 886.2 ΜΩΥ
+  4: 886.2ΜΩΥ
   5: 1687-1486
   8: ΒΑΚΩΝ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 90Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΔΡΑΜΑ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -9815,15 +9810,15 @@
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΑΛΗ ΠΑΣΑΣ
   14: ΑΛΗ ΠΑΣΑΣ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;51
 - 0: 750
   1: ΙΩΑΝΝΙΔΗΣ,ΛΑΚΗ Α
   2: ΕΥΡΩΠΗ
   3: ΣΚΕΨΕΙΣ ΔΙΑ ΤΗΝ ΙΔΕΑΝ ΤΗΣ ΕΝΩΣΕΩΣ ΤΗΣ
-  4: 914 ΙΩΑ
+  4: 914ΙΩΑ
   5: '2775'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1968'
   11: 173Σ
   12: ΠΑΓΚΟΣΜΙΑ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
   13: ΕΥΡΩΠΗ-ΙΣΤΟΡΙΑ
@@ -9863,30 +9858,30 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΠΡΩΤΙΑ
   13: ΘΕΣΠΡΩΤΙΑ-ΙΣΤΟΡΙΑ
   17: 3 ΑΝΤΙΤΥΠΑ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;47
 - 0: 754
   1: ΚΙΤΣΟΥ-ΠΙΤΟΥΛΗ,ΧΡΙΣΤΙΝΑ
   2: ΗΠΕΙΡΩΤΕΣ ΕΚΔΟΤΕΣ ΚΑΙ ΤΥΠΟΓΡΑΦΟΙ ΤΗΣ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
-  4: 938.4 ΚΙΤ
+  4: 938.4ΚΙΤ
   5: 2725-2726
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1980'
   11: 286Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΗΠΕΙΡΟΣ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   14: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΤΥΠΟΓΡΑΦΟΙ
   15: ΤΥΠΟΓΡΑΦΟΙ-ΗΠΕΙΡΟΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;52
 - 0: 755
   1: ΚΑΛΥΔΟΠΟΥΛΟΣ,Γ.Δ
   2: ΤΟ ΕΛΛΗΝΙΚΟ ΧΩΡΙΟ
   3: ΑΝΑΓΚΗ ΔΙΑΣΩΣΕΩΣ ΤΟΥ ΔΙΑΜΑΝΤΕΝΙΟΥ ΑΥΤΟΥ ΘΕΜΕΛΙΟΥ ΤΟΥ ΕΛΛΗΝΙΚ
-  4: 938 ΚΑΛ
+  4: 938ΚΑΛ
   5: '2774'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1961'
   11: 278Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΧΩΡΙΟ
   13: ΧΩΡΙΟ-ΕΛΛΑΔΑ
@@ -9903,15 +9898,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΔΙΤΣΑ-ΜΟΡΦΕΣ
   13: ΚΑΡΔΙΤΣΑ-ΜΟΡΦΕΣ
   14: ΣΕΡΑΦΕΙΜ
   15: ΚΑΡΑΙΣΚΑΚΗΣ-ΠΛΑΣΤΗΡΑΣ
 - 0: 757
   1: ΛΥΚΙΣΣΑΣ,ΜΙΧΑΛΗΣ Γ
   2: Η ΙΣΤΟΡΙΑ ΤΗΣ ΙΟΝΙΟΥ ΑΚΑΔΗΜΙΑΣ
-  4: 938 ΛΥΚ
+  4: 938ΛΥΚ
   5: '2805'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1993'
   11: 84Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΟΝΙΟΣ ΑΚΑΔΗΜΙΑ
   13: ΙΟΝΙΟΣ ΑΚΑΔΗΜΙΑ-ΙΣΤΟΡΙΑ
@@ -9941,15 +9936,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΙΚΗ ΑΠΕΙΛΗ
   13: ΤΟΥΡΚΙΚΗ ΑΠΕΙΛΗ
   14: ΚΑΡΑΜΑΝΛΗΣ-ΤΟΥΡΚΙΚΗ ΑΠΕΙΛΗ
 - 0: 760
   1: ΜΑΥΡΟΥΛΙΔΟΥ,ΛΟΥΛΑ
   2: ΤΟ ΚΟΥΡΣΕΜΑ ΤΗΣ ΠΟΛΗΣ ΑΠ'ΤΟΥΣ ΦΡΑΓΚΟΥΣ ΚΑΙ ΣΤΕΡΓΙΩΜΑ ΤΟΥΣ
   3: ΣΤΟΝ ΕΛΛΗΝΙΚΟ ΝΟΤΙΑ
-  4: 889.21 ΜΑΥ
+  4: 889.21ΜΑΥ
   5: '2549'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1957'
   11: 305Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
   13: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΦΡΑΓΚΟΙ
@@ -9979,15 +9974,15 @@
   11: 286Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΙΣΤΟΡΙΕΣ
 - 0: 763
   1: ΝΑΚΟΣ,ΓΡΗΓΟΡΙΟΣ ΧΡ
   2: Η ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΤΗΣ
   3: ΑΠΟ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΤΩΝ ΚΑΘ'ΗΜΑΣ
-  4: 938.21 ΝΑΚ
+  4: 938.21ΝΑΚ
   5: '2518'
   8: Χ.Ε
   9: ΑΡΤΑ
   10: '1969'
   11: 144Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΡΤΑ
@@ -10005,15 +10000,15 @@
   13: ΕΛΛΗΝΙΣΜΟΣ-ΣΥΝΘΗΚΗ ΤΟΥ ΑΓΙΟΥ ΣΤΕΦΑΝΟΥ
   14: ΣΥΝΘΗΚΗ ΑΓΙΟΥ ΣΤΕΦΑΝΟΥ
 - 0: 765
   1: ΝΑΛΤΣΑΣ,ΧΡΙΣΤΟΦΟΡΟΣ Α.
   2: ΦΙΛΙΠΠΟΣ Β' Ο ΜΑΚΕΔΩΝ
   3: Ο ΕΝΩΤΗΣ ΤΩΝ ΕΛΛΗΝΩΝ
   4: 938.171ΝΑΛ
-  5: '1951'
+  5: 1951-15688
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1970'
   11: 885Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ-ΦΙΛΙΠΠΟΣ Β'
   13: ΜΑΚΕΔΟΝΙΑ-ΦΙΛΙΠΠΟΣ Β'
   14: ΦΙΛΙΠΠΟΣ Β'
@@ -10043,15 +10038,15 @@
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΑΙΔΙΚΟ
   14: ΠΑΙΔΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΠΑΙΔΙΚΟ
 - 0: 768
   1: ΝΕΖΕΡΙΤΟΣ,ΑΓΓΕΛΟΣ
   2: '"ΕΝΟΤΗΣ ΠΑΝΤΩΝ ΤΩΝ ΕΛΛΗΝΩΝ ΜΟΝΗ ΣΩΤΗΡΙΑ ΤΗΣ ΠΑΤΡΙΔΑΣ"'
   3: Ο ΣΛΑΒΙΚΟΣ ΚΙΝΔΥΝΟΣ
-  4: 938 ΝΕΖ
+  4: 938ΝΕΖ
   5: '2345'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1947'
   11: 47Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-Ο ΣΛΑΒΙΚΟΣ ΚΙΝΔΥΝΟΣ
   13: ΣΛΑΒΙΚΟΣ ΚΙΝΔΥΝΟΣ
@@ -10068,15 +10063,15 @@
   11: 204Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΔΕΣΠΟΤΑΤΟ
   14: ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
 - 0: 770
   1: ΝΙΚΟΛΑΟΥ,Χ.Ν
   2: ΕΠΙΤΙΜΟΣ ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ ΕΙΣ ΕΡΩΤΗΣΕΙΣ
-  4: 938 ΝΙΚ
+  4: 938ΝΙΚ
   5: '2336'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 178Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΡΩΤΗΣΕΙΣ
   13: ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΡΩΤΗΣΕΙΣ
@@ -10152,25 +10147,25 @@
   10: '1982'
   11: 81Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΝΤΙΣΤΑΣΙΑΚΗ
   13: ΑΝΤΙΣΤΑΣΙΑΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 777
   1: ΝΤΟΡΕΝ,ΚΑΡΛ
   2: ΣΥΝΤΟΜΗ ΙΣΤΟΡΙΑ ΤΗΣ ΑΜΕΡΙΚΑΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-  4: 810 ΝΤΟ
+  4: 810ΝΤΟ
   5: '381'
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1953'
   11: 122Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
 - 0: 778
   1: ΝΤΟΥΡΑΝ,ΓΟΥΙΛ
   2: ΕΚΦΡΑΣΕΙΣ ΤΗΣ ΖΩΗΣ
-  4: 800 ΝΤΟ
+  4: 800ΝΤΟ
   5: 1255-2701
   6: ΜΑΡΔΑ,ΕΛΕΝΗ
   8: ΜΠΕΡΓΑΔΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 394Σ
   12: ΠΑΓΚΟΣΜΙΑ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -10186,15 +10181,15 @@
   11: 110Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΝΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
   13: ΒΥΖΑΝΤΙΟ-ΑΥΤΟΚΡΑΤΟΡΙΑ
   14: ΚΟΡΑΝΙΟ-ΔΙΑΤΡΙΒΗ
 - 0: 780
   1: ΝΟΥΤΣΟΣ,ΠΑΝΑΓΙΩΤΗΣ ΧΡ
   2: ΟΥΤΟΠΙΑ ΚΑΙ ΙΣΤΟΡΙΑ
-  4: 938 ΝΟΥ
+  4: 938ΝΟΥ
   5: '2367'
   8: ΚΕΔΡΟΣ
   9: ΑΘΗΝΑ
   10: '1979'
   11: 186Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΟΥΤΟΠΙΑ
   13: ΟΥΤΟΠΙΑ ΚΑΙ ΙΣΤΟΡΙΑ
@@ -10224,15 +10219,15 @@
   12: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   14: ΑΡΧΕΙΟ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
 - 0: 783
   1: ΝΤΟΒΑΣ,ΙΩΑΝΝΗΣ Ν
   2: ΟΙ ΝΤΟΒΑΙΟΙ
   3: ΛΗΣΜΟΝΗΜΕΝΟΙ ΖΥΓΙΩΤΕΣ ΑΓΩΝΙΣΤΕΣ
-  4: 938.5 ΝΤΟ
+  4: 938.5ΝΤΟ
   5: '1901'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1965'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΩΝΙΣΤΕΣ 1821
   13: 1821-ΑΓΩΝΙΣΤΕΣ
   14: ΝΤΟΒΑΙΟΙ-ΑΓΩΝΙΣΤΕΣ
@@ -10248,15 +10243,15 @@
   10: '1930'
   11: 234Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΩΝΣΤΑΝΤΙΝΟΣ Α'
   13: ΚΩΝΣΤΑΝΤΙΝΟΣ Α'
 - 0: 785
   1: ΝΤΥΡΡΕΝΜΑΤ,ΦΡΕΙΔΕΡΙΚΟΣ
   2: Η ΕΠΙΣΚΕΨΗ ΤΗΣ ΓΗΡΑΙΑΣ ΚΥΡΙΑΣ
-  4: 832 ΝΤΥ
+  4: 832ΝΤΥ
   5: '1368'
   6: ΑΜΑΝΑΚΗΣ,ΗΩ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 140Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -10275,28 +10270,28 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ
   14: ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ
 - 0: 787
   1: ΞΑΝΘΟΥΔΙΔΟΥ,ΣΤΕΦ
   2: ΕΠΙΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΚΡΗΤΗΣ
   3: ΑΠΟ ΤΗΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΤΩΝ ΚΑΘ'ΗΜΑΣ
-  4: 938.98 ΞΑΝ
+  4: 938.98ΞΑΝ
   5: '2074'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1909'
   11: 173Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΡΗΤΗ
   13: ΚΡΗΤΗ
   18: ΧΑΡΤ
 - 0: 788
   1: ΞΕΝΟΣ,ΝΙΚΟΣ Γ
   2: ΠΤΥΧΕΣ ΕΥΡΩΠΗΣ
   3: ΟΔΟΙΠΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ
-  4: 940 ΞΕΝ
+  4: 940ΞΕΝ
   5: 387-2577
   8: ΚΑΣΤΑΛΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 280Σ
   12: ΕΥΡΩΠΑΙΚΗ ΙΣΤΟΡΙΑ-ΠΤΥΧΕΣ
   13: ΕΥΡΩΠΗ-ΠΤΥΧΕΣ
@@ -10323,15 +10318,15 @@
   11: 251Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΕΠΙΣΤΟΛΕΣ
   13: ΑΘΗΝΑ-ΕΠΙΣΤΟΛΕΣ
   14: ΕΠΙΣΤΟΛΕΣ-ΑΘΗΝΑ
 - 0: 791
   1: ΞΕΝΟΠΟΥΛΟΣ,ΓΡΗΓΟΡΗΣ
   2: Ο ΚΑΚΟΣ ΔΡΟΜΟΣ
-  4: 884.22 ΞΕΝ
+  4: 884.22ΞΕΝ
   5: '1049'
   7: 2ΕΚΔ
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1922'
   11: 102Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -10402,15 +10397,15 @@
   13: ΠΟΛΕΜΟΣ-ΕΛΛΗΝΟΤΟΥΡΚΙΚΟΣ
   14: 1897-ΕΛΛΗΝΟΤΟΥΡΚΙΚΟΣ ΠΟΛΕΜΟΣ
   18: ΕΙΚ,ΧΑΡΤΕΣ
 - 0: 797
   1: ΟΙΚΟΝΟΜΟΥ,ΑΛΕΞΑΝΔΡΟΣ
   2: ΤΡΕΙΣ ΑΝΘΡΩΠΟΙ
   3: ΣΥΜΒΟΛΗ ΕΙΣ ΤΗΝ ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΛΑΟΥ (1780-1935)
-  4: 938.6 ΟΙΚ
+  4: 938.6ΟΙΚ
   5: '1809'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1950'
   11: 551Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΟΙΚΟΝΟΜΟΣ-ΙΣΤΟΡΙΑ
@@ -10429,15 +10424,15 @@
   13: ΕΠΑΝΑΣΤΑΣΗ 1821
   14: ΠΑΛΙΓΓΕΝΕΣΙΑ-ΙΣΤΟΡΙΚΑ
   15: ΙΣΤΟΡΙΚΑ-(1821-1830)
 - 0: 799
   1: ΟΙΚΟΝΟΜΟΥ,ΓΕΩΡΓΙΟΣ
   2: ΙΣΤΟΡΙΑ ΤΩΝ ΤΡΙΩΝ ΕΛΙΣΑΒΕΤΕΙΩΝ ΠΑΡΘΕΝΑΓΩΓΕΙΩΝ ΤΩΝ ΙΩΑΝΝΙΝΩΝ
   3: ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ (1848-1913)
-  4: 938.4 ΟΙΚ
+  4: 938.4ΟΙΚ
   5: '2365'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1957'
   11: 91Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΩΑΝΝΙΝΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΙΩΑΝΝΙΝΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
@@ -10467,28 +10462,28 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΒΥΖΑΝΤΙΝΑ ΜΝΗΜΕΙΑ
   14: ΜΝΗΜΕΙΑ-ΒΥΖΑΝΤΙΝΑ
   15: ΒΥΖΑΝΤΙΝΑ ΜΝΗΜΕΙΑ ΑΡΤΑΣ
 - 0: 802
   1: ΟΣΜΠΟΡΝ,ΤΖΩΝ
   2: ΞΕΝΟΔΟΧΕΙΟ ΣΤΟ ΑΜΣΤΕΡΝΤΑΜ ΚΑΙ ΤΩΡΙΝΟΣ ΚΑΙΡΟΣ
-  4: 822 ΟΣΜ
+  4: 822ΟΣΜ
   5: '1374'
   6: ΜΗΤΡΟΠΟΥΛΟΣ,ΚΩΣΤ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 175Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 803
   1: ΟΣΤΡΟΓΚΟΣΚΗ,ΤΖΙΟΡΤΖΙΟ
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΒΥΖΑΝΤΙΝΟΥ ΚΡΑΤΟΥΣ
-  4: 938.3 ΟΣΤ
+  4: 938.3ΟΣΤ
   5: 1766-1767-
   6: ΠΑΝΑΓΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ
   8: ΒΑΣΙΛΟΠΟΥΛΟΣ
   9: ΑΘΗΝΑ
   10: '1979'
   11: 329Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
@@ -10506,15 +10501,15 @@
   11: 72Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΔΡΟΥΤΣΟΣ
   13: ΑΝΔΡΟΥΤΣΟΣ
 - 0: 805
   1: ΟΥΡΑΝΗΣ,ΚΩΣΤΑΣ
   2: ΙΣΠΑΝΙΑ
   3: ΤΑΞΙΔΙΑ
-  4: 889.21 ΟΥΡ
+  4: 889.21ΟΥΡ
   5: '396'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 352Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΙΣΠΑΝΙΑ
   13: ΤΑΞΙΔΙΑ-ΙΣΠΑΝΙΑ
@@ -10532,40 +10527,40 @@
   13: ΑΤΛΑΝΤΙΚΟΣ-ΤΑΞΙΔΙΑ
   14: ΜΑΥΡΗ ΘΑΛΑΣΣΑ-ΤΑΞΙΔΙΑ
   15: ΤΑΞΙΔΙΑ-ΑΤΛΑΝΤΙΚΟΣ ΕΩΣ ΜΑΥΡΗ ΘΑΛΑΣΣΑ
 - 0: 807
   1: ΟΥΡΑΝΗΣ,ΚΩΣΤΑΣ
   2: ΙΤΑΛΙΑ
   3: ΤΑΞΙΔΙΑ
-  4: 889.21 ΟΥΡ
+  4: 889.21ΟΥΡ
   5: '393'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 220Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΙΤΑΛΙΑ
   13: ΤΑΞΙΔΙΑ-ΙΤΑΛΙΑ
   14: ΙΤΑΛΙΑ-ΤΑΞΙΔΙΑ
 - 0: 808
   1: ΟΥΡΑΝΗΣ,ΚΩΣΤΑΣ
   2: ΕΛΛΑΔΑ
   3: ΤΑΞΙΔΙΑ
-  4: 899.21 ΟΥΡ
+  4: 899.21ΟΥΡ
   5: '373'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 425Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
   13: ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
   14: ΕΛΛΑΔΑ-ΤΑΞΙΔΙΑ
 - 0: 809
   1: ΟΥΩΛΤΕΡ,ΤΟΜΑΣ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΓΕΡΜΑΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-  4: 830 ΟΥΩ
+  4: 830ΟΥΩ
   5: '201'
   6: ΣΕΡΟΥΙΟΥ,Γ
   8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '1931'
   11: 280Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -10594,15 +10589,15 @@
   11: 71Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
   13: ΚΑΠΟΔΙΣΤΡΙΑΣ
   14: ΕΛΛΗΝΙΚΟ ΚΡΑΤΟΣ-ΚΑΠΟΔΙΣΤΡΙΑΣ
 - 0: 812
   1: ΠΑΛΑΙΟΛΟΓΟΣ,ΠΑΥΛΟΣ
   2: Η ΡΩΣΙΑ ΟΠΩΣ ΤΗΝ ΕΙΔΑ
-  4: 914.47 ΠΑΛ
+  4: 914.47ΠΑΛ
   5: '407'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1957'
   11: 170Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΡΩΣΙΑ
   13: ΤΑΞΙΔΙΑ-ΡΩΣΙΑ
@@ -10642,15 +10637,15 @@
   11: 139Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   14: ΠΟΙΗΜΑΤΑ
 - 0: 816
   1: ΠΑΛΑΜΑΣ,ΚΩΣΤΗΣ
   2: ΑΡΙΣΤΟΤΕΛΗΣ ΒΑΛΑΩΡΙΤΗΣ(1824-1924)
-  4: 889.25 ΠΑΛ
+  4: 889.25ΠΑΛ
   5: '997'
   8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '1924'
   11: 141Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΒΑΛΑΩΡΙΤΗΣ
@@ -10691,27 +10686,27 @@
   11: 121Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΧΙΟΣ
   13: ΤΑΞΙΔΙΑ-ΧΙΟΣ
   14: ΧΙΟΣ-ΤΑΞΙΔΙΑ
 - 0: 820
   1: ΠΑΜΠΟΥΚΗΣ,ΠΑΝΟΣ Χ
   2: ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
-  4: 938.99 ΠΑΜ
+  4: 938.99ΠΑΜ
   5: 369-2382
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1955'
   11: 115Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
   13: ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ-ΑΠΟΔΗΜΟΣ
 - 0: 821
   1: ΠΑΝΑΣ,Κ.Ι.
   2: Η ΕΛΛΗΝΙΚΗ ΜΟΥΣΙΚΗ ΚΑΙ ΤΟ ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ
-  4: 782.42 ΠΑΝ
+  4: 782.42ΠΑΝ
   5: '714'
   8: ΚΑΓΙΑΦΑ
   9: ΑΘΗΝΑ
   10: '1958'
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   14: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
@@ -10742,28 +10737,28 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   15: ΠΑΛΑΜΑΣ
 - 0: 824
   1: ΠΑΝΑΓΙΩΤΟΠΟΥΛΟΣ,ΜΕΜΟΣ
   2: ΝΕΟΕΛΛΗΝΙΚΗ ΠΟΙΗΤΙΚΗ ΑΝΘΟΛΟΓΙΑ
-  4: 880.08 ΠΑΝ
+  4: 880.08ΠΑΝ
   5: 625-626-627-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 492Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΑΝΘΟΛΟΓΙΑ
   14: ΑΝΘΟΛΟΓΙΑ-ΝΕΟΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΝΕΟΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
 - 0: 825
   1: ΠΑΝΑΓΙΩΤΟΠΟΥΛΟΣ,ΙΜ
   2: Η ΑΦΡΙΚΗ ΑΦΥΠΝΙΖΕΤΑΙ
-  4: 916 ΠΑΝ
+  4: 916ΠΑΝ
   5: '414'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1963'
   11: 199Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΑΦΡΙΚΗ
   13: ΤΑΞΙΔΙΑ-ΑΦΡΙΚΗ
@@ -10779,40 +10774,40 @@
   11: 183Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΥΠΡΟΣ
   13: ΤΑΞΙΔΙΑ-ΚΥΠΡΟΣ
   14: ΚΥΠΡΟΣ-ΤΑΞΙΔΙΑ
 - 0: 827
   1: ΠΑΝΑΓΙΩΤΟΠΟΥΛΟΣ,Ι.Μ.
   2: ΕΛΛΗΝΙΚΟΙ ΟΡΙΖΟΝΤΕΣ
-  4: 914.95 ΠΑΝ
+  4: 914.95ΠΑΝ
   5: '372'
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 413Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΗΝΙΚΟΙ ΟΡΙΖΟΝΤΕΣ
   13: ΤΑΞΙΔΙΑ-ΕΛΛΗΝΙΚΟΙ ΟΡΙΖΟΝΤΕΣ
   14: ΕΛΛΗΝΙΚΟΙ ΟΡΙΖΟΝΤΕΣ-ΤΑΞΙΔΙΑ
 - 0: 828
   1: ΠΑΝΑΓΙΩΤΟΠΟΥΛΟΣ,Ι.Μ
   2: ΤΑ ΠΡΟΣΩΠΑ ΚΑΙ ΤΑ ΚΕΙΜΕΝΑ
-  4: 880.4 ΠΑΝ
+  4: 880.4ΠΑΝ
   5: '2639'
   8: ΑΕΤΟΣ
   9: ΑΘΗΝΑ
   10: '1944'
   11: 258Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΡΟΣΩΠΑ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   14: ΠΑΛΑΜΑΣ-ΣΥΓΓΡΑΦΕΙΣ
 - 0: 829
   1: ΠΑΝΙΤΣΑΣ,ΓΙΑΝΝΗΣ
   2: ΤΑΞΙΔΕΥΟΝΤΑΣ
   3: ΜΟΡΙΑΣ
-  4: 914.95 ΠΑΝ
+  4: 914.95ΠΑΝ
   5: '2574'
   8: Χ.Ε
   9: Χ.Τ
   10: '1965'
   11: 126Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΜΟΡΙΑΣ
   13: ΤΑΞΙΔΙΑ-ΜΟΡΙΑΣ
@@ -10830,15 +10825,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΛΕΣΤΙΝΛΗΣ
   13: ΒΕΛΕΣΤΙΝΛΗΣ
   14: ΡΗΓΑΣ ΦΕΡΑΙΟΣ
   15: ΦΕΡΑΙΟΣ
 - 0: 831
   1: ΠΑΝΤΑΖΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ Ι.
   2: ΕΛΛΗΝΩΝ ΣΥΣΣΩΜΑΤΩΣΕΙΣ ΚΑΤΑ ΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑΝ
-  4: 938.4 ΠΑΝ
+  4: 938.4ΠΑΝ
   5: '1842'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1958'
   11: 39Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ
@@ -10868,28 +10863,28 @@
   11: 38Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΕΛΛΗΝΙΚΟ ΔΙΚΑΙΟ
   14: ΕΛΛΗΝΙΚΟ ΔΙΚΑΙΟ
 - 0: 834
   1: ΠΑΝΤΑΖΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ Ι.
   2: ΚΟΙΝΟΤΙΚΟΣ ΒΙΟΣ ΕΙΣ ΤΗΝ ΘΕΤΤΑΛΟΜΑΓΝΗΣΙΑΝ ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑ
-  4: 938.4 ΠΑΝ
+  4: 938.4ΠΑΝ
   5: '1905'
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1967'
   11: 103Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΘΕΤΤΑΛΟΜΑΓΝΗΣΙΑ
   14: ΘΕΤΤΑΛΟΜΑΓΝΗΣΙΑ
   18: ΠΙΝΑΚΕΣ
 - 0: 835
   1: ΠΑΝΣΕΛΗΝΟΣ,ΑΣΗΜΑΚΗΣ
   2: Η ΚΙΝΑ Η ΔΙΚΗ ΜΟΥ
-  4: 915.31 ΠΑΝ
+  4: 915.31ΠΑΝ
   5: '457'
   8: ΚΕΔΡΟΣ
   9: ΑΘΗΝΑ
   10: '1983'
   11: 140Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΙΝΑ
   13: ΤΑΞΙΔΙΑ-ΚΙΝΑ
@@ -10906,41 +10901,41 @@
   11: 303Σ
   12: ΕΛΛΗΝΙΚΗΙΣΤΟΡΙΑ-ΑΛΩΣΗ ΤΗΣ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ
   13: ΑΛΩΣΗ ΤΗΣ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗΣ
   14: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΑΛΩΣΗ
 - 0: 837
   1: ΠΑΝΤΟΠΟΥΛΟΣ,ΕΥΑΓ.
   2: Η ΝΥΦΗ ΤΗΣ ΚΟΥΛΟΥΡΗΣ
-  4: 880.2 ΠΑΝ
+  4: 880.2ΠΑΝ
   5: '1436'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 68Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
 - 0: 838
   1: ΠΑΠΠΑΣ,ΣΤΕΦΑΝΟΣ Β.
   2: ΤΑ ΝΕΑ ΨΑΡΑ
   3: ΔΡΑΜΑ
-  4: 886.2 ΠΑΠ
+  4: 886.2ΠΑΠ
   5: '1476'
   8: ΚΑΓΙΑΦΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 32Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
   14: ΔΡΑΜΑ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
 - 0: 839
   1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ-ΦΙΛΙΑΣ,ΓΕΩΡΓΙΟΣ Β.
   2: ΕΛΠΙΔΕΣ-ΕΝΘΟΥΣΙΑΣΜΟΙ ΠΟΝΟΙ ΚΑΙ ΑΠΟΓΟΗΤΕΥΣΕΙΣ
-  4: 938.7 ΠΑΠ
+  4: 938.7ΠΑΠ
   5: '2551'
   8: ΑΝΤΙΚΟΣΜΟΙ
   9: ΑΘΗΝΑ
   10: '1992'
   11: 394Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΙΚΑ ΓΕΓΟΝΟΤΑ
   13: ΠΟΛΕΜΙΚΑ ΓΕΓΟΝΟΤΑ
@@ -10958,15 +10953,15 @@
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   15: ΠΑΛΑΜΑΣ-ΑΡΤΑ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 841
   1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΠΥΡΟΣ
   2: ΑΚΕΛ ΤΟ ΑΛΛΟ ΚΚΕ
-  4: 938.8 ΠΑΠ
+  4: 938.8ΠΑΠ
   5: 2312-2313
   8: ΛΑΔΙΑΣ
   9: ΑΘΗΝΑ
   10: '1984'
   11: 379Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΚΕΛ
   13: ΑΚΕΛ-ΙΣΤΟΡΙΑ
@@ -11010,40 +11005,40 @@
   13: ΚΥΠΡΟΣ-ΦΑΚΕΛΛΟΣ
   14: ΑΤΤΙΛΑΣ-ΚΥΠΡΟΣ
   15: ΖΥΡΙΧΗ-ΚΥΠΡΟΣ
 - 0: 845
   1: ΠΑΠΑΓΙΑΝΝΗΣ,ΓΕΩΡΓΙΟΣ ΕΠ.
   2: ΑΙ ΤΡΕΙΣ ΜΕΓΑΛΥΤΕΡΑΙ ΣΥΜΦΟΡΑΙ ΤΩΝ ΕΛΛΗΝΩΝ
   3: ΚΑΤΑ ΤΟΝ ΙΕΡΟΝ ΑΓΩΝΑ
-  4: 938.5 ΠΑΠ
+  4: 938.5ΠΑΠ
   5: '1847'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 500Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΕΡΟΣ ΑΓΩΝΑΣ
   13: ΙΕΡΟΣ ΑΓΩΝΑΣ
 - 0: 846
   1: ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΤΑΚΗΣ Ε.
   2: ΕΛΛΑΣ-ΚΟΡΕΑ
   3: ΑΡΧΑΙΟΙ ΚΑΙ ΣΥΓΧΡΟΝΟΙ ΔΕΣΜΟΙ ΤΩΝ ΔΥΟ ΛΑΩΝ
-  4: 938 ΠΑΠ
+  4: 938ΠΑΠ
   5: '366'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1976'
   11: 272Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
   13: ΕΛΛΑΣ-ΚΟΡΕΑ
   14: ΚΟΡΕΑ-ΕΛΛΑΣ
 - 0: 847
   1: ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΤΑΚΗΣ Ε.
   2: Η ΕΠΟΠΟΙΙΑ ΤΟΥ ΜΠΙΖΑΝΙΟΥ
   3: ΗΘΙΚΟΣ ΘΡΙΑΜΒΟΣ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  4: 938.68 ΠΑΠ
+  4: 938.68ΠΑΠ
   5: '1943'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1980'
   11: 51Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΠΙΖΑΝΙ
   13: ΜΠΙΖΑΝΙ-ΕΠΟΠΟΙΙΑ
@@ -11062,15 +11057,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ
   13: ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ-(1923-1940)
   14: 1940-ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ
   15: ΣΤΡΑΤΟΣ-ΕΛΛΗΝΙΚΟΣ
 - 0: 849
   1: ΠΑΠΑΔΑΚΗΣ,Β.Π.
   2: ΔΙΠΛΩΜΑΤΙΚΗ ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΠΟΛΕΜΟΥ 1940-1945
-  4: 938.75 ΠΑΠ
+  4: 938.75ΠΑΠ
   5: '2008'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1956'
   11: 510Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΙΠΛΩΜΑΤΙΑ
   13: ΔΙΠΛΩΜΑΤΙΚΗ ΙΣΤΟΡΙΑ-1940
@@ -11087,42 +11082,42 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-1942
   14: 1942-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   15: ΑΝΤΙΣΤΑΣΗ-ΕΘΝΙΚΗ
 - 0: 851
   1: ΠΑΠΑΔΗΜΗΤΡΙΟΥ,ΒΙΒΗ ΔΗΜ
   2: Η ΚΟΙΝΩΝΙΚΗ ΠΟΛΙΤΙΚΗ ΚΑΙ ΟΙ ΗΠΕΙΡΩΤΑΙ ΕΘΝΙΚΟΙ ΕΥΕΡΓΕΤΑΙ
-  4: 938 ΠΑΠ
+  4: 938ΠΑΠ
   5: 2038-2039-9270
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 26Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΟΙΝΩΝΙΚΗ ΠΟΛΙΤΙΚΗ
   13: ΠΟΛΙΤΙΚΗ -ΚΟΙΝΩΝΙΚΗ
   14: ΕΘΝΙΚΟΙ ΕΥΕΡΓΕΤΕΣ
   15: ΕΥΕΡΓΕΤΕΣ-ΕΘΝΙΚΟΙ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;28
 - 0: 852
   1: ΠΑΠΑΔΗΜΗΤΡΙΟΥ,Γ.Α
   2: ΜΝΗΜΗ ΑΠΟΣΤΟΛΟΥ ΑΡΣΑΚΗ
-  4: 938 ΠΑΠ
+  4: 938ΠΑΠ
   5: '2051'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 69Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΠΡΟΣΩΠΑ=ΑΡΣΑΚΗΣ
   14: ΑΡΣΑΚΗΣ-ΜΝΗΜΗ
   15: ΜΝΗΜΗ-ΑΡΣΑΚΗΣ
 - 0: 853
   1: ΠΑΠΑΔΗΜΗΤΡΙΟΥ,ΡΟΥΛΑ
   2: ΣΤΗΝ ΕΠΟΠΟΙΙΑ ΤΟΥ 40
-  4: 938.75 ΠΑΠ
+  4: 938.75ΠΑΠ
   5: '2009'
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1958'
   11: 108Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΟΠΟΙΙΑ ΤΟΥ 40
   13: ΕΠΟΠΟΙΙΑ-1940
@@ -11263,27 +11258,27 @@
   11: 96Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ 1770
   13: ΕΠΑΝΑΣΤΑΣΗ 1770
   14: 1770-ΕΠΑΝΑΣΤΑΣΗ
 - 0: 865
   1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ
   2: ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
-  4: 938.5 ΠΑΠ
-  5: 2127-1852
+  4: 938.5ΠΑΠ
+  5: 2127-1852-14176
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1969'
   11: 62Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΑΓΩΝΕΣ
   14: ΑΓΩΝΕΣ-ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ
   15: ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ
 - 0: 866
   1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ Ι.
-  2: ΤΑ ΤΕΛΕΥΤΑΙ ΕΤΗ ΤΟΥ ΑΓΩΝΟΣ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ ΚΑΙ Η ΠΕΡΙΟΔΟΣ
+  2: ΤΑ ΤΕΛΕΥΤΑΙΑ ΕΤΗ ΤΟΥ ΑΓΩΝΟΣ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ ΚΑΙ Η ΠΕΡΙΟΔΟΣ
   3: ΔΙΑΚΥΒΕΡΝΗΣΕΙΣ ΤΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
   4: 938.571ΠΑΠ
   5: '1790'
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1976'
   11: 131Σ
@@ -11368,26 +11363,26 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
   13: ΚΑΠΟΔΙΣΤΡΙΑΣ-ΚΟΧΡΑΝ
   14: ΚΟΧΡΑΝ-ΝΑΥΑΡΧΟΣ
   15: ΝΑΥΑΡΧΟΣ ΚΟΧΡΑΝ
 - 0: 873
   1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΩΤΕΡΗΣ ΕΛΛΑΔΟΣ
-  4: 938.57 ΠΑΠ
+  4: 938.57ΠΑΠ
   5: '1853'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1983'
   11: 115Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΕΩΤΕΡΗ
   13: ΝΕΩΤΕΡΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
 - 0: 874
   1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ
   2: ΣΥΜΜΕΙΚΤΑ ΝΕΩΤΕΡΗΣ ΙΣΤΟΡΙΑΣ
-  4: 938.6 ΠΑΠ
+  4: 938.6ΠΑΠ
   5: '1856'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1982'
   11: 111Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΕΩΤΕΡΗ
   13: ΝΕΩΤΕΡΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
@@ -11419,15 +11414,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΠΕΛΕΥΘΕΡΩΣΗ
   14: ΗΠΕΙΡΩΤΕΣ-ΑΠΕΛΕΥΘΕΡΩΣΗ
 - 0: 877
   1: ΠΑΠΑΖΟΓΛΟΥ,ΘΕΟΔΩΡΟΣ Π.
   2: Η ΦΙΛΙΑ ΕΙΝΑΙ ΣΥΜΦΕΡΟΝ
   3: ΚΩΜΩΔΙΑ
-  4: 886.2 ΠΑΠ
+  4: 886.2ΠΑΠ
   5: '1524'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1956'
   11: 74Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
@@ -11446,15 +11441,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΧΑΣΙΩΤΗΣ
   14: ΧΑΣΙΩΤΗΣ-ΗΠΕΙΡΩΤΗΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;26
 - 0: 879
   1: ΠΑΠΑΘΑΝΑΣΟΠΟΥΛΟΣ,ΘΑΝΑΣΗΣ
   2: ΛΟΓΟΤΕΧΝΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
-  4: 880.4 ΠΑΠ
+  4: 880.4ΠΑΠ
   5: '195'
   8: ΘΟΥΚΥΔΙΔΗΣ
   9: ΑΘΗΝΑ
   10: '1982'
   11: 258Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΜΕΛΕΤΗΜΑΤΑ
@@ -11486,40 +11481,40 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΡΗΤΗ
   13: ΚΡΗΤΗ-Η ΜΑΧΗ ΤΗΣ ΚΡΗΤΗΣ
   14: Η ΜΑΧΗ ΤΗΣ ΚΡΗΤΗΣ
   15: 1941-ΚΡΗΤΗ
 - 0: 882
   1: ΠΑΠΑΘΕΟΔΩΡΟΥ,ΑΠΟΣΤ Π.
   2: ΣΥΜΒΟΛΗ ΣΤΗΝ ΝΕΩΤΕΡΗ ΙΣΤΟΡΙΑ ΤΗΣ ΠΕΡΙΟΧΗΣ ΔΩΔΩΝΗΣ
-  4: 938 ΠΑΠ
+  4: 938ΠΑΠ
   5: '2060'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1980'
   11: 34Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΩΔΩΝΗ
   13: ΔΩΔΩΝΗ-ΙΣΤΟΡΙΑ
 - 0: 883
   1: ΠΑΠΑΙΩΑΝΝΟΥ,ΔΗΜΗΤΡΙΟΣ
   2: ΣΧΟΛΙΚΑ ΤΡΑΓΟΥΔΙΑ
-  4: 782.42 ΠΑΠ
+  4: 782.42ΠΑΠ
   5: 712-713
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1959'
   11: 18Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
   14: ΤΡΑΓΟΥΔΙΑ-ΣΧΟΛΙΚΑ
   15: ΣΧΟΛΙΚΑ ΤΡΑΓΟΥΔΙΑ
   17: 14 ΑΝΤΙΤΥΠΑ
 - 0: 884
   1: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΣ,Θ.Φ
   2: Η ΜΑΧΗ ΤΗΣ ΕΛΛΑΔΟΣ(1940-1941)
-  4: 938.75 ΠΑΠ
+  4: 938.75ΠΑΠ
   5: 2602-1956
   8: ΓΑΛΑΞΙΑΣ
   9: ΑΘΗΝΑ
   10: '1966'
   11: 483Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-Η ΜΑΧΗ ΤΗΣ ΕΛΛΑΔΟΣ
   13: Η ΜΑΧΗ ΤΗΣ ΕΛΛΑΔΟΣ(1940-1941)
@@ -11536,28 +11531,28 @@
   11: 140Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΙΣΤΟΡΙΑ
   14: ΚΥΒΕΡΝΗΣΕΙΣ-ΕΛΛΗΝΙΚΕΣ
 - 0: 886
   1: ΠΑΠΑΝΤΩΝΙΟΥ,ΓΕΩΡΓΙΟΣ
   2: ΑΡΧΑΙΑ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
-  4: 938.1 ΠΑΠ
+  4: 938.1ΠΑΠ
   5: 1913-1912-1927-1928-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1979'
   11: 717Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΜΥΔΙΚΟΙ-ΑΧΑΙΑ
   14: ΠΕΛΟΠΟΝΝΗΣΙΑΚΟΣ ΠΟΛΕΜΟΣ
   15: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
 - 0: 887
   1: ΠΑΠΑΠΑΝΑΓΙΩΤΟΥ,ΚΩΣΤΑΣ
   2: ΒΑΣΙΛΕΙΟΣ Ο ΒΟΥΛΓΑΡΟΚΤΟΝΟΣ
-  4: 886.2 ΠΑΠ
+  4: 886.2ΠΑΠ
   5: '1467'
   8: ΚΑΜΠΑΝΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 182Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΙΛΟΓΙΑ
@@ -11573,28 +11568,28 @@
   10: '1990'
   11: 170Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ
   13: ΚΑΡΑΙΣΚΑΚΗΣ
 - 0: 889
   1: ΠΑΠΑΣΤΡΑΤΟΣ,ΕΥΑΓΓΕΛΟΣ Α.
   2: Η ΔΟΥΛΕΙΑ ΚΙ Ο ΚΟΠΟΣ ΤΗΣ
-  4: 938.09ΠΑΠ
+  4: 938.009ΠΑΠ
   5: 2431-5748
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1964'
   11: 255Σ
   12: ΒΙΟΓΡΑΦΙΑ
   13: ΒΙΟΓΡΑΦΙΕΣ
   14: ΒΙΟΓΡΑΦΙΕΣ
 - 0: 890
   1: ΠΑΠΑΣΤΑΥΡΟΣ,ΙΩΑΝΝΗΣ ΣΤ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΑΔΟΣ ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ
   3: ΜΕΧΡΙ ΤΩΝ ΠΑΡΑΜΟΝΩΝ ΤΗΣ ΡΩΜΑΙΚΗΣ ΚΥΡΙΑΡΧΙΑΣ
-  4: 938.1 ΠΑΠ
+  4: 938.1ΠΑΠ
   5: '1910'
   8: ΧΟΥΡΖΑΜΑΝΗ
   9: ΑΘΗΝΑ
   10: '1968'
   11: 543Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ
@@ -11611,27 +11606,27 @@
   11: 301Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ
   13: ΚΑΡΑΙΣΚΑΚΗΣ-ΔΙΚΗ
   14: ΔΙΚΗ-ΚΑΡΑΙΣΚΑΚΗΣ
 - 0: 892
   1: ΠΑΡΑΣΧΟΣ,ΚΛΕΩΝΟΣ Β.
   2: ΜΕΣΟΓΕΙΟ
-  4: 910 ΠΑΡ
+  4: 910ΠΑΡ
   5: '384'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 173Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΜΕΣΟΓΕΙΟΣ
   13: ΤΑΞΙΔΙΑ-ΜΕΣΟΓΕΙΟΣ
   14: ΜΕΣΟΓΕΙΟΣ-ΤΑΞΙΔΙΑ
 - 0: 893
   1: ΠΑΡΑΣΧΟΣ,ΚΛΕΩΝΟΣ
   2: ΕΥΡΩΠΑΙΚΗ ΠΕΖΟΓΡΑΦΙΑ ΚΑΙ ΠΟΙΗΣΗ
-  4: 800.1 ΠΑΡ
+  4: 800.1ΠΑΡ
   5: '2651'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1956'
   11: 214Σ
   12: ΕΥΡΩΠΑΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
   13: ΠΕΖΟΓΡΑΦΙΑ-ΕΥΡΩΠΗ
@@ -11648,28 +11643,28 @@
   11: 220Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΡΟΒΛΗΜΑΤΑ
   13: ΠΡΟΒΛΗΜΑΤΑ-ΛΟΓΟΤΕΧΝΙΑ
 - 0: 895
   1: ΠΑΡΑΣΧΟΣ,ΚΛΕΩΝΟΣ Β.
   2: ΕΛΛΗΝΕΣ ΛΥΡΙΚΟΙ
   3: ΑΠΟ ΤΟΝ ΣΟΛΩΜΟ ΕΩΣ ΣΗΜΕΡΑ
-  4: 880.3 ΠΑΡ
+  4: 880.3ΠΑΡ
   5: '226'
   8: ΣΠΥΡΟΠΟΥΛΟΣ
   9: ΑΘΗΝΑ
   10: '1953'
   11: 260Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΤΕΧΝΙΑ-ΛΥΡΙΚΟΙ
   13: ΛΥΡΙΚΟΙ-ΕΛΛΗΝΕΣ
   14: ΔΟΚΙΜΙΑ-ΛΥΡΙΚΟΙ
   15: ΣΥΓΓΡΑΦΕΙΣ
 - 0: 896
   1: ΠΑΡΑΣΧΟΣ,ΚΛΕΩΝΟΣ Β.
   2: ΔΕΚΑ ΕΛΛΗΝΕΣ ΛΥΡΙΚΟΙ
-  4: 880.3 ΠΑΡ
+  4: 880.3ΠΑΡ
   5: '1008'
   7: 2ΕΚΔ
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 214Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΛΥΡΙΚΟΙ
@@ -11701,42 +11696,42 @@
   11: 255Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΛΩΣΗ ΤΗΣ ΚΩΣΤΑΝΤΙΝΟΥΠΟΛΗΣ
   13: ΑΛΩΣΗ ΤΗΣ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗΣ
   14: ΚΩΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΑΛΩΣΗ
 - 0: 899
   1: ΠΑΤΑΤΖΗΣ,ΣΩΤΗΡΗΣ
   2: ΔΟΝ ΚΑΜΙΛΛΟ
-  4: 886.2 ΠΑΤ
+  4: 886.2ΠΑΤ
   5: '2663'
   8: ΦΙΛΙΠΠΟΤΗ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 86Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΑΤΥΡΑ
   13: ΣΑΤΥΡΑ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΣΑΤΥΡΑ
 - 0: 900
   1: ΠΑΤΡΙΑΡΧΕΑΣ,ΒΑΣΙΛΕΙΟΣ Δ.
   2: ΑΙ ΤΕΛΕΥΤΑΙΑΙ ΗΜΕΡΑΙ ΤΟΥ ΒΥΖΑΝΤΙΟΥ
   3: ΔΡΑΜΑ
-  4: 886.2 ΠΑΤ
+  4: 886.2ΠΑΤ
   5: '1466'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 90Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΒΥΖΑΝΤΙΟ
   14: ΕΛΛΗΝΙΚΟ ΔΡΑΜΑ-ΒΥΖΑΝΤΙΟ
   15: ΒΥΖΑΝΤΙΟ-ΘΕΑΤΡΟ
 - 0: 901
   1: ΠΑΤΡΙΑΡΧΕΑΣ,ΒΑΣ.Δ.
   2: Ο ΑΡΙΣΤΟΤΕΛΗΣ ΒΑΛΑΩΡΙΤΗΣ ΠΕΡΙ ΤΗΣ ΑΓΓΛΟΚΡΑΤΙΑΣ
   3: ΕΝ ΤΑΙΣ ΙΟΝΙΟΙΣ ΝΗΣΟΙΣ
-  4: 889.25 ΠΑΤ
+  4: 889.25ΠΑΤ
   5: 1000-999
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1955'
   11: 64Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
@@ -11780,15 +11775,15 @@
   11: 258Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΔΕΛΒΙΝΑΚΙ
   13: ΗΠΕΙΡΟΣ-ΔΕΛΒΙΝΑΚΙ
   14: ΔΕΛΒΙΝΑΚΙ
 - 0: 905
   1: ΠΑΤΣΙΟΥ,ΒΙΚΥ
   2: ΤΑ ΠΡΟΣΩΠΑ ΤΟΥ ΠΑΙΔΙΟΥ ΣΤΗΝ ΠΕΖΟΓΡΑΦΙΑ(1880-1930)
-  4: 880.3 ΠΑΤ
+  4: 880.3ΠΑΤ
   5: '1634'
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: '1991'
   11: 153Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -11806,79 +11801,79 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΟΠΕΥΤΗΡΙΟ ΤΗΣ ΚΑΙΣΑΡΙΑΝΗΣ
   13: ΣΚΟΠΕΥΤΗΡΙΟ ΤΗΣ ΚΑΙΣΑΡΙΑΝΗΣ-ΚΕΙΜΕΝΑ
   14: ΚΕΙΜΕΝΑ-ΣΚΟΠΕΥΤΗΡΙΟ ΤΗΣ ΚΑΙΣΑΡΙΑΝΗΣ
   15: ΚΑΙΣΑΡΙΑΝΗ
 - 0: 907
   1: ΠΑΧΥΣ,ΓΕΩΡΓΙΟΣ
   2: ΤΟ ΕΝ ΗΠΕΙΡΩ ΑΓΡΟΤΙΚΟΝ ΖΗΤΗΜΑ
-  4: 938.93 ΠΑΧ
+  4: 938.93ΠΑΧ
   5: '2153'
   8: ΠΕΡΡΗ
   9: ΑΘΗΝΑ
   10: '1882'
   11: 85Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
   14: ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ-ΗΠΕΙΡΟΣ
 - 0: 908
   1: ΠΑΧΥΣ,ΓΕΩΡΓΙΟΣ
   2: ΝΤΟΚΟΥΜΕΝΤΑ
-  4: 938.65 ΠΑΧ
+  4: 938.65ΠΑΧ
   5: 2078-2138-2176
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1981'
   11: 49Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΤΟΚΟΥΜΕΝΤΑ
   13: ΚΑΡΑΠΑΝΟΣ-ΔΗΜΟΚΡΑΤΙΑ
   14: ΒΟΥΛΓΑΡΕΛΙ-ΑΡΤΑ
   15: 1822-ΝΤΟΚΟΥΜΕΝΤΑ
 - 0: 909
   1: ΠΕΛΕΚΙΔΗ,ΧΡΥΣΗ Σ.
   2: ΙΔΕΟΛΟΓΙΚΑ ΡΕΥΜΑΤΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ ΤΗΣ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
   3: ΠΑΝΗΓΥΡΙΚΟΣ ΛΟΓΟΣ
-  4: 938.4 ΠΕΛ
+  4: 938.4ΠΕΛ
   5: '2555'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1974'
   11: 21Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΛΟΓΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ-ΙΔΕΟΛΟΓΙΚΑ ΡΕΥΜΑΤΑ
   15: ΙΔΕΟΛΟΓΙΚΑ ΡΕΥΜΑΤΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
 - 0: 910
   1: ΠΕΛΕΚΙΔΗ,ΧΡΥΣΗ
   2: ΜΕΛΕΤΕΣ ΑΡΧΑΙΑΣ ΙΣΤΟΡΙΑΣ
-  4: 938.1 ΠΕΛ
+  4: 938.1ΠΕΛ
   5: '1914'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1979'
   11: 95Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ-ΜΕΛΕΤΕΣ
   13: ΑΡΧΑΙΟΤΗΤΑ-ΜΕΛΕΤΕΣ
   14: ΜΕΛΕΤΕΣ-ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ
 - 0: 911
   1: ΠΕΝΛΙΔΗΣ,ΚΩΝ/ΝΟΣ
   2: Η ΔΙΔΑΣΚΑΛΙΑ ΤΟΥ ΠΕΖΟΓΡΑΦΗΜΑΤΟΣ
-  4: 880.09 ΠΕΝ
+  4: 880.09ΠΕΝ
   5: '2625'
   8: ΧΣ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1962'
   11: 74Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΔΙΔΑΣΚΑΛΙΑ
   14: ΠΕΖΟΓΡΑΦΙΑ-ΔΙΔΑΣΚΑΛΙΑ
 - 0: 912
   1: ΠΕΝΙΝΤΖΟΝ,ΧΕΛ
   2: ΔΥΟ ΚΟΣΜΟΙ
   3: ΑΜΕΡΙΚΗ ΚΑΙ ΡΩΣΙΑ
-  4: 970 ΡΕΝ
+  4: 970ΡΕΝ
   5: '439'
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 179Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ
   13: ΑΜΕΡΙΚΗ-ΙΣΤΟΡΙΑ
@@ -11944,63 +11939,63 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   14: ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 918
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
   2: Ο ΤΣΕΛΙΓΚΑΣ
-  4: 889.30 ΠΕΡ
+  4: 889.30ΠΕΡ
   5: '1167'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 319Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑΤΙΚΗ ΒΙΟΓΡΑΦΙΑ
   13: ΚΡΥΣΤΑΛΛΗΣ-ΒΙΟΓΡΑΦΙΑ
   14: ΒΙΟΓΡΑΦΙΑ-ΚΡΥΣΤΑΛΛΗΣ
 - 0: 919
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧΑΗΛ
   2: Η ΣΚΛΗΡΗ ΒΡΟΧΗ
   3: ΧΡΟΝΙΚΟ ΤΟΥ ΠΟΛΕΜΟΥ
-  4: 889.30 ΠΕΡ
+  4: 889.30ΠΕΡ
   5: '1175'
   7: 2ΕΚΔ
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1961'
   11: 161Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΧΡΟΝΙΚΟ ΠΟΛΕΜΟΥ
   14: ΠΟΛΕΜΟΣ-ΧΡΟΝΙΚΟ
 - 0: 920
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
   2: Ο ΔΑΙΜΟΝΑΣ
-  4: 889.30 ΠΕΡ
+  4: 889.30ΠΕΡ
   5: 1172-1173-1174-
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1974'
   11: 429Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΑΝΔΡΟΥΤΣΟΣ
   14: ΑΝΔΡΟΥΤΣΟΣ-ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 921
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
   2: ΤΟ ΧΡΩΜΑ ΤΗΣ ΘΑΛΑΣΣΑΣ
-  4: 889.30 ΠΕΡ
+  4: 889.30ΠΕΡ
   5: '1171'
   8: ΑΡΓΩ
   9: ΑΘΗΝΑ
   10: '1963'
   11: 392Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
 - 0: 922
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
   2: ΣΟΥΛΙΩΤΕΣ
-  4: 889.30 ΠΕΡ
+  4: 889.30ΠΕΡ
   5: 1177-1176-1170
   6: 2ΕΚΔ
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1957'
   11: 475Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -12022,30 +12017,30 @@
   14: ΚΑΒΑΦΗΣ-ΒΙΟΓΡΑΦΙΑ
   15: ΒΙΟΓΡΑΦΙΑ-ΚΑΒΑΦΗΣ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 924
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
   2: ΑΝΘΟΛΟΓΙΑ ΤΗΣ ΠΟΙΗΣΕΩΣ
   3: ΑΠΟ ΤΗΝ ΑΛΩΣΗ ΩΣ ΣΗΜΕΡΑ
-  4: 880.08 ΠΕΡ
+  4: 880.08ΠΕΡ
   5: 628-629-630-
   8: ΠΕΡΑΝΘΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 781Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΑΝΘΟΛΟΓΙΑ
   14: ΑΘΟΛΟΓΙΑ-ΠΟΙΗΣΗ
   15: ΠΟΙΗΣΗ
 - 0: 925
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
   2: ΑΜΒΡΑΚΙΑ
   3: ΧΡΟΝΟΓΡΑΦΙΑ ΜΙΑΣ ΠΡΩΤΕΥΟΥΣΑΣ
-  4: 938.21 ΠΕΡ
-  5: 2187-2273
+  4: 938.21ΠΕΡ
+  5: 2187-2273-13268
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1954'
   11: 212Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΜΒΡΑΚΙΑ
   13: ΑΜΒΡΑΚΙΑ-ΧΡΟΝΟΓΡΑΦΙΑ
   14: ΧΡΟΝΟΓΡΑΦΙΑ
@@ -12061,29 +12056,29 @@
   11: 157Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821-ΜΕΛΕΤΕΣ
   13: 1821-ΜΕΛΕΤΕΣ
   14: ΕΙΚΟΣΙΕΝΑ-ΜΕΛΕΤΗΜΑΤΑ
 - 0: 927
   1: ΠΕΡΙΣΤΕΡΗΣ,ΣΠΥΡΟΣ Δ.
   2: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ ΗΠΕΙΡΟΥ ΚΑΙ ΜΩΡΗΑ
-  4: 782.42 ΠΕΡ
+  4: 782.42ΠΕΡ
   5: '2622'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1950'
   11: 135Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΜΩΡΗΑΣ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   14: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ-ΗΠΕΙΡΟΣ
   15: ΗΠΕΙΡΟΣ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
 - 0: 928
   1: ΠΕΡΕΣΙΑΔΟΣ,ΣΠΥΡΙΔΩΝΟΣ
   2: Η ΣΚΛΑΒΑ
   3: ΔΡΑΜΑ
-  4: 886.2 ΠΕΡ
+  4: 886.2ΠΕΡ
   5: '2674'
   8: ΣΑΛΙΒΕΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 68Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -12100,28 +12095,28 @@
   11: 158Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΑΙΔΙΚΗ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΟΔΟΙΠΟΡΙΚΟ
   14: ΔΕΛΤΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 930
   1: ΠΕΤΙΜΕΖΑΣ,ΝΙΚΟΛΑΟΣ Η.
   2: ΗΜΕΡΟΛΟΓΙΟΝ ΕΚΣΤΡΑΤΕΙΑΣ 1912-13
-  4: 938.68 ΠΕΤ
+  4: 938.68ΠΕΤ
   5: '2079'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1981'
   11: 287Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΜΕΡΟΛΟΓΙΟ
   13: ΗΜΕΡΟΛΟΓΙΟ-1912
   14: 1912-ΕΚΣΤΡΑΤΕΙΑ
   15: ΕΚΣΤΡΑΤΕΙΑ-1912
 - 0: 931
   1: ΠΕΤΡΑΚΑΚΟΣ,ΔΗΜΗΤΡΙΟΣ Α.
   2: ΚΟΙΝΟΒΟΥΛΕΥΤΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΑΔΟΣ
-  4: 938.62 ΠΕΤ
+  4: 938.62ΠΕΤ
   5: 2143-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1946'
   11: 565Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΟΙΝΟΒΟΥΛΙΟ
   13: ΚΟΙΝΟΒΟΥΛΙΟ-ΙΣΤΟΡΙΑ
@@ -12149,15 +12144,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   14: ΠΑΛΑΜΑΣ-ΔΟΚΙΜΙΟ
   15: ΚΑΒΑΦΗΣ-ΔΟΚΙΜΙΟ
 - 0: 934
   1: ΧΑΡΗ, ΠΕΤΡΟΥ
   2: ΔΑΛΜΑΤΙΚΕΣ ΑΚΤΕΣ ΚΑΙ ΟΙ ΠΟΛΙΤΕΙΕΣ ΚΑΙ ΘΑΛΑΣΣΕΣ
-  4: 919 ΧΑΡ
+  4: 919ΧΑΡ
   5: '421'
   7: 2ΕΚΔ
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1961'
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΔΑΛΜΑΤΙΚΕΣ ΑΚΤΕΣ
   13: ΤΑΞΙΔΙΑ-ΔΑΛΜΑΤΙΚΕΣ ΑΚΤΕΣ
@@ -12198,79 +12193,79 @@
   11: 96Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΕΛΦΟΙ
   13: ΔΕΛΦΟΙ-ΙΣΤΟΡΙΑ
 - 0: 938
   1: ΠΕΤΣΑΛΗΣ-ΔΙΟΜΗΔΗΣ,Θ.
   2: Ο ΜΕΓΑΣ ΕΣΠΕΡΙΝΟΣ
   3: ΔΡΑΜΑ
-  4: 886.2 ΠΕΤ
+  4: 886.2ΠΕΤ
   5: '1520'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1960'
   11: 93Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
   14: ΔΡΑΜΑ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΔΡΑΜΑ
 - 0: 939
   1: ΠΕΤΣΚΟΥ,ΧΑΡ.Δ.
   2: Η ΠΗΝΕΛΟΠΗ ΣΕ ΗΠΕΙΡΩΤΙΚΟ ΧΩΡΙΟ
-  4: 886.2 ΠΕΤ
+  4: 886.2ΠΕΤ
   5: '1465'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 151Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
 - 0: 940
   1: ΠΙΕΡΙΔΗΣ,Γ
   2: ΕΝΑ ΤΑΞΙΔΙ ΤΟΥ Π.ΜΕΛΕΤΙΟΥ ΣΤΗ Β.ΑΦΡΙΚΗ
-  4: 916 ΠΙΕ
+  4: 916ΠΙΕ
   5: '415'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1955'
   11: 29Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-Β.ΑΦΡΙΚΗ
   13: ΑΦΡΙΚΗ-ΤΑΞΙΔΙΑ
   14: ΤΑΞΙΔΙΑ-Β.ΑΦΡΙΚΗ
 - 0: 941
   1: ΠΙΜΠΛΗΣ,ΣΠΥΡΟΣ
   2: ΔΡΑΜΑΤΟΥΡΓΙΑ
   3: Η ΘΕΑΤΡΙΚΗ ΔΡΑΣΗ
-  4: 886.2 ΠΙΜ
+  4: 886.2ΠΙΜ
   5: '2689'
   8: ΑΘΗΝΑ
   9: Χ.Ε
   10: '1980'
   11: 137Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
   14: ΔΡΑΜΑ-ΔΡΑΜΑΤΟΥΡΓΙΑ
   15: ΔΡΑΜΑΤΟΥΡΓΙΑ-ΔΡΑΜΑ
 - 0: 942
   1: ΠΙΝΤΕΡ,ΧΑΡΟΛΝΤ
   2: ΠΑΛΙΟΙ ΚΑΙΡΟΙ
-  4: 822 ΠΙΝ
+  4: 822ΠΙΝ
   5: '1405'
   6: ΤΟΛΙΚΑ,ΟΛΥΜΠΙΑ
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 28Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 943
   1: ΠΙΝΤΕΡ,ΧΑΡΟΛΝΤ
   2: ΤΟ ΘΕΡΜΟΚΗΠΙΟ
-  4: 822 ΠΙΝ
+  4: 822ΠΙΝ
   5: '1406'
   6: ΤΟΛΙΚΑ,ΟΛΥΜΠΙΑ
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 79Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -12299,67 +12294,67 @@
   10: '1951'
   11: 215Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΕΩΡΓΙΟΣ Β'
   13: ΓΕΩΡΓΙΟΣ Β'
 - 0: 946
   1: ΠΙΡΑΝΤΕΛΛΟ,ΛΟΥΙΤΖΙ
   2: ΕΤΣΙ ΕΙΝΑΙ (ΑΝ ΕΤΣΙ ΝΟΜΙΖΕΤΕ)
-  4: 852 ΠΙΡ
+  4: 852ΠΙΡ
   5: '1557'
   6: ΠΛΩΡΙΤΗΣ,ΜΑΡΙΟΣ
   8: ΓΝΩΣΗ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 87Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΙΤΑΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΙΤΑΛΙΑ
 - 0: 947
   1: ΠΙΡΑΝΤΕΛΛΟ,ΛΟΥΙΤΖΙ
   2: ΑΠΟΨΕ ΑΥΤΟΣΧΕΔΙΑΖΟΥΜΕ
-  4: 852 ΠΙΡ
+  4: 852ΠΙΡ
   5: '1559'
   6: ΜΥΡΑΤ,ΔΗΜΗΤΡΙΟΣ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 105Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΙΤΑΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΙΤΑΛΙΑ
 - 0: 948
   1: ΠΙΡΑΝΤΕΛΛΟ,ΛΟΥΙΤΖΙ
   2: ΘΕΑΤΡΙΚΑ ΕΡΓΑ
-  4: 852 ΠΙΡ
+  4: 852ΠΙΡ
   5: '1578'
   8: ΓΚΟΝΗ
   9: ΑΘΗΝΑ
   10: '1966'
   11: 262Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΙΤΑΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
   14: ΘΕΑΤΡΙΚΑ ΕΡΓΑ-ΙΤΑΛΙΑ
 - 0: 949
   1: ΠΙΡΑΝΤΕΛΛΟ,ΛΟΥΙΤΖΙ
   2: ΝΑ ΝΤΥΣΟΥΜΕ ΤΟΥΣ ΓΥΜΝΟΥΣ
-  4: 852 ΠΙΡ
+  4: 852ΠΙΡ
   5: '1556'
   6: ΠΛΩΡΙΤΗΣ,ΜΑΡΙΟΣ
   8: ΓΝΩΣΗ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 89Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΙΤΑΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΙΤΑΛΙΑ
 - 0: 950
   1: ΠΛΑΤΕΡΟ,ΝΤΑΝΙΕΛ
   2: ΟΛΥΜΠΙΑΔΑ
   3: Η ΜΗΤΕΡΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
-  4: 938.17 ΔΗΜ
+  4: 938.17ΔΗΜ
   5: '1710'
   6: ΣΚΑΡΑ,ΜΙΡΚΑ
   8: ΝΕΑ ΣΥΝΟΡΑ
   9: ΑΘΗΝΑ
   10: '1991'
   11: 400Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
@@ -12376,27 +12371,27 @@
   10: '1965'
   11: 189Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΕΡΙΑΧΙΟΝ
   13: ΤΕΡΙΑΧΙΟΝ
 - 0: 952
   1: ΠΛΙΑΤΣΙΚΑΣ,ΒΑΣΙΛΕΙΟΣ Α.
   2: ΗΠΕΙΡΩΤΙΚΕΣ ΑΝΑΔΡΟΜΕΣ
-  4: 938.7 ΠΛΙ
+  4: 938.7ΠΛΙ
   5: '2068'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 213Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΝΑΔΡΟΜΕΣ
   14: ΗΠΕΙΡΩΤΙΚΕΣ-ΑΝΑΔΡΟΜΕΣ
 - 0: 953
   1: ΠΛΙΑΤΣΙΚΑΣ,ΒΑΣΙΛΕΙΟΣ Α
   2: ΠΛΑΝΕΜΜΑΤΑ ΣΤΑ ΞΕΝΑ
-  4: 938.99 ΠΛΙ
+  4: 938.99ΠΛΙ
   5: '368'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1969'
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΔΙΑΣΠΟΡΑΣ
   13: ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΔΙΑΣΠΟΡΑΣ
@@ -12442,64 +12437,64 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΠΥΡΡΟΣ
   14: ΠΥΡΡΟΣ-Ο ΒΑΣΙΛΕΙΑΣ ΤΗΣ ΗΠΕΙΡΟΥ
   15: ΒΑΣΙΛΕΙΑΣ-ΠΥΡΡΟΣ
 - 0: 957
   1: ΠΟΛΙΤΑΡΧΗΣ,Γ.Μ.
   2: ΠΡΟΣΩΠΑ ΚΑΙ ΙΔΕΕΣ
-  4: 880.4 ΠΟΛ
+  4: 880.4ΠΟΛ
   5: '1002'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1963'
   11: 133Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΔΟΚΙΜΙΑ
   14: ΔΟΚΙΜΙΑ-ΣΥΓΓΡΑΦΕΙΣ
 - 0: 958
   1: ΠΟΛΙΤΑΡΧΗΣ,Γ.Μ.
   2: ΚΡΙΤΙΚΑ ΔΟΚΙΜΙΑ
-  4: 880.4 ΠΟΛ
+  4: 880.4ΠΟΛ
   5: '1012'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 260Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΡΙΤΙΚΑ ΔΟΚΙΜΙΑ
   13: ΚΡΙΤΙΚΑ ΔΟΚΙΜΙΑ
   14: ΔΟΚΙΜΙΑ-ΚΡΙΤΙΚΑ
 - 0: 959
   1: ΠΟΛΙΤΗΣ,ΛΙΝΟΣ
   2: Ο ΣΟΛΩΜΟΣ ΣΤΑ ΓΡΑΜΜΑΤΑ ΤΟΥ
-  4: 889.15 ΠΟΛ
+  4: 889.15ΠΟΛ
   5: '1208'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 78Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΣΟΛΩΜΟΣ
   15: ΣΟΛΩΜΟΣ
 - 0: 960
   1: ΠΟΛΙΤΗΣ,ΛΙΝΟΣ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΟΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-  4: 880.09 ΠΟΛ
+  4: 880.09ΠΟΛ
   5: 1286-2564-2787
   7: 4ΕΚΔ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1985'
   11: 446Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
   13: ΝΕΟΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
 - 0: 961
   1: ΠΟΛΙΤΗΣ,ΛΙΝΟΣ
   2: ΣΥΝΟΠΤΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΑΣ ΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-  4: 880.9 ΠΟΛ
+  4: 880.9ΠΟΛ
   5: '184'
   7: 3ΕΚΔ
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1977'
   11: 167Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -12516,27 +12511,27 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   15: ΠΑΛΑΜΑΣ
 - 0: 963
   1: ΠΟΛΙΤΗΣ,Ν.Γ.
   2: ΕΚΛΟΓΑΙ ΑΠΟ ΤΑ ΤΡΑΓΟΥΔΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΛΑΟΥ
-  4: 880.14 ΠΟΛ
+  4: 880.14ΠΟΛ
   5: '2636'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 309Σ
   12: ΕΛΛΗΝΙΚ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   14: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
 - 0: 964
   1: ΠΟΛΙΤΗΣ,ΝΙΚΟΛΑΟΣ Γ
   2: ΠΑΡΟΙΜΙΑΙ
-  4: 398 ΠΟΛΙ
+  4: 398ΠΟΛ
   5: 233-234-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 503Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΑΡΟΙΜΙΕΣ
   13: ΠΑΡΟΙΜΙΕΣ
@@ -12551,27 +12546,27 @@
   11: 342Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΠΟΛΙΤΗΣ
   14: ΠΟΛΙΤΗΣ
 - 0: 966
   1: ΠΟΛΙΤΗΣ,ΦΩΤΗΣ
   2: ΘΕΑΤΡΙΚΕΣ ΕΠΙΦΥΛΛΙΔΕΣ
-  4: 880.09 ΠΟΛ
+  4: 880.09ΠΟΛ
   5: '1408'
   8: ΓΑΛΑΞΙΑ
   9: ΑΘΗΝΑ
   10: '1964'
   11: 306Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
   14: ΘΕΑΤΡΙΚΕΣ ΕΠΙΦΥΛΛΙΔΕΣ
 - 0: 967
   1: ΠΟΛΙΤΗΣ,Ν.Γ.
   2: ΚΛΕΦΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
-  4: 782.42 ΠΟΛ
+  4: 782.42ΠΟΛ
   5: '2630'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 110Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -12600,28 +12595,28 @@
   11: 26Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ-ΣΚΟΥΠΑ
   13: ΑΡΤΑ-ΣΚΟΥΠΑ
   14: ΣΚΟΥΠΑ
 - 0: 970
   1: ΠΟΛΥΧΡΟΝΟΠΟΥΛΟΣ,ΠΑΝΟΣ
   2: ΤΑΞΙΔΙΑ ΣΤΙΣ ΧΩΡΕΣ ΤΟΥ ΗΛΙΟΥ ΚΑΙ ΤΗΣ ΟΜΙΧΛΗΣ
-  4: 914.46 ΠΟΛ
+  4: 914.46ΠΟΛ
   5: '399'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1965'
   11: 158Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΙΣΠΑΝΙΑ
   13: ΤΑΞΙΔΙΑ-ΙΣΠΑΝΙΑ
   14: ΙΣΠΑΝΙΑ
   15: ΑΓΓΛΙΑ
 - 0: 971
   1: ΠΟΛΥΧΡΟΝΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ ΕΥΣΤ.
   2: ΟΙ ΒΑΣΙΛΕΙΣ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΙ Η ΒΥΖΑΝΤΙΝΗ ΤΩΝ ΚΑΤΑΓΩΓΗ
-  4: 938.6 ΠΟΛ
+  4: 938.6ΠΟΛ
   5: 2002-2003-2004
   8: ΔΗΜΟΠΟΥΛΟΥ
   9: ΑΘΗΝΑ
   10: '1961'
   11: 174Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΑΣΙΛΕΙΑΔΕΣ
   13: ΒΑΣΙΛΕΙΑΣ-ΕΛΛΗΝΕΣ
@@ -12638,15 +12633,15 @@
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΗΝΙΚΑ ΝΗΣΙΑ
   13: ΤΑΞΙΔΙΑ-ΕΛΛΗΝΙΚΑ ΝΗΣΙΑ
   14: ΕΛΛΗΝΙΚΑ ΝΗΣΙΑ
 - 0: 973
   1: ΠΟΥΛΟΥ,ΙΩΑΝΝΗΣ ΧΡ.
   2: ΤΟ ΕΠΕΙΣΟΔΙΟΝ ΜΟΥΣΟΥΡΟΥ
   3: Η ΕΛΛΗΝΟΤΟΥΡΚΙΚΗ ΔΙΕΝΕΞΙΣ ΤΟΥ 1847
-  4: 938.63 ΠΟΥ
+  4: 938.63ΠΟΥ
   6: '1836'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1958'
   11: 116Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΟΤΟΥΡΚΙΚΗ-ΔΙΕΝΕΞΗ
   13: ΕΛΛΗΝΟΤΟΥΡΚΙΚΗ ΔΙΕΝΕΞΗ
@@ -12684,17 +12679,17 @@
   9: ΑΘΗΝΑ
   10: '1961'
   12: ΠΑΓΚΟΣΜΙΑ ΛΟΓΟΤΕΧΝΙΑ-ΒΙΟΓΡΑΦΙΕΣ
   13: ΟΥΓΚΩ
   14: ΖΟΛΑ
   15: ΣΥΜΒΟΛΙΣΜΟΣ
 - 0: 977
-  1: ΠΡΕΒΕΛΑΚΗΣ,ΕΛΕΥΘΕΡΙΟΣ
-  2: ΕΠΙΤΟΜΑΙ ΕΓΓΡΑΦΩΝ ΤΟΥ ΒΡΕΤΑΝΝΙΚΟΥ ΥΠΟΥΡΓΕΙΟΥ ΤΩΝ ΕΞΩΤΕΡΙΚΩΝ
-  4: 938.501ΠΡΕ
+  1: Χ.Σ
+  2: ΜΝΗΜΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑΣ
+  4: 938.501Χ.Σ
   5: 1805-1857-1806-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 270Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΓΓΡΑΦΑ
   13: ΕΓΓΡΑΦΑ-ΕΞΩΤΕΡΙΚΟΥ
@@ -12712,15 +12707,15 @@
   13: ΣΥΓΓΡΑΦΕΙΣ-ΚΑΖΑΝΤΖΑΚΗΣ
   14: ΚΑΖΑΝΤΖΑΚΗΣ
   15: ΟΔΥΣΣΕΙΑ-ΠΟΙΗΜΑ
 - 0: 979
   1: ΠΡΕΒΕΛΑΚΗΣ,Π
   2: ΤΟ ΗΦΑΙΣΤΕΙΟ
   3: ΔΡΑΜΑ
-  4: 886.2 ΠΡΕ
+  4: 886.2ΠΡΕ
   5: '1508'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1962'
   11: 133Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
@@ -12751,29 +12746,29 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΣΙΚΕΛΙΑΝΟΣ
   15: ΣΙΚΕΛΙΑΝΟΣ-ΒΙΟΓΡΑΦΙΑ
 - 0: 982
   1: ΠΡΟΔΡΟΜΟΥ,ΘΕΟΔΩΡΟΣ
   2: ΚΑΤΟΜΥΟΜΑΧΙΑ(ΠΟΝΤΙΚΟΓΑΤΟΠΟΛΕΜΟΣ)
-  4: 886.2 ΠΡΟ
+  4: 886.2ΠΡΟ
   5: 1510-1511
   6: ΜΑΡΚΑΚΗΣ,ΠΕΤΡΟΣ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1955'
   11: 18Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΒΥΖΑΝΤΙΟ
   14: ΒΥΖΑΝΤΙΟ-ΙΛΑΡΟΤΡΑΓΩΔΙΑ
   15: ΤΡΑΓΩΔΙΑ-ΒΥΖΑΝΤΙΟ
 - 0: 983
   1: ΠΡΩΤΟΠΑΠΑ-ΜΠΟΥΜΠΟΥΛΙΔΟΥ,ΓΛΥΚΕΡΙΑ
   2: ΤΟ ΘΕΑΤΡΟΝ ΕΝ ΖΑΚΥΝΘΟ ΑΠΟ ΤΟΥ ΙΖ' ΤΟΥ ΙΘ' ΑΙΩΝΟΣ
-  4: 886.2 ΠΡΩ
+  4: 886.2ΠΡΩ
   5: 1425-1426
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1958'
   11: 101Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ0ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΖΑΚΥΝΘΟΣ
@@ -12799,25 +12794,26 @@
   10: '1978'
   11: 202Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
   13: ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
   14: Β.ΗΠΕΙΡΟΣ-ΖΗΤΗΜΑ
 - 0: 986
   1: ΠΡΩΤΟΨΑΛΤΗΣ,ΕΜΜΑΝ Γ.
-  2: ΙΓΝΑΤΙΟΣ ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ (1766-1828)
+  2: ΜΝΗΜΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑΣ ΤΕΥΧΟΣ 1-2
+  3: ΙΓΝΑΤΙΟΣ ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ (1766-1828)
   4: 938.488ΠΡΩ
   5: 1707-1714-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1959'
   11: 295Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ
   13: ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ
   14: ΙΓΝΑΤΙΟΣ-ΜΗΤΡΟΠΟΛΙΤΗΣ ΟΥΓΓΡΟΒΛΑΧΙΑΣ
-  15: ΟΥΓΓΡΟΒΛΑΧΙΑ-ΙΓΑΝΑΤΙΟΣ
+  15: ΟΥΓΓΡΟΒΛΑΧΙΑ-ΙΓΝΑΤΙΟΣ
 - 0: 987
   1: ΠΡΩΤΟΨΑΛΤΗΣ,ΕΜΜΑΝ.Γ
   2: ΑΛΛΗΛΟΓΡΑΦΙΑ ΦΡΟΥΡΑΣ ΜΕΣΟΛΟΓΓΙΟΥ 1825-1826
   4: 938.559ΠΡΩ
   5: '2125'
   8: Χ.Ε
   9: ΑΘΗΝΑ
@@ -12826,15 +12822,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΣΟΛΟΓΓΙ
   13: ΜΕΣΟΛΟΓΓΙ-ΑΛΛΗΛΟΓΡΑΦΙΑ ΦΡΟΥΡΑΣ
   14: ΑΛΛΗΛΟΓΡΑΦΙΑ ΦΡΟΥΡΑΣ-ΜΕΣΟΛΟΓΓΙ
   15: ΦΡΟΥΡΑ-ΜΕΣΟΛΟΓΓΙ
 - 0: 988
   1: ΠΡΩΤΟΨΑΛΤΗΣ,ΕΜΜΑΝΟΥΗΛ
   2: ΔΙΔΑΓΜΑΤΑ ΑΠΟ ΤΗΝ ΕΠΑΝΑΣΤΑΣΙΝ ΤΟΥ 1821
-  4: 938.5 ΠΡΩ
+  4: 938.5ΠΡΩ
   5: '2702'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 23Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ 1821
   13: ΕΠΑΝΑΣΤΑΣΗ 1821-ΔΙΔΑΓΜΑΤΑ
@@ -12852,15 +12848,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΟΥΛΙ
   13: ΣΟΥΛΙ-ΣΟΥΛΙΩΤΕΣ
   14: ΣΟΥΛΙΩΤΕΣ-ΣΟΥΛΙ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;53
 - 0: 990
   1: ΠΡΩΤΟΨΑΛΤΗΣ,ΕΜΜΑΝΟΥΗΛ Γ.
   2: ΤΟ ΕΙΚΟΣΙΕΝΑ ΚΑΙ Η ΗΠΕΙΡΟΣ
-  4: 938.5 ΠΡΩ
+  4: 938.5ΠΡΩ
   5: 2722-2723
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 50Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-1821
   13: ΗΠΕΙΡΟΣ-1821
@@ -13086,27 +13082,27 @@
   13: ΚΡΥΣΤΑΛΛΗΣ
   14: ΜΑΒΙΛΗΣ
   15: ΡΟΔΟΚΑΝΑΚΗΣ
 - 0: 1009
   1: ΡΟΖΑΚΗΣ,ΣΤΕΦΑΝΟΣ
   2: ΔΟΚΙΜΙΑ ΚΡΙΤΙΚΗΣ
   3: Ο ΜΥΘΟΣ ΚΑΙ ΤΟ ΠΕΡΙΒΛΗΜΑ
-  4: 880.4 ΡΟΖ
+  4: 880.4ΡΟΖ
   5: '2654'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 153Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΟΚΙΜΙΑ
   13: ΔΟΚΙΜΙΑ-ΚΡΙΤΙΚΗ
   14: ΚΡΙΤΙΚΗ-ΔΟΚΙΜΙΑ
 - 0: 1010
   1: ΡΟΖΑΚΗΣ,ΠΑΝΤΕΛΗΣ Μ.
   2: ΔΙΠΛΩΜΑΤΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΕΥΡΩΠΗΣ (1920-1970)
-  4: 940 ΡΟΖ
+  4: 940ΡΟΖ
   5: '2310'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 554Σ
   12: ΕΥΡΩΠΑΙΚΗ ΙΣΤΟΡΙΑ-ΔΙΠΛΩΜΑΤΙΚΗ
   13: ΔΙΠΛΩΜΑΤΙΚΗ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
@@ -13137,27 +13133,27 @@
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
   14: ΤΡΑΓΩΔΙΑ-ΣΟΦΟΚΛΗΣ
   15: ΣΟΦΟΚΛΗΣ-ΤΡΑΓΩΔΙΑ
 - 0: 1013
   1: ΡΟΥΦΟΥ,ΡΟΔΗΣ
   2: Η ΜΕΡΑ ΤΗΣ ΚΡΙΣΗΣ
   3: ΣΚΗΝΙΚΟΣ ΜΥΘΟΣ
-  4: 886.2 ΡΟΥ
+  4: 886.2ΡΟΥ
   5: '1507'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1957'
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΜΥΘΟΣ
   15: ΜΥΘΟΣ-ΕΡΓΟ
 - 0: 1014
   1: ΡΩΜΑΝΟΣ,ΙΩΑΝΝΗΣ
   2: ΙΣΤΟΡΙΚΑ ΕΡΓΑ
-  4: 938 ΡΩΜ
+  4: 938ΡΩΜ
   5: '2155'
   8: Χ.Ε
   9: ΚΕΡΚΥΡΑ
   10: '1959'
   11: 405Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΡΓΑ
   13: ΙΣΤΟΡΙΚΑ ΕΡΓΑ
@@ -13173,29 +13169,29 @@
   11: 336Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΤΙΣΤΑΣΗ
   13: ΑΝΤΙΣΤΑΣΗ-ΠΡΟΔΟΣΙΑ
   14: ΠΡΟΔΟΣΙΑ-ΑΝΤΙΣΤΑΣΗ
 - 0: 1016
   1: ΣΑΘΑΣ,ΚΩΝ
   2: ΤΟΥΡΚΟΚΡΑΤΟΥΜΕΝΗ ΕΛΛΑΣ(1453-1821)
-  4: 938.4 ΣΑΘ
+  4: 938.4ΣΑΘ
   5: '1851'
   8: ΚΑΜΑΡΙΝΟΠΟΥΛΟΥ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 666Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΕΛΛΑΣ
   14: 1821-ΤΟΥΡΚΟΚΡΑΤΙΑ
 - 0: 1017
   1: ΣΑΘΑΣ,ΚΩΝ/ΝΟΣ Ν.
   2: ΙΣΤΟΡΙΚΟΝ ΔΟΚΙΜΙΟΝΠΕΡΙ ΤΩΝ ΠΡΟΣ ΑΠΟΤΙΝΑΞΙΝ ΤΟΥ ΟΘΩΜΑΝΙΚΟΥ
   3: ΖΥΓΟΥ ΕΠΑΝΑΣΤΑΣΕΩΝ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ(1453-1821)
   4: 938.401ΣΑΘ
-  5: '1712'
+  5: 1712-21719
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1869'
   11: 666Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΔΟΚΙΜΙΟ
   14: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ
@@ -13212,593 +13208,593 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΙΑΤΡΙΒΗ
   13: ΙΣΤΟΡΙΚΕΣ ΔΙΑΤΡΙΒΕΣ
   14: ΔΙΑΤΡΙΒΕΣ-ΙΣΤΟΡΙΑ
 - 0: 1019
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΒΑΣΙΛΙΑΣ ΛΗΡ
   3: ΤΡΑΓΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: 1329-1382
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 140Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
 - 0: 1020
   1: ΣΑΙΞΠΗΡ,ΟΥΛΛΙΑΜ
   2: ΔΩΔΕΚΑΤΗ ΝΥΧΤΑ Η ΟΤΙ ΘΕΛΕΤΕ
   3: ΚΩΜΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1330'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 108Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
   14: ΚΩΜΩΔΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΚΩΜΩΔΙΑ
 - 0: 1021
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΙΟΥΛΙΟΣ ΚΑΙΣΑΡΑΣ
   3: ΤΡΑΓΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1327'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 109Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
 - 0: 1022
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΛΙΑΣ ΡΙΧΑΡΔΟΣ Ο Γ'
   3: ΤΡΑΓΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1383'
   6: ΚΑΡΘΑΙΟΣ,Κ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 190Σ
   12: ΑΓΓΚΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
 - 0: 1023
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΙΟΥΛΙΟΣ ΚΑΙΣΑΡΑΣ
   3: ΤΡΑΓΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1381'
   6: ΚΑΡΘΑΙΟΣ,Κ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 147Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
 - 0: 1024
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΧΕΙΜΩΝΙΑΤΙΚΟ ΠΑΡΑΜΥΘΙ
   3: ΚΩΜΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1384'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 125Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
   14: ΚΩΜΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΚΩΜΩΔΙΑ
 - 0: 1025
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο Δ'
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1389'
   6: ΠΑΛΛΗΣ,Α
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 109Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1026
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΑΛΜΕΤ
   3: ΤΡΑΓΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1390'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 151Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
 - 0: 1027
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Η ΤΡΙΚΥΜΙΑ
   3: ΚΩΜΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1387'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 101Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
   14: ΚΩΜΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΚΩΜΩΔΙΑ
 - 0: 1028
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΛΙΑΣ ΡΙΧΑΡΔΟΣ Ο Β'
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1331'
   6: ΚΑΡΘΑΙΟΣ,Κ
   8: ΒΑΣΙΛΕΙΟΥ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 156Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1029
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΕΜΠΟΡΟΣ ΤΗΣ ΒΕΝΕΤΙΑΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1388'
   6: ΠΑΛΛΗΣ,ΑΛΕΞ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 98Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1030
   1: ΣΑΙΞΠΗΡ.ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΑΣ ΕΡΡΙΚΟΣ Ο ΣΤ'
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: 2475-2474-
   6: ΡΩΤΑΣ.ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 142Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1031
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΠΟΛΥ ΚΑΚΟ ΓΙΑ ΤΙΠΟΤΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1350'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 132Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1032
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΜΑΚΜΠΕΘ
   3: ΤΡΑΓΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1385'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 102Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
 - 0: 1033
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΔΩΔΕΚΑΤΗ ΝΥΧΤΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1335'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 134Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1034
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΜΕ ΤΟ ΙΔΙΟ ΜΕΤΡΟ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1348'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 135Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1035
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΤΟ ΧΕΙΜΩΝΙΑΤΙΚΟ ΠΑΡΑΜΥΘΙ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1340'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 154Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1036
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Η ΚΩΜΩΔΙΑ ΜΕ ΠΛΑΝΕΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1346'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 94Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1037
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΟΝΕΙΡΟ ΚΑΛΟΚΑΙΡΙΝΗΣ ΝΥΧΤΑΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1353'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 115Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
   15: ΚΩΜΩΔΙΑ-ΑΓΓΛΙΑ
 - 0: 1038
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΟΙ ΕΥΘΥΜΕΣ ΚΥΡΑΔΕΣ ΤΟΥ ΟΥΙΝΖΟΡ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1333'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 141Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1039
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΤΡΩΙΛΟΣ ΚΑΙ ΧΡΥΣΙΔΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1357'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 175Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1040
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΟΝΕΙΡΟ ΚΑΛΟΚΑΙΡΙΝΗΣ ΝΥΧΤΑΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1386'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 96Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
   14: ΚΩΜΩΔΙΑ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΚΩΜΩΔΙΑ
 - 0: 1041
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο ΣΤ'
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: 1324-1325-1326-
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1042
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΡΩΜΑΙΟΣ ΚΑΙ ΙΟΥΛΙΕΤΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1356'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1991'
   11: 153Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1043
   1: ΣΑΙΞΠΗΡ,ΟΥΛΛΙΑΜ
   2: Ο ΕΜΠΟΡΟΣ ΤΗΣ ΒΕΝΕΤΙΑΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: 1352-2470-2471
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1044
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΤΙΤΟΣ ΑΝΔΡΟΝΙΚΟΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: 1358-2472-2473
   6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 132Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1045
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΚΟΡΙΟΛΑΝΟΣ
   3: ΤΡΑΓΩΔΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1328'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 141Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΑΓΓΛΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
 - 0: 1046
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Η ΤΡΙΚΥΜΙΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1354'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 121Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1047
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΑΝΤΩΝΙΟΣ ΚΑΙ ΚΛΕΟΠΑΤΡΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1345'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 175Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1048
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΑΜΛΕΤ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1343'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 194Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1049
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο Δ'
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: 1341-1338-
   6: ΡΩΤΑΣ,ΒΑΣΙΛΕΙΟΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1988'
   11: 147Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1050
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΒΑΣΙΛΙΑΣ ΙΩΑΝΝΗΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1349'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 126Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1051
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΤΙΜΩΝ Ο ΑΘΗΝΑΙΟΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1355'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 121Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1052
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο Ε'
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1347'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 164Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1053
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΤΟ ΗΜΕΡΩΜΑ ΤΗΣ ΣΤΡΙΓΓΛΑΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1351'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 132Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1054
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΤΕΛΟΣ ΚΑΛΟ ΟΛΑ ΚΑΛΑ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1336'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 143Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1055
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΠΕΡΙΚΛΗΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1339'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1988'
   11: 123Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1056
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΑΓΑΠΗΣ ΑΓΩΝΑΣ ΑΓΟΝΟΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1359'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1988'
   11: 135Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1057
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΛΙΑΣ ΡΙΧΑΡΔΟΣ Ο Γ'
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1337'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1987'
   11: 176Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1058
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: Ο ΒΑΣΙΛΙΑΣ ΕΡΡΙΚΟΣ Ο Η'
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1344'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1059
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΚΟΡΙΟΛΑΝΟΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: 2468-2469
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 172Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1060
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΚΥΜΒΕΛΙΝΟΣ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1334'
   6: ΡΩΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1988'
   11: 171Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1061
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΜΑΚΒΕΘ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1332'
   6: ΚΑΡΘΑΙΟΣ,Κ
   8: ΒΑΣΙΛΕΙΟΥ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 103Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΓΓΛΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΓΓΛΙΑ
 - 0: 1062
   1: ΣΑΙΞΠΗΡ,ΟΥΙΛΛΙΑΜ
   2: ΟΠΩΣ ΑΓΑΠΑΤΕ
-  4: 822.33 ΣΑΙ
+  4: 822.33ΣΑΙ
   5: '1342'
   6: ΡΩΤΑΣ,ΒΑΣΙΛΗΣ
   8: ΕΠΙΚΑΙΡΟΤΗΤΑ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 136Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -13817,15 +13813,15 @@
   13: ΣΥΓΓΡΑΦΕΙΣ-ΜΑΒΙΛΗΣ
   14: ΜΑΒΙΛΗΣ-ΚΡΙΤΙΚΟΣ
   15: ΑΚΑΔΗΜΙΑ ΑΘΗΝΩΝ
 - 0: 1064
   1: ΣΑΚΕΛΛΑΡΙΟΥ,ΧΑΡΗΣ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΠΑΙΔΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ ΕΛΛΗΝΙΚΗ ΚΑΙ ΠΑΓΚΟΣΜΙΑ
   3: ΑΠΟ ΤΗΝ ΑΡΧΑΙΟΤΗΤΑ ΩΣ ΤΙΣ ΜΕΡΕΣ ΜΑΣ
-  4: 880.09 ΣΑΚ
+  4: 880.09ΣΑΚ
   5: '1283'
   8: ΦΙΛΙΠΠΟΤΗ
   9: ΑΘΗΝΑ
   10: '1984'
   11: 571Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΑΙΔΙΚΗ-ΙΣΤΟΡΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
@@ -13840,26 +13836,26 @@
   11: 75Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΠΑΙΔΙΚΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΑΙΔΙΚΟ
   14: ΠΑΙΔΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
 - 0: 1066
   1: ΣΑΚΕΛΛΑΡΙΟΥ,ΧΑΡΗΣ
   2: ΠΑΘΟΛΟΓΙΑ ΤΗΣ ΠΝΕΥΜΑΤΙΚΗΣ ΖΩΗΣ
-  4: 880.4 ΣΑΚ
+  4: 880.4ΣΑΚ
   5: '1013'
   8: ΦΙΛΙΠΠΟΤΗ
   9: ΑΘΗΝΑ
   10: '1983'
   11: 131Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΟΚΙΜΙΑ
   13: ΔΟΚΙΜΙΑ-ΛΟΓΟΤΕΧΝΙΑ
 - 0: 1067
   1: ΣΑΚΕΛΛΑΡΙΔΗΣ,ΝΙΚΗΤΑΣ Ο.Δ.
   2: ΤΑΞΙΔΙ-ΠΡΟΣΚΥΝΗΜΑ
-  4: 914.95 ΣΑΚ
+  4: 914.95ΣΑΚ
   5: '413'
   8: Χ.Ε
   9: Χ.Τ
   10: '1976'
   11: 20Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΠΡΟΣΚΥΝΗΜΑ
   13: ΤΑΞΙΔΙΑ-ΠΡΟΣΚΥΝΗΜΑ
@@ -13875,15 +13871,15 @@
   11: 5Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   14: ΠΑΠΑΔΙΑΜΑΝΤΗΣ
 - 0: 1069
   1: ΣΑΚΚΑΣ,ΓΡΗΓΟΡΙΟΣ ΣΠ.
   2: ΗΠΕΙΡΩΤΙΚΑ ΔΙΗΓΗΜΑΤΑ-ΧΡΟΝΟΓΡΑΦΗΜΑΤΑ
-  4: 889.21 ΣΑΚ
+  4: 889.21ΣΑΚ
   5: '2546'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1949'
   11: 100Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΧΡΟΝΟΓΡΑΦΗΜΑΤΑ
@@ -14008,15 +14004,15 @@
   11: 13Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΟΣΧΟΠΟΛΗΣ
   13: ΜΟΣΧΟΠΟΛΗ
 - 0: 1080
   1: ΣΑΡΔΕΛΗΣ,ΚΩΣΤΑΣ
   2: ΓΕΩΡΓΙΟΣ ΒΑΡΝΑΚΩΤΗΣ
   3: Ο ΠΡΟΔΟΜΕΝΟΣ ΣΤΡΑΤΗΓΟΣ ΤΟΤ 1821
-  4: 938.5 ΣΑΡ
+  4: 938.5ΣΑΡ
   5: '1954'
   8: ΕΡΕΥΝΑ
   9: ΑΘΗΝΑ
   10: '1980'
   11: 470Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821
   13: 1821-ΣΤΡΑΤΗΓΟΣ
@@ -14033,15 +14029,15 @@
   10: Χ.Χ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΑΙΔΙΚΟ
   14: ΠΑΙΔΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
 - 0: 1082
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΤΟ ΓΑΙΤΑΝΑΚΙ
-  4: 880.2 ΣΑΡ
+  4: 880.2ΣΑΡ
   5: '1607'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 72Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -14058,28 +14054,28 @@
   11: 80Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
   14: ΕΥΡΙΠΙΔΗΣ
 - 0: 1084
   1: ΣΑΧΙΝΗΣ,ΑΠΟΣΤΟΛΟΣ
   2: ΤΟ ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
-  4: 880.3 ΣΑΧ
+  4: 880.3ΣΑΧ
   5: '221'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1957'
   11: 172Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
 - 0: 1085
   1: ΣΑΧΙΝΗΣ,ΑΠΟΣΤΟΛΟΣ
   2: ΤΟ ΝΕΟΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   3: ΙΣΤΟΡΙΑ ΚΑΙ ΚΡΙΤΙΚΗ
-  4: 880.3 ΣΑΧ
+  4: 880.3ΣΑΧ
   5: '220'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1958'
   11: 316Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
@@ -14097,15 +14093,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΡΗΤΗ
   13: ΚΡΗΤΗ-ΒΕΝΙΖΕΛΟΣ
   14: ΒΕΝΙΖΕΛΟΣ-ΚΡΗΤΗ
 - 0: 1087
   1: ΣΒΟΛΟΠΟΥΛΟΣ,Δ.Κ
   2: ΠΑΝΑΓΗΣ ΤΣΑΛΔΑΡΗΣ
   3: Ο ΚΗΡΥΞ ΤΗΣ ΝΟΜΙΜΟΤΗΤΑΣ ΚΑΙ ΕΙΡΗΝΕΥΤΗΣ ΤΟΥ ΛΑΟΥ
-  4: 938.6 ΣΒΟ
+  4: 938.6ΣΒΟ
   5: '1918'
   8: ΠΥΡΣΟΣ
   9: ΑΘΗΝΑ
   10: '1946'
   11: 222Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΣΑΛΔΑΡΗΣ
   13: ΤΣΑΛΔΑΡΗΣ
@@ -14194,15 +14190,15 @@
   11: 146Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΟΡΙΝΘΟΣ
   13: ΚΟΡΙΝΘΟΣ-1821
   14: 1821-ΚΟΡΙΝΘΟΣ
 - 0: 1095
   1: ΣΙΑΤΟΠΟΥΛΟΣ,ΔΗΜΗΤΡΗΣ
   2: ΣΗΜΕΡΙΝΗ ΕΥΡΩΠΗ
-  4: 914 ΣΙΑ
+  4: 914ΣΙΑ
   5: '383'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 171Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
   13: ΕΥΡΩΠΗ-ΤΑΞΙΔΙΑ
@@ -14218,15 +14214,15 @@
   11: 66Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΔΕΣΣΑ
   13: ΕΔΕΣΣΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   14: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΕΔΕΣΣΑ
 - 0: 1097
   1: ΣΙΔΕΡΗΣ,ΓΙΑΝΝΗΣ
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΝΕΟΥ ΕΛΛΗΝΙΚΟΥ ΘΕΑΤΡΟΥ(1794-1944)
-  4: 886.2 ΣΙΔ
+  4: 886.2ΣΙΔ
   5: '1431'
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 247Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
@@ -14318,15 +14314,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΑΥΜΑΧΙΑ ΤΟΥ ΝΑΒΑΡΙΝΟΥ
   13: ΝΑΥΜΑΧΙΑ ΤΟΥ ΝΑΒΑΡΙΝΟΥ
   14: ΝΑΒΑΡΙΝΟΥ-1827
   15: 1827-ΝΑΒΑΡΙΝΟΥ
 - 0: 1105
   1: ΣΙΝΟΣ,ΑΛΕΞΑΝΔΡΟΣ
   2: Η ΓΕΩΓΡΑΦΙΚΗ ΕΝΟΤΗΣ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΜΕΣΟΓΕΙΑΚΟΥ ΧΩΡΟΥ
-  4: 914.95 ΣΙΝ
+  4: 914.95ΣΙΝ
   5: 2221-2222-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1945'
   11: 95Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΜΕΣΟΓΕΙΟΣ
   13: ΜΕΣΟΓΕΙΟΣ-ΓΕΩΓΡΑΦΙΚΗ ΕΝΟΤΗΤΑ
@@ -14342,15 +14338,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΠΡΟΞΕΝΕΙΟ ΑΡΤΑΣ
   14: ΠΡΟΞΕΝΕΙΟ ΑΡΤΑΣ
   15: ΓΑΛΛΙΚΟ ΠΡΟΞΕΝΕΙΟ ΑΡΤΑΣ
 - 0: 1107
   1: ΣΙΩΜΟΠΟΥΛΟΣ,ΚΩΣΤΑΣ
   2: Η ΚΑΤΕΡΓΑΡΑ
-  4: 886.2 ΣΙΩ
+  4: 886.2ΣΙΩ
   5: '1529'
   8: Χ.Ε
   9: ΑΡΤΑ
   10: '1930'
   11: 86Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -14366,15 +14362,15 @@
   11: 116Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΒΙΩΜΑΤΑ
 - 0: 1109
   1: ΣΙΩΜΟΠΟΥΛΟΣ,ΤΑΚΗΣ
   2: ΑΛΕΞΑΝΔΡΟΣ ΠΑΛΛΗΣ
   3: ΚΡΙΤΙΚΗ ΜΕΛΕΤΗ
-  4: 880.4 ΣΙΩ
+  4: 880.4ΣΙΩ
   5: '2649'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1955'
   11: 27Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΛΗΣ
@@ -14431,79 +14427,79 @@
   13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ-ΦΟΙΝΙΚΗ
   14: ΦΟΙΝΙΚΗ-ΣΥΝΘΗΚΗ
   15: ΣΥΝΘΗΚΗ ΦΟΙΝΙΚΗΣ
 - 0: 1114
   1: ΣΙΩΜΟΠΟΥΛΟΣ,ΣΤΥΛΙΑΝΟΣ Κ.
   2: ΠΟΛΕΜΟΣ ΚΑΙΣΑΡΑ ΚΑΙ ΠΟΜΠΗΙΟΥ ΣΤΗΝ ΗΠΕΙΡΟ ΚΑΙ ΤΗΝ ΙΛΛΥΡΙΑ
   3: (49-48Π.Χ)
-  4: 938.21 ΣΙΩ
+  4: 938.21ΣΙΩ
   5: '2244'
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1981'
   11: 91Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΚΑΙΣΑΡΑΣ
   14: ΠΟΜΠΗΙΑ
   15: ΗΠΕΙΡΟΣ-ΚΑΙΣΑΡΑΣ
 - 0: 1115
   1: ΣΚΑΛΤΣΑΡΗ,ΣΤΕΛΛΑ
   2: ΣΤΑ ΒΟΥΝΑ ΚΑΙ ΣΤΑ ΛΑΓΚΑΔΙΑ ΤΗΣ ΣΑΧΑΡΑΣ
-  4: 916 ΣΚΑ
+  4: 916ΣΚΑ
   5: '416'
   8: Χ.Ε
   9: ΠΕΙΡΑΙΑΣ
   10: '1969'
   11: 93Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΣΑΧΑΡΑ
   13: ΤΑΞΙΔΙΑ-ΣΑΧΑΡΑ
   14: ΣΑΧΑΡΑ-ΤΑΞΙΔΙΑ
 - 0: 1116
   1: ΣΚΑΝΔΑΛΗΣ,ΧΡΗΣΤΟΣ
   2: Ο ΣΚΥΛΟΣΟΦΟΣ
   3: ΙΣΤΟΡΙΚΟ ΔΡΑΜΑ
-  4: 886.2 ΣΚΑ
+  4: 886.2ΣΚΑ
   5: '1485'
   8: Χ.Ε
   9: ΓΙΑΝΝΙΝΑ
   10: '1985'
   11: 48Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΔΡΑΜΑ
   14: ΔΡΑΜΑ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΔΡΑΜΑ
 - 0: 1117
   1: ΣΚΑΝΔΑΛΗΣ,ΧΡΗΣΤΟΣ
   2: ΣΤΗΝ ΑΡΧΑΙΑ ΑΜΒΡΑΚΙΑ
-  4: 938.21 ΣΚΑ
+  4: 938.21ΣΚΑ
   5: '284'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 109Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΑΜΒΡΑΚΙΑ
   14: ΑΡΧΑΙΑ ΑΜΒΡΑΚΙΑ
 - 0: 1118
   1: ΣΚΟΥΡΤΗΣ,ΓΙΩΡΓΟΣ
   2: Ο ΚΑΡΑΓΚΙΟΖΗΣ...ΚΑΡΑΓΚΙΟΖΗΣ
-  4: 886.2 ΣΚΟ
+  4: 886.2ΣΚΟ
   5: '1531'
   8: ΚΕΔΡΟΣ
   9: ΑΘΗΝΑ
   10: '1983'
   11: 183Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΑΡΑΓΚΙΟΖΗΣ
   14: ΚΑΡΑΓΚΙΟΖΗΣ-ΘΕΑΤΡΟ ΣΚΙΩΝ
   15: ΘΕΑΤΡΙ ΣΚΙΩΝ
 - 0: 1119
   1: ΣΜΟΚΟΒΙΤΗΣ,ΓΙΩΡΓΟΣ ΒΑΣ
   2: ΑΝΘΡΩΠΕ ΑΚΟΥ ΤΗ ΜΟΥΣΙΚΗ ΣΟΥ ΠΑΙΞΕ ΣΤΟ ΡΥΘΜΟ ΣΟΥ
-  4: 886.2 ΣΜΟ
+  4: 886.2ΣΜΟ
   5: '1496'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 48Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -14519,15 +14515,15 @@
   11: 427Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-Β' ΠΑΓΚΟΣΜΙΟΣ ΠΟΛΕΜΟΣ
   13: Β'ΠΑΓΚΟΣΜΙΟΣ ΠΟΛΕΜΟΣ
   14: ΠΟΛΕΜΟΣ-Β'ΠΑΓΚΟΣΜΙΟΣ
 - 0: 1121
   1: ΣΜΥΡΝΙΑΔΟΣ,ΒΙΩΝΟΣ
   2: Η ΔΗΜΑΓΩΓΙΑ ΕΝ ΑΘΗΝΑΙΣ ΚΑΤΑ ΤΗΝ ΑΡΧΑΙΟΤΗΤΑ
-  4: 938.1 ΣΜΥ
+  4: 938.1ΣΜΥ
   5: '1757'
   8: ΚΛΕΙΣΙΟΥΝΗΣ
   9: ΑΘΗΝΑ
   10: '1945'
   11: 87Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΑΘΗΝΑ-ΑΡΧΑΙΑ ΔΗΜΑΓΩΓΙΑ
@@ -14571,15 +14567,15 @@
   12: ΠΑΓΚΟΣΜΙΑ ΛΟΓΟΤΕΧΝΙΑ-ΚΙΝΗΜΑΤΟΓΡΑΑΦΟΣ
   13: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   14: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   15: ΑΡΧΕΙΑ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
 - 0: 1125
   1: ΣΟΛΩΜΟΣ,ΑΛΕΞΗΣ
   2: ΘΕΑΤΡΙΚΟ ΤΕΤΡΑΔΙΟ
-  4: 886.2 ΣΟΛ
+  4: 886.2ΣΟΛ
   5: '1410'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 179Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΘΕΑΤΡΙΚΑ ΤΕΤΡΑΔΙΑ
@@ -14596,15 +14592,15 @@
   11: 61Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   14: ΠΟΙΗΜΑΤΑ-ΙΤΑΛΙΚΑ
 - 0: 1127
   1: ΣΟΛΩΜΟΣ,Δ
   2: ΑΠΑΝΤΑ
-  4: 889.15 ΣΟΛ
+  4: 889.15ΣΟΛ
   5: 46-44-45
   8: ΓΡΗΓΟΡΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 267Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
@@ -14624,39 +14620,39 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΜΕΛΕΤΗΜΑΤΑ
   14: ΒΑΛΚΑΝΙΑ-ΜΕΛΕΤΗΜΑΤΑ
   15: ΜΕΛΕΤΗΜΑΤΑ
 - 0: 1129
   1: ΣΟΥΛΗΣ,ΧΡΗΣΤΟΣ
   2: ΑΦΙΕΡΩΜΑ ΕΙΣ ΤΗΝ ΗΠΕΙΡΟΝ
-  4: 938.93 ΣΟΥ
+  4: 938.93ΣΟΥ
   5: 2146-2383
   8: ΜΥΡΤΙΔΗ
   9: ΑΘΗΝΑ
   10: '1956'
   11: 253Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΦΙΕΡΩΜΑ
 - 0: 1130
   1: ΣΟΥΛΤΑΤΗΣ,ΝΙΚΟΛΑΟΣ
   2: Η ΠΑΤΡΙΣ ΜΑΣ
-  4: 938 ΣΟΥ
+  4: 938ΣΟΥ
   5: '1919'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1962'
   11: 79Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΤΡΙΔΑ
   13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   14: ΠΑΤΡΙΔΑ
 - 0: 1131
   1: ΣΟΥΤΖΟΣ,ΔΗΜΗΤΡΙΟΣ
   2: ΑΓΩΝΕΣ ΓΙΑ ΤΗ ΛΕΥΤΕΡΙΑ
   3: ΤΡΕΙΣ ΙΣΤΟΡΙΚΟΙ ΣΤΑΘΜΟΙ ΤΟΥ ΝΕΩΤΕΡΟΥ ΕΛΛΗΝΙΣΜΟΥ 1854,1878,97
-  4: 938.65 ΣΟΥ
+  4: 938.65ΣΟΥ
   5: '2252'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 111Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
   13: ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
@@ -14713,28 +14709,28 @@
   11: 38Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΡΧΑΙΟ
 - 0: 1136
   1: ΣΟΥΡΑΣ,ΑΘΑΝΑΣΙΟΣ Χ
   2: Η ΣΥΜΒΟΛΗ ΤΩΝ ΑΔΕΛΦΩΝ ΡΙΖΑΡΗ ΕΙΣ ΤΗΝ ΕΠΑΝΑΣΤΑΣΙΝ ΤΟΥ 1821
-  4: 938.5 ΣΟΥ
+  4: 938.5ΣΟΥ
   5: 2729-2730-9266
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1972'
   11: 35Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ 1821
   13: ΕΠΑΝΑΣΤΑΣΗ 1821
   14: 1821-ΕΠΑΝΑΣΤΑΣΗ
   15: ΡΙΖΑΡΗΣ-1821
 - 0: 1137
   1: ΣΠΑΘΑΡΗΣ,ΣΙΜΟΣ
   2: ΤΑ ΤΡΑΓΟΥΔΙΑ ΤΟΥ ΑΙΧΜΑΛΩΤΟΥ (1941-1943)
-  4: 782.42 ΣΠΑ
+  4: 782.42ΣΠΑ
   5: '729'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1973'
   11: 77Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -14784,42 +14780,42 @@
   9: ΘΕΣ/ΝΙΚΗ
   10: '1962'
   11: 59Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΟΚΙΜΙΟ
   13: ΔΟΚΙΜΙΟ-ΕΛΛΗΝΙΚΟΤΗΤΑ
   14: ΕΛΛΗΝΙΚΟΤΗΤΑ
 - 0: 1142
-  1: ΣΠΑΡΟΥΝΗΣ,ΑΘΑΝ.Ι
+  1: ΣΜΠΑΡΟΥΝΗΣ,ΑΘΑΝ.Ι
   2: ΣΚΕΨΕΙΣ ΤΙΝΕΣ ΔΙΑ ΜΕΤΑΠΟΛΕΜΙΚΗΝ
-  4: 938 ΣΠΑ
+  4: 938ΣΜΠ
   5: '1959'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1945'
   11: 180Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΤΑΠΟΛΙΤΕΥΣΗ
   13: ΜΕΤΑΠΟΛΙΤΕΥΣΗ-1821
   14: 1821-ΜΕΤΑΠΟΛΙΤΕΥΣΗ
 - 0: 1143
   1: ΣΠΑΤΑΛΑΣ,ΓΕΡΑΣΙΜΟΣ
   2: ΣΥΓΧΡΟΝΗ ΙΤΑΛΙΚΗ ΠΟΙΗΣΗ
-  4: 851 ΣΠΑ
+  4: 851ΣΠΑ
   5: 230-231
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1959'
   11: 63Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΙΤΑΛΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   14: ΠΟΙΗΜΑΤΑ-ΙΤΑΛΙΚΑ
 - 0: 1144
   1: ΣΠΕΡΑΝΤΣΑΣ,ΣΤΕΛΙΟΣ
   2: ΟΙ ΕΛΛΗΝΕΣ ΓΙΑΤΡΟΙ-ΛΟΓΟΤΕΧΝΕΣ
   3: ΑΠΟ ΤΗΝ ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ ΩΣ ΣΤΑ ΣΗΜΕΡΑ
-  4: 880.3 ΣΠΕ
+  4: 880.3ΣΠΕ
   5: '196'
   8: ΠΕΧΛΙΒΑΝΙΔΗΣ
   9: ΑΘΗΝΑ
   10: '1961'
   11: 199Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΓΙΑΤΡΟΙ
@@ -14836,38 +14832,38 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΠΑΙΔΙΚΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΠΑΙΔΙΚΟ
   14: ΠΑΙΔΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΠΑΙΔΙΚΟ
 - 0: 1146
   1: ΣΤΑΘΑΚΗΣ,ΙΩΑΝΝΗΣ
   2: Η ΖΩΗ ΜΟΥ ΕΙΣ ΜΙΑΝ ΑΚΤΙΝΑ ΗΛΙΟΥ
-  4: 938.7 ΣΤΑ
+  4: 938.7ΣΤΑ
   5: '2108'
   8: ΓΕΩΡΓΙΑΔΗΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 247Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΦΗΓΗΣΕΙΣ
   13: ΠΟΛΙΤΙΚΕΣ-ΑΦΗΓΗΣΕΙΣ
   14: ΙΣΤΟΡΙΚΕΣ-ΑΦΗΓΗΣΕΙΣ
 - 0: 1147
   1: ΣΤΑΘΑΚΗΣ,ΝΙΚΟΣ Α
   2: ΑΠΟ ΤΗ ΣΤΑΧΤΗ ΣΤΗ ΖΩΗ
-  4: 950 ΣΤΑ
+  4: 950ΣΤΑ
   5: '2638'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1982'
   11: 257Σ
   12: ΑΣΙΑΤΙΚΗ ΙΣΤΟΡΙΑ
   13: ΑΣΙΑ-ΙΣΤΟΡΙΑ
 - 0: 1148
   1: ΣΤΑΘΑΚΟΠΟΥΛΟΣ,ΛΟΥΚΑΣ
   2: ΑΝΘΟΛΟΓΙΑ ΠΟΙΗΤΩΝ ΑΡΓΟΛΙΔΟΣ
-  4: 880.08 ΣΤΑ
+  4: 880.08ΣΤΑ
   5: '640'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1958'
   11: 256Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΑΝΘΟΛΟΓΙΑ
@@ -14885,15 +14881,15 @@
   12: ΚΥΠΡΙΑΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΚΥΠΡΙΑΚΟ ΘΕΑΤΡΟ-ΕΠΙΚΟ ΠΟΙΗΜΑ
   14: ΕΠΙΚΟ ΠΟΙΗΜΑ
   15: ΚΥΠΡΟΣ-ΕΠΙΚΟ ΠΟΙΗΜΑ
 - 0: 1150
   1: ΣΤΑΘΗΣ,ΓΕΩΡΓΙΟΣ
   2: ΑΠΟ Τ'ΑΓΡΑΦΑ
-  4: 938.93 ΣΤΑ
+  4: 938.93ΣΤΑ
   5: '313'
   8: Χ.Ε
   9: Η.Π.Α
   10: '1957'
   11: 267Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΡΑΦΑ
   13: ΑΓΡΑΦΑ-ΙΣΤΟΡΙΑ
@@ -14910,27 +14906,27 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ-ΕΔΕΣΣΑ
   13: ΕΔΕΣΣΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   14: ΤΟΥΡΚΟΚΡΑΤΙΑ
   21: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ;6
 - 0: 1152
   1: ΣΤΑΛΙΟΣ,Ζ
   2: ΙΑΠΩΝΙΑ
-  4: 915 ΣΤΑ
+  4: 915ΣΤΑ
   5: '452'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1962'
   11: 238Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΙΑΠΩΝΙΑ
   13: ΤΑΞΙΔΙΑ-ΙΑΠΩΝΙΑ
   14: ΙΑΠΩΝΙΑ-ΤΑΞΙΔΙΑ
 - 0: 1153
   1: ΣΤΑΜΑΤΟΠΟΥΛΟΣ,ΤΑΚΗΣ Α
   2: Ο ΕΣΩΤΕΡΙΚΟΣ ΑΓΩΝΑΣ ΠΡΙΝ ΚΑΙ ΚΑΤΑ ΤΗΝ ΕΠΑΝΑΣΤΑΣΗ ΤΟΥ 1821
-  4: 938.41 ΣΤΑ
+  4: 938.41ΣΤΑ
   5: '1810'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1957'
   11: 422Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ 1821
   13: ΕΠΑΝΑΣΤΑΣΗ 1821-ΕΣΩΤΕΡΙΚΟΣ ΑΓΩΝΑΣ
@@ -15023,15 +15019,15 @@
   11: '62'
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ
   14: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
 - 0: 1161
   1: ΣΤΑΣΙΝΟΠΟΥΛΟΣ,ΝΙΚΟΣ Α.
   2: ΤΡΑΓΟΥΔΙΑ ΣΤΑ ΚΑΛΑΒΡΥΤΑ
-  4: 782.42 ΣΤΑ
+  4: 782.42ΣΤΑ
   5: '747'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 30Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -15063,40 +15059,40 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΝΙΚΑΙΑ
   13: ΝΙΚΑΙΑ-13 ΑΙΩΝΑΣ
   14: ΗΠΕΙΡΟΣ-13 ΑΙΩΝΑΣ
   21: ΕΤΑΙΡΕΙΑ ΒΥΖΑΝΤΙΝΩΝ ΕΡΕΥΝΩΝ;7
 - 0: 1164
   1: ΣΤΑΥΡΙΔΟΥ,ΜΑΡΙΑ
   2: ΣΥΓΧΡΟΝΟ ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ
-  4: 886.2 ΣΤΑ
+  4: 886.2ΣΤΑ
   5: 1491-1490
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1976'
   11: 163Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΣΥΓΧΡΟΝΟ
   14: ΘΕΑΤΡΙΚΑ ΕΡΓΑ-ΣΥΓΧΡΟΝΑ
 - 0: 1165
   1: ΣΤΑΥΡΙΔΟΥ,ΜΑΡΙΑ
   2: ΣΥΓΧΡΟΝΟ ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ
-  4: 886.2 ΣΤΑ
+  4: 886.2ΣΤΑ
   5: '1489'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1979'
   11: 207Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΣΥΓΧΡΟΝΟ
   14: ΘΕΑΤΡΙΚΑ ΕΡΓΑ-ΣΥΓΧΡΟΝΑ
   15: ΘΕΑΤΡΟ ΣΚΙΩΝ-ΕΡΓΑ
 - 0: 1166
   1: ΣΤΑΥΡΟΥ,ΤΑΤΙΑΝΑ
   2: ΤΕΤΡΑΔΙΑ ΜΝΗΜΗΣ
-  4: 880.3 ΣΤΑ
+  4: 880.3ΣΤΑ
   5: '1009'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1982'
   11: 110Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΜΥΡΙΒΗΛΗΣ
@@ -15115,15 +15111,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   15: ΠΑΛΑΜΑΣ
 - 0: 1168
   1: ΣΤΑΥΡΟΠΟΥΛΟΣ,ΧΑΡΑΛΑΜΠΟΣ Π
   2: Η ΖΩΗ ΤΟΥ ΕΛΛΗΝΟΣ ΣΤΗΝ ΑΜΕΡΙΚΗ
-  4: 938.99 ΣΤΑ
+  4: 938.99ΣΤΑ
   5: '2346'
   7: 2ΕΚΔ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1956'
   11: 95Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΔΙΑΣΠΟΡΑΣ
@@ -15154,62 +15150,62 @@
   11: 19Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΖΟΥΜΕΡΚΑ-1821
   13: ΗΠΕΙΡΟΣ-ΤΖΟΥΜΕΡΚΑ
   14: ΤΖΟΥΜΕΡΚΑ-ΗΠΕΙΡΟΣ
 - 0: 1171
   1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,ΚΩΝΣΤ.
   2: ΠΑΡΑΤΗΡΗΣΕΙΣ ΕΙΣ ΤΗΝ ΝΕΩΤΕΡΑΝ ΓΕΩΓΡΑΦΙΑΝ ΤΗΣ ΗΠΕΙΡΟΥ
-  4: 914.95 ΣΤΕ
+  4: 914.95ΣΤΕ
   5: '2544'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1937'
   11: 98Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΓΕΩΓΡΑΦΙΑ
 - 0: 1172
   1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ.
   2: ΟΙ ΥΠΕΥΘΥΝΟΙ ΠΟΛΕΜΟΥ ΚΑΤΑ ΤΟΥΣ ΑΡΧΑΙΟΥΣ ΧΡΟΝΟΥΣ
-  4: 938.1 ΣΤΕ
+  4: 938.1ΣΤΕ
   5: 2515-2586
   8: ΣΙΔΕΡΗ
   9: ΑΘΗΝΑ
   10: '1952'
   11: 192Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ-ΥΠΕΥΘΥΝΟΙ ΠΟΛΕΜΟΥ
   14: ΠΟΛΕΜΟΣ-ΥΠΕΥΘΥΝΟΙ
 - 0: 1173
   1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ.
   2: ΤΑ ΒΟΡΕΙΑ ΣΥΝΟΡΑ ΤΗΣ ΗΠΕΙΡΟΥ
-  4: 938.93 ΣΤΕ
+  4: 938.93ΣΤΕ
   5: '2553'
   8: ΓΡΗΓΟΡΙΑΔΗ
   9: ΑΘΗΝΑ
   10: '1945'
   11: 79Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΣΥΝΟΡΑ
   14: ΣΥΝΟΡΑ-ΗΠΕΙΡΟΣ
 - 0: 1174
   1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
   2: Η ΑΡΧΑΙΑ ΑΙΤΩΛΙΑ
-  4: 938.22 ΣΤΕ
+  4: 938.22ΣΤΕ
   5: 2215-2587
   8: ΔΗΜΗΤΡΑΚΟΥ
   9: ΑΘΗΝΑ
   10: '1939'
   11: 191Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΙΑ
   14: ΑΙΤΩΛΙΑ-ΑΡΧΑΙΑ
 - 0: 1175
   1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
   2: Η ΙΣΤΟΡΙΚΗ ΜΝΗΜΗ
-  4: 938 ΣΤΕ
+  4: 938ΣΤΕ
   5: '2110'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1972'
   11: 21Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΝΗΜΗ
   13: ΜΝΗΜΗ ΙΣΤΟΡΙΚΗ
@@ -15264,15 +15260,15 @@
   11: 93Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΑΡΤΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   14: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΑΡΤΑ
 - 0: 1180
   1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
   2: ΑΙ ΗΠΕΙΡΩΤΙΣΣΑΙ ΕΙΣ ΤΟΥΣ ΕΘΝΙΚΟΥΣ ΑΓΩΝΑΣ
-  4: 938 ΣΤΕ
+  4: 938ΣΤΕ
   5: 2030-2031-9268
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 32Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΙΣΣΕΣ
@@ -15390,56 +15386,56 @@
   11: 896Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΝΙΚΗΦΟΡΟΣ ΦΩΚΑΣ
   14: ΦΩΚΑΣ ΝΙΚΗΦΟΡΟΣ
 - 0: 1190
   1: ΣΕΜΠΕΡ ΚΑΙ ΡΟΥΣΣΕΤ
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΓΑΛΛΟ-ΓΕΡΜΑΝΙΚΟΥ ΠΟΛΕΜΟΥ (1870-1871)
-  4: 940.2 ΣΕΜ
+  4: 940.2ΣΕΜ
   5: '2311'
   6: ΝΕΟΚΛΕΟΥΣ,Χ
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1898'
   11: 556Σ
   12: ΕΥΡΩΠΑΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
   13: ΓΑΛΛΟ-ΓΕΡΜΑΝΙΚΟΣ ΠΟΛΕΜΟΣ
   14: ΓΑΛΛΙΑ-ΠΟΛΕΜΟΣ
   15: ΓΕΡΜΑΝΙΑ-ΠΟΛΕΜΟΣ
 - 0: 1191
   1: ΣΤΡΑΒΟΛΕΜΟΣ,ΔΙΟΝΥΣΙΟΣ Χ.
   2: ΕΝΑΣ ΗΡΩΙΣΜΟΣ-ΜΙΑ ΔΙΚΑΙΩΣΗ
   3: Η ΔΙΑΣΩΣΗ ΤΩΝ ΕΒΡΑΙΩΝ ΤΗΣ ΖΑΚΥΝΘΟΥ ΣΤΗ ΚΑΤΟΧΗ
-  4: 938.7 ΣΤΡ
+  4: 938.7ΣΤΡ
   5: '1985'
   8: Χ.Χ
   9: ΑΘΗΝΑ
   10: '1988'
   11: 124Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΖΑΚΥΝΘΟΣ
   13: ΖΑΚΥΝΘΟΣ-ΚΑΤΟΧΗ
   14: ΚΑΤΟΧΗ-ΕΒΡΑΙΟΙ
   15: ΕΒΡΑΙΟΙ
 - 0: 1192
   1: ΣΤΡΑΤΗΣ,ΚΩΝ
   2: ΧΡΟΝΙΚΟΝ ΑΡΤΗΣ
   4: 938.939ΣΤΡ
-  5: 2148-8014
+  5: 2148-8014-10001
   8: Χ.Ε
   9: ΑΡΤΑ
   10: '1969'
   11: 176Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΧΡΟΝΙΚΟ
   14: ΧΡΟΝΙΚΟ-ΑΡΤΑ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 1193
   1: ΣΤΡΑΤΗΣ,ΚΩΝΑΝΤΩΝ
   2: ΑΜΒΡΑΚΙΑ-ΑΡΑΧΘΕΙΑ ΑΚΑΡΝΑΝΙΚΗ-ΑΡΤΑ
-  4: 938.21 ΣΤΡ
+  4: 938.21ΣΤΡ
   5: '2259'
   8: Χ.Ε
   9: ΑΡΤΑ
   10: '1976'
   11: 97Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΜΒΡΑΚΙΑ
   13: ΑΜΒΡΑΚΙΑ-ΙΣΤΟΡΙΑ
@@ -15456,41 +15452,41 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΙΣΤΟΡΙΑ
   14: ΚΩΝΣΤΑΝΤΙΝΟΣ Γ'-ΒΥΖΑΝΤΙΟ
   15: ΚΩΝΣΤΑΝΤΙΝΟΣ Δ'-ΒΥΖΑΝΤΙΟ
 - 0: 1195
   1: ΣΥΓΚΕΛΛΟΣ,ΓΕΩΡΓΙΟΣ
   2: ΕΚΛΟΓΗ ΧΡΟΝΟΓΡΑΦΙΑΣ
-  4: 938.31 ΣΥΓ
+  4: 938.31ΣΥΓ
   5: '2548'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 788Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΧΡΟΝΟΓΡΑΦΙΑ
   14: ΧΡΟΝΟΓΡΑΦΙΑ-ΒΥΖΑΝΤΙΟ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 1196
   1: ΣΥΝΑΔΙΝΟΣ,ΝΙΚ Θ
   2: ΔΑΝΙΑ
   3: Η ΧΩΡΑ ΤΟΥ ΑΝΤΕΡΣΕΝ
-  4: 914.49 ΣΥΝ
+  4: 914.49ΣΥΝ
   5: '401'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1964'
   11: 130Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΔΑΝΙΑ
   13: ΤΑΞΙΔΙΑ-ΔΑΝΙΑ
   14: ΔΑΝΙΑ-ΤΑΞΙΔΙΑ
 - 0: 1197
   1: ΣΥΡΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   2: Η ΑΜΕΡΙΚΗ ΧΩΡΙΣ ΦΑΝΤΑΣΙΑ
-  4: 970 ΣΥΡ
+  4: 970ΣΥΡ
   5: '437'
   8: ΑΕΤΟΣ
   9: ΑΘΗΝΑ
   10: '1954'
   11: 176Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ
   13: ΑΜΕΡΙΚΗ-ΙΣΤΟΡΙΑ
@@ -15530,15 +15526,15 @@
   11: 190Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΣΠΑΝΙΚΕΣ ΕΠΙΧΕΙΡΗΣΕΙΣ
   13: ΙΣΠΑΝΙΚΕΣ ΕΠΙΧΕΙΡΗΣΕΙΣ-ΕΛΛΑΔΑ
   14: ΕΠΙΧΕΙΡΗΣΕΙΣ-ΙΣΠΑΝΙΚΕΣ
 - 0: 1201
   1: ΣΩ,ΜΠΕΡΝΑΡ
   2: Ο ΑΝΘΡΩΠΟΣ ΚΑΙ ΤΑ ΟΠΛΑ
-  4: 828.99 ΣΩ
+  4: 828.99ΣΩ
   5: '1369'
   6: ΜΠΕΛΛΟΥ,ΖΕΤΤΑ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 151Σ
   12: ΙΡΛΑΝΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -15557,15 +15553,15 @@
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
   14: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ-ΚΑΠΠΑΔΟΚΙΑ
   15: ΚΑΠΠΑΔΟΚΙΑ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
 - 0: 1203
   1: ΤΑΞΙΑΡΧΗΣ,ΝΤΙΝΟΣ
   2: ΕΝΑ ΔΡΑΜΑ ΤΙΜΗΣ
   3: ΜΟΝΟΠΡΑΚΤΟ
-  4: 886.2 ΤΑΞ
+  4: 886.2ΤΑΞ
   5: '1521'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1960'
   11: 46Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΜΟΝΟΠΡΑΚΤΟ
@@ -15595,28 +15591,28 @@
   11: 95Σ
   12: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   14: ΑΡΧΕΙΟ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
 - 0: 1206
   1: ΤΑΡΣΟΥΛΗ,ΓΕΩΡΓΙΑ
   2: ΜΩΡΑΙΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
-  4: 782.42 ΤΑΡ
+  4: 782.42ΤΑΡ
   5: '726'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 208Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
   14: ΤΡΑΓΟΥΔΙΑ-ΜΩΡΑΙΤΙΚΑ
   15: ΜΩΡΑΙΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
 - 0: 1207
   1: ΤΑΤΣΙΟΠΟΥΛΟΣ,ΛΑΜΠΡΟΣ ΑΠ
   2: ΝΙΚΟΛΑΟΣ ΣΚΟΥΦΑΣ
-  4: 886.2 ΤΑΤ
+  4: 886.2ΤΑΤ
   5: 1482-1483-9279Α
   8: Χ.Ε
   9: ΑΡΤΑ
   10: '1971'
   11: 40Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
@@ -15638,28 +15634,28 @@
   15: ΑΓΡΟΤΙΚΟ ΚΙΝΗΜΑ-ΚΟΜΠΟΤΙ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 1209
   1: ΤΑΤΣΙΟΠΟΥΛΟΣ,ΛΑΜΠΡΟΣ ΑΠ
   2: ΝΙΚΟΛΑΟΣ ΣΚΟΥΦΑΣ
   3: Ο ΕΘΝΕΓΕΡΤΗΣ ΑΡΧΗΓΟΣ ΤΗΣ ΦΙΛΙΚΗΣ ΕΤΑΙΡΕΙΑΣ
   4: 938.487ΤΑΤ
-  5: 2256-1034-1661
+  5: 2256-1034-1661-1482.
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1980'
   11: 73Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΟΥΦΑΣ
   13: ΣΚΟΥΦΑΣ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
   14: ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ-ΣΚΟΥΦΑΣ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 1210
   1: ΤΑΤΣΙΟΠΟΥΛΟΣ,ΛΑΜΠΡΟΣ ΑΠ.
   2: ΕΥΣΤΑΘΙΟΣ ΓΕΡΟΣΤΑΘΗΣ
   3: Ο ΣΟΦΟΣ ΔΑΣΚΑΛΟΣ
-  4: 938.7 ΤΑΤ
+  4: 938.7ΤΑΤ
   5: '2405'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1982'
   11: 78Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ- ΓΕΡΟΣΤΑΘΗΣ
   13: ΓΕΡΟΣΤΑΘΗΣ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
@@ -15687,15 +15683,15 @@
   11: 15Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-1821
   14: 1821-ΑΡΤΑ
 - 0: 1213
   1: ΤΕΝΕΚΙΔΟΣ,ΓΕΩΡΓΙΟΣ
   2: ΑΙ ΑΡΧΑΙΟΕΛΛΗΝΙΚΑΙ ΡΙΖΑΙ ΤΟΥ ΕΙΚΟΣΙΕΝΑ
-  4: 938.5 ΤΕΝ
+  4: 938.5ΤΕΝ
   5: '1879'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1962'
   11: 43Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821
   13: 1821-ΠΑΝΗΓΥΡΙΚΟΣ ΛΟΓΟΣ
@@ -15738,15 +15734,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΤΕΡΖΑΚΗΣ
   14: ΤΕΡΖΑΚΗΣ
 - 0: 1217
   1: ΤΕΡΖΑΚΗΣ,ΑΓΓΕΛΟΣ
   2: Ο ΣΤΑΥΡΟΣ ΚΑΙ ΤΟ ΣΠΑΘΙ
   3: ΤΡΑΓΩΔΙΑ
-  4: 886.2 ΤΕΡ
+  4: 886.2ΤΕΡ
   5: '1525'
   8: ΑΕΤΟΣ
   9: ΑΘΗΝΑ
   10: '1950'
   11: 125Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
@@ -15762,15 +15758,15 @@
   11: 296Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΤΕΡΖΑΚΗΣ
   14: ΤΕΡΖΑΚΗΣ
 - 0: 1219
   1: ΤΕΡΖΑΚΗΣ,ΑΓΓΕΛΟΣ
   2: ΘΕΑΤΡΟ
-  4: 886.2 ΤΕΡ
+  4: 886.2ΤΕΡ
   5: '1568'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 238Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
@@ -15849,28 +15845,28 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΤΕΡΖΑΚΗΣ
   14: ΤΕΡΖΑΚΗΣ
 - 0: 1226
   1: ΤΖΙΑΚΟΖΑ,ΙΩΣΗΦ
   2: ΣΑΝ ΤΑ ΦΥΛΛΑ
   3: ΚΩΜΩΔΙΑ
-  4: 852 ΤΖΙ
+  4: 852ΤΖΙ
   5: '1392'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1916'
   11: 84Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΙΤΑΛΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
   14: ΚΩΜΩΔΙΑ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΚΩΜΩΔΙΑ
 - 0: 1227
   1: ΤΖΙΟΒΑΣ,ΔΗΜΗΤΡΙΟΣ
   2: Η ΠΕΖΟΓΡΑΦΙΑ ΤΟΥ ΔΗΜΗΤΡΗ ΧΑΤΖΗ
-  4: 880.5 ΤΖΙ
+  4: 880.5ΤΖΙ
   5: '2645'
   8: Χ.Ε
   9: ΓΙΑΝΝΙΝΑ
   10: '1980'
   11: 23Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΣΥΓΓΡΑΦΕΙΣ
@@ -15901,15 +15897,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ
   14: ΔΙΑΜΑΝΤΗ-ΖΩΗ ΚΑΙ ΕΡΓΟ
 - 0: 1230
   1: ΤΖΟΥΝΗΣ,ΤΡΙΑΝΤ
   2: ΜΕΤΑ 49 ΧΡΟΝΙΑ ΣΤΗΝ ΠΑΛΙΑ ΠΑΤΡΙΔΑ
   3: Η ΝΟΣΤΑΛΓΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΘΡΑΚΗΣ
-  4: 938 ΤΖΟ
+  4: 938ΤΖΟ
   5: '2140'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1966'
   11: 15Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
   13: ΘΡΑΚΗ-ΕΛΛΗΝΕΣ
@@ -15938,15 +15934,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΡΗΤΗ
   13: ΚΡΗΤΗ-ΧΑΝΙΑ
   14: ΧΑΝΙΑ-ΚΑΜΠΑΝΟΥ
   15: ΚΑΜΠΑΝΟΥ-ΧΑΝΙΑ
 - 0: 1233
   1: ΔΙΑΜΑΝΤΟΠΟΥΛΟΣ,ΙΑΚΩΒΟΣ Γ.
   2: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΗΝ 15 ΙΟΥΛΙΟΥ 1965
-  4: 938.78 ΔΙΑ
+  4: 938.78ΔΙΑ
   5: '2781'
   8: Χ.Ε
   9: Χ.Τ
   10: '1972'
   11: 30Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΑΜΝΗΣΕΙΣ
   13: ΑΝΑΜΝΗΣΕΙΣ-1965
@@ -15965,15 +15961,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΔΙΧΟΝΟΙΑ
   14: ΔΙΧΟΝΟΙΑ
 - 0: 1235
   1: ΚΑΛΟΓΙΑΝΝΗΣ,ΒΑΣΟΣ
   2: Η ΧΡΥΣΗ ΒΙΒΛΟΣ ΤΟΥ ΔΗΜΟΥ-ΛΑΡΙΣΗΣ
   3: ΑΠΟ ΤΗΝ ΜΑΚΡΑΙΩΝΗ ΙΣΤΟΡΙΑ ΤΗΣ ΘΕΣΣΑΛΙΚΗΣ ΠΡΩΤΕΥΟΥΣΗΣ
-  4: 938.21 ΚΑΛ
+  4: 938.21ΚΑΛ
   5: '2374'
   8: ΔΗΜΗΤΡΑΚΟΠΟΥΛΟΥ
   9: ΛΑΡΙΣΑ
   10: '1963'
   11: 390Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΣΑΛΙΑ-ΛΑΡΙΣΑ
   13: ΘΕΣΣΑΛΙΑ-ΛΑΡΙΣΑ
@@ -15991,15 +15987,15 @@
   13: ΑΛΒΑΝΙΑ
   14: ΒΟΥΛΓΑΡΙΑ
   15: ΓΙΟΥΓΚΟΣΛΑΒΙΑ
 - 0: 1237
   1: ΠΕΤΣΑΣ,ΦΩΤΙΟΣ Μ.
   2: ΣΕΛΙΔΕΣ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΤΩΝ ΗΠΕΙΡΩΤΩΝ
   3: ΑΠΟ ΤΟΥΣ ΜΥΘΙΚΟΥΣ ΧΡΟΝΟΥΣ ΩΣ ΤΗΣ ΜΕΡΕΣ ΜΑΣ
-  4: 938.21 ΠΕΤ
+  4: 938.21ΠΕΤ
   5: '2815'
   8: ΙΑΙΑΧ
   9: ΙΩΑΝΝΙΝΑ
   10: '1993'
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ
@@ -16014,56 +16010,56 @@
   11: 189Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΣΗ ΑΝΑΤΟΛΗ
   13: ΜΕΣΗ ΑΝΑΤΟΛΗ-ΑΝΩΜΑΛΙΕΣ
   14: ΜΙΚΡΑ ΑΣΙΑ-ΑΝΩΜΑΣΙΕΣ
 - 0: 1239
   1: ΛΑΖΑΡΙΔΗΣ,ΚΩΣΤΑΣ Π.
   2: ΑΠΟ ΤΑ ΛΑΟΓΡΑΦΙΚΑ ΤΟΥ ΧΩΡΙΟΥ ΜΟΥ ΚΟΥΚΟΥΛΙΟΥ-ΖΑΓΟΡΙΟΥ
-  4: 938.93 ΛΑΖ
+  4: 938.93ΛΑΖ
   5: '310'
   8: ΗΠ.ΕΣΤΙΑ
   9: ΓΙΑΝΝΙΝΑ
   10: '1980'
   11: 63Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΚΟΥΚΟΥΛΙΑ
   14: ΚΟΥΚΟΥΛΙΑ-ΖΑΓΟΡΙ
   15: ΖΑΓΟΡΙ-ΚΟΥΚΟΥΛΙΑ
 - 0: 1240
   1: ΣΑΛΑΜΑΓΚΑΣ,Δ
   2: ΕΛΕΝΗ ΑΓΓΕΛΙΝΑ ΔΟΥΚΑΙΝΑ
   3: Η ΤΡΑΓΙΚΗ ΜΟΡΦΗ ΜΙΑΣ ΗΠΕΙΡΩΤΟΠΟΥΛΑΣ ΠΡΙΓΚΗΠΕΣΣΑΣ
-  4: 938.4 ΣΑΛ
+  4: 938.4ΣΑΛ
   5: '2800'
   8: Χ.Ε
   9: ΓΙΑΝΝΙΝΑ
   10: '1961'
   11: 13Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΠΡΩΣΟΠΑ
   14: ΔΟΥΚΑΙΝΑ-ΠΡΙΓΚΗΠΕΣΣΑ
   15: ΠΡΙΓΚΗΠΙΣΣΑ ΔΟΥΚΑΙΝΑ
 - 0: 1241
   1: ΣΟΥΡΑΣ,ΑΘΑΝΑΣΙΟΣ
   2: ΟΙ ΔΙΟΙΚΗΣΑΝΤΕΣ ΤΑ ΤΗΣ ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΚΑΤΑ ΤΗΝ ΑΠΟ ΤΗΣ
   3: ΑΝΑΣΥΣΤΑΣΕΩΣ ΤΗΣ ΤΕΣΣΑΡΑΚΟΝΤΑΕΤΗ ΠΕΡΙΟΔΟΝ 1934-1974
-  4: 938.93 ΣΟΥ
+  4: 938.93ΣΟΥ
   5: '2782'
   8: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
   9: ΑΘΗΝΑ
   10: '1977'
   11: 13Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
   14: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ;3
 - 0: 1242
   1: ΤΟΥΝΓΚ,ΜΑΟ ΤΣΕ
   2: ΤΟ ΚΟΚΚΙΝΟ ΒΙΒΛΙΟ
-  4: 952 ΤΟΥ
+  4: 952ΤΟΥ
   5: '2576'
   8: ΓΕΡΟΝΤΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 227Σ
   12: ΙΑΠΩΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΕΚΙΝΟ
   13: ΠΕΚΙΝΟ-ΙΣΤΟΡΙΑ
@@ -16080,15 +16076,15 @@
   11: 42Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
   13: ΘΡΑΚΗ-ΠΝΕΥΜΑΤΙΚΟΙ ΑΝΤΡΕΣ
   14: ΠΝΕΥΜΑΤΙΚΟΙ ΑΝΤΡΕΣ-ΘΡΑΚΗ
 - 0: 1244
   1: ΤΟΥΡΛΙΔΟΣ,ΓΕΩΡΓΙΟΣ ΑΘ
   2: Η ΘΡΑΚΗ ΕΝ ΤΗ ΠΟΙΗΣΕΙ ΤΟΥ ΕΝΝΙΟΥ
-  4: 880.1 ΤΟΥ
+  4: 880.1ΤΟΥ
   5: '2696'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 6Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΘΡΑΚΗ
@@ -16104,15 +16100,15 @@
   10: '1976'
   11: 123Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΕΛΛΗΝΙΣΜΟΣ
 - 0: 1246
   1: ΤΟΥΡΛΙΔΟΣ,ΓΕΩΡΓΙΟΣ ΑΘ
   2: Η ΕΠΕΚΤΑΤΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΡΩΜΗΣ ΚΑΙ Ο ΟΡΑΤΙΟΣ
-  4: 938.19 ΤΟΥ
+  4: 938.19ΤΟΥ
   5: '2513'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1976'
   11: 95Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ
   13: ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ-ΟΡΑΤΙΟΣ
@@ -16144,27 +16140,27 @@
   13: ΗΠΕΙΡΟΣ-ΔΩΔΩΝΗ
   14: ΔΩΔΩΝΗ-ΜΑΝΤΕΙΟ
   15: ΜΑΝΤΕΙΟ-ΔΩΔΩΝΗ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ;43
 - 0: 1249
   1: ΔΕΛΑΠΟΡΤΑΣ,ΠΑΥΛΟΣ Γ.
   2: ΜΝΗΜΗ ΓΕΩΡΓΙΟΥ ΓΚΑΛΚΟΥ
-  4: 938.7 ΔΕΛ
+  4: 938.7ΔΕΛ
   5: 2796-3695
   8: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
   9: ΑΘΗΝΑ
   10: '1977'
   11: 38Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΓΚΑΛΚΟΣ
   14: ΓΚΑΛΚΟΣ-ΗΠΕΙΡΟΣ
 - 0: 1250
   1: ΒΙΤΤΗΣ,ΦΩΤΗΣ Σ.
   2: ΙΣΤΟΡΙΚΑ ΠΑΡΑΔΟΣΙΑΚΑ ΠΑΡΑΘΕΜΑΤΑ
-  4: 938.4 ΒΙΤ
+  4: 938.4ΒΙΤ
   5: '2766'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1984'
   11: 8Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΡΑΔΟΣΗ
   13: ΠΑΡΑΔΟΣΗ-1821
@@ -16182,15 +16178,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΩΣΟΠΑ
   13: ΚΛΟΝΑΡΗΣ-ΑΡΕΙΟΣ ΠΑΓΟΣ
   14: ΑΡΕΙΟΣ ΠΑΓΟΣ-ΚΛΟΝΑΡΗΣ
 - 0: 1252
   1: ΤΣΟΥΚΑΝΕΛΗΣ,ΑΛΕΞΑΝΔΡΟΣ Σ
   2: ΧΑΡΑΛΑΜΠΟΣ ΚΑΤΣΙΜΗΤΡΟΣ
   3: ΠΡΟΜΑΧΟΣ ΤΗΣ ΗΠΕΙΡΟΥ
-  4: 938.7 ΤΣΟ
+  4: 938.7ΤΣΟ
   5: 2765-9282
   8: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
   9: ΑΘΗΝΑ
   10: '1978'
   11: 93Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΚΑΤΣΙΜΗΤΡΟΣ
@@ -16217,17 +16213,17 @@
   9: ΑΘΗΝΑ
   10: '1984'
   11: 94Σ
   12: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   14: ΑΡΧΕΙΟ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
 - 0: 1255
-  1: ΤΡΙΚΟΥΠΗΣ,ΧΑΡΙΛΑΟΣ
+  1: Χ.Σ
   2: ΠΕΡΙ ΧΑΡΙΛΑΟΥ ΤΡΙΚΟΥΠΗ
-  4: 938.647ΤΡΙ
+  4: 938.647Χ.Σ
   5: 1938-1937-1936-1935-
   6: 1933-1870-1869-1866-
   7: '1932'
   8: ΣΑΚΕΛΛΑΡΙΟΥ
   9: ΑΘΗΝΑ
   10: '1907'
   11: 1064Σ
@@ -16247,15 +16243,15 @@
   11: 374Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΚΡΥΣΤΑΛΛΗΣ-ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ
   14: ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ-ΚΡΥΣΤΑΛΛΗΣ
 - 0: 1257
   1: ΤΡΟΥΣΛΟ,ΑΝΤΑΜΣ
   2: Η ΕΠΟΠΟΙΙΑ ΤΗΣ ΑΜΕΡΙΚΗΣ
-  4: 970 TRU
+  4: 970TRU
   5: '433'
   8: ΑΕΤΟΣ
   9: ΑΘΗΝΑ
   10: '1952'
   11: 244Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΟΠΟΙΙΑ
   13: ΑΜΕΡΙΚΗ-ΕΠΟΠΟΙΙΑ
@@ -16287,15 +16283,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1944
   13: 1944-Η ΜΑΧΗ ΤΩΝ ΑΘΗΝΩΝ
   14: Η ΜΑΧΗ ΤΩΝ ΑΘΗΝΩΝ-1944
   15: ΑΘΗΝΑ-1944
 - 0: 1260
   1: ΤΣΑΚΩΝΑΣ,ΔΗΜ Γ.
   2: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΟΝ ΝΕΟΝ ΕΛΛΗΝΙΣΜΟΝ
-  4: 938.7 ΤΣΑ
+  4: 938.7ΤΣΑ
   5: '1903'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1958'
   11: 191Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ
@@ -16312,15 +16308,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΣΙΚΕΛΙΑΝΟΣ
   15: ΣΙΚΕΛΙΑΝΟΣ
 - 0: 1262
   1: ΤΣΑΠΑΛΗΣ,ΛΑΜΠΡΟΣ
   2: ΣΥΝΤΟΜΗ ΙΣΤΟΡΙΑ ΗΠΕΙΡΟΥ
-  4: 938.21 ΤΣΑ
+  4: 938.21ΤΣΑ
   5: '2265'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1988'
   11: 15Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
@@ -16337,15 +16333,15 @@
   12: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΥΤΟΒΙΟΓΡΑΦΙΑ
   13: ΑΥΤΟΒΙΟΓΡΑΦΙΑ-ΤΣΑΠΛΙΝ
   14: ΤΣΑΠΛΙΝ-ΑΥΤΟΒΙΟΓΡΑΦΙΑ
   15: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΤΣΑΠΛΙΝ
 - 0: 1264
   1: ΤΣΑΡΜΑΚΗΣ,ΑΘΑΝΑΣΙΟΣ Γ.
   2: ΛΑΜΙΑ-ΤΕΠΕΛΕΝΙ 1940
-  4: 938.75 ΤΣΑ
+  4: 938.75ΤΣΑ
   5: '2019'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1981'
   11: 87Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΛΑΜΙΑ
   13: ΛΑΜΙΑ-1940
@@ -16361,27 +16357,27 @@
   10: Χ.Χ
   11: 31Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
   13: ΚΑΠΟΔΙΣΤΡΙΑΣ
 - 0: 1266
   1: ΤΣΑΤΣΟΣ,ΚΩΝ/ΝΟΣ
   2: ΑΙΣΘΗΤΙΚΑ ΔΟΚΙΜΙΑ
-  4: 880.4 ΤΣΑ
+  4: 880.4ΤΣΑ
   5: '1229'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1961'
   11: 214Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΟΚΙΜΙΑ
   13: ΔΟΚΙΜΙΑ-ΑΙΣΘΗΤΙΚΑ
   14: ΑΙΣΘΗΤΙΚΑ ΔΟΚΙΜΙΑ
 - 0: 1267
   1: ΤΣΑΤΣΟΣ,ΚΩΝ/ΝΟΣ
   2: ΑΙΣΘΗΤΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
-  4: 880.4 ΤΣΑ
+  4: 880.4ΤΣΑ
   5: '1230'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 283Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΕΛΕΤΗΜΑΤΑ
   13: ΜΕΛΕΤΗΜΑΤΑ-ΑΙΣΘΗΤΙΚΑ
@@ -16474,40 +16470,40 @@
   11: 411Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΑΜΝΗΣΕΙΣ
   13: ΗΠΕΙΡΟΣ-ΑΓΩΝΙΣΤΗΣ
   14: ΑΓΩΝΙΣΤΗΣ-ΗΠΕΙΡΟΣ
 - 0: 1275
   1: ΤΣΕΧΩΦ,ΑΝΤΟΝ
   2: Ο ΓΛΑΡΟΣ-ΘΕΙΟΣ ΒΑΝΙΑΣ-ΠΡΟΤΑΣΗ ΓΑΜΟΥ-Η ΑΡΚΟΥΔΑ
-  4: 891.7 ΤΣΕ
+  4: 891.7ΤΣΕ
   5: 1563-1562-
   6: ΚΑΛΕΡΓΗΣ,ΛΥΚΟΥΡΓΟΣ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: '1986'
   11: 230Σ
   12: ΡΩΣΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΡΩΣΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΑ
   14: ΘΕΑΤΡΙΚΑ ΕΡΓΑ-ΡΩΣΙΑ
 - 0: 1276
   1: ΤΣΙΑΤΗΣ,ΒΑΣΙΛΗΣ Ε
   2: ΣΚΑΝΔΙΝΑΒΙΚΗ ΑΝΑΠΟΛΗΣΗ
-  4: 914.48 ΤΣΙ
+  4: 914.48ΤΣΙ
   5: '403'
   8: Χ.Ε
   9: ΠΕΙΡΑΙΑ
   10: '1985'
   11: 154Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΣΚΑΝΔΙΝΑΒΙΑ
   13: ΤΑΞΙΔΙΑ-ΣΚΑΝΔΙΝΑΒΙΑ
   14: ΣΚΑΝΔΙΝΑΒΙΑ-ΤΑΞΙΔΙΑ
 - 0: 1277
   1: ΤΣΙΑΤΗΣ,ΒΑΣΙΛΗΣ
   2: ΗΛΙΟΛΟΥΣΤΗ ΚΑΙ ΘΑΛΑΣΣΟΦΙΛΗΤΗ ΧΩΡΑ
-  4: 889.21 ΤΣΙ
+  4: 889.21ΤΣΙ
   5: '377'
   8: Χ.Ε
   9: ΠΕΙΡΑΙΑ
   10: '1981'
   11: 170Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΥΠΡΟΣ
   13: ΤΑΞΙΔΙΑ-ΚΥΠΡΟΣ
@@ -16523,15 +16519,15 @@
   11: 128Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΑΡΤΑ
   14: ΑΡΤΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
 - 0: 1279
   1: ΤΣΙΜΑΝΗΣ,ΠΡΟΚΟΠΙΟΣ
   2: ΟΙ ΠΑΤΡΙΑΡΧΑΙ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ
-  4: 938.4 ΤΣΙ
+  4: 938.4ΤΣΙ
   5: 1811-1812-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1981'
   11: 384Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
   13: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΠΑΤΡΙΑΡΧΕΣ
@@ -16561,50 +16557,50 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΚΑΒΑΦΗΣ
   15: ΚΑΒΑΦΗΣ
 - 0: 1282
   1: ΤΣΙΡΟΠΟΥΛΟΣ,ΚΩΣΤΑΣ Ε.
   2: ΑΜΕΡΙΚΑΝΙΚΗ ΑΝΘΡΩΠΟΓΕΩΓΡΑΦΙΑ
-  4: 917 ΤΣΙ
+  4: 917ΤΣΙ
   5: 429-430
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1976'
   11: 153Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΑΜΕΡΙΚΗ
   13: ΑΜΕΡΙΚΗ-ΑΝΘΡΩΠΟΓΕΩΓΡΑΦΙΑ
   14: ΑΝΘΡΩΠΟΓΕΩΓΡΑΦΙΑ-ΑΜΕΡΙΚΗ
 - 0: 1283
   1: ΤΣΙΡΠΑΝΛΗΣ,ΖΑΧ Ν.
   2: Η ΔΥΤΙΚΗ ΕΥΡΩΠΗ ΣΤΟΥΣ ΜΕΣΟΥΣ ΧΡΟΝΟΥΣ(5-15ΑΙ)
-  4: 940.1 ΤΣΙ
+  4: 940.1ΤΣΙ
   5: '2496'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1973'
   11: 289Σ
   12: ΕΥΡΩΠΑΙΚΗ ΙΣΤΟΡΙΑ-(5-15ΑΙ)
   13: ΕΥΡΩΠΗ-ΙΣΤΟΡΙΑ
 - 0: 1284
   1: ΤΣΙΤΣΑΣ,ΣΕΡΑΦΕΙΜ Κ.
   2: Ο ΤΡΑΓΟΥΔΙΣΤΗΣ ΤΟΥ ΒΟΥΝΟΥ ΚΑΙ ΤΟΥ ΔΑΣΟΥΣ
-  4: 782.42 ΤΣΙ
+  4: 782.42ΤΣΙ
   5: '715'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1980'
   11: 63Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
   14: ΤΡΑΓΟΥΔΙΑ-ΒΟΥΝΟ
 - 0: 1285
   1: ΤΣΙΤΣΑΣ,ΣΕΡΑΦΕΙΜ Κ.
   2: Τ'ΑΓΡΑΦΑ ΤΗΣ ΠΙΝΔΟΥ
-  4: 938.93 ΤΣΙ
+  4: 938.93ΤΣΙ
   5: '314'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 95Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΡΑΦΑ
   13: ΑΓΡΑΦΑ-ΙΣΤΟΡΙΑ
@@ -16620,15 +16616,15 @@
   11: 272Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΡΙΚΟΥΠΗΣ
   13: ΤΡΙΚΟΥΠΗΣ-ΒΙΟΓΡΑΦΙΑ
   14: ΒΙΟΓΡΑΦΙΑ-ΤΡΙΚΟΥΠΗΣ
 - 0: 1287
   1: ΤΣΟΚΟΠΟΥΛΟΣ,Γ.Β
   2: ΓΥΝΑΙΚΕΣ ΤΟΥ ΒΥΖΑΝΤΙΟΥ
-  4: 938.3 ΤΣΟ
+  4: 938.3ΤΣΟ
   5: '1983'
   8: ΣΙΔΕΡΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 162Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΓΥΝΑΙΚΕΣ
@@ -16644,15 +16640,15 @@
   11: 844Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΙΑ
   13: ΑΙΤΩΛΙΑ-ΔΕΡΒΕΚΙΣΤΑ
   14: ΔΕΡΒΕΚΙΣΤΑ-ΑΙΤΩΛΙΑ
 - 0: 1289
   1: ΤΣΟΝΙΔΗΣ,ΤΑΚΗΣ ΧΡ.
   2: ΤΟ ΓΕΝΟΣ ΚΑΡΑΘΕΟΔΩΡΗ 1740-1950
-  4: 938.4 ΤΣΟ
+  4: 938.4ΤΣΟ
   5: 2447-2446
   8: Χ.Ε
   9: Ν.ΟΡΕΣΤΙΑ
   10: '1989'
   11: 352Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΚΑΡΑΘΕΟΔΩΡΗ-(1740-1950)
@@ -16668,27 +16664,27 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΓΗ
   14: ΓΗ-ΓΕΩΡΓΟΙ
   15: ΓΕΩΡΓΟΙ-ΤΟΥΡΚΟΚΡΑΤΙΑ
 - 0: 1291
   1: ΤΣΟΥΤΣΙΝΟΣ,ΓΙΑΝΝΗΣ
   2: ΠΕΝΤΕ ΑΡΤΙΝΑ ΜΕΛΕΤΗΜΑΤΑ
-  4: 938.21 ΤΣΟ
+  4: 938.21ΤΣΟ
   5: 2481-2482
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1982'
   11: 38Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΜΕΛΕΤΗΜΑΤΑ
   14: ΜΕΛΕΤΗΜΑΤΑ-ΑΡΤΑ
 - 0: 1292
   1: ΤΣΟΥΤΣΙΝΟΣ,ΓΙΑΝΝΗΣ
   2: Ο ΕΝΤΙΜΟΣ ΘΑΝΑΤΟΣ ΤΗΣ ΑΜΒΡΑΚΙΑΣ
-  4: 938.21 ΤΣΟ
+  4: 938.21ΤΣΟ
   5: 2216-13251
   8: Χ.Ε
   9: ΓΙΑΝΝΙΝΑ
   10: '1967'
   11: 35Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΜΒΡΑΚΙΑ
   13: ΑΜΒΡΑΚΙΑ
@@ -16703,15 +16699,15 @@
   11: 11Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΤΟΠΩΝΥΜΙΟ
   14: ΤΟΠΩΝΥΜΙΟ-ΑΡΤΑ
 - 0: 1294
   1: ΤΩΜΑΔΑΚΗΣ,Ν.Β
   2: ΕΟΡΤΑΣΤΙΚΟΙ ΛΟΓΟΙ
-  4: 889.21 ΤΩΜ
+  4: 889.21ΤΩΜ
   5: '2529'
   8: ΓΡΗΓΟΡΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 116Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΟΡΤΑΣΤΙΚΟΙ ΛΟΓΟΙ
   13: ΕΟΡΤΑΣΤΙΚΟΙ ΛΟΓΟΙ
@@ -16727,15 +16723,15 @@
   11: 205Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ
   13: ΒΕΝΙΖΕΛΟΣ
 - 0: 1296
   1: ΤΩΜΑΔΑΚΗΣ,ΝΙΚΟΛΑΟΣ Β.
   2: ΑΠΑΝΘΙΣΜΑΤΑ
   3: ΓΡΑΜΜΑΤΟΛΟΓΙΚΑΙ ΚΑΙ ΒΙΟΓΡΑΦΙΚΑ ΤΗΣ ΝΕΑΣ ΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑ
-  4: 886.2 ΤΩΜ
+  4: 886.2ΤΩΜ
   5: '2642'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 294Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΕΛΕΤΕΣ
   13: ΜΕΛΕΤΕΣ-ΛΟΓΟΤΕΧΝΙΑ
@@ -16764,26 +16760,26 @@
   11: 285Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΡΥΓΙΑΝΝΗΣ
   13: ΜΑΚΡΥΓΙΑΝΝΗΣ-ΚΡΟΚΥΛΙΟ
   14: ΚΡΟΚΥΛΙΟ-ΜΑΚΡΥΓΙΑΝΝΗΣ
 - 0: 1299
   1: ΦΑΚΟΥ,ΠΑΝΤΕΛΗΣ Π.
   2: ΓΝΩΡΙΣΤΕ ΤΟ ΞΗΡΟΜΕΡΟ
-  4: 398 ΦΑΚ
+  4: 938.917ΦΑΚ
   5: '320'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 176Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΞΗΡΟΜΕΡΟ
   13: ΞΗΡΟΜΕΡΟ
 - 0: 1300
   1: ΦΑΝΑΡΙΩΤΟΥ-ΦΙΛΙΠΠΟΥ,ΑΘΗΝΑ Δ
   2: ΛΥΡΙΚΑ ΤΡΑΓΟΥΔΙΑ
-  4: 880.14 ΦΑΝ
+  4: 880.14ΦΑΝ
   5: 745-746
   8: Χ.Ε
   9: ΝΕΑ ΥΟΡΚΗ
   10: Χ.Χ
   11: 40Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΤΡΑΓΟΥΔΙΑ
@@ -16801,27 +16797,27 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΒΙΒΛΙΟ
   13: ΒΙΒΛΙΟ-ΕΙΚΟΝΟΓΡΑΦΗΜΕΝΟ
   14: ΕΙΚΟΝΟΓΡΑΦΗΜΕΝΟ ΒΙΒΛΙΟ
 - 0: 1302
   1: ΦΕΡΕΝΤΙΝΟΣ,ΓΕΩΡΓΙΟΣ Α.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΚΑΡΝΑΝΙΑΣ ΑΠΟ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ
   3: ΤΗΣ ΕΠΟΧΗΣ ΤΟΥ ΧΡΙΣΤΟΥ
-  4: 938.22 ΦΕΡ
+  4: 938.22ΦΕΡ
   5: 1720-1719-
   8: ΠΑΠΑΖΗΣΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 319Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΚΑΡΝΑΝΙΑ
   13: ΑΚΑΡΝΑΝΙΑ
   14: ΑΙΤΩΛΟΚΑΡΝΑΝΙΑ
 - 0: 1303
   1: ΦΕΡΤΑΚΗΣ,ΒΑΣΙΛΕΙΟΣ ΕΥΘ
   2: Η ΕΝ ΕΛΛΑΔΙ ΜΕΤΑΠΟΛΙΤΕΥΣΙΣ
-  4: 938.8 ΦΕΡ
+  4: 938.8ΦΕΡ
   5: '2486'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1976'
   11: 154Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΤΑΠΟΛΙΤΕΥΣΗ
   13: ΜΕΤΑΠΟΛΙΤΕΥΣΗ-ΕΛΛΑΔΑ
@@ -16850,15 +16846,15 @@
   11: 399Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
   13: ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ-ΔΟΚΙΜΙΟ
   14: ΔΟΚΙΜΙΟ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
 - 0: 1306
   1: ΦΙΛΙΠΠΟΥ,ΕΝΤΟΥΑΡΝΤΟ ΝΤΕ
   2: ΦΙΛΟΥΜΕΝΑ ΜΑΡΤΟΥΡΑΝΟ
-  4: 852 ΦΙΛ
+  4: 852ΦΙΛ
   5: '1561'
   6: ΜΠΟΥΜΗ,ΡΙΤΑ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 106Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -16887,123 +16883,123 @@
   11: 143Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΑΓΩΝΙΣΤΕΣ
   14: ΑΓΩΝΙΣΤΕΣ-ΚΥΠΡΟΣ
 - 0: 1309
   1: ΦΙΣΕΡ,ΕΡΒΕΡΤΟΥ
   2: ΝΑΠΟΛΕΩΝ
-  4: 944 ΦΙΣ
+  4: 944ΦΙΣ
   5: '1267'
   6: ΣΤΑΥΡΙΝΙΔΟΣ,Δ.Θ.
   8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '1930'
   11: 173Σ
   12: ΓΑΛΛΙΚΗ ΙΣΤΟΡΙΑ-ΝΑΠΟΛΕΩΝ
   13: ΝΑΠΟΛΕΩΝ-ΙΣΤΟΡΙΑ
   14: ΓΑΛΛΙΑ-ΝΑΠΟΛΕΩΝ
 - 0: 1310
   1: ΦΛΑΜΙΝΙ,ΚΡΕΜΙΕ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΙΤΑΛΙΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
-  4: 850 ΦΛΑ
+  4: 850ΦΛΑ
   5: '202'
   6: ΣΕΡΟΥΙΟΥ,Γ
   8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '1930'
   11: 239Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΑ
 - 0: 1311
   1: FLEMING,G.DAVID
   2: JOHN CAPODISTRIAS AND THE CONFERERCE OF LONDON(1828-1831)
-  4: 938.57 FLE
+  4: 938.57FLE
   5: '1771'
   8: X.E
   9: THE/NIKI
   10: '1970'
   11: 398S
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
   13: ΚΑΠΟΔΙΣΤΡΙΑΣ-(1828-1831)
 - 0: 1312
   1: ΦΛΟΥΔΑΣ,ΝΙΚΟΛΑΟΣ Ι
   2: ΒΥΖΙΚΙΩΤΙΚΑ
-  4: 398 ΦΛΟ
+  4: 398ΦΛΟ
   5: '333'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1960'
   11: 144Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΙΚΙΩΤΙΚΑ
   13: ΒΥΖΙΚΙΩΤΙΚΑ
 - 0: 1313
   1: ΦΛΩΡΟΣ,ΠΑΥΛΟΣ
   2: ΕΛΛΗΝΙΚΟΙ ΔΡΟΜΟΙ
   3: ΤΑΞΙΔΙΑ
-  4: 914.95 ΦΛΩ
+  4: 914.95ΦΛΩ
   5: '2579'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 284Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
   13: ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
   14: ΕΛΛΑΔΑ-ΤΑΞΙΔΙΑ
   15: ΓΕΩΓΡΑΦΙΑ-ΕΛΛΑΔΑ
 - 0: 1314
   1: ΦΛΩΡΟΣ,ΠΑΥΛΟΣ
   2: ΣΤΑΥΡΟΔΡΟΜΙΑ ΤΗΣ ΕΥΡΩΠΗΣ
-  4: 914.4 ΦΛΩ
+  4: 914.4ΦΛΩ
   5: '394'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1964'
   11: 216Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
   13: ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
   14: ΕΥΡΩΠΗ-ΤΑΞΙΔΙΑ
 - 0: 1315
   1: ΦΟΝΤΟΝ,ΧΟΥΑΝ
   2: Η ΧΙΛΗ ΘΑ ΝΙΚΗΣΗ
-  4: 819.7 ΦΟΝ
+  4: 819.7ΦΟΝ
   5: '1377'
   6: ΜΠΑΟΥΔΑΚΗ,ΕΛΠΙΔΑ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 75Σ
   12: ΧΙΛΙΑΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΧΙΛΙΑΝΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΧΙΛΗ
 - 0: 1316
   1: ΦΟΥΡΙΩΤΗΣ,ΑΓΓΕΛΟΣ
   2: ΤΟ ΜΥΘΙΣΤΟΡΗΜΑ
-  4: 880.3 ΦΟΥ
+  4: 880.3ΦΟΥ
   5: '222'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1959'
   11: 368Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΕΛΛΗΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
 - 0: 1317
   1: FOSS,ARTHUR
   2: EPIRUS
-  4: 938.21 FOS
+  4: 938.21FOS
   5: 2181-2274
   8: FADER
   9: LONDON
   10: '1978'
   11: 223S
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
 - 0: 1318
   1: ΦΟΥΛΜΡΙΤΖ,ΤΖ
   2: Η ΑΛΑΖΟΝΕΙΑ ΤΗΣ ΔΥΝΑΜΕΩΣ
-  4: 970 ΦΟΥ
+  4: 970ΦΟΥ
   5: '2629'
   6: ΠΑΠΑΜΑΡΓΑΡΗ,Θ
   8: ΠΑΠΑΖΗΣΗ
   9: ΑΘΗΝΑ
   10: '1970'
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΥΝΑΜΕΙΣ
   13: ΑΜΕΡΙΚΗ-ΠΡΟΒΛΗΜΑΤΑ
@@ -17021,41 +17017,41 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
   13: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ-ΟΠΛΑΡΧΗΓΟΥ
   14: ΦΟΥΦΑΣ-ΟΠΛΑΡΧΗΓΟΣ
   15: ΜΑΚΕΔΟΝΙΑ-ΟΠΛΑΡΧΗΓΟΣ
 - 0: 1320
   1: ΦΡΑΓΚΟΠΟΥΛΟΣ,Θ.Δ
   2: ΚΑΡΤΕΡΙΑ
-  4: 886.2 ΦΡΑ
+  4: 886.2ΦΡΑ
   5: '1497'
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1957'
   11: 118Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
 - 0: 1321
   1: ΦΡΑΓΚΟΠΟΥΛΟΣ,Θ.Δ
   2: ΚΑΠΟΔΙΣΤΡΙΑΣ
   3: ΘΕΑΤΡΟ
-  4: 886.2 ΦΡΑ
+  4: 886.2ΦΡΑ
   5: '1498'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1959'
   11: 50Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
 - 0: 1322
   1: ΦΡΑΓΚΟΥ,ΚΩΝ/ΝΟΣ
   2: Η 21 ΦΕΒΡΟΥΑΡΙΟΥ 1913 ΩΣ ΜΙΑ ΤΩΝ ΕΚΒΟΛΩΝ ΤΗΣ ΑΓΩΓΗΣ ΚΑΙ
   3: ΤΟΥΗΘΟΥΣ ΤΩΝ ΠΡΟ ΑΥΤΗΣ ΕΛΛΗΝΙΚΩΝ ΓΕΝΕΩΝ
-  4: 938.68 ΦΡΑ
+  4: 938.68ΦΡΑ
   5: '2104'
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1967'
   11: 14Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1913
   13: 1913-21 ΦΕΒΡΟΥΑΡΙΟΥ
@@ -17072,52 +17068,52 @@
   11: 324Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΦΡΕΙΔΕΡΙΚΗ
   13: ΦΡΕΙΔΕΡΙΚΗ-ΒΑΣΙΛΙΣΣΑ
   14: ΒΑΣΙΛΙΣΣΑ-ΦΡΕΙΔΕΡΙΚΗ
 - 0: 1324
   1: ΦΤΕΡΗΣ,Γ
   2: ΜΑΝΗ ΠΑΤΡΙΔΑ ΜΟΥ
-  4: 938.92 ΦΤΕ
+  4: 938.92ΦΤΕ
   5: '324'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1976'
   11: 178Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΝΗ
   13: ΜΑΝΗ-ΙΣΤΟΡΙΑ
 - 0: 1325
   1: ΦΤΕΡΗΣ,ΓΕΩΡΓΙΟΣ
   2: ΕΛΛΗΝΙΚΕΣ ΜΟΡΦΕΣ
-  4: 880.3 ΦΤΕ
+  4: 880.3ΦΤΕ
   5: '2652'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1979'
   11: 236Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΕΛΛΗΝΕΣ
   14: ΛΟΓΟΤΕΧΝΕΣ-ΕΛΛΗΝΕΣ
 - 0: 1326
   1: ΦΩΤΙΑΔΟΥ,ΑΘΑΝΑΣΙΟΣ(ΛΟΓΙΟΣ)
   2: ΚΑΡΑΓΚΙΟΖΗΣ Ο ΠΡΟΣΦΥΓΑΣ
   3: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ ΣΚΙΩΝ
-  4: 886.2 ΦΩΤ
+  4: 886.2ΦΩΤ
   5: '1535'
   8: GYTENBERG
   9: ΑΘΗΝΑ
   10: '1977'
   11: 522Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΑΡΑΓΚΙΟΖΗΣ
   14: ΚΑΡΑΓΚΙΟΖΗΣ-ΘΕΑΤΡΟ ΣΚΙΩΝ
   15: ΘΕΑΤΡΙΟ ΣΚΙΩΝ-ΚΑΡΑΓΚΙΟΖΗΣ
 - 0: 1327
   1: ΦΩΤΙΑΔΟΥ,Φ.Δ
   2: ΠΑΡΙΣΙΟΙ
-  4: 914.44 ΦΩΤ
+  4: 914.44ΦΩΤ
   5: '402'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 147Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΠΑΡΙΣΙ
   13: ΤΑΞΙΔΙΑ-ΠΑΡΙΣΙ
@@ -17133,29 +17129,29 @@
   11: 31Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΡΟΥΜΑΝΙΑ
   13: ΤΑΞΙΔΙΑ-ΡΟΥΜΑΝΙΑ
   14: ΡΟΥΜΑΝΙΑ-ΤΑΞΙΔΙΑ
 - 0: 1329
   1: ΦΩΤΙΑΔΟΥ,ΕΡΜΗΝΕΙΑ
   2: ΞΕΝΟΙ ΤΟΠΟΙ
-  4: 910 ΦΩΤ
+  4: 910ΦΩΤ
   5: '2603'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1972'
   11: 99Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΞΕΝΟΙ ΤΟΠΟΙ
   13: ΙΣΠΑΝΙΑ-ΤΑΞΙΔΙΑ
   14: ΓΑΛΛΙΑ-ΤΑΞΙΔΙΑ
   15: ΕΛΒΕΤΙΑ-ΤΑΞΙΔΙΑ
 - 0: 1330
   1: ΦΩΤΙΑΔΗΣ,ΕΥΑΓΓΕΛΟΣ Π.
   2: ΣΠΥΡΙΔΩΝ ΛΑΜΠΡΟΣ
   3: ΜΝΗΜΟΣΥΝΟΣ ΛΟΓΟΣ
-  4: 938 ΦΩΤ
+  4: 938ΦΩΤ
   5: 2023-2733-9254Α
   7: 2ΕΚΔ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 35Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
@@ -17172,27 +17168,27 @@
   10: '1966'
   11: 505Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ
   13: ΚΑΡΑΙΣΚΑΚΗΣ
 - 0: 1332
   1: ΦΩΤΟΠΟΥΛΟΣ,Κ.Ι
   2: ΧΡΟΝΙΚΟ ΤΟΥ ΜΕΓΑΛΟΥ ΣΗΚΩΜΟΥ ΤΟΥ ΓΕΝΟΥΣ
-  4: 938.5 ΦΩΤ
+  4: 938.5ΦΩΤ
   5: '2142'
   8: Χ.Ε
   9: ΓΙΑΝΝΙΝΑ
   10: Χ.Χ
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΧΡΟΝΙΚΟ
   13: ΧΡΟΝΙΚΟ-ΞΕΣΗΚΩΜΟΣ
   14: ΞΕΣΗΚΟΜΩΣ ΤΟΥ ΓΕΝΟΥΣ
 - 0: 1333
   1: ΦΩΤΟΠΟΥΛΟΣ,ΑΘΑΝΑΣΙΟΣ Θ.
   2: ΙΣΤΟΡΙΚΑ ΤΩΝ ΠΕΤΙΜΕΖΑΙΩΝ
-  4: 938.5 ΦΩΤ
+  4: 938.5ΦΩΤ
   5: '2128'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1982'
   11: 105Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΕΤΙΜΕΖΑΙΟΙ
   13: ΠΕΤΙΜΕΖΑΙΟΙ
@@ -17221,15 +17217,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΟΥΦΑΣ
   13: ΣΚΟΥΦΑΣ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
   14: ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ-ΙΔΡΥΤΗΣ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 1336
   1: ΧΑΜΜΕΡ,Ι
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΟΘΩΜΑΝΙΚΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
-  4: 956.1 ΧΑΜ
+  4: 956.1ΧΑΜ
   5: 2302-2303-2304-2305-
   6: ΚΡ0ΚΙΔΑΣ,Κ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1870'
   11: 385Σ
   12: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-ΙΣΤΟΡΙΑ
@@ -17245,27 +17241,27 @@
   11: 366Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΧΙΟΣ
   13: ΧΙΟΣ-1822
   14: 1822-ΧΙΟΣ
 - 0: 1338
   1: ΧΑΜΟΝΤ,Ν
   2: ΗΠΕΙΡΟΣ
-  4: 938.21 ΧΑΜ
+  4: 938.21ΧΑΜ
   5: 2269-2270-2271-
   6: ΓΙΑΓΚΑΣ,ΑΘ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1971'
   11: 214Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
 - 0: 1339
   1: ΧΑΝΤΚΕ,ΠΕΤΕΡ
   2: ΚΑΣΠΑΡ
-  4: 832 ΧΑΝ
+  4: 832ΧΑΝ
   5: '1373'
   6: ΑΙΝΤΕΝΑΙΕΡ,ΝΙΚΗ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 111Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
@@ -17282,38 +17278,38 @@
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΠΕΖΟΓΡΑΦΟΙ
   14: ΠΕΖΟΓΡΑΦΟΙ-ΕΛΛΗΝΕΣ
 - 0: 1341
   1: ΧΑΡΗΣ,ΠΕΤΡΟΣ
   2: Η ΚΙΝΑ ΕΞΩ ΑΠΟ ΤΑ ΤΕΙΧΗ
-  4: 915.31 ΧΑΡ
+  4: 915.31ΧΑΡ
   5: 451-455-450
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1963'
   11: 246Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΙΝΑ
   13: ΤΑΞΙΔΙΑ-ΚΙΝΑ
   14: ΚΙΝΑ-ΤΑΞΙΔΙΑ
 - 0: 1342
   1: ΧΑΡΗΣ,ΠΕΤΡΟΣ
   2: Η ΠΝΕΥΜΑΤΙΚΗ ΕΛΕΥΘΕΡΙΑ ΚΑΙ ΟΙ ΜΕΤΑΠΟΛΕΜΙΚΟΙ ΑΝΘΡΩΠΟΙ
-  4: 880.4 ΧΑΡ
+  4: 880.4ΧΑΡ
   5: '1003'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 243Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΛΟΓΟΤΕΧΝΕΣ
 - 0: 1343
   1: ΧΑΤΖΗΣ,ΘΑΝΑΣΗΣ
   2: Η ΝΙΚΗΦΟΡΑ ΕΠΑΝΑΣΤΑΣΗ ΠΟΥ ΧΑΘΗΚΕ
-  4: 938.75 ΧΑΤ
+  4: 938.75ΧΑΤ
   5: 2290-2291-2292-
   8: ΠΑΠΑΖΗΣΗ
   9: ΑΘΗΝΑ
   10: '1977'
   11: 473Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
   13: 1940-ΕΠΑΝΑΣΤΑΣΗ
@@ -17342,15 +17338,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
   13: ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
   14: ΗΠΕΙΡΟΣ-ΔΕΣΠΟΤΑΤΟ
 - 0: 1346
   1: ΧΑΤΖΗΙΩΑΝΝΟΥ,ΓΙΑΝΝΗΣ
   2: ΠΕΖΟΓΡΑΦΗΜΑΤΑ (1989-1990)
   3: ΠΟΙΗΤΙΚΑ ΘΕΜΑΤΑ Β'(ΜΕΛΕΤΗΜΑ)
-  4: 880.3 ΧΑΤ
+  4: 880.3ΧΑΤ
   5: '1667'
   8: Χ.Ε
   9: ΘΕΣ/ΝΙΚΗ
   10: '1990'
   11: 137Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΠΕΖΟΓΡΑΦΗΜΑΤΑ
@@ -17430,37 +17426,39 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   14: ΠΑΠΑΔΙΑΜΑΝΤΗΣ
 - 0: 1353
   1: ΧΕΜΠΕΛ,ΦΡΕΙΔΕΡΙΚΗ
   2: ΙΟΥΔΗΘ
   3: ΤΡΑΓΩΔΙΑ
-  4: 832 ΧΕΜ
+  4: 832ΧΕΜ
   5: '1375'
   6: ΔΙΚΤΑΙΟΣ,ΑΡΗΣ
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 142Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ-ΓΕΡΜΑΝΙΑ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΓΕΡΜΑΝΙΑ
 - 0: 1354
   1: ΧΕΡΤΣΒΕΡΓ,ΓΟΥΣΤΑΒΟΥ ΦΡΕΙΔΕΡΙΚΟΥ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΑΔΟΣ ΑΠΟ ΤΗΣ ΛΗΞΕΩΣ ΤΟΥ ΑΡΧΑΙΟΥ ΒΙΟΥ ΜΕΧΡΙ
   3: ΣΗΜΕΡΟΝ
-  4: 938 ΧΕΡ
+  4: 938ΧΕΡ
   5: 1752-1753-1855-2175-
   6: ΚΑΡΟΛΙΔΟΣ,Π
   8: ΣΑΚΕΛΛΑΡΙΟΥ
   9: ΑΘΗΝΑ
   10: '1906'
   11: 634Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
+  13: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
+  14: ΙΣΤΟΡΙΑ
   17: (1752-2 ΑΝΤΙΤΥΠΑ)
 - 0: 1355
   1: ΧΙΔΙΡΟΓΛΟΥ,ΠΑΥΛΟΣ
   2: ΟΙ ΕΛΛΗΝΕΣ ΠΟΜΑΚΟΙ ΚΑΙ Η ΣΧΕΣΗ ΤΟΥΣ ΜΕ ΤΗΝ ΤΟΥΡΚΙΑ
   4: 938.699ΧΙΔ
   5: '1987'
   8: ΤΕΛΕΘΡΙΟΝ
@@ -17582,41 +17580,41 @@
   14: ΗΠΕΙΡΟΣ-ΤΑΞΙΔΙΑ
   15: ΙΟΝΙΑ ΝΗΣΙΑ-ΤΑΞΙΔΙΑ
   17: ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ ΣΤΟΝ ΕΛΛΗΝΙΚΟ ΧΩΡΟ 8
   30: HENRY HOLLAND
 - 0: 1365
   1: ΧΟΦΜΑΝ,ΦΡΕΝΤ
   2: ΤΟ ΣΥΓΧΡΟΝΟ ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ(1900-1950)
-  4: 880.3XOF
+  4: 880.ΧΟΦ
   5: '2655'
   8: ΑΕΤΟΣ
   9: ΑΘΗΝΑ
   10: '1954'
   11: 167Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΜΕΡΙΚΗ
   15: ΑΜΕΡΙΚΗ-ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 1366
   1: ΧΟΥΡΜΟΥΖΙΑΔΗΣ,Γ.Δ.
   2: ΑΝΘΟΛΟΓΙΑ ΤΟΝ ΑΡΓΕΝΤΙΝΟΥ ΔΙΗΓΗΜΑΤΟΣ
-  4: 810 ΧΟΥ
+  4: 810ΧΟΥ
   5: '2640'
   8: ΒΑΚΩΝ
   9: ΑΘΗΝΑ
   10: '1967'
   11: 175Σ
   12: ΑΡΓΕΝΤΙΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΑΡΓΕΝΤΙΝΟ ΔΙΗΓΗΜΑ-ΑΝΘΟΛΟΓΙΑ
   14: ΔΙΗΓΗΜΑ-ΑΡΓΕΝΤΙΝΗ
 - 0: 1367
   1: ΧΟΥΡΜΟΥΖΙΑΔΗΣ,Γ.Δ.
   2: EΠΟΠΤΕΙΕΣ
   3: ΒΙΩΜΑΤΑ ΚΑΙ ΔΟΚΙΜΙΑ
-  4: 880.4 ΧΟΥ
+  4: 880.4ΧΟΥ
   5: '2719'
   8: ΣΙΔΕΡΗΣ
   9: ΑΘΗΝΑ
   10: '1972'
   11: 174Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΟΚΙΜΙΑ
   13: ΔΟΚΙΜΙΑ-ΛΟΓΟΤΕΧΝΙΑ
@@ -17633,27 +17631,27 @@
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   15: ΠΑΛΑΜΑΣ
 - 0: 1369
   1: ΧΟΦΜΑΝ,ΠΩΛ
   2: ΗΝΩΜΕΝΕΣ ΠΟΛΙΤΕΙΕΣ
   3: Η ΑΕΝΑΗ ΕΠΑΝΑΣΤΑΣΙΣ
-  4: 973 ΧΟΦ
+  4: 973ΧΟΦ
   5: '435'
   8: Χ.Ε
   9: ΝΕΑ ΥΟΡΚΗ
   10: '1951'
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΝΩΜΕΝΕΣ ΠΟΛΙΤΕΙΕΣ
   13: ΗΝΩΜΕΝΕΣ ΠΟΛΙΤΕΙΕΣ-ΙΣΤΟΡΙΑ
   14: ΑΕΝΑΗ-ΕΠΑΝΑΣΤΑΣΗ
 - 0: 1370
   1: ΧΟΧΟΥΤ,ΡΟΛΦ
   2: ΣΤΡΑΤΙΩΤΕΣ
   3: ΤΡΑΓΩΔΙΑ
-  4: 832 ΧΟΧ
+  4: 832ΧΟΧ
   5: '1367'
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 222Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΕΡΜΑΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
@@ -17685,27 +17683,27 @@
   13: ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΕΝΩΣΗ-1944
   14: 1944-ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΕΝΩΣΗ
   15: ΑΛΒΑΝΙΑ-ΕΛΛΗΝΙΑΛΒΑΝΙΚΗ ΕΝΩΣΗ
 - 0: 1373
   1: ΨΑΘΑΣ,ΔΗΜΗΤΡΙΟΣ
   2: Ο ΦΟΝ ΔΗΜΗΤΡΑΚΗΣ
   3: ΚΩΜΩΔΙΑ
-  4: 880.2 ΨΑΘ
+  4: 880.2ΨΑΘ
   5: '1399'
   8: ΜΑΡΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 111Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΚΩΜΩΔΙΑ
 - 0: 1374
   1: ΨΑΘΑΣ,Δ
   2: ΤΟ ΣΤΡΑΒΟΞΥΛΟ
-  4: 886.2 ΨΑΘ
+  4: 886.2ΨΑΘ
   5: '1574'
   8: ΜΑΡΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 132Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
@@ -17723,15 +17721,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΨΥΧΑΡΗΣ
   14: ΨΥΧΑΡΗΣ
 - 0: 1376
   1: ΓΟΥΕΛ,ΤΖΟΝ
   2: ΡΟΣΑΜΠΩ ΚΑΙ Ο ΠΟΛΕΜΟΣ ΤΗΣ ΒΟΡΕΙΟΑΜΕΡΙΚΑΝΙΚΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ
   3: 1725-1807
-  4: 970 ΓΟΥ
+  4: 970ΓΟΥ
   5: '2523'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1936'
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΕΞΑΡΤΗΣΙΑ
   13: ΡΟΣΑΜΠΩ-ΑΜΕΡΙΚΗ
   14: ΑΜΕΡΙΚΗ-ΒΟΡΕΙΟΑΜΕΡΙΚΑΝΙΚΗ ΑΝΕΞΑΡΤΗΣΙΑ
@@ -17747,15 +17745,15 @@
   10: '1973'
   11: 544S
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΠΟΔΙΣΤΡΙΑΣ
   13: ΚΑΠΟΔΙΣΤΡΙΑΣ
 - 0: 1378
   1: ΓΟΥΝΤΑΡ,ΒΑΝ
   2: ΣΥΓΚΡΙΤΙΚΑ ΔΟΚΙΜΙΑ ΓΥΡΩ ΑΠΟ ΤΗΝ ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ
-  4: 970 ΓΟΥ
+  4: 970ΓΟΥ
   5: '427'
   6: ΤΑΧΤΣΗΣ,Κ
   8: ΠΑΛΤΕΖΑΝΑΚΗ
   9: ΑΘΗΝΑ
   10: '1969'
   11: 518Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΟΚΙΜΙΑ
@@ -17774,50 +17772,50 @@
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΑΜΕΡΙΚΑΝΙΚΟ ΘΕΑΤΡΟ-ΕΡΓΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΜΕΡΙΚΗ
 - 0: 1380
   1: Χ.Σ
   2: ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ
   3: ΑΡΧΑΙΟΤΗΤΕΣ ΚΑΙ ΜΝΗΜΕΙΑ ΑΙΤΩΛΟΚΑΡΝΑΝΙΑΣ
-  4: 938.22 ΑΙΤ
+  4: 938.22ΑΙΤ
   5: '321'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 15Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ
   13: ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ-ΜΝΗΜΕΙΑ
   14: ΜΝΗΜΕΙΑ-ΑΙΤΩΛΟΚΑΡΝΑΝΙΑ
 - 0: 1381
   1: Χ.Σ
   2: ΑΠΕΙΛΗ ΝΕΟΥ ΑΚΡΩΤΗΡΙΑΣΜΟΥ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ
-  4: 938.7 ΑΠΕ
+  4: 938.7ΑΠΕ
   5: '1975'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 125Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΠΕΙΛΗ ΑΚΡΩΤΗΡΙΑΣΜΟΥ
   13: ΑΠΕΙΛΗ ΑΚΡΩΤΗΡΙΑΣΜΟΥ
 - 0: 1382
   1: Χ.Σ
   2: ΑΠΟΚΑΛΥΠΤΗΡΙΑ ΠΡΟΤΟΜΗΣ ΑΡΧΙΣΤΑΤΗΓΟΥ ΓΕΩΡΓΙΟΥ ΚΑΡΑΙΣΚΑΚΗ
-  4: 938.566ΑΠΟ
+  4: 938.566Χ.Σ
   5: '1878'
   8: Χ.Ε
   9: ΑΡΤΑ
   10: '1965'
   11: 44Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΑΡΑΙΣΚΑΚΗΣ
   13: ΚΑΡΑΙΣΚΑΚΗΣ
 - 0: 1383
   1: Χ.Σ
   2: ΑΡΤΑ
   3: ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
-  4: 938.939ΑΡΤ
+  4: 938.939Χ.Σ
   5: '305'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 19Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΜΝΗΜΕΙΑ
@@ -17833,15 +17831,15 @@
   11: 15Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΡΧΑΙΑ
 - 0: 1385
   1: Χ.Σ
   2: ΑΡΧΕΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΠΑΛΙΓΓΕΝΕΣΙΑΣ ΜΕΧΡΙ ΤΗΣ ΕΓΚΑΤΑΣΤΑΣΕΩΣ
   3: ΤΗΣ ΒΑΣΙΛΕΙΑΣ
-  4: 938.501ΑΡΧ
+  4: 938.501Χ.Σ
   5: 1907-1908
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1971'
   11: 572Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΕΙΑ
   13: ΑΡΧΕΙΑ-ΠΑΛΙΓΓΕΝΕΣΙΑ
@@ -17887,66 +17885,66 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΓΓΡΑΦΑ
   13: ΕΓΓΡΑΦΑ-ΔΙΠΛΩΜΑΤΙΚΑ
   14: ΔΙΠΛΩΜΑΤΙΚΑ ΕΓΓΡΑΦΑ-1913
   15: 1913-ΔΙΠΛΩΜΑΤΙΚΑ ΕΓΓΡΑΦΑ
 - 0: 1389
   1: Χ.Σ
   2: ΕΙΚΟΝΟΓΡΑΦΙΑ ΤΟΥ 21
-  4: 938.5 ΕΙΚ
+  4: 938.5Χ.Σ
   5: '2565'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1971'
   11: 86Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821-ΕΙΚΟΝΟΓΡΑΦΙΑ
   13: 1821-ΕΙΚΟΝΟΓΡΑΦΙΑ
   14: ΜΑΚΡΥΓΙΑΝΝΗΣ-ΕΙΚΟΝΟΓΡΑΦΙΑ
 - 0: 1390
   1: Χ.Σ
   2: ΤΟ ΕΙΚΟΣΙΕΝΑ
   3: ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ
-  4: 938.5 ΕΙΚ
+  4: 938.5Χ.Σ
   5: '1883'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 1024Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821
   13: 1821-ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ
   14: ΕΙΚΟΣΙΕΝΑ-ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ
   15: ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ
 - 0: 1391
   1: Χ.Σ
   2: 28 ΟΚΤΩΒΡΙΟΥ 1940
   3: Η ΕΛΛΑΔΑ ΣΤΟ ΧΑΡΑΚΩΜΑ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
-  4: 938.752ΟΚΤ
+  4: 938.752Χ.Σ
   5: '2539'
   8: ΕΥΘΥΝΗ
   9: ΑΘΗΝΑ
   10: '1980'
   11: 259Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
   13: 1940-28 ΟΚΤΩΒΡΙΟΥ
   14: 28 ΟΚΤΩΒΡΙΟΥ-1940
 - 0: 1392
   1: Χ.Σ
   2: ΕΙΣ ΜΝΗΜΗΝ Κ. ΑΜΑΝΤΟΥ(1874-1960)
-  4: 938.64 ΜΝΗ
+  4: 938.64ΜΝΗ
   5: 1881-2341
   8: ΜΥΡΤΙΔΗ
   9: ΑΘΗΝΑ
   10: '1960'
   11: 531Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΑΜΑΝΤΟΣ-ΜΝΗΜΗ
 - 0: 1393
   1: Χ.Σ
   2: Η ΕΚΣΤΡΑΤΕΙΑ ΕΙΣ ΤΗΝ ΜΙΚΡΑΝ ΑΣΙΑΝ(1919-1922)
   3: ΕΠΙΘΕΤΙΚΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ ΔΕΚΕΜΒΡΙΟΥ 1920 ΜΑΡΤΙΟΥ 1921
-  4: 938.721ΕΚΣ
+  4: 938.721Χ.Σ
   5: 1793-1873-8192
   8: ΓΕΝ.ΕΠΙΤ.ΣΤΡΑΤΟΥ
   9: ΑΘΗΝΑ
   10: '1963'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
   13: ΜΙΚΡΑ ΑΣΙΑ-ΕΚΣΤΡΑΤΕΙΑ
   14: 1919-ΜΙΚΡΑ ΑΣΙΑ
@@ -17965,15 +17963,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   13: ΣΤΡΑΤΟΣ
   14: '1959'
   15: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
 - 0: 1395
   1: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
   2: ΕΛΛΑΣ
-  4: 938 ΕΛΛ
+  4: 938ΕΛΛ
   5: 362-363-364-
   8: ΕΛΕΥΘΕΡΟΥΔΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '1926'
   11: 156Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΑΣ
   13: ΕΛΛΑΣ
@@ -18003,107 +18001,107 @@
   11: 133Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΓΑΛΛΙΑ
   13: ΓΑΛΛΙΑ-ΛΟΓΟΙ
   14: ΕΛΛΑΣ-ΛΟΓΟΙ
 - 0: 1398
   1: Χ.Σ
   2: ΕΛΛΗΝΙΚΑ ΔΙΠΛΩΜΑΤΙΚΑ ΕΓΓΡΑΦΑ 1940-41
-  4: 938.75ΕΛΛ
+  4: 938.75Χ.Σ
   5: '2393'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1980'
   11: 244Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΓΓΡΑΦΑ
   13: ΕΓΓΡΑΦΑ-ΔΙΠΛΩΜΑΤΙΚΑ
   14: ΔΙΠΛΩΜΑΤΙΚΑ ΕΓΓΡΑΦΑ-1940
   15: 1940-ΕΓΓΡΑΦΑ
 - 0: 1399
   1: Χ.Σ
   2: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ 1940-1941
   3: Η ΙΤΑΛΙΚΗ ΕΙΣΒΟΛΗ
-  4: 938.752ΕΛΛ
+  4: 938.752Χ.Σ
   5: '2136'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1960'
   11: 342Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
   13: ΠΟΛΕΜΟΣ-ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ
   14: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ
   15: 1940-ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ
 - 0: 1400
   1: Χ.Σ
   2: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ 1940-1941
   3: ΧΕΙΜΕΡΙΝΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ-ΙΤΑΛΙΚΗ ΕΠΙΘΕΣΕΙΣ ΜΑΡΤΙΟΥ
-  4: 938.752ΕΛΛ
+  4: 938.752Χ.Σ
   5: '2135'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1966'
   11: 250Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
   13: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ
   14: 1940-ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ
   15: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
 - 0: 1401
   1: Χ.Σ
   2: Η ΕΛΛΗΝΙΚΗ ΑΝΤΕΠΙΘΕΣΙΣ 1940-1941
-  4: 938.75ΕΛΛ
+  4: 938.75Χ.Σ
   5: '2137'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1966'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
   13: 1940-ΑΝΤΕΠΙΘΕΣΗ
   14: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
 - 0: 1402
   1: Χ.Σ
   2: ΤΟ ΕΛΛΗΝΙΚΟΝ ΕΚΣΤΡΑΤΕΥΤΙΚΟΝ ΣΩΜΑ ΕΙΣ ΜΕΣΗΜΒΡΙΝΗΝ ΡΩΣΙΑΝ 1919
-  4: 938.72ΕΛΛ
+  4: 938.72Χ.Σ
   5: '1877'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1955'
   11: 446Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΣΙΑ
   13: ΡΩΣΙΑ-1919
   14: 1919-ΡΩΣΙΑ
   15: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
 - 0: 1403
   1: Χ.Σ
   2: Ο ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΠΡΩΤΟΝ ΠΑΓΚΟΣΜΙΟΝ ΠΟΛΕΜΟΝ
   3: 1914-1918
-  4: 938.721ΕΛΛ
+  4: 938.721Χ.Σ
   5: 1874-1875-
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1958'
   11: 374Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
   13: ΠΟΛΕΜΟΣ-Α'ΠΑΓΚΟΣΜΙΟΣ
   14: Α'ΠΑΓΚΟΣΜΙΟΣ ΠΟΛΕΜΟΣ
   15: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
 - 0: 1404
   1: Χ.Σ
   2: Ο ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΔΕΥΤΕΡΟ ΠΑΓΚΟΣΜΙΟ ΠΟΛΕΜΟΝ
   3: ΑΙΤΙΑ ΚΑΙ ΑΦΟΡΜΑΙ ΕΛΛΗΝΟ-ΙΤΑΛΙΚΟΥ ΠΟΛΕΜΟΥ (1940-1941)
-  4: 938.75 ΕΛΛ
+  4: 938.75Χ.Σ
   5: '1876'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1959'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
   13: ΠΟΛΕΜΟΣ-Β'ΠΑΓΚΟΣΜΙΟΣ
   14: Β'ΠΑΓΚΟΣΜΙΟΣ ΠΟΛΕΜΟΣ
   15: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
 - 0: 1405
   1: Χ.Σ
   2: ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ ΚΑΤΑ ΤΟΝ ΑΝΤΙΣΥΜΜΟΡΙΑΚΟΥ ΑΓΩΝΑ (1946-1949)
-  4: 938.774ΕΛΛ
+  4: 938.774Χ.Σ
   5: '2238'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 469Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ
   13: ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ
@@ -18121,160 +18119,160 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΑΣΙΛΕΙΣ
   13: ΒΑΣΙΛΕΙΣ-ΕΛΛΗΝΕΣ
   14: ΕΛΛΗΝΕΣ ΒΑΣΙΛΕΙΣ
 - 0: 1407
   1: Χ.Σ
   2: Η ΕΞΕΛΙΞΙΣ ΤΟΥ ΚΥΠΡΙΑΚΟΥ ΚΑΙ ΟΙ ΘΕΣΕΙΣ ΤΗΣ ΝΕΑΣ ΔΗΜΟΚΡΑΤΙΚΗΣ
   3: ΚΙΝΗΣΕΩΣ
-  4: 938.497ΕΞΕ
+  4: 938.497Χ.Σ
   5: '2233'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ
 - 0: 1408
-  1: Χ.Ε
+  1: Χ.Σ
   2: Ο ΕΟΡΤΑΣΜΟΣ ΤΗΣ 100ΕΤΗΡΙΔΟΣ
   3: ΑΝΤΩΝΙΟΥ Δ.ΚΕΡΑΜΟΠΟΥΛΛΟΥ
-  4: 938 ΕΟΡ
+  4: 938Χ.Σ
   5: '2348'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 33Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΚΕΡΑΜΟΠΟΥΛΟΣ-ΙΣΤΟΡΙΑ
 - 0: 1409
   1: Χ.Σ
   2: Ο ΕΟΡΤΑΣΜΟΣ ΤΗΣ 100ΕΤΗΡΙΔΟΣ ΤΟΥ ΗΡΩΟΣ ΤΟΥ ΜΑΚΕΔΟΝΙΚΟΥ ΑΓΩΝΟΣ
   3: ΠΑΥΛΟΥ ΜΕΛΑ
-  4: 938.667ΕΟΡ
+  4: 938.667Χ.Σ
   5: '2347'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1972'
   11: 29Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΠΑΥΛΟΣ ΜΕΛΑΣ
   14: ΜΕΛΑΣ-ΜΑΚΕΔΟΝΙΑ
 - 0: 1410
   1: Χ.Σ
   2: ΕΠΙΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΕΙΣ ΜΙΚΡΑΝ ΑΣΙΑΝ ΕΚΣΤΡΑΤΕΙΑΣ (1919-1922
-  4: 938.72 ΕΠΙ
+  4: 938.72Χ.Σ
   5: 1793-8192
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 495Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
   13: ΜΙΚΡΑ ΑΣΙΑ-1919
   14: 1919-ΜΙΚΡΑ ΑΣΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 1411
   1: Χ.Σ
   2: ΕΠΙΧΕΙΡΗΣΕΙΣ ΕΙΣ ΘΡΑΚΗΝ(1919-1923)
-  4: 938.695ΕΠΙ
+  4: 938.695Χ.Σ
   5: '2132'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1969'
   11: 221Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
   13: ΘΡΑΚΗ-ΕΠΙΧΕΙΡΗΣΕΙΣ
   14: 1919-ΘΡΑΚΗ
   15: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
 - 0: 1412
   1: Χ.Σ
   2: Η ΕΥΡΩΠΑΙΚΗ ΟΛΟΚΛΗΡΩΣΗ
   3: Η ΕΛΛΑΔΑ ΜΕΤΑ ΤΟ ΜΑΑΣΤΡΙΧΤ
-  4: 938.87 ΕΥΡ
+  4: 938.87Χ.Σ
   5: '2561'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1992'
   11: 377Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΥΡΩΠΗ
   13: ΕΥΡΩΠΗ-ΜΑΑΣΤΡΙΧΤ
   14: ΜΑΑΣΤΡΙΧΤ
   15: ΕΛΛΑΔΑ-ΜΑΑΣΤΡΙΧ
 - 0: 1413
   1: Χ.Σ
   2: ΗΠΕΙΡΟΣ
   3: ΙΣΤΟΡΙΑ,ΓΕΩΓΡΑΦΙΑ,ΓΛΩΣΣΑ Κ.Λ.Π
-  4: 938.93 ΗΠΕ
+  4: 938.93Χ.Σ
   5: '2094'
   8: ΗΠΕΙΡΩΤΙΚΗ ΕΣΤΙΑ
   9: ΙΩΑΝΝΙΝΑ
   10: '1952'
   11: 162Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
 - 0: 1414
   1: Χ.Σ
   2: ΗΠΕΙΡΟΣ
   3: Η ΕΤΑΙΡΕΙΑ ΗΠΕΙΡΩΤΙΚΩΝ ΜΕΛΕΤΩΝ
-  4: 938.93 ΗΠΕ
+  4: 938.93Χ.Σ
   5: '2089'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1989'
   11: 110Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΙΣΤΟΡΙΑ
 - 0: 1415
   1: Χ.Σ
   2: Ο ΙΠΠΟΤΗΣ ΙΩΑΝΝΗΣ ΓΑΒΡΙΗΛ
-  4: 938.545ΙΠΠ
+  4: 938.545Χ.Σ
   5: '2425'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1963'
   11: 69Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΦΙΛΕΛΛΗΝΑΣ
   13: ΦΙΛΕΛΛΗΝΑΣ-ΓΑΒΡΙΗΛ
   14: ΓΑΒΡΙΗΛ-ΙΠΠΟΤΗΣ
 - 0: 1416
   1: Χ.Σ
   2: ΙΣΡΑΗΛ
   3: ΓΕΓΟΝΟΤΑ ΚΑΙ ΑΡΙΘΜΟΙ
-  4: 950 ΙΣΡ
+  4: 950Χ.Σ
   5: '444'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1979'
   11: 247Σ
   12: ΙΣΡΑΗΛΙΝΗ ΙΣΤΟΡΙΑ
   13: ΙΣΡΑΗΛ-ΙΣΤΟΡΙΑ
 - 0: 1417
   1: Χ.Σ
   2: Η ΙΣΤΟΡΙΑ ΤΗΣ ΑΜΕΡΙΚΑΝΙΚΗΣ ΠΡΟΣΠΑΘΕΙΑΣ ΕΙΣ ΤΗΝ ΕΛΛΑΔΑ
-  4: 970 ΙΣΤ
+  4: 970Χ.Σ
   5: '1947'
   8: Χ.Ε
   9: Χ.Τ
   10: '1952'
   11: 144Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΧΕΔΙΟ ΜΑΡΣΑΛΛ
   13: ΣΧΕΔΙΟ ΜΑΡΣΑΛ
   14: ΜΑΡΣΑΛ-ΣΧΕΔΙΟ
 - 0: 1418
   1: Χ.Σ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΑΔΑΣ
-  4: 938.1 Χ.Σ
+  4: 938.1Χ.Σ
   5: '1909'
   8: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ
   9: ΑΘΗΝΑ
   10: '1978'
   11: 600Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
 - 0: 1419
   1: Χ.Σ
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΛΑΟΥ ΤΟΥ ΙΣΡΑΗΛ ΜΕΧΡΙ ΤΟΥ 1880
-  4: 950 Χ.Σ
+  4: 950Χ.Σ
   5: 441-442
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1974'
   11: 360Σ
   12: ΙΣΡΑΗΛΙΝΗ ΙΣΤΟΡΙΑ
   13: ΙΣΡΑΗΛ-ΙΣΤΟΡΙΑ
@@ -18288,15 +18286,15 @@
   10: '1966'
   11: 369Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ
 - 0: 1421
   1: Χ.Σ
   2: ΚΥΠΡΟΣ '74 ΤΟ ΑΛΛΟ ΠΡΟΣΩΠΟ ΤΗΣ ΑΦΡΟΔΙΤΗΣ
-  4: 938.497ΚΥΠ
+  4: 938.497Χ.Σ
   5: '380'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 277Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΑΦΡΟΔΙΤΗ
@@ -18339,22 +18337,23 @@
   10: '1980'
   11: 95Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
 - 0: 1425
   1: Χ.Σ
   2: ΜΕΓΑΛΕΣ ΜΟΡΦΕΣ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
-  4: 938 ΜΕΓ
+  4: 938Χ.Σ
   5: 1957-2355
   8: ΚΟΤΖΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 10Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΟΡΦΕΣ
   13: ΜΟΡΦΕΣ ΤΗΣ ΙΣΤΟΡΙΑΣ
+  14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
 - 0: 1426
   1: Χ.Σ
   2: ΜΟΡΦΑΙ ΤΗΣ ΜΑΓΝΗΣΙΑΣ
   4: 938.931ΜΟΡ
   5: 1973-1974
   8: Χ.Ε
   9: ΒΟΛΟΣ
@@ -18363,26 +18362,26 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΓΝΗΣΙΑ
   13: ΜΑΓΝΗΣΙΑ-ΜΟΡΦΕΣ
   14: ΜΟΡΦΕΣ ΜΑΓΝΗΣΙΑΣ
 - 0: 1427
   1: Χ.Σ
   2: ΜΩΣΑΒ ΚΑΙ ΚΙΜΠΟΥΤΖ
   3: ΤΡΟΠΟΙ ΑΓΡΟΤΙΚΗΣ ΖΩΗΣ ΣΤΟ ΙΣΡΑΗΛ
-  4: 915.35 ΜΩΣ
+  4: 915.35ΜΩΣ
   5: '440'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1979'
   11: 34Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΙΣΡΑΗΛ-ΑΓΡΟΤΙΚΗ
   13: ΙΣΡΑΗΛ-ΓΕΩΓΡΑΦΙΑ
 - 0: 1428
   1: Χ.Σ
   2: ΠΑΝΗΓΥΡΙΚΟΙ ΛΟΓΟΙ ΑΚΑΔΗΜΑΙΚΩΝ ΓΙΑ ΤΗΝ 28 ΟΚΤΩΒΡΙΟΥ 1940
-  4: 938.752ΠΑΝ
+  4: 938.752ΧΑΡ
   5: '2505'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 608Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940-28 ΟΚΤΩΒΡΙΟΥ
   13: 1940-28 ΟΚΤΩΒΡΙΟΥ
@@ -18412,26 +18411,26 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΩΑΝΝΙΝΑ
   13: ΙΩΑΝΝΙΝΑ-ΠΡΑΜΑΝΤΑ
   14: ΠΡΑΜΑΝΤΑ
   15: ΤΖΟΥΜΕΡΚΑ-ΠΡΑΜΑΝΤΑ
 - 0: 1431
   1: Χ.Σ
   2: ΠΡΟΒΛΗΜΑΤΑ ΕΔΑΦΙΚΗΣ ΑΚΕΡΑΙΟΤΗΤΑΣ (ΑΙΓΑΙΟ)
-  4: 938.7 ΠΡΟ
+  4: 938.7ΠΡΟ
   5: '1977'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 32Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΔΑΦΙΚΗ ΑΚΕΡΑΙΟΤΗΤΑ
   13: ΕΔΑΦΙΚΗ ΑΚΕΡΑΙΟΤΗΤΑ
 - 0: 1432
   1: Χ.Σ
   2: Η ΠΡΟΣ ΠΟΛΕΜΟΝ ΠΡΟΠΑΡΑΣΚΕΥΗ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΣΤΡΑΤΟΥ (1923-1940
-  4: 938.73ΠΡΟ
+  4: 938.73Χ.Σ
   5: '2134'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1969'
   11: 171Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ
   13: ΕΛΛΗΝΙΚΟΣ ΣΤΡΑΤΟΣ-1940
@@ -18447,109 +18446,109 @@
   11: 180Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΛΕΣΤΙΝΛΗΣ
   13: ΒΕΛΕΣΤΙΝΛΗΣ
   14: ΦΕΡΑΙΟΣ
 - 0: 1434
   1: Χ.Σ
   2: ΤΟ ΡΟΥΜΑΝΙΚΟ ΒΙΒΛΙΟ
-  4: 949.8 ΡΟΥ
+  4: 949.8Χ.Σ
   5: '2563'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Τ
   11: 133Σ
   12: ΡΟΥΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
   13: ΡΟΥΜΑΝΙΑ-ΙΣΤΟΡΙΑ
 - 0: 1435
   1: Χ.Σ
   2: ΣΥΝΤΟΜΗ ΙΣΤΟΡΙΑ ΤΩΝ Η.Π.Α
-  4: 973 ΣΥΝ
+  4: 973Χ.Σ
   5: '428'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 199Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΙΣΤΟΡΙΑ-Η.Π.Α
   13: ΑΜΕΡΙΚΗ-ΙΣΤΟΡΙΑ
   14: Η.Π.Α-ΙΣΤΟΡΙΑ
 - 0: 1436
   1: Χ.Σ
   2: ΣΥΝΟΨΗ ΤΗΣ ΓΕΩΓΡΑΦΙΑΣ ΤΗΣ ΑΜΕΡΙΚΗΣ
-  4: 917 ΣΥΝ
+  4: 917Χ.Σ
   5: '2324'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 205Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΑΜΕΡΙΚΗ
   13: ΑΜΕΡΙΚΗ-ΓΕΩΓΡΑΦΙΑ
 - 0: 1437
   1: Χ.Σ
   2: ΣΤΡΑΤΗΓΟΥ ΜΑΚΡΥΓΙΑΝΝΗ
   3: ΠΡΑΓΜΑΤΑ ΚΑΙ ΟΡΑΜΑΤΑ
-  4: 938.478ΣΤΡ
+  4: 938.478Χ.Σ
   5: '1694'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 211Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΡΥΓΙΑΝΝΗΣ
   13: ΜΑΚΡΥΓΙΑΝΝΗΣ
 - 0: 1438
   1: Χ.Σ
   2: ΣΤΕΡΕΑ ΕΛΛΑΣ
   3: ΕΙΚΟΝΟΓΡΑΦΗΜΕΝΗ ΕΠΙΘΕΩΡΗΣΙΣ ΤΗΣ ΡΟΥΜΕΛΗΣ
-  4: 938.91 ΣΤΕ
+  4: 938.91Χ.Σ
   5: '336'
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΤΕΡΕΑ ΕΛΛΑΣ
   13: ΣΤΕΡΕΑ ΕΛΛΑΣ
   14: ΡΟΥΜΕΛΗ
 - 0: 1439
   1: Χ.Σ
   2: ΤΡΙΑ ΕΤΗ ΔΙΑΚΥΒΕΡΝΗΣΕΩΣ ΤΟΥ Κ.ΙΩΑΝΝΟΥ ΜΕΤΑΞΑ (1936-1939)
-  4: 938.714ΤΡΙ
+  4: 938.714Χ.Σ
   5: '2557'
   8: ΠΥΡΣΟΣ
   9: ΑΘΗΝΑ
   10: '1939'
   11: 323Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΤΑΞΑΣ
   13: ΜΕΤΑΞΑΣ
 - 0: 1440
   1: Χ.Σ
   2: ΦΑΚΕΛΛΟΣ ΑΙΓΑΙΟ
-  4: 938.7 ΦΑΚ
+  4: 938.7Χ.Σ
   5: '1976'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 78Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΦΑΚΕΛΛΟΣ ΑΙΓΑΙΟΥ
   13: ΑΙΓΑΙΟ-ΦΑΚΕΛΛΟΣ
 - 0: 1441
   1: Χ.Σ
   2: ΧΡΟΝΙΚΟΝ 1940-1944
   3: ΕΜΠΡΟΣ ΤΗΣ ΕΛΛΑΔΟΣ ΠΑΙΔΙΑ
-  4: 938.75 ΧΡΟ
+  4: 938.75Χ.Σ
   5: '2295'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 375Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1940
   13: 1940-ΧΡΟΝΙΚΟ
   14: ΧΡΟΝΙΚΟ-1940
   15: 1944-ΧΡΟΝΙΚΟ
 - 0: 1442
-  1: Χ.Σ
+  1: ΜΟΔΗ,ΓΕΩΡΓΙΟΥ
   2: ΧΩΡΙΑ-ΦΡΟΥΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
-  4: 938.664ΧΩΡ
+  4: 938.664ΜΟΔ
   5: '349'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1964'
   11: 16Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΧΩΡΙΑ ΦΡΟΥΡΙΑ
@@ -18970,15 +18969,15 @@
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΒΙΟΓΡΑΦΙΑ
   14: ΒΙΟΓΡΑΦΙΑ-ΚΟΥΝ
   15: ΚΟΥΝ-ΒΙΟΓΡΑΦΙΑ
 - 0: 1475
   1: Χ.Σ
   2: ΕΛΕΥΘΕΡΙΟΣ ΒΕΝΙΖΕΛΟΣ
   3: Η ΖΩΗ ΚΑΙ ΤΟ ΕΡΓΟΝ ΤΟΥ
-  4: 938.672ΕΛΕ
+  4: 938.672Χ.Σ
   5: '2585'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1936'
   11: 175Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ
   13: ΒΕΝΙΖΕΛΟΣ-ΖΩΗ ΚΑΙ ΕΡΓΟ
@@ -19014,27 +19013,27 @@
   10: Χ.Χ
   11: 194Σ
   12: ΓΗ-ΙΣΤΟΡΙΑ
   13: ΑΝΑΚΑΛΥΨΗ ΤΗΣ ΓΗΣ
 - 0: 1479
   1: Χ.Σ
   2: ΜΝΗΜΗ ΔΗΜΗΤΡΙΟΥ ΑΙΓΝΗΤΟΥ (1862-1934)
-  4: 938.729ΜΝΗ
+  4: 938.729Χ.Σ
   5: '2378'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1975'
   11: 469Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΑΙΓΙΝΗΤΗΣ-(1862-1934)
 - 0: 1480
   1: Χ.Σ
   2: ΓΕΩΡΓΙΟΥ ΠΑΠΑΝΔΡΕΟΥ
   3: ΚΕΙΜΕΝΑ (1913-1942)
-  4: 938.791ΓΕΩ
+  4: 938.791Χ.Σ
   5: '2379'
   8: ΜΠΙΡΗΣ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 318Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΓΕΤΕΣ
   13: ΗΓΕΤΕΣ-ΠΑΠΑΝΔΡΕΟΥ ΓΕΩΓΡΙΟΣ
@@ -19152,26 +19151,26 @@
   9: ΑΘΗΝΑ
   10: '1990'
   11: 240Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΕΠΕΛΕΝΛΗ
   13: ΤΕΠΕΛΕΝΛΗ-ΑΛΗ ΠΑΣΑΣ
   14: ΑΛΗ ΠΑΣΑΣ-ΤΕΠΕΛΕΝΛΗ
 - 0: 1490
-  1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΤΕΦΑΝΟΣ Π.
-  2: ΤΟ ΧΕΡΣΑΙΟ ΔΙΚΤΥΟ ΕΠΙΚΟΙΝΩΝΙΑΣ ΣΤΟ ΚΡΑΤΟΣ ΤΟΥ ΑΛΗ ΠΑΣΑ
-  3: ΤΕΠΕΛΕΝΛΗ
-  4: 938.484ΜΑΚ
-  5: 1708-4160
-  8: ΠΑΠΑΖΗΣΗ
+  1: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ,ΘΩΜΑΣ
+  2: ΤΟ ΠΡΟΕΠΑΝΑΣΤΑΤΙΚΟ ΚΙΝΗΜΑ ΤΟΥ ΠΑΠΑ ΕΥΘΥΜΙΟΥ ΒΛΑΧΑΒΑ ΣΤΗ
+  3: ΘΕΣΣΑΛΑΙ (1807-1809) ΚΑΙ ΟΙ ΞΕΝΟΙ ΙΣΤΟΡΙΚΟΙ-ΠΕΡΙΗΓΗΤΕΣ
+  4: 938.485ΠΑΠ
+  5: '5194'
+  8: ΟΛΥΜΠΟΣ
   9: ΑΘΗΝΑ
-  10: '1990'
-  11: 240Σ
-  12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΕΠΕΛΕΝΛΗ
-  13: ΤΕΠΕΛΕΝΛΗ-ΑΛΗ ΠΑΣΑΣ
-  14: ΑΛΗ ΠΑΣΑΣ-ΤΕΠΕΛΕΝΛΗ
+  10: '1998'
+  11: '91'
+  12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ
+  13: ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ-ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
+  14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ
 - 0: 1491
   1: ΤΖΟΥΒΑΡΑ-ΣΟΥΛΗ,ΧΡΥΣΗΙΣ
   2: ΑΜΒΡΑΚΙΑ
   4: 938.21 ΤΖΟ
   5: 2818-2819
   8: Χ.Ε
   9: Χ.Τ
@@ -19419,28 +19418,28 @@
   11: 128Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΦΗΓΗΜΑ
   13: ΑΦΗΓΗΜΑ-ΤΟ ΓΕΦΥΡΙ ΤΗΣ ΑΡΤΑΣ
   14: ΤΟ ΓΕΦΥΡΙ ΤΗΣ ΑΡΤΑΣ-ΑΦΗΓΗΜΑ
 - 0: 1511
   1: Χ.Σ
   2: ΜΟΥΣΕΙΟ "ΕΛΕΥΘΕΡΙΟΣ Κ.ΒΕΝΙΖΕΛΟΣ"
-  4: 938.672ΜΟΥ
+  4: 938.672Χ.Σ
   5: '2884'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1992'
   11: 154Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΝΙΖΕΛΟΣ
   13: ΒΕΝΙΖΕΛΟΣ-ΜΟΥΣΕΙΟ
   14: ΜΟΥΣΕΙΟ-ΒΕΝΙΖΕΛΟΣ
 - 0: 1512
   1: ΨΑΘΑΣ,ΔΗΜΗΤΡΗΣ
   2: ΖΗΤΕΙΤΑΙ ΨΕΥΤΗΣ
   3: ΚΩΜΩΔΙΑ
-  4: 886.2 ΨΑΘ
+  4: 886.2ΨΑΘ
   5: '2888'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1993'
   11: 107Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
@@ -19497,27 +19496,27 @@
   11: 22Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΤΟΥΡΛΙΔΗΣ-ΠΟΝΤΟΣ
   14: ΠΟΝΤΟΣ-ΤΟΥΡΛΙΔΗΣ
 - 0: 1517
   1: ΤΖΙΟΒΑΣ,ΠΑΝΟΣ ΔΗΜ
   2: ΗΠΕΙΡΩΤΙΚΑ ΑΝΕΚΔΟΤΑ
-  4: 398 ΤΖΙ
+  4: 938.93ΤΖΙ
   5: 2883-10439
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1992'
   11: 93Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΝΕΚΔΟΤΑ
   14: ΑΝΕΚΔΟΤΑ-ΗΠΕΙΡΟΣ
 - 0: 1518
   1: ΑΘΗΝΑΙΟΣ,ΑΝΔΡΕΑΣ
-  2: 7ΕΛΛΗΝΙΚΑ ΘΕΜΑΤΑ
-  4: 938 ΑΘΗ
+  2: ΕΛΛΗΝΙΚΑ ΘΕΜΑΤΑ
+  4: 938ΑΘΗ
   5: '2882'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1976'
   11: 46Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΜΑΤΑ
   13: ΘΕΜΑΤΑ-ΕΛΛΑΔΑ
@@ -19536,15 +19535,15 @@
   15: ΠΕΡΙΟΔΙΚΟ-ΘΕΣΣΑΛΙΑ
   17: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
   30: ΤΟΜΟΣ 10
 - 0: 1520
   1: ΠΑΠΑΚΩΣΤΑΣ,ΝΙΚ
   2: ΗΠΕΙΡΩΤΙΚΑ
   3: ΑΘΑΝΑΝΙΚΑ
-  4: 938.93 ΠΑΠ
+  4: 938.93ΠΑΠ
   5: 1380-3016
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 646Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΙΚΑ
@@ -19670,16 +19669,16 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΩΣΟΠΑ
   13: ΗΠΕΙΡΟΣ-ΛΑΙΚΗ ΤΕΧΝΗ
   14: ΛΑΙΚΗ ΤΕΧΝΗ-ΗΠΕΙΡΟΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;16
 - 0: 1530
   1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ,ΙΩΑΝΝΗΣ
   2: Ο ΣΥΓΧΡΟΝΟΣ ΤΡΑΓΙΚΟΣ ΑΝΘΡΩΠΟΣ ΚΑΙ ΤΟ ΛΥΤΡΩΤΙΚΟΝ  ΡΟΔΟΧΑΡΑΜΑ
-  4: 938.009ΠΑΠ
-  5: 5771-2875-2876
+  4: 938ΠΑΠ
+  5: 5771-2875-2876-12496
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1976'
   11: 85Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΘΡΩΠΟΣ
   13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΝΘΡΩΠΟΣ
   14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -19881,15 +19880,15 @@
   10: '1978'
   11: 13Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΒΙΒΛΙΟΚΡΙΣΙΕΣ
   13: ΒΙΒΛΙΟΚΡΙΣΙΕΣ-ΛΟΓΟΤΕΧΝΙΑ
 - 0: 1547
   1: ΛΟΥΚΑΤΟΣ,ΔΗΜΗΤΡΙΟΣ Σ
   2: Ο ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ ΤΩΝ ΗΠΕΙΡΩΤΩΝ
-  4: 938.93 ΛΟΥ
+  4: 938.93ΛΟΥ
   5: 2768-2887
   8: ΑΘΗΝΑ
   9: Χ.Ε
   10: '1976'
   11: 36Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ
@@ -20139,31 +20138,31 @@
   9: Χ.Τ
   10: '1991'
   11: 25Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   14: ΠΟΙΗΜΑΤΑ
 - 0: 1566
-  1: ΜΥΡΣΙΝΗ-ΜΑΝΘΟΥ,ΑΛΚΗ
+  1: ΜΑΝΘΟΥ,ΜΥΡΣΙΝΗ-ΑΛΚΗ
   2: ΗΠΕΙΡΩΤΑΙ ΔΗΜΟΣΙΟΓΡΑΦΟΙ ΣΤΗ ΡΟΥΜΑΝΙΑ
   3: Ζ.ΣΑΡΔΕΛΛΗΣ Κ ΥΙΟΙ,ΣΠ.ΣΙΜΟΣ,Ι.ΟΙΚΟΝΟΜΟΥ,Κ.ΒΕΛΕΝΤΖΑΣ Κ.Α
-  4: 938.93 ΜΥΡ
+  4: 938.93ΜΑΝ
   5: 2828-2827-9248
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1973'
   11: 31Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΩΤΕΣ ΔΗΜΟΣΙΟΓΡΑΦΟΙ
   13: ΗΠΕΙΡΟΣ-ΔΗΜΟΣΙΟΓΡΑΦΟΙ
   14: ΔΗΜΟΣΙΟΓΡΑΦΟΙ-ΗΠΕΙΡΩΤΕΣ
 - 0: 1567
   1: ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ ΑΧ
   2: ΓΕΩΡΓΙΟΣ ΧΑΤΖΗΣ-ΠΕΛΛΕΡΕΝ
   3: Ο ΗΠΕΙΡΩΤΗΣ ΑΓΩΝΙΣΤΗΣ,Ο ΔΗΜΟΣΙΟΓΡΑΦΟΣ,Ο ΠΟΙΗΤΗΣ
-  4: 938.93 ΒΑΒ
+  4: 938.93ΒΑΒ
   5: '2773'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1963'
   11: 31Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΧΑΤΖΗΣ
@@ -20171,15 +20170,15 @@
   15: ΑΓΩΝΙΣΤΗΣ-ΧΑΤΖΗΣ
   17: ΦΩΤΟΤΥΠΙΑ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;7
 - 0: 1568
   1: ΛΑΜΠΡΙΔΗΣ,ΣΤΑΘΗΣ Δ
   2: ΚΩΣΤΑΣ ΓΚΡΑΤΖΙΟΣ
   3: Ο ΜΕΓΑΛΟΣ ΗΠΕΙΡΩΤΗΣ ΕΚΠΑΙΔΕΥΤΗΣ
-  4: 938.93 ΛΑΜ
+  4: 938.93ΛΑΜ
   5: '2829'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1983'
   11: 48Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΓΚΡΑΤΖΙΟΣ
@@ -20197,15 +20196,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   14: ΤΕΧΝΗ ΛΟΓΟΥ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 1570
   1: ΣΦΑΕΛΛΟΣ,ΔΗΜ Κ
   2: ΕΘΝΙΚΗ ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΚΑΙ ΕΘΝΙΚΑ ΙΔΑΝΙΚΑ
-  4: 938.032ΣΦΑ
+  4: 938.05ΣΦΑ
   5: 2747-2748
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 56Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ
   13: ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ-ΕΛΛΑΣ
@@ -20280,16 +20279,16 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΖΑΓΟΡΙ
   13: ΖΑΓΟΡΙ-ΛΑΜΠΡΙΔΗΣ
   14: ΛΑΜΠΡΙΔΗΣ-ΓΙΑΤΡΟΣ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;49
 - 0: 1576
   1: ΚΑΡΑΤΖΕΝΗΣ,ΔΗΜΗΤΡΙΟΣ ΦΩΤΙΟΣ
   2: Η ΕΚΑΤΟΝΤΑΕΤΗΡΙΣ ΤΗΣ ΑΡΤΑΣ(1881-1981)
-  4: 938.65 ΚΑΡ
-  5: '2807'
+  4: 938.939ΚΑΡ
+  5: 2807-15812-16445
   8: ΣΚΟΥΦΑΣ
   9: ΑΘΗΝΑ
   10: '1982'
   11: 62Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΡΤΑ
   14: ΑΡΤΑ-(1881-1981)
@@ -20345,15 +20344,15 @@
   13: ΜΑΚΕΔΟΝΙΑ-ΣΛΑΒΙΚΗ ΠΡΟΠΑΓΑΝΔΑ
   14: ΣΛΑΒΟΙ-ΣΛΑΒΙΚΗ ΠΡΟΠΑΓΑΝΔΑ
   15: ΣΛΑΒΙΚΗ ΠΡΟΠΑΓΑΝΔΑ
 - 0: 1581
   1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞ Χ
   2: ΛΑΙΚΗ ΑΡΧΙΤΕΚΤΟΝΙΚΗ
   3: ΗΠΕΙΡΩΤΕΣ ΜΑΣΤΟΡΟΙ ΚΑΙ ΓΕΦΥΡΙΑ
-  4: 938.93 ΜΑΜ
+  4: 938.93ΜΑΜ
   5: 2898-2899
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1973'
   11: 48Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΑΡΧΙΤΕΚΤΟΝΙΚΗ
@@ -20382,17 +20381,17 @@
   10: '1989'
   11: 135Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   14: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ-1821
   15: 1821-ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
 - 0: 1584
-  1: Χ.Σ
+  1: ΕΜΜΑΝΟΥΗΛ,ΦΙΛΙΠΠΟΣ
   2: Η ΕΝΝΟΙΑ ΤΗΣ ΠΑΡΑΔΟΣΕΩΣ ΚΑΙ Η ΗΠΕΙΡΟΣ
-  4: 398 Χ.Σ.
+  4: 938.93ΕΜΜ
   5: '2902'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1980'
   11: 28Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΠΑΡΑΔΟΣΗ
@@ -22086,15 +22085,15 @@
   13: ΚΑΤΟΧΗ-1944
   14: 1944-ΚΑΤΟΧΗ
   15: ΑΝΤΙΣΤΑΣΗ-1944
 - 0: 1709
   1: Χ.Σ
   2: ΤΡΑΝΣΤΕΚΟΜ
   3: ΛΕΥΚΩΜΑ
-  4: 938.5 ΤΡΑ
+  4: 938.5Χ.Σ
   5: '3164'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-1821
   13: 1821-ΛΕΥΚΩΜΑ
   14: ΛΕΥΚΩΜΑ-1821
@@ -22293,15 +22292,15 @@
   13: ΒΥΖΑΝΤΙΟ-ΜΕΛΕΤΕΣ
   14: ΜΕΛΕΤΕΣ-ΒΥΖΑΝΤΙΟ
   15: ΒΥΖΑΝΤΙΝΕΣ ΜΕΛΕΤΕΣ
 - 0: 1724
   1: Χ.Σ
   2: ΚΑΣΣΩΠΗ-ΖΑΛΟΓΓΟ
   3: ΑΠΟ ΤΟ ΟΔΟΙΠΟΡΙΚΟ ΣΤΟΝ ΕΛΛΗΝΙΚΟ ΧΩΡΟ
-  4: 938.93 ΚΑΣ
+  4: 938.93Χ.Σ
   5: '291'
   8: Χ.Ε
   9: Χ.Τ
   10: '1973'
   11: 61Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΚΑΣΣΩΠΗ
@@ -22425,15 +22424,15 @@
   10: '1978'
   11: 142Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
   13: ΘΡΑΚΗ-ΑΡΧΑΙΟΙ
 - 0: 1734
   1: ΑΡΑΒΑΝΤΙΝΟΣ,Π
   2: ΗΠΕΙΡΩΤΙΚΟΝ ΓΛΩΣΣΑΡΙΟΝ
-  4: 938.93 ΑΡΑ
+  4: 938.93ΑΡΑ
   5: '3021'
   8: ΠΕΤΡΑΚΟΥ
   9: ΑΘΗΝΑ
   10: '1909'
   11: 102Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΓΛΩΣΣΑΡΙΟ
@@ -29414,29 +29413,29 @@
   13: ΔΙΚΑΙΟΙ-ΦΛΕΣΑΙΟΙ
   14: ΦΛΕΣΑΙΟΙ
   15: ΕΘΝΕΓΕΡΣΙΑ
 - 0: 2316
   1: Χ.Σ
   2: ΤΟ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟΝ ΖΗΤΗΜΑ
   3: ΠΑΡΕΛΘΟΝ-ΠΑΡΟΝ-ΜΕΛΛΟΝ ΠΡΑΚΤΙΚΑ
-  4: 938.694ΒΟΡ
+  4: 938.694Χ.Σ
   5: '3653'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1992'
   11: 623Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
   13: ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ-ΠΡΑΚΤΙΚΑ
   14: ΠΡΑΚΤΙΚΑ-ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
   17: Β' ΠΑΝΕΛΛΗΝΙΟ ΕΠΙΣΤΗΜΟΝΙΚΟ ΣΥΝΕΔΡΙΟ
   30: ΚΟΝΙΤΣΑ 23-26 ΑΥΓΟΥΣΤΟΥ 1990
 - 0: 2317
   1: Χ.Σ
   2: Η ΑΡΧΑΙΑ ΕΛΛΑΣ
-  4: 938.1 ΑΡΧ
+  4: 938.1ΑΡΧ
   5: '256'
   8: ΚΑΔΜΟΣ
   9: ΑΘΗΝΑ
   10: '1957'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΑΡΧΑΙΟΤΗΤΑ-ΦΙΛΟΣΟΦΙΑ
   14: ΦΙΛΟΣΟΦΙΑ-ΑΡΧΑΙΑ
@@ -29495,28 +29494,28 @@
   13: ΚΥΠΡΟΣ-ΑΥΤΟΔΙΑΘΕΣΗ
   14: ΛΑΟΙ-ΑΥΤΟΔΙΑΘΕΣΗ
   15: ΔΙΚΑΙΩΜΑΤΑ-ΛΑΟΙ
 - 0: 2322
   1: Χ.Σ
   2: ΕΝΑΣ ΕΛΛΗΝΑΣ ΤΟΥ 20 ΑΙΩΝΟΣ
   3: ΕΜΜΑΝΟΥΗΛ ΜΠΕΝΑΚΗΣ
-  4: 938.8 ΕΛΛ
+  4: 938.8Χ.Σ
   5: '3677'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1931'
   11: 27Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-20 ΑΙΩΝΑΣ
   13: 20 ΑΙΩΝΑΣ-ΜΠΕΝΑΚΗΣ
   14: ΜΠΕΝΑΚΗΣ
 - 0: 2323
-  1: ΧΙΩΤΑΚΗ, ΑΜΑΛΙΑ
+  1: ΧΙΩΤΑΚΗ,ΑΜΑΛΙΑ
   2: Η ΣΥΜΠΕΡΙΦΟΡΑ ΤΟΥ ΤΡΑΠΕΖΙΚΟΥ ΚΕΦΑΛΑΙΟΥ ΣΕ ΜΙΑ ΑΓΡΟΤΙΚΗ ΚΟΙΝ
   3: Η ΠΕΡΙΠΤΩΣΗ ΤΗΣ ΤΡΑΠΕΖΑΣ ΗΠΕΙΡΟΘΕΣΣΑΛΙΑΣ ΣΤΗΝ ΑΡΤΑ
-  4: 938.6 ΧΙΩ
+  4: 938.6ΧΙΩ
   5: '3674'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1994'
   11: 509Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΓΡΟΤΙΚΗ ΚΟΙΝΩΝΙΑ
   13: ΑΓΡΟΤΙΚΗ ΚΟΙΝΩΝΙΑ-ΑΡΤΑ
@@ -29784,15 +29783,15 @@
   11: 15Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΙΑΘΟΣ
   13: ΣΚΙΑΘΟΣ-ΠΑΡΑΔΟΣΗ
   14: ΠΑΡΑΔΟΣΗ-ΣΚΙΑΘΟΣ
 - 0: 2344
   1: ΑΘΑΝΑΣΙΑΔΗ-ΝΟΒΑ,ΘΕΜ
   2: ΣΤΗΝ ΤΟΥΡΚΙΑ ΜΕ ΔΗΜΟΣΙΑΓΡΑΦΙΚΟ ΦΑΚΟ(1925-1926)
-  4: 938.73 ΑΘΑ
+  4: 938.73ΑΘΑ
   5: '2540'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΟΥΡΚΙΑ
   13: ΤΟΥΡΚΙΑ-ΔΗΜΟΣΙΟΓΡΑΦΙΑ(1925-1926)
   14: ΔΗΜΟΣΙΟΓΡΑΦΙΑ(1925-1926)
@@ -34582,15 +34581,15 @@
   13: ΛΟΡΔΟΣ ΒΥΡΩΝΑΣ
   14: ΚΟΡΙΝΘΟΣ-ΠΟΛΙΟΡΚΙΑ
   15: ΠΟΛΙΟΡΚΙΑ ΤΗΣ ΚΟΡΙΝΘΟΥ
 - 0: 2755
   1: ΛΟΙΖΙΔΗΣ,ΣΑΒΒΑΣ
   2: ΑΤΥΧΗ ΚΥΠΡΟΣ
   3: ΠΩΣ ΕΖΗΣΑ ΤΟΥΣ ΠΟΘΟΥΣ ΚΑΙ ΤΟΥΣ ΚΑΗΜΟΥΣ ΤΗΣ 1910-1980
-  4: 938.799ΛΟΙ
+  4: 938.497ΛΟΙ
   5: '4084'
   8: ΜΠΕΡΓΑΔΗ
   9: ΑΘΗΝΑ
   10: '1980'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ
 - 0: 2756
@@ -34631,15 +34630,15 @@
   11: 223S
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ
 - 0: 2759
   1: Χ.Σ
   2: Η ΕΠΕΚΤΑΤΙΚΗ ΠΟΛΙΤΙΚΗ ΤΩΝ ΣΚΟΠΙΩΝ
   3: ΣΥΛΛΟΓΗ ΕΓΓΡΑΦΩΝ (1934-1992)
-  4: 938.692ΕΠΕ
+  4: 938.692Χ.Σ
   5: '3033'
   8: Ι.Μ.Χ.Α
   9: ΘΕΣ/ΝΙΚΗ
   10: '1993'
   11: 72Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΟΠΙΑ
   13: ΣΚΟΠΙΑ-ΠΟΛΙΤΙΚΗ
@@ -34740,15 +34739,15 @@
   13: ΡΟΥΜΕΛΗ-ΟΙΚΟΓΕΝΕΙΕΣ
   14: ΣΚΑΛΤΣΟΔΗΜΟΥ
   15: ΣΤΑΙΚΟΥ
   17: ΙΣΤΟΡΙΚΕΣ ΟΙΚΟΓΕΝΕΙΕΣ:ΣΚΑΛΤΣΟΔΗΜΟΥ,ΣΤΑΙΚΟΥ,ΠΑΠΑΙΩΑΝΝΟΥ
 - 0: 2767
   1: Χ.Σ
   2: ΗΠΕΙΡΟΣ ΚΟΙΝΩΝΙΑ-ΟΙΚΟΝΟΜΙΑ 15ΟΣ-20ΟΣ ΑΙΩΝΑΣ
-  4: 938.408ΔΙΕ
+  4: 938.408Χ.Σ
   5: '2158'
   9: ΓΙΑΝΝΙΝΑ
   10: '1987'
   11: 370Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΠΡΑΚΤΙΚΑ
   13: ΗΠΕΙΡΟΣ-ΠΡΑΚΤΙΚΑ
   14: ΠΡΑΚΤΙΚΑ ΔΙΕΘΝΟΥΣ ΣΥΝΕΔΡΙΟΥ
@@ -36508,15 +36507,15 @@
   11: 310Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΛΟΓΟΤΕΧΝΕΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΛΟΓΟΤΕΧΝΕΣ
 - 0: 2905
   1: ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜ
   2: Η ΚΑΤΑ ΤΩΝ ΡΩΜΑΙΩΝ ΕΚΣΤΡΑΤΕΙΑ ΤΟΥ ΑΝΤΙΟΧΟΥ ΤΟΥ Γ'ΕΙΣ ΤΗΝ
   3: ΕΛΛΑΔΑ
-  4: 938.19 ΒΡΑ
+  4: 938.19ΒΡΑ
   5: '4174'
   8: ΣΠΑΝΟΠΟΥΛΟΥ
   9: ΑΘΗΝΑ
   10: '1974'
   11: 107Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΜΑΙΟΙ
   13: ΡΡΩΜΑΙΟΙ-ΑΝΤΙΟΧΙΟΣ Γ'
@@ -57071,17 +57070,17 @@
   9: ΑΘΗΝΑ
   10: '1991'
   11: 70Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 4653
-  1: ΡΙΤΣΙ,ΡΙΤΑ
+  1: RITCHIE,RITA
   2: ΤΑ ΧΡΥΣΑ ΓΕΡΑΚΙΑ ΤΟΥ ΤΖΕΝΓΚΙΣ ΧΑΝ
-  4: 808.899ΡΙΤ
+  4: 808.899RIT
   5: '4792'
   6: ΕΡΡ.ΜΠΑΡΤΖΙΝΟΠΟΥΛΟΣ
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '1993'
   11: 187Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -57211,31 +57210,29 @@
   9: ΑΘΗΝΑ
   10: '1976'
   11: 259Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 4664
-  1: ΝΤΑΓΛΑΣ,Λ.
-  2: Ο ΧΙΤΩΝ
-  4: 808.899ΝΤΑ
-  5: '6665'
-  6: ΜΑΡ.ΨΑΡΡΑ
-  8: ΑΓΚΥΡΑ
+  1: ΠΕΛΩ,ΠΙΕΡ
+  2: ΤΟ ΠΑΙΔΙ ΚΑΙ ΤΟ ΑΣΤΕΡΙ
+  4: 808.899ΠΕΛ
+  5: '20651'
+  8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
-  10: '1971'
-  11: 189Σ
+  10: '1979'
+  11: '160'
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
-  17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 4665
   1: ΚΡΟΝΙΝ,Α
   2: ΤΑ ΑΓΟΥΡΑ ΧΡΟΝΙΑ
-  4: 823ΚΡΟ
+  4: 8Ο8.899ΚΡΟ
   5: 6666,9596,20585
   6: ΠΑΠΑΔΑΚΗ-ΜΑΥΡΟΕΙΔΗ,Σ
   8: ΑΣΤΗΡ
   9: ΑΘΗΝΑ
   10: '1978'
   11: 320Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
@@ -67523,15 +67520,15 @@
   11: 56Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 5571
   1: ΝΙΚΟΡΕΤΖΟΣ,ΔΗΜΗΤΡΗΣ
   2: ΛΟΓΙΑ ΤΗΣ ΚΑΡΔΙΑΣ
-  4: 880.09ΝΙΚ
+  4: 808.899ΝΙΚ
   5: '6690'
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   11: 60Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -68704,27 +68701,27 @@
   10: '1952'
   11: 189Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΓΩΓΟΥ
 - 0: 5659
-  1: DOUGLAS,L.
+  1: ΝΤΑΓΚΛΑΣ,ΛΟΥΔ
   2: Ο ΧΙΤΩΝ
-  4: 889DOU
-  5: '6999'
+  4: 808.899ΝΤΑ
+  5: 6999,6665
   6: ΓΙΑΝΝΗ ΛΑΜΨΑ
   7: 2η
   8: ΔΑΜΑΣΚΟΣ
   9: ΑΘΗΝΑ
   10: '1950'
   11: 438Σ
-  12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
-  13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
-  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΓΩΓΟΥ
 - 0: 5660
   1: SWEIG,S.
   2: ΜΑΡΙΑ ΣΤΟΥΑΡΤ
   4: 889SWE
   5: '7132'
   6: ΓΙΑΝΝΗ ΑΣΤΕΡΙΑΔΗ
@@ -75679,15 +75676,15 @@
   11: 161Σ
   12: ΕΥΡΩΠΑΙΚΗ ΕΝΩΣΗ
   13: ΕΘΝΙΚΕΣ ΓΛΩΣΣΕΣ
   14: ΕΥΡΩΠΑΙΚΗ ΕΝΩΣΗ
 - 0: 6209
   1: Χ.Σ
   2: ΘΡΑΚΗ 80 ΧΡΟΝΙΑ ΑΠΟ ΤΗΝ ΕΝΣΩΜΑΤΩΣΗ
-  4: 938.695ΘΡΑ
+  4: 938.695Χ.Σ
   5: 8078-6857-
   8: ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 24Σ
   12: ΘΡΑΚΗ-ΕΝΣΩΜΑΤΩΣΗ
   13: ΕΝΣΩΜΑΤΩΣΗ-ΘΡΑΚΗ
@@ -76230,15 +76227,15 @@
   11: 147Σ
   12: ΚΩΝΣΤΑΝΤΙΝΟΣ ΚΑΡΑΜΑΝΛΗΣ
   13: ΚΩΝΣΤΑΝΤΙΝΟΣ ΚΑΡΑΜΑΝΛΗΣ
   14: ΚΩΝΣΤΑΝΤΙΝΟΣ ΚΑΡΑΜΑΝΛΗΣ
 - 0: 6256
   1: Χ.Σ
   2: ΓΙΑΝΝΙΝΑ-ΗΠΕΙΡΟΣ 19ος-20ος ΑΙΩΝΑΣ
-  4: '938.939'
+  4: 938.939Χ.Σ
   5: '8164'
   9: ΓΙΑΝΝΙΝΑ
   10: '1993'
   11: 341Σ
   12: ΓΙΑΝΝΙΝΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΠΟΛΙΤΙΣΜΟΣ
   14: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
@@ -79301,15 +79298,15 @@
   11: 174Σ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   14: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 6515
   1: ΜΠΟΡΟΒΣΚΙ,ΤΑΝΤΕΟΥΣ
   2: ΑΠΟ ΔΩ ΓΙΑ ΤΑ ΑΕΡΙΑ ΚΥΡΙΕΣ ΚΑΙ ΚΥΡΙΟΙ
-  4: 938.87ΜΠΟ8
+  4: 938.87ΜΠΟ
   5: '8645'
   8: ΣΤΟΧΑΣΤΗΣ
   9: ΑΘΗΝΑ
   10: '1981'
   11: 149Σ
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -80076,18 +80073,18 @@
   10: '2003'
   11: 211Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   15: ΔΙΗΓΗΜΑΤΑ
 - 0: 6579
-  1: ΤΟΥΡΑΤΣΟΓΛΟΥ ΙΩΑΝΝΗΣ
+  1: ΤΟΥΡΑΤΣΟΓΛΟΥ,ΙΩΑΝΝΗΣ
   2: ΜΑΚΕΔΟΝΙΑ
   3: ΙΣΤΟΡΙΑ ΜΝΗΜΕΙΑ ΜΟΥΣΕΙΑ
-  4: 398.666ΤΟΥ
+  4: 938.666ΤΟΥ
   5: 9298Α
   8: ΕΚΔΟΤΙΚΗ ΑΘΗΝΩΝ
   9: ΑΘΗΝΑ
   10: '1996'
   11: 459Σ
   12: ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ
@@ -80251,20 +80248,22 @@
   11: 435Σ
   12: ΚΥΠΡΟΣ-ΑΧΝΑ
   13: ΑΧΝΑ-ΚΥΠΡΟΣ
   14: ΚΥΠΡΟΣ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 6596
   1: Χ.Σ
-  2: ΠΕΡΙ ΠΕΤΡΟΓΕΦΥΡΩΝ...
-  5: '8656'
-  9: ΑΘΗΝΑ
-  10: '2003'
-  11: 229Σ
-  17: ΠΡΑΚΤΙΚΑ
+  2: ΟΠΛΑΡΧΗΓΟΥ ΑΠΟΣΤΟΛΟΥ Γ. ΠΑΠΑΚΩΣΤΑ
+  3: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
+  4: 938.764ΠΑΠ
+  5: '7863'
+  11: '474'
+  12: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
+  13: ΠΑΠΑΚΩΣΤΑΣ ΑΠΟΣΤΟΛΟΣ
+  14: ΟΠΛΑΡΧΗΓΟΣ
 - 0: 6597
   1: ΜΑΡΚΟΥ ΗΛΙΑΣ
   2: ΙΣΤΟΡΙΚΗ ΑΛΗΘΕΙΑ ΔΙΑ ΤΟ ΜΑΚΕΔΟΝΙΚΟΝ
   4: 938.695ΜΑΡ
   5: '5226'
   8: ΑΠΟΣΤΟΛΟΣ ΠΑΥΛΟΣ
   9: ΑΘΗΝΑ
@@ -81871,15 +81870,15 @@
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
 - 0: 6730
   1: Χ.Σ.
   2: ΡΗΓΑΣ ΓΙΑ ΜΙΑ ΝΕΑ ΕΡΕΥΝΗΤΙΚΗ ΣΥΓΚΟΜΙΔΗ
-  4: 949.483ΡΗΓ
+  4: 938.483Χ.Σ
   5: '6822'
   9: ΙΩΑΝΝΙΝΑ
   10: '1998'
   11: 92Σ
   12: ΣΥΝΕΔΡΙΟ-ΡΗΓΑΣ
   13: ΣΥΝΕΔΡΙΟ-ΡΗΓΑΣ
   14: ΣΥΝΕΔΡΙΟ-ΡΗΓΑΣ
@@ -81895,28 +81894,28 @@
   11: 108Σ
   12: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΛΗΣ
   13: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΛΗΣ
   14: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΛΗΣ
 - 0: 6732
   1: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΛΗΣ
   2: ΦΥΣΙΚΗΣ ΑΠΑΝΘΙΣΜΑ
-  4: 949.483ΒΕΛ
+  4: 938.483Χ.Σ
   5: '6828'
   8: ΦΕΡΡΩΝ-ΒΕΛΕΣΤΙΝΟΥ-ΡΗ
   9: ΑΘΗΝΑ
   10: '1991'
   11: 200Σ
   12: ΕΘΝΙΚΟ ΔΙΑΦΩΤΙΣΤΙΚΟ ΕΡΓΟ ΡΗΓΑ
   13: ΕΘΝΙΚΟ ΔΙΑΦΩΤΙΣΤΙΚΟ ΕΡΓΟ ΡΗΓΑ
   14: ΕΘΝΙΚΟ ΔΙΑΦΩΤΙΣΤΙΚΟ ΕΡΓΟ ΡΗΓΑ
 - 0: 6733
   1: Χ.Σ.
   2: ΡΗΓΑ ΒΕΛΕΣΤΙΝΛΗ
   3: ΑΠΑΝΘΙΣΜΑ ΚΕΙΜΕΝΩΝ
-  4: 949.483ΡΗΓ
+  4: 938.483Χ.Σ
   5: '6860'
   9: ΑΘΗΝΑ
   10: '1998'
   11: 158Σ
   12: ΕΠΙΛΟΓΗ ΚΕΙΜΕΝΩΝ ΡΗΓΑ
   13: ΕΠΙΛΟΓΗ ΚΕΙΜΕΝΩΝ ΡΗΓΑ
   14: ΕΠΙΛΟΓΗ ΚΕΙΜΕΝΩΝ ΡΗΓΑ
@@ -82148,15 +82147,15 @@
   11: 31Σ
   12: ΠΥΡΣΟΓΙΑΝΝΗ
   13: ΠΥΡΣΟΓΙΑΝΝΗ
   14: ΠΥΡΣΟΓΙΑΝΝΗ
 - 0: 6754
   1: ΒΟΥΡΝΑΣ,ΤΑΣΟΣ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΩΤΕΡΗΣ ΚΑΙ ΣΥΓΧΡΟΝΗΣ ΕΛΛΑΔΑΣ
-  4: 949.597ΒΟΥ
+  4: 949.7ΒΟΥ
   5: '8884'
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '1999'
   11: 621Σ
   12: ΙΣΤΟΡΙΑ-ΝΕΩΤΕΡΗ-ΣΥΓΧΡΟΝΗ ΕΛΛΑΔΑ
   13: ΙΣΤΟΡΙΑ-ΝΕΩΤΕΡΗ ΣΥΓΧΡΟΝΗ ΕΛΛΑΔΑ
@@ -82465,15 +82464,15 @@
   13: ΗΠΕΙΡΩΤΙΚΟΣ ΓΑΜΟΣ
   14: ΗΠΕΙΡΩΤΙΚΟΣ ΓΑΜΟΣ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 6780
   1: ΑΘΑΝΑΣΙΟΥ,ΘΕΟΦΙΛΟΣ
   2: ΗΜΟΥΝΑ ΚΙ ΕΓΩ ΕΚΕΙ
   3: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
-  4: 938.764ΑΘΑ
+  4: 920ΑΘΑ
   5: '8804'
   9: ΑΘΗΝΑ
   10: '2005'
   11: 286Σ
   12: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
   13: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
   14: ΠΡΟΣΩΠΙΚΕΣ ΜΑΡΤΥΡΙΕΣ
@@ -82793,15 +82792,15 @@
   11: 462Σ
   12: ΒΟΗΘΗΜΑ ΕΚΘΕΣΕΩΝ
   13: ΒΟΗΘΗΜΑ ΕΚΘΕΣΕΩΝ
   14: ΒΟΗΘΗΜΑ ΕΚΘΕΣΕΩΝ
 - 0: 6808
   1: NICOL,DONALD
   2: ΒΙΟΓΡΑΦΙΚΟ ΛΕΞΙΚΟ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
-  4: 998.301NIC
+  4: 938.301NIC
   5: '8951'
   8: ΕΛΛΗΝΙΚΗ ΕΥΡΩΕΚΔΟΤΙΚ
   9: ΑΘΗΝΑ
   10: '1993'
   11: 350Σ
   12: ΒΙΟΓΡΑΦΙΚΟ ΛΕΞΙΚΟ-ΒΥΖΑΝΤΙΝΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
   13: ΒΥΖΑΝΤΙΝΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΚΟ ΛΕΞΙΚΟ
@@ -82912,16 +82911,16 @@
   12: ΦΩΤΟΓΡΑΦΙΚΟ ΛΕΥΚΩΜΑ-ΑΡΤΑ
   13: ΑΡΤΑ-ΦΩΤΟΓΡΑΦΙΚΟ ΛΕΥΚΩΜΑ
   14: ΦΩΤΟΓΡΑΦΙΚΟ ΛΕΥΚΩΜΑ
   15: ΑΡΤΑ
 - 0: 6818
   1: Χ.Σ
   2: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ ΜΑΚΡΥΓΙΑΝΝΗ
-  4: 920.008ΜΑΚ
-  5: '8936'
+  4: 938.478Χ.Σ
+  5: 8936-98
   9: ΑΘΗΝΑ
   10: '1995'
   11: 221Σ
   12: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ-ΜΑΚΡΥΓΙΑΝΝΗΣ
   13: ΜΑΚΡΥΓΙΑΝΝΗΣ-ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
   14: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
   15: ΜΑΚΡΥΓΙΑΝΝΗΣ
@@ -82958,25 +82957,26 @@
   10: '1995'
   11: 208Σ
   12: ΒΥΖΑΝΤΙΝΟΙ ΑΥΤΟΚΡΑΤΟΡΕΣ
   13: ΒΥΖΑΝΤΙΝΟΙ ΑΥΤΟΚΡΑΤΟΡΕΣ
   14: ΒΥΖΑΝΤΙΝΟΙ ΑΥΤΟΚΡΑΤΟΡΕΣ
   17: 3 ΤΟΜΟΙ
 - 0: 6822
-  1: ΚΑΡΑΤΖΕΝΗΣ,ΔΗΜΗΤΡΙΟΣ
-  2: ΠΟΛΙΤΙΚΕΣ ΠΡΟΣΩΠΙΚΟΤΗΤΕΣ ΝΟΜΟΥ ΑΡΤΗΑΣ
-  3: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ ΔΗΜΑΡΧΟΣ-ΒΟΥΛΕΥΤΗΣ
-  4: 920ΚΑΡ
-  5: '8942'
-  9: ΑΘΗΝΑ
-  10: '1983'
-  11: 125Σ
-  12: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ
-  13: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ
-  14: ΕΥΑΓΓΕΛΟΣ ΓΑΡΟΥΦΑΛΙΑΣ
+  1: ΤΟΥΝΤΑ ΧΑΤΖΟΥΔΗ,ΕΛΕΝΗ
+  2: ΤΑΞΙΔΕΥΟΝΤΑΣ ΑΠΟ ΤΗΝ ΑΘΗΝΑ ΣΤΟ ΜΠΙΖΑΝΙ
+  4: 938.93ΤΟΥ
+  5: '22935'
+  9: ΙΩΑΝΝΙΝΑ
+  10: '2012'
+  11: 345Σ
+  12: ΙΣΤΟΡΙΑ-ΜΠΙΖΑΝΙ
+  13: ΜΠΙΖΑΝΙ
+  14: ΙΣΤΟΡΙΑ
+  18: '9789609897'
+  19: '693'
 - 0: 6823
   1: Χ.Σ
   2: ΙΣΤΟΡΙΑ ΔΕΥΤΕΡΟΥ ΠΑΓΚΟΣΜΙΟΥ ΠΟΛΕΜΟΥΙ-ΙΙ
   4: 940.530ΙΣΤ
   5: '8932'
   8: ΠΑΠΥΡΟΣ
   9: ΑΘΗΝΑ
@@ -84010,15 +84010,15 @@
   11: 206Σ
   12: ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ
   14: ΚΥΠΡΟΣ
 - 0: 6906
   1: Χ.Σ.
   2: ΚΥΠΡΟΣ Η ΛΕΗΛΑΣΙΑ ΕΝΟΣ ΠΟΛΙΤΙΣΜΟΥ
-  4: 938.497ΚΥΠ
+  4: 938.497Χ.Σ
   5: '6879'
   8: ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 237Σ
   12: ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ
@@ -84209,28 +84209,28 @@
   11: 78Σ
   12: ΑΙΒΑΛΙ
   13: ΑΙΒΑΛΙ
   14: ΑΙΒΑΛΙ
 - 0: 6922
   1: ΚΑΡΑΘΑΝΑΣΗ,ΑΘΑΝΑΣΙΟ
   2: ΚΑΠΠΑΔΟΚΙΑΣ ΤΥΧΑΙ
-  4: 938.498ΚΑΡ
+  4: 938.392ΚΑΡ
   5: '6823'
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2000'
   11: 109Σ
   12: ΚΑΠΠΑΔΟΚΙΑ
   13: ΚΑΠΠΑΔΟΚΙΑ
   14: ΚΑΠΠΑΔΟΚΙΑ
 - 0: 6923
   1: MURAT,JOHN
   2: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
   3: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
   4: 938.498ΜΟΥ
-  5: 5363-1950
+  5: '5363'
   9: ΑΘΗΝΑ
   10: '1982'
   11: 542Σ
   12: ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
   17: 2 ANTITYΠΑ
@@ -84803,14 +84803,15 @@
   12: ΠΑΤΡΙΑΡΧΕΣ ΒΥΖΑΝΤΙΟΥ
   13: ΠΑΤΡΙΑΡΧΕΣ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ
   14: ΠΑΤΡΙΑΡΧΕΣ
   15: ΒΥΖΑΝΤΙΟΥ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ
 - 0: 6969
   1: ΣΤΑΜΑΤΗΣ,ΕΛΕΥΘΕΡΙΟΣ
   2: ΚΥΡΙΟΙ, ΠΑΤΕ ΓΙΑ ΥΠΝΟ
+  4: 938.799ΣΤΑ
   5: '9011'
   8: ΔΟΥΡΕΙΟΣ ΙΠΠΟΣ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 298Σ
   12: ΤΡΑΓΩΔΙΑΚΥΠΡΟΥ
   13: ΤΡΑΓΩΔΙΑ-ΚΥΠΡΟΣ
@@ -85203,16 +85204,16 @@
   13: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   14: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   15: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 6998
   1: ΛΑΜΠΡΗ,Π.ΠΑΝΑΓΙΩΤΑ
   2: ΡΟΔΑΥΓΗ
-  3: ΤΟ ΡΟΔΟ ΤΗΣ ΑΥΓΗΣ
-  4: ' 938939ΛΑΜ'
+  3: ΤΟ ΡΟΔΟ ΤΗΣ ΑΥΓΗΣ                                          Τ
+  4: 938.939ΛΑΜ
   5: '9037'
   8: ΤΑΧΥΤΥΠΟ
   10: '2006'
   11: 495Σ
   12: ΛΑΟΓΡΑΦΙΑ-ΡΟΔΑΥΓΗ
   13: ΡΟΔΑΥΓΗ-ΛΑΟΓΡΑΦΙΑ
   14: ΡΟΔΑΥΓΗ
@@ -88051,14 +88052,15 @@
   15: ΘΕΑΤΡΟ
   18: 960-90890-
   19: 0-3
 - 0: 7197
   1: MANFREDI,VALERIO MASSIMO
   2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   3: Ο ΓΙΟΣ ΤΟΥ ΟΝΕΙΡΟΥ
+  4: 938.174MAN
   5: '9255'
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '1999'
   11: 224Σ
   12: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
@@ -88066,14 +88068,15 @@
   17: 2 ΤΟΜΟΙ
   18: 960-14-005
   19: 6-7
 - 0: 7198
   1: MANFREDI,VALERIO MASSIMO
   2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   3: Η ΑΜΜΟΣ ΤΟΥ ΑΜΜΩΝΑ
+  4: 938.174MAN
   5: '9256'
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '1999'
   11: 439Σ
   12: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
@@ -88081,14 +88084,15 @@
   17: 2 ΤΟΜΟΙ
   18: 960-14-012
   19: 7-Χ
 - 0: 7199
   1: MANFREDI,VALERIO MASSIMO
   2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   3: ΤΑ ΠΕΡΑΤΑ ΤΟΥ ΚΟΣΜΟΥ
+  4: 938.174MAN
   5: '9257'
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 515Σ
   12: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
@@ -88249,14 +88253,15 @@
   14: ΚΑΤΟΧΗ
   18: 960-224-98
   19: 3-8
 - 0: 7211
   1: IRVING,DAVID
   2: Ο ΠΟΛΕΜΟΣ ΤΩΝ ΣΤΡΑΤΗΓΩΝ
   3: ΣΤΑ ΕΝΔΟΤΕΡΑ ΤΩΝ ΣΥΜΜΑΧΙΚΩΝ ΔΥΝΑΜΕΩΝ 1944-1945
+  4: 938.764IRV
   5: '9169'
   6: ΣΤΕΛΙΟΣ ΧΟΥΡΜΟΥΖΙΑΔΗ
   8: ΙΩΛΚΟΣ
   9: ΑΘΗΝΑ
   10: '2005'
   11: 655Σ
   12: ΠΟΛΕΜΟΣ ΣΤΡΑΤΗΓΩΝ
@@ -88589,26 +88594,27 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
 - 0: 7235
   1: ΧΟΥΤΑ,ΣΤΥΛΙΑΝΟΥ
   2: Η ΜΑΧΗ ΤΟΥ ΜΑΚΡΥΝΟΡΟΥΣ (14-22 ΙΟΥΛΙΟΥ 1943)
+  4: 938.765ΧΟΥ
   5: '9183'
   8: ΣΙΔΕΡΗΣ
   9: ΑΘΗΝΑ
   10: '1983'
   11: 83Σ
   12: ΜΑΚΡΥΝΟΡΟΣ
   13: ΜΑΧΗ ΜΑΚΡΥΝΟΡΟΣ
   14: ΜΑΚΡΥΝΟΡΟΣ
 - 0: 7236
   1: ΣΑΡΑΝΤΗ,ΘΕΟΔΩΡΟΥ
   2: Η ΣΥΝΟΜΩΣΙΑ ΚΑΤΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
-  4: 938,695ΣΑΡ
+  4: 938.695ΣΑΡ
   5: '9182'
   9: ΑΘΗΝΑ
   10: '1984'
   11: 207Σ
   12: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΙΣΤΟΡΙΑ
   14: ΜΑΚΕΔΟΝΙΑ
@@ -89036,15 +89042,15 @@
   13: ΛΕΞΙΚΟ ΚΑΙΝΗΣ ΔΙΑΘΗΚΗΣ
   14: ΛΕΞΙΚΟ ΚΑΙΝΗΣ ΔΙΑΘΗΚΗΣ
   18: 960-400-15
   19: 8-2
 - 0: 7268
   1: ΚΑΜΠΦ,ΜΑΙΝ
   2: Α.ΧΙΤΛΕΡ Ο ΑΓΩΝ ΜΟΥ
-  4: 938.87ΧΙΤ
+  4: 938.87ΚΑΜ
   5: '9178'
   6: ΔΗΜΗΤΡΗΣ ΚΩΣΤΕΛΕΝΟΣ
   8: Δ.ΔΑΡΕΜΑ
   9: ΑΘΗΝΑ
   11: 450Σ
   12: ΧΙΤΛΕΡ
   13: ΧΙΤΛΕΡ
@@ -89132,36 +89138,39 @@
   12: ΑΡΧΑΙΟΛΟΓΙΚΑ-ΔΙΑΤΡΟΦΗ
   13: ΑΡΧΑΙΟΛΟΓΙΚΑ-ΒΙΒΛΙΟΘΗΚΗ
   14: ΑΡΧΑΙΛΟΓΙΚΑ-ΑΞΙΕΣ
 - 0: 7275
   1: ΣΕΡΒΕΤΑ,ΘΕΟΦΙΛΟΥ
   2: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
   3: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
+  4: 938ΣΕΡ
   5: '9274'
   9: ΑΘΗΝΑ
   10: '2002'
   11: 137Σ
   12: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   13: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   14: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
 - 0: 7276
   1: ΣΕΡΒΕΤΑΣ,ΘΕΟΦΙΛΟΣ
   2: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
   3: ΑΡΧΑΙΑ ΡΩΜΗ
+  4: 938ΣΕΡ
   5: '9275'
   9: ΑΘΗΝΑ
   10: '2003'
   11: 130Σ
   12: ΑΡΧΑΙΑ ΡΩΜΗ
   13: ΑΡΧΑΙΑ ΡΩΜΗ
   14: ΑΡΧΑΙΑ ΡΩΜΗ
 - 0: 7277
   1: ΣΕΡΒΕΤΑ,ΘΕΟΦΙΛΟΥ
   2: ΟΨΕΙΣ ΤΟΥ ΑΡΧΑΙΟΥ ΚΟΣΜΟΥ
   3: ΒΥΖΑΝΤΙΟ
+  4: 938ΣΕΡ
   5: '9276'
   9: ΑΘΗΝΑ
   10: '2004'
   11: 154Σ
   12: ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ
   14: ΒΥΖΑΝΤΙΟ
@@ -89418,15 +89427,16 @@
   11: 571Σ
   12: ΙΣΤΟΡΙΑ ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   13: ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   14: ΙΣΤΟΡΙΑ
 - 0: 7297
   1: Χ.Σ.
   2: 1453 Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
-  5: '9293'
+  4: 938.498Χ.Σ
+  5: 9293-12662
   8: NATIONAL GEOGRAPHIC
   11: 127Σ
   12: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
   13: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
   14: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
   18: 978-960-46
   19: 9-076-3
@@ -90817,15 +90827,15 @@
   11: 63Σ
   12: ΕΛΛΗΝΙΣΜΟΣ-ΤΟΥΡΚΟΚΡΑΤΙΑ
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
 - 0: 7403
   1: ΚΑΣΤΡΙΤΗ,ΝΑΤΑΣΑ
   2: Η ΕΛΛΑΔΑ ΤΟΥ 21 ΜΕ ΤΗ ΜΑΤΙΑ ΤΩΝ ΦΙΛΕΛΛΗΝΩΝ
-  4: 949.506ΚΑΣ
+  4: 938.5ΚΑΣ
   5: '9420'
   8: ΙΣΤ.ΕΘΝ.ΕΤΑΙΡ.ΕΛΛΑΔΟ
   9: ΑΘΗΝΑ
   10: '2006'
   11: 145ΣΕΛ
   12: ΙΣΤΟΡΙΑ-ΦΙΛΕΛΛΗΝΕΣ
   13: ΦΙΛΕΛΛΗΝΕΣ-ΙΣΤΟΡΙΑ
@@ -90888,22 +90898,23 @@
   9: ΑΘΗΝΑ
   10: '1983'
   11: 440Σ
   12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
   14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
 - 0: 7408
-  1: Χ.Σ.
-  2: ΕΜΠΡΟΣ ΤΗΣ ΕΛΛΑΔΟΣ ΤΑ ΠΑΙΔΙΑ
-  3: ΧΡΟΝΙΚΟΝ 1940-1944
-  4: 938.752Χ.Σ
-  5: 9295Α
+  1: ΒΙΔΑΛΗΣ,ΟΡΕΣΤΗΣ
+  2: ΙΣΤΟΡΙΚΟ ΗΜΕΡΟΛΟΓΙΟ
+  3: ΧΡΟΝΙΑ ΕΚΠΑΤΡΙΣΜΟΥ 1968-1975
+  4: 938.790ΒΙΔ
+  5: 4288,4292
+  8: LIBRO
   9: ΑΘΗΝΑ
-  10: '1978'
-  11: 376Σ
+  10: '1997'
+  11: '570'
   12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
   14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
 - 0: 7409
   1: Χ.Σ.
   2: ΜΕΓΑΛΗ ΕΛΛΑΔΑ
   3: ΠΕΡΙΟΔΟΣ 1944-1945
@@ -91019,15 +91030,15 @@
   13: ΒΑΛΚΑΝΙΚΟΙ ΠΟΛΕΜΟΙ-ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   15: ΒΑΛΚΑΝΙΚΟΙ ΠΟΛΕΜΟΙ
 - 0: 7417
   1: Χ.Σ.
   2: ΤΟ ΕΠΟΣ ΤΟΥ 40
   3: ΛΑΙΚΗ ΕΙΚΟΝΟΓΡΑΦΙΑ
-  4: 938.752Σ
+  4: 938.752Χ.Σ
   5: '9416'
   8: ΙΣΤ.ΕΘΝ.ΕΤ.ΕΛΛΑΔΟΣ
   9: ΑΘΗΝΑ
   10: '1987'
   11: 217Σ
   12: ΙΣΤΟΡΙΑ-ΕΠΟΣ 40
   13: ΕΠΟΣ 40-ΙΣΤΟΡΙΑ
@@ -91844,15 +91855,15 @@
   10: '1969'
   11: 61Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 7482
   1: Χ.Σ
   2: ΑΥΤΟΒΙΟΓΡΑΦΙΑ ΙΩΑΝΝΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
-  4: 889Χ.Σ
+  4: 938.571Χ.Σ
   5: '9953'
   7: 3Η
   8: ΓΑΛΑΞΙΑΣ
   9: ΑΘΗΝΑ
   10: '1971'
   11: 172Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΥΤΟΒΙΟΓΡΑΦΙΑ
@@ -92441,14 +92452,15 @@
   14: ΕΛΛΗΝΙΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
 - 0: 7533
   1: Χ.Σ
   2: ΤΟ ΑΙΩΝΙΟΝ ΖΗΤΗΜΑ
   3: ΤΟ ΑΝΑΤΟΛΙΚΟΝ ΖΗΤΗΜΑ
+  4: 938.652Χ.Σ
   5: '10077'
   8: ΕΚΔΟΣΕΙΣ ΜΠΕΡΓΑΔΗ
   9: ΑΘΗΝΑ
   11: 262Σ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
 - 0: 7534
   1: ΑΒΡΑΑΜ ΚΩΣΤΑΣ
@@ -93230,20 +93242,25 @@
   2: ΟΙΚΟΝΟΜΙΚΟΝ ΔΙΚΑΙΟΝ
   5: '10046'
   9: ΑΘΗΝΑ
   10: '1960'
   11: 16Σ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
 - 0: 7622
-  1: ΚΑΣΙΜΑΤΗΣ ΓΡΗΓΟΡΗΣ
-  2: ΠΑΙΔΕΣ ΕΛΛΗΝΩΝ ΙΤΕ
-  5: '10043'
-  9: ΑΘΗΝΑ
-  10: '1972'
-  17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
+  1: ΨΗΜΜΕΝΟΥ,ΝΙΚΟΥ
+  2: ΕΡΜΗΝΕΥΤΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ
+  4: 199.495ΨΗΜ
+  5: '21494'
+  8: ΔΩΤΙΟΝ
+  9: ΙΩΑΝΝΙΝΑ
+  10: '2019'
+  11: '100'
+  12: ΠΟΙΗΣΗ
+  13: ΙΣΤΟΡΙΚΑ ΚΑΙ ΚΡΙΤΙΚΗ
+  14: ΔΙΑΤΡΙΒΗ
 - 0: 7623
   1: ΖΑΚΑΣ ΠΑΝΟΣ
   2: ΝΟΜΟΘΕΣΙΑ ΤΩΝ ΔΗΜΟΣΙΩΝ ΕΡΓΩΝ
   5: '10041'
   8: ΜΑΡΖΕΛΟΣ
   9: ΜΥΤΙΛΗΝΗ
   10: '1937'
@@ -93383,23 +93400,24 @@
   5: '10051'
   8: ΡΟΔΗΣ
   9: ΑΘΗΝΑ
   10: '1967'
   11: 172Σ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
 - 0: 7640
-  1: ΡΗΓΑΣ.ΓΙΩΡΓΟΣ. ΣΚΟΥΤΕΛΑΣ
+  1: ΣΚΟΥΤΕΛΑΣ,ΡΗΓΑΣ
   2: ΘΕΟΔΩΡΙΑΝΑ ΑΡΤΑΣ
-  4: '938.939'
+  4: 938.939ΣΚΟ
   5: '10129'
   9: ΑΘΗΝΑ
   10: '1994'
   11: 638Σ
-  12: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
-  13: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
+  12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
+  13: ΘΕΟΔΩΡΙΑΝΑ
+  14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 7641
   1: ΜΑΚΡΗΣ. ΕΥΡΙΠΙΔΗΣ
   2: ΖΩΗ ΚΑΙ ΠΑΡΑΔΟΣΗ ΤΩΝ ΣΑΡΑΚΑΤΣΑΝΑΙΩΝ
   4: 398ΜΑΚ
   5: '10150'
@@ -93421,23 +93439,23 @@
   11: 245Σ
   12: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
   17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
 - 0: 7643
   1: Χ.Σ
   2: ΑΚΡΙΤΙΚΟΣ ΑΛΥΤΡΩΤΟΣ ΑΠΟΔΗΜΟΣ ΕΛΛΗΝΙΣΜΟΣ
-  4: 398Χ.Σ.
+  4: 938.695Χ.Σ
   5: 8053-10128
   8: ΚΥΡΙΑΚΙΔΗΣ
   9: ΒΕΡΟΙΑ
   10: '1996'
   11: 234Σ
-  12: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
-  13: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
-  14: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
+  12: ΕΛΛΗΝΙΣΜΟΣ
+  13: ΕΛΛΗΝΙΣΜΟΣ
+  14: ΕΛΛΗΝΙΣΜΟΣ
   17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
   30: 3 ΑΝΤΙΤΥΠΑ
 - 0: 7644
   1: ΚΑΛΟΥΣΙΟΣ. ΔΗΜΗΤΡΙΟΣ
   2: ΤΟ ΜΑΤΣΟΥΚΙ ΙΩΑΝΝΙΝΩΝ
   4: 398ΚΑΛ
   5: '10125'
@@ -93548,15 +93566,15 @@
   11: 176Σ
   12: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
   17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
   30: ΤΟΜΟΣ Α-ΤΟΜΟΣ Β(2 ΑΝΤΙΤΥΠΑ)
 - 0: 7655
   1: ΜΕΛΙΚΗΣ. ΓΙΩΡΓΗΣ
-  2: ΤΑ ΛΑΟΓΡΑΦΙΚΣ ΤΗΣ ΜΕΛΙΚΗΣ
+  2: ΤΑ ΛΑΟΓΡΑΦΙΚΑ ΤΗΣ ΜΕΛΙΚΗΣ
   4: 398ΜΕΛ
   5: 10151-8079
   9: ΜΕΛΙΚΗ
   11: 220Σ
   12: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΑΟΓΡΑΦΙΑ
   17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
@@ -93660,15 +93678,15 @@
   10: '2001'
   11: 140Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ Ν. ΛΙΟΝΤΟΥ
 - 0: 7665
   1: Χ.Σ
-  2: ΠΟΙΗΤΙΚΗ ΑΝΘΟΛΟΓΙΑΔΙΟΝΥΣΙΟΣ ΣΟΛΩΜΟΣ
+  2: ΠΟΙΗΤΙΚΗ ΑΝΘΟΛΟΓΙΑ ΔΙΟΝΥΣΙΟΣ ΣΟΛΩΜΟΣ
   4: 880.08Χ.Σ
   5: '8519'
   8: ΜΑΛΛΙΑΡΗΣ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1976'
   11: 300Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
@@ -94232,23 +94250,24 @@
   9: ΘΕΣ/ΝΙΚΗ
   10: '2008'
   11: 235Σ
   12: ΙΣΤΟΡΙΚΑ ΚΕΙΜΕΝΑ
   13: ΙΣΤΟΡΙΚΑ ΚΕΙΜΕΝΑ
   17: ΔΩΡΕΑ ΓΙΩΡΓΟΥ ΨΩΜΑ
 - 0: 7713
-  1: ΤΟΥΤΣΙΝΟΣ ΓΙΑΝΝΗΣ
+  1: ΤΣΟΥΤΣΙΝΟΣ ΓΙΑΝΝΗΣ
   2: ΑΡΤΙΝΑ ΙΣΤΟΡΙΚΑ ΘΕΜΑΤΑ
   4: 938.939ΤΟΥ
   5: '4420'
   9: ΑΡΤΑ
   10: '2001'
   11: 265Σ
-  12: ΙΣΤΟΡΙΚΑ
+  12: ΑΡΤΙΝΑ ΘΕΜΑΤΑ
   13: ΙΣΤΟΡΙΚΑ
+  14: ΑΡΤΑ
   17: ΔΩΡΕΑ ΓΙΩΡΓΟΥ ΨΩΜΑ
 - 0: 7714
   1: ΣΤΟΥΚΑΣ ΓΕΩΡΓΙΟΣ
   2: ΑΡΧΑΙΟΣ ΕΛΛΗΝΙΚΟΣ ΠΟΛΙΤΙΣΜΟΣ
   4: 938.1ΣΤΟ
   5: 10213-10214-9555-955
   6: '4'
@@ -94383,15 +94402,15 @@
   9: ΝΑΥΠΑΚΤΟΣ
   10: '2001'
   11: 115Σ
   12: ΘΡΗΣΚΕΥΤΙΚΑ
   13: ΘΡΗΣΚΕΥΤΙΚΑ
   17: ΔΩΡΕΑ ΕΛΕΝΗΣ ΜΑΝΙΚΑ
 - 0: 7726
-  1: ΕΛΕΝΗ ΚΑΡΙΤΑ
+  1: ΚΑΡΙΤΑ,ΕΛΕΝΗ
   2: Η ΜΟΡΦΗ ΜΙΑΣ ΑΓΙΑΣ
   4: 230ΚΑΡ
   5: '10251'
   8: Ι. ΜΗΤΡ.ΧΑΛΚΙΔΟΣ
   10: '1973'
   11: 219Σ
   12: ΘΡΗΣΚΕΥΤΙΚΑ
@@ -94485,15 +94504,15 @@
   9: ΑΘΗΝΑ
   10: '1993'
   11: 99Σ
   12: ΘΡΗΣΚΕΥΤΙΚΑ
   13: ΘΡΗΣΚΕΥΤΙΚΑ
   17: ΔΩΡΕΑ ΕΛΕΝΗΣ ΜΑΝΙΚΑ
 - 0: 7735
-  1: ΧΑΡΑΛΑΜΠΙΔΗΣ ΓΡΗΓΟΡΙΟΣ
+  1: ΧΑΡΑΛΑΜΠΙΔΗΣ,ΓΡΗΓΟΡΙΟΣ
   2: ΤΟ ΣΑΡΑΚΙ ΤΗΣ ΨΥΧΗΣ
   4: 230ΧΑΡ
   5: '10241'
   7: 9Η
   8: Ο ΣΩΤΗΡ
   9: ΑΘΗΝΑ
   10: '2003'
@@ -101124,16 +101143,16 @@
   10: '2007'
   11: 416Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 8285
   1: ΣΧΙΣΜΕΝΟΣ ΑΡΙΣΤΕΙΔΗΣ
   2: ΜΥΘΟΙ ΚΑΙ ΠΑΡΑΔΟΣΕΙΣ ΜΝΗΜΕΙΩΝ ΚΑΙ ΤΟΠΟΘΕΣΙΩΝ ΤΟΥ ΝΟΜΟΥ ΑΡΤΑΣ
-  4: 398 ΣΧΙ
-  5: '9589'
+  4: 938.939ΣΧΙ
+  5: 9589-16177
   8: ΥΔΡΟΓΕΙΟΣ
   9: ΘΕΣ\ΝΙΚΗ
   10: '2009'
   11: 369Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
@@ -103011,15 +103030,15 @@
   11: 102Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
 - 0: 8438
   1: Χ.Σ
   2: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΗΣ
-  4: 398.483ΡΗΓ
+  4: 938.483ΡΗΓ
   5: '9422'
   9: ΑΘΗΝΑ
   10: '1998'
   11: 141Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
 - 0: 8439
@@ -103028,39 +103047,46 @@
   4: 938.498ΚΑΡ
   5: '9889'
   6: ΚΟΥΝΕΖΗ
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2006'
   11: 318Σ
+  12: ΙΣΤΟΡΙΑ-ΣΜΥΡΝΗ
+  13: ΙΣΤΟΡΙΑ-ΣΜΥΡΝΗ
+  14: ΣΜΥΡΝΗ-ΙΣΤΟΡΙΑ
 - 0: 8440
   1: ΤΖΑΝΑΚΑΡΗΣ ΒΑΣΙΛΗΣ
   2: ΣΤΟ ΟΝΟΜΑ ΤΗΣ ΠΡΟΣΦΥΓΙΑΣ
   4: 938.498ΤΖΑ
   5: '9890'
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2009'
   11: 575Σ
+  12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+  13: ΙΣΤΟΡΙΑ-ΣΜΥΡΝΗ
+  14: ΙΣΤΟΡΙΑ
+  15: ΠΟΝΤΟΣ-ΣΜΥΡΝΗ
 - 0: 8441
   1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ ΝΙΚΟΣ
   2: ΥΠΕΡ ΒΩΜΩΝ ΚΑΙ ΕΣΤΙΩΝ
   4: 938.764ΠΑΠ
   5: '9668'
   9: ΑΘΗΝΑ
   10: '2003'
   11: 159Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
 - 0: 8442
-  1: ΑΘΑΝΑΣΑΚΗ ΑΝΤΩΝΙΟΥ
+  1: ΑΘΑΝΑΣΑΚΗ,ΑΝΤΩΝΙΟΥ
   2: ΠΕΡΙΛΗΠΤΙΚΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ
   3: ΑΠΟ ΤΟ 1897 ΜΕΧΡΙ ΤΟ 1940-41
-  4: '938.764'
+  4: 938.764ΑΘΑ
   5: '9659'
   8: ΠΕΤΡΑ
   9: ΑΘΗΝΑ
   10: '2010'
   11: 141Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
@@ -103123,31 +103149,40 @@
   1: ΑΡΚΑΔΙΝΟΣ ΠΟΛΙΒΙΟΣ
   2: Η ΕΣΩΤΕΡΙΚΗ ΚΡΙΣΙΣ ΤΟΥ Κ.Κ.Ε
   4: 938.8ΑΡΚ
   5: '9839'
   9: ΑΘΗΝΑ
   10: '1954'
   11: 136Σ
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
 - 0: 8449
   1: ΔΗΜΟΣ ΤΑΣΟΣ
   2: ΕΝΑ ΓΑΡΥΦΑΛΛΟ ΠΟΥ ΔΕΝ Τ ΑΦΗΝΟΥΝ Ν ΑΝΘΙΣΕΙ
-  4: '938.8'
+  4: 938.8ΔΗΜ
   5: '4350'
   8: ΓΛΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1982'
   11: 98Σ
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
 - 0: 8450
   1: ΛΑΜΠΡΙΝΙΔΗΣ ΜΗΝΑΣ
   2: Η ΑΛΒΑΝΙΑ ΣΗΜΕΡΑ
-  4: '941.2'
+  4: 941.2ΛΑΜ
   5: '5372'
   9: ΑΘΗΝΑ
   10: '1987'
   11: 173Σ
+  12: ΑΛΒΑΝΙΑ
+  13: ΑΛΒΑΝΙΑ
+  14: ΑΛΒΑΝΙΑ
 - 0: 8451
   1: Χ.Σ.
   2: Η ΚΟΙΝΟΠΟΛΙΤΕΙΑ ΕΝ ΣΥΝΤΟΜΙΑ
   4: 973 Χ.Σ
   5: '6728'
   10: '1968'
   11: 45Σ
@@ -103229,15 +103264,15 @@
   11: 79Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
 - 0: 8460
   1: ΛΙΧΤΧΑΙΜ ΤΖΩΡΤΖ
   2: ΣΥΝΤΟΜΗ ΠΑΓΚΟΣΜΙΑ ΙΣΤΟΡΙΑ ΤΟΥ ΣΟΣΙΑΛΙΣΜΟΥ
-  4: 938.8 ΛΙΧ
+  4: 938.8ΛΙΧ
   5: '10662'
   6: ΚΩΣΤΕΛΕΝΙΟΣ
   8: ΓΛΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1976'
   11: 409Σ
   12: ΙΣΤΟΡΙΑ
@@ -103322,29 +103357,29 @@
   9: ΑΘΗΝΑ
   10: '2008'
   11: 371Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 8470
-  1: ΚΕΛΑΙΔΗ ΠΑΡΙ
+  1: ΚΕΛΑΙΔΗ,ΠΑΡΙ
   2: ΚΡΗΤΙΚΟΙ ΕΘΕΛΟΝΤΕΣ ΣΤΟΥΣ ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΥΣ ΠΟΛΕΜΟΥΣ 1912-13
-  4: '938.655'
+  4: 938.655ΚΕΛ
   5: '10686'
   8: ΚΑΡΑΒΙ ΚΑΙ ΤΟΞΟ
   9: ΑΘΗΝΑ
   10: '1995'
   11: 295Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
 - 0: 8471
   1: ΤΟΚΒΙΛ ΑΛΕΞΗΣ
   2: Η ΔΗΜΟΚΡΑΤΙΑ ΣΤΗΝ ΑΜΕΡΙΚΗ
-  4: 970 ΤΟΚ
+  4: 970ΤΟΚ
   5: '9303'
   8: ΣΤΟΧΑΣΤΗΣ
   9: ΑΘΗΝΑ
   10: '1997'
   11: 722Σ
 - 0: 8472
   1: ΜΑΛΑΜΑΣ ΛΑΜΠΡΟΣ
@@ -103381,30 +103416,37 @@
   11: 96Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8475
   1: ΣΠΗΛΙΟΣ ΑΠΟΣΤΟΛΟΣ
   2: ΠΕΛΑΣΓΙΚΗ ΗΠΕΙΡΟΣ ΚΑΙ ΑΡΑΧΘΟΣ Ο ΠΕΛΑΣΓΙΚΟΣ
-  3: '                                                           9'
   4: 938.21ΣΠΗ
-  5: '9335'
+  5: 9335-17184
   8: ΘΕΣΙΣ
   9: ΑΘΗΝΑ
   10: '2002'
   11: 135Σ
+  12: ΗΠΕΙΡΟΣ-ΑΡΑΧΘΟΣ
+  13: ΙΣΤΟΡΙΑ
+  14: ΑΡΑΧΘΟΣ
+  15: ΗΠΕΙΡΟΣ
 - 0: 8476
   1: ΒΑΚΑΛΟΠΟΥΛΟΣ ΚΩΝΣΤΑΝΤΙΝΟΣ
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΒΟΡΕΙΟΥ ΕΛΛΗΝΙΣΜΟΥ ΘΡΑΚΗ
   4: 938.695ΒΑΚ
   5: '9305'
   8: ΚΥΡΙΑΚΙΗΣ
   9: ΘΕΣ\ΝΙΚΗ
   10: '1993'
   11: 567Σ
+  12: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
+  13: ΘΡΑΚΗ
+  14: ΙΣΤΟΡΙΑ
+  15: ΒΟΡΕΙΟΣ ΕΛΛΗΝΙΣΜΟΣ
 - 0: 8477
   1: ΛΑΖΑΝΑΣ ΒΑΣΙΛΗΣ
   2: Η ΑΝΘΟΛΟΓΙΑ ΑΡΧΑΙΩΝ ΕΛΛΗΝΙΚΩΝ ΕΠΙΓΡΑΜΜΑΤΩΝ ΤΟΥ ΜΑΞΙΜΟΥ ΠΛΑΝΟ
   3: ΥΔΗ
   4: 809 ΛΑΖ
   5: '10680'
   8: ΠΑΠΑΔΗΜΑ
@@ -104228,17 +104270,17 @@
   11: '121'
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-7198-1
   19: 0-7
 - 0: 8537
-  1: ΕΝΙΝΤ,ΜΠΛΑΙΤΟΝ
+  1: ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
   2: ΤΟ ΒΙΒΛΙΟ ΜΕ ΤΙΣ ΝΕΡΑΙΔΕΣ
-  4: 808.899ΕΝΙ
+  4: 808.899ΜΠΛ
   5: '10818'
   6: ΜΙΡΚΑ ΚΟΝΔΑΚΗ
   7: 2η εκδ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '1996'
   11: '216'
@@ -113199,16 +113241,16 @@
   11: '159'
   12: ΙΣΤΟΡΙΑ-ΕΜΦΥΛΙΟΣ
   13: ΙΣΤΟΡΙΑ-ΕΜΦΥΛΙΟΣ
   14: ΙΣΤΟΡΙΚΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9157
   1: SCHMINCK-GUSTAVUS CHRISTOPH U.
-  2: ΕΛΛΗΝΕΣ ΚΡΑΤΟΥΜΕΝΟΙ ΚΙΑ Ο ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
-  4: 938.764CUS
+  2: ΕΛΛΗΝΕΣ ΚΡΑΤΟΥΜΕΝΟΙ ΚAI Ο ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
+  4: 938.764GUS
   5: '11528'
   8: ΦΙΛΙΣΤΩΡ
   9: ΑΘΗΝΑ
   10: '2004'
   11: '203'
   12: ΙΣΤΟΡΙΚΑ-ΚΑΤΟΧΗ
   13: ΙΣΤΟΡΙΚΑ-ΚΑΤΟΧΗ
@@ -113849,15 +113891,15 @@
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
   18: 960-03-178
   19: 0-1
 - 0: 9204
-  1: ΑΒΔΟΥΛΟΣ,ΣΤΑΥΡΟΑ
+  1: ΑΒΔΟΥΛΟΣ,ΣΤΑΥΡΟΣ
   2: ΝΙΚΟΣ ΖΑΧΑΡΙΑΔΗΣ
   3: ΜΥΘΟΣ ΚΑΙ ΠΡΑΓΜΑΤΙΚΟΤΗΤΑ
   4: 938.764ΑΒΔ
   5: '11490'
   8: ΠΑΡΑΣΚΗΝΙΟ
   9: ΑΘΗΝΑ
   10: '2009'
@@ -117758,26 +117800,27 @@
   9: ΑΘΗΝΑ
   11: 363Σ
   12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9488
-  1: ΜΠΑΣΤΑΝΗΣ,ΠΑΝΑΓΙΩΤΗΣ
-  2: ΤΟ ΤΡΕΝΟ ΤΟΥ ΦΩΤΟΣ
-  4: 889.21ΜΠΑ
-  5: '11773'
-  8: ΔΩΔΩΝΗ
+  1: ΛΑΡΣΟΝ,ΟΣΑ
+  2: PAX ΤΟ ΦΑΝΤΑΣΜΑ
+  4: 808.899ΛΑΡ
+  5: '22602'
+  8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
-  10: '1991'
-  11: 724Σ
-  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-  14: ΛΟΓΟΤΕΧΝΙΑ
-  17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
+  10: '2018'
+  11: '215'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  19: '9786180124'
+  22: 095
 - 0: 9489
   1: DAVIES,PAUL
   2: ΕΙΜΑΣΤΕ ΜΟΝΟΙ;
   4: 574.999DAV
   5: '11777'
   8: ΚΑΤΟΠΡΟ
   9: ΑΘΗΝΑ
@@ -118922,15 +118965,15 @@
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9574
   1: ΠΡΙΑΜΟΣ
   2: ΜΕ ΤΟ 7ο ΣΥΝΤΑΓΜΑ ΤΟΥ ΕΛΑΣ ΣΤΑ ΒΟΥΝΑ ΤΗΣ ΕΥΒΟΙΑΣ
-  4: 938.764ΠΡΙ
+  4: 938.764Χ.Σ
   5: '11817'
   9: ΑΘΗΝΑ
   11: 136Σ
   12: ΙΣΤΟΡΙΑ-ΕΜΦΥΛΙΟΣ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
@@ -119247,15 +119290,15 @@
   13: ΙΣΤΟΡΙΑ-ΜΑΚΡΟΝΗΣΟΣ
   14: ΜΑΚΡΟΝΗΣΟΣ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
   30: Α ΤΟΜΟΣ
 - 0: 9599
   1: ΠΑΠΑΙΩΑΝΝΟΥ,ΑΧΙΛΛΕΑΣ
   2: Η ΑΠΑΓΟΡΕΥΜΕΝΗ ΕΙΚΟΝΑ
-  4: 938.77ΠΑΠ
+  4: 938.764ΠΑΠ
   5: '11891'
   8: ΦΙΛΙΣΤΩΡ
   9: ΑΘΗΝΑ
   10: '2001'
   11: 208Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
@@ -119995,16 +120038,16 @@
   14: ΠΟΛΙΤΙΚΗ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
   18: 960-86296-
   19: 8-3
 - 0: 9649
   1: Χ.Σ.
   2: ΠΕΡΙ ΠΕΤΡΟΓΕΦΥΡΩΝ..
-  4: 624.609ΠΡΑ
-  5: '11920'
+  4: 938.939Χ.Σ
+  5: 11920-8656
   8: ΚΕ.ΜΕ.ΠΕ.Γ
   9: ΑΘΗΝΑ
   10: '2005'
   11: 414Σ
   12: ΓΕΦΥΡΕΣ-ΠΕΤΡΙΝΕΣ-ΗΠΕΙΡΟΣ
   13: ΓΕΦΥΡΕΣ-ΤΟΞΟΕΙΔΕΣ-ΗΠΕΙΡΟΣ
   14: ΓΕΦΥΡΕΣ-ΗΠΕΙΡΟΣ
@@ -120059,17 +120102,17 @@
   10: '1987'
   11: 289Σ
   12: ΜΙΚΡΟΦΥΣΙΚΗ
   13: ΜΙΚΡΟΦΥΣΙΚΗ
   14: ΜΙΚΡΟΦΥΣΙΚΗ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9654
-  1: ΠΡΑΚΤΙΚΑ
+  1: Χ.Σ
   2: ΟΙ ΔΙΚΕΣ ΤΗΣ ΧΟΥΝΤΑΣ
-  4: 938.79ΠΡΑ
+  4: 938.79Χ.Σ
   5: '11916'
   11: 210Σ
   12: ΙΣΤΟΡΙΑ-ΧΟΥΝΤΑ
   13: ΧΟΥΝΤΑ
   14: ΧΟΥΝΤΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9655
@@ -121195,27 +121238,27 @@
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9738
   1: Χ.Σ
   2: ΠΟΛΗ 1955
   3: Η ΤΕΛΕΥΤΑΙΑ ΑΛΩΣΗ
   4: 938.498Χ.Σ
-  5: '12047'
+  5: 12047-14151
   8: ΤΕΓΟΠΟΥΛΟΣ
   9: ΑΘΗΝΑ
   11: 192Σ
   12: ΙΣΤΟΡΙΑ-ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
   13: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
   14: ΑΛΩΣΗ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9739
   1: Χ.Σ
   2: ΔΕΚΕΜΒΡΗΣ 44
   3: ΟΙ ΜΑΧΕΣ ΣΤΙΣ ΓΕΙΤΟΝΙΕΣ ΤΗΣ ΑΘΗΝΑΣ
-  4: 938.771Χ.Σ
+  4: 938.764Χ.Σ
   5: '12046'
   8: ΤΕΓΟΠΟΥΛΟΣ
   9: ΑΘΗΝΑ
   11: 192Σ
   12: ΙΣΤΟΡΙΑ-ΔΕΚΕΜΒΡΙΑΝΑ
   13: ΙΣΤΟΡΙΑ-ΔΕΚΕΜΒΡΙΑΝΑ
   14: ΔΕΚΕΜΒΡΙΑΝΑ
@@ -121411,17 +121454,17 @@
   10: '2007'
   11: 304Σ
   12: ΚΟΚ
   13: ΚΟΚ
   14: ΚΟΚ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9755
-  1: ΜΠΕΛΟΓΙΑΝΝΗ
+  1: Χ.Σ
   2: ΟΙ ΜΕΓΑΛΕΣ ΔΙΚΕΣ
-  4: 938.764ΜΠΕ
+  4: 938.764Χ.Σ
   5: '12033'
   8: ΦΩΤΟΕΚΔΟΤΙΚΗ
   9: ΑΘΗΝΑ
   10: '2011'
   11: 207Σ
   12: ΙΣΤΟΡΙΑ-ΜΠΕΛΟΓΙΑΝΝΗΣ
   13: ΜΠΕΛΟΓΙΑΝΝΗΣ-ΔΙΚΗ
@@ -122265,17 +122308,17 @@
   12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
   18: 978-960-83
   19: 59-37-6
 - 0: 9822
-  1: ΑΝΤΥΠΑΣ,ΣΤΑΥΡΟΣ
+  1: Χ.Σ
   2: ΝΟΕΜΒΡΗΣ ΗΤΑΝ,ΟΙ ΧΡΟΝΙΕΣ..1973-2003
-  4: 938.79ΑΝΤ
+  4: 938.79Χ.Σ
   5: '12123'
   8: ΓΡΑΦΕΣ
   9: ΑΘΗΝΑ
   10: '2003'
   11: 173Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΛΥΤΕΧΝΕΙΟ
   13: ΠΟΛΥΤΕΧΝΕΙΟ
@@ -122392,15 +122435,15 @@
   13: ΛΕΥΚΩΜΑ
   14: ΛΕΥΚΩΜΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 9832
   1: ΠΡΑΚΤΙΚΑ ΕΚΔΗΛΩΣΗΣ
   2: 40 ΧΡΟΝΙΑ
   3: ΜΑΗΣ 68
-  4: 938.79ΠΡΑ
+  4: 938.79Χ.Σ
   5: '12096'
   8: ΜΙΛΗΤΟΣ
   9: ΑΘΗΝΑ
   11: 331Σ
   12: ΙΣΤΟΡΙΑ-ΠΡΑΞΙΚΟΠΗΜΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
@@ -126784,32 +126827,34 @@
   11: 187Σ
   12: ΙΣΤΟΡΙΑ-ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ-ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   18: 978-960-78
   19: 15-24-8
 - 0: 10227
-  1: ΔΑΡΔΑΒΕΣΗΣ,ΘΕΟΔΩΡΟΥ
+  1: Χ.Σ
   2: ΓΕΡΜΑΝΙΚΗ ΚΑΤΟΧΗ
   3: ΙΣΤΟΡΙΕΣ ΑΠΟ ΤΑ ΣΥΣΣΙΤΙΑ ΣΤΗ ΦΙΛΟΠΤΩΧΟ ΑΔΕΛΦΟΤΗΤΑ ΑΝΔΡΩΝ ΘΕΣ
-  4: 938.764ΔΑΡ
+  4: 938.764Χ.Σ
   5: '12511'
   8: ΦΑΑΘ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2012'
   11: 150Σ
   12: ΙΣΤΟΡΙΑ-ΚΑΤΟΧΗ
   13: ΙΣΤΟΡΙΑ-ΚΑΤΟΧΗ
   14: ΓΕΡΜΑΝΙΚΗ ΚΑΤΟΧΗ
   18: 978-960-96
   19: 94-06-3
 - 0: 10228
   1: ΒΑΣΙΛΑΚΗΣ,ΧΡΗΣΤΟΣ
   2: ΤΟ ΑΙΜΑ ΤΩΝ ΜΑΡΤΥΡΩΝ
   3: ΤΟ ΚΟΜΜΕΝΟ ΣΤΑ ΧΡΟΝΙΑ ΤΗΣ ΓΕΡΜΑΝΙΚΗΣ ΚΑΤΟΧΗΣ
+  4: 938.939ΒΑΣ
+  5: '12512'
   8: ΓΡΗΓΟΡΗ
   9: ΑΘΗΝΑ
   10: '2012'
   11: 327Σ
   12: ΙΣΤΟΡΙΑ-ΚΟΜΜΕΝΟ
   13: ΚΟΜΜΕΝΟ-ΚΑΤΟΧΗ
   14: ΙΣΤΟΡΙΑ
@@ -127437,15 +127482,15 @@
   14: ΘΡΗΣΚΕΙΑ
   15: ΑΠΟΣΤΟΛΟΣ ΠΑΥΛΟΣ
   18: 978-618-80
   19: 066-1-4
 - 0: 10274
   1: Χ.Σ.
   2: ΜΙΚΡΑΣΙΑΤΙΚΗ ΚΑΤΑΣΤΡΟΦΗ
-  3: ΤΙ ΕΦΤΕΙΞΕ
+  3: ΤΙ ΕΦΤΑΙΞΕ
   4: 938.498Χ.Σ
   5: '12629'
   8: ΕΛΕΥΘΕΡΟΣ ΤΥΠΟΣ
   9: ΑΘΗΝΑ
   11: 160Σ
   12: ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
   13: ΜΙΚΡΑΣΙΑΤΙΚΗ ΚΑΤΑΣΤΡΟΦΗ
@@ -130131,15 +130176,15 @@
   17: ΔΩΕΡΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-54
   19: 2-2
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10451
   1: ΣΑΜΟΥΗΛΙΔΗΣ,ΧΡΗΣΤΟΣ
   2: ΑΜΙΣΟΣ (ΣΑΜΨΟΥΝΤΑ) ΚΑΙ Η ΠΕΡΙΦΕΡΕΙΑ ΤΗΣ
-  4: 938.993ΣΑΜ
+  4: 938.498ΣΑΜ
   5: '13033'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2004'
   11: 187Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130147,15 +130192,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-77
   19: 8-6
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10452
   1: ΤΣΙΡΟΖΗΣ-ΤΣΙΡΟΖΙΔΗΣ,ΣΤΑΥΡΟΣ
   2: ΤΟ ΧΩΡΙΟ ΜΟΥ ΤΣΙΤΑ ΣΤΑ ΣΟΥΡΜΕΝΑ ΤΟΥ ΠΟΝΤΟΥ
-  4: 938.993ΤΣΙ
+  4: 938.498ΤΣΙ
   5: '13032'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2000'
   11: 176Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130163,15 +130208,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-56
   19: 0-0
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10453
   1: ΜΠΑΚΑΛΑΚΗ-ΕΜΠΕΟΓΛΟΥ,ΕΥΔΟΚΙΑ
   2: Η ΑΜΑΣΕΙΑ
-  4: 938.993ΜΠΑ
+  4: 938.498ΜΠΑ
   5: '13031'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1988'
   11: 176Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130191,15 +130236,15 @@
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10455
   1: ΚΥΝΗΓΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ
   2: ΠΑΦΡΑ ΤΟΥ ΠΟΝΤΟΥ Η ΧΩΡΑ ΤΩΝ ΓΕΝΝΑΙΩΝ
-  4: 938.993ΚΥΝ
+  4: 938.498ΚΥΝ
   5: '13029'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2012'
   11: 308Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130223,15 +130268,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-46
   19: 7-101-4
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10457
   1: ΧΑΡΗΣ,ΘΕΟΧΑΡΗΣ
   2: ΤΟ ΚΑΡΑΟΥΡΓΑΝ ΤΟΥ ΚΑΡΣ ΚΑΙ Η ΖΩΗ ΜΟΥ
-  4: 938.993ΧΑΡ
+  4: 938.498ΧΑΡ
   5: '13027'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2001'
   11: 235Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130239,15 +130284,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-59
   19: 6-1
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10458
   1: ΧΑΤΖΗΚΥΡΙΑΚΙΔΗ,ΚΥΡΙΑΚΟ
   2: ΤΟ ΜΕΤΑΛΛΕΙΟ ΤΑΥΡΟΥ (ΜΠΟΥΓΑ ΜΑΝΤΕΝ)1826-1924
-  4: 938.993ΧΑΤ
+  4: 938.498ΧΑΤ
   5: '13026'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2004'
   11: 280Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130287,15 +130332,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-63
   19: 7-2
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10461
   1: ΛΑΠΑΡΙΔΗΣ,ΝΙΚΟΣ
   2: Η ΖΑΒΕΡΑ ΤΗΣ ΜΑΤΣΟΥΚΑΣ ΤΟΥ ΠΟΝΤΟΥ
-  4: 938.993ΛΑΠ
+  4: 938.498ΛΑΠ
   5: '13042'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2003'
   11: 118Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130304,15 +130349,15 @@
   18: 960-343-72
   19: 5-5
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10462
   1: ΣΠΥΡΑΝΤΗ,ΑΝΔΡΕΑ
   2: ΤΡΑΠΕΖΟΥΣ ΚΑΙ Η ΜΟΝΗ ΣΟΥΜΕΛΑ ΤΟΥ ΠΟΝΤΟΥ
   3: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΑ ΧΡΟΝΙΑ 1910-1922
-  4: 938.993ΣΠΥ
+  4: 938.498ΣΠΥ
   5: '13041'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1991'
   11: 110Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130352,15 +130397,15 @@
   14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ\
   18: 978-960-46
   19: 7-431-2
 - 0: 10465
   1: ΛΑΠΑΡΙΔΗ,ΝΙΚΟΥ
   2: Η ΜΑΤΣΟΥΚΑ ΤΟΥ ΠΟΝΤΟΥ
-  4: 938.993ΛΑΠ
+  4: 938.498ΛΑΠ
   5: '13039'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1996'
   11: 181Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130368,15 +130413,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-37
   19: 8-0
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10466
   1: ΠΑΠΑΔΟΠΟΥΛΟΣ,ΓΙΩΡΓΟΣ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΑΥΛΗΑΝΝΑΣ
-  4: 938.993ΠΑΠ
+  4: 938.498ΠΑΠ
   5: '13037'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2000'
   11: 175Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130512,15 +130557,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-76
   19: 2-Χ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10475
   1: ΚΟΥΛΟΧΕΡΗ,ΙΑΚΩΒΟΣ
   2: Η ΑΜΙΣΟΣ ΚΑΙ ΤΑ ΠΑΘΗ ΤΗΣ
-  4: 938.993ΚΟΥ
+  4: 938.498ΚΟΥ
   5: '13047'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1991'
   11: 151Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130528,15 +130573,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-08
   19: 8-9
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10476
   1: ΤΣΑΡΤΙΛΙΔΗ,ΧΡΗΣΤΟΥ
   2: Η ΚΡΩΜΝΗ
-  4: 938.993ΤΣΑ
+  4: 938.498ΤΣΑ
   5: '13046'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2007'
   11: 192Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130561,15 +130606,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-70
   19: 4-2
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10478
   1: ΤΣΑΝΙΚΛΙΔΗ,ΚΩΝ/ΝΟ
   2: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΟΝ ΠΟΝΤΟ
-  4: 938.993ΤΣΑ
+  4: 938.498ΤΣΑ
   5: '13044'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2002'
   11: 167Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130577,15 +130622,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-62
   19: 5-9
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10479
   1: ΤΑΞΙΔΗ,ΕΥΣΤΑΘΙΟΥ
   2: ΑΠΟ ΤΗΝ ΤΣΙΜΕΡΑ ΤΟΥ ΠΟΝΤΟΥ ΣΤΗΝ ΕΛΛΑΔΑ
-  4: 938.993ΤΑΞ
+  4: 938.498ΤΑΞ
   5: '13061'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2007'
   11: 448Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -130675,15 +130720,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-34
   19: 3-990-5
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10485
   1: ΚΑΙΚΟΥΝΙΔΗΣ,ΜΙΧΑΗΛ
   2: ΣΑΜΨΟΥΝΤΑ ΠΟΛΗ ΤΗΣ ΦΩΤΙΑΣ
-  4: 938.993ΚΑΙ
+  4: 938.498ΚΑΙ
   5: '13053'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2009'
   11: 218Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΓΕΩΓΡΑΦΙΑ
@@ -131533,29 +131578,29 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-34
   19: 3-988-2
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10538
   1: ΚΑΝΕΩΣ-ΚΑΝΔΗΛΑΤΟΥ,ΓΕΩΡΓΙΟΥ
   2: ΠΟΝΤΙΑΚΑΙ ΑΝΑΜΝΗΣΕΙΣ
-  4: 938.498ΚΑΝ
+  4: 938.4ΚΑΝ
   5: '13115'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1965'
   11: 72Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10539
   1: ΚΑΝΕΩΣ-ΚΑΝΔΗΛΑΤΟΥ,ΓΕΩΡΓΙΟΥ
   2: Ο ΕΛΛΗΝΟΜΗΜΩΝ ΤΟΥ ΠΟΝΤΟΥ
-  4: 938.498ΚΑΝ
+  4: 938.4ΚΑΝ
   5: '13116'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2006'
   11: 256Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -131898,17 +131943,17 @@
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-75
   19: 2-2
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10561
-  1: BENESEVIC,V.N
+  1: USPENSKIJ,F.I-BENESEVIC,V.N
   2: ΤΑ ACTA ΤΗΣ ΜΟΝΗΣ ΒΑΖΕΛΩΝΟΣ
-  4: 938.498BEN
+  4: 938.498USP
   5: '13109'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2007'
   11: 391Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -131967,23 +132012,23 @@
   18: 978-960-46
   19: 7-187-8
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10565
   1: ΑΠΟΣΤΟΛΙΔΗ,ΠΑΥΛΟΥ
   2: Η ΜΗΤΡΟΠΟΛΙΣ ΡΟΔΟΠΟΛΕΩΣ
   3: ΤΟ ΖΗΤΗΜΑ ΤΩΝ ΕΞΑΡΧΙΩΝ ΤΟΥ ΠΟΝΤΟΥ
-  4: 956.5ΑΠ0
+  4: 938.498ΑΠΟ
   5: 12958-16967
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2007'
   11: 480Σ
-  12: ΠΟΝΤΟΣ-ΘΡΗΣΚΕΙΑ
-  13: ΠΟΝΤΟΣ-ΘΡΗΣΚΕΙΑ
-  14: ΠΟΝΤΟΣ-ΘΡΗΣΚΕΙΑ
+  12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ ΔΩΡΕΑ ΣΩΜΑΤΕΙΟΥ ΠΑΝΑΓΙΑΣ ΣΟΥΜΕΛΑ
   18: 978-960-34
   19: 3-968-4
   30: 2 ΑΝΤΙΤΥΠΑ  &  2 ΑΝΤΙΤΥΠΑ
 - 0: 10566
   1: ΚΑΝΕΩΣ-ΚΑΝΔΗΛΑΤΟΥ,ΓΕΩΡΓΙΟΥ
   2: ΤΟ ΠΡΟΣΚΥΝΗΤΑΡΙΟΝ ΗΤΟΙ ΙΣΤΟΡΙΑ
@@ -132193,23 +132238,23 @@
   14: ΠΟΝΤΟΣ-ΘΡΗΣΚΕΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-34
   19: 3-190-9
 - 0: 10579
   1: ΒΗΣΣΑΡΙΩΝΟΣ
   2: ΕΓΚΩΜΙΟΝ ΕΙΣ ΤΡΑΠΕΖΟΥΝΤΑ
-  4: 230ΒΗΣ
+  4: 938.498ΒΗΣ
   5: '12950'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2000'
   11: 62Σ
-  12: ΠΟΝΤΟΣ-ΕΓΚΩΜΙΑ
-  13: ΠΟΝΤΟΣ-ΕΓΚΩΜΙΑ
-  14: ΠΟΝΤΟΣ-ΕΓΚΩΜΙΑ
+  12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-55
   19: 6-2
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10580
   1: Χ.Σ
   2: Ο ΚΩΔΙΚΑΣ ΤΗΣ ΙΕΡΗΣ ΜΟΝΗΣ ΑΓΙΟΥ ΓΕΩΡΓΙΟΥ ΠΕΡΙΣΤΕΡΕΩΤΑ
@@ -133077,15 +133122,15 @@
   18: 978-960-46
   19: 7-295-0
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10634
   1: ΟΡΦΑΝΙΔΟΥ,ΕΛΕΝΗ
   2: ΤΟ ΧΩΡΙΟ ΜΟΥ ΤΑΧΤΑΡΓΑΝ (ΚΑΡΣ-ΚΑΥΚΑΣΟΥ)
   3: ΒΙΟΓΡΑΦΙΑ ΠΑΥΛΟΥ ΟΡΦΑΝΙΔΗ
-  4: 938.993ΟΡΦ
+  4: 938.498ΟΡΦ
   5: '13063'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2006'
   11: 80Σ
   12: ΠΟΝΤΟΣ-ΑΥΤΟΒΙΟΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΑΥΤΟΒΙΟΓΡΑΦΙΑ
@@ -133353,15 +133398,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-343-58
   19: 6-4
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10651
   1: ΒΑΛΑΒΑΝΗ,ΓΕΩΡΓΙΟΥ
   2: ΣΥΓΧΡΟΝΟΣ ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ
-  4: 938.498ΒΑΛ
+  4: 938.4ΒΑΛ
   5: '13088'
   8: ΑΔΕΛΦΩΝ ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1986'
   11: 317Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -133789,15 +133834,15 @@
   14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   22: ΑΡΧΕΙΟΝ ΠΟΝΤΟΥ
   23: ΠΑΡΑΡΤΗΜΑ 18
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10677
   1: ΛΑΥΡΕΝΤΙΔΗ,ΙΣΑΑΚ
-  2: ΟΙ ΕΚ ΣΟΒΙΕΤΙΚΗΕ ΕΝΩΣΕΩΣ ΕΛΛΗΝΕΣ ΠΟΝΤΙΑΚΗΣ ΚΑΤΑΓΩΓΗΣ ΚΑΙ ΤΑ
+  2: ΟΙ ΕΚ ΣΟΒΙΕΤΙΚΗΣ ΕΝΩΣΕΩΣ ΕΛΛΗΝΕΣ ΠΟΝΤΙΑΚΗΣ ΚΑΤΑΓΩΓΗΣ ΚΑΙ ΤΑ
   3: ΕΚ ΤΗΣ ΣΥΝΘΗΚΗΣ ΤΗΣ ΛΩΖΑΝΗΣ ΔΙΚΑΙΩΜΑΤΑ ΤΩΝ
   4: 938.498ΛΑΥ
   5: '12536'
   8: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ
   9: ΑΘΗΝΑ
   10: '1986'
   11: 168Σ
@@ -133878,15 +133923,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   22: ΑΡΧΕΙΟΝ ΠΟΝΤΟΥ
   23: ΠΑΡΑΡΤΗΜΑ 8
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10682
   1: ΚΩΝΣΤΑΝΤΙΝΙΔΟΥ-ΒΑΡΒΕΡΗ,ΔΕΣΠΟΙΝΑ
   2: ΤΑ ΣΩΖΟΜΕΝΑ ΕΓΓΡΑΦΑ ΤΗΣ ΕΠΙΤΡΟΠΕΙΑΣ ΠΟΝΤΙΩΝ ΕΛΛΗΝΩΝ ΚΩΝ/ΠΟΛΕ
-  4: 938.498ΚΩΝ
+  4: 938.498ΒΑΡ
   5: '12592'
   8: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ
   9: ΑΘΗΝΑ
   10: '2012'
   11: 702Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
@@ -133895,15 +133940,15 @@
   18: 1109-8071
   22: ΑΡΧΕΙΟΝ ΠΟΝΤΟΥ
   23: ΠΑΡΑΡΤΗΜΑ 29
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10683
   1: ΛΑΜΨΙΔΟΥ,ΟΔ.
   2: ΑΝΔΡΕΟΥ ΛΙΒΑΔΗΝΟΥ ΒΙΟΣ ΚΑΙ ΕΡΓΑ
-  4: 938.993ΛΑΜ
+  4: 938.498ΛΑΜ
   5: '12524'
   8: ΕΠΙΤ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕΤ
   9: ΑΘΗΝΑ
   10: '1975'
   11: 296Σ
   12: ΠΟΝΤΟΣ-ΒΙΟΓΡΑΦΙΑ
   13: ΠΟΝΤΟΣ-ΒΙΟΓΡΑΦΙΑ
@@ -134170,15 +134215,15 @@
   13: ΛΟΓΟΤΕΧΝΙΑ
   14: ΛΟΓΟΤΕΧΝΙΑ
   18: 960-248-99
   19: 3-6
 - 0: 10701
   1: ΝΑΝΑΚΗΣ,ΑΝΔΡΕΑΣ
   2: ΜΙΚΡΑ ΑΣΙΑ ΠΡΟΣΦΥΓΙΚΑ ΑΤΕΛΕΥΤΗΤΑ
-  4: 938.498ΝΑΝ
+  4: 938.499ΝΑΝ
   5: 13149-19961
   8: ΑΝΤ.ΣΤΑΜΟΥΛΗΣ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2012'
   11: 248Σ
   12: ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
   13: ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
@@ -134258,23 +134303,23 @@
   13: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
   14: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
   17: ΤΟΜΟΣ ΙΕ
   18: 1106-7063
 - 0: 10707
   1: ΛΥΤ,ΧΡΙΣΤΙΑΝΑ
   2: ΜΙΑ ΔΑΝΕΖΑ ΣΤΗΝ ΑΥΛΗ ΤΟΥ ΟΘΩΝΑ
-  4: 889.21ΛΥΤ
+  4: 938.009ΛΥΤ
   5: '12425'
   8: ΕΡΜΗΣ
   9: ΑΘΗΝΑ
   10: '1988'
   11: 366Σ
-  12: ΛΟΓΟΤΕΧΝΙΑ
-  13: ΛΟΓΟΤΕΧΝΙΑ
-  14: ΛΟΓΟΤΕΧΝΙΑ
+  12: ΙΣΤΟΡΙΑ-ΜΑΡΤΥΡΙΑ
+  13: ΜΑΡΤΥΡΙΑ
+  14: ΙΣΤΟΡΙΚΗ ΜΑΡΤΥΡΙΑ
 - 0: 10708
   1: ΝΕΡΑΤΖΗΣ,ΙΩΑΝΝΗΣ
   2: ΕΠΙΓΡΑΦΕΣ ΚΑΙ ΑΡΧΑΙΟΛΟΓΙΚΑ ΕΥΡΗΜΑΤΑ ΑΡΧΑΙΑΣ ΑΚΑΡΝΑΝΙΑΣ ΣΤΟ
   3: ΜΟΥΣΕΙΟ ΘΥΡΡΕΙΟΥ ΑΚΑΡΝΑΝΙΑΣ
   4: 938.495ΝΕΡ
   5: '13154'
   9: ΑΓΡΙΝΙΟ
@@ -134516,22 +134561,22 @@
   13: ΕΛΛΗΝΙΚΟ ΔΡΑΜΑ
   14: ΕΛΛΗΝΙΚΟ ΔΡΑΜΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10725
   1: ΑΝΔΡΕΑΔΗ,ΓΕΩΡΓΙΟΥ
   2: ΤΟ ΤΣΑΓΡΑΚ ΤΗΣ ΚΕΡΑΣΟΥΝΤΑΣ ΤΟΥ ΠΟΝΤΟΥ
-  4: 398ΑΝΔ
+  4: 938.498ΑΝΔ
   5: '13182'
   9: ΑΘΗΝΑ
   10: '1999'
   11: 214Σ
-  12: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
-  13: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
-  14: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
+  12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10726
   1: ΣΑΜΟΥΗΛΙΔΗ,ΧΡΗΣΤΟΣ
   2: ΣΤΟΥΣ ΠΕΝΤΕ ΑΝΕΜΟΥΣ ΤΟΥ ΚΑΥΚΑΣΟΥ
   4: 889.21ΣΑΜ
   5: '13162'
@@ -134635,15 +134680,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10733
   1: Χ.Σ.
   2: Ο ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΜΑΥΡΗΣ ΘΑΛΑΣΣΑΣ
   3: ΠΟΝΤΟΣ-ΡΩΣΙΑ
   4: 938.498Χ.Σ
-  5: '13203'
+  5: 13203-21362
   9: ΑΘΗΝΑ
   10: '1996'
   11: 188Σ
   12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
@@ -134730,15 +134775,15 @@
   14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10740
   1: ΑΡΓΥΡΟΣ,ΑΝΤΩΝΗΣ
   2: ΤΟ ΝΟΜΙΚΟ ΚΑΘΕΣΤΩΣ ΤΩΝ ΠΑΛΙΝΝΟΥΣΤΟΥΝΤΩΝ
   4: 938.498ΑΡΓ
-  5: '13989'
+  5: '13189'
   9: ΑΘΗΝΑ
   10: '1996'
   11: 415Σ
   12: ΠΟΝΤΟΣ-ΠΡΟΣΦΥΓΕΣ
   13: ΠΟΝΤΟΣ-ΠΡΟΣΦΥΓΕΣ
   14: ΠΟΝΤΟΣ-ΠΡΟΣΦΥΓΕΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
@@ -134784,22 +134829,22 @@
   12: ΠΟΝΤΟΣ-ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΟΝΤΟΣ-ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΟΝΤΟΣ-ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 10744
   1: ΠΑΥΛΙΔΗΣ,ΑΝΤΩΝΗΣ
   2: Ο ΓΚΙΟΥΛΜΠΑΞΕΣ ΕΡΥΘΡΑΙΑΣ
-  4: 398ΠΑΥ
+  4: 938.498ΠΑΥ
   5: '13185'
   9: ΑΘΗΝΑ
   10: '2010'
   11: 187Σ
-  12: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
-  13: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
-  14: ΠΟΝΤΟΣ-ΛΑΟΓΡΑΦΙΑ
+  12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  13: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  14: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-99
   19: 299-0-5
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10745
   1: ΑΓΤΖΙΔΗΣ,ΒΛΑΣΗΣ
   2: ΕΛΛΗΝΕΣ ΤΟΥ ΠΟΝΤΟΥ
@@ -136134,15 +136179,15 @@
   14: ΛΑΟΓΡΑΦΙΑ-ΕΚΜΑΘΗΣΗ ΠΟΝΤΙΑΚΗΣ ΛΥΡΑΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-98
   19: 015-0-8
 - 0: 10837
   1: Χ.Σ.
   2: Η ΓΕΝΟΚΤΟΝΙΑ ΤΟΥ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  4: 938.993Χ.Σ
+  4: 938.498Χ.Σ
   5: 13404-13945
   8: Ο.Π.Σ.Ν.Ε
   9: ΑΘΗΝΑ
   10: '1996'
   11: 16Σ
   12: ΙΣΤΟΡΙΑ-ΓΕΝΟΚΤΟΝΙΑ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
   13: ΙΣΤΟΡΙΑ-ΓΕΝΟΚΤΟΝΙΑ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
@@ -136374,15 +136419,15 @@
   12: ΠΕΡΙΟΔΙΚΟ ΠΟΝΤΙΑΚΑ ΦΥΛΛΑ
   13: ΠΕΡΙΟΔΙΚΟ ΠΟΝΤΙΑΚΑ ΦΥΛΛΑ
   14: ΠΕΡΙΟΔΙΚΟ ΠΟΝΤΙΑΚΑ ΦΥΛΛΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 10854
   1: ΜΙΧΑΗΛΙΔΗΣ,ΧΡΗΣΤΟΣ-ΑΘΑΝΑΣΙΑΔΗΣ,ΑΝΔΡΕΑΣ
   2: ΓΕΝΝΗΘΕΙΣ ΕΙΣ ΚΑΥΚΑΣΟΝ ΡΩΣΙΑΣ
-  4: 938.498ΜΙΧ
+  4: 938.498ΑΘΑ
   5: '13451'
   8: ΙΝΦΟΓΝΩΜΩΝ
   9: ΑΘΗΝΑ
   10: '2010'
   11: 384Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -136435,17 +136480,17 @@
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-83
   19: 62-59-8
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10858
-  1: ΚΥΠΑΡΛΗ-ΑΚΡΙΤΙΔΟΥ,ΕΛΙΣΑΒΕΤ
+  1: ΑΚΡΙΤΙΔΟΥ-ΚΥΠΑΡΛΗ,ΕΛΙΣΑΒΕΤ
   2: Η ΧΡΥΣΑΝΝΑ ΤΟΥ ΠΟΝΤΟΥ
-  4: 938.498ΚΥΠ
+  4: 938.498ΑΚΡ
   5: '13444'
   8: ΙΝΦΟΓΝΩΜΩΝ
   9: ΑΘΗΝΑ
   10: '2012'
   11: 84Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -136701,29 +136746,29 @@
   12: ΠΟΝΤΙΑΚΟΣ ΕΛΛΗΝΙΣΜΟΣ
   13: ΠΟΝΤΙΑΚΟΣ ΕΛΛΗΝΙΣΜΟΣ
   14: ΠΟΝΤΙΑΚΟΣ ΕΛΛΗΝΙΣΜΟΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 10876
   1: ΓΑΛΑΝΙΔΟΥ-ΜΠΑΛΦΟΥΣΙΑ,ΕΛΣΑ
   2: ΕΞΟΧΕΣ ΚΑΙ ΠΑΡΧΑΡΙΑ ΤΗΣ ΤΡΑΠΕΖΟΥΝΤΑΣ
-  4: 938.498ΓΑΛ
+  4: 938.498ΜΠΑ
   5: '13434'
   8: ΕΝ.ΠΟΝ.ΜΕΛΙΣΣΙΩΝ ΑΤΤ
   9: ΑΘΗΝΑ
   10: '1982'
   11: 20Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10877
   1: ΓΑΛΑΝΙΔΟΥ-ΜΠΑΛΦΟΥΣΙΑ,ΕΛΣΑ
   2: ΟΙ ΕΛΛΗΝΕΣ ΤΟΥ ΠΟΝΤΟΥ ΚΙ Η ΠΑΝΑΓΙΑ ΣΟΥΜΕΛΑ
-  4: 938.498ΓΑΛ
+  4: 938.498ΜΠΑ
   5: '13433'
   8: ΕΝ.ΠΟΝ.ΜΕΛΙΣΣΙΩΝ ΑΤΤ
   9: ΑΘΗΝΑ
   10: '1997'
   11: 29Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -137312,15 +137357,15 @@
   18: 978-960-68
   19: 26-00-9
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10920
   1: ΡΟΔΑΚΗΣ,ΠΕΡΙΚΛΗΣ
   2: Η ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ Α)ΑΠΟ ΤΑ ΜΥΘΙΚΑ ΧΡΟΝΙΑ ΩΣ ΤΗΝ ΤΟΥΡΚΙΚΗ
   3: ΚΑΤΑΚΤΗΣΗ Β)ΑΠΟ ΤΗΝ ΤΟΥΡΚΙΚΗ ΚΑΤΑΚΤΗΣΗ ΩΣ ΤΗ ΓΕΝΟΚΤΟΝΙΑ
-  4: 938.498ΡΟΔ
+  4: 938.4ΡΟΔ
   5: '13486'
   8: ΓΟΡΔΙΟΣ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 415Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -137654,23 +137699,23 @@
   18: 978-960-68
   19: 26-17-7
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10941
   1: ΤΣΙΛΙΜΑΓΚΟΥ-ΕΥΣΤΑΘΙΑΔΟΥ,ΣΟΥΛΑ
   2: ΚΙ ΥΣΤΕΡΑ Ο ΞΕΡΙΖΩΜΟΣ
   3: ΕΛΛΗΝΕΣ ΤΗΣ ΚΑΠΠΑΔΟΚΙΑΣ
-  4: 889.21ΤΣΙ
+  4: 938.498ΤΣΙ
   5: '13481'
   8: ΓΟΡΔΙΟΣ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 238Σ
-  12: ΛΟΓΟΤΕΧΝΙΑ
-  13: ΛΟΓΟΤΕΧΝΙΑ
-  14: ΛΟΓΟΤΕΧΝΙΑ
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-70
   19: 83-93-7
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10942
   1: ΔΡΑΓΟΥΜΗ,ΜΑΡΚΟΥ
   2: Η ΠΑΡΑΔΟΣΙΑΚΗ ΜΑΣ ΜΟΥΣΙΚΗ
@@ -138518,15 +138563,15 @@
   19: 3-6
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10998
   1: ΠΑΠΑΤΡΙΑΝΤΑΦΥΛΛΟΥ,ΑΘΑΝΑΣΙΟΣ
   2: ΘΡΑΚΗ ΙΣΤΟΡΙΕΣ ΖΩΗΣ
   3: ΟΔΟΙΠΟΡΙΚΟ ΤΡΙΩΝ ΑΙΩΝΩΝ
   4: 938.498ΠΑΠ
-  5: '13623'
+  5: '13627'
   8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 304Σ
   12: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
   13: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
   14: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
@@ -139757,15 +139802,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-95
   19: 33-03-4
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 11078
   1: ΓΙΑΝΝΟΥΛΑΤΣΟΥ-ΔΕΣΤΟΥΝΗ,ΜΑΡΙΑ-ΧΡΙΣΤΙΝΑ
   2: ΠΟΝΤΟΣ ΚΑΙ ΑΣΗΜΙ
-  4: 398ΓΙΑ
+  4: 938.498ΔΕΣ
   5: '13687'
   11: 13Σ
   12: ΜΟΥΣΕΙΟ ΜΠΕΝΑΚΗ
   13: ΜΟΥΣΕΙΟ ΜΠΕΝΑΚΗ
   14: ΜΟΥΣΕΙΟ ΜΠΕΝΑΚΗ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-8347-1
@@ -140557,15 +140602,15 @@
   16: ΧΡΙΣΤΟΦΟΡΙΔΗ ΧΡ.
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΔΙΔΗ
   19: '9789604672'
 - 0: 11132
   1: ΤΟΙΛΟΣ ΧΡΗΣΤΟΣ ΥΠΟΣΤΡΑΤΗΓΟΣ
   2: Η ΠΟΡΕΙΑ ΤΟΥ ΒΕΛΛΗΝΙΣΜΟΥ ΠΡΟΣ ΤΗΝ ΕΠΑΝΑΣΤΑΣΗ ΤΟΥ 1821
   3: (ΣΥΝΟΔΕΥΕΤΑΙ ΑΠΟ 155 ΣΛΑΙΤΣ
-  4: '938.498'
+  4: 938.498Χ.Σ
   5: '13813'
   9: ΜΕΛΙΣΣΙΑ
   10: '2000'
   11: 56Σ
   12: ΔΙΑΛΕΞΗ
   13: ΔΙΑΛΕΞΗ
   14: ΔΙΑΛΕΞΗ
@@ -140878,18 +140923,19 @@
   10: '1993'
   11: 281Σ
   12: ΙΣΤΟΡΙΚΟ
   13: ΙΣΤΟΡΙΚΟ
   14: ΙΣΤΟΡΙΚΟ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 11158
-  1: GRIECHISCHES PARLAMENT
+  1: ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩΝ
   2: ΠΕΡΙΚΛΕΟΥΣ ΕΠΙΤΑΦΙΟΣ
-  4: 938.498GRI
+  4: 881ΘΟΥ
   5: '13790'
+  11: '25'
   12: ΙΣΤΟΡΙΚΟ
   13: ΙΣΤΟΡΙΚΟ
   14: ΙΣΤΟΡΙΚΟ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 11159
   1: ΜΑΓΕΡ,ΦΡΑΝΚ ΧΕΡΜΑΝ
   2: ΑΠΟ ΤΗ ΒΙΕΝΝΗ ΣΤΑ ΚΑΛΑΒΡΥΤΑ
@@ -142657,18 +142703,18 @@
   10: '1999'
   11: 351Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 11297
-  1: ΕΥΑΓΓΕΛΙΑ ΓΙΑΜΑΛΗ- ΧΑΖΤΗΙΩΑΝΝΟΥ
+  1: ΧΑΤΖΗΙΩΑΝΝΟΥ-ΓΙΑΜΜΑΛΗ,ΕΥΑΓΓΕΛΙΑ
   2: ΜΙΚΡΑΣΙΑΤΙΚΟΣ ΕΛΛΗΝΙΣΜΟΣ
-  3: ΟΔΟΙΠΟΡΙΚΟΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
-  4: 938.488ΧΑΤ
+  3: ΟΔΟΙΠΟΡΙΚΟ  ΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
+  4: 938.498ΧΑΤ
   5: '14086'
   9: ΝΙΚΑΙΑ
   10: '2001'
   11: 55Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
@@ -142770,25 +142816,27 @@
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 7-095-935-
   19: '0155'
 - 0: 11306
-  1: ΕΥΑΓΓΕΛΙΑ ΓΙΑΜΑΛΗ-ΧΑΤΖΗΙΩΑΝΝΟΥ
-  2: ΜΙΚΡΑΣΙΑΤΙΚΟΣ ΕΛΛΗΝΙΣΜΟΣ ΟΔΟΙΠΟΡΙΚΟΘΑΝΑΤΟΥ ΚΑΙ ΑΝΑΣΤΑΣΗΣ
-  4: 938.498ΧΑΤ
-  5: '14086'
-  8: ΔΗΜΟΣ ΝΙΚΑΙΑΣ
-  10: '2001'
-  11: 56Σ
-  12: ΙΣΤΟΡΙΑ
-  13: ΙΣΤΟΡΙΑ
-  14: ΙΣΤΟΡΙΑ
-  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
+  1: ΚΑΛΠΟΥΖΟΣ,ΓΙΑΝΝΗΣ
+  2: ΚΑΛΝΤΕΡΙΜΙ 99ΧΡΟΝΙΑ ΣΤΗ ΣΑΛΟΝΙΚΗ
+  4: 889.21ΚΑΛ
+  5: '22886'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2023'
+  11: '576'
+  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+  18: '9786180149'
+  19: '234'
 - 0: 11307
   1: Χ. Σ.
   2: ΜΕΡΕΣ ΦΡΙΚΗΣ ΣΤΗ ΧΙΛΗ
   4: 330Χ. Σ
   5: '11886'
   6: ΠΑΝΑΓΗ Β. ΜΕΤΑΞΑ
   8: ΜΗΝΥΜΑ
@@ -142820,15 +142868,15 @@
   12: ΠΕΡΙΟΔΙΚΟ
   13: ΠΕΡΙΟΔΙΚΟ
   14: ΠΕΡΙΟΔΙΚΟ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: ΤΟΜΟΙ2)Ζ,ΙΓ, ΣΤ,Ε,Β,Δ
 - 0: 11310
   1: Χ. Σ.
-  2: ΝΑΥΠΗΓΙΚΗΓ ΚΑΙ ΠΛΟΙΑ ΤΗΑ ΑΝΑΤΟΛΙΚΗΣ ΜΕΣΟΓΕΙΟΥ ΚΑΙ ΜΑΥΡ ΘΑΛΑΣ
+  2: ΝΑΥΠΗΓΙΚΗ ΚΑΙ ΠΛΟΙΑ ΤΗΑ ΑΝΑΤΟΛΙΚΗΣ ΜΕΣΟΓΕΙΟΥ ΚΑΙ ΜΑΥΡ ΘΑΛΑΣ
   3: ΣΑΣ ΚΑΤΑ ΤΟΝ 18 ΚΑΙ 19 ΑΙΩΝΑ
   4: 938.498Χ.Σ
   5: '13989'
   8: ΠΝΕΥΜΑΤΙΚΟΚΕΝ ΑΘΗΝΩΝ
   11: 146Σ
   12: ΝΑΥΠΗΓΙΚΗ ΤΕΧΝΗ
   13: ΝΑΥΠΗΓΙΚΗ ΤΕΧΝΗ
@@ -142937,15 +142985,15 @@
   5: '14065'
   9: ΙSTANBUL
   12: TOYRKIA
   13: TOYRKIA
   14: TOYRKIA
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 11320
-  1: ΑΧΙΛΛΕΑΣ ΙΩΑΝΝΟΥ ΛΑΜΤΖΙΔΗΣ
+  1: ΛΑΜΤΖΙΔΗΣ,ΑΧΙΛΛΕΑΣ
   2: ΣΥΜΒΟΛΗ ΣΤΗ ΔΗΜΟΓΡΑΦΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΕΝΟΡΙΑΣ ΥΠΑΠΑΝΤΗΣ ΤΗΣ
   3: ' ΤΡΑΠΕΖΟΥΝΤΑΣ (1920-1923)'
   4: 938.498ΛΑΜ
   5: '13990'
   9: ΑΘΗΝΑ
   10: '1997'
   11: 251Σ
@@ -143066,15 +143114,15 @@
   12: ΔΗΜΟΓΡΑΦΙΚΑ ΠΡΟΒΛΗΜΑΤΑ
   13: ΔΗΜΟΓΡΑΦΙΚΑ ΠΡΟΒΛΗΜΑΤΑ
   14: ΔΗΜΟΓΡΑΦΙΚΑ ΠΡΟΒΛΗΜΑΤΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-86167-
   19: 0-0
 - 0: 11330
-  1: ΜΑΡΙΑ ΝΥΣΤΑΖΟΠΟΥΛΟΠΥ-ΠΕΛΕΚΙΔΟΥ
+  1: ΠΕΛΕΚΙΔΟΥ-ΝΥΣΤΑΖΟΠΟΥΛΟΥ,ΜΑΡΙΑ
   2: ΤΟ ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ
   3: ΙΣΤΟΡΙΚΗ ΘΕΩΡΗΣΗ ΤΟΥ ΠΡΟΒΛΗΜΑΤΟΣ
   4: 938.498ΠΕΛ
   5: '14113'
   8: ΚΕΝΤΡΟ ΣΠΟΥΔΩΝ ΝΑ.ΕΥ
   9: ΑΘΗΝΑ
   10: '1998'
@@ -143097,15 +143145,15 @@
   14: ΠΑΙΔΕΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 11332
   1: ΓΕΩΡΓΙΟΣ ΧΑΡ. ΠΑΠΑΔΟΠΟΥΛΟΣ
   2: Η ΕΘΝΙΚΗ ΕΛΛΗΝΙΚΗ ΜΕΙΟΝΟΤΗΣ ΕΙΣ ΤΗΝ ΑΛΒΑΝΙΑΝ ΚΑΙ ΤΟ ΣΧΟΛΙΚΟΝ
   3: ' ΑΥΤΗΣ ΖΗΤΗΜΑ'
   4: 938.498ΠΑΠ
-  5: '14022'
+  5: '14092'
   8: ΙΔΡΥΜΑ ΒΟΡ/ΚΩΝ ΕΡΕΥΝ
   9: ΙΩΑΝΝΙΝΑ
   10: '1981'
   11: 296Σ
   12: ΙΣΤΟΡΙΑ ΑΛΒΑΝΙΑ
   13: ΙΣΤΟΡΙΑ ΑΛΒΑΝΙΑ
   14: ΙΣΤΟΡΙΑ ΑΛΒΑΝΙΑ
@@ -144654,30 +144702,30 @@
   10: '1989'
   11: 87Σ
   12: ΥΠΟΛΟΓΙΣΤΕΣ
   13: ΥΠΟΛΟΓΙΣΤΕΣ
   14: ΥΠΟΛΟΓΙΣΤΕΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 11446
-  1: ΓΕΡΑΣΙΜΟΣ Μ. ΒΛΑΧΟΣ
+  1: ΒΛΑΧΟΣ,ΓΕΡΑΣΙΜΟΣ
   2: ΤΟ ΑΡΧΕΙΟΝ ΤΗΣ ΙΟΝΙΚΗΣ ΤΡΑΠΕΖΗΣ
   3: ΕΓΓΡΑΦΑ ΤΗΣ ΠΕΡΙΟΔΟΥ 1833-1920
   4: 938.498ΒΛΑ
   5: '13530'
   8: ΕΤΑΙΡ ΜΕΛ ΕΛΛΗΝ ΙΣΤ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 32Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   30: 3 ΑΝΤΙΤΥΠΑ
 - 0: 11447
-  1: ΣΠΥΡΟΣ ΔΗΜ. ΛΟΥΚΑΤΟΣ
+  1: ΛΟΥΚΑΤΟΣ,ΣΠΥΡΟΣ
   2: ΠΟΛΙΤΕΙΟΓΡΑΦΙΑ ΤΗΣ ΝΟΜΑΡΧΙΑΚΗΣ ΠΕΡΙΕΦΕΡΕΙΑΣ ΤΗΣ ΘΕΣΣΑΛΟΝΙΚΗΣ
   4: 304.60ΛΟΥ
   5: '14104'
   8: ΚΕΝΤ ΣΠ ΝΑ ΕΥΡΩΠΗΣ
   9: ΑΘΗΝΑ
   10: '1987'
   11: 139Σ
@@ -144949,24 +144997,28 @@
   5: '14147'
   12: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   14: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ
   30: ΤΟΜΟΙ ΕΠΤΑ ΛΕΙΠΕΙ Ο Ζ ΤΟΜΟΣ
 - 0: 11470
-  1: ΣΑΡΑΝΤΟΣ Ι. ΚΑΡΓΑΛΟΣ
+  1: ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
   2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   3: Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
   4: 938.498ΚΑΡ
-  5: '14148'
-  12: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
-  13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
-  14: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
+  5: 14148-17352
+  8: REAL NEWS
+  9: ΑΘΗΝΑ
+  10: '2014'
+  11: '224'
+  12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+  13: ΜΕΓΑ ΑΛΕΞΑΝΔΡΟΣ
+  14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
-  30: ΤΟΜΟΙ 3
+  30: ΤΟΜΟΙ 2
 - 0: 11471
   1: ΓΡΗΓΟΡΙΑΔΗΣ,ΣΟΛΩΝ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΣΥΓΧΡΟΝΗΣ ΕΛΛΑΔΑΣ 1941-1974
   4: 938.498ΓΡΗ
   5: '15094'
   8: ΤΕΓΟΠΟΥΛΟΣ
   9: ΑΘΗΝΑ
@@ -144975,18 +145027,20 @@
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   14: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   18: 978-960-94
   19: '87634'
   30: 12 ΤΟΜΟΙ
 - 0: 11472
-  1: ΠΕΡΙΟΔΙΚΟ
+  1: Χ.Σ
   2: ΕΛΛΗΝΩΝ ΙΣΤΟΡΙΚΑ
-  4: 938.498ΠΕΡ
+  4: 938.498Χ.Σ
   5: '14149'
+  9: ΑΘΗΝΑ
+  11: '155'
   12: ΠΕΡΙΟΔΙΚΟ
   13: ΠΕΡΙΟΔΙΚΟ
   14: ΠΕΡΙΟΔΙΚΟ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   30: 12 ΤΕΥΧΗ
 - 0: 11473
   1: ΠΕΡΙΟΔΙΚΟ
@@ -145011,15 +145065,15 @@
   12: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   14: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   18: 960-14-053
   19: 5-6
 - 0: 11475
-  1: ΒΑΣΙΛΙΚΗ ΛΑΖΟΥ
+  1: ΛΑΖΟΥ,ΒΑΣΙΛΙΚΗ
   2: ΠΟΛΗ 1955 Η ΤΕΛΕΥΤΑΙΑ ΑΛΩΣΗ
   4: 938.498ΛΑΖ
   8: ΕΛΕΥΘΕΡΟΤΥΠΙΑ
   9: ΑΘΗΝΑ
   10: '2010'
   11: 192Σ
   12: ΙΣΤΟΡΙΑ
@@ -145033,49 +145087,54 @@
   5: '14154'
   12: ΤΑΞΙΔΙΩΤΙΚΟΙ ΟΔΗΓΟΙ
   13: ΤΑΞΙΔΙΩΤΙΚΟΙ ΟΔΗΓΟΙ
   14: ΤΑΞΙΔΙΩΤΙΚΟΙ ΟΔΗΓΟΙ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   30: 3 ΤΕΥΧΗ
 - 0: 11477
-  1: ΓΙΩΡΓΟΣ ΞΕΠΑΠΑΔΑΚΟΣ
+  1: ΞΕΠΑΠΑΔΑΚΟΣ,ΓΙΩΡΓΟΣ
   2: ΘΡΑΚΕΣ ΤΣΑΚΩΝΕΣ ΜΑΚΕΔΟΝΕΣ ΑΡΒΑΝΙΤΕΣ ΜΙΚΡΑΣΙΑΤΕΣ
   4: 910 ΞΕΠ
   5: '14153'
   12: ΡΙΖΕΣ ΕΛΛΗΝΩΝ
   13: ΡΙΖΕΣ ΕΛΛΗΝΩΝ
   14: ΡΙΖΕΣ ΕΛΛΗΝΩΝ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   30: 5 ΤΟΜΟΙ
 - 0: 11478
-  1: ΒΑΣΙΛΙΚΗ ΛΑΖΟΥ
-  2: ΚΙΝΗΜΑΤΑ ΠΡΑΞΙΚΟ[ΠΗΜΑΤΑ ΔΙΚΤΑΤΟΡΙΕΣ
+  1: ΛΑΖΟΥ,ΒΑΣΙΛΙΚΗ
+  2: ΚΙΝΗΜΑΤΑ ΠΡΑΞΙΚΟΠΗΜΑΤΑ ΔΙΚΤΑΤΟΡΙΕΣ
   4: 938.498ΛΑΖ
   5: '14152'
+  8: ΕΛΕΥΘΕΡΟΤΥΠΙΑ
+  9: ΑΘΗΝΑ
+  10: '2011'
   11: 193Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
+  18: '9789609487'
+  19: '733'
 - 0: 11479
-  1: ΓΕΩΡΓΙΟΣ ΒΙΖΥΗΝΟΣ
+  1: ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
   2: ΑΤΘΙΔΕΣ ΑΥΡΑΙ
   4: 889.21ΒΙΖ
   5: '14163'
   8: ΛΑΜΠΡΑΚΗΣ
   10: '2014'
   11: 330Σ
   12: ΠΟΙΗΣΗ
   13: ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   18: 978-960-50
   19: 3-471-9
 - 0: 11480
-  1: ΚΩΣΤΗΣ ΠΑΛΑΜΑΣ
+  1: ΠΑΛΑΜΑΣ,ΚΩΣΤΗΣ
   2: Ο ΔΩΔΕΚΑΛΟΓΟΣ ΤΟΥ ΓΥΦΤΟΥ
   4: 889.21ΠΑΛ
   5: '14162'
   8: ΤΟ ΒΗΜΑ
   9: ΑΘΗΝΑ
   10: '2014'
   11: 204Σ
@@ -145095,26 +145154,26 @@
   10: '1962'
   11: 394Σ
   12: ΨΥΧΟΛΟΓΙΑ
   13: ΨΥΧΟΛΟΓΙΑ
   14: ΨΥΧΟΛΟΓΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11482
-  1: ΠΑΝΟΣ ΜΠΑΙΛΗΣ
+  1: ΜΠΑΙΛΗΣ,ΠΑΝΟΣ
   2: ΤΟΥ ΛΟΓΟΥ ΜΟΥ Ο ΜΟΝΑΧΟΣ ΠΑΙΣΙΟΣ
   4: 938.993ΜΠΑ
   5: '14159'
   8: ΧΡΗΣΤΟΣ ΚΤΕΝΑΣ
   11: 111Σ
   12: ΘΡΗΣΚΕΙΑ
   13: ΘΡΗΣΚΕΙΑ
   14: ΘΡΗΣΚΕΙΑ
   17: ΔΩΡΕΑ ΔΥΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11483
-  1: ΘΕΟΦ. ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ
+  1: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ
   2: ΠΟΛΙΤΙΚΗ ΑΓΩΓΗ
   4: 320.071ΠΑΠ
   5: '14169'
   8: KABANAS
   9: ΑΘΗΝΑΙ
   10: '1970'
   12: ΠΟΛΙΤΙΚΗ ΑΓΩΓΗ
@@ -145168,15 +145227,15 @@
   10: '2013'
   11: 223Σ
   12: ΨΑΡΙΑ
   13: ΨΑΡΙΑ
   14: ΨΑΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11488
-  1: ΛΕΝΑ ΛΟΥΚΙΔΟΥ
+  1: ΔΟΥΚΙΔΟΥ,ΛΕΝΑ
   2: ΠΩΣ ΦΤΑΣΑΜΕ ΣΤΗ ΔΙΚΤΑΤΟΡΙΑ ΤΟΥ 67
   4: 938.498ΔΟΥ
   5: '14168'
   8: ΛΑΜΠΡΑΚΗ
   10: '2012'
   11: 251Σ
   12: ΙΣΤΟΡΙΑ
@@ -145261,15 +145320,15 @@
   8: ΤΕΓΟΠΟΥΛΟΣ
   11: 398Σ
   12: ΠΟΙΗΣΗ
   13: ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11495
-  1: ΣΤΑΥΡΟΣ ΨΥΧΑΡΗΣ
+  1: ΨΥΧΑΡΗΣ,ΣΤΑΥΡΟΣ
   2: ΟΙ ΕΒΔΟΜΗΝΤΑ ΚΡΙΣΙΜΕΣ ΗΜΕΡΕΣ
   4: 938.498ΨΥΧ
   5: '14189'
   8: ΛΑΜΠΡΑΚΗ
   10: '2013'
   11: 303Σ
   12: ΙΣΤΟΡΙΑ
@@ -145359,43 +145418,43 @@
   9: ΑΘΗΝΑ
   11: 323Σ
   12: ΦΙΛΟΣΟΦΙΑ\
   13: ΦΙΛΟΣΟΦΙΑ
   14: ΦΙΛΟΣΟΦΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11503
-  1: ΣΤΕΦΑΝΟΣ, ΠΑΠΑΔΟΠΟΥΛΟΣ
-  2: ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΕΠΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
-  4: 938.498ΠΑΠ
-  5: '14176'
-  9: ΘΕΣ/ΝΙΚΗ
-  10: '1969'
-  11: 62Σ
-  12: ΙΣΤΟΡΙΑ
-  13: ΙΣΤΟΡΙΑ
-  14: ΙΣΤΟΡΙΑ
-  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
+  1: ΗΛΙΟΠΟΥΛΟΣ,ΓΙΩΡΓΟΣ
+  2: Ο ΑΓΝΩΣΤΟΣ ΑΛΕΞΑΝΔΡΟΣ
+  4: 938.070ΗΛΙ
+  5: '17213'
+  9: ΑΘΗΝΑ
+  10: '2003'
+  11: '250'
+  12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+  13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+  14: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
+  18: '9607882229'
 - 0: 11504
   1: Ε. Π. ΠΑΠΑΝΟΥΤΣΟΥ
   2: ΨΥΧΟΛΟΓΙΑ
   4: 150ΠΑΠ
   5: '14173'
   8: ΔΩΔΩΝΗ
   9: ΑΘΗΝΑΙ
   10: '1970'
   11: 220Σ
   12: ΨΥΧΟΛΟΓΙΑ
   13: ΨΥΧΟΛΟΓΙΑ
   14: ΨΥΧΟΛΟΓΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11505
-  1: ΦΩΤΕΙΝΗ ΤΖΙΚΟΥ
+  1: ΤΖΙΚΟΥ,ΦΩΤΕΙΝΗ
   2: Ο ΑΓΝΩΣΤΟΣ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  4: 938.498ΤΖΙ
-  5: '14172'
+  4: 938.174ΤΖΙ
+  5: 14172-17408
   7: Β
   8: ΑΡΧΕΤΥΠΟ
   10: '2005'
   11: 254Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
@@ -145664,15 +145723,15 @@
   9: ΑΘΗΝΑ
   10: '1896'
   12: ΑΛΦΑΒΗΤΑΡΙΟΝ
   13: ΑΛΦΑΒΗΤΑΡΙΟΝ
   14: ΑΛΦΑΒΗΤΑΡΙΟΝ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11526
-  1: ΚΑΡΛ ΜΕΝΤΕΛΣΟΝ -ΜΠΑΡΤΟΛΝΤΙ
+  1: ΜΕΝΤΕΛΣΟΝ-ΜΠΑΡΤΟΛΝΤΙ,ΚΑΡΛ
   2: ΕΠΙΤΟΜΗ ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
   4: 938.498ΜΕΝ
   5: '15029'
   8: ΤΕΓΟΠΟΥΛΟΣ
   10: '2011'
   11: 235Σ
   12: ΕΠΙΤΟΜΗ ΙΣΤΟΡΙΑ
@@ -145853,27 +145912,27 @@
   12: ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   17: ΔΩΡΕΑΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   18: 978-960-50
   19: 3-278-4
 - 0: 11541
-  1: Α. ΘΑΒΩΡΗΣ
+  1: ΘΑΒΩΡΗΣ,Α
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΓΛΩΣΣΑΣ
   4: 938.498ΘΑΒ
   5: '15001'
   9: ΙΩΑΝΝΙΝΑ
   10: '1971'
   11: 153Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
-  17: ΔΩΡΕΑΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11542
-  1: ΓΕΩΡΓΙΟΥ Ι. ΘΕΟΧΑΡΙΔΟΥ
+  1: ΘΕΟΧΑΡΙΔΟΥ,ΓΕΩΡΓΙΟΥ
   2: ΙΣΤΟΡΙΑ ΜΕΣΩΝ ΧΡΟΝΩΝ
   4: 938.498ΘΕΟ
   5: '14197'
   9: ΘΕΣ/ΝΙΚΗ
   10: '1970'
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
@@ -146049,15 +146108,15 @@
   11: 144Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   13: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   18: 978-960-47
   19: 5-151-8
-  30: 5 ΤΟΜΟΙ
+  30: 7 ΤΟΜΟΙ
 - 0: 11556
   1: DIEHL,CHARLES
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
   4: 938.498DIE
   5: '15036'
   8: ΗΛΙΑΔΗ
   11: 118Σ
@@ -146381,15 +146440,15 @@
   12: ΦΙΛΟΣΟΦΙΑ
   13: ΦΙΛΟΣΟΦΙΑ
   14: ΦΙΛΟΣΟΦΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
   18: 978-960-83
   19: 59-92-5
 - 0: 11581
-  1: ΜΠΑΙΡΟΝ
+  1: ΠΡΟΚΟΣ,ΦΡΕΝΤΕΡΙΚ
   2: ΤΑ ΧΕΙΡΟΓΡΑΦΑ ΤΟΥ ΜΕΣΟΛΟΓΓΙΟΥ
   4: 938.483ΜΠΑ
   5: '15049'
   6: ΠΑΝΑΓΙΩΤΗΣ ΣΚΟΝΔΡΑΣ
   8: ΤΕΓΟΠΟΥΛΟΣ
   10: '2011'
   11: 301Σ
@@ -146492,15 +146551,15 @@
   8: ΤΟ ΒΗΜΑ
   11: 160Σ
   12: ΜΝΗΜΝΕΙΑ
   13: ΜΝΗΜΕΙΑ
   14: ΜΝΗΜΕΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11590
-  1: Ν. ΤΣΙΦΟΡΟΥ
+  1: ΤΣΙΦΟΡΟΥ,Ν.
   2: ΙΑΣΟΝΑΣ
   4: 808.899ΤΣΙ
   5: '15072'
   10: '2013'
   11: 49Σ
   12: ΜΥΘΟΛΟΓΙΑ
   13: ΜΥΘΟΛΟΓΙΑ
@@ -148716,15 +148775,15 @@
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11754
   1: Χ.Σ.
   2: ΟΙ 100 ΜΕΓΑΛΥΤΕΡΕΣ ΜΑΧΕΣ ΤΗΣ ΙΣΤΟΡΙΑ
   4: 938.498Χ.Σ
-  5: '15234'
+  5: '15237'
   8: ΕΘΝΟΣ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 79Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
@@ -150763,15 +150822,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 11905
   1: Χ.Σ.
   2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  4: 938.498Χ.Σ
+  4: 938.174Χ.Σ
   5: '15350'
   8: ΤΕΓΟΠΟΥΛΟΣ
   11: 194Σ
   12: ΙΣΤΙΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   14: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
@@ -154660,18 +154719,18 @@
   10: '1964'
   11: 220Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΕΡΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12210
-  1: THOMPSON HOMER
+  1: Χ.Σ
   2: Η ΑΓΟΡΑ ΤΗΣ ΑΡΧΑΙΑΣ ΑΘΗΝΑ
   3: ΣΥΝΤΟΜΟΣ ΟΔΗΓΟΣ
-  4: 938.498THO
+  4: 938.498Χ.Σ
   5: '15612'
   8: ΑΜΕΡ ΣΧ ΚΛΑΣΣΙΚ ΣΠ
   9: ΑΘΗΝΑ
   10: '1985'
   11: 32Σ
   12: ΙΣΤΟΡΙΑ ΑΡΧΑΙΑ ΑΘΗΝΑ
   13: ΙΣΤΟΡΙΑ ΑΡΧΑΙΑ ΑΘΗΝΑ
@@ -155587,15 +155646,15 @@
   12: ΑΝΘΡΩΠΟΓΕΩΓΡΑΦΙΑ
   13: ΑΝΘΡΩΠΟΓΕΩΓΡΑΦΙΑ
   14: ΑΝΘΡΩΠΟΓΕΩΓΡΑΦΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12282
   1: ΓΟΡΓΩ-ΑΛΕΞΙΟΥ,ΓΕΩΡΓΙΑ
   2: ΤΟ ΟΙΚΟΥΜΕΝΙΚΟ ΟΡΑΜΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
-  4: 938.498ΓΟΡ
+  4: 938.07ΓΟΡ
   5: '15710'
   8: ΕΡΩΔΙΟΣ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2010'
   11: 48Σ
   12: ΙΣΤΟΡΙΑ-ΑΛΕΞΑΝΔΡΟΣ
   13: ΙΣΤΟΡΙΑ-ΑΛΕΞΑΝΔΡΟΣ
@@ -155626,15 +155685,15 @@
   12: ΙΣΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΑ
   13: ΙΣΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΑ
   14: ΙΣΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12285
   1: Χ.Σ.
   2: ΤΟ ΣΥΜΒΟΥΛΙΟ ΤΗΣ ΕΠΙΚΡΑΤΕΙΑΣ ΣΤΗΝ ΕΛΛΑΔΑ
-  4: 938.498ΙΣΤ
+  4: 938.498Χ.Σ
   5: '15518'
   8: ΑΡΜΕΝΟΠΟΥΛΟ
   9: ΑΘΗΝΑ
   10: '1979'
   11: 167Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
@@ -155651,15 +155710,15 @@
   11: 380Σ
   12: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   13: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   14: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
   30: ΤΟΜΟΙ Β-Γ-Δ
 - 0: 12287
-  1: ΓΚΑΡΟΥΦ,Β-ΤΣΙΜΠΟΥΚΙΔΗΣ,ΔΗΜ
+  1: ΓΚΑΦΟΥΡΟΦ,Β-ΤΣΙΜΠΟΥΚΙΔΗΣ,ΔΗΜ
   2: ΑΛΕΞΑΝΔΡΟΣ Ο ΜΑΚΕΔΩΝ ΚΑΙ Η ΑΝΑΤΟΛΗ
   4: 938.498ΓΚΑ
   5: '15714'
   8: ΠΑΠΑΔΗΜΑ
   9: ΑΘΗΝΑ
   10: '1982'
   11: 735Σ
@@ -156843,15 +156902,15 @@
   12: ΘΕΑΤΡΟ
   13: ΘΕΑΤΡΟ
   14: ΘΕΑΤΡΟ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12379
   1: RICE,E.E
   2: ΑΛΕΞΑΝΔΡΟΣ Ο ΜΕΓΑΣ
-  4: 938.07RIC
+  4: 938.174RIC
   5: '15873'
   8: ΝΕΦΕΛΗ
   9: ΑΘΗΝΑ
   10: '2003'
   11: 87Σ
   12: ΒΙΟΓΡΑΦΙΑ
   13: ΒΙΟΓΡΑΦΙΑ
@@ -157360,15 +157419,15 @@
   12: ΔΗΜΟΚΡΑΤΙΑ-ΕΛΛΑΔΑ
   13: ΔΗΜΟΚΡΑΤΙΑ-ΕΛΛΑΔΑ
   14: ΔΗΜΟΚΡΑΤΙΑ-ΕΛΛΑΔΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12420
   1: ΠΑΒΑΓΙΩΤΙΔΟΥ,ΙΑΚΩΒΟΥ
   2: ΑΛΕΞΑΝΔΡΟΣ Ο ΠΑΜΜΕΓΙΣΤΟΣ
-  4: 938.07ΠΑΝ
+  4: 938.174ΠΑΝ
   5: '15829'
   8: ΓΕΩΡΓΙΑΔΗΣ
   9: ΑΘΗΝΑ
   10: '1998'
   11: 261Σ
   12: ΙΣΤΟΡΙΑ-ΑΛΕΞΑΝΔΡΟΣ
   13: ΙΣΤΟΡΙΑ-ΑΛΕΞΑΝΔΡΟΣ
@@ -158217,15 +158276,15 @@
   12: ΕΒΡΑΙΟΙ
   13: ΕΒΡΑΙΟΙ
   14: ΕΒΡΑΙΟΙ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12487
   1: ΧΡΗΣΤΟΥ,ΠΑΝΑΓΙΩΤΗ
   2: ΕΚΘΕΣΙΣ ΠΕΠΡΑΓΜΕΝΩΝ
-  4: 949.565ΧΡΗ
+  4: 949.498ΧΡΗ
   5: '15852'
   9: ΘΕΣ/ΝΙΚΗ
   10: '1968'
   11: 83Σ
   12: ΠΕΠΡΑΓΜΕΝΑ ΑΡΙΣΤΟΤΕΛΕΙΟΥ
   13: ΠΕΠΡΑΓΜΕΝΑ ΑΡΙΣΤΟΤΕΛΕΙΟΥ
   14: ΠΕΠΡΑΓΜΕΝΑ ΑΡΙΣΤΟΤΕΛΕΙΟΥ
@@ -159509,18 +159568,19 @@
   10: '2005'
   11: 53Σ
   12: ΘΡΗΣΚΕΙΑ
   13: ΘΡΗΣΚΕΙΑ
   14: ΘΡΗΣΚΕΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12590
-  1: ΖΩΙΔΗ,Γ.
+  1: ΚΟΛΟΜΠΟΒΑ,Κ.Μ
   2: Η ΖΩΗ ΣΤΗΝ ΑΡΧΑΙΑ ΕΛΛΑΔΑ
-  4: 938.498ΖΩΙ
+  4: 938.498ΚΟΛ
   5: '16064'
+  6: ΖΩΙΔΗ,Γ
   8: ΔΡΑΚΟΠΟΥΛΟΥ
   11: 223Σ
   12: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   13: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   14: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12591
@@ -159713,17 +159773,17 @@
   9: ΑΘΗΝΑ
   11: 292Σ
   12: ΒΙΟΓΡΑΦΙΑ
   13: ΒΙΟΓΡΑΦΙΑ
   14: ΒΙΟΓΡΑΦΙΑ
   17: ΔΩΡΕΑ ΚΩΝΣΤΑΝΤΙΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12606
-  1: ΣΤΥΛΙΑΝΟΣ ΧΡΑΠΗΣ
+  1: ΧΡΑΠΗΣ,ΣΤΥΛΙΑΝΟΣ
   2: Ο ΔΡΟΜΟΣ ΤΟΥ ΗΓΕΤΗ
-  4: 938.498ΣΤΥ
+  4: 938.07ΧΡΑ
   5: '16085'
   8: ΔΗΛΙΟΣ
   9: ΘΕΣ/ΚΗ
   11: 191Σ
   12: ΙΣΤΟΡΙΑ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΙΣΤΟΡΙΑ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   14: ΙΣΤΟΡΙΑ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -160071,17 +160131,17 @@
   10: '1967'
   11: 205Σ
   12: ΣΩΚΡΑΤΗΣ
   13: ΣΩΚΡΑΤΗΣ
   14: ΣΩΚΡΑΤΗΣ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12634
-  1: ΖΩΓΡΑΦΙΚΗ,ΓΕΩΡΓΙΟΥ
+  1: ΖΩΓΡΑΦΑΚΗ,ΓΕΩΡΓΙΟΥ
   2: ΘΕΣΣΑΛΟΝΙΚΗ
-  3: ΠΕΡΙΠΑΤΟΣ ΑΝΑ ΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΚΑΙ ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
+  3: ΠΕΡΙΠΑΤΟΣ ΑΝΑΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΚΑΙ ΤΑ ΜΝΗΜΕΙΑ ΤΗΣ
   4: 949.565ΖΩΓ
   5: '16070'
   8: ΜΑΣΤΟΡΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1967'
   11: 50Σ
   12: ΙΣΤΟΡΙΑ-ΘΕΣ/ΝΙΚΗ
@@ -161606,23 +161666,25 @@
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
   18: 978-960-87
   19: 037-2-8
 - 0: 12756
   1: ΦΙΝΛΕΥ,ΓΕΩΡΓΙΟΥ
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
   4: 938.6ΦΙΝ
-  5: '16201'
+  5: 16201-19214
   6: ΓΙΑΝΝΗ ΚΟΡΔΑΤΟΥ
   8: Ο ΚΟΣΜΟΑ
   9: ΑΘΗΝΑ
   11: 423Σ
   12: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
   13: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
   14: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
-  17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
+  17: ΤΟΜΟΙ 2
+  18: '9789606757'
+  19: '051'
 - 0: 12757
   1: ΣΚΟΥΤΕΛΑΣ,ΠΕΤΡΟΣ
   2: ΕΥΘΥΜΕΣ ΚΑΙ ΠΙΚΑΝΤΙΚΕΣ ΚΑΤΑΒΟΛΕΣ
   4: 398ΣΚΟ
   5: '16200'
   9: ΑΘΗΝΑ
   10: '2007'
@@ -162102,15 +162164,15 @@
   12: ΘΡΗΣΚΕΙΑ
   13: ΘΡΗΣΚΕΙΑ
   14: ΘΡΗΣΚΕΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12795
   1: ΠΕΤΡΑΚΑΚΟΥ.ΔΗΜΗΤΡΙΟΥ
   2: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  4: 938.07ΠΕΤ
+  4: 938.174ΠΕΤ
   5: '16269'
   9: ΑΘΗΝΑ
   10: '1944'
   11: 103Σ
   12: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   14: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -163777,14 +163839,15 @@
   12: ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ
   14: ΠΟΙΗΜΑΤΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12932
   1: Χ.Σ.
   2: ΟΔΗΓΟΣ ΤΗΣ ΘΑΣΟΥ
+  4: 914.009Χ.Σ
   5: '16411'
   8: ΓΑΛΛΙΚΗ ΑΡΧΣΙΟΛΟΓΙΚΗ
   9: ΑΘΗΝΑ
   10: '1974'
   11: 202Σ
   12: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΟΤΗΤΕΣ
   13: ΙΣΤΟΡΙΑ-ΑΡΧΑΙΟΤΗΤΕΣ
@@ -164210,18 +164273,18 @@
   10: '1974'
   11: 276Σ
   12: ΙΑΤΡΙΚΗ
   13: ΙΑΤΡΙΚΗ
   14: ΙΑΤΡΙΚΗ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12967
-  1: ΚΑΛΛΙΝΑΚΗ,ΜΑΡΙΑ-ΓΟΥΔΗΣ,ΧΡΙΣΤΟΣ
+  1: ΓΟΥΔΗΣ,ΧΡΙΣΤΟΣ-ΚΑΛΛΙΝΑΚΗ ΜΑΡΙΑ
   2: 1821 Η ΕΙΚΟΝΟΓΡΑΦΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΗΣ
   3: Α.Η ΕΠΟΧΗ ΤΗΑ ΑΥΤΟΓΝΩΣΙΑΣ Β.Η ΜΕΓΑΛΗ ΕΚΡΗΞΗ Γ. Η ΔΙΚΑΙΩΣΗ
-  4: 938ΚΑΛ
+  4: 938ΓΟΥ
   5: '16460'
   8: ΚΑΔΜΟΣ
   9: ΑΘΗΝΑ
   10: '2012'
   11: 295Σ
   12: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   13: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
@@ -164526,31 +164589,31 @@
   10: '1997'
   11: 69Σ
   12: ΑΜΒΡΑΚΙΚΟΣ
   13: ΑΜΒΡΑΚΙΚΟΣ
   14: ΑΜΒΡΑΚΙΚΟΣ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12990
-  1: ΤΕΡΖΟΠΟΥΛΟΥ,ΛΟΛΑ,ΠΑΤΣΑΛΙΑ,ΚΑΤΕΡΙΝΑ
+  1: ΠΑΤΣΑΛΙΑ,ΚΑΤΕΡΙΝΑ,ΤΕΡΖΟΠΟΥΛΟΥ,ΛΟΛΑ
   2: ΝΟΜΟΛΟΓΙΑ ΤΟΥ ΠΡΩΤΟΔΙΚΕΙΟΥ ΑΡΤΗΣ ΕΠΙ ΤΟΥ ΑΓΡΟΤΙΚΟΥ ΖΗΤΗΜΑΤΟΣ
-  4: 938.65ΤΕΡ
-  5: '16456'
+  4: 938.65ΠΑΤ
+  5: 16456-17229
   8: Μ/Φ ΣΥΛΛΟΓΟΣ ΣΚΟΥΦΑΣ
   9: ΑΡΤΑ
   10: '1981'
   11: 31Σ
   12: ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
   13: ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
   14: ΑΓΡΟΤΙΚΟ ΖΗΤΗΜΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 12991
   1: Χ.Σ.
   2: ΠΑΙΔΕΣ ΕΛΛΗΝΩΝ ΙΤΕ
   4: 938ΚΑΣ
-  5: '16506'
+  5: 16506-10043
   8: ΑΚΑΔΗΜΙΑ ΑΘΗΝΩΝ
   9: ΑΘΗΝΑ
   10: '1972'
   11: 18Σ
   12: ΠΑΝΗΓΥΡΙΚΗ ΣΥΝΕΔΡΙΑ
   13: ΠΑΝΗΓΥΡΙΚΗ ΣΥΝΕΔΡΙΑ
   14: ΠΑΝΗΓΥΡΙΚΗ ΣΥΝΕΔΡΙΑ
@@ -165043,16 +165106,16 @@
   12: ΠΝΕΥΜΑΤΙΚΗ ΖΩΗ
   13: ΠΝΕΥΜΑΤΙΚΗ ΖΩΗ
   14: ΠΝΕΥΜΑΤΙΚΗ ΖΩΗ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 13031
   1: NATIONAL GEOGRAPHIC
   2: Η ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ 1453
-  4: 949.504Χ.Σ
-  5: '16502'
+  4: 938.389Χ.Σ
+  5: 16502-12662
   11: 159Σ
   12: ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
   13: ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
   14: ΑΛΩΣΗ ΤΗΣ ΠΟΛΗΣ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 13032
   1: ΑΘΑΝΑΣΟΓΛΟΥ,ΝΙΝΑ
@@ -165542,15 +165605,15 @@
   17: ΔΩΡΕΑ ΛΑΜΠΡΙΝΗΣ ΕΞΑΡΧΟΥ
   18: 960-8305-0
   19: 1-2
   30: ΤΟΜΟΙ 3
 - 0: 13069
   1: Χ.Σ
   2: ΘΗΣΑΥΡΟΙ ΤΗΣ ΑΡΜΕΝΙΑΣ
-  4: 938ΑΡΜ
+  4: 938Χ.Σ
   5: '16558'
   8: ΙΟΝΙΚΗ ΤΡΑΠΕΖΑ
   9: ΑΘΗΝΑ
   10: '1998'
   11: 240Σ
   12: ΠΟΛΙΤΙΣΜΟΣ-ΑΡΜΕΝΙΑ
   13: ΠΟΛΙΤΙΣΜΟΣ-ΑΡΜΕΝΙΑ
@@ -167563,15 +167626,15 @@
   14: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΚΑΙ ΕΛΕΝΗΣ ΚΟΙΛΙΑ
   18: 960-8094-1
   19: 4-3
 - 0: 13207
   1: ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
   2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
-  4: 938.07ΚΑΡ
+  4: 938.174ΚΑΡ
   5: '16650'
   8: REAL MEDIA
   9: ΑΘΗΝΑ
   10: '2014'
   11: 271Σ
   12: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -167767,15 +167830,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-87522-
   19: 9-9
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 13220
   1: ΕΥΑΓΓΕΛΙΔΗΣ,ΜΑΡΓΑΡΙΤΗΣ
   2: Η ΜΗΧΑΝΙΩΝΑ ΤΗΣ ΚΥΖΙΚΟΥ ΙΣΤΟΡΙΑ ΚΑΙ ΠΑΡΑΔΟΣΙΣ
-  4: 938.498ΕΥΑ
+  4: 938.494ΕΥΑ
   5: '16704'
   8: ΕΤ.ΜΕΛ.ΑΝΑΤΟΛΗΣ
   9: ΑΘΗΝΑ
   10: '2005'
   11: 311Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
@@ -170726,23 +170789,23 @@
   13: ΞΕΝΠΓΛΩΣΣΟ
   14: ΞΕΝΠΓΛΩΣΣΟ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 13432
   1: ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
   2: Η ΕΠΙΣΤΡΟΦΗ
   3: Η ΑΛΗΘΙΝΗ ΙΣΤΟΡΙΑ ΤΟΥ ΜΙΧΑΗΛ ΘΕΟΔΟΡΟΒΙΤΣ ΚΥΡΙΑΚΟΒ
-  4: 889.21ΠΑΠ
+  4: 938.498ΠΑΠ
   5: '16946'
   8: ΔΙΟΠΤΡΑ
   9: ΑΘΗΝΑ
   10: '2012'
   11: 528Σ
-  12: ΛΟΓΟΤΕΧΝΙΑ
-  13: ΛΟΓΟΤΕΧΝΙΑ
-  14: ΛΟΓΟΤΕΧΝΙΑ
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-36
   19: 4-469-9
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 13433
   1: ΠΟΛΥΧΡΟΝΙΔΗΣ,ΧΡΗΣΤΟΣ
   2: ΤΡΑΝΤΕΛΛΕΝΟΙ ... ΚΑΙ ΠΕΡΑ ΑΠΟ ΤΟ ΘΑΝΑΤΟ
@@ -170758,15 +170821,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-8229-4
   19: 8-0
 - 0: 13434
   1: ΦΕΣΤΕΡΙΔΗΣ,ΤΑΣΟΣ
   2: Η ΕΛΛΗΝΙΚΗ ΠΟΝΤΙΑΚΗ ΚΟΙΝΟΤΗΤΑ ΤΟΥ ΜΕΤΑΛΛΕΙΟΥ ΤΑΥΡΟΥ (ΜΠΟΥΓΑ
   3: ΜΑΝΤΕΝ) ΤΗΣ ΜΙΚΡΑΣ ΑΣΙΑΣ
-  4: 938.993ΦΕΣ
+  4: 938.498ΦΕΣ
   5: '16947'
   8: ΜΕΛΙΣΣΑ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1999'
   11: 271Σ
   12: ΙΣΤΟΡΙΑ-ΛΑΟΓΡΑΦΙΑ
   13: ΙΣΤΟΡΙΑ-ΛΑΟΓΡΑΦΙΑ
@@ -173133,15 +173196,15 @@
   14: ΠΟΛΙΤΙΚΗ
   17: ΔΩΡΕΑ ΚΩΣΤΑΣ ΜΠΑΝΙΑΣ
   18: 960-85076-
   19: 0-Χ
 - 0: 13604
   1: ΟΙΚΟΝΟΜΙΔΗ,ΦΟΙΒΟΥ
   2: ΟΙ ΠΡΟΣΤΑΤΕΣ Η ΑΛΗΘΙΝΗ ΙΣΤΟΡΙΑ ΤΗΣ ΑΝΤΙΣΤΑΣΗΣ
-  4: 320ΟΙΚ
+  4: 938.760ΟΙΚ
   5: '17106'
   8: ΟΡΦΕΑΣ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 431Σ
   12: ΠΟΛΙΤΙΚΗ
   13: ΠΟΛΙΤΙΚΗ
@@ -173540,28 +173603,28 @@
   12: ΠΛΟΥΤΑΡΧΟΣ
   13: ΠΛΟΥΤΑΡΧΟΣ
   14: ΠΛΟΥΤΑΡΧΟΣ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
   18: 960-316-24
   19: 6-9
 - 0: 13632
-  1: ΣΠΗΛΙΟΣ,ΑΠΟΣΤΟΛΟΣ
-  2: ΠΕΛΑΣΓΙΚΗ ΗΠΕΙΡΟΣ ΚΑΙ ΑΡΑΧΘΟΣ Ο ΠΕΛΑΣΓΙΚΟΣ
-  4: 938.939ΣΠΗ
-  5: '17184'
-  8: ΝΕΑ ΘΕΣΙΣ
+  1: Χ.Σ
+  2: 28 ΟΚΤΩΒΡΙΟΥ 1940
+  3: 70 ΧΡΟΝΙΑ ΜΕΤΑ
+  4: 938.752Χ.Σ
+  5: '21620'
+  8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
-  10: '2002'
-  11: 151Σ
-  12: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΑΡΑΧΘΟΣ
-  13: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΑΡΑΧΘΟΣ
-  14: ΗΠΕΙΡΟΣ-ΑΡΑΧΘΟΣ
-  17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
-  18: 960-7076-0
-  19: 9-5
+  10: '2010'
+  11: '78'
+  12: ΙΣΤΟΡΙΑ-28 ΟΚΤΩΒΡΙΟΥ
+  13: ΙΣΤΟΡΙΑ-28 ΟΚΤΩΒΡΙΟΥ
+  14: 28 ΟΚΤΩΒΡΙΟΥ
+  18: '9789604751'
+  19: '662'
 - 0: 13633
   1: ΠΑΣΧΑΛΙΔΗΣ,ΝΙΚΟΣ
   2: ΥΠΟΨΙΑ ΦΟΝΟΥ
   4: 889.21ΠΑΣ
   5: '17197'
   9: ΘΕΣ/ΝΙΚΗ
   10: '1972'
@@ -173664,15 +173727,15 @@
   14: ΙΣΤΟΡΙΑ-ΦΙΛΛΙΠΟΣ-ΑΛΕΞΑΝΔΡΟΣ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
   18: 960-01-041
   19: 9-0
 - 0: 13641
   1: ΣΔΡΑΚΑ,ΕΥΑΓΓΕΛΟΥ
   2: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΩΣ ΥΙΟΣ ΤΟΥ ΘΕΟΥ ΑΜΜΩΝΟΣ-ΔΙΟΣ
-  4: 938.070ΣΔΡ
+  4: 938.174ΣΔΡ
   5: '17182'
   8: ΚΥΡΟΜΑΝΟΣ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1995'
   11: 170Σ
   12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -173959,30 +174022,30 @@
   14: ΛΑΟΓΡΑΦΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
   18: 978-960-89
   19: 404-2-0
 - 0: 13663
   1: FAURE,PAUL
   2: Η ΚΑΘΗΜΕΡΙΝΗ ΖΩΗ ΤΗΝ ΕΠΟΧΗ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
-  4: 938.070FAU
+  4: 938.174FAU
   5: '17158'
   8: ΠΑΠΑΔΗΜΑ
   9: ΑΘΗΝΑ
   10: '1977'
   11: 400Σ
   12: ΙΣΤΟΡΙΑ-ΜΕΓΑΛΟΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΙΣΤΟΡΙΑ-ΜΕΓΑΛΟΣ ΑΛΕΞΑΝΔΡΟΣ
   14: ΙΣΤΟΡΙΑ-ΜΕΓΑΛΟΣ ΑΛΕΞΑΝΔΡΟΣ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
   18: 960-206-15
   19: 9-6
 - 0: 13664
   1: STONEMAN,RICHARD
   2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΘΡΥΛΟΣ-ΜΥΘΟΣ-ΙΣΤΟΡΙΑ
-  4: 938.070STO
+  4: 938.174STO
   5: '17159'
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '1993'
   11: 279Σ
   12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΚΑΝΔΡΟΣ
@@ -174336,15 +174399,15 @@
   12: ΟΙΚΟΓΕΝΕΙΑΚΟ ΔΙΚΑΙΟ
   13: ΟΙΚΟΓΕΝΕΙΑΚΟ ΔΙΚΑΙΟ
   14: ΟΙΚΟΓΕΝΕΙΑΚΟ ΔΙΚΑΙΟ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 13692
   1: ΧΡΥΣΑΝΘΟΠΟΥΛΟΥ,ΦΩΤΙΟΥ
   2: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ ΠΕΡΙ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
-  4: 938.509ΦΩΤ
+  4: 938.509ΧΡΥ
   5: '17188'
   9: ΑΘΗΝΑ
   10: '1899'
   11: 470Σ
   12: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   13: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   14: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
@@ -176042,15 +176105,15 @@
   13: ΘΡΗΣΚΕΙΑ
   14: ΘΡΗΣΚΕΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
   18: 960-7553-0
   19: 0-4
 - 0: 13828
   1: ΝΤΑΛΑ,ΧΡΗΣΤΟΥ
-  2: ΤΟ ΔΙΑΣΤΡΑΤΟ ΠΟΥ ΑΓΑΠΗΣΑΜΕ
+  2: ΤΟ ΔΙΣΤΡΑΤΟ ΠΟΥ ΑΓΑΠΗΣΑΜΕ
   4: 938.939ΝΤΑ
   5: '17329'
   9: ΑΘΗΝΑ
   10: '2008'
   11: 191Σ
   12: ΙΣΤΟΡΙΑ-ΔΙΣΤΡΑΤΟ
   13: ΙΣΤΟΡΙΑ-ΔΙΣΤΡΑΤΟ
@@ -176412,27 +176475,23 @@
   10: '1986'
   11: 112Σ
   12: ΞΕΝΟΓΛΩΣΣΟ-ΙΣΤΟΡΙΑ
   13: ΞΕΝΟΓΛΩΣΣΟ-ΙΣΤΟΡΙΑ
   14: ΞΕΝΟΓΛΩΣΣΟ-ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 13858
-  1: ΚΑΡΓΑΚΟΣ,ΣΑΡΑΝΤΟΣ
-  2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ Ο ΑΝΘΡΩΠΟΣ ΦΑΙΝΟΜΕΝΟ
-  4: 938.070ΚΑΡ
-  5: '17352'
-  8: REAL NEWS
-  9: ΑΘΗΝΑ
-  10: '2014'
-  11: 224Σ
-  12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  14: ΙΣΤΟΡΙΑ -ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
-  30: ΤΟΜΟ Β-Γ
+  1: ΤΕΛΩΝΑ,ΝΙΚΟΛΑΟΥ
+  2: ΤΑ ΕΝ ΚΑΡΒΑΣΑΡΑ ΑΠΟ ΤΗΣ ΕΝΑΡΞΕΩΣ ΤΟΥ ΙΕΡΟΥ ΑΓΩΝΟΣ
+  4: 938.22ΤΕΛ
+  5: '13207'
+  8: ΒΙΒΛΙΟΘΗΚΗ ΑΜΦΙΛΟΧΙΑ
+  11: '238'
+  12: ΙΣΤΟΡΙΑ-ΚΑΡΒΑΣΑΡΑΣ
+  13: ΙΣΤΟΡΙΑ-ΚΑΡΒΑΣΑΡΑΣ
+  14: ΙΣΤΟΡΙΑ-ΚΑΡΒΑΣΑΡΑΣ
 - 0: 13859
   1: ΣΦΕΝΔΟΝΗ,Ν.
   2: ΜΑΚΕΔΟΝΙΚΟΝ ΗΜΕΡΟΛΟΓΙΟΝ
   4: 889.21ΣΦΕ
   5: '17370'
   9: ΘΕΣ/ΝΙΚΗ
   10: '1925'
@@ -176834,14 +176893,15 @@
   13: ΑΡΧΑΙΟΛΟΓΙΑ
   14: ΑΡΧΑΙΟΛΟΓΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 13891
   1: FASSO,GUIDO
   2: Η ΔΗΜΟΚΡΑΤΙΑ ΣΤΗΝ ΕΛΛΑΔΑ
   4: 938FAS
+  5: '17420'
   8: ΠΟΣΕΙΔΩΝΑΣ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1971'
   11: 176Σ
   12: ΠΟΛΙΤΙΚΗ
   13: ΠΟΛΙΤΙΚΗ
   14: ΠΟΛΙΤΙΚΗ
@@ -176867,28 +176927,25 @@
   10: '1994'
   11: 273Σ
   12: ΘΡΗΣΚΕΙΑ
   13: ΘΡΗΣΚΕΙΑ
   14: ΘΡΗΣΚΕΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 13894
-  1: ΤΖΙΚΟΥ,ΦΩΤΕΙΝΗ
-  2: Ο ΑΓΝΩΣΤΟΣ ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  4: 938.07ΤΖΙ
-  5: '17408'
-  8: ΑΡΧΕΤΥΠΟ
-  9: ΑΘΗΝΑ
-  10: '2004'
-  11: 254Σ
-  12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  14: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
-  18: 960-421-03
-  19: 0-0
+  1: ΨΗΜΜΕΝΟΥ,ΝΙΚΟΥ
+  2: ΑΙΤΩΛΟΑΚΑΡΝΑΝΕΣ ΛΟΓΙΟΙ
+  4: 938.22ΨΗΜ
+  5: '21490'
+  8: ΔΩΤΙΟΝ
+  9: ΙΩΑΝΝΙΝΑ
+  10: '2021'
+  11: '95'
+  12: ΛΟΓΙΟΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
+  13: ΛΟΓΙΟΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
+  14: ΛΟΓΙΟΙ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
 - 0: 13895
   1: Χ.Σ
   2: Η ΙΣΤΟΡΙΑ ΤΟΥ ΕΘΝΙΚΟΥ ΔΙΧΑΣΜΟΥ
   4: 938.7ΙΣΤ
   5: '17409'
   8: ΚΥΡΟΜΑΝΟΣ
   9: ΘΕΣ/ΝΙΚΗ
@@ -177319,23 +177376,23 @@
   10: '1972'
   11: 137Σ
   12: ΤΡΑΓΩΔΙΑ
   13: ΤΡΑΓΩΔΙΑ
   14: ΤΡΑΓΩΔΙΑ
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
 - 0: 13928
-  1: ΣΔΡΑΚΑ,ΕΥΑΓΓΕΛΟΥ
-  2: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΩΣ ΥΙΟΣ ΤΟΥ ΘΕΟΥ ΑΜΜΩΝΟΣ-ΔΙΟΣ
-  9: ΘΕΣ/ΝΙΚΗ
-  10: '1971'
-  11: 110Σ
-  12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  13: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  14: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
-  17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
+  1: ΓΡΗΓΟΡΟΓΙΑΝΝΗ,Α.
+  2: Ο ΜΕΙΖΩΝ ΕΛΛΗΝΙΣΜΟΣ
+  4: 938.1ΓΡΗ
+  5: '21549'
+  8: ΕΚΔΟΣΕΙΣ ΑΣΕ Α.Ε
+  11: '235'
+  12: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
+  13: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
+  14: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
 - 0: 13929
   1: ΠΑΝΤΑΖΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΥ
   2: Ο ΑΡΙΣΤΟΤΕΛΗΣ ΚΑΙ ΟΙ ΣΟΦΙΣΤΕΣ
   4: 882ΠΑΝ
   5: '17438'
   9: ΘΕΣ/ΝΙΚΗ
   10: '1980'
@@ -178328,15 +178385,15 @@
   17: ΔΩΡΕΑ ΚΩΝ/ΝΟΥ ΤΣΙΛΙΓΙΑΝΝΗ
   18: 978-960-19
   19: -0038-4
 - 0: 14008
   1: Χ.Σ.
   2: ΕΚΘΕΣΙΣ ΤΩΝ ΓΕΝΟΜΕΝΩΝ ΖΗΜΙΩΝ ΕΝ ΓΕΝΕΙ ΗΠΕΙΡΟΥ ΑΠΟ ΤΗΣ ΚΗΡΥΞΕ
   3: ΤΟΥ ΕΛΛΗΝΟΙΤΑΛΙΚΟΥ ΜΕΧΡΙ ΤΗΣ ΑΠΕΛΕΥΘΕΡΩΣΕΩΣ ΤΗΣ ΟΚΤΩΒΡΙΟΣ 44
-  4: 938.752ΕΚΘ
+  4: 938.752Χ.Σ
   5: '17525'
   9: ΑΘΗΝΑ
   10: '1987'
   11: 175Σ
   12: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ-ΗΠΕΙΡΟΣ
   13: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ-ΑΡΤΑ
   14: ΕΛΛΗΝΟΙΤΑΛΙΚΟΣ ΠΟΛΕΜΟΣ-ΙΣΤΟΡΙΑ
@@ -178778,15 +178835,15 @@
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 14045
   1: ΟΙΚΟΝΟΜΟΥ,ΜΑΝΘΟΥ
   2: ΜΑΝΘΟΣ ΟΙΚΟΝΟΜΟΥ Ο ΠΡΩΘΥΠΟΥΡΓΟΣ ΤΟΥ ΑΛΗ ΠΑΣΑ
-  4: 938.484ΟΙΚ
+  4: 938.494ΟΙΚ
   5: '17568'
   8: ΗΠΕΙΡΩΤΙΚΗ ΕΣΤΙΑ
   9: ΙΩΑΝΝΙΝΑ
   10: '1959'
   11: 16Σ
   12: ΙΣΤΟΡΙΑ-ΑΛΗ ΠΑΣΑ
   13: ΙΣΤΟΡΙΑ-ΑΛΗ ΠΑΣΑ
@@ -179745,15 +179802,15 @@
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   18: 978-618-51
   19: 45-24-8
 - 0: 14116
   1: Χ.Σ.
   2: ΣΚΟΤΕΙΝΗ ΕΠΤΑΕΤΙΑ
   3: 1967-1974 Η ΔΙΚΤΑΤΟΡΙΑ ΤΩΝ ΣΥΝΤΑΓΜΑΤΑΡΧΩΝ
-  4: 938.79ΣΚΟ
+  4: 938.79Χ.Σ
   5: '1707'
   8: ΙΔΡΥΜΑ ΒΟΥΛΗ ΕΛΛΗΝΩΝ
   9: ΑΘΗΝΑ
   10: '2014'
   11: 167Σ
   12: ΙΣΤΟΡΙΑ-ΔΙΚΤΑΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ-ΔΙΚΤΑΤΟΡΙΑ
@@ -181675,15 +181732,15 @@
   14: ΠΟΛΕΜΟΣ 1912-13-ΜΑΚΕΔΟΝΙΑ-ΗΠΕΙΡΟΣ
   17: ΔΩΡΕΑ ΙΔΡΥΜΑ ΒΟΥΛΗΣ ΤΩΝ ΕΛΛΗΝΩΝ
   18: 978-960-67
   19: 57-59-4
 - 0: 14255
   1: ΑΜΠΑΤΖΗ,ΕΥΡΙΔΙΚΗ
   2: Η ΑΤΤΙΚΗ ΓΗ ΥΠΟΔΕΧΕΤΑΙ ΤΟΥΣ ΠΡΟΣΦΥΓΕΣ ΤΟΥ 22
-  4: 362.870ΑΜΠ
+  4: 938.498ΑΜΠ
   5: '17720'
   8: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ
   9: ΑΘΗΝΑ
   10: '2016'
   11: 193Σ
   12: ΠΡΟΣΦΥΓΕΣ 22
   13: ΠΡΟΣΦΥΓΕΣ 22
@@ -181748,18 +181805,18 @@
   12: ΦΙΛΟΣΟΦΙΑ ΣΤΗΝ ΑΡΧΑΙΑ ΕΛΛΑΔΑ-ΠΟΛΙΤΙΚΗ
   13: ΦΙΛΟΣΟΦΙΑ ΣΤΗΝ ΑΡΧΑΙΑ ΕΛΛΑΔΑ-ΠΟΛΙΤΙΚΗ
   14: ΦΙΛΟΣΟΦΙΑ ΣΤΗΝ ΑΡΧΑΙΑ ΕΛΛΑΔΑ-ΠΟΛΙΤΙΚΗ
   17: ΔΩΡΕΑ ΙΔΡΥΜΑ ΒΟΥΛΗΣ ΤΩΝ ΕΛΛΗΝΩΝ
   18: 978-960-67
   19: 57-58-7
 - 0: 14260
-  1: ΓΟΥΝΑΡΗΣ,ΒΑΣΙΛΗΣ
+  1: Χ.Σ
   2: ΤΟ ΑΓΝΩΣΤΟ ΜΕΤΩΠΟ ΤΩΝ ΒΑΛΚΑΝΙΚΩΝ ΠΟΛΕΜΩΝ
   3: Η ΔΙΟΙΚΗΤΙΚΗ ΕΝΣΩΜΑΤΩΣΗ ΤΩΝ ΝΕΩΝ ΧΩΡΩΝ
-  4: 938.683ΓΟΥ
+  4: 938.683Χ.Σ
   5: '17721'
   8: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ
   9: ΑΘΗΝΑ
   10: '2012'
   11: 190Σ
   12: ΒΑΛΚΑΝΙΚΟΣ ΠΟΛΕΜΟΣ-ΕΝΣΩΜΑΤΩΣΗ
   13: ΒΑΛΚΑΝΙΚΟΣ ΠΟΛΕΜΟΣ-ΕΝΣΩΜΑΤΩΣΗ
@@ -182029,14 +182086,15 @@
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΣΗ
   18: 960-7290-8
   19: 0-1
 - 0: 14278
   1: ΒΑΚΑΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
   2: ΠΡΩΙΜΟΙ ΑΠΕΛΕΥΘΕΡΩΤΙΚΟΙ ΑΓΩΝΕΣ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΤΑ ΤΗΝ ΟΘΩΜΑΝΟΚ
   3: ΡΑΤΙΑ (1453-1669) ΠΟΛΕΜΙΚΑ,ΠΟΛΙΤΙΚΑ ΚΑΙ ΘΡΗΣΚΕΥΤΙΚΑ ΓΕΓΟΝΟΤΑ
+  4: 938.498ΒΑΚ
   5: '17772'
   8: ΑΝΤ.ΣΤΑΜΟΥΛΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2000'
   11: 642Σ
   12: ΟΘΩΜΑΝΟΚΡΑΤΙΑ
   13: ΟΘΩΜΑΝΟΚΡΤΑΙΑ
@@ -182346,15 +182404,15 @@
   14: ΙΣΤΟΡΙΑ-ΠΡΟΣΦΥΓΕΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 960-7290-7
   19: 1-2
 - 0: 14299
   1: ΖΟΥΡΑΒΛΙΟΒΑ-ΠΑΠΠΟΥ,ΑΙΚΑΤΕΡΙΝΗ
   2: ΓΛΩΣΣΑ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΑΖΟΦΙΚΗΣ
-  4: 956,5ΖΟΥ
+  4: 983.498ΖΟΥ
   5: '17777'
   8: ΑΝΤ.ΣΤΑΜΟΥΛΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2009'
   11: 477Σ
   12: ΠΑΙΔΕΙΑ
   13: ΠΑΙΔΕΙΑ
@@ -182870,15 +182928,15 @@
   15: ΠΡΑΚΤΙΚΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: 978-960-67
   19: 57-19-8
 - 0: 14333
   1: Χ.Σ.
   2: ΣΥΝΤΑΓΜΑΤΙΚΑ ΚΕΙΜΕΝΑ ΤΗΣ ΗΓΕΜΟΝΙΑΣ ΣΑΜΟΥ
-  4: 938.75ΣΥΝ
+  4: 938.75Χ.Σ
   5: '17803'
   8: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ
   9: ΑΘΗΝΑ
   10: '2013'
   11: 534Σ
   12: ΣΥΝΤΑΓΜΑΤΙΚΑ ΚΕΙΜΕΝΑ-ΣΑΜΟΣ
   13: ΣΥΝΤΑΓΜΑΤΙΚΑ ΚΕΙΜΕΝΑ-ΣΑΜΟΣ
@@ -184048,15 +184106,15 @@
   14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: '9789607957'
   19: '498'
 - 0: 14427
   1: ΤΣΙΡΚΙΝΙΔΗ,ΧΑΡΗ
   2: ΑΓΩΝΕΣ ΧΩΡΙΣ ΔΙΚΑΙΩΣΗ
-  4: 938.498ΤΣΙ
+  4: 938.473ΤΣΙ
   5: '17855'
   8: ΕΡΩΔΙΟΣ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2002'
   11: 361Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
@@ -184124,30 +184182,30 @@
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: '9789602440'
   19: 087
 - 0: 14432
   1: ΣΥΜΕΩΝΙΔΟΥ-ΠΑΠΑΔΟΠΟΥΛΟΥ,ΠΑΡΥΣΑΤΙΣ
   2: ΤΡΑΠΕΖΟΥΣ Η ΠΟΛΗ ΣΤΟ ΦΩΣ ΤΟΥ ΠΟΛΙΤΙΣΜΟΥ ΤΗΣ
-  4: 938.498SYM
+  4: 938.498ΣΥΜ
   5: '17848'
   8: UNIVERSITY STUDIO
   9: ΘΕΣ/ΝΙΚΗ
   10: '2011'
   11: 415Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   19: '9789601219'
   22: '691'
 - 0: 14433
   1: ΧΡΗΣΤΟΥ,ΣΤΑΥΡΟΣ
   2: ΟΙ ΕΛΛΗΝΕΣ ΣΤΗ ΝΟΤΙΑ ΡΩΣΙΑ
-  4: 938.993ΣΤΑ
+  4: 938.498ΧΡΗ
   5: '17847'
   8: UNIVERSITY STUDIO
   9: ΘΕΣ/ΝΙΚΗ
   10: '2009'
   11: 169Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
@@ -184194,15 +184252,15 @@
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: '9609308458'
 - 0: 14437
   1: Χ.Σ.
-  2: ΜΟΝΟΓΡΑΦΙΕΣ Η ΠΡΩΤΗ ΝΙΚΞΗ 1940-1941
+  2: ΜΟΝΟΓΡΑΦΙΕΣ Η ΠΡΩΤΗ ΝΙΚΗ 1940-1941
   4: 938.498ΜΟΝ
   5: '17868'
   8: NATONAL GEOGRAPHIC
   9: ΑΘΗΝΑ
   10: '2010'
   11: 158Σ
   12: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ
@@ -184340,14 +184398,15 @@
   18: '9789604887'
   19: '972'
   30: ΤΟΜΟΙ 1-2-3-4
 - 0: 14446
   1: ΜΠΑΕΤΕΝ.ΛΙΒΕ-ΜΠΕΝΚΕ-ΚΟΥΝΤΣΛΕΡ,ΡΟΖΜΑΡΙ
   2: ΑΛΛΟΣ ΓΙΑ ΤΟ ΝΗΠΙΑΓΩΓΕΙΟ
   4: 808.899ΜΠΑ
+  5: '17880'
   6: ΜΑΡΙΑ ΑΓΓΕΛΙΔΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 20Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -184406,14 +184465,15 @@
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΑΦΡΟΔΙΤΗΣ ΚΑΤΣΑΟΥΝΟΥ
 - 0: 14451
   1: CARMI,EUGENIO-ECO,UMBERTO
   2: ΟΙ ΝΑΝΟΙ ΤΟΥ ΓΚΝΟΥ
   4: 808.899ECO
+  5: '17873'
   6: ΕΦΗ ΚΑΛΛΙΦΑΤΙΔΗ
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 36Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -185617,17 +185677,17 @@
   12: ΠΑΙΔΕΙΑ
   13: ΠΑΙΔΕΙΑ
   14: ΠΑΙΔΕΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: '11090871'
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 14536
-  1: ΚΥΡΙΑΚΟΥ-ΞΑΝΘΟΠΟΥΛΟΥ,ΑΡΤΕΜΙΣ
+  1: ΧΑΤΖΗΚΥΡΙΑΚΙΔΗΣ,ΚΥΡΙΑΚΟΣ-ΚΥΡΙΑΚΟΥ ΑΡΤΕΜΙ
   2: ΟΙ ΕΛΛΗΝΕΣ ΤΟΥ ΠΟΝΤΟΥ ΚΑΙ Η ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ 1461-1923
-  4: 938.498ΚΥΡ
+  4: 938.4ΧΑΤ
   5: '17960'
   9: ΑΘΗΝΑ
   10: '2015'
   11: 436Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -189614,17 +189674,17 @@
   10: '1999'
   11: 151Σ
   12: ΜΕΛΕΤΕΣ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΜΕΛΕΤΕΣ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΕΛΕΤΕΣ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: '9603604992'
 - 0: 14829
-  1: ΤΖΟΡΙ,ΤΖΟΝ-ΜΠΑΡΝΕΤ,ΜΑΚ
+  1: ΜΠΑΡΝΕΤ,ΜΑΚ-ΤΖΟΡΙ,ΤΖΟΝ
   2: ΤΟ ΤΡΟΜΕΡΟ ΔΙΔΥΜΟ
-  4: 808.899ΤΖΟ
+  4: 808.899ΜΠΑ
   5: '19656'
   6: ΕΥΓΕΝΙΑ ΚΟΛΥΔΑ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2015'
   11: 227Σ
   12: ΝΕΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -191005,15 +191065,15 @@
   10: '2000'
   11: 34Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: '9605351390'
 - 0: 14928
-  1: ΝΙΚΟΛΑΟΠΟΥΛΟΥ,ΑΓΓΕΛΙΚΗ
+  1: ΝΙΚΟΛΟΠΟΥΛΟΥ,ΑΓΓΕΛΙΚΗ
   2: ΟΤΑΝ ΟΙ ΠΕΡΣΕΣ
   4: 808.899ΝΙΚ
   5: '19902'
   8: ΑΣΤΕΡΟΣ
   9: ΑΘΗΝΑ
   10: '1994'
   11: 225Σ
@@ -191750,14 +191810,16 @@
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 14982
   1: ΚΟΝΤΑΡΑΣ,ΘΟΔΩΡΗΣ
   2: ΟΙ ΤΕΛΕΥΤΑΙΕΣ ΣΤΙΓΜΕΣ ΤΩΝ ΕΛΛΗΝΙΚΩΝ ΒΟΥΡΛΩΝ
+  4: 938.498ΚΟΝ
+  5: '22885'
   8: ΜΠΑΛΤΑ
   9: ΑΘΗΝΑ
   10: '2018'
   11: 79Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -192124,14 +192186,15 @@
   14: ΤΣΑΡΙΚΗ ΡΩΣΙΑ
   17: ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: '9789609533'
   19: '393'
 - 0: 15008
   1: ΣΥΜΕΩΝΙΔΟΥ-ΠΑΠΑΔΟΠΟΥΛΟΥ,ΠΑΡΥΣΑΤΙΣ
   2: ΠΛΗΘΥΣΜΙΑΚΟΙ ΣΤΡΟΒΙΛΟΙ ΣΤΟΝ 21 ΑΙΩΝΑ
+  4: 938.43ΣΥΜ
   5: '19968'
   8: ΚΥΡΙΑΚΙΔΗ
   9: ΘΕΣ/ΝΙΚΗ
   10: '2016'
   11: 205ΣΙΣ
   12: ΙΣΤΟΡΙΑ-ΠΛΗΘΥΣΜΟΣ
   13: ΣΥΡΙΑ-ΕΛΛΑΔΑ
@@ -193269,14 +193332,15 @@
   13: ΕΚΠΑΙΔΕΥΤΙΚΟ ΒΙΒΛΙΟ
   14: ΕΚΠΑΙΔΕΥΤΙΚΟ ΒΙΒΛΙΟ
   18: 690423661Χ
 - 0: 15089
   1: BLYTON,ENID
   2: ΤΑ ΠΕΝΤΕ ΛΑΓΩΝΙΚΑ ΤΟ ΜΥΣΤΗΡΙΟ ΤΟΥ ΣΚΟΤΕΙΝΟΥ ΣΠΙΤΙΟΥ
   4: 808.899BLY
+  5: '20080'
   6: ΚΩΣΤΑΣ ΓΙΟΥΡΓΟΣ
   8: GUTENBERG
   9: ΑΘΗΝΑ
   11: 181Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -194725,15 +194789,15 @@
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΒΑΣΙΛΙΚΗΣ ΤΣΩΝΟΥ
 - 0: 15196
   1: ΤΣΕΧΩΦ,ΑΝΤΟΝ
   2: ΤΑ ΠΑΙΔΙΚΑ ΔΙΓΗΜΑΤΑ
   4: 808.899ΤΣΕ
-  5: '20164'
+  5: '20161'
   6: ΓΙΩΡΓΗΣ ΠΟΛΙΤΟΠΟΥΛΟΣ
   8: ΓΛΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1981'
   11: 117Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -195233,14 +195297,15 @@
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΒΑΣΙΛΙΚΗΣ ΤΣΩΝΟΥ
 - 0: 15235
   1: ΧΑΤΟΓΛΟΥ,ΦΡΟΣΩ
   2: ΚΑΛΗΜΕΡΑ ΕΙΡΗΝΗ
   4: 808.899ΧΑΤ
+  5: '20414'
   8: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ
   9: ΑΘΗΝΑ
   11: 46Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΒΑΣΙΛΙΚΗΣ ΤΣΩΝΟΥ
@@ -196826,14 +196891,15 @@
   17: ΔΩΡΕΑ ΟΙΚ. ΑΝΤΩΝΙΑΣ ΜΠΟΥΚΑ
   18: '9789600401'
   19: '462'
 - 0: 15349
   1: ΖΑΙΡΗ-ΡΩΣΣΗ,ΡΕΝΑ
   2: ΔΥΟ ΦΙΛΙΑ ΓΙΑ ΤΗΝ ΑΜΕΛΙΑ
   4: 889.21ΖΑΙ
+  5: '22779'
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2016'
   11: 562Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -199275,15 +199341,15 @@
   11: 332Σ
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   18: '960140574'
 - 0: 15527
   1: GRISHAM,JOHN
-  2: ΤΟ ΝΗΣΙΣ ΚΑΜΙΝΟ
+  2: ΤΟ ΝΗΣΙ ΚΑΜΙΝΟ
   4: 810.11GRI
   5: '20382'
   6: ΓΙΩΡΓΟΣ ΜΠΑΡΟΥΞΗΣ
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '2021'
   11: 380Σ
@@ -199632,29 +199698,29 @@
   11: 115Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: '9789601656'
   19: '649'
 - 0: 15554
-  1: ΓΕΩΡΓΙΑΔΗ-ΤΣΟΡΩΝΗ,ΓΙΟΛΑΝΤΑ
+  1: ΤΣΟΡΩΝΗ-ΓΕΩΡΓΙΑΔΗ,ΓΙΟΛΑΝΤΑ
   2: ΕΝΑ ΠΑΡΑΞΕΝΟ ΧΡΙΣΤΟΥΓΕΝΝΙΑΤΙΚΟ ΔΕΝΤΡΟ
-  4: 808.899ΓΕΩ
+  4: 808.899ΤΣΟ
   5: '20663'
   8: ΣΑΒΒΑΛΑΣ
   9: ΑΘΗΝΑ
   10: '2020'
   11: 29Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: '9789604938'
   19: '100'
 - 0: 15555
-  1: ΓΕΩΡΓΙΑΔΗ-ΤΣΟΡΩΝΗ,ΓΙΟΛΑΝΤΑ
+  1: ΤΣΟΡΩΝΗ-ΓΕΩΡΓΙΑΔΗ,ΓΙΟΛΑΝΤΑ
   2: Ο ΜΕΓΑΣ ΜΕΛΟΜΑΚΑΡΩΝ ΠΟΥ ΜΕΛΟΜΑΚΑΡΩΝΕ
   4: 808.899ΓΕΩ
   5: '20664'
   8: ΣΑΒΒΑΛΑΣ
   9: ΑΘΗΝΑ
   10: '2018'
   11: 28Σ
@@ -200551,17 +200617,17 @@
   9: ΑΘΗΝΑ
   10: '1954'
   11: 603Σ
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 15620
-  1: DRIAULT,E.
+  1: ΝΤΡΙΟΤ,Ε.
   2: Ο ΒΑΣΙΛΕΥΣ ΚΩΝΣΤΑΝΤΙΝΟΣ
-  4: 938.687DRI
+  4: 938.687ΝΤΡ
   5: '16049'
   8: ΠΡΩΙΑΣ
   9: ΑΘΗΝΑ
   10: '1930'
   11: 237Σ
   12: ΙΣΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΑ
   13: ΙΣΤΟΡΙΑ-ΒΙΟΓΡΑΦΙΑ
@@ -201944,21 +202010,24 @@
   2: Ο ΙΟΥΔΑΙΟΣ
   3: ΜΙΑ ΑΛΗΘΙΝΗ ΙΣΤΟΡΙΑ
   5: '21077'
   9: ΑΘΗΝΑ
   10: '1971'
   11: '223'
 - 0: 15741
-  1: ΣΤΑΜΑΤΗΣ, ΕΛΕΥΘΕΡΙΟΣ
-  2: ΚΥΡΙΟΙ, ΠΑΤΕ ΓΙΑ ΥΠΝΟ
-  5: '21078'
-  8: ΔΟΥΡΕΙΟΣ ΙΠΠΟΣ
-  9: ΑΘΗΝΑ
-  10: '2007'
-  11: '298'
+  1: ΒΟΥΛΤΣΙΑΔΗ,ΓΕΩΡΓΙΟΥ
+  2: Η ΠΡΟΣΩΤΣΑΝΗ ΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ
+  4: 938.764ΒΟΥ
+  5: '12423'
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1995'
+  11: '437'
+  12: ΠΡΟΣΩΤΣΑΝΗ
+  13: ΙΣΤΟΡΙΑ
+  14: ΠΡΟΣΩΤΣΑΝΗ
   18: '9789608835'
   19: '535'
 - 0: 15742
   1: SOOTHILL,W.E
   2: ΟΙ ΤΡΕΙΣ ΘΡΗΣΚΕΙΕΣ ΤΗΣ ΚΙΝΑΣ
   5: '21079'
   8: Γ.ΠΑΠΑΔΗΜΗΤΡΙΟΥ
@@ -202134,19 +202203,23 @@
   8: ΕΚΔ.ΔΙΕΘ.ΕΠΙΚΑΙΡ.
   9: ΑΘΗΝΑ
   10: '1972'
   11: '120'
 - 0: 15763
   1: ΘΕΟΔΩΡΑΚΟΠΟΥΛΟΥ,Ι.Ν.
   2: ΤΟ ΕΙΚΟΣΙΕΝΑ ΚΑΙ Ο ΣΥΓΧΡΟΝΟΣ ΕΛΛΗΝΙΣΜΟΣ
+  4: 938.5ΘΕΟ
   5: '21098'
   8: ΕΚΔ.ΤΩΝ ΦΙΛΩΝ
   9: ΑΘΗΝΑ
   10: '1972'
   11: '92'
+  12: ΙΣΤΟΡΙΑ-ΕΙΚΟΣΙΕΝΑ
+  13: ΕΙΚΟΣΙΕΝΑ
+  14: ΙΣΤΟΡΙΑ
 - 0: 15764
   1: ΤΟΤΗ,Τ
   2: ΑΝΤΙΘΕΤΑ ΣΤΟ ΡΕΥΜΑ
   4: 230ΤΟΤ
   5: '21099'
   8: ΦΩΣ
   9: ΑΘΗΝΑ
@@ -202171,21 +202244,25 @@
   2: Η ΒΑΣΙΛΙΚΗ ΔΥΝΑΣΤΕΙΑ 1863-1973
   5: '21102'
   8: ΜΕΤΡΟΝ
   9: ΑΘΗΝΑ
   10: '2007'
   11: '143'
 - 0: 15768
-  1: ΤΟΛΙΑΣ,Γ.
+  1: Χ.Σ
   2: ΣΥΛΛΟΓΙΚΟ, Ο ΠΥΡΕΤΟΣ ΤΩΝ ΜΑΡΜΑΡΩΝ
+  4: 930.1Χ.Σ
   5: '21104'
   8: ΤΟ ΒΗΜΑ
   9: ΑΘΗΝΑ
   10: '1996'
   11: '329'
+  12: ΙΣΤΟΡΙΑ-ΠΟΛΙΤΙΣΜΟΣ
+  13: ΠΟΛΙΤΙΣΜΟΣ
+  14: ΙΣΤΟΡΙΑ
   18: '9789604697'
   19: '861'
 - 0: 15769
   1: ΑΡΧΟΝΤΙΔΗΣ,ΑΣΤΕΡΙΟΣ
   2: ΜΕΤΑΞΥ ΒΕΝΕΤΩΝ ΚΑΙ ΤΟΥΡΚΩΝ
   5: '21105'
   8: ΠΑΡΑΤΗΡΗΤΗΣ
@@ -202231,34 +202308,41 @@
   5: '21110'
   9: ΒΕΝΕΤΙΑ
   10: '2001'
   11: '442'
 - 0: 15775
   1: CASSIRER,ERNST
   2: ΔΟΚΙΜΙΟ ΓΙΑ ΤΟΝ ΑΝΘΡΩΠΟ
+  4: 901CAS
   5: '21111'
   8: ΚΑΛΒΟΣ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1972'
   11: '358'
+  12: ΦΙΛΟΣΟΦΙΑ
+  13: ΦΙΛΟΣΟΦΙΑ
+  14: ΦΙΛΟΣΟΦΙΑ
 - 0: 15776
   1: ΠΟΛΑΡ,ΖΕΚΗ
   2: ΑΙΤΙΑ ΚΑΤΑΡΡΕΥΣΕΩΣ ΤΗΣ ΟΘΩΜΑΝΙΚΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
   5: '21112'
   9: ΑΘΗΝΑ
   10: '1965'
   11: '99'
 - 0: 15777
-  1: ΣΤΑΥΡΙΔΟΥ-ΖΑΦΡΑΚΑ ΑΛΚΜΙΝΗ
+  1: ΖΑΦΡΑΚΑ-ΣΤΑΥΡΙΔΟΥ,ΑΛΚΜΗΝΗ
   2: ΙΓ ΠΑΝΕΛΛΗΝΙΟ ΙΣΤΟΡΙΚΟ ΣΥΝΕΔΡΙΟ
-  4: 938.498ΣΤΑ
+  4: 938.498ΖΑΦ
   5: '21113'
   9: ΘΕΣ/ΝΙΚΗ
   10: '1993'
   11: '178'
+  12: ΠΡΑΚΤΙΚΑ
+  13: ΠΡΑΚΤΙΚΑ
+  14: ΠΡΑΚΤΙΚΑ
 - 0: 15778
   1: ΒΑΣΔΡΑΒΕΛΛΗ,ΙΩΑΝ.
   2: Η ΘΕΣΣΑΛΟΝΙΚΗ
   3: ΚΑΤΑ ΤΟΝ ΑΓΩΝΑ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ
   4: 938.498ΒΑΣ
   5: '21114'
   8: ΜΑΚΕΔΟΝΙΚΗ ΒΙΒ/ΚΗ
@@ -202302,18 +202386,21 @@
   9: ΑΘΗΝΑ
   10: '1998'
   11: '157'
 - 0: 15784
   1: Χ.Σ.
   2: ΙΣΤΟΡΙΚΗ ΠΟΡΕΙΑ ΤΗΣ ΘΕΣΣΑΛΟΝΙΚΗΣ
   4: 938.498Χ.Σ
-  5: '1120'
+  5: '21120'
   9: ΑΘΗΝΑ
   10: '1988'
   11: '62'
+  12: ΙΣΤΟΡΙΑ-ΘΕΣΣΑΛΟΝΙΚΗ
+  13: ΘΕΣΣΑΛΟΝΙΚΗ
+  14: ΙΣΤΟΡΙΑ
 - 0: 15785
   1: ΧΑΣΙΩΤΗΣ,Ι.Κ
   2: ΜΑΚΑΡΙΟΣ,ΘΟΔΩΡΟΣ ΚΑΙ ΝΙΚΗΦΟΡΟΣ ΟΙ ΜΕΛΙΣΣΗΝΟΙ(ΜΕΛΙΣΣΟΥΡΓΟΙ)
   5: '21121'
   8: ΕΤΑΙΡΕΙΑ ΜΑΚ.ΣΠΟΥΔΩΝ
   9: ΘΕΣ/ΝΙΚΗ
   10: '1966'
@@ -202422,39 +202509,51 @@
   5: '21134'
   9: ΘΕΣ/ΝΙΚΗ
   10: '1969'
   11: '19'
 - 0: 15799
   1: ΧΡΙΣΤΟΠΟΥΛΟΣ,Κ.Π.
   2: ΤΟ ΕΛΛΗΝΙΚΟΝ ΠΡΟΒΛΗΜΑ
+  4: 938.764ΧΡΙ
   5: '21135'
   9: ΘΕΣ/ΝΙΚΗ
   10: '1945'
   11: '123'
+  12: ΙΣΤΟΡΙΑ-1940
+  13: ΙΣΤΟΡΙΑ
+  14: '1940'
 - 0: 15800
-  1: Π.Ο.Α.Ε.Α
+  1: Χ.Σ
   2: Η ΕΠΟΠΟΙΙΑ ΤΗΣ ΕΘΝΙΚΗΣ ΜΑΣ ΑΝΤΙΣΤΑΣΗΣ (1941-1945)
+  4: 938.764Χ.Σ
   5: '21136'
   11: '133'
+  12: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
+  13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
+  14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
 - 0: 15801
   1: ΠΙΤΣΑΚΗΣ,Κ
   2: Η ΑΥΤΟΚΡΑΤΟΡΙΑ ΣΕ ΚΡΙΣΗ(;)ΤΟ ΒΥΖΑΝΤΙΟ ΤΟΝ 11ο ΑΙΩΝΑ(1025-108
   3: 1)
   5: '21137'
   8: ΔΙΕΘΝΗ ΣΥΜΠΟΣΙΑ 11
   9: ΑΘΗΝΑ
   10: '2003'
   11: '266'
 - 0: 15802
-  1: ΧΡΗΣΤΟΣ,ΚΩΣΤΑΣ
+  1: ΧΡΗΣΤΟΥ,ΚΩΣΤΑΣ
   2: ΖΥΓΟΣ ΛΕΒΙΤΣΙΚΟ ΙΣΤΟΡΙΑ ΚΑΙ ΠΑΡΑΔΟΣΗ
+  4: 938.939ΧΡΗ
   5: '21138'
   9: ΑΘΗΝΑ
   10: '2000'
   11: '317'
+  12: ΙΤΟΡΙΑ
+  13: ΖΥΓΟΣ ΛΕΒΙΝΣΙΚΟ
+  14: ΙΣΤΟΡΙΑ
 - 0: 15803
   1: Χ.Σ.
   2: ΒΙΟΣ ΤΗΣ ΠΑΝΑΓΙΑΣ,ΒΙΟΣ ΤΟΥ ΧΡΙΣΤΟΥ
   4: 230Χ.Σ.
   5: '21139'
   11: '300'
 - 0: 15804
@@ -204705,14 +204804,15 @@
   14: ΠΟΛΙΤΙΚΕΣ ΔΟΛΟΦΟΝΙΕΣ
   17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
   18: '9789606353'
   19: 048
 - 0: 15968
   1: Χ.Σ.
   2: 70 ΕΠΙΣΤΗΜΟΝΕΣ ΠΟΥ ΑΛΛΑΞΑΝ ΤΟΝ ΚΟΣΜΟ
+  4: 920Χ.Σ
   5: '20986'
   8: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ
   9: ΑΘΗΝΑ
   10: '2017'
   11: '127'
   12: ΕΠΙΣΤΗΜΗ
   13: ΕΠΙΣΤΗΜΗ
@@ -204736,28 +204836,30 @@
   17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
   18: '9789606390'
   19: '722'
 - 0: 15970
   1: Χ.Σ.
   2: 1955 ΣΕΠΤΕΜΒΡΙΑΝΑ
   3: ΟΙ ΜΑΥΡΕΣ ΜΕΡΕΣ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ ΤΗΣ ΠΟΛΗΣ
+  4: 938.498Χ.Σ
   5: '20977'
   8: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ
   9: ΑΘΗΝΑ
   10: '2018'
   11: '299'
   12: ΙΣΤΟΡΙΚΟ ΑΡΧΕΙΟ
   13: ΙΣΤΟΡΙΚΟ ΑΡΧΕΙΟ
   14: ΙΣΤΟΡΙΚΟ ΑΡΧΕΙΟ
   17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
   18: '9789605039'
   19: '646'
 - 0: 15971
   1: ΑΝΤΩΝΙΑΔΗΣ,ΑΝΤΩΝΗΣ
   2: ΤΑ 100 ΓΕΓΟΝΟΤΑ ΠΟΥ ΣΗΜΑΔΕΨΑΝ ΤΗΝ ΕΛΛΑΔΑ ΑΠ ΤΟ 1821 ΕΩΣ ΣΗΜΕ
+  4: 938.498ΑΝΤ
   5: '20984'
   8: ΤΟ ΒΗΜΑ ΑΛΤΕΡ ΕΓΚΟ
   9: ΑΘΗΝΑ
   10: '2021'
   11: '263'
   12: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   13: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
@@ -204766,14 +204868,15 @@
   17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
   18: '9789604367'
   19: '450'
 - 0: 15972
   1: Χ.Σ.
   2: 1922 ΠΩΣ ΧΑΣΑΜΕ ΤΗ ΣΜΥΡΝΗ
   3: ΒΑΣΙΣΜΕΝΟ ΣΕ ΑΓΝΩΣΤΑ ΚΑΙ ΑΠΟΚΑΛΥΠΤΙΚΑ ΕΓΓΡΑΦΑ
+  4: 938.498Χ.Σ
   5: '20987'
   8: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ
   9: ΑΘΗΝΑ
   10: '2018'
   11: '267'
   12: ΣΜΥΡΝΗ
   13: ΣΜΥΡΝΗ
@@ -204796,14 +204899,15 @@
   16: ΜΑΛΟΥΧΟΣ,Γ.
   17: ΔΩΡΕΑ ΑΛΤΕΡ ΕΓΚΟ
   18: '9789605039'
   19: '806'
 - 0: 15974
   1: Χ.Σ.
   2: 70 ΦΙΛΟΣΟΦΟΙ ΠΟΥ ΑΛΛΑΞΑΝ ΤΟΝ ΚΟΣΜΟ
+  4: 920Χ.Σ
   5: '20986'
   8: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ
   9: ΑΘΗΝΑ
   10: '2017'
   11: '127'
   12: ΦΙΛΟΣΟΦΟΙ
   13: ΦΙΛΟΣΟΦΟΙ
@@ -204975,29 +205079,29 @@
   10: '1997'
   11: '100'
   12: ΤΡΑΓΟΥΔΙΑ
   13: ΤΡΑΓΟΥΔΙΑ
   14: ΤΡΑΓΟΥΔΙΑ
 - 0: 15987
   1: ΤΣΟΥΤΣΙΝΟΣ,ΓΙΑΝΝΗΣ
-  2: ΑΡΤΙΝΑ ΙΣΤΟΡΙΜΑΤΑ
+  2: ΑΡΤΙΝΑ ΙΣΤΟΡΗΜΑΤΑ
   4: 938.939ΤΣΟ
   5: '21196'
   8: ΠΕΡΙΟΔΙΚΟ ΣΚΟΥΦΑΣ
   9: ΑΡΤΑ
   10: '1975'
   11: '36'
   12: ΑΡΤΑ
   13: ΑΡΤΑ
   14: ΑΡΤΑ
 - 0: 15988
   1: NICOL,DONALD
   2: ΗΠΕΙΡΩΤΙΚΑ ΧΡΟΝΙΚΑ
   3: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
-  4: 938.939DON
+  4: 938.384NIC
   5: '21197'
   8: ΑΠΕΙΡΩΤΑΝ
   9: ΙΩΑΝΝΙΝΑ
   10: '1992'
   11: '59'
   12: ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ
@@ -205011,17 +205115,17 @@
   9: ΑΘΗΝΑ
   10: '1978'
   11: '93'
   12: ΑΡΤΑ
   13: ΑΡΤΑ
   14: ΑΡΤΑ
 - 0: 15990
-  1: NICOL, M. DONALD
+  1: NICOL,DONALD
   2: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ 1267-1479
-  4: 938.939DON
+  4: 938.375NIC
   5: '21199'
   8: ΕΛ.ΕΥΡΩΕΚΔΟΤΙΚΗ ΕΠΕ
   9: ΑΘΗΝΑ
   10: '1991'
   11: '327'
   12: ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ
@@ -205333,35 +205437,36 @@
 - 0: 16014
   1: Χ.Σ.
   2: ΜΝΗΜΗ ΣΟΥΛΙΟΥ
   4: 938.526Χ.Σ
   5: '21252'
   8: ΟΙ ΦΙΛΟΙ ΤΟΥ ΣΟΥΛΙΟΥ
   9: ΑΘΗΝΑ
-  10: '2007'
+  10: '2016'
   11: '343'
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
-  17: ΤΟΜΟΣ ΠΡΩΤΟΣ
+  17: ΤΟΜΟΙ 4
   22: ΣΟΥΛΙ
   23: ΣΟΥΛΙ
   24: ΣΟΥΛΙ
 - 0: 16015
   1: Χ.Σ.
-  2: ΜΝΗΜΗ ΣΟΥΛΙΟΥ ΔΕΥΤΕΡΟΣ ΤΟΜΟΣ
+  2: ΜΝΗΜΗ ΣΟΥΛΙΟΥ
   4: 938.526Χ.Σ
   5: '21253'
   8: ΟΙ ΦΙΛΟΙ ΤΟΥ ΣΟΥΛΙΟΥ
   9: ΑΘΗΝΑ
   10: '1973'
   11: '365'
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
+  17: ΤΟΜΟΙ 2
   22: ΣΟΥΛΙ
   23: ΣΟΥΛΙ
   24: ΣΟΥΛΙ
 - 0: 16016
   1: HELLER,ROBERT
   2: ΣΥΜΒΟΥΛΟΣ ΜΑΝΑΤΖΕΡ
   3: ΠΩΣ ΝΑ ΞΕΧΩΡΙΣΕΤΕ
@@ -205377,15 +205482,15 @@
   14: ΑΥΤΟΒΕΛΤΙΩΣΗ
   17: 6 ΤΟΜΟΙ ΤΗΣ ΙΔΙΑΣ ΣΕΙΡΑΣ
   18: '9603936774'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16017
   1: HELLER,ROBERT
   2: ΣΥΜΒΟΥΛΟΣ ΜΑΝΑΤΖΕΡ
-  3: ΕΠΙΚΟΙΝΩΝΙΣΤΕ ΑΠΟΤΕΛΕΣΜΑΤΙΚΑ
+  3: ΕΠΙΚΟΙΝΩΝΗΣΤΕ ΑΠΟΤΕΛΕΣΜΑΤΙΚΑ
   4: 658.4HEL
   5: '21295'
   6: ΠΕΡΑΝΤΑΚΟΥ,ΜΑΙΡΗ
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '2001'
   11: '72'
@@ -205476,60 +205581,60 @@
   13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
   18: '9789604751'
   19: '754'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16023
   1: Χ.Σ.
-  2: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   3: ΑΛΕΞΑΝΔΡΕΙΑ
   4: 909.048Χ.Σ
   5: '21232'
   8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
   11: '128'
   12: ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
   18: '9789604751'
   19: '761'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16024
   1: Χ.Σ.
-  2: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   3: ΟΔΗΣΣΟΣ
   4: 909.048Χ.Σ
   5: '21233'
   8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
   11: '96'
   12: ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
   18: '9789604751'
   19: '778'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16025
   1: Χ.Σ.
-  2: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   3: ΣΜΥΡΝΗ
   4: 909.048Χ.Σ
   5: '21234'
   8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
   11: '101'
   12: ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
   18: '9789604751'
   19: '785'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16026
   1: Χ.Σ.
-  2: ΚΟΙΤΗΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   3: ΜΙΛΗΤΟΣ
   4: 909.048Χ.Σ
   5: '21235'
   8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
   11: '96'
   12: ΕΛΛΗΝΙΣΜΟΣ
@@ -205566,15 +205671,15 @@
   13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
   18: '9789604751'
   19: '815'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16029
   1: Χ.Σ.
-  2: ΚΟΙΤΙΔΕΣ ΠΟΛΙΤΙΣΜΟΥ
+  2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   3: ΠΕΡΓΑΜΟΣ
   4: 909.048Χ.Σ
   5: '21238'
   8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
   11: '88'
   12: ΕΛΛΗΝΙΣΜΟΣ
@@ -205589,15 +205694,15 @@
   3: ΒΕΝΕΤΙΑ
   4: 909.048Χ.Σ
   5: '21239'
   8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
   11: '102'
   12: ΕΛΛΗΝΙΣΜΟΣ
-  13: ΕΛΛΗΝΙΣΜΟ
+  13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
   18: '9789604751'
   19: '839'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16031
   1: Χ.Σ.
   2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
@@ -205657,15 +205762,15 @@
   14: ΕΛΛΗΝΙΣΜΟΣ
   18: '9789604751'
   19: '853'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16035
   1: Χ.Σ.
   2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
-  3: ΑΛΛΟΧΩΣΤΟΣ
+  3: ΑΜΜΟΧΩΣΤΟΣ
   4: 909.048Χ.Σ
   5: '21244'
   8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
   11: '96'
   12: ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ
@@ -205716,15 +205821,15 @@
   13: ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ
   18: '9789604751'
   19: '945'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16039
   1: Χ.Σ.
-  2: ΚΟΙΤΟΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
+  2: ΚΟΙΤΙΔΕΣ ΕΛΛΗΝΙΣΜΟΥ
   3: ΚΑΜΠΑΝΙΑ ΚΑΙ ΑΠΟΥΛΙΑ
   4: 909.048Χ.Σ
   5: '21248'
   8: ΚΑΘΗΜΕΡΙΝΗ
   9: ΑΘΗΝΑ
   11: '88'
   12: ΕΛΛΗΝΙΣΜΟΣ
@@ -206254,15 +206359,15 @@
   13: ΤΑΞΙΔΙΩΤΙΚΟΙ ΟΔΗΓΟΙ
   14: ΤΑΞΙΔΙΩΤΙΚΟΙ ΟΔΗΓΟΙ
   18: '9603682195'
   30: ΔΩΡΕΑ Ι.ΠΝΕΥΜΑΤΙΚΟΥ
 - 0: 16075
   1: Χ.Σ.
   2: ΟΔΗΓΟΙ ΤΟΥ ΚΟΣΜΟΥ
-  3: ΑΙΓΗΠΤΟΣ
+  3: ΑΙΓΥΠΤΟΣ
   4: 910.202Χ.Σ
   5: '21286'
   8: GALLIMARD
   9: ΑΘΗΝΑ
   10: '2000'
   11: '479'
   12: ΤΑΞΙΔΙΩΤΙΚΟΙ ΟΔΗΓΟΙ
@@ -209003,23 +209108,23 @@
   8: ΠΑΠΑΔΟΠΟΥΛΟΣ
   11: '85'
   12: Ο ΠΛΑΤΕΡΟ ΚΙ ΕΓΩ
   13: Ο ΠΛΑΤΕΡΟ ΚΙ ΕΓΩ
   14: Ο ΠΛΑΤΕΡΟ ΚΙ ΕΓΩ
   17: ΔΩΡΕΑ ΜΑΡΙΑΣ ΚΟΛΙΟΥ
 - 0: 16276
-  1: MARK TWAIN
+  1: TWAIN,MARK
   2: ΤΟΜ ΣΟΓΕΡ
   4: 808.899TWA
   5: '21741'
   8: ΠΑΠΑΔΟΠΟΥΛΟΣ
   11: '156'
-  12: ΤΟΜ ΣΟΓΕΡ
-  13: ΤΟΜ ΣΟΓΕΡ
-  14: ΤΟΜ ΣΟΓΕΡ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΜΑΡΙΑΣ ΚΟΛΙΟΥ
 - 0: 16277
   1: RUDYARD KIPLING
   2: ΜΟΓΛΗΣ
   4: 808.899KIP
   5: '21739'
   8: ΠΑΠΑΔΟΠΟΥΛΟΣ
@@ -219441,15 +219546,15 @@
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2022'
   11: 438Σ
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
-  17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΑΣ
+  17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
   18: '9786180143'
   19: '003'
 - 0: 17124
   1: ΛΑΓΚΕΡΚΡΑΝΤΖ,ΝΤΑΒΙΝΤ
   2: ΤΟ ΚΟΡΙΤΣΙ ΣΤΟΝ ΙΣΤΟ ΤΗΣ ΑΡΑΧΝΗΣ
   6: ΞΕΝΟΦΩΝ ΠΑΓΚΑΛΙΑΣ
   8: ΨΥΧΟΓΙΟΣ
@@ -219531,14 +219636,15 @@
   19: '922'
   30: ΤΟΜΟΣ 6
 - 0: 17129
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   3: ΤΟ ΠΟΤΗΡΙ ΞΕΧΕΙΛΙΣΕ
   4: 808.899ΚΙΝ
+  5: '22580'
   6: ΧΑΡΑ ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2021'
   11: 225Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219548,14 +219654,15 @@
   19: '665'
   30: ΤΟΜΟΣ 3
 - 0: 17130
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   3: Ο ΡΟΝΤΡΙΚ ΔΕΝ ΠΑΙΖΕΤΑΙ
   4: 808.899ΚΙΝ
+  5: '22579'
   6: ΧΑΡΑ ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2022'
   11: 225Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219565,14 +219672,15 @@
   19: '248'
   30: ΤΟΜΟΣ 2
 - 0: 17131
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   3: ΣΚΥΛΙΣΙΑ ΖΩΗ
   4: 808.899ΚΙΝ
+  5: '22581'
   6: ΧΑΡΑ ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2022'
   11: 224Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219582,14 +219690,15 @@
   19: '716'
   30: ΤΟΜΟΣ 4
 - 0: 17132
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   3: ΘΑ ΠΑΕΙ ΜΑΚΡΙΑ Η ΒΑΛΙΤΣΑ
   4: 808.899ΚΙΝ
+  5: '22584'
   6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2021'
   11: 225Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219599,14 +219708,15 @@
   19: '262'
   30: ΤΟΜΟΣ 9
 - 0: 17133
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   3: Η ΑΠΟΔΡΑΣΗ
   4: 808.899ΚΙΝ
+  5: '22585'
   6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2022'
   11: 225Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219616,14 +219726,15 @@
   19: '381'
   30: ΤΟΜΟΣ 12
 - 0: 17134
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   3: Η ΣΚΛΗΡΗ ΑΛΗΘΕΙΑ
   4: 808.899ΚΙΝ
+  5: '22582'
   6: ΧΑΡΑ ΓΙΑΝΝΑΚΟΠΟΥΛΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2022'
   11: 225Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219633,47 +219744,51 @@
   19: '071'
   30: ΤΟΜΟΣ 5
 - 0: 17135
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΣΠΑΣΙΚΛΑ
   3: ΣΤΟΥΣ ΔΥΟ ΤΡΙΤΟΣ ΔΕ ΧΩΡΕΙ
   4: 808.899ΚΙΝ
+  5: '22583'
   6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2022'
   11: 226Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
   18: '9786180100'
   19: '136'
   30: ΤΟΜΟΣ 7
 - 0: 17136
-  1: ΛΑΖΑΡ,ΡΑΛΦ-ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ
+  1: ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ-ΛΑΖΑΡ,ΡΑΛΦ
   2: Ο ΝΤΕΤΕΚΤΙΒ ΡΟΝΙ
   3: ΒΑΖΕΙ ΤΑ ΓΕΛΙΑ ΜΠΡΟΣΤΑ ΣΤΟΝ ΚΙΝΔΥΝΟ
-  4: 808.899ΛΑΖ
+  4: 808.899ΚΛΟ
+  5: '22604'
   6: ΕΥΓΕΝΙΑ ΚΟΛΥΔΑ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2019'
   11: 350Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
   18: '9786180129'
   19: '342'
   30: ΤΟΜΟΣ 2
 - 0: 17137
-  1: ΛΑΖΑΡ,ΡΑΛΦ-ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ
+  1: ΚΛΟΟΥΒΕΡ,ΑΝΤΡΙΟΥ-ΛΑΖΑΡ,ΡΑΛΦ
   2: Ο ΝΤΕΤΕΚΤΙΒ ΡΟΝΙ
   3: ΠΑΤΑΕΙ ΣΤΟ ΚΕΦΑΛΙ ΤΟΥΣ ΚΑΚΟΥΣ
+  4: 808.899ΚΛΟ
+  5: '22605'
   6: ΕΥΓΕΝΙΑ ΚΟΛΥΔΑ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2020'
   11: 282Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219732,14 +219847,15 @@
   18: '9786180138'
   19: '696'
   30: ΤΟΜΟΣ 3
 - 0: 17141
   1: ΜΟΥΡΙΚΗ,ΚΑΤΕΡΙΝΑ
   2: ΠΑΥΛΟΣ Ο ΑΠΟΣΤΟΛΟΣ ΤΩΝ ΕΘΝΩΝ
   4: 808.899ΜΟΥ
+  5: '22594'
   8: ΟΥΡΑΝΟΣ
   9: ΑΘΗΝΑ
   10: '2020'
   11: 50Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219774,28 +219890,30 @@
   17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
   18: '9789607021'
   19: '854'
 - 0: 17144
   1: ΓΕΩΡΓΟΣΤΑΘΗ,ΕΛΕΝΗ
   2: ΧΑΘΗΚΕ Η ΜΠΑΛΑ
   4: 808.899ΓΕΩ
+  5: '22597'
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2017'
   11: 93Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
   18: '9786180118'
   19: '75'
 - 0: 17145
   1: ΔΗΜΟΠΟΥΛΟΣ,ΧΡΗΣΤΟΣ
   2: ΤΟ ΠΡΩΤΟ ΣΥΝΤΑΓΜΑ ΤΗΣ ΕΛΛΑΔΑΣ ΓΙΑ ΠΑΙΔΙΑ
   4: 808.899ΔΗΜ
+  5: '22593'
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2020'
   11: 39Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219817,29 +219935,31 @@
   17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
   18: '9786180141'
   19: '986'
 - 0: 17147
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΤΟ ΗΜΕΡΟΛΟΓΙΟ ΕΝΟΣ ΑΠΙΣΤΕΥΤΑ ΚΑΛΟΥ ΠΑΙΔΙΟΥ
   4: 808.899ΚΙΝ
+  5: '22599'
   6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2019'
   11: 226Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
   18: '9786180131'
   19: 093
 - 0: 17148
   1: ΚΙΝΙ,ΤΖΕΦ
   2: ΟΙ ΑΠΙΣΤΕΥΤΑ ΚΑΛΕΣ ΙΣΤΟΡΙΕΣ ΤΡΟΜΟΥ
-  4: 808.899ΝΙΚ
+  4: 808.899ΚΙΝ
+  5: '22600'
   6: ΠΕΤΡΟΥΛΑ ΓΑΒΡΙΗΛΙΔΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2021'
   11: 226Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219893,16 +220013,17 @@
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΕΚΔΟΣΕΙΣ ΨΥΧΟΓΙΟΣ
   18: '9786180124'
   19: 095
   30: ΤΟΜΟΣ 5
 - 0: 17152
   1: ΠΙΛΚΙ,ΝΤΕΙΒ
-  2: Ο ΚΑΠΕΤΑ ΒΡΑΚΑΣ ΚΑΙ Η ΜΕΓΑΛΗ ΜΑΝΙΑΣΜΕΝΗ ΜΑΧΗ
+  2: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΜΕΓΑΛΗ ΜΑΝΙΑΣΜΕΝΗ ΜΑΧΗ
   4: 808.899ΠΙΛ
+  5: '22611'
   6: ΣΟΦΙΑ ΓΡΗΓΟΡΙΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2021'
   11: 177Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219911,14 +220032,15 @@
   18: '9786180124'
   19: '35'
   30: ΤΟΜΟΣ 6
 - 0: 17153
   1: ΠΙΛΚΙ,ΝΤΕΙΒ
   2: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΠΡΟΣΜΕΝΗ ΕΠΙΣΤΡΟΦΗ
   4: 808.899ΠΙΛ
+  5: '22612'
   6: ΣΟΦΙΑ ΓΡΗΓΟΡΙΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2019'
   11: 298Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219927,14 +220049,15 @@
   18: '9786180130'
   19: '22'
   30: ΤΟΜΟΣ 9
 - 0: 17154
   1: ΠΙΛΚΙ,ΝΤΕΙΒ
   2: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΝΕΚΔΙΗΓΗΤΗ ΕΚΔΙΚΗΣΗ
   4: 808.899ΠΙΛ
+  5: '22613'
   6: ΣΟΦΙΑ ΓΡΗΓΟΡΙΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2020'
   11: 224Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -219943,14 +220066,15 @@
   18: '9786180134'
   19: '551'
   30: ΤΟΜΟΣ 10
 - 0: 17155
   1: ΠΙΛΚΙ,ΝΤΕΙΒ
   2: Ο ΚΑΠΕΤΑΝ ΒΡΑΚΑΣ ΚΑΙ Η ΑΒΑΣΤΑΧΤΗ ΒΑΡΒΑΡΟΤΗΤΑ
   4: 808.899ΠΙΛ
+  5: '22610'
   6: ΜΑΙΡΗ ΓΡΑΜΜΕΝΟΥ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2022'
   11: 170Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -221229,24 +221353,30 @@
   2: ΣΠΑΣΤΕ ΤΑ ΔΕΣΜΑ ΤΗΣ ΧΑΜΗΛΗΣ ΑΥΤΟΕΚΤΙΜΗΣΗΣ
   4: 306.7SOR
   5: '22522'
   8: ΦΥΤΡΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '1998'
   11: '418'
+  12: ΑΥΤΟΕΚΤΙΜΗΣΗ
+  13: ΑΥΤΟΕΚΤΙΜΗΣΗ
+  14: ΑΥΤΟΕΚΤΙΜΗΣΗ
   18: '9605354896'
 - 0: 17256
   1: ΠΑΠΑΔΑΤΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   2: ΤΑ ΠΡΩΤΑ 6 ΧΡΟΝΙΑ ΤΗΣ ΖΩΗΣ ΤΟΥ ΠΑΙΔΙΟΥ
   4: 305.231ΠΑΠ
   5: '22548'
   8: NESTLE
   9: ΑΘΗΝΑ
   10: '1996'
   11: '76'
+  12: ΠΡΟΣΧΟΛΙΚΗ ΗΛΙΚΙΑ
+  13: ΠΡΟΣΧΟΛΙΚΗ ΗΛΙΚΙΑ
+  14: ΠΡΟΣΧΟΛΙΚΗ ΗΛΙΚΙΑ
 - 0: 17257
   1: RANG-DALE
   2: ΦΑΡΜΑΚΟΛΟΓΙΑ
   4: 615.1RAN
   5: '22633'
   6: ΑΙΚΑΤΕΡΙΝΗ ΑΛΕΞΙΟΥ
   8: ΠΑΡΙΣΙΑΝΟΥ
@@ -221631,15 +221761,15 @@
   6: ΠΑΓΚΑΛΙΑΣ ΞΕΝ.
   8: ΚΕΔΡΟΣ
   9: ΑΘΗΝΑ
   10: '2021'
   11: '436'
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
-  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ ΜΥΘΙΣΤΟΡΙΜΑ
+  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   18: '9789600451'
   19: '825'
 - 0: 17285
   1: CONNELLY,MICHAEL
   2: ΟΙ ΔΥΟ ΟΨΕΙΣ ΤΗΣ ΑΛΗΘΕΙΑΣ
   4: 810.11CON
@@ -221677,17 +221807,17 @@
   5: '22684'
   6: ΚΑΝΕΛΟΠΟΥΛΟΥ ΔΕΣ.
   7: 1Η
   8: ΚΑΣΤΑΝΙΟΤΗΣ NOIR
   9: ΑΘΗΝΑ
   10: '2020'
   11: '564'
-  12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
-  13: ΞΕΝΗ ΛΟΗΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
-  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
+  12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+  13: ΞΕΝΗ ΛΟΗΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   18: '9789600367'
   19: '546'
 - 0: 17288
   1: ΑΝΑΣΤΑΣΕΑ,ΝΙΚΗ
   2: ΠΟΛΥ ΧΙΟΝΙ ΜΠΡΟΣΤΑ ΣΤΟ ΣΠΙΤΙ
   4: 889.21ΑΝΑ
@@ -221708,17 +221838,17 @@
   4: 850.11ΜΑΣ
   5: '22682'
   6: ΟΙΚΟΝΟΜΙΔΟΥ ΜΑΡΙΑ
   8: ΠΑΤΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '2021'
   11: '652'
-  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
-  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
-  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΙΜΑ
+  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
+  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   18: '9789601692'
   19: '715'
 - 0: 17290
   1: ΣΕΡΕΦΑΣ,ΣΑΚΗΣ
   2: ΠΩΛΟΥΝΤΑΙ ΣΚΙΕΣ
   4: 808.899ΣΕΡ
@@ -221823,17 +221953,18 @@
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
   18: '9789605071'
   19: '387'
 - 0: 17297
-  1: ΜΕΓΕΡ,ΜΑΡΙΣΣΑ
+  1: MEYER,MARISSA
   2: ΣΙΝΤΕΡ
   3: Η ΤΕΤΡΑΛΟΓΙΑ ΤΗΣ ΣΕΛΗΝΗΣ
+  4: 823MEY
   5: '22678'
   6: ΚΑΛΟΦΟΛΙΑΣ
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2012'
   11: '486'
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
@@ -221848,17 +221979,17 @@
   4: 843ΣΙΝ
   5: '22677'
   6: ΚΟΚΚΙΝΟΥ ΒΑΣΙΛΙΚΗ
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2005'
   11: '390'
-  12: ΜΥΘΙΣΤΟΡΙΜΑ
-  13: ΜΥΘΙΣΤΟΡΙΜΑ
-  14: ΜΥΘΙΣΤΟΡΙΜΑ
+  12: ΜΥΘΙΣΤΟΡΗΜΑ
+  13: ΜΥΘΙΣΤΟΡΗΜΑ
+  14: ΜΥΘΙΣΤΟΡΗΜΑ
   17: ΔΩΡΕΑ ΙΩΑΝΝΑ ΠΕΤΡΙΔΟΥ
 - 0: 17299
   1: ΚΡΗΤΙΚΟΣ,ΜΑΡΚΟΣ
   2: ΤΟ ΜΠΛΟΥΖ ΤΗΣ ΠΕΤΑΛΟΥΔΑΣ
   4: 889.21ΚΡΗ
   5: '22676'
   8: ΜΕΤΑΙΧΜΙΟ
@@ -222146,7 +222277,2809 @@
   11: '197'
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΒΑΣΙΛΗ ΚΟΝΤΑΞΗ
   18: '9789600446'
   19: '432'
+- 0: 17319
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  2: ΜΙΑ ΠΛΩΤΗ ΠΟΛΙΤΕΙΑ
+  3: ΝΑΥΤΙΚΟΣ ΑΠΟΚΛΕΙΣΜΟΣ
+  4: 808.899ΒΕΡ
+  5: '22777'
+  6: Κ.ΜΠΟΥΛΟΥΚΟΥ
+  8: ΤΕΣΣΕΡΑ ΠΙ
+  9: ΑΘΗΝΑ
+  10: '2011'
+  11: '254'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789604883'
+  19: '264'
+- 0: 17320
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  2: ΡΟΒΗΡΟΣ Ο ΚΑΤΑΚΤΗΤΗΣ
+  4: 808.899ΒΕΡ
+  5: '20776'
+  6: Χ.ΤΡΑΙΤΟΡΑΚΗ
+  8: ΤΕΣΣΕΡΑ ΠΙ
+  9: ΑΘΗΝΑ
+  10: '2011'
+  11: '230'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789604883'
+  19: 097
+- 0: 17321
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  2: ΒΟΡΡΑΣ ΕΝΑΝΤΙΟΝ ΝΟΤΟΥ
+  4: 808.899ΒΕΡ
+  5: '22775'
+  6: Μ.ΜΑΥΡΟΜΑΤΑΚΗ
+  8: ΤΕΣΣΕΡΑ ΠΙ
+  9: ΑΘΗΝΑ
+  10: '2011'
+  11: '393'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789604883'
+  19: '509'
+- 0: 17322
+  1: SMITH,WILBOUR
+  2: ΚΥΝΗΓΟΙ ΔΙΑΜΑΝΤΩΝ
+  4: 823SMI
+  5: '22766'
+  6: ΑΛΕΚΟΣ ΜΑΝΩΛΙΔΗΣ
+  8: BELL
+  9: ΑΘΗΝΑ
+  10: '2021'
+  11: '317'
+  12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789604502'
+  19: '752'
+- 0: 17323
+  1: ΚΑΡΑΦΥΛΛΗ,ΙΡΕΝΑ
+  2: Η ΑΣΥΜΒΙΒΑΣΤΗ ΜΟΥΣΑ
+  4: 889.21ΚΑΡ
+  5: '22768'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2008'
+  11: '540'
+  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789604534'
+  19: '289'
+- 0: 17324
+  1: ΑΚΡΙΤΑ,ΕΛΕΝΑ
+  2: ΧΤΥΠΟΚΑΡΔΙΑ ΣΤΟ ΚΡΑΝΙΟ
+  4: 889.21ΑΚΡ
+  5: '22768'
+  8: ΚΑΣΤΑΝΙΩΤΗΣ
+  9: ΑΘΗΝΑ
+  10: '2011'
+  11: 181Σ
+  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789600353'
+  19: '723'
+- 0: 17325
+  1: ΚΑΡΙΖΩΝΗ,ΚΑΤΕΡΙΝΑ
+  2: ΜΕΓΑΛΟ ΑΛΓΕΡΙ
+  4: 889.21ΚΑΡ2
+  5: '2770'
+  8: ΚΑΣΤΑΝΙΩΤΗΣ
+  9: ΑΘΗΝΑ
+  10: '2006'
+  11: '272'
+  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9600342547'
+- 0: 17326
+  1: KOONTZ,DEAN
+  2: ΟΣΑ ΞΕΡΕΙ Η ΝΥΧΤΑ
+  4: 823ΚΟΟ
+  5: '22769'
+  6: ΠΑΛΜΥΡΑ ΙΣΜΥΡΙΔΟΥ
+  8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
+  9: ΑΘΗΝΑ
+  10: '2010'
+  11: 426Σ
+  12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789606354'
+  19: '304'
+- 0: 17327
+  1: ΘΕΟΤΟΚΑΣ,ΓΙΩΡΓΟΣ
+  2: ΑΡΓΩ
+  3: ΙΣΤΟΡΙΑ ΣΤΗ ΛΟΓΟΤΕΧΝΙΑ
+  4: 889.21ΘΕΟ
+  5: '22771'
+  8: ΤΟ ΒΗΜΑ
+  9: ΑΘΗΝΑ
+  10: '2015'
+  11: '378'
+  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789605036'
+  19: '010'
+- 0: 17328
+  1: BARKS,CARL
+  2: ΤΟ ΔΑΧΤΥΛΙΔΙ ΤΗΣ ΜΟΥΜΙΑΣ
+  4: 808.899BAR
+  5: '22774'
+  8: ΚΑΘΗΜΕΡΙΝΗ
+  9: ΑΘΗΝΑ
+  10: '2016'
+  11: '191'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789605850'
+  19: '425'
+- 0: 17329
+  1: STRANDBERG,MATS
+  2: Η ΚΡΟΥΑΖΙΕΡΑ ΤΟΥ ΤΡΟΜΟΥ
+  4: 839.72STR
+  5: '22773'
+  6: ΓΙΩΡΓΟΣ ΜΑΘΟΠΟΥΛΟΣ
+  8: ΚΕΔΡΟΣ
+  9: ΑΘΗΝΑ
+  10: '2019'
+  11: '576'
+  12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789600449'
+  19: '570'
+- 0: 17330
+  1: MASTERTON,GRAHAM
+  2: ΠΛΗΓΩΜΕΝΟΙ ΑΓΓΕΛΟΙ
+  4: 823MAS
+  5: '22772'
+  6: ΜΑΡΙΑ ΜΟΥΝΤΟΚΑΛΑΚΗ
+  8: ΟΞΥ
+  9: ΑΘΗΝΑ
+  10: '2017'
+  11: '432'
+  12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
+  18: '9789604363'
+  19: '544'
+- 0: 17331
+  1: ΒΡΑΚΑΣ,ΦΩΤΗΣ
+  2: ΦΙΛΙΠΠΙΑΔΑ Ο ΧΩΡΟΣ Ο ΟΙΚΙΣΜΟΣ Ο ΚΑΖΑΣ
+  4: 938.937ΒΡΑ
+  5: '22781'
+  8: 24 ΓΡΑΜΜΑΤΑ
+  9: ΑΘΗΝΑ
+  10: '2022'
+  11: 359Σ
+  12: ΙΣΤΟΡΙΑ-ΦΙΛΙΠΠΙΑΔΑ
+  13: ΟΙΚΙΣΜΟΣ
+  14: ΦΙΛΙΠΠΙΑΔΑ
+  15: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΦΩΤΗ ΒΡΑΚΑ
+  18: '9786182015'
+  19: '032'
+- 0: 17332
+  1: ΣΤΑΥΡΟΣ,ΧΡΗΣΤΟΣ
+  2: ΡΟΔΑΥΓΗ ΕΝΑ ΤΑΞΙΔΙ ΣΤΟ ΧΤΕΣ
+  4: 938.939ΣΤΑ
+  5: '22780'
+  8: ΕΝΤΥΠΩΣΙΣ
+  9: ΑΡΤΑ
+  10: '2020'
+  11: '199'
+  12: ΙΣΤΟΡΙΑ-ΡΟΔΑΥΓΗ
+  13: ΦΩΤΟΓΡΑΦΙΚΟ ΛΕΥΚΩΜΑ
+  14: ΡΟΔΑΥΓΗ
+  15: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΧΡΗΣΤΟΣ ΣΤΑΥΡΟΣ
+  18: '9786180021'
+  19: 097
+- 0: 17333
+  1: ΓΟΥΒΕΛΗ,ΓΙΩΤΑ
+  2: ΤΟ ΔΑΚΡΥ ΤΗΣ ΜΑΝΤΙΣΣΑΣ
+  4: 889.21ΓΟΥ
+  5: '22778'
+  8: ΔΙΟΠΤΡΑ
+  9: ΑΘΗΝΑ
+  10: '2022'
+  11: '501'
+  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789606539'
+  19: '152'
+- 0: 17334
+  1: ΣΚΛΑΒΕΝΙΤΗΣ,ΔΗΜΗΤΡΗΣ
+  2: 1922 ΜΕ ΞΙΦΟΛΟΓΧΗ ΚΑΙ ΓΡΑΦΙΔΑ ΣΤΟ ΜΙΚΡΑΣΙΑΤΙΚΟ ΜΕΤΩΠΟ
+  5: '22782'
+  8: ΜΟΡΦΩΤ.ΙΔΡΥΜΑ ΕΣΗΕΑ
+  9: ΑΘΗΝΑ
+  10: '2022'
+  11: '301'
+  12: ΑΡΧΕΙΑΚΕΣ ΣΥΛΛΟΓΕΣ
+  13: ΜΙΚΡΑΣΙΑΤΙΚΟ ΜΕΤΩΠΟ
+  14: ΕΦΗΜΕΡΙΔΕΣ ΕΛΛΗΝΩΝ ΣΤΡΑΤΙΩΤΩΝ
+  18: '9789960888'
+  19: '9545'
+- 0: 17335
+  1: ΚΟΜΖΙΑΣ,ΓΕΩΡΓΙΟΣ
+  2: ΤΟ ΑΡΤΙΝΟ ΛΑΙΚΟ ΧΟΡΟΣΤΑΣΙ
+  4: 938.939ΚΟΜ
+  5: '22783'
+  8: SOUL TWINKLES
+  9: ΑΘΗΝΑ
+  10: '2021'
+  11: '406'
+  12: ΙΣΤΟΡΙΑ-ΑΡΤΑ
+  13: ΧΟΡΟΣΤΑΣΙ
+  14: ΑΡΤΑ
+  15: ΛΑΟΓΡΑΦΙΑ
+  18: '9786188389'
+  19: '731'
+- 0: 17336
+  1: ΓΑΙΤΑΝΙΔΗΣ,ΠΑΥΛΟΣ
+  2: ΜΟΥΣΙΚΗ ΤΩΝ ΕΛΛΗΝΩΝ ΤΟΥ ΠΟΝΤΟΥ
+  4: 781.62ΓΑΙ
+  5: '22786'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2022'
+  11: '150'
+  12: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+  13: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+  14: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606022'
+  19: '586'
+- 0: 17337
+  1: ΓΑΙΤΑΝΙΔΗΣ,ΠΑΥΛΟΣ
+  2: Η ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ ΩΣ ΕΠΕΚΤΑΣΗ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΜΟΥΣΙΚΗΣ
+  4: 781.62ΓΑΙ
+  5: '22787'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2022'
+  11: '268'
+  12: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+  13: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+  14: ΠΟΝΤΙΑΚΗ ΜΟΥΣΙΚΗ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606023'
+  19: '361'
+- 0: 17338
+  1: ΤΣΙΝΑΛΗΣ,ΚΟΣΜΑΣ
+  2: ΕΝΑΝ ΖΑΝΤΟΝ ΑΡΚΟΥΔΟΠΟΝ
+  4: 889.3ΤΣΙ
+  5: '22790'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2022'
+  11: '70'
+  12: ΠΟΝΤΙΑΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
+  13: ΠΟΝΤΙΑΚΟ ΠΑΡΑΜΥΘΙ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606023'
+  19: '613'
+- 0: 17339
+  1: ΝΤΕ ΣΑΙΝΤ-ΕΞΥΠΕΡΥ,ΑΝΤΟΥΑΝ
+  2: Ο ΜΙΚΡΟΣ Ο ΠΡΙΓΚΙΠΑΣ
+  4: 889.3ΝΤΕ
+  5: '22798'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2022'
+  11: '150'
+  12: ΠΟΝΤΙΑΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
+  13: ΠΟΝΤΙΑΚΟ ΠΑΡΑΜΥΘΙ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606022'
+  19: '678'
+- 0: 17340
+  1: ΜΑΥΡΙΔΟΥ,ΜΑΡΙΑ
+  2: ΤΗ ΦΤΕΧΟΥ ΤΟ ΚΑΜΙΣ ΚΑΙ ΤΟ ΞΕΦΤΙΛΕΡ
+  4: 887ΜΑΥ
+  5: '22799'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2021'
+  11: '144'
+  12: ΠΟΝΤΙΑΚΟ ΘΕΑΤΡΟ
+  13: ΘΕΑΤΡΙΚΟ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606023'
+  19: '057'
+- 0: 17341
+  1: ΦΥΛΑΧΤΟΣ,ΧΡΗΣΤΟΣ
+  2: ΑΠ ΤΟ ΧΟΛΟΜΩΝΤΑ ΣΤΟ ΣΑΓΓΑΡΙΟ
+  4: 887ΦΥΛ
+  5: '22785'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2017'
+  11: '111'
+  12: ΠΟΝΤΙΑΚΟ ΘΕΑΤΡΟ
+  13: ΘΕΑΤΡΙΚΟ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606023'
+  19: '200'
+- 0: 17342
+  1: ΛΑΖΙΟΥ,ΓΙΟΥΛΗ
+  2: ΑΣ ΣΗΝ ΛΑΛΙΑΝ Σ ΣΟ ΓΡΑΨΙΜΟΝ
+  4: 889.3ΛΑΖ
+  5: '22791'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2022'
+  11: '157'
+  12: ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+  13: ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606023'
+  19: '533545'
+- 0: 17343
+  1: ΧΑΤΖΗΘΕΟΔΩΡΙΔΗΣ,ΒΑΣΙΛΗΣ
+  2: ΨΗΓΜΑΤΑ ΠΟΝΤΙΑΚΗΣ ΛΟΓΟΤΕΧΝΙΑΣ
+  4: 889.3ΧΑΤ
+  5: '22784'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2021'
+  11: '144'
+  12: ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+  13: ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606023'
+  19: '323'
+- 0: 17344
+  1: ΧΑΤΖΗΘΕΟΔΩΡΙΔΗΣ,ΒΑΣΙΛΗΣ
+  2: ΣΑΝ ΤΑ ΠΟΥΛΙΑ ΣΤΗΝ ΜΠΟΡΑ
+  4: 920.7ΧΑΤ
+  5: '22800'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2019'
+  11: '445'
+  12: ΑΥΤΟΒΙΟΓΡΑΦΙΕΣ
+  13: ΒΙΟΓΡΑΦΙΕΣ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606022'
+  19: '494'
+- 0: 17345
+  1: ΙΩΑΝΝΙΔΟΥ,ΓΙΩΤΑ
+  2: ΙΣΚΙΛΙ
+  4: 889.3ΙΩΑ
+  5: '22797'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2020'
+  11: '348'
+  12: ΠΟΝΤΙΑΚΗ ΠΕΖΟΓΡΑΦΙΑ
+  13: ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606022'
+  19: '487'
+- 0: 17346
+  1: ΑΛΕΞΙΑΔΗΣ,ΘΩΜΑΣ
+  2: Ο ΠΟΛΕΜΑΡΧΟΣ ΤΗΣ ΕΥΠΑΤΟΡΙΑΣ ΑΝΑΣΤΑΣΙΟΣ ΠΑΠΑΔΟΠΟΥΛΟΣ
+  4: 938.71ΑΛΕ
+  5: '22796'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2020'
+  11: '324'
+  12: ΠΟΝΤΟΣ
+  13: ΙΣΤΟΡΙΑ
+  14: ΑΝΤΑΡΤΙΚΟ ΤΟΥ ΠΟΝΤΟΥ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606022'
+  19: '906'
+- 0: 17347
+  1: ΚΑΡΙΠΙΔΟΥ,ΑΝΝΥ
+  2: ΙΛΙΑΔΑ
+  4: 881ΚΑΡ
+  5: '22794'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2020'
+  11: '205'
+  12: ΠΟΝΤΙΑΚΗ ΔΙΑΛΕΚΤΟΣ
+  13: ΕΠΙΚΗ ΠΟΙΗΣΗ
+  14: ΟΜΗΡΟΥ ΙΛΙΑΔΑ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606022'
+  19: '739'
+- 0: 17348
+  1: ΠΕΤΡΟΠΟΥΛΟΥ,ΙΩΑΝΝΑ
+  2: Η ΣΜΥΡΝΗ ΤΩΝ ΒΙΒΛΙΩΝ
+  4: 070.509ΠΕΤ
+  5: '22792'
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '204'
+  12: ΕΚΔΟΤΕΣ ΚΑΙ ΕΚΔΟΣΕΙΣ ΣΤΗ ΣΜΥΡΝΗ
+  13: ΕΚΔΟΤΕΣ ΚΑΙ ΕΚΔΟΣΕΙΣ ΣΤΗ ΣΜΥΡΝΗ
+  14: ΕΚΔΟΤΕΣ ΚΑΙ ΕΚΔΟΣΕΙΣ ΣΤΗ ΣΜΥΡΝΗ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789609586'
+  19: '023'
+- 0: 17349
+  1: ΕΛΕΥΘΕΡΙΑΔΟΥ,ΡΟΖΑΛΙΑ
+  2: ΤΑΞΙΔΙ ΣΤΟΝ ΠΑΡΑΔΕΙΣΟ
+  4: 889.3ΕΛΕ
+  5: '22793'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2021'
+  11: '15'
+  12: ΠΟΝΤΙΑΚΗ ΠΕΖΟΓΡΑΦΙΑ
+  13: ΠΟΝΤΙΑΚΟ ΔΙΗΓΗΜΑ
+  14: ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606022'
+  19: '500'
+- 0: 17350
+  1: ΒΕΝΕΖΗΣ,ΗΛΙΑΣ
+  2: Η ΚΙΒΩΤΟΣ ΤΟΥ ΜΙΚΡΑΣΙΑΤΙΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
+  5: '22789'
+  9: ΑΘΗΝΑ
+  10: '2021'
+  11: '180'
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789609586'
+  19: '030'
+- 0: 17351
+  1: ΛΙΑΖΟΣ,ΝΙΚΟΛΑΟΣ
+  2: ΤΑ ΤΟΥΡΚΙΚΑ ΑΝΑΓΝΩΣΤΙΚΑ ΕΓΧΕΙΡΙΔΙΑ ΤΗΣ ΠΡΩΤΟΒΑΘΜΙΑΣ ΕΚΠΑΙΔ
+  4: 956.5ΛΙΑ
+  5: '22788'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2022'
+  11: '192'
+  12: ΕΚΠΑΙΔΕΥΣΗ-ΠΟΝΤΟΣ-ΔΥΤΙΚΗ ΘΡΑΚΗ
+  13: ΠΟΝΤΟΣ-ΕΚΠΑΙΔΕΥΣΗ
+  14: ΕΚΠΑΙΔΕΥΣΗ ΜΕΙΟΝΟΤΙΚΗ ΔΥΤΙΚΗ ΘΡΑΚΗ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606023'
+  19: '729'
+- 0: 17352
+  1: ΕΛΕΥΘΕΡΙΑΔΟΥ,ΡΟΖΑΛΙΑ
+  2: ΤΑ ΧΡΩΜΑΤΑ ΤΗΣ ΘΑΛΑΣΣΑΣ
+  4: 889.11ΕΛΕ
+  5: '22795'
+  8: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2022'
+  11: '16'
+  12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
+  13: ΠΟΝΤΟΣ-ΠΟΙΗΜΑΤΑ
+  14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
+  15: ΠΟΙΗΜΑΤΑ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΣ ΤΟΜΠΟΥΛΙΔΗΣ
+  18: '9789606023'
+  19: '484'
+- 0: 17353
+  1: ΔΑΡΛΑΣΗ,ΑΓΓΕΛΙΚΗ
+  2: ΟΙ ΟΝΕΙΡΟΦΥΛΑΚΕΣ ΚΑΙ Ο ΦΑΡΟΣ ΤΩΝ ΟΝΕΙΡΩΝ
+  4: 808.899ΔΑΡ
+  5: '19459'
+  8: ΠΑΤΑΚΗΣ
+  9: ΑΘΗΝΑ
+  10: '2013'
+  11: 266Σ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789601648'
+  19: '552'
+- 0: 17354
+  1: ΖΕΗ,ΑΛΚΗ
+  2: Ο ΜΕΓΑΛΟΣ ΠΕΡΙΠΑΤΟΣ ΤΟΥ ΠΕΤΡΟΥ
+  4: 808.899ΖΕΗ
+  5: '19462'
+  8: ΚΕΔΡΟΣ
+  9: ΑΘΗΝΑ
+  10: '1987'
+  11: 260Σ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9600400695'
+- 0: 17355
+  1: ΙΩΑΝΝΙΔΗΣ,Ι.Δ
+  2: ΚΑΒΑΛΑ ΣΤΟ ΧΡΟΝΟΔΙΑΒΙΤΗ
+  4: 808.899ΙΩΑ
+  5: '22801'
+  8: ΚΑΣΤΑΝΙΩΤΗΣ
+  9: ΑΘΗΝΑ
+  10: '1989'
+  11: '151'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9600303525'
+- 0: 17356
+  1: ΙΩΑΝΝΟΥ,ΓΙΩΡΓΟΣ
+  2: ΠΑΡΑΜΥΘΙΑ ΤΟΥ ΛΑΟΥ ΜΑΣ
+  4: 808.899ΙΩΑ
+  5: '20638'
+  8: ΕΡΜΗΣ
+  9: ΑΘΗΝΑ
+  10: '2008'
+  11: 375Σ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17357
+  1: ΚΩΖΙΝΣ,ΜΑΡΓΚΑΡΕΤ
+  2: ΒΕΝΙΑΜΙΝ ΦΡΑΓΚΛΙΝΟΣ
+  4: 808.899ΚΩΖ
+  5: '20413'
+  8: ΑΤΛΑΝΤΙΣ
+  9: ΑΘΗΝΑ
+  11: 159Σ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΣΠΥΡΙΔΩΝ ΣΠΥΡΟΥ
+- 0: 17358
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  2: Ο ΚΥΡΙΑΡΧΟΣ ΤΟΥ ΚΟΣΜΟΥ
+  4: 808.899ΒΕΡ
+  5: 9170Α
+  6: Λ.ΟΛΥΜΠΙΟΥ
+  8: ΑΤΤΙΚΟΣ
+  9: ΑΘΗΝΑ
+  11: '212'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17359
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  2: ΚΟΥΡΣΑΡΟΙ ΤΟΥ ΑΙΓΑΙΟΥ
+  4: 808.899ΒΕΡ
+  5: 9175Α
+  6: Δ.Π.ΚΩΣΤΕΛΕΝΟΣ
+  8: ΑΤΤΙΚΟΣ
+  9: ΑΘΗΝΑ
+  11: '206'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17360
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  2: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
+  4: 808.899ΒΕΡ
+  5: '13461'
+  6: Λ.ΟΛΥΜΠΙΟΥ
+  8: ΑΤΤΙΚΟΣ
+  9: ΑΘΗΝΑ
+  11: '260'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17361
+  1: ΑΝΤΕΡΣΕΝ,ΧΑΝΣ ΚΡΙΣΤΙΑΝ
+  2: ΑΠΑΝΤΑ Ε
+  4: 808.899ΑΝΤ
+  6: Σ.ΠΡΩΤΟΠΑΠΑ
+  8: ΑΡΣΕΝΙΔΗΣ
+  9: ΑΘΗΝΑ
+  11: '188'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17362
+  1: ΑΝΤΡΙΟΥΣ,ΤΖΟΥΛΙ
+  2: ΜΑΝΤΥ
+  4: 808.899ΑΝΤ
+  6: Κ.ΣΙΝΟΥ
+  8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
+  9: ΑΘΗΝΑ
+  11: '148'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17363
+  1: Χ.Σ.
+  2: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΚΟΥΣΤΩ
+  3: ΟΑΣΗ ΣΤΟ ΔΙΑΣΤΗΜΑ
+  4: 808.899ΚΟΥ
+  5: '7402'
+  6: ΟΜΗΡΟΣ ΑΒΡΑΜΙΔΗΣ
+  8: ΑΛΚΥΩΝ
+  9: ΑΘΗΝΑ
+  10: '1973'
+  11: '141'
+  12: ΠΑΙΔΙΚΗ ΒΙΒΛΙΟΘΗΚΗ-ΕΓΚΥΚΛΟΑΠΙΔΕΙΑ
+  13: ΠΑΙΔΙΚΗ ΒΙΒΛΙΟΘΗΚΗ
+  14: ΕΓΚΥΚΛΟΑΠΙΔΕΙΑ
+  17: ΤΟΜΟΣ 1
+- 0: 17364
+  1: ΒΑΡΕΛΛΑ,ΑΓΓΕΛΙΚΗ
+  2: ΤΗΛΕΦΩΝΗΜΑΤΑ ΚΙ ΕΝΑΣ ΛΑΓΟΣ
+  4: 808.899ΒΑΡ
+  5: '20419'
+  8: ΜΙΝΩΑΣ ΕΚΔΟΣΕΙΣ
+  9: ΑΘΗΝΑ
+  10: '2003'
+  11: '77'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  19: '9605421038'
+- 0: 17365
+  1: ΚΟΛΕΤ,ΒΙΒΙΕ
+  2: ΤΟ ΠΟΛΙΚΟ ΑΣΤΕΡΙ
+  4: 808.899ΚΟΛ
+  5: '20427'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '1990'
+  11: '210'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  19: '9607020030'
+- 0: 17366
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  2: ΜΠΡΟΣΤΑ ΣΤΗ ΣΗΜΑΙΑ
+  4: 808.899ΒΕΡ
+  5: '22804'
+  8: ΑΣΤΗΡ
+  9: ΑΘΗΝΑ
+  10: '1978'
+  11: '272'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17367
+  1: ΓΚΟΡΚΙ,ΜΑΞΙΜ
+  2: Η ΦΛΟΓΕΡΗ ΚΑΡΔΙΑ ΤΟΥ ΝΤΑΝΚΟ
+  4: 808.899ΓΚΟ
+  5: '20152'
+  8: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ
+  9: ΑΘΗΝΑ
+  10: '1983'
+  11: '98'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17368
+  1: ΓΟΥΕΛΣ,ΡΕΝΑΤΕ
+  2: Η ΜΕΛΑΝΙ ΚΑΙ ΤΑ ΜΑΓΙΑ
+  4: 808.899ΓΟΥ
+  5: '19455'
+  8: ΠΑΤΑΚΗ
+  9: ΑΘΗΝΑ
+  11: '125'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  19: '9606000389'
+- 0: 17369
+  1: ΓΟΥΛΙΜΗ,ΑΛΚΗΣ
+  2: Η ΑΟΡΑΤΗ ΣΕΛΙΔΑ
+  4: 808.899ΓΟΥ
+  5: '22805'
+  8: ΝΕΑΝΙΚΗ ΒΙΒΛΙΟΘΗΚΗ
+  9: ΑΘΗΝΑ
+  10: '1989'
+  11: '385'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  19: 960030260Χ
+- 0: 17370
+  1: ΓΟΥΠΟΣ,ΘΕΟΔΩΡΟΣ
+  2: Η ΓΛΩΣΣΑ ΜΟΥ ΓΙΑ ΤΗΝ Α ΔΗΜΟΤΙΚΟΥ
+  4: 808.899ΓΟΥ
+  5: '20630'
+  8: ΕΚΔΟΣΕΙΣ ΚΑΜΠΑΝΑ
+  9: ΑΘΗΝΑ
+  11: '230'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  19: '9602572337'
+- 0: 17371
+  1: ΓΙΑΝΣΣΟΝ,ΤΟΥΒΕ
+  2: ΤΟ ΚΑΠΕΛΟ ΤΟΥ ΜΑΓΟΥ ΜΟΥΜΕΡΛΙΝ
+  4: 808.899ΓΙΑ
+  5: '22700'
+  8: ΠΑΤΑΚΗ
+  9: ΑΘΗΝΑ
+  11: '174'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789601646'
+  19: '992'
+- 0: 17372
+  1: ΓΕΩΡΓΟΣΤΑΘΗ,ΕΛΕΝΗ
+  2: ΧΑΘΗΚΕ Η ΜΠΑΛΑ
+  4: 808.899ΓΕΩ
+  5: '22597'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2017'
+  11: '105'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180118'
+  19: '759'
+- 0: 17373
+  1: ΓΚΑΛΚΙΝΑ,ΑΝΑΣΤΑΣΙΑ
+  2: ΜΙΑ ΥΠΕΡΟΧΗ ΜΕΡΑ
+  4: 808.899ΓΚΑ
+  5: '22615'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  11: '30'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17374
+  1: ΛΑΡΣΟΝ,ΟΣΑ
+  2: PAX ΤΟ ΑΒΑΠΤΙΣΤΟ
+  4: 808.899ΛΑΡ
+  5: '22601'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  11: '205'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180119'
+  19: '510'
+- 0: 17375
+  1: ΛΑΡΙ,Χ.Ι
+  2: ΨΗΦΙΑΚΟΙ ΕΙΣΒΟΛΕΙΣ
+  4: 808.899ΛΑΡ
+  5: '22603'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2013'
+  11: '105'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180108'
+  19: '224'
+- 0: 17376
+  1: ΛΙΝΤΓΚΡΕΝ,ΑΣΤΡΙΝΤ
+  2: ΣΚΑΝΤΑΛΙΕΣ ΣΤΟ ΜΙΚΡΟ ΧΩΡΙΟ
+  4: 808.899ΛΙΝ
+  5: '20418'
+  8: ΜΕΤΟΠΗ
+  11: '125'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17377
+  1: ΛΙΝΤΓΚΡΕΝ,ΑΣΤΡΙΝΤ
+  2: Η ΠΙΠΗ ΦΑΚΙΔΟΜΥΤΗ ΣΤΙΣ ΝΟΤΙΕΣ ΘΑΛΑΣΣΕΣ
+  4: 808.899ΛΙΝ
+  5: '22608'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '160'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180138'
+  19: '696'
+- 0: 17378
+  1: ΜΑΛΟ,ΕΚΤΟΡΑΣ
+  2: ΧΩΡΙΣ ΟΙΚΟΓΕΝΕΙΑ
+  4: 808.899ΜΑΛ
+  5: '20637'
+  8: ΣΠ. ΔΑΡΕΜΑ
+  9: ΑΘΗΝΑ
+  11: '483'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17379
+  1: ΜΑΝΔΗΛΑΡΑΣ,ΦΙΛΙΠΠΟΣ
+  2: Ο ΠΑΠΠΟΥΣ ΜΑΣ ΑΦΗΣΕ
+  4: 808.899ΜΑΝ
+  5: '22697'
+  8: ΠΑΤΑΚΗ
+  9: ΑΘΗΝΑ
+  11: '56'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789601628'
+  19: '622'
+- 0: 17380
+  1: ΜΑΥΡΟΜΑΤΗΣ,ΘΩΜΑΣ
+  2: ΑΛΗΘΙΝΟΙ ΗΡΩΕΣ - ΗΡΩΕΣ ΤΟΥ ΠΟΝΤΙΑΚΟΥ ΕΛΛΗΝΙΣΜΟΥ
+  4: 808.899ΜΑΥ
+  5: '21511'
+  8: ΕΚΔΟΣΕΙΣ ΕΑΡ ΠΑΙΔΙΚΑ
+  9: ΑΘΗΝΑ
+  10: '2022'
+  11: '15'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786185368'
+  19: '951'
+- 0: 17381
+  1: ΜΙΛΑΝΙ,ΜΙΝΟ
+  2: ΣΑΝΤΑ ΑΛΕΓΚΡΑΝΤΣΑ
+  4: 808.899ΜΙΛ
+  5: '20421'
+  6: ΑΛΚΗ ΤΡΟΠΑΙΤΗ
+  8: ΧΑΡΗ ΠΑΤΣΗ
+  9: ΑΘΗΝΑ
+  11: '212'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17382
+  1: ΟΥΓΚΩ,ΒΙΚΤΩΡ
+  2: ΟΙ ΑΘΛΙΟΙ
+  4: 808.899ΟΥΓ
+  5: '19892'
+  8: ΕΚΔΟΣΕΙΣ ΑΣΤΗΡ
+  9: ΑΘΗΝΑ
+  11: '215'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17383
+  1: ΟΥΓΚΩ,ΒΙΚΤΩΡ
+  2: Η ΠΑΝΑΓΙΑ ΤΩΝ ΠΑΡΙΣΙΩΝ
+  4: 808.899ΟΥΓ
+  5: '22806'
+  8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
+  9: ΑΘΗΝΑ
+  11: '128'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17384
+  1: NOZIERE,JEAN-PAUL
+  2: ΕΚΔΙΚΗΣΗ ΤΙΤΟΣ
+  4: 808.899NOZ
+  5: '22681'
+  8: Χ.Ε ΔΑΡΔΑΝΟΣ
+  9: ΑΘΗΝΑ
+  10: '1998'
+  11: '180'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  19: '9603800465'
+- 0: 17385
+  1: ΝΟΡΘΦΙΛΝΤ,ΓΚΑΡΙ
+  2: ΙΟΥΛΙΟΣ ΖΕΒΡΑ ΒΙΒΛΙΟ 2
+  4: 808.899ΝΟΡ
+  5: '22606'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2017'
+  11: '250'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180118'
+  19: '698'
+- 0: 17386
+  1: ΝΟΡΘΦΙΛΝΤ,ΓΚΑΡΙ
+  2: ΙΟΥΛΙΟΣ ΖΕΒΡΑ ΒΙΒΛΙΟ 3
+  4: 808.899ΝΟΡ
+  5: '22607'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2018'
+  11: '300'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180125'
+  19: '177'
+- 0: 17387
+  1: Χ.Σ
+  2: Η ΜΑΓΕΜΕΝΗ ΒΑΣΙΛΟΠΟΥΛΑ
+  4: 808.899Χ.Σ
+  5: '22808'
+  8: ΑΓΚΥΡΑ
+  9: ΑΘΗΝΑ
+  11: '20'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9602343060'
+- 0: 17388
+  1: ΤΣΙΜΙΚΑΛΗ,ΠΙΠΙΝΑ
+  2: ΤΟ ΚΑΛΟΚΑΙΡΑΚΙ - ΠΑΙΖΩ ΚΑΙ ΜΑΘΑΙΝΩ
+  4: 808.899ΤΣΙ
+  5: '22807'
+  8: ΑΓΚΥΡΑ
+  9: ΑΘΗΝΑ
+  11: '20'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9602343052'
+- 0: 17389
+  1: ΝΤΙΞΟΝ,ΦΡΑΝΚΛΙΝ
+  2: ΟΙ ΓΙΓΑΝΤΕΣ ΤΗΣ ΕΡΗΜΟΥ
+  4: 808.899ΝΤΙ
+  5: '22809'
+  8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
+  9: ΑΘΗΝΑ
+  11: '170'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17390
+  1: ΟΥΑΛΙΑΜΣ,ΝΤΕΙΒΙΝΤ
+  2: Ο ΧΛΑΠΑΤΣΑ
+  4: 808.899ΟΥΑ
+  5: '22598'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2022'
+  11: '325'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180141'
+  19: '986'
+- 0: 17391
+  1: ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+  2: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΤΑΛΑΝΤΟΥΧΑ ΠΟΠ ΣΤΑΡ
+  4: 808.899ΡΑΣ
+  5: '22577'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2011'
+  11: 320ΠΑΙ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789604964'
+  19: 079
+- 0: 17392
+  1: ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+  2: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΧΑΡΟΥΜΕΝΗ ΚΑΡΔΙΟΚΑΤΑΚΤΗΤΡΙΑ
+  4: 808.899ΡΑΣ
+  5: '22578'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2013'
+  11: '350'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180103'
+  19: '922'
+- 0: 17393
+  1: ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+  2: ΦΤΙΑΞΕ ΤΟ ΔΙΚΟ ΣΟΥ ΞΕΝΕΡΩΤΟ ΗΜΕΡΟΛΟΓΙΟ
+  4: 808.899ΡΑΣ
+  5: '22575'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2011'
+  11: '350'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789604968'
+  19: '930'
+- 0: 17394
+  1: ΡΑΣΕΛ,ΡΕΙΤΣΕΛ-ΡΕΝΕ
+  2: ΙΣΤΟΡΙΕΣ ΑΠΟ ΜΙΑ ΟΧΙ ΚΑΙ ΤΟΣΟ ΛΑΜΠΕΡΗ TV STAR
+  4: 808.899ΡΑΣ
+  5: '22576'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2014'
+  11: '350'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180108'
+  19: '118'
+- 0: 17395
+  1: ΕΞΥΠΕΡΥ,ΑΝΤΟΥΑΝ
+  2: Ο ΜΙΚΡΟΣ ΠΡΙΓΚΙΠΑΣ
+  4: 808.899ΕΞΥ
+  5: '22815'
+  8: ΝΕΦΕΛΗ
+  9: ΑΘΗΝΑ
+  10: '1984'
+  11: '97'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17396
+  1: ΣΑΡΗ,ΖΩΡΖ
+  2: Ε.Π
+  4: 808.899ΣΑΡ
+  5: '22814'
+  8: ΠΑΤΑΚΗ
+  9: ΑΘΗΝΑ
+  10: '1995'
+  11: '254'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9603605115'
+- 0: 17397
+  1: ΣΑΡΗ,ΖΩΡΖ
+  2: ΤΟ ΨΕΜΑ
+  4: 808.899ΣΑΡ
+  5: '22813'
+  8: ΚΕΔΡΟΣ
+  9: ΑΘΗΝΑ
+  10: '1987'
+  11: '144'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9600400660'
+- 0: 17398
+  1: ΣΑΡΗ,ΖΩΡΖ
+  2: ΤΟ ΠΑΡΑΡΑΔΙΑΣΜΑ
+  4: 808.899ΣΑΡ
+  5: '22812'
+  8: ΠΑΤΑΚΗ
+  9: ΑΘΗΝΑ
+  10: '1989'
+  11: '205'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9602934778'
+- 0: 17399
+  1: ΣΕΡΕΦΑΣ,ΣΑΚΗΣ
+  2: ΠΩΛΟΥΝΤΑΙ ΣΚΙΕΣ
+  4: 808.899ΣΕΡ
+  5: '22691'
+  8: ΠΑΤΑΚΗ
+  9: ΑΘΗΝΑ
+  11: '40'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789601638'
+  19: '478'
+- 0: 17400
+  1: ΣΙΝΟΥ,ΚΙΡΑ
+  2: ΤΟ ΤΕΛΟΣ ΤΩΝ ΤΕΡΑΤΩΝ
+  4: 808.899ΣΙΝ
+  5: '22811'
+  8: ΚΕΔΡΟΣ
+  9: ΑΘΗΝΑ
+  10: '1987'
+  11: '160'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9600402868'
+- 0: 17401
+  1: ΣΠΙΡΙ,ΓΙΟΧΑΝΑ
+  2: ΧΑΙΝΤΙ
+  4: 808.899ΣΠΙ
+  5: '22810'
+  8: ΚΑΘΗΜΕΡΙΝΗ
+  9: ΑΘΗΝΑ
+  11: '48'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789604750'
+  19: '788'
+- 0: 17402
+  1: ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+  2: ΑΥΡΙΟ ΕΙΝΑΙ ΚΥΡΙΑΚΗ
+  4: 808.899ΣΟΥ
+  5: '17875'
+  8: ΝΕΟΙ ΑΚΡΙΤΕΣ
+  9: ΑΘΗΝΑ
+  10: '1999'
+  11: '56'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9607006933'
+- 0: 17403
+  1: ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+  2: Ο ΜΕΓΑΛΟΣ ΑΠΟΧΑΙΡΕΤΙΣΜΟΣ
+  4: 808.899ΣΟΥ
+  5: '22596'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2021'
+  11: '190'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789607021'
+  19: '854'
+- 0: 17404
+  1: ΣΟΦΟΚΛΗ
+  2: ΟΙΔΙΠΟΥΣ ΤΥΡΑΝΝΟΣ
+  4: 808.899ΣΟΦ
+  5: '19984'
+  8: ΣΑΒΒΑΛΑΣ
+  9: ΑΘΗΝΑ
+  10: '2012'
+  11: '55'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9604609734'
+- 0: 17405
+  1: ΣΤΑΝΤΛΕΡ,ΑΛΕΞΑΝΤΕΡ
+  2: ΤΖΟΥΛΙΑΝ ΡΟΝΤΡΙΓΚΕΖ
+  4: 808.899ΣΤΑ
+  5: '22690'
+  8: ΠΑΤΑΚΗ
+  9: ΑΘΗΝΑ
+  11: '140'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17406
+  1: ΣΤΟΟΥ-ΜΠΙΤΣΕΡ,ΧΑΡΙΕΤ
+  2: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+  4: 808.899ΣΤΟ
+  5: '20973'
+  8: ΤΑ ΝΕΑ
+  9: ΑΘΗΝΑ
+  10: '2018'
+  11: '225'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789605039'
+  19: '554'
+- 0: 17407
+  1: ΣΤΟΟΥ,ΜΠΗΤΣΕΡ
+  2: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+  4: 808.899ΣΤΟ
+  5: '20640'
+  8: ΠΑΓΚΟΣΜΙΑ ΛΟΓΟΤΕΧΝΙΑ
+  9: ΑΘΗΝΑ
+  11: '125'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17408
+  1: ΣΤΡΑΤΟΛΑΤΗ-ΝΙΚΗΤΑ,ΧΡ.
+  2: ΤΑ ΜΑΤΙΑ ΤΗΣ ΜΑΝΑΣ
+  4: 808.899ΣΤΡ
+  5: '16257'
+  8: ΑΛΚΑΙΟΣ
+  9: ΑΘΗΝΑ
+  11: 149Σ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17409
+  1: ΣΟΥΡΕΛΗ-ΓΡΗΓΟΡΙΑΔΟΥ,ΓΑΛΑΤΕΙΑ
+  2: ΦΟΥΡΦΟΥΡΗΣ Ο ΚΟΤΣΥΦΑΣ
+  4: 808.899ΣΟΥ
+  5: '22740'
+  7: 9Η
+  8: ΠΑΤΑΚΗΣ
+  9: ΑΘΗΝΑ
+  10: '1999'
+  11: '72'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΙΑΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  19: '9603602051'
+- 0: 17410
+  1: ΤΡΙΑΝΤΑΦΥΛΛΟΥ,ΣΩΤΗ
+  2: Η ΜΙΛΕΝΑ ΚΑΙ ΤΟ ΦΡΙΚΤΟ ΨΑΡΙ
+  4: 808.899ΤΡΙ
+  5: '22702'
+  7: 1Η
+  8: ΠΑΤΑΚΗΣ
+  9: ΑΘΗΝΑ
+  10: '2011'
+  11: '25'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789601640'
+  19: '266'
+- 0: 17411
+  1: ΛΑΓΟΥ-ΠΑΠΑΚΟΥ,ΑΥΓΗ
+  2: ΟΙ ΘΑΥΜΑΣΙΕΣ ΗΛΙΑΧΤΙΔΕΣ
+  4: 808.899ΛΑΓ
+  5: '20645'
+  7: 3Η
+  8: ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ
+  9: ΑΘΗΝΑ
+  10: '1983'
+  11: '47'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17412
+  1: ΠΑΠΑΔΙΑΜΑΝΤΗΣ
+  2: ΠΑΙΔΙΚΑ ΔΙΗΓΗΜΑΤΑ
+  4: 808.899ΠΑΠ
+  5: '20631'
+  6: ΑΘΑΝ.ΘΕΟΔΩΡΑΚΗ
+  8: ΖΑΝΑΚΗ
+  9: ΑΘΗΝΑ
+  11: '188'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17413
+  1: ΠΑΣΧΟΥ,ΒΑΣΙΛΗ
+  2: ΠΡΩΤΟΠΟΡΟΙ ΣΤΟ ΔΙΑΣΤΗΜΑ
+  4: 808.899ΠΑΣ
+  5: '20424'
+  8: ΦΙΛΟΛΟΓΙΚΗ
+  9: ΑΘΗΝΑ
+  11: '196'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17414
+  1: ΠΕΡΩ,ΣΟΥΖΑΝΑ
+  2: Η ΕΚΔΙΚΗΣΗ ΤΟΥ ΡΟΜΠΕΝ
+  4: 808.899ΠΕΡ
+  5: '20422'
+  6: ΟΘ.ΑΡΓΥΡΟΠΟΥΛΟΥ
+  8: ΧΑΡΗ ΠΑΤΣΗ
+  9: ΑΘΗΝΑ
+  10: '1967'
+  11: '199'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΕΥΣΤΑΘΙΟΣ ΚΑΓΚΑΡΑΣ
+- 0: 17415
+- 0: 17416
+  1: DAHL,ROALD
+  2: ΝΤΑΝΙ,Ο ΠΡΩΤΑΘΛΗΤΗΣ ΤΟΥ ΚΟΣΜΟΥ
+  4: 808.899DAH
+  5: '22592'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '250'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180137'
+  19: '248'
+- 0: 17417
+  1: DAHL,ROALD
+  2: Ο ΤΖΙΜΗΣ ΚΑΙ ΤΟ ΓΙΓΑΝΤΟΡΟΔΑΚΙΝΟ
+  4: 808.899DAH
+  5: '22591'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '200'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180137'
+  19: '255'
+- 0: 17418
+  1: DAHL,ROALD
+  2: ΜΑΤΙΛΝΤΑ
+  4: 808.899DAH
+  5: '22590'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '280'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180137'
+  19: '224'
+- 0: 17419
+  1: DAHL,ROALD
+  2: Ο ΤΣΑΡΛΙ ΚΑΙ ΤΟ ΕΡΓΟΣΤΑΣΙΟ ΣΟΚΟΛΑΤΑΣ
+  4: 808.899DAH
+  5: '22589'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '210'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180137'
+  19: '309'
+- 0: 17420
+  1: DAHL,ROALD
+  2: Ο ΑΠΙΘΑΝΟΣ ΚΥΡΙΟΣ ΦΟΞ
+  4: 808.899DAH
+  5: '22588'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '95'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180137'
+  19: '231'
+- 0: 17421
+  1: DAHL,ROALD
+  2: ΟΙ ΜΑΓΙΣΣΕΣ
+  4: 808.899DAH
+  5: '22587'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '240'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180137'
+  19: '262'
+- 0: 17422
+  1: DAHL,ROALD
+  2: ΟΙ ΒΛΑΚΕΝΤΙΟΙ
+  4: 808.899DAH
+  5: '22586'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2020'
+  11: '115'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180137'
+  19: '286'
+- 0: 17423
+  1: ΤΣΙΑΛΤΑ,ΕΛΕΝΗ
+  2: ΕΝΑ ΚΟΥΒΑΡΙ ΜΥΣΤΙΚΑ
+  4: 808.899ΤΣΙ
+  5: '22595'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2015'
+  11: '75'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180109'
+  19: '306'
+- 0: 17424
+  1: ΤΣΙΛΙΜΕΝΗ,ΤΑΣΟΥΛΑ
+  2: Η ΑΠΑΓΩΓΗ ΤΗΣ ΜΟΒ ΓΡΑΒΑΤΑΣ
+  4: 808.899ΤΣΙ
+  5: '19940'
+  8: ΚΕΔΡΟΣ
+  9: ΑΘΗΝΑ
+  10: '2006'
+  11: '50'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: 960043333Χ
+- 0: 17425
+  1: ΧΙΝΤΛΕΥ,ΚΕΙΤ
+  2: ΟΔΟΣ ΧΑΡΑΣ - Η ΜΠΟΥΓΑΤΣΑ ΠΟΥ ΠΕΤΑΕΙ!
+  4: 808.899ΧΙΤ
+  5: '22621'
+  8: ΠΑΤΑΚΗ
+  9: ΑΘΗΝΑ
+  11: '20'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789601699'
+  19: '790'
+- 0: 17426
+  1: ΧΙΤΣΚΟΚ,ΑΛΦΡΕΝΤ
+  2: ΜΥΣΤΗΡΙΟ ΤΗΣ ΚΛΕΜΜΕΝΗΣ ΦΑΛΑΙΝΑΣ
+  4: 808.899ΧΙΤ
+  5: '20089'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '1992'
+  11: '190'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9602740272'
+- 0: 17427
+  1: ΧΟΡΤΙΑΤΗ,ΘΕΤΗ
+  2: Ο ΚΟΚΚΙΝΟΣ ΚΑΚΤΟΣ
+  4: 808.899ΧΟΡ
+  5: '22818'
+  8: ΠΕΡΙΠΛΟΥΣ
+  9: ΑΘΗΝΑ
+  10: '2000'
+  11: '95'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9608151422'
+- 0: 17428
+  1: COLEMAN,MICHAEL
+  2: ΣΦΑΛΜΑ ΣΥΣΤΗΜΑΤΟΣ
+  4: 808.899COL
+  5: '22689'
+  8: ΜΕΤΑΙΧΜΙΟ ΠΑΙΔΙΚΟ
+  9: ΑΘΗΝΑ
+  10: '2002'
+  11: '152'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9603753548'
+- 0: 17429
+  1: DETHISE,JEANNE
+  2: ΤΟ ΔΕΛΦΙΝΙ ΤΟΥ ΓΙΩΡΓΑΚΗ
+  4: 808.899DET
+  5: '17872'
+  8: ΠΑΠΑΔΟΠΟΥΛΟΣ
+  9: ΑΘΗΝΑ
+  11: '22'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17430
+  1: LEGO
+  2: ΣΤΟΝ ΠΥΡΟΣΒΕΣΤΙΚΟ ΣΤΑΘΜΟ LEGO CITY
+  4: 808.899LEG
+  5: '22620'
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  11: '10'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9786180141'
+  19: '351'
+- 0: 17431
+  1: MILLER,FRANK
+  2: BATMAN Ο ΣΚΟΤΕΙΝΟΣ ΙΠΠΟΤΗΣ ΕΠΙΣΤΡΕΦΕΙ
+  4: 808.899MIL
+  5: '22817'
+  8: ANUBIS
+  9: ΑΘΗΝΑ
+  10: '2008'
+  11: '200'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789603066'
+  19: '729'
+- 0: 17432
+  1: EXUPERY,ANTOINE
+  2: Ο ΜΙΚΡΟΣ ΠΡΙΓΚΙΠΑΣ
+  4: 808.899EXU
+  5: '19464'
+  8: ΠΕΡΙΒΟΛΑΚΙ
+  9: ΑΘΗΝΑ
+  11: '80'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9607412648'
+- 0: 17433
+  1: DUMAS,ALEXANDRE
+  2: ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+  4: 808.899DUM
+  5: '22816'
+  8: ΑΛΚΥΩΝ
+  9: ΑΘΗΝΑ
+  10: '2004'
+  11: '260'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9603260967'
+- 0: 17434
+  1: STAHL,P.G
+  2: ΤΑ ΑΣΗΜΕΝΙΑ ΠΑΓΟΠΕΔΙΛΑ
+  4: 808.899STA
+  5: '20688'
+  8: ΑΓΚΥΡΑ ΠΑΙΔΙΚΑ
+  9: ΑΘΗΝΑ
+  11: '120'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+- 0: 17435
+- 0: 17436
+  1: ΚΑΛΑΤΖΟΠΟΥΛΟΣ,ΓΙΑΝΝΗΣ
+  2: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ ΚΑΙ ... ΕΞΥΠΝΟΥΣ ΜΕΓΑΛΟΥΣ
+  4: 886.2ΚΑΛ
+  5: 22839,22840
+  8: ΦΙΛΝΤΙΣΙ
+  9: ΑΘΗΝΑ
+  10: '2021'
+  11: '335'
+  12: ΘΕΑΤΡΟ
+  13: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ
+  14: ΘΕΑΤΡΙΚΟ ΓΙΑ ΠΑΙΔΙΑ
+  17: ΔΩΡΕΑ ΕΛΠΙΔΟΦΟΡΟΣ ΙΝΤΖΕΜΠΕΛΗΣ
+  18: '9786185456'
+  19: '481'
+  30: 2 ΤΟΜΟΙ
+- 0: 17437
+  1: ΓΙΑΝΣΣΟΝ,ΤΟΥΒΕ
+  2: ΘΑΛΑΣΣΙΝΟ ΤΑΞΙΔΙ
+  4: 808.899ΓΙΑ
+  5: '22847'
+  6: ΜΑΡΙΑ ΑΓΓΕΛΙΔΟΥ
+  8: ΠΑΤΑΚΗΣ
+  9: ΑΘΗΝΑ
+  10: '2013'
+  11: '248'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789601647'
+  19: '012'
+- 0: 17438
+  1: ΔΕΛΤΑ,Π.Σ
+  2: ΜΑΓΚΑΣ
+  4: 808.899ΔΕΛ
+  5: '22848'
+  8: ΕΣΤΙΑ
+  9: ΑΘΗΝΑ
+  10: '1975'
+  11: '305'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17439
+  1: ΔΟΥΜΑΣ,ΑΛΕΞΑΝΔΡΟΣ
+  2: ΟΙ ΤΡΕΙΣ ΣΩΜΑΤΟΦΥΛΑΚΕΣ
+  4: 808.899ΔΟΥ
+  5: '22851'
+  8: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ
+  9: ΑΘΗΝΑ
+  11: '234'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789606756'
+  19: '382'
+- 0: 17440
+  1: ΠΟΥΣΚΙΝ,ΑΛΕΞΑΝΤΡ
+  2: Η ΚΟΡΗ ΤΟΥ ΛΟΧΑΓΟΥ
+  4: 808.899ΠΟΥ
+  5: '22852'
+  8: ΕΡΕΥΝΗΤΕΣ
+  9: ΑΘΗΝΑ
+  11: '140'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789603684'
+  19: '336'
+- 0: 17441
+  1: ΝΤΕΦΟΕ,ΝΤΑΝΙΕΛ
+  2: ΡΟΒΙΝΣΩΝ ΚΡΟΥΣΟΣ
+  4: 808.899ΝΤΕ
+  5: '22853'
+  6: ΓΙΑΝΝΗΣ ΚΟΤΣΙΚΑΣ
+  8: ΠΑΠΑΔΗΜΗΤΡΙΟΥ
+  9: ΑΘΗΝΑ
+  10: '2016'
+  11: '126'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789605851'
+  19: 095
+- 0: 17442
+  1: ΝΤΙΚΕΝΣ,ΚΑΡΟΛ
+  2: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
+  4: 808.899ΝΤΙ
+  5: '22854'
+  6: ΔΗΜΗΤΡΗΣ ΚΟΡΙΝΗΣ
+  8: ΠΑΠΑΔΗΜΗΤΡΙΟΥ
+  9: ΑΘΗΝΑ
+  10: '2016'
+  11: '319'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789605851'
+  19: '071'
+- 0: 17443
+  1: ΤΟΥΕΙΝ,ΜΑΡΚ
+  2: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΤΟΜ ΣΟΓΙΕΡ
+  4: 808.899ΤΟΥ
+  5: '22855'
+  6: ΑΘΑΝΑΣΙΑ ΜΠΙΡΗ
+  8: ΚΑΛΟΚΑΘΗ
+  9: ΑΘΗΝΑ
+  10: '2008'
+  11: '48'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789603963'
+  19: '905'
+- 0: 17444
+  1: ΠΑΠΑΝΤΩΝΙΟΥ,ΖΑΧΑΡΙΑΣ
+  2: ΤΑ ΨΗΛΑ ΒΟΥΝΑ
+  4: 808.899ΠΑΠ
+  5: '22856'
+  8: ΠΕΡΙΒΟΛΑΚΗ
+  9: ΑΘΗΝΑ
+  10: '1996'
+  11: '227'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9607412273'
+- 0: 17445
+  1: ΝΤΙΚΕΝΣ,ΤΣΑΡΛΣ
+  2: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
+  4: 808.899ΝΤΙ
+  5: '22857'
+  6: ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+  8: ΜΙΝΩΑΣ
+  9: ΑΘΗΝΑ
+  10: '2013'
+  11: '211'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789604817'
+  19: '429'
+- 0: 17446
+  1: ΣΤΟΟΥ,ΧΑΡΙΕΤ-ΜΠΙΤΣΕΡ
+  2: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
+  4: 808.899ΣΤΟ
+  5: '22858'
+  6: ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+  8: ΜΙΝΩΑΣ
+  9: ΑΘΗΝΑ
+  10: '2013'
+  11: '219'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789604816'
+  19: '606'
+- 0: 17447
+  1: ΡΟΟΥΛΙΝΓΚ,ΤΖ.Κ
+  2: Ο ΧΑΡΙ ΠΟΤΕΡ ΚΑΙ Η ΚΑΜΑΡΑ ΜΕ ΤΑ ΜΥΣΤΙΚΑ
+  4: 808.899ΡΟΟ
+  5: '22864'
+  6: ΚΑΙΤΗ ΟΙΚΟΝΟΜΟΥ
+  8: ΨΥΧΟΓΙΟΣ
+  9: ΑΘΗΝΑ
+  10: '2017'
+  11: 358Σ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789602744'
+  19: '017'
+- 0: 17448
+  1: ΦΙΝΕΜΟΡ,ΤΖΟΝ
+  2: Ο ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+  4: 808.899ΦΙΝ
+  5: '22849'
+  6: ΕΡ. ΜΠΑΡΤΖΙΝΟΠΟΥΛΟΣ
+  8: ΑΓΚΥΡΑ
+  9: ΑΘΗΝΑ
+  10: '2016'
+  11: '220'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789605851'
+  19: 088
+- 0: 17449
+  1: PYLE,HOWARD
+  2: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΡΟΜΠΕΝ ΤΩΝ ΔΑΣΩΝ
+  4: 808.899PYL
+  5: '22850'
+  9: ΑΘΗΝΑ
+  10: '2013'
+  11: '64'
+  12: ΑΙΔΙΚΗ ΠΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17450
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  2: ΜΙΧΑΗΛ ΣΤΡΟΓΚΟΦ
+  4: 808.899ΒΕΡ
+  5: '22859'
+  8: ΣΜΥΡΝΙΩΤΑΚΗΣ
+  9: ΑΘΗΝΑ
+  11: '254'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9602990678'
+- 0: 17451
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  2: Ο ΔΕΚΑΠΕΝΤΑΕΤΗΣ ΠΛΟΙΑΡΧΟΣ
+  4: 808.899ΒΕΡ
+  5: '22860'
+  8: ΣΜΥΡΝΙΩΤΑΚΗΣ
+  9: ΑΘΗΝΑ
+  11: '254'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9602990732'
+- 0: 17452
+  1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  2: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
+  4: 808.899ΒΕΡ
+  5: '22861'
+  6: ΔΗΜΗΤΡΗΣ ΚΑΡΑΔΗΜΑΣ
+  8: ΜΙΝΩΑΣ
+  9: ΑΘΗΝΑ
+  11: '251'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9786180201'
+  19: '888'
+- 0: 17453
+  1: ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
+  2: ΠΑΡΑΜΥΘΙ ΧΩΡΙΣ ΟΝΟΜΑ
+  4: 808.899ΔΕΛ
+  5: '22862'
+  8: ΜΙΝΩΑΣ
+  9: ΑΘΗΝΑ
+  10: '2014'
+  11: '231'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789604816'
+  19: '439'
+- 0: 17454
+  1: DOYLE,ARTHUR,CONAN
+  2: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΣΕΡΛΟΚ ΧΟΛΜΣ
+  4: 808.899DOY
+  5: '22863'
+  6: ΑΡΓΥΡΩ ΠΙΠΙΝΗ
+  8: ΠΑΠΑΔΟΠΟΥΛΟΣ
+  9: ΑΘΗΝΑ
+  10: '2005'
+  11: '109'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9604124242'
+- 0: 17455
+  1: ROWLING,J.K.
+  2: HARRY POTTER AND THE PHILOSOPHER'S STONE
+  4: 808.899ROW
+  5: '22865'
+  8: BLOOMSBURY
+  9: LONDON
+  10: '2014'
+  11: '332'
+  12: ΞΕΝΟΓΛΩΣΣΟ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΞΕΝΟΓΛΩΣΣΟ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΞΕΝΟΓΛΩΣΣΟ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9781488556'
+  19: '52'
+- 0: 17456
+  1: BLYTON,ENID
+  2: ΟΙ ΠΕΝΤΕ ΦΙΛΟΙ ΠΑΛΙ ΣΤΟ ΝΗΣΙ ΤΟΥ ΚΙΡΡΙΝ
+  4: 808.899BLY
+  5: '22842'
+  6: ΜΑΡΙΑ ΑΥΓΕΡΟΥ
+  8: GUTENBERG
+  9: ΑΘΗΝΑ
+  10: '1984'
+  11: '165'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17457
+  1: BLYTON,ENID
+  2: ΟΙ ΠΕΝΤΕ ΦΙΛΟΙ ΠΕΦΤΟΥΝ ΣΕ ΠΕΡΙΠΕΤΕΙΑ
+  4: 808.899BLY
+  5: '22843'
+  6: ΜΑΡΙΑ ΑΥΓΕΡΟΥ
+  8: GUTENBERG
+  9: ΑΘΗΝΑ
+  10: '1985'
+  11: '183'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17458
+  1: BLYTON,ENID
+  2: ΟΙ ΜΥΣΤΙΚΟΙ 7 ΣΤΗΝ ΠΕΡΙΠΕΤΕΙΑ ΤΟΥ ΚΕΡΥ ΜΠΛΟΥ
+  4: 808.899BLY
+  5: '22846'
+  6: ΜΑΡΙΑ ΤΣΑΟΥΣΗ
+  8: GUTENBERG
+  9: ΑΘΗΝΑ
+  10: '2012'
+  11: '106'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789600115'
+  19: 079
+- 0: 17459
+  1: ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+  2: ΣΩΣΤΕ ΤΟΝ ΣΚΑΜΠΕΡΜΥΣΤΙΚΟΙ ΕΦΤΑ
+  4: 808.899ΜΠΛ
+  5: '22845'
+  6: ΑΛΕΞΑΝΔΡΑ ΒΑΣΙΛΕΙΟΥ
+  8: GUTENBERG
+  9: ΑΘΗΝΑ
+  10: '1985'
+  11: 134Σ
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17460
+  1: ΜΠΛΑΙΤΟΝ,ΕΝΙΝΤ
+  2: ΟΙ ΜΥΣΤΙΚΟΙ ΕΦΤΑ ΣΕ ΜΙΑ ΔΙΑΣΚΕΔΑΣΤΙΚΗ ΠΕΡΙΠΕΤΕΙΑ
+  4: 808.899ΜΠΛ
+  5: '22844'
+  6: ΑΛΕΞΑΝΔΡΑ ΒΑΣΙΛΕΙΟΥ
+  8: GUTENBERG
+  9: ΑΘΗΝΑ
+  10: '1985'
+  11: '114'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17461
+  1: Χ.Σ
+  2: Η ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΓΙΑ ΤΟ ΔΗΜΟΤΙΚΟ
+  4: 808.899Χ.Σ
+  5: '22869'
+  6: ΜΠΕΣΣΥ ΠΛΑΚΟΥΛΑ
+  8: MODREN TIMES
+  9: ΑΘΗΝΑ
+  10: '2004'
+  11: '174'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17462
+  1: BOURNIER,ISABELLE
+  2: ΤΟ ΜΕΓΑΛΟ ΒΙΒΛΙΟ ΓΙΑ ΤΗΝ ΕΙΡΗΝΗ
+  4: 808.899BOU
+  5: '22870'
+  6: ΜΑΡΙΑ ΜΠΑΣΤΑ
+  8: ΕΡΕΥΝΗΤΕΣ
+  9: ΑΘΗΝΑ
+  10: '2008'
+  11: '94'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789603684'
+  19: '206'
+- 0: 17463
+  1: Χ.Σ.
+  2: Η ΓΗ
+  4: 808.899Χ.Σ
+  5: '22868'
+  6: ΣΩΤΗΡΙΑ ΟΡΦΑΝΙΔΟΥ
+  8: ΣΑΒΒΑΛΑΣ
+  9: ΑΘΗΝΑ
+  10: '2005'
+  11: '79'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17464
+  1: Χ.Σ
+  2: ΑΦΡΙΚΗ 1
+  4: 808.899Χ.Σ
+  5: '22866'
+  8: DE AGOSTINI
+  9: ΑΘΗΝΑ
+  10: '2008'
+  11: '57'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789604166'
+  19: '312'
+- 0: 17465
+  1: Χ.Σ.
+  2: ΚΛΑΣΣΙΚΑ ΕΙΚΟΝΟΓΡΑΦΗΜΕΝΑ
+  4: 808.899Χ.Σ
+  5: '22871'
+  8: ΑΤΛΑΝΤΙΣ
+  9: ΑΘΗΝΑ
+  11: '360'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  30: ΤΟΜΟΙ 3 - 4
+- 0: 17466
+  1: DOOLEY,JENNY
+  2: EXCALIBUR- ACTIVITY BOOK
+  4: 808.899DOO
+  5: '22872'
+  8: EXPRESS PUBLISHING
+  9: ENGLAND
+  10: '2006'
+  11: '47'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΞΕΝΟΓΛΩΣΣΟ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΞΕΝΟΓΛΩΣΣΟ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΞΕΝΟΓΛΩΣΣΟ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+- 0: 17467
+  1: Χ.Σ.
+  2: FILOMATHIX
+  3: ΕΠΙΣΤΗΜΕΣ ΤΗΣ ΓΗΣ
+  4: 808.899Χ.Σ
+  5: '22867'
+  8: ΠΕΔΙΟ
+  9: ΑΘΗΝΑ
+  10: '2009'
+  11: '56'
+  12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  17: ΔΩΡΕΑ ΖΩΗ ΜΠΑΝΤΑΛΟΥΚΑ
+  18: '9789604750'
+  19: '887'
+- 0: 17468
+  1: Χ.Σ
+  2: ΕΛΛΑΔΑ ΙΣΤΟΡΙΑ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ
+  3: ΤΟ ΝΕΟ ΕΛΛΗΝΙΚΟ ΚΡΑΤΟΣ Η ΟΙΚΟΝΟΜΙΑ
+  4: 938Χ.Σ
+  5: '10666'
+  8: ΜΑΛΛΙΑΡΗΣ
+  9: ΑΘΗΝΑ
+  10: '1982'
+  11: '506'
+  12: ΙΣΤΟΡΙΑ-ΠΟΛΙΤΙΣΜΟΣ
+  13: ΕΛΛΑΔΑ
+  14: ΙΣΤΟΡΙΑ
+  15: ΠΟΛΙΤΙΣΜΟΣ
+  17: ΤΟΜΟΣ 8
+  18: '9602392290'
+- 0: 17469
+  1: ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  2: ΔΗΜΟΣΘΕΝΟΥΣ ΠΡΟΣ ΠΟΛΥΚΛΕΑ ΠΕΡΙ ΤΟΥ ΕΠΙΤΡΙΗΡΑΡΧΗΜΑΤΟΣ
+  3: Η ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ ΚΑΤΑ ΤΟΝ 4ΟΝ ΑΙΩΝΑ Π.Χ
+  4: 938.02ΒΕΤ
+  5: '22873'
+  9: ΘΕΣ/ΝΙΚΗ
+  10: '2022'
+  11: '54'
+  12: ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ
+  13: ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ
+  14: ΑΘΗΝΑ
+  18: '960920130'
+- 0: 17470
+  1: DROYSEN,JOHANN-GUSTAV
+  2: ΙΣΤΟΡΙΑ ΤΩΝ ΔΙΑΔΟΧΩΝ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+  4: 938.18DRO
+  5: '21528'
+  8: ΕΛΕΥΘΕΡΟΤΥΠΙΑ
+  9: ΑΘΗΝΑ
+  10: '1993'
+  11: '325'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+  14: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
+  17: 2 ΤΟΜΟΙ
+- 0: 17471
+  1: ΜΕΤΑΛΛΗΝΟΥ,ΓΕΩΡΓΙΟΥ
+  2: ΤΟΥΡΚΟΚΡΑΤΙΑ
+  3: ΟΙ ΕΛΛΗΝΕΣ ΣΤΗΝ ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
+  4: 938.4ΜΕΤ
+  5: '21576'
+  8: ΑΚΡΙΤΑΣ
+  9: ΑΘΗΝΑ
+  10: '1998'
+  11: 268Σ
+  12: ΙΣΤΟΡΙΑ-ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ
+  18: '9607006062'
+- 0: 17472
+  1: MOSSE,C.
+  2: ΤΟ ΤΕΛΟΣ ΤΗΣ ΑΘΗΝΑΙΚΗΣ ΔΗΜΟΚΡΑΤΙΑΣ
+  4: 938MOS
+  5: '17207'
+  6: Γ.Κ. ΒΛΑΧΟΥ
+  8: ΠΑΠΑΖΗΣΗ
+  9: ΑΘΗΝΑ
+  10: '1978'
+  11: '639'
+  12: ΙΣΤΟΡΙΑ-ΑΘΗΝΑΙΚΗ ΔΗΜΟΚΡΑΤΙΑ
+  13: ΑΘΗΝΑΙΚΗ ΔΗΜΟΚΡΑΤΙΑ
+  14: ΙΣΤΟΡΙΑ
+- 0: 17473
+  1: DROYSEN,JOHANN-GUSTAV
+  2: ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+  4: 938.174DRO
+  5: '22874'
+  8: ΕΛΕΥΘΕΡΟΤΥΠΙΑ
+  9: ΑΘΗΝΑ
+  10: '1993'
+  11: '390'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
+  14: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
+  17: ΤΟΜΟΙ 1-2.
+- 0: 17474
+  1: ΠΛΟΥΜΙΔΗΣ,ΓΕΩΡΓΙΟΣ
+  2: ΚΑΝΟΝΙΣΜΟΙ ΤΗΣ ΝΗΣΟΥ ΚΥΠΡΟΥ (1507-1522)
+  4: 938.497ΠΛΟ
+  5: '7789'
+  9: ΙΩΑΝΝΙΝΑ
+  10: '1987'
+  11: '90'
+  12: ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
+  13: ΚΥΠΡΟΣ-ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  15: ΚΥΠΡΟΣ
+- 0: 17475
+  1: ΝΙΑΡΧΟΣ,Θ.
+  2: ΚΥΠΡΟΣ ΝΗΣΙ ΤΟΥ ΠΑΘΟΥΣ ΚΑΙ ΤΩΝ ΜΑΡΤΥΡΙΩΝ
+  4: 938.497ΝΙΑ
+  5: '21225'
+  8: ΛΑΜΠΡΑΚΗΣ
+  9: ΑΘΗΝΑ
+  10: '2013'
+  11: '187'
+  12: ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
+  13: ΚΥΠΡΟΣ-ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  15: ΚΥΠΡΟΣ
+  18: '9789605033'
+  19: '958'
+- 0: 17476
+  1: Χ.Σ.
+  2: Η ΠΡΩΤΗ ΝΙΚΗ 1940-1941
+  4: 949.507Χ.Σ
+  5: '12668'
+  8: NATIONAL GEOGRAPHIC
+  9: ΑΘΗΝΑ
+  11: '158'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  18: '9789604880'
+  19: '935'
+- 0: 17477
+  1: Χ.Σ.
+  2: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ ΠΑΙΔΕΙΑ
+  4: 039.89ΜΑΛ
+  5: '22882'
+  8: ΜΑΛΛΙΑΡΗΣ
+  9: ΑΘΗΝΑ
+  10: '1976'
+  11: '200'
+  12: ΕΓΚΥΚΛΟΑΠΙΔΕΙΑ
+  13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
+  14: ΕΓΚΥΚΛΟΑΠΙΔΕΙΑ
+  17: ΤΟΜΟΙ 20
+- 0: 17478
+  1: ΧΡΙΣΤΟΔΟΥΛΟΥ,ΑΝΑΣΤΑΣΙΑ
+  2: ΠΑΙΔΕΙΑ, ΕΚΠΑΙΔΕΥΣΗ, ΑΞΙΕΣ
+  3: ΣΗΜΕΙΩΤΙΚΗ ΠΡΟΣΕΓΓΙΣΗ
+  4: 302.2ΧΡΙ
+  5: '22884'
+  8: UNIVERSITY STUDIO PR
+  9: ΘΕΣ/ΝΙΚΗ
+  10: '2012'
+  11: '145'
+  12: ΕΚΠΑΙΔΕΥΣΗ-ΠΑΙΔΕΙΑ
+  13: ΠΑΙΔΕΙΑ-ΕΚΠΑΙΔΕΥΣΗ
+  14: ΕΚΠΑΙΔΕΥΣΗ
+  15: ΠΑΙΔΕΙΑ
+  17: ΔΩΡΕΑ ΕΛΠΙΔΟΦΟΡΟΥ ΙΝΤΖΕΜΠΕΛΗ
+  18: '9789601221'
+  19: '281'
+- 0: 17479
+  1: ΤΖΙΜΑΣ,ΔΗΜΗΤΡΗΣ
+  2: ΤΟ ΝΕΟΧΩΡΑΚΙ ΑΡΤΑΣ
+  4: 938.939ΤΖΙ
+  5: '22883'
+  9: ΑΡΤΑ
+  11: '239'
+  12: ΙΣΤΟΡΙΑ-ΝΕΟΧΩΡΑΚΙ ΑΡΤΑ
+  13: ΑΡΤΑ
+  14: ΙΣΤΟΡΙΑ
+  15: ΝΕΟΧΩΡΑΚΙΑ ΑΡΤΑΣ
+  17: ΔΩΡΕΑ ΕΛΠΙΔΟΦΟΡΟΥ ΙΝΤΖΕΜΠΕΛΗ
+  18: '9789609313'
+  19: '308'
+- 0: 17480
+  1: ΣΑΡΡΗΓΙΑΝΝΙΔΗΣ,ΚΩΝ.
+  2: Ο ΠΟΝΤΟΣ 28 ΑΙΩΝΕΣ ΔΟΞΗΣ ΚΑΙ ΘΡΥΛΟΥ
+  4: 938ΣΑΡ
+  5: '20915'
+  11: 93Σ
+  12: ΠΟΝΤΟΣ-ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+  14: ΠΟΝΤΟΣ
+  15: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
+- 0: 17481
+  1: ΘΕΟΔΩΡΙΔΗΣ,ΚΩΣΤΑΣ
+  2: ΜΝΗΜΕΣ ΠΟΥ ΑΝΤΙΣΤΕΚΟΝΤΑΙ ...
+  4: 938.498ΘΕΟ
+  5: '20393'
+  8: ΚΥΡΙΑΚΙΔΗΣ
+  9: ΘΕΣ/ΝΙΚΗ
+  10: '2019'
+  11: '606'
+  12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+  13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+  14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
+  18: '9789605992'
+  19: '835'
+- 0: 17482
+  1: ΚΑΛΑΜΒΡΕΖΟΣ,ΔΙΟΝΥΣΙΟΣ
+  2: Ο ΕΛΛΗΝΙΣΜΟΣ ΣΤΗ ΡΩΣΙΑ ΚΑΙ ΣΤΙΣ ΑΛΛΕΣ ΧΩΡΕΣ ΤΗΣ Τ. ΕΣΣΔ
+  4: 938.498ΚΑΛ
+  5: '20399'
+  8: ΠΑΠΑΖΗΣΗ
+  9: ΑΘΗΝΑ
+  10: '2017'
+  11: '909'
+  12: ΔΙΕΘΝΗ ΠΟΛΙΤΙΚΗ
+  13: ΔΙΕΘΝΗ ΠΟΛΙΤΙΚΗ
+  14: ΔΙΕΘΝΗ ΠΟΛΙΤΙΚΗ
+  17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
+  18: '9789600232'
+  19: '912'
+- 0: 17483
+  1: Χ.Σ.
+  2: ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ
+  3: 8ΟΣ ΑΙΩΝΑΣ Π.Χ -1922
+  4: 938.497Χ.Σ
+  5: 12667-15039
+  8: ΤΕΣΣΕΡΑ ΠΙ
+  9: ΑΘΗΝΑ
+  10: '2012'
+  11: '126'
+  12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+  13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+  14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
+- 0: 17484
+  1: ΣΠΥΡΟΜΙΛΙΟΥ,ΜΙΛΤΟΥ
+  2: ΕΛΛΑΣ ΚΑΙ ΑΛΒΑΝΙΑ Ο ΓΚΙΟΛΕΚΑΣ
+  4: 941.2ΣΠΥ
+  5: '22898'
+  8: Ν. ΚΟΥΒΑΡΑ
+  9: ΑΘΗΝΑ
+  10: '1966'
+  11: '107'
+  12: ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΙΣΤΟΡΙΑ
+  13: ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΙΣΤΟΡΙΑ
+  14: ΕΛΛΗΝΟΑΛΒΑΝΙΚΗ ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ.ΒΕΤΣΙΟΣ
+- 0: 17485
+  1: ΚΟΥΚΚΟΥ,ΕΛΕΝΗ
+  2: ΙΣΤΟΡΙΑ ΤΩΝ ΕΠΤΑΝΗΣΩΝ
+  4: 938.481ΚΟΥ
+  5: '22899'
+  8: ΠΑΠΑΔΗΜΑ
+  9: ΑΘΗΝΑ
+  10: '1999'
+  11: '250'
+  12: ΙΣΤΟΡΙΑ - ΕΠΤΑΝΗΣΑ
+  13: ΙΣΤΟΡΙΑ - ΕΠΤΑΝΗΣΑ
+  14: ΙΣΤΟΡΙΑ - ΕΠΤΑΝΗΣΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17486
+  1: ΚΑΡΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ
+  2: ΕΙΣΑΓΩΓΗ ΣΤΗΝ ΤΕΧΝΙΚΗ ΤΗΣ ΕΠΙΣΤΗΜΟΝΙΚΗΣ ΙΣΤΟΡΙΚΗΣ ΕΡΓΑΣΙΑΣ
+  4: 907.2ΚΑΡ
+  8: ΒΑΝΙΑΣ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1988'
+  11: '110'
+  12: ΕΠΙΣΤΗΜΟΝΙΚΕΣ ΕΡΓΑΣΙΕΣ
+  13: ΕΠΙΣΤΗΜΟΝΙΚΕΣ ΕΡΓΑΣΙΕΣ
+  14: ΕΠΙΣΤΗΜΟΝΙΚΕΣ ΕΡΓΑΣΙΕΣ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17487
+  1: ΣΤΑΛΙΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  2: ΟΙ ΣΥΝΤΕΧΝΙΕΣ ΚΑΙ ΤΑ ΕΠΑΓΓΕΛΜΑΤΑ ΣΤΗΝ ΕΔΕΣΣΑ
+  4: 938.492ΣΤΑ
+  5: '22897'
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1999'
+  11: '240'
+  12: ΙΣΤΟΡΙΑ - ΕΠΑΓΓΕΛΜΑΤΑ
+  13: ΙΣΤΟΡΙΑ - ΕΠΑΓΓΕΛΜΑΤΑ
+  14: ΙΣΤΟΡΙΑ - ΕΠΑΓΓΕΛΜΑΤΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17488
+  1: ΑΣΔΡΑΧΑΣ,ΣΠΥΡΟΣ
+  2: ΟΙΚΟΝΟΜΙΑ ΚΑΙ ΝΟΟΤΡΟΠΙΕΣ
+  4: 949.505ΑΣΔ
+  5: '22907'
+  8: ΕΡΜΗΣ
+  9: ΑΘΗΝΑ
+  10: '1988'
+  11: '260'
+  12: ΙΣΤΟΡΙΑ-ΟΙΚΟΝΟΜΙΑ
+  13: ΙΣΤΟΡΙΑ-ΟΙΚΟΝΟΜΙΑ
+  14: ΙΣΤΟΡΙΑ-ΟΙΚΟΝΟΜΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17489
+  1: ΠΑΠΑΓΙΑΝΝΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
+  2: ΡΩΣΣΑΓΓΛΟΓΑΛΛΟΣ
+  4: 949.505ΠΑΠ
+  5: '22910'
+  8: ΡΕΚΟΣ
+  11: '200'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17490
+  1: ΔΡΟΥΛΙΑ,ΛΟΥΚΙΑ
+  2: ΠΡΟΣΕΓΓΙΣΕΙΣ ΣΤΙΣ ΝΟΟΤΡΟΠΙΕΣ ΤΩΝ ΒΑΛΚΑΝΙΚΩΝ ΛΑΩΝ
+  4: 949.6ΔΡΟ
+  5: '22909'
+  8: Ι.ΖΑΧΑΡΟΠΟΥΛΟΣ
+  9: ΑΘΗΝΑ
+  10: '1988'
+  11: '170'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17491
+  1: ΔΡΟΥΛΙΑ,ΛΟΥΚΙΑ
+  2: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ
+  4: 910.9ΔΡΟ
+  5: '22908'
+  9: ΑΘΗΝΑ
+  10: '1993'
+  11: '550'
+  12: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ-ΒΑΛΚΑΝΙΑ
+  13: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ-ΒΑΛΚΑΝΙΑ
+  14: ΠΕΡΙΗΓΗΤΙΚΑ ΘΕΜΑΤΑ-ΒΑΛΚΑΝΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17492
+  1: ΣΥΓΚΕΛΟΥ,ΕΥΣΤΡΑΤΙΑ
+  2: Ο ΠΟΛΕΜΟΣ ΣΤΟΝ ΔΥΤΙΚΟ ΕΛΛΑΔΙΚΟ ΧΩΡΟ ΚΑΤΑ ΤΟΝ ΔΕΥΤΕΡΟ ΜΕΣΑΙΩΝ
+  3: Α
+  4: 938.375ΣΥΓ
+  5: '22906'
+  9: ΑΘΗΝΑ
+  10: '2008'
+  11: '450'
+  12: ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
+  13: ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
+  14: ΙΣΤΟΡΙΑ-ΠΟΛΕΜΟΣ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17493
+  1: NICOL,DONALD
+  2: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
+  4: 938.375NIC
+  5: '22905'
+  8: ΕΛΛΗΝΙΚΗ ΕΥΕΩΕΚΔΟΤΙΚ
+  9: ΑΘΗΝΑ
+  10: '1991'
+  11: '380'
+  12: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
+  13: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
+  14: ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17494
+  1: ΑΝΤΩΝΙΑΔΗΣ,ΞΕΝΟΦΩΝ
+  2: Η ΣΚΥΡΟΣ ΣΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑ
+  4: 938.495ΑΝΤ
+  5: '22904'
+  9: ΑΘΗΝΑ
+  10: '1997'
+  11: '341'
+  12: ΙΣΤΟΡΙΑ-ΣΚΥΡΟΣ
+  13: ΙΣΤΟΡΙΑ-ΣΚΥΡΟΣ
+  14: ΙΣΤΟΡΙΑ-ΣΚΥΡΟΣ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17495
+  1: ΣΙΑΤΡΑΣ,ΔΗΜΗΤΡΗΣ
+  2: ΟΙ ΑΓΟΡΑΠΩΛΗΣΙΕΣ ΑΚΙΝΗΤΩΝ ΣΤΗΝ ΤΟΥΡΚΟΚΡΑΤΟΥΜΕΝΗ ΕΛΛΑΔΑ
+  4: 938.76ΣΙΑ
+  5: '22903'
+  8: ΓΝΩΣΗ
+  9: ΑΘΗΝΑ
+  10: '1992'
+  11: '275'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17496
+  1: ΤΣΙΡΠΑΝΛΗΣ,ΖΑΧΑΡΙΑΣ
+  2: ΕΙΣΑΓΩΓΗ ΣΤΗ ΜΕΣΑΙΩΝΙΚΗ ΙΣΤΟΡΙΑ ΤΗΣ ΔΥΤΙΚΗΣ ΕΥΡΩΠΗΣ
+  4: 940.1ΤΣΙ
+  5: '22902'
+  8: ΖΗΤΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1996'
+  11: '325'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17497
+  1: HERING-ΚΑΤΣΙΑΡΔΗ,ΟΛΓΑ
+  2: ΤΕΧΝΙΤΕΣ ΚΑΙ ΤΕΧΝΙΚΕΣ ΒΑΦΗΣ ΝΗΜΑΤΩΝ
+  4: 677.009HER
+  5: '22901'
+  8: ΗΡΟΔΟΤΟΣ
+  11: '381'
+  12: ΥΦΑΝΤΟΥΡΓΙΑ-ΧΡΩΜΑΤΑ-ΒΑΦΕΣ
+  13: ΥΦΑΝΤΟΥΡΓΙΑ-ΧΡΩΜΑΤΑ-ΒΑΦΕΣ
+  14: ΘΕΣΣΑΛΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17498
+  1: ΚΥΡΙΑΚΟΥ,ΑΡΤΕΜΗ
+  2: Η ΕΛΛΗΝΙΚΗ ΚΟΙΝΟΤΗΤΑ ΤΗΣ ΒΕΝΕΤΙΑΣ
+  4: 938.499ΚΥΡ
+  5: '22896'
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1978'
+  11: '300'
+  12: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΚΟΙΝΟΤΗΤΑ
+  13: ΕΛΛΗΝΙΚΗ ΚΟΙΝΟΤΗΤΑ-ΒΕΝΕΤΙΑ
+  14: ΔΙΔΑΚΤΟΡΙΚΗ ΔΙΑΤΡΙΒΗ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17499
+  1: ΚΑΡΑΓΕΩΡΓΑΚΗ,ΜΑΡΙΑ
+  2: ΣΥΓΧΡΟΝΕΣ ΜΕΘΟΔΟΛΟΓΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ ΣΤΗ ΔΙΔΑΣΚΑΛΙΑ ΤΗΣ ΙΣΤΟ
+  3: ΡΙΑΣ
+  4: 907ΚΑΡ
+  5: '22888'
+  8: ΚΥΡΙΑΚΙΔΗ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2007'
+  11: '370'
+  12: ΔΙΔΑΣΚΑΚΙΑ ΤΗΣ ΙΣΤΟΡΙΑΣ
+  13: ΙΣΤΟΡΙΑ
+  14: ΘΕΜΑΤΑ ΙΣΤΟΡΙΚΑ- ΔΙΔΑΣΚΑΛΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17500
+  1: ΓΛΑΒΙΝΑ,ΑΠΟΣΤΟΛΟΥ
+  2: ΕΓΓΡΑΦΑ ΠΕΡΙ ΤΗΣ ΠΡΑΞΙΚΟΠΗΜΑΤΙΚΗΣ ΣΥΓΚΡΟΤΗΣΕΩΣ ΤΗΣ ΣΥΝΟΔΟΥ Τ
+  3: ΗΣ ΟΡΘΟΔΟΞΟΥ ΕΚΚΛΗΣΙΑΣ ΤΗΣ ΑΛΒΑΝΙΑΣ
+  4: 281.949ΓΛΑ
+  5: '22895'
+  8: ΙΜΙΑΧ
+  9: ΙΩΑΝΝΙΝΑ
+  10: '1981'
+  11: '80'
+  12: ΕΚΚΛΗΣΙΑ-ΑΛΒΑΝΙΑ
+  13: ΑΛΒΑΝΙΑ-ΕΚΚΛΗΣΙΑ
+  14: ΕΚΚΛΗΣΙΑ ΑΛΒΑΝΙΑΣ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17501
+  1: ΕΝΕΠΕΚΙΔΗΣ,Π.Κ.
+  2: ΜΑΚΕΔΟΝΙΚΕΣ ΠΟΛΕΙΣ ΚΑΙ ΟΙΚΟΓΕΝΕΙΕΣ 1750-1930
+  4: 914.95ΕΝΕ
+  5: '22894'
+  8: ΒΙΒΛΟΠΩΛΕΙΟΝ ΕΣΤΙΑΣ
+  9: ΑΘΗΝΑ
+  10: '1984'
+  11: '324'
+  12: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
+  13: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
+  14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17502
+  1: ΒΑΚΑΛΟΠΟΥΛΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  2: ΟΙΚΟΝΟΜΙΚΗ ΛΕΙΤΟΥΡΓΙΑ ΤΟΥ ΜΑΚΕΔΟΝΙΚΟΥ ΚΑΙ ΘΡΑΚΙΚΟΥ ΧΩΡΟΥ ΣΤΑ
+  3: ' ΜΕΣΑ ΤΟΥ 19ΟΥ ΑΙΩΝΑ ΣΤΑ ΠΛΑΙΣΙΑ ΤΟΥ ΔΙΕΘΝΟΥΣ ΕΜΠΟΡΙΟΥ'
+  4: 330.949ΒΑΚ
+  5: '22891'
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1980'
+  11: '215'
+  12: ΟΙΚΟΝΟΜΙΑ-ΙΣΤΟΡΙΑ
+  13: ΟΙΚΟΝΟΜΙΚΑ
+  14: ΟΙΚΟΝΟΜΙΚΑ ΘΕΜΑΤΑ ΜΑΚΕΔΟΝΙΑΣ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17503
+  1: ΛΙΑΤΑ,ΕΥΤΥΧΙΑ
+  2: ΑΡΓΕΙΑ ΓΗ
+  4: 938.921ΛΙΑ
+  5: '22893'
+  9: ΑΘΗΝΑ
+  10: '2003'
+  11: '140'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17504
+  1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΓΕΩΡΓΙΟΣ
+  2: ΟΙ ΣΥΝΤΕΧΝΙΕΣ ΣΤΑ ΓΙΑΝΝΕΝΑ ΚΑΤΑ ΤΟΝ 19ο ΚΑΙ ΤΙΣ ΑΡΧΕΣ ΤΟΥ 20
+  3: ου ΑΙΩΝΑ
+  4: 938.936ΠΑΠ
+  5: '22892'
+  8: ΙΜΙΑΧ
+  9: ΙΩΑΝΝΙΝΑ
+  10: '1988'
+  11: '363'
+  12: ΙΣΤΟΡΙΑ-ΓΙΑΝΝΕΝΑ
+  13: ΙΣΤΟΡΙΑ ΙΩΑΝΝΙΝΑ
+  14: ΙΣΤΟΡΙΚΑ ΤΩΝ ΙΩΑΝΝΙΝΩΝ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17505
+  1: ΚΟΝΤΟΓΙΑΝΝΗ,ΠΑΝΤΕΛΗ
+  2: ΟΙ ΕΛΛΗΝΕΣ
+  4: 938.471ΚΟΝ
+  5: '22890'
+  8: Π.Δ. ΣΑΚΕΛΛΑΡΙΟΥ
+  9: ΑΘΗΝΑ
+  11: '528'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17506
+  1: ΠΑΝΑΓΟΠΟΥΛΟΣ,ΑΓΓΕΛΙΚΗ
+  2: ΟΙ ΔΙΠΛΩΜΑΤΙΚΟΙ ΓΑΜΟΙ ΣΤΟ ΒΥΖΑΝΤΙΟ
+  4: 949.503ΠΑΝ
+  5: '22889'
+  8: Α.Α. ΛΙΒΑΝΗ
+  10: '2006'
+  11: '550'
+  12: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+  13: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+  14: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17507
+  1: ΣΒΟΡΩΝΟΣ,ΝΙΚΟΣ
+  2: ΕΠΙΣΚΟΠΗΣΗ ΤΗΣ ΝΕΟΕΛΛΗΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
+  4: 938.3ΣΒΟ
+  5: '22887'
+  8: ΘΕΜΕΛΙΟ
+  9: ΑΘΗΝΑ
+  10: '1985'
+  11: '339'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17508
+  1: MILLER,WILLIAM
+  2: Η ΦΡΑΓΚΟΚΡΑΤΙΑ ΣΤΗΝ ΕΛΛΑΔΑ 1204-1566
+  4: 938.37MIL
+  5: '22921'
+  8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
+  9: ΑΘΗΝΑ
+  10: '1997'
+  11: '742'
+  12: ΙΣΤΟΡΙΑ-ΦΡΑΓΚΟΚΡΑΤΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17509
+  1: ΚΡΕΜΜΥΔΑΣ,ΒΑΣΙΛΗΣ
+  2: ΕΛΛΗΝΙΚΗ ΝΑΥΤΙΛΙΑ 1776-1835
+  4: 387.51ΚΡΕ
+  5: '22913'
+  9: ΑΘΗΝΑ
+  10: '1985'
+  11: '155'
+  12: ΝΑΥΤΙΛΙΑ
+  13: ΕΛΛΗΝΙΚΗ ΝΑΥΤΙΛΙΑ
+  14: ΝΑΥΤΙΛΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17510
+  1: ΠΕΛΕΚΙΔΟΥ,ΜΑΡΙΑ
+  2: ΟΙ ΒΑΛΚΑΝΙΚΟΙ ΛΑΟΙ
+  4: 949.6ΠΕΛ
+  5: '22914'
+  8: ΒΑΝΙΑΣ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1991'
+  11: '380'
+  12: ΙΣΤΟΡΙΑ-ΒΑΛΚΑΝΙΑ
+  13: ΒΑΛΚΑΝΙΚΟΙ ΛΑΟΙ
+  14: ΒΑΛΚΑΝΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17511
+  1: ΛΙΑΤΑ,ΕΥΤΥΧΙΑ
+  2: Η ΣΕΡΙΦΟΣ ΚΑΤΑ ΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑ
+  4: 938.496ΛΙΑ
+  5: '22915'
+  9: ΑΘΗΝΑ
+  10: '1987'
+  11: '235'
+  12: ΙΣΤΟΡΙΑ-ΣΕΡΙΦΟΣ
+  13: ΙΣΤΟΡΙΑ-ΣΕΡΙΦΟΣ
+  14: ΙΣΤΟΡΙΑ-ΣΕΡΙΦΟΣ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17512
+  1: ΣΑΒΒΙΔΗΣ,ΑΛΕΞΙΟΣ
+  2: ΔΟΚΙΜΙΑ ΟΘΩΜΑΝΙΚΗΣ ΙΣΤΟΡΙΑΣ
+  4: 956.015ΣΑΒ
+  5: '22916'
+  8: ΠΑΠΑΖΗΣΗ
+  9: ΑΘΗΝΑ
+  10: '2004'
+  11: '300'
+  12: ΙΣΤΟΡΙΑ
+  13: ΟΘΩΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
+  14: ΔΟΚΙΜΙΑ ΙΣΤΟΡΙΚΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17513
+  1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΓΕΩΡΓΙΟΣ
+  2: Ο ΕΚΣΥΧΡΟΝΙΣΜΟΣ ΤΟΥ ΕΛΛΗΝΑ ΠΡΑΓΜΑΤΕΥΤΗ ΣΥΜΦΩΝΑ ΜΕ ΤΑ ΕΥΡΩΠΑΙ
+  3: ΚΑ ΠΡΟΤΥΠΑ
+  4: 938.501ΠΑΠ
+  5: '22917'
+  8: ΑΦΟΙ ΤΟΛΙΔΗ
+  9: ΑΘΗΝΑ
+  11: '201'
+  12: ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17514
+  1: ΤΣΙΛΗ,ΓΕΩΡΓΙΟΥ
+  2: ΣΟΥΛΙ-ΚΑΤΑΓΩΓΗ ΣΟΥΛΙΩΤΩΝ
+  4: 938.478ΤΣΙ
+  5: '22918'
+  8: APIROS HORA
+  9: ΑΘΗΝΑ
+  10: '2008'
+  11: '193'
+  12: ΙΣΤΟΡΙΑ-ΣΟΥΛΙ
+  13: ΙΣΤΟΡΙΚΑ ΣΟΥΛΙΩΤΩΝ
+  14: ΙΣΤΟΡΙΑ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17515
+  1: ΠΛΑΚΟΓΙΑΝΝΑΚΗΣ,ΚΙΜΩΝ-ΕΜΜΑΝΟΥΗΛ
+  2: ΤΙΜΗΤΙΚΟΙ ΤΙΤΛΟΙ ΚΑΙ ΕΝΕΡΓΑ ΑΞΙΩΜΑΤΑ ΣΤΟ ΒΥΖΑΝΤΙΟ
+  4: 938.3ΠΛΑ
+  5: '22919'
+  8: ΙΑΝΟΣ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2001'
+  11: '400'
+  12: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+  13: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+  14: ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17516
+  1: ΜΑΡΙΝΑΚΟΥ,ΕΛΕΝΗ
+  2: ΑΙ ΕΝ ΘΡΑΚΗ ΣΥΝΤΕΧΝΙΑΙ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΤΑ ΤΗΝ ΤΟΥΡΚΟΚΡΑΤΙΑΝ
+  4: 938.416ΜΑΡ
+  5: '22920'
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1950'
+  11: '202'
+  12: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
+  13: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
+  14: ΙΣΤΟΡΙΑ-ΘΡΑΚΗ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17517
+  1: Χ.Σ
+  2: ΕΩΑ ΚΑΙ ΕΣΠΕΡΙΑ
+  4: 025Χ.Σ
+  5: '22932'
+  9: ΑΘΗΝΑ
+  10: '2006'
+  11: '310'
+  12: ΠΕΡΙΟΔΙΚΟ
+  13: ΠΕΡΙΟΔΙΚΟ
+  14: ΠΕΡΙΟΔΙΚΟ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ 1-6
+- 0: 17518
+  1: Χ.Σ
+  2: Ο ΕΡΑΝΙΣΤΗΣ
+  4: 025Χ.Σ
+  5: '22933'
+  9: ΑΘΗΝΑ
+  10: '1993'
+  11: '380'
+  12: ΠΕΡΙΟΔΙΚΟ
+  13: ΠΕΡΙΟΔΙΚΟ
+  14: ΠΕΡΙΟΔΙΚΟ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17519
+  1: Χ.Σ
+  2: ΤΕΤΡΑΔΙΑ ΕΡΓΑΣΙΑΣ
+  4: 025Χ.Σ
+  5: '22934'
+  9: ΑΘΗΝΑ
+  10: '2004'
+  11: '370'
+  12: ΠΕΡΙΟΔΙΚΟ
+  13: ΠΕΡΙΟΔΙΚΟ
+  14: ΠΕΡΙΟΔΙΚΟ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ 1-5
+- 0: 17520
+  1: Χ.Σ
+  2: Ζ ΠΑΝΙΟΝΙΟ ΣΥΝΕΔΡΙΟ - ΠΡΑΚΤΙΚΑ
+  4: 938.26Χ.Σ
+  5: '22923'
+  9: ΑΘΗΝΑ
+  10: '2004'
+  11: '760'
+  12: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  13: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  14: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ Α ΚΑΙ Β
+- 0: 17521
+  1: Χ.Σ
+  2: ΣΤ ΔΙΕΘΝΕΣ ΠΑΝΙΟΝΙΟ ΣΥΝΕΔΡΙΟ - ΠΡΑΚΤΙΚΑ
+  4: 938.26Χ.Σ
+  5: '22922'
+  9: ΑΘΗΝΑ
+  10: '2001'
+  11: '662'
+  12: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  13: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  14: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ
+- 0: 17522
+  1: Χ.Σ
+  2: Β ΔΙΕΘΝΕΣ ΙΣΤΟΡΙΚΟ ΚΑΙ ΑΡΧΑΙΟΛΟΓΙΚΟ ΣΥΝΕΔΡΙΟ ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ
+  4: 938.106Χ.Σ
+  5: '22912'
+  9: ΑΓΡΙΝΙΟ
+  10: '2004'
+  11: '1150'
+  12: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  13: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  14: ΠΡΑΚΤΙΚΑ ΣΥΝΕΔΡΙΟΥ
+  17: ΔΩΡΕΑ ΕΛ. ΒΕΤΣΙΟΣ - ΤΟΜΟΙ Α ΚΑΙ Β
+- 0: 17523
+  1: ΣΑΙΞΠΗΡ
+  2: ΟΝΕΙΡΟ ΚΑΛΟΚΑΙΡΙΝΗΣ ΝΥΧΤΑΣ
+  4: 822.33ΣΑΙ
+  5: '22926'
+  11: '30'
+  12: ΘΕΑΤΡΟ
+  13: ΘΕΑΤΡΟ
+  14: ΘΕΑΤΡΟ
+  17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗΣ
+- 0: 17524
+  1: ΙΨΕΝ
+  2: ΜΝΗΣΤΗΡΕΣ ΤΟΥ ΘΡΟΝΟΥ
+  4: 839.82ΙΨΕ
+  5: '22927'
+  8: ΔΩΔΩΝΗ
+  9: ΑΘΗΝΑ
+  10: '1975'
+  11: '192'
+  12: ΘΕΑΤΡΟ
+  13: ΘΕΑΤΡΟ
+  14: ΘΕΑΤΡΟ
+  17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+- 0: 17525
+  1: ΛΥΠΟΥΡΛΗΣ,ΔΗΜΗΤΡΙΟΣ
+  2: ΙΠΠΟΚΡΑΤΗΣ - ΙΑΤΡΙΚΗ ΔΕΟΝΤΟΛΟΓΙΑ ΚΑΙ ΝΟΣΟΛΟΓΙΑ
+  4: 887.3ΛΥΠ
+  5: '22928'
+  8: ΖΗΤΡΟΣ
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '2001'
+  11: '496'
+  12: ΑΡΧΑΙΟ ΚΕΙΜΕΝΟ
+  13: ΑΡΧΑΙΟ ΚΕΙΜΕΝΟ
+  14: ΑΡΧΑΙΟ ΚΕΙΜΕΝΟ
+  17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+- 0: 17526
+  1: ΚΟΛΛΑΤΟΥ,ΔΗΜΗΤΡΗ
+  2: Ο ΑΓΙΟΣ ΠΡΕΒΕΖΗΣ
+  4: 889.23ΚΟΛ
+  5: '22931'
+  8: ΠΕΜΠΤΗ ΕΠΟΧΗ
+  9: ΠΡΕΒΕΖΑ
+  11: '175'
+  12: ΘΕΑΤΡΟ
+  13: ΘΕΑΤΡΟ
+  14: ΘΕΑΤΡΟ
+  17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
+- 0: 17527
+  1: ΡΩΤΑ,ΒΑΣΙΛΗ
+  2: ΘΕΑΤΡΟ
+  4: 889.23ΡΩΤ
+  5: '22929'
+  8: ΙΚΑΡΟΣ
+  11: '285'
+  12: ΘΕΑΤΡΟ
+  13: ΘΕΑΤΡΟ
+  14: ΘΕΑΤΡΟ
+  17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ - 2 ΒΙΒΛΙΑ
+- 0: 17528
+  1: ΦΩΤΙΑΔΟΥ,ΜΑΡΙΑ
+  2: ΟΜΑΔΕΣ ΑΙΜΑΤΟΣ-RH-ΑΙΜΟΛΥΤΙΚΗ ΑΝΑΙΜΙΑ ΤΩΝ ΝΕΟΓΝΩΝ
+  4: 610.73ΦΩΤ0
+  5: '22930'
+  9: ΘΕΣΣΑΛΟΝΙΚ
+  10: '1980'
+  11: '38'
+  12: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
+  13: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
+  14: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
+  17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field04_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field04_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field05_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field05_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field06_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field06_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field07_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field07_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field08_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field08_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field09_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field09_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field16_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field16_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field17_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field17_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field18_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field18_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field19_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field19_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/field30_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/field30_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/first_names.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/first_names.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/topic_replacements.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/topic_replacements.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/data/translator_corrections.yml` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/data/translator_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/dbf_to_yaml.py` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/dbf_to_yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Convert dbf files to human readable yaml"""
+from __future__ import annotations
+
 import sys
 from collections import OrderedDict
 
 import dbfread
 import yaml
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/field_extractors.py` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/generate_reports.py` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/generate_reports.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 import os
 import pprint
 import shutil
 import sys
 from collections import defaultdict
 
 import yaml
-from snakemd import Document, InlineText, MDCheckList, MDList, Table
+from snakemd import Document, Inline, MDList, Table
 
 from skoufas_dbf_reader.correction_data import plain_author_re
 from skoufas_dbf_reader.field_extractors import *
 from skoufas_dbf_reader.utilities import all_entries, check_ean, check_isbn, check_issn, is_valid_dewey_strict, romanize
 
 
 def report_single_fields(reports_directory: str):
     field_values: list[set[str]] = [set() for _ in range(31)]
     os.makedirs(os.path.join(reports_directory, "single-field"), exist_ok=True)
     for entry in all_entries():
         for i in range(1, 31):
             if i in entry and entry[i] and entry[i].strip():
                 field_values[i].add(entry[i].strip())
     for i in range(1, 31):
-        doc = Document(f"Τιμές στη θέση {i:02}")
-        doc.add_header(f"Τιμές στη θέση {i:02}")
+        doc = Document()
+        doc.add_heading(f"Τιμές στη θέση {i:02}")
         doc.add_unordered_list([f"`{v}`" for v in sorted(field_values[i])])
         with open(
             os.path.join(reports_directory, "single-field", f"field_{i:02}.md"), "w", encoding="utf-8"
         ) as outfile:
             outfile.write(str(doc))
 
-    doc = Document("Τιμές στις στήλες των καρτελών")
-    doc.add_header("Τιμές στις στήλες των καρτελών")
-    doc.add_unordered_list([InlineText(f"Στήλη {i}", url=f"./field_{i:02}.html").render() for i in range(1, 31)])
+    doc = Document()
+    doc.add_heading("Τιμές στις στήλες των καρτελών")
+    doc.add_unordered_list([Inline(f"Στήλη {i}", link=f"./field_{i:02}.html") for i in range(1, 31)])
     with open(os.path.join(reports_directory, "single-field", "index.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(doc))
 
 
 def report_single_extracted_fields(reports_directory: str):
     field_values: defaultdict[str, list[str | list[str]]] = defaultdict(list)
     for entry in all_entries():
@@ -151,46 +151,44 @@
             if not check_issn(isbn):
                 field_values["issn"].append(isbn)
             if not check_ean(isbn):
                 field_values["ean"].append(isbn)
 
     os.makedirs(os.path.join(reports_directory, "calculated-field"), exist_ok=True)
 
-    index = Document("Υπολογισμένες Τιμές")
-    index.add_header("Υπολογισμένες Τιμές")
+    index = Document()
+    index.add_heading("Υπολογισμένες Τιμές")
     links: list[str] = []
 
     for k, values in field_values.items():
         values = [pprint.pformat(value) for value in values]
         with open(
             os.path.join(reports_directory, "calculated-field", f"calculated_field_{k}.md"), "w", encoding="utf-8"
         ) as outfile:
-            doc = Document(f"Υπολογισμένες τιμές για την ιδιότητα {k}")
-            doc.add_header(f"Υπολογισμένες τιμές για την ιδιότητα {k}, αλφαβητικά")
+            doc = Document()
+            doc.add_heading(f"Υπολογισμένες τιμές για την ιδιότητα {k}, αλφαβητικά")
             doc.add_unordered_list([f"`{v}`" for v in sorted(set(values))])
             outfile.write(str(doc))
             links.append(
-                InlineText(
-                    f"Υπολογισμένες τιμές για την ιδιότητα {k}, αλφαβητικά", url=f"./calculated_field_{k}.html"
-                ).render()
+                Inline(f"Υπολογισμένες τιμές για την ιδιότητα {k}, αλφαβητικά", link=f"./calculated_field_{k}.html")
             )
         with open(
             os.path.join(reports_directory, "calculated-field", f"calculated_field_{k}_romanize_sort.md"),
             "w",
             encoding="utf-8",
         ) as outfile:
-            doc = Document(f"Υπολογισμένες τιμές για την ιδιότητα {k}")
-            doc.add_header(f"Υπολογισμένες τιμές για την ιδιότητα {k}, φωνητικά")
+            doc = Document()
+            doc.add_heading(f"Υπολογισμένες τιμές για την ιδιότητα {k}, φωνητικά")
             doc.add_unordered_list([f"`{v}` # *{romanize(v)}*" for v in sorted(set(values), key=romanize)])
             outfile.write(str(doc))
             links.append(
-                InlineText(
+                Inline(
                     f"Υπολογισμένες τιμές για την ιδιότητα {k}, φωνητικά",
-                    url=f"./calculated_field_{k}_romanize_sort.html",
-                ).render()
+                    link=f"./calculated_field_{k}_romanize_sort.html",
+                )
             )
     index.add_unordered_list(links)
     with open(os.path.join(reports_directory, "calculated-field", "index.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(index))
 
 
 def report_invalid_dewey(reports_directory: str):
@@ -203,23 +201,23 @@
                 invalid_output_dewey[dewey].append(str(entry[0]))
         else:
             if none_if_empty_or_stripped(entry[4]):
                 no_output_dewey[entry[4]].append(str(entry[0]))
 
     os.makedirs(os.path.join(reports_directory, "checks"), exist_ok=True)
     with open(os.path.join(reports_directory, "checks", "invalid_dewey.md"), "w", encoding="utf-8") as outfile:
-        doc = Document("Dewey με προβληματικές τιμές")
-        doc.add_header("Dewey με προβληματικές τιμές στην έξοδο")
+        doc = Document()
+        doc.add_heading("Dewey με προβληματικές τιμές στην έξοδο")
         for k, v in sorted(invalid_output_dewey.items()):
-            doc.add_header(k, level=2)
-            doc.add_unordered_list([InlineText(entry, url=f"../entries/entry_{entry:05}.html").render() for entry in v])
-        doc.add_header("Dewey στην είσοδο που δεν βγαίνουν στην έξοδο")
+            doc.add_heading(k, level=2)
+            doc.add_unordered_list([Inline(entry, link=f"../entries/entry_{entry:05}.html") for entry in v])
+        doc.add_heading("Dewey στην είσοδο που δεν βγαίνουν στην έξοδο")
         for k, v in sorted(no_output_dewey.items()):
-            doc.add_header(k, level=2)
-            doc.add_unordered_list([InlineText(entry, url=f"../entries/entry_{entry:05}.html").render() for entry in v])
+            doc.add_heading(k, level=2)
+            doc.add_unordered_list([Inline(entry, link=f"../entries/entry_{entry:05}.html") for entry in v])
         outfile.write(str(doc))
 
 
 def report_translators(reports_directory: str):
     os.makedirs(os.path.join(reports_directory, "checks"), exist_ok=True)
     weird_translators: list[str] = []
     valid_translator_re = re.compile(r"[Α-Ω\-]+,[Α-Ω\.]*\.?")
@@ -227,16 +225,16 @@
         translator = translator_from_a06(entry[6])
         if translator:
             translators = translator.split("!!")
             for translator in translators:
                 if not valid_translator_re.fullmatch(translator):
                     weird_translators.append(translator)
     with open(os.path.join(reports_directory, "checks", "invalid_translators.md"), "w", encoding="utf-8") as outfile:
-        doc = Document("Μεταφραστές με παράξενα ονόματα")
-        doc.add_header("Μεταφραστές με παράξενα ονόματα")
+        doc = Document()
+        doc.add_heading("Μεταφραστές με παράξενα ονόματα")
         doc.add_unordered_list(sorted(weird_translators))
         outfile.write(str(doc))
 
 
 def report_donors(reports_directory: str):
     os.makedirs(os.path.join(reports_directory, "checks"), exist_ok=True)
     count_map: defaultdict[str, int] = defaultdict(int)
@@ -246,23 +244,23 @@
             for donor in donors.split("!!"):
                 count_map[donor] = count_map[donor] + 1
     donor_count_list: list[list[str]] = []
     for donor, count in sorted(count_map.items(), reverse=True, key=lambda x: x[1]):
         donor_count_list.append([donor, str(count)])
 
     with open(os.path.join(reports_directory, "checks", "donors.md"), "w", encoding="utf-8") as outfile:
-        doc = Document("Δωρητές")
-        doc.add_header("Δωρητές")
+        doc = Document()
+        doc.add_heading("Δωρητές")
         doc.add_table(["Δωρητής", "Αριθμός βιβλίων"], donor_count_list)
         outfile.write(str(doc))
 
 
 def report_isbns(reports_directory: str):
-    doc = Document("Προβληματικά ISBN")
-    doc.add_header("Προβληματικά ISBN")
+    doc = Document()
+    doc.add_heading("Προβληματικά ISBN")
     doc.add_table_of_contents()
 
     for entry in all_entries():
         result = isbn_from_a17_a18_a19_a22_a30(
             entry[17],
             entry[18],
             entry[19],
@@ -271,32 +269,32 @@
         )
         if not result:
             continue
         checks = [check_isbn(result), check_issn(result), check_ean(result)]
         if None in checks:
             continue
 
-        doc.add_header(result, level=2)
+        doc.add_heading(result, level=2)
         doc.add_unordered_list([check for check in checks if check])
 
-        doc.add_header("Αρχική Καρτέλα στο DBASE", level=3)
+        doc.add_heading("Αρχική Καρτέλα στο DBASE", level=3)
         doc.add_code(code=entry_as_yaml(entry, minimal=True), lang="yaml")
 
     with open(os.path.join(reports_directory, "checks", "invalid_isbn.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(doc))
 
 
 def report_entry_numbers(reports_directory: str):
     all_entry_numbers: dict[str, dict[int, str]] = dict()
 
-    no_entry_numbers = Document("Καρτέλες χωρίς αριθμό εισαγωγής")
-    no_entry_numbers.add_header("Καρτέλες χωρίς αριθμό εισαγωγής")
+    no_entry_numbers = Document()
+    no_entry_numbers.add_heading("Καρτέλες χωρίς αριθμό εισαγωγής")
 
-    non_numeric = Document("Καρτέλες με μή αριθμητικό αριθμό εισαγωγής")
-    non_numeric.add_header("Καρτέλες με μή αριθμητικό αριθμό εισαγωγής")
+    non_numeric = Document()
+    non_numeric.add_heading("Καρτέλες με μή αριθμητικό αριθμό εισαγωγής")
 
     duplicate_entry_numbers: defaultdict[str, list[dict[int, str]]] = defaultdict(list)
 
     for entry in all_entries():
         entry_numbers = entry_numbers_from_a04_a05_a06_a07_a08_a18_a19(
             entry[4], entry[5], entry[6], entry[7], entry[8], entry[18], entry[19]
         )
@@ -323,16 +321,16 @@
         os.path.join(reports_directory, "checks", "non_numeric_entry_numbers.md"), "w", encoding="utf-8"
     ) as outfile:
         outfile.write(str(non_numeric))
 
     with open(
         os.path.join(reports_directory, "checks", "duplicate_entry_numbers.md"), "w", encoding="utf-8"
     ) as outfile:
-        dup = Document("Καρτέλες με διπλοπερασμένο αριθμητικό αριθμό εισαγωγής")
-        dup.add_header("Καρτέλες με διπλοπερασμένο αριθμητικό αριθμό εισαγωγής")
+        dup = Document()
+        dup.add_heading("Καρτέλες με διπλοπερασμένο αριθμητικό αριθμό εισαγωγής")
         for entry_number, entries in duplicate_entry_numbers.items():
             dup.add_horizontal_rule()
             dup.add_paragraph(entry_number)
             for entry in entries:
                 dup.add_code(entry_as_yaml(entry, minimal=True), lang="yaml")
         outfile.write(str(dup))
 
@@ -398,24 +396,24 @@
             if not check_isbn(isbn_issn_ean):
                 isbn = isbn_issn_ean
             if not check_issn(isbn_issn_ean):
                 issn = isbn_issn_ean
             if not check_ean(isbn_issn_ean):
                 ean = isbn_issn_ean
 
-        doc = Document(f"entry_{entry[0]:05}")
+        doc = Document()
 
-        doc.add_header("Τίτλος")
+        doc.add_heading("Τίτλος")
         doc.add_paragraph(str(title_from_a02(entry[2])))
         doc.add_paragraph(str(subtitle_from_a03(entry[3])))
 
-        doc.add_header("Συγγραφείς", level=2)
+        doc.add_heading("Συγγραφείς", level=2)
         doc.add_unordered_list(authors_from_a01(entry[1]))
 
-        doc.add_header("Αριθμοί Εισαγωγης", level=2)
+        doc.add_heading("Αριθμοί Εισαγωγης", level=2)
         doc.add_unordered_list(
             entry_numbers_from_a04_a05_a06_a07_a08_a18_a19(
                 entry[4], entry[5], entry[6], entry[7], entry[8], entry[18], entry[19]
             )
         )
 
         doc.add_table(
@@ -426,15 +424,15 @@
                 ["Dewey", str(dewey_from_a04_a05(entry[4], entry[5]))],
                 ["Έκδοση", str(edition_from_a07(entry[7]))],
                 ["Εκδότης (Πόλη)", f"{editor}"],
                 ["Χρόνος έκδοσης", f"{edition_year_from_a09_a10(entry[9], entry[10])}"],
                 ["Σελίδες", f"{pages_from_a11(entry[11])}"],
                 ["Επιμελητής", f"{curator_from_a16(entry[16])}"],
                 ["Αντίτυπα", f"{copies_from_a17_a18_a30(entry[17], entry[18], entry[30])}"],
-                ["Δωρητές", MDList(donors).render()],
+                ["Δωρητές", MDList(donors)],
                 ["Τεύχος/Τόμος", f"{volume_from_a17_a18_a20_a30(entry[17], entry[18], entry[20], entry[30])}"],
                 ["Υλικό", f"{material_from_a18_a30(entry[18], entry[30])}"],
                 ["Σημειώσεις", f"{notes_from_a17_a18_a21_a30(entry[17], entry[18], entry[21], entry[30])}"],
                 ["ISBN", isbn],
                 ["ISSN", issn],
                 ["EAN", ean],
             ],
@@ -445,16 +443,16 @@
         doc.add_paragraph("Μεταφραστές")
         doc.add_unordered_list(translators)
 
         doc.add_paragraph("Θέματα")
         doc.add_unordered_list(topic_list)
 
         doc.add_paragraph("Ιδιότητες")
-        doc.add_element(
-            MDCheckList(
+        doc.add_block(
+            MDList(
                 ["Εχει CD"],
                 checked=has_cd_from_a02_a03_a12_a13_a14_a17_a18_a22_a30(
                     [
                         entry[2],
                         entry[3],
                         entry[12],
                         entry[13],
@@ -464,28 +462,28 @@
                         entry[22],
                         entry[30],
                     ]
                 ),
             )
         )
 
-        doc.add_element(
-            MDCheckList(
+        doc.add_block(
+            MDList(
                 ["Εχει DVD"],
                 checked=has_dvd_from_a30(
                     [
                         entry[30],
                     ]
                 ),
             )
         )
 
-        doc.add_element(MDCheckList(["Ανάτυπο"], checked=offprint_from_a17_a21_a30(entry[17], entry[21], entry[30])))
+        doc.add_block(MDList(["Ανάτυπο"], checked=offprint_from_a17_a21_a30(entry[17], entry[21], entry[30])))
 
-        doc.add_header("Αρχική Καρτέλα στο DBASE", level=1)
+        doc.add_heading("Αρχική Καρτέλα στο DBASE", level=1)
         doc.add_code(code=entry_as_yaml(entry, minimal=False), lang="yaml")
 
         title = title_from_a02(entry[2])
         if not title:
             title = "Χωρίς Τίτλο"
         subtitle = subtitle_from_a03(entry[3])
         if subtitle:
@@ -506,91 +504,88 @@
             by_dewey["Xωρίς dewey"].append((entry[0], title))
 
         with open(
             os.path.join(reports_directory, "entries", f"entry_{entry[0]:05}.md"), "w", encoding="utf-8"
         ) as outfile:
             outfile.write(str(doc))
 
-    index = Document("Όλες οι καρτέλες")
-    index.add_header("Όλες οι καρτέλες")
+    index = Document()
+    index.add_heading("Όλες οι καρτέλες")
     index.add_table_of_contents(range(1, 3))
 
     def divide_chunks(inlist: list[tuple[str, str]], size: int):
         for i in range(0, len(inlist), size):
             yield inlist[i : i + size]
 
     all_divided = list(divide_chunks(all, 1000))
     for thousands, sublist in enumerate(all_divided):
-        index.add_header(f"Απο {thousands*1000} ως {thousands*1000+len(sublist)}")
-        sublist = [
-            InlineText(f"{int(id):05}: {title}", url=f"./entry_{int(id):05}.html").render() for id, title in sublist
-        ]
+        index.add_heading(f"Απο {thousands*1000} ως {thousands*1000+len(sublist)}")
+        sublist = [Inline(f"{int(id):05}: {title}", link=f"./entry_{int(id):05}.html") for id, title in sublist]
         index.add_unordered_list(sublist)
 
     with open(os.path.join(reports_directory, "entries", "index.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(index))
 
-    index_by_author = Document("Όλες οι καρτέλες, κατα συγγραφέα")
-    index_by_author.add_header("Όλες οι καρτέλες, κατα συγγραφέα")
+    index_by_author = Document()
+    index_by_author.add_heading("Όλες οι καρτέλες, κατα συγγραφέα")
     index_by_author.add_table_of_contents(range(1, 3))
     for author_initial, author_dict in sorted(by_author.items()):
-        index_by_author.add_header(author_initial, level=2)
+        index_by_author.add_heading(author_initial, level=2)
         for author, entry_list in sorted(author_dict.items()):
-            index_by_author.add_header(author, level=3)
+            index_by_author.add_heading(author, level=3)
             entry_list = [
-                InlineText(f"{int(id):05}: {title}", url=f"./entry_{int(id):05}.html").render()
-                for id, title in entry_list
+                Inline(f"{int(id):05}: {title}", link=f"./entry_{int(id):05}.html") for id, title in entry_list
             ]
             index_by_author.add_unordered_list(entry_list)
     with open(os.path.join(reports_directory, "entries", "index_by_author.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(index_by_author))
 
-    index_by_dewey = Document("Όλες οι καρτέλες, κατα συγγραφέα")
-    index_by_dewey.add_header("Όλες οι καρτέλες, κατα συγγραφέα")
+    index_by_dewey = Document()
+    index_by_dewey.add_heading("Όλες οι καρτέλες, κατα συγγραφέα")
     index_by_dewey.add_table_of_contents(range(1, 3))
     for dewey, entry_list in sorted(by_dewey.items()):
-        index_by_dewey.add_header(dewey, level=2)
-        entry_list = [
-            InlineText(f"{int(id):05}: {title}", url=f"./entry_{int(id):05}.html").render() for id, title in entry_list
-        ]
+        index_by_dewey.add_heading(dewey, level=2)
+        entry_list = [Inline(f"{int(id):05}: {title}", link=f"./entry_{int(id):05}.html") for id, title in entry_list]
         index_by_dewey.add_unordered_list(entry_list)
     with open(os.path.join(reports_directory, "entries", "index_by_dewey.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(index_by_dewey))
 
 
 def add_index(reports_directory: str):
     os.makedirs(reports_directory, exist_ok=True)
-    doc = Document("index")
+    doc = Document()
 
-    doc.add_header("Βιβλιοθήκη Σκουφά: προσωρινός κατάλογος βιβλίων")
+    doc.add_heading("Βιβλιοθήκη Σκουφά: προσωρινός κατάλογος βιβλίων")
     doc.add_table_of_contents()
 
-    doc.add_paragraph(InlineText("Όλες οι καρτέλες", url="./entries/index.html").render())
-    doc.add_paragraph(InlineText("Όλες οι καρτέλες, κατα συγγραφέα", url="./entries/index_by_author.html").render())
-    doc.add_paragraph(InlineText("Όλες οι καρτέλες, κατα dewey", url="./entries/index_by_dewey.html").render())
-
-    doc.add_header("Τιμές κατα στήλη")
-    doc.add_paragraph(InlineText("Υπολογισμένες τιμές", url="./calculated-field/index.html").render())
-    doc.add_paragraph(InlineText("Τιμές στις στήλες των καρτελών", url="./single-field/index.html").render())
+    doc.add_paragraph(str(Inline("Όλες οι καρτέλες", link="./entries/index.html")))
+    doc.add_paragraph(str(Inline("Όλες οι καρτέλες, κατα συγγραφέα", link="./entries/index_by_author.html")))
+    doc.add_paragraph(str(Inline("Όλες οι καρτέλες, κατα dewey", link="./entries/index_by_dewey.html")))
+
+    doc.add_heading("Τιμές κατα στήλη")
+    doc.add_paragraph(str(Inline("Υπολογισμένες τιμές", link="./calculated-field/index.html")))
+    doc.add_paragraph(str(Inline("Τιμές στις στήλες των καρτελών", link="./single-field/index.html")))
 
-    doc.add_header("Ελεγκτικές Αναφορές")
+    doc.add_heading("Ελεγκτικές Αναφορές")
     doc.add_paragraph(
-        InlineText(
-            "Καρτέλες με διπλοπερασμένο αριθμητικό αριθμό εισαγωγής", url="./checks/duplicate_entry_numbers.html"
-        ).render()
+        str(
+            Inline(
+                "Καρτέλες με διπλοπερασμένο αριθμητικό αριθμό εισαγωγής", link="./checks/duplicate_entry_numbers.html"
+            )
+        )
     )
-    doc.add_paragraph(InlineText("Καρτέλες χωρίς αριθμό εισαγωγής", url="./checks/no_entry_numbers.html").render())
+    doc.add_paragraph(str(Inline("Καρτέλες χωρίς αριθμό εισαγωγής", link="./checks/no_entry_numbers.html")))
     doc.add_paragraph(
-        InlineText("Καρτέλες με μή αριθμητικό αριθμό εισαγωγής", url="./checks/non_numeric_entry_numbers.html").render()
+        str(Inline("Καρτέλες με μή αριθμητικό αριθμό εισαγωγής", link="./checks/non_numeric_entry_numbers.html"))
     )
-    doc.add_paragraph(InlineText("Dewey με προβληματικές τιμές", url="./checks/invalid_dewey.html").render())
-    doc.add_paragraph(InlineText("Μεταφραστές με παράξενα ονόματα", url="./checks/invalid_translators.html").render())
-    doc.add_paragraph(InlineText("Προβληματικά ISBN", url="./checks/invalid_isbn.html").render())
+    doc.add_paragraph(str(Inline("Dewey με προβληματικές τιμές", link="./checks/invalid_dewey.html")))
+    doc.add_paragraph(str(Inline("Μεταφραστές με παράξενα ονόματα", link="./checks/invalid_translators.html")))
+    doc.add_paragraph(str(Inline("Προβληματικά ISBN", link="./checks/invalid_isbn.html")))
 
-    doc.add_paragraph(InlineText("Δωρητές", url="./checks/donors.html").render())
+    doc.add_paragraph(str(Inline("Δωρητές", link="./checks/donors.html")))
 
     with open(os.path.join(reports_directory, "index.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(doc))
 
 
 def main():
     """Create markdown reports"""
```

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/src/skoufas_dbf_reader/utilities.py` & `skoufas_dbf_reader-0.0.2rc152.post1/src/skoufas_dbf_reader/utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/tests/test_field_extractors.py` & `skoufas_dbf_reader-0.0.2rc152.post1/tests/test_field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/tests/test_reports.py` & `skoufas_dbf_reader-0.0.2rc152.post1/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/tests/test_utilities.py` & `skoufas_dbf_reader-0.0.2rc152.post1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas-dbf-reader-0.0.2rc140.post1/PKG-INFO` & `skoufas_dbf_reader-0.0.2rc152.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: skoufas-dbf-reader
-Version: 0.0.2rc140.post1
+Version: 0.0.2rc152.post1
 Summary: Library for reading legacy DBF file with library data
 Author-email: Claudio Bantaloukas <rockreamer@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: dbfread==2.0.7
-Requires-Dist: snakemd==0.15.0
+Requires-Dist: snakemd==2.1.0
 Requires-Dist: PyYAML==6.0
 Requires-Dist: bandit[toml]==1.7.5 ; extra == "test"
 Requires-Dist: black==23.3.0 ; extra == "test"
 Requires-Dist: check-manifest==0.49 ; extra == "test"
 Requires-Dist: flake8-bugbear==23.3.23 ; extra == "test"
 Requires-Dist: flake8-docstrings ; extra == "test"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "test"
 Requires-Dist: flake8==6.0.0 ; extra == "test"
 Requires-Dist: pre-commit==3.2.2 ; extra == "test"
 Requires-Dist: pylint==2.17.2 ; extra == "test"
 Requires-Dist: pylint_junit ; extra == "test"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "test"
 Requires-Dist: pytest-mock<3.10.1 ; extra == "test"
 Requires-Dist: pytest-runner ; extra == "test"
-Requires-Dist: pytest==7.2.2 ; extra == "test"
+Requires-Dist: pytest==7.3.1 ; extra == "test"
 Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
 Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test"
 Project-URL: Documentation, https://github.com/skoufas/skoufas-dbf-reader#readme
 Project-URL: Source, https://github.com/skoufas/skoufas-dbf-reader
 Project-URL: Tracker, https://github.com/skoufas/skoufas-dbf-reader/issues
 Provides-Extra: test
```

