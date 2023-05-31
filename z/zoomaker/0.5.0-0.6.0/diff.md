# Comparing `tmp/zoomaker-0.5.0.tar.gz` & `tmp/zoomaker-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.5.0.tar", max compression
+gzip compressed data, was "zoomaker-0.6.0.tar", max compression
```

## Comparing `zoomaker-0.5.0.tar` & `zoomaker-0.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6424 2023-05-23 15:27:26.401882 zoomaker-0.5.0/README.md
--rw-r--r--   0        0        0      587 2023-05-23 15:30:53.191905 zoomaker-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6855 2023-05-23 15:29:01.177122 zoomaker-0.5.0/zoomaker.py
--rw-r--r--   0        0        0     7131 1970-01-01 00:00:00.000000 zoomaker-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     6710 2023-05-30 08:35:06.044965 zoomaker-0.6.0/README.md
+-rw-r--r--   0        0        0      587 2023-05-31 13:30:33.057192 zoomaker-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7123 2023-05-31 13:30:29.148792 zoomaker-0.6.0/zoomaker.py
+-rw-r--r--   0        0        0     7417 1970-01-01 00:00:00.000000 zoomaker-0.6.0/PKG-INFO
```

### Comparing `zoomaker-0.5.0/README.md` & `zoomaker-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 ![zoomaker_social_keyvisual](https://github.com/hfg-gmuend/zoomaker/assets/480224/75d3d492-fe54-4711-afbf-02768bbb4033)
 
 Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 ========
 
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
 
-- **single source of truth**: all resources are neatly definied in the `zoo.yaml` file
+- **single source of truth**: all resources are neatly defined in the `zoo.yaml` file
 - **freeze versions**: know exactly which revision of a resources is installed at any time
 - **only download once**: optimize bandwidth and cache your models locally
 - **optimize disk usage**: downloaded models are symlinked to the installation folder (small files <5MB are duplicate)
 
 ## 😻 TL;DR
 
 1. Install Zoomaker `pip install zoomaker`
 2. Define your resources in the `zoo.yaml` file
 3. Run `zoomaker install` to install them
+(on Windows: `zoomaker install --no-symlinks`, see [hints](https://github.com/hfg-gmuend/zoomaker#%EF%B8%8F-limitations-on-windows) below)
 
 
 ## 📦 Installation
 
 ```bash
 pip install zoomaker
 ```
@@ -117,18 +118,17 @@
   resources:
     - name: analog-diffusion-v1
       src: https://civitai.com/api/download/models/1344
       type: download
       install_to: ./stable-diffusion-webui/models/Stable-diffusion/
       rename_to: analog-diffusion-v1.safetensors
 ```
-</details>
-
 Please note:
-The resource `type: download` can be seen as the last resort. Currently there is no caching or symlinking of web downloads. Recommended to avoid it.
+The resource `type: download` can be seen as the last resort. Currently there is no caching or symlinking of web downloads. Recommended to avoid it :)
+</details>
 
 ## 🧮 zoo.yaml Structure
 
 <details>
 <summary>Top level:</summary>
 
 - `name` (mandatory)
@@ -173,7 +173,8 @@
 
 ```bash
 huggingface-cli login
 ```
 
 ## 🙏 Acknowledgements
 - Most of the internal heavy lifting is done be the [huggingface_hub library](https://huggingface.co/docs/huggingface_hub/guides/download) by Hugging Face. Thanks!
+- "Zoomaker Safari Hacker Cat" cover image by Alia Tasler, based on this [OpenMoji](https://openmoji.org/library/emoji-1F431-200D-1F4BB/). Thanks!
```

### Comparing `zoomaker-0.5.0/pyproject.toml` & `zoomaker-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zoomaker"
-version = "0.5.0"
+version = "0.6.0"
 description = "Zoomaker - Friendly house keeping for your AI model zoo and related resources."
 authors = ["Benedikt Groß"]
 readme = "README.md"
 homepage = "https://github.com/hfg-gmuend/zoomaker"
 documentation = "https://github.com/hfg-gmuend/zoomaker"
 repository = "https://github.com/hfg-gmuend/zoomaker"
```

### Comparing `zoomaker-0.5.0/zoomaker.py` & `zoomaker-0.6.0/zoomaker.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
                 # Hugging Face Hub
                 if type == "huggingface":
                     repo_id = "/".join(src.split("/")[0:2])
                     repo_filepath = "/".join(src.split("/")[2:])
                     downloaded = hf_hub_download(repo_id=repo_id, filename=repo_filepath, local_dir=install_to, revision=revision, local_dir_use_symlinks=False if no_symlinks else "auto")
                     if rename_to:
-                        os.rename(downloaded, os.path.join(install_to, rename_to))
+                        self._rename_file(downloaded, os.path.join(install_to, rename_to))
                 # Git
                 elif type == "git":
                     repo_path = os.path.join(install_to, self._get_repo_name(src))
                     if rename_to:
                         print(f"\trename_to is not supported for git repos. Ignoring rename_to: {rename_to}")
                     # existing repo
                     if os.path.exists(repo_path):
@@ -85,15 +85,15 @@
                         else:
                             repo.remotes.origin.pull()
                             print(f"\tgit pull latest: {repo.head.object.hexsha}")
                 # Download
                 else:
                     downloaded = self._download_file(src, os.path.join(install_to, os.path.basename(src)))
                     if rename_to:
-                        os.rename(downloaded, os.path.join(install_to, rename_to))
+                        self._rename_file(downloaded, os.path.join(install_to, rename_to))
                     if revision:
                         print(f"\trevision is not supported for download. Ignoring revision: {revision}")
 
         print(f"\n✅ {counter} resources installed.")
 
     def run(self, script_name: str):
         if script_name not in self.data["scripts"]:
@@ -108,14 +108,22 @@
 
     def _get_repo_name(self, src: str):
         if src.endswith(".git"):
             return os.path.basename(src).replace(".git", "")
         else:
             return os.path.basename(src)
 
+    def _rename_file(self, src, dest):
+        # remove dest if exists due to os.rename limitation in Windows
+        if os.path.exists(dest):
+            os.remove(dest)
+            os.rename(src, dest)
+        else:
+            os.rename(src, dest)
+
     def _download_file(self, url, filename):
         response = requests.get(url, stream=True)
         total_size_in_bytes = int(response.headers.get('content-length', 0))
         block_size = 1024
         progress_bar = tqdm(desc="\tdownloading", total=total_size_in_bytes, unit='iB', unit_scale=True, ncols=100)
         with open(filename, 'wb') as file:
             for data in response.iter_content(block_size):
@@ -128,15 +136,15 @@
         return filename
 
 def main():
     parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file.")
     parser.add_argument("command", nargs="?", choices=["install", "run"], help="The command to execute.")
     parser.add_argument("script", nargs="?", help="The script name to execute.")
     parser.add_argument("--no-symlinks", action='store_true', help="Do not create symlinks for the installed resources.")
-    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.5.0")
+    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.6.0")
     args = parser.parse_args()
 
     if args.command == "install":
         Zoomaker("zoo.yaml").install(args.no_symlinks)
     elif args.command == "run":
         Zoomaker("zoo.yaml").run(args.script)
     else:
```

### Comparing `zoomaker-0.5.0/PKG-INFO` & `zoomaker-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoomaker
-Version: 0.5.0
+Version: 0.6.0
 Summary: Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 Home-page: https://github.com/hfg-gmuend/zoomaker
 Author: Benedikt Groß
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,24 +18,25 @@
 ![zoomaker_social_keyvisual](https://github.com/hfg-gmuend/zoomaker/assets/480224/75d3d492-fe54-4711-afbf-02768bbb4033)
 
 Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 ========
 
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
 
-- **single source of truth**: all resources are neatly definied in the `zoo.yaml` file
+- **single source of truth**: all resources are neatly defined in the `zoo.yaml` file
 - **freeze versions**: know exactly which revision of a resources is installed at any time
 - **only download once**: optimize bandwidth and cache your models locally
 - **optimize disk usage**: downloaded models are symlinked to the installation folder (small files <5MB are duplicate)
 
 ## 😻 TL;DR
 
 1. Install Zoomaker `pip install zoomaker`
 2. Define your resources in the `zoo.yaml` file
 3. Run `zoomaker install` to install them
+(on Windows: `zoomaker install --no-symlinks`, see [hints](https://github.com/hfg-gmuend/zoomaker#%EF%B8%8F-limitations-on-windows) below)
 
 
 ## 📦 Installation
 
 ```bash
 pip install zoomaker
 ```
@@ -134,18 +135,17 @@
   resources:
     - name: analog-diffusion-v1
       src: https://civitai.com/api/download/models/1344
       type: download
       install_to: ./stable-diffusion-webui/models/Stable-diffusion/
       rename_to: analog-diffusion-v1.safetensors
 ```
-</details>
-
 Please note:
-The resource `type: download` can be seen as the last resort. Currently there is no caching or symlinking of web downloads. Recommended to avoid it.
+The resource `type: download` can be seen as the last resort. Currently there is no caching or symlinking of web downloads. Recommended to avoid it :)
+</details>
 
 ## 🧮 zoo.yaml Structure
 
 <details>
 <summary>Top level:</summary>
 
 - `name` (mandatory)
@@ -190,8 +190,9 @@
 
 ```bash
 huggingface-cli login
 ```
 
 ## 🙏 Acknowledgements
 - Most of the internal heavy lifting is done be the [huggingface_hub library](https://huggingface.co/docs/huggingface_hub/guides/download) by Hugging Face. Thanks!
+- "Zoomaker Safari Hacker Cat" cover image by Alia Tasler, based on this [OpenMoji](https://openmoji.org/library/emoji-1F431-200D-1F4BB/). Thanks!
```

