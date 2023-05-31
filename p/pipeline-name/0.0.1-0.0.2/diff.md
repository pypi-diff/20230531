# Comparing `tmp/pipeline_name-0.0.1.tar.gz` & `tmp/pipeline_name-0.0.2.tar.gz`

## Comparing `pipeline_name-0.0.1.tar` & `pipeline_name-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,12 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/message.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/.snakemake/log/2023-05-31T142730.797117.snakemake.log
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/.snakemake/log/2023-05-31T142734.485459.snakemake.log
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/.snakemake/log/2023-05-31T142743.154337.snakemake.log
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/.snakemake/log/2023-05-31T142746.964132.snakemake.log
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/.snakemake/log/2023-05-31T142823.561216.snakemake.log
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/.snakemake/log/2023-05-31T142831.553105.snakemake.log
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/.snakemake/metadata/bWVzc2FnZS50eHQ=
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/src/pipeline_name/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/src/pipeline_name/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/src/pipeline_name/__main__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/src/pipeline_name/config.yaml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/src/pipeline_name/cli/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/src/pipeline_name/workflow/Snakefile
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/README.md
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 pipeline_name-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/src/pipeline_name/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/src/pipeline_name/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/src/pipeline_name/__main__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/src/pipeline_name/config.yaml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/src/pipeline_name/cli/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/src/pipeline_name/workflow/Snakefile
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/README.md
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pipeline_name-0.0.2/PKG-INFO
```

### Comparing `pipeline_name-0.0.1/LICENSE.txt` & `pipeline_name-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pipeline_name-0.0.1/pyproject.toml` & `pipeline_name-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,17 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "snk",
 ]
 
 [project.urls]
-Documentation = "https://github.com/unknown/pipeline-name#readme"
-Issues = "https://github.com/unknown/pipeline-name/issues"
-Source = "https://github.com/unknown/pipeline-name"
+Documentation = "https://github.com/Wytamma/snk-pipeline-package-example#readme"
+Issues = "https://github.com/Wytamma/snk-pipeline-package-example/issues"
+Source = "https://github.com/Wytamma/snk-pipeline-package-example"
 
 [project.scripts]
 pipeline-name = "pipeline_name.cli:pipeline_name"
 
 [tool.hatch.version]
 path = "src/pipeline_name/__about__.py"
```

