# Comparing `tmp/s3local-0.3.0.tar.gz` & `tmp/s3local-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3local-0.3.0.tar", last modified: Sat Sep  3 06:09:39 2022, max compression
+gzip compressed data, was "s3local-0.4.0.tar", last modified: Wed May 31 12:35:36 2023, max compression
```

## Comparing `s3local-0.3.0.tar` & `s3local-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)        0 2022-09-03 06:09:39.209108 s3local-0.3.0/
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)     5041 2022-09-03 06:09:39.208802 s3local-0.3.0/PKG-INFO
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)     3460 2021-11-06 05:32:19.000000 s3local-0.3.0/README.md
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)       38 2022-09-03 06:09:39.209215 s3local-0.3.0/setup.cfg
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)     1182 2022-09-03 06:08:11.000000 s3local-0.3.0/setup.py
-drwxr-xr-x   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)        0 2022-09-03 06:09:39.198931 s3local-0.3.0/src/
-drwxr-xr-x   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)        0 2022-09-03 06:09:39.204324 s3local-0.3.0/src/s3local/
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)      199 2021-05-21 15:14:12.000000 s3local-0.3.0/src/s3local/__init__.py
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)     2913 2022-09-03 06:07:24.000000 s3local-0.3.0/src/s3local/commands.py
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)      153 2021-05-13 14:53:36.000000 s3local-0.3.0/src/s3local/constants.py
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)     1650 2022-03-07 09:22:17.000000 s3local-0.3.0/src/s3local/core.py
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)     2140 2022-03-18 16:04:51.000000 s3local-0.3.0/src/s3local/downloader.py
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)      301 2022-03-07 09:24:12.000000 s3local-0.3.0/src/s3local/logger.py
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)     2014 2022-09-03 06:07:24.000000 s3local-0.3.0/src/s3local/uploader.py
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)      885 2022-03-07 09:23:35.000000 s3local-0.3.0/src/s3local/util.py
-drwxr-xr-x   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)        0 2022-09-03 06:09:39.208248 s3local-0.3.0/src/s3local.egg-info/
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)     5041 2022-09-03 06:09:39.000000 s3local-0.3.0/src/s3local.egg-info/PKG-INFO
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)      449 2022-09-03 06:09:39.000000 s3local-0.3.0/src/s3local.egg-info/SOURCES.txt
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)        1 2022-09-03 06:09:39.000000 s3local-0.3.0/src/s3local.egg-info/dependency_links.txt
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)       51 2022-09-03 06:09:39.000000 s3local-0.3.0/src/s3local.egg-info/entry_points.txt
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)        1 2021-05-12 13:31:11.000000 s3local-0.3.0/src/s3local.egg-info/not-zip-safe
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)       29 2022-09-03 06:09:39.000000 s3local-0.3.0/src/s3local.egg-info/requires.txt
--rw-r--r--   0 hiroshi.toyama (817137910) DENA\Domain Users (1522739515)        8 2022-09-03 06:09:39.000000 s3local-0.3.0/src/s3local.egg-info/top_level.txt
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.263472 s3local-0.4.0/
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     4195 2023-05-31 12:35:36.263318 s3local-0.4.0/PKG-INFO
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     3628 2023-05-31 01:44:34.000000 s3local-0.4.0/README.md
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       38 2023-05-31 12:35:36.263522 s3local-0.4.0/setup.cfg
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     1183 2023-05-31 12:30:10.000000 s3local-0.4.0/setup.py
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.258824 s3local-0.4.0/src/
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.261051 s3local-0.4.0/src/s3local/
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      199 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/__init__.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2913 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/commands.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      153 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/constants.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2010 2023-05-31 12:16:10.000000 s3local-0.4.0/src/s3local/core.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2140 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/downloader.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      301 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/logger.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     2108 2023-05-31 12:16:10.000000 s3local-0.4.0/src/s3local/uploader.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      885 2023-05-29 11:53:08.000000 s3local-0.4.0/src/s3local/util.py
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.262478 s3local-0.4.0/src/s3local.egg-info/
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)     4195 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/PKG-INFO
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      491 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/SOURCES.txt
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        1 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/dependency_links.txt
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       50 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/entry_points.txt
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        1 2023-05-30 12:42:58.000000 s3local-0.4.0/src/s3local.egg-info/not-zip-safe
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)       29 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/requires.txt
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)        8 2023-05-31 12:35:36.000000 s3local-0.4.0/src/s3local.egg-info/top_level.txt
+drwxr-xr-x   0 hiroshi.toyama   (503) staff       (20)        0 2023-05-31 12:35:36.262977 s3local-0.4.0/tests/
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      686 2023-05-29 11:53:08.000000 s3local-0.4.0/tests/test_commands.py
+-rw-r--r--   0 hiroshi.toyama   (503) staff       (20)      402 2023-05-29 11:53:08.000000 s3local-0.4.0/tests/test_util.py
```

### Comparing `s3local-0.3.0/PKG-INFO` & `s3local-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,141 +1,147 @@
 Metadata-Version: 2.1
 Name: s3local
-Version: 0.3.0
+Version: 0.4.0
 Summary: Command Line utility for s3 local caching.
 Home-page: https://github.com/toyama0919/s3local
 Author: Hiroshi Toyama
 Author-email: toyama0919@gmail.com
 License: MIT
-Description: # s3local
-        
-        [![PyPI version](https://badge.fury.io/py/s3local.svg)](https://badge.fury.io/py/s3local)
-        [![tests](https://github.com/toyama0919/s3local/actions/workflows/tests.yml/badge.svg)](https://github.com/toyama0919/s3local/actions/workflows/tests.yml)
-        
-        Cache the object in s3 to localhost.
-        
-        Create a cache corresponding to s3 and automatically create a path for localhost and return it.
-        
-        Once downloaded files remain in localhost as cache, the second migration download will be skipped
-        
-        works on python3.6 or higher
-        
-        ## Settings
-        
-        aws auth support following.
-        
-        * environment variables
-        * profile(use --aws-profile option.)
-        * instance profile
-        
-        ## Examples
-        
-        #### download object and list object
-        
-        ```bash
-        $ s3local download -u s3://mybucket/artifacts/ --debug
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main2.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main3.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
-        
-        # next download is skip
-        $ s3local download -u s3://mybucket/artifacts/ --debug
-        2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main.log
-        2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main2.log
-        2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main3.log
-        
-        # overwrite download. (not skip)
-        $ s3local download -u s3://mybucket/artifacts/ --debug --no-skip-exist
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main2.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main3.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
-        ```
-        
-        By default `$HOME/.s3local` is the root directory.
-        
-        The format of path in local is as follows:
-        
-        ```
-        $HOME/.s3local/s3/${bucket}/${key}
-        ```
-        
-        You can change root by setting an environment variable S3LOCAL_ROOT.
-        
-        ```bash
-        $ s3local list-local -u s3://mybucket/artifacts/
-        /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
-        /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
-        /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
-        ```
-        
-        ## Python API
-        
-        ### download
-        
-        ```python
-        from s3local import Downloader
-        
-        s3local = Downloader("s3://mybucket/artifacts/")
-        list = s3local.list_local_path(download=True)
-        print(list)
-        #=> [
-        #     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log",
-        #     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log",
-        #     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log",
-        # ]
-        
-        ```
-        
-        ### upload
-        
-        ```python
-        from s3local import Uploader
-        
-        s3local = Uploader("s3://mybucket/artifacts/")
-        
-        uploader.upload("output/hoge.txt")
-        #=> s3://mybucket/artifacts/hoge.txt
-        
-        uploader.upload("output")
-        #=> s3://mybucket/artifacts/output/hoge.txt
-        
-        ```
-        
-        ## Installation
-        
-        ```sh
-        pip install s3local
-        ```
-        
-        ## CI
-        
-        ### install test package
-        
-        ```
-        $ ./scripts/ci.sh install
-        ```
-        
-        ### test
-        
-        ```
-        $ ./scripts/ci.sh run-test
-        ```
-        
-        flake8 and black and pytest.
-        
-        ### release pypi
-        
-        ```
-        $ ./scripts/ci.sh release
-        ```
-        
-        git tag and pypi release.
-        
 Keywords: s3local tool aws s3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
+
+# s3local
+
+[![PyPI version](https://badge.fury.io/py/s3local.svg)](https://badge.fury.io/py/s3local)
+[![tests](https://github.com/toyama0919/s3local/actions/workflows/tests.yml/badge.svg)](https://github.com/toyama0919/s3local/actions/workflows/tests.yml)
+
+Cache the object in s3 to localhost.
+
+Create a cache corresponding to s3 and automatically create a path for localhost and return it.
+
+Once downloaded files remain in localhost as cache, the second migration download will be skipped
+
+works on python3.6 or higher
+
+## Settings
+
+aws auth support following.
+
+* environment variables
+* profile(use --aws-profile option.)
+* instance profile
+
+## Examples
+
+#### download object and list object
+
+```bash
+$ s3local download -u s3://mybucket/artifacts/ --debug
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main2.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main3.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
+
+# next download is skip
+$ s3local download -u s3://mybucket/artifacts/ --debug
+2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main.log
+2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main2.log
+2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main3.log
+
+# overwrite download. (not skip)
+$ s3local download -u s3://mybucket/artifacts/ --debug --no-skip-exist
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main2.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main3.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
+```
+
+By default `$HOME/.s3local` is the root directory.
+
+The format of path in local is as follows:
+
+```
+$HOME/.s3local/s3/${bucket}/${key}
+```
+
+You can change root by setting an environment variable S3LOCAL_ROOT.
+
+```bash
+$ s3local list-local -u s3://mybucket/artifacts/
+/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
+/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
+/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
+```
+
+#### upload object
+
+```bash
+$ s3local upload -s tox.ini -u s3://mybucket/test/
+2023-05-31 10:44:08,474 INFO - Copying to s3: tox.ini => s3://mybucket/test/tox.ini
+```
+
+## Python API
+
+### download
+
+```python
+from s3local import Downloader
+
+s3local = Downloader("s3://mybucket/artifacts/")
+list = s3local.list_local_path(download=True)
+print(list)
+#=> [
+#     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log",
+#     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log",
+#     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log",
+# ]
+
+```
+
+### upload
+
+```python
+from s3local import Uploader
+
+s3local = Uploader("s3://mybucket/artifacts/")
+
+uploader.upload("output/hoge.txt")
+#=> s3://mybucket/artifacts/hoge.txt
+
+uploader.upload("output")
+#=> s3://mybucket/artifacts/output/hoge.txt
+
+```
+
+## Installation
+
+```sh
+pip install s3local
+```
+
+## CI
+
+### install test package
+
+```
+$ ./scripts/ci.sh install
+```
+
+### test
+
+```
+$ ./scripts/ci.sh run-test
+```
+
+flake8 and black and pytest.
+
+### release pypi
+
+```
+$ ./scripts/ci.sh release
+```
+
+git tag and pypi release.
```

### Comparing `s3local-0.3.0/README.md` & `s3local-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,21 @@
 ```bash
 $ s3local list-local -u s3://mybucket/artifacts/
 /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
 /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
 /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
 ```
 
+#### upload object
+
+```bash
+$ s3local upload -s tox.ini -u s3://mybucket/test/
+2023-05-31 10:44:08,474 INFO - Copying to s3: tox.ini => s3://mybucket/test/tox.ini
+```
+
 ## Python API
 
 ### download
 
 ```python
 from s3local import Downloader
```

### Comparing `s3local-0.3.0/setup.py` & `s3local-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 install_requires = ["boto3", "click>=7.0"]
 extras_require = {"test": ["tox"]}
 
 setup(
     name="s3local",
-    version="0.3.0",
+    version="0.4.0",
     description="Command Line utility for s3 local caching.",
     long_description=open(os.path.join(here, "README.md")).read(),
     long_description_content_type="text/markdown",
     classifiers=[
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="s3local tool aws s3",
     author="Hiroshi Toyama",
     author_email="toyama0919@gmail.com",
     url="https://github.com/toyama0919/s3local",
     license="MIT",
     packages=find_packages("src", exclude=["tests"]),
```

### Comparing `s3local-0.3.0/src/s3local/commands.py` & `s3local-0.4.0/src/s3local/commands.py`

 * *Files identical despite different names*

### Comparing `s3local-0.3.0/src/s3local/core.py` & `s3local-0.4.0/src/s3local/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,10 +44,18 @@
             ).delete()
         else:
             os.remove(self.local_path)
             self.bucket.delete_object(
                 Key=self.prefix,
             )
 
-    def exists_key(self, key: str) -> bool:
-        keys = self.bucket.objects.filter(Prefix=key)
-        return key in [k.key for k in keys]
+    def should_skip(self, objects_collection, key: str, source_path: str) -> bool:
+        objects = [o for o in objects_collection if o.key == key]
+        if len(objects) > 0:
+            size = objects[0].size
+            print(objects[0].__class__)
+            if os.path.getsize(source_path) == size:
+                self.logger.info(
+                    f"skip upload. match filesize ({size} byte) s3://{self.bucket_name}/{key}"
+                )
+                return True
+        return False
```

### Comparing `s3local-0.3.0/src/s3local/downloader.py` & `s3local-0.4.0/src/s3local/downloader.py`

 * *Files identical despite different names*

### Comparing `s3local-0.3.0/src/s3local/uploader.py` & `s3local-0.4.0/src/s3local/uploader.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,29 +15,36 @@
             if self.prefix.endswith("/"):
                 key = f"{self.prefix}{basename}"
             else:
                 # change basename
                 key = self.prefix
 
             # Check if the key exists
-            if skip_exist and self.exists_key(key=key):
-                self.logger.info(f"skip upload {source_path} > {key}")
+            objects = self.bucket.objects.filter(
+                Prefix=key,
+            )
+            if skip_exist and self.should_skip(
+                objects, key=key, source_path=source_path
+            ):
+                pass
             else:
                 self.upload_file(source_path, key, extra_args)
         elif os.path.isdir(source_path):
             if self.recursive:
                 objects = self.bucket.objects.filter(
                     Prefix=self.prefix,
                 )
-                already_upload_keys = [o.key for o in objects]
                 pair = Util.relative_files_from_dir(directory=source_path)
                 for abspath, relative_path in pair.items():
                     upload_key = f"{self.prefix}{relative_path}"
-                    if upload_key in already_upload_keys:
-                        self.logger.info(f"skip upload {upload_key}")
+
+                    if skip_exist and self.should_skip(
+                        objects, key=upload_key, source_path=abspath
+                    ):
+                        pass
                     else:
                         self.upload_file(abspath, upload_key, extra_args)
             else:
                 raise "not implement"
 
     def upload_file(self, local_path: str, key: str, extra_args: dict = None):
         # copy local
```

### Comparing `s3local-0.3.0/src/s3local/util.py` & `s3local-0.4.0/src/s3local/util.py`

 * *Files identical despite different names*

### Comparing `s3local-0.3.0/src/s3local.egg-info/PKG-INFO` & `s3local-0.4.0/src/s3local.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,141 +1,147 @@
 Metadata-Version: 2.1
 Name: s3local
-Version: 0.3.0
+Version: 0.4.0
 Summary: Command Line utility for s3 local caching.
 Home-page: https://github.com/toyama0919/s3local
 Author: Hiroshi Toyama
 Author-email: toyama0919@gmail.com
 License: MIT
-Description: # s3local
-        
-        [![PyPI version](https://badge.fury.io/py/s3local.svg)](https://badge.fury.io/py/s3local)
-        [![tests](https://github.com/toyama0919/s3local/actions/workflows/tests.yml/badge.svg)](https://github.com/toyama0919/s3local/actions/workflows/tests.yml)
-        
-        Cache the object in s3 to localhost.
-        
-        Create a cache corresponding to s3 and automatically create a path for localhost and return it.
-        
-        Once downloaded files remain in localhost as cache, the second migration download will be skipped
-        
-        works on python3.6 or higher
-        
-        ## Settings
-        
-        aws auth support following.
-        
-        * environment variables
-        * profile(use --aws-profile option.)
-        * instance profile
-        
-        ## Examples
-        
-        #### download object and list object
-        
-        ```bash
-        $ s3local download -u s3://mybucket/artifacts/ --debug
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main2.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main3.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
-        
-        # next download is skip
-        $ s3local download -u s3://mybucket/artifacts/ --debug
-        2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main.log
-        2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main2.log
-        2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main3.log
-        
-        # overwrite download. (not skip)
-        $ s3local download -u s3://mybucket/artifacts/ --debug --no-skip-exist
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main2.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
-        2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main3.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
-        ```
-        
-        By default `$HOME/.s3local` is the root directory.
-        
-        The format of path in local is as follows:
-        
-        ```
-        $HOME/.s3local/s3/${bucket}/${key}
-        ```
-        
-        You can change root by setting an environment variable S3LOCAL_ROOT.
-        
-        ```bash
-        $ s3local list-local -u s3://mybucket/artifacts/
-        /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
-        /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
-        /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
-        ```
-        
-        ## Python API
-        
-        ### download
-        
-        ```python
-        from s3local import Downloader
-        
-        s3local = Downloader("s3://mybucket/artifacts/")
-        list = s3local.list_local_path(download=True)
-        print(list)
-        #=> [
-        #     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log",
-        #     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log",
-        #     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log",
-        # ]
-        
-        ```
-        
-        ### upload
-        
-        ```python
-        from s3local import Uploader
-        
-        s3local = Uploader("s3://mybucket/artifacts/")
-        
-        uploader.upload("output/hoge.txt")
-        #=> s3://mybucket/artifacts/hoge.txt
-        
-        uploader.upload("output")
-        #=> s3://mybucket/artifacts/output/hoge.txt
-        
-        ```
-        
-        ## Installation
-        
-        ```sh
-        pip install s3local
-        ```
-        
-        ## CI
-        
-        ### install test package
-        
-        ```
-        $ ./scripts/ci.sh install
-        ```
-        
-        ### test
-        
-        ```
-        $ ./scripts/ci.sh run-test
-        ```
-        
-        flake8 and black and pytest.
-        
-        ### release pypi
-        
-        ```
-        $ ./scripts/ci.sh release
-        ```
-        
-        git tag and pypi release.
-        
 Keywords: s3local tool aws s3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
+
+# s3local
+
+[![PyPI version](https://badge.fury.io/py/s3local.svg)](https://badge.fury.io/py/s3local)
+[![tests](https://github.com/toyama0919/s3local/actions/workflows/tests.yml/badge.svg)](https://github.com/toyama0919/s3local/actions/workflows/tests.yml)
+
+Cache the object in s3 to localhost.
+
+Create a cache corresponding to s3 and automatically create a path for localhost and return it.
+
+Once downloaded files remain in localhost as cache, the second migration download will be skipped
+
+works on python3.6 or higher
+
+## Settings
+
+aws auth support following.
+
+* environment variables
+* profile(use --aws-profile option.)
+* instance profile
+
+## Examples
+
+#### download object and list object
+
+```bash
+$ s3local download -u s3://mybucket/artifacts/ --debug
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main2.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main3.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
+
+# next download is skip
+$ s3local download -u s3://mybucket/artifacts/ --debug
+2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main.log
+2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main2.log
+2021-05-14 14:08:02,970 DEBUG - skip already exists in local: s3://mybucket/artifacts/main3.log
+
+# overwrite download. (not skip)
+$ s3local download -u s3://mybucket/artifacts/ --debug --no-skip-exist
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main2.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
+2021-05-14 11:27:13,367 DEBUG - Copying: s3://mybucket/artifacts/main3.log > /Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
+```
+
+By default `$HOME/.s3local` is the root directory.
+
+The format of path in local is as follows:
+
+```
+$HOME/.s3local/s3/${bucket}/${key}
+```
+
+You can change root by setting an environment variable S3LOCAL_ROOT.
+
+```bash
+$ s3local list-local -u s3://mybucket/artifacts/
+/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log
+/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log
+/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log
+```
+
+#### upload object
+
+```bash
+$ s3local upload -s tox.ini -u s3://mybucket/test/
+2023-05-31 10:44:08,474 INFO - Copying to s3: tox.ini => s3://mybucket/test/tox.ini
+```
+
+## Python API
+
+### download
+
+```python
+from s3local import Downloader
+
+s3local = Downloader("s3://mybucket/artifacts/")
+list = s3local.list_local_path(download=True)
+print(list)
+#=> [
+#     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main.log",
+#     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main2.log",
+#     "/Users/hiroshi.toyama/.s3local/s3/mybucket/artifacts/main3.log",
+# ]
+
+```
+
+### upload
+
+```python
+from s3local import Uploader
+
+s3local = Uploader("s3://mybucket/artifacts/")
+
+uploader.upload("output/hoge.txt")
+#=> s3://mybucket/artifacts/hoge.txt
+
+uploader.upload("output")
+#=> s3://mybucket/artifacts/output/hoge.txt
+
+```
+
+## Installation
+
+```sh
+pip install s3local
+```
+
+## CI
+
+### install test package
+
+```
+$ ./scripts/ci.sh install
+```
+
+### test
+
+```
+$ ./scripts/ci.sh run-test
+```
+
+flake8 and black and pytest.
+
+### release pypi
+
+```
+$ ./scripts/ci.sh release
+```
+
+git tag and pypi release.
```

