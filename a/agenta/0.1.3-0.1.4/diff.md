# Comparing `tmp/agenta-0.1.3.tar.gz` & `tmp/agenta-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenta-0.1.3.tar", max compression
+gzip compressed data, was "agenta-0.1.4.tar", max compression
```

## Comparing `agenta-0.1.3.tar` & `agenta-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.3/README.md
--rw-r--r--   0        0        0       53 2023-05-20 06:49:49.205423 agenta-0.1.3/agenta/__init__.py
--rw-r--r--   0        0        0     3045 2023-05-30 19:16:46.669891 agenta-0.1.3/agenta/agenta.py
--rw-r--r--   0        0        0     5924 2023-05-29 13:26:47.815435 agenta-0.1.3/agenta/cli.py
--rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.3/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.3/agenta/client/__init__.py
--rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.3/agenta/client/api_models.py
--rw-r--r--   0        0        0     1479 2023-05-26 07:44:13.475577 agenta-0.1.3/agenta/client/client.py
--rw-r--r--   0        0        0      550 2023-05-11 14:46:01.166162 agenta-0.1.3/agenta/config.py
--rw-r--r--   0        0        0       91 2023-05-12 12:52:29.405049 agenta-0.1.3/agenta/config.toml
--rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.3/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.3/agenta/docker/docker-assets/README.md
--rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.3/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     2585 2023-05-27 10:11:21.981693 agenta-0.1.3/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      407 2023-05-22 17:58:10.352282 agenta-0.1.3/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.3/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.3/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.3/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0      513 2023-05-31 17:02:54.646010 agenta-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 agenta-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-05-31 15:39:19.179107 agenta-0.1.4/README.md
+-rw-r--r--   0        0        0       53 2023-05-20 06:49:49.205423 agenta-0.1.4/agenta/__init__.py
+-rw-r--r--   0        0        0     3045 2023-05-30 19:16:46.669891 agenta-0.1.4/agenta/agenta.py
+-rw-r--r--   0        0        0     6292 2023-05-31 17:19:38.375403 agenta-0.1.4/agenta/cli.py
+-rw-r--r--   0        0        0      131 2023-05-15 11:40:40.483678 agenta-0.1.4/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2023-05-15 11:36:10.263480 agenta-0.1.4/agenta/client/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-26 07:42:52.867662 agenta-0.1.4/agenta/client/api_models.py
+-rw-r--r--   0        0        0     1479 2023-05-26 07:44:13.475577 agenta-0.1.4/agenta/client/client.py
+-rw-r--r--   0        0        0      550 2023-05-11 14:46:01.166162 agenta-0.1.4/agenta/config.py
+-rw-r--r--   0        0        0       91 2023-05-12 12:52:29.405049 agenta-0.1.4/agenta/config.toml
+-rw-r--r--   0        0        0      337 2023-05-24 09:05:58.092867 agenta-0.1.4/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2023-05-11 15:47:22.031685 agenta-0.1.4/agenta/docker/docker-assets/README.md
+-rw-r--r--   0        0        0      256 2023-05-20 06:49:49.205919 agenta-0.1.4/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     2585 2023-05-27 10:11:21.981693 agenta-0.1.4/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      482 2023-05-31 17:12:43.842983 agenta-0.1.4/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      660 2023-05-31 17:02:48.853909 agenta-0.1.4/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       31 2023-05-10 09:29:53.673600 agenta-0.1.4/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2023-05-15 11:25:55.227110 agenta-0.1.4/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0      513 2023-05-31 17:20:07.454240 agenta-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 agenta-0.1.4/PKG-INFO
```

### Comparing `agenta-0.1.3/agenta/agenta.py` & `agenta-0.1.4/agenta/agenta.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.3/agenta/cli.py` & `agenta-0.1.4/agenta/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,20 @@
         variant_name = questionary.select(
             'Please choose a variant',
             choices=config['variants']
         ).ask()
 
     endpoint = client.start_variant(app_name, variant_name)
     click.echo(
-        f"Started variant {variant_name} for App {app_name}. Endpoint: {endpoint}")
+        f"""Variant {variant_name} for App {app_name} added successfully to Agenta!\n
+        You app has been deployed locally as an api: {endpoint}/openapi.json \n\n
+
+        Go to the playground to experiment with your app : http://localhost:3000/apps/{app_name}/playground \n
+        """
+    )
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -119,19 +124,19 @@
     config = {"app-name": app_name}
     with open('config.toml', 'w') as config_file:
         toml.dump(config, config_file)
 
     # Ask for init option
     init_option = questionary.select(
         "How do you want to initialize your app?",
-        choices=['Blank App', 'From Template']
+        choices=['Blank App', 'Start from template']
     ).ask()
 
     # If the user selected the second option, show a list of available templates
-    if init_option == 'From Template':
+    if init_option == 'Start from template':
         current_dir = Path.cwd()
         template_dir = Path(__file__).parent / "templates"
         templates = [folder.name for folder in template_dir.iterdir()
                      if folder.is_dir()]
         template_desc = [toml.load(
             (template_dir / name / 'template.toml'))['short_desc'] for name in templates]
 
@@ -144,14 +149,16 @@
 
         # Copy the template files to the current directory
         chosen_template_dir = template_dir / template
         for file in chosen_template_dir.glob("*"):
             if file.name != 'template.toml' and not file.is_dir():
                 shutil.copy(file, current_dir / file.name)
     click.echo("App initialized successfully")
+    if init_option == 'Start from template':
+        click.echo("Please check the README.md for further instructions to setup the template.")
 
 
 @click.command(name='start')
 @click.option('--variant_name', default=None)
 @click.argument('app_folder', default=".")
 def start_variant_cli(variant_name: str, app_folder: str):
     """Start a variant."""
```

### Comparing `agenta-0.1.3/agenta/client/client.py` & `agenta-0.1.4/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.3/agenta/config.py` & `agenta-0.1.4/agenta/config.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.3/agenta/docker/docker_utils.py` & `agenta-0.1.4/agenta/docker/docker_utils.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.3/agenta/templates/simple_prompt/app.py` & `agenta-0.1.4/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `agenta-0.1.3/pyproject.toml` & `agenta-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agenta"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Mahmoud Mabrouk <mahmoudmabrouk.mail@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 docker = "^6.1.1"
```

### Comparing `agenta-0.1.3/PKG-INFO` & `agenta-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agenta
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Mahmoud Mabrouk
 Author-email: mahmoudmabrouk.mail@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

