# Comparing `tmp/snk-0.6.7.tar.gz` & `tmp/snk-0.6.8.tar.gz`

## Comparing `snk-0.6.7.tar` & `snk-0.6.8.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.7/Dockerfile
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.6.7/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.7/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.7/docs/CNAME
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.7/docs/index.md
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.6.7/docs/managing_pipelines.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.7/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.7/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.7/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.7/docs/reference/nest.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.7/snk/__about__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.7/snk/__init__.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.7/snk/errors.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.6.7/snk/main.py
--rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 snk-0.6.7/snk/nest.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.7/snk/pipeline.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.7/snk/cli/__init__.py
--rw-r--r--   0        0        0    18451 2020-02-02 00:00:00.000000 snk-0.6.7/snk/cli/cli.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 snk-0.6.7/snk/cli/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.7/snk/cli/options.py
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.7/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.7/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.7/tests/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.7/tests/conftest.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.7/tests/test_nest.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.7/tests/test_pipline_cli.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.7/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.7/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/pipeline/.snk
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/pipeline/cli.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/pipeline/resources/data.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/pipeline/workflow/Snakefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/pipeline/workflow/envs/base.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.7/tests/data/pipeline/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.7/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.7/LICENSE.txt
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 snk-0.6.7/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 snk-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.8/Dockerfile
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 snk-0.6.8/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.8/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.8/docs/CNAME
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.8/docs/index.md
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 snk-0.6.8/docs/managing_pipelines.md
+-rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 snk-0.6.8/docs/pipeline_packages.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 snk-0.6.8/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.8/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.8/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.8/docs/reference/nest.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.8/snk/__about__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 snk-0.6.8/snk/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 snk-0.6.8/snk/errors.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 snk-0.6.8/snk/main.py
+-rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 snk-0.6.8/snk/nest.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 snk-0.6.8/snk/pipeline.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/__init__.py
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/cli.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/options.py
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 snk-0.6.8/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.8/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.8/tests/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snk-0.6.8/tests/conftest.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.8/tests/test_nest.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 snk-0.6.8/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 snk-0.6.8/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.8/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/cli.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/resources/data.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/workflow/Snakefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/workflow/envs/base.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.8/tests/data/pipeline/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 snk-0.6.8/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.8/LICENSE.txt
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 snk-0.6.8/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 snk-0.6.8/PKG-INFO
```

### Comparing `snk-0.6.7/mkdocs.yml` & `snk-0.6.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/.github/workflows/publish.yml` & `snk-0.6.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/.github/workflows/tests.yml` & `snk-0.6.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/docs/index.md` & `snk-0.6.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/docs/managing_pipelines.md` & `snk-0.6.8/docs/managing_pipelines.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/snk/main.py` & `snk-0.6.8/snk/main.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/snk/nest.py` & `snk-0.6.8/snk/nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/snk/pipeline.py` & `snk-0.6.8/snk/pipeline.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/snk/cli/cli.py` & `snk-0.6.8/snk/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -212,14 +212,19 @@
         Examples:
           >>> with CLI.copy_resources(resources, cleanup=True):
           ...     # do something
         """
         copied_resources = []
 
         def copy_resource(src, dst, symlink=False):
+            if self.verbose:
+                typer.secho(
+                    f"- Copying resource '{src}' to '{dst}'",
+                    fg=typer.colors.YELLOW,
+                )
             target_is_directory = src.is_dir()
             if symlink:
                 os.symlink(src, dst, target_is_directory=target_is_directory)
             elif target_is_directory:
                 shutil.copytree(src, dst)
             else:
                 shutil.copy(src, dst)
@@ -228,47 +233,36 @@
             if resource.is_symlink():
                 resource.unlink()
             elif resource.is_dir():
                 shutil.rmtree(resource)
             else:
                 os.remove(resource)
 
+
+        resources_folder = self.pipeline.path / 'resources'
+        if resources_folder.exists():
+            resources.insert(0, Path('resources'))
+        if self.verbose:
+            typer.secho(
+                f"Copying {len(resources)} resources to working directory...",
+                fg=typer.colors.YELLOW,
+            )
         try:
-            # 
-            resources_folder = self.pipeline.path / 'resources'
-            # destination = Path(".") / 'resources'
-            # if destination.exists():
-            #     typer.secho(
-            #         "Resources folder exists! Skipping...\n",
-            #         fg=typer.colors.RED,
-            #     )
-            # else:
-            #     if resources_folder.exists():
-            #         if symlink_resources:
-            #             symlink_resource(resources_folder, destination)
-            #         else:
-            #             copy_resource(resources_folder, destination)
-            #         copied_resources.append(destination)
-            if resources_folder.exists():
-                resources.insert(0, Path('resources'))
             for resource in resources:
                 abs_path = self.pipeline.path / resource
                 destination = Path(".") / resource.name
                 if not destination.exists():
                     # make sure you don't delete files that are already there...
                     copy_resource(abs_path, destination, symlink=symlink_resources)
                     copied_resources.append(destination)
-                elif destination.exists() and not cleanup:
+                elif self.verbose:
                     typer.secho(
-                        f"Resource '{resource.name}' already exists! Skipping...",
-                        fg=typer.colors.RED,
+                        f"- Resource '{resource.name}' already exists! Skipping...",
+                        fg=typer.colors.YELLOW,
                     )
-                else:
-                    raise FileExistsError(f"Resource '{resource.name}' already exists!")
-
             yield
         finally:
             if not cleanup:
                 return
             for copied_resource in copied_resources:
                 if copied_resource.exists():
                     if self.verbose:
@@ -430,30 +424,32 @@
         ]
         if configs:
             args.extend(["--config", *configs])
         if verbose:
             typer.secho(f"snakemake {' '.join(args)}\n", fg=typer.colors.MAGENTA)
 
         self.snk_config.add_resources(resource, self.pipeline.path)
-
-        with self.copy_resources(
-            self.snk_config.resources, 
-            cleanup=not keep_resources, 
-            symlink_resources=self.snk_config.symlink_resources
-        ):
-            try:
-                snakemake.main(args)
-            except SystemExit as e:
-                status = int(str(e))
-                if status:
-                    sys.exit(status)
-        if not keep_snakemake and Path(".snakemake").exists():
-            if verbose:
-                typer.secho("Deleting '.snakemake' folder...", fg="yellow")
-            shutil.rmtree(".snakemake")
+        try:
+            with self.copy_resources(
+                self.snk_config.resources, 
+                cleanup=not keep_resources, 
+                symlink_resources=self.snk_config.symlink_resources
+            ):
+                try:
+                    snakemake.main(args)
+                except SystemExit as e:
+                    status = int(str(e))
+                    if status:
+                        sys.exit(status)
+            if not keep_snakemake and Path(".snakemake").exists():
+                if verbose:
+                    typer.secho("Deleting '.snakemake' folder...", fg="yellow")
+                shutil.rmtree(".snakemake")
+        except FileExistsError as e:
+            typer.secho(e, fg=typer.colors.RED)
 
     def info(self):
         """
         Display information about current pipeline install.
         Returns:
           str: A JSON string containing information about the current pipeline install.
         Examples:
```

### Comparing `snk-0.6.7/snk/cli/config.py` & `snk-0.6.8/snk/cli/config.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/snk/cli/utils.py` & `snk-0.6.8/snk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/.DS_Store` & `snk-0.6.8/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/conftest.py` & `snk-0.6.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/test_nest.py` & `snk-0.6.8/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/test_pipline_cli.py` & `snk-0.6.8/tests/test_pipline_cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/test_snk.py` & `snk-0.6.8/tests/test_snk.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/utils.py` & `snk-0.6.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/data/artic_v4.1.bed` & `snk-0.6.8/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/data/config.yaml` & `snk-0.6.8/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/tests/data/cov.fasta` & `snk-0.6.8/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/LICENSE.txt` & `snk-0.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/README.md` & `snk-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/pyproject.toml` & `snk-0.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.6.7/PKG-INFO` & `snk-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.6.7
+Version: 0.6.8
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

