# Comparing `tmp/spida-0.3.3.tar.gz` & `tmp/spida-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.3.3.tar", last modified: Tue May 30 20:24:17 2023, max compression
+gzip compressed data, was "spida-0.3.4.tar", last modified: Tue May 30 22:41:42 2023, max compression
```

## Comparing `spida-0.3.3.tar` & `spida-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 20:24:17.265165 spida-0.3.3/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.3.3/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6148 2023-05-30 20:24:17.263147 spida-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 20:24:17.265165 spida-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-30 20:22:48.000000 spida-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:24:17.217922 spida-0.3.3/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.3.3/spida/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:24:17.255073 spida-0.3.3/spida/data/
--rw-rw-rw-   0        0        0        2 2023-05-30 16:55:04.000000 spida-0.3.3/spida/data/config.json
--rw-rw-rw-   0        0        0    18821 2023-05-30 20:22:02.000000 spida-0.3.3/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:24:17.262137 spida-0.3.3/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.3.3/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.3.3/spida/utils/img.py
--rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.3.3/spida/utils/misc.py
--rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.3.3/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:24:17.253060 spida-0.3.3/spida.egg-info/
--rw-rw-rw-   0        0        0     6148 2023-05-30 20:24:17.000000 spida-0.3.3/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-30 20:24:17.000000 spida-0.3.3/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 20:24:17.000000 spida-0.3.3/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-30 20:24:17.000000 spida-0.3.3/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 20:24:17.000000 spida-0.3.3/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 22:41:42.954024 spida-0.3.4/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6148 2023-05-30 22:41:42.953020 spida-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 22:41:42.954024 spida-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-05-30 22:39:19.000000 spida-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:41:42.913304 spida-0.3.4/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.3.4/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:41:42.943889 spida-0.3.4/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-30 22:39:05.000000 spida-0.3.4/spida/data/config.json
+-rw-rw-rw-   0        0        0    19008 2023-05-30 22:36:47.000000 spida-0.3.4/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:41:42.950448 spida-0.3.4/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.3.4/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.3.4/spida/utils/img.py
+-rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.3.4/spida/utils/misc.py
+-rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.3.4/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:41:42.941756 spida-0.3.4/spida.egg-info/
+-rw-rw-rw-   0        0        0     6148 2023-05-30 22:41:42.000000 spida-0.3.4/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-30 22:41:42.000000 spida-0.3.4/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 22:41:42.000000 spida-0.3.4/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-30 22:41:42.000000 spida-0.3.4/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 22:41:42.000000 spida-0.3.4/spida.egg-info/top_level.txt
```

### Comparing `spida-0.3.3/LICENSE` & `spida-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.3.3/PKG-INFO` & `spida-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `spida-0.3.3/README.md` & `spida-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `spida-0.3.3/setup.py` & `spida-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.3.3",
+    version="0.3.4",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
```

### Comparing `spida-0.3.3/spida/stable_diffusion.py` & `spida-0.3.4/spida/stable_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class NoneProcessError(Exception):
     pass
 
 
 # initialize global variables
 config = {}
 webui_process = None
+webui_started = False
 request_fail_message = "Local server not running, starting..."
 
 # get config.json path
 with impres.as_file(impres.files("spida").joinpath("data")) as data_path:
     config_path = data_path.joinpath("config.json")
 
 
@@ -51,20 +52,20 @@
             webui_startfile if webui_startfile else "webui-user.bat"
         )
         url = input(
             "\nPlease input API url\n(if ENTER defaults to http://127.0.0.1:7860)\n"
         )
         config["url"] = url if url else "http://127.0.0.1:7860"
         use_subprocess = input(
-            "\nWould you like to start the Stable Diffusion WebUI using subprocess? [y/n]\n(ENTER defaults to y)\n"
+            "\nWould you like to start the Stable Diffusion WebUI using subprocess? [y/n]\n(if possible, ENTER defaults to n)\n"
         )
         config["use_subprocess"] = (
             False
-            if (use_subprocess.lower() if use_subprocess else "y") is "n"
-            and sys.platform is "win32"
+            if (use_subprocess.lower() if use_subprocess else "n") == "n"
+            and sys.platform == "win32"
             else True
         )
         print()
     else:
         config.update(config_dict)
     with open(config_path, "w") as f:
         json.dump(config, f)
@@ -89,27 +90,31 @@
     starts the file specified in the configuration, and then changes back to the original directory.
 
     Returns
     -------
     None
         This function does not return a value; it initiates the local API.
     """
-    if config["use_subprocess"]:
-        global webui_process
-        webui_process = subprocess.Popen(
-            config["webui_path"] + "/" + config["webui_startfile"],
-            cwd=config["webui_path"],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-        )
-    else:
-        cwd = os.getcwd()
-        os.chdir(config["webui_path"])
-        os.startfile(config["webui_startfile"])
-        os.chdir(cwd)
+    if not webui_started:
+        if config["use_subprocess"]:
+            global webui_process
+            webui_process = subprocess.Popen(
+                config["webui_path"] + "/" + config["webui_startfile"],
+                cwd=config["webui_path"],
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+            )
+        else:
+            cwd = os.getcwd()
+            os.chdir(config["webui_path"])
+            os.startfile(config["webui_startfile"])
+            os.chdir(cwd)
+
+        global webui_started
+        webui_started = True
 
 
 def stop(shell=False):
     """
     Stops the local API. If not a subprocess, kills all cmd or powershell terminals.
 
     Parameters
@@ -120,42 +125,45 @@
     Returns
     -------
     None
         This function does not return a value; it stops the local API.
     """
     if config["use_subprocess"]:
         if webui_process is None:
-            raise NoneProcessError("Could not find subprocess, webui must be running.")
+            raise NoneProcessError("Could not find subprocess.")
         else:
             if webui_process.poll() is None:
                 webui_process.terminate()
             else:
                 print("Process is already stopped.")
     else:
         if shell:
             os.system("taskkill /f /im powershell.exe")
         else:
             os.system("taskkill /f /im cmd.exe")
 
+    global webui_started
+    webui_started = False
+
 
 def print_webui_console():
     """
     Prints the standard output of the webui subprocess.
 
     Returns
     -------
     None
         This function does not return a value; it prints the webui console.
     """
     if config["use_subprocess"]:
         if webui_process is None:
-            raise NoneProcessError("Could not find subprocess, webui must be running.")
+            raise NoneProcessError("Could not find subprocess.")
         else:
-            stdout, stderr = webui_process.communicate()
-            print(stdout.read())
+            for line in webui_process.stdout:
+                print(line.decode().strip())
     else:
         print("Webui must be running as subprocess to use this function.")
 
 
 def model(name: str, search: bool = True):
     """
     Sets the Stable Diffusion (SD) model to be used.
```

### Comparing `spida-0.3.3/spida/utils/img.py` & `spida-0.3.4/spida/utils/img.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.3/spida/utils/misc.py` & `spida-0.3.4/spida/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.3/spida/utils/net.py` & `spida-0.3.4/spida/utils/net.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.3/spida.egg-info/PKG-INFO` & `spida-0.3.4/spida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

