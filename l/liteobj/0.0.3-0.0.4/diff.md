# Comparing `tmp/liteobj-0.0.3.tar.gz` & `tmp/liteobj-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteobj-0.0.3.tar", last modified: Thu May 25 22:18:58 2023, max compression
+gzip compressed data, was "liteobj-0.0.4.tar", last modified: Tue May 30 23:38:59 2023, max compression
```

## Comparing `liteobj-0.0.3.tar` & `liteobj-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 22:18:58.542070 liteobj-0.0.3/
--rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.3/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-05-25 22:18:58.542070 liteobj-0.0.3/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1349 2023-05-25 22:11:37.000000 liteobj-0.0.3/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 22:18:58.532070 liteobj-0.0.3/liteobj/
--rw-r--r--   0 user      (1000) user      (1000)       20 2023-05-25 22:02:13.000000 liteobj-0.0.3/liteobj/__init__.py
--rwxr-xr-x   0 user      (1000) user      (1000)     3541 2023-05-25 22:12:29.000000 liteobj-0.0.3/liteobj/lite.py
--rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.3/liteobj/requirements.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 22:18:58.542070 liteobj-0.0.3/liteobj.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      275 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       29 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-25 22:18:58.000000 liteobj-0.0.3/liteobj.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-25 22:18:58.542070 liteobj-0.0.3/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)      706 2023-05-25 22:15:21.000000 liteobj-0.0.3/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:38:59.970169 liteobj-0.0.4/
+-rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.4/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-05-30 23:38:59.970169 liteobj-0.0.4/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1066 2023-05-25 23:05:01.000000 liteobj-0.0.4/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:38:59.970169 liteobj-0.0.4/liteobj/
+-rw-r--r--   0 user      (1000) user      (1000)       20 2023-05-25 22:02:13.000000 liteobj-0.0.4/liteobj/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     3056 2023-05-30 23:38:02.000000 liteobj-0.0.4/liteobj/lite.py
+-rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.4/liteobj/requirements.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 23:38:59.970169 liteobj-0.0.4/liteobj.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      275 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       29 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-05-30 23:38:59.000000 liteobj-0.0.4/liteobj.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-30 23:38:59.970169 liteobj-0.0.4/setup.cfg
+-rwxr-xr-x   0 user      (1000) user      (1000)      706 2023-05-30 22:51:51.000000 liteobj-0.0.4/setup.py
```

### Comparing `liteobj-0.0.3/LICENSE` & `liteobj-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `liteobj-0.0.3/README.md` & `liteobj-0.0.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 # Liteobj
 
 Liteweight configuration format for defining and recursively instantiating python objects composed of nested object parameters
 
-See [tutorial.ipynb](https://github.com/1lint/liteobj/blob/master/tutorial.ipynb) example use of `liteobj` (tutorial for previous version, currently out of date, will be fixed soon)
-
 ## Install
 
 Install from pip
 ```
 pip install liteobj
 ```
 
-## Quickstart Example
-As a basic example, run the Pytorch Lightning Basic GAN tutorial from https://pytorch-lightning.readthedocs.io/en/stable/notebooks/lightning_examples/basic-gan.html
+## Quickstart Example with Gradio
 ```
 git clone https://github.com/1lint/liteobj
 cd liteobj
-python -m pip install -r basic_gan/requirements.txt
-python lite.py basic_gan/lab.yaml fit
-```
-
-To run lite.py in other directories, install the pip package. Then run configurations with the `lite` console script 
+pip install liteobj==0.0.3 gradio==3.31.0
+lite demo.yaml launch --server_port=7680 --server_name=0.0.0.0
 ```
-python -m pip install .
-lite basic_gan/lab.yaml fit
-```
-
 CLI syntax is 
 ```
 lite {config_path} {object_method} {method_args} {method_kwargs}
 ```
 `config_path` is path to the yaml file to instantiate, and is the only required parameter. Returns the instantiated object instance
 `object_method` is the name of the object method to invoke once the object is instantiated. If passed, returns the output of the object method
 `method_args` and `method_kwargs` are passed directly into the object method. 
 
+## Tutorial
+(tutorial currently out of date, to be updated)
+See [tutorial.ipynb](https://github.com/1lint/liteobj/blob/master/tutorial.ipynb) for example use of `liteobj` to quickly run training with pytorch-lightning
```

### Comparing `liteobj-0.0.3/liteobj/lite.py` & `liteobj-0.0.4/liteobj/lite.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,30 @@
 from importlib import import_module
 from fire import Fire
 from omegaconf import OmegaConf, DictConfig
-from typing import Any
+from typing import Any, List
 import sys
-import os
 from time import time
 from pathlib import Path
 
 SUPER_CONFIG_KEY = 'super'
 CLASS_STRING = 'class_string' 
 
 KWARGS = 'kwargs'
 ARGS = 'args'
 METHOD_KEY = 'method'
 
 METADATA_KEY = 'lite_metadata'
 
-
-# compile function source and assign object to target_name
-def compile_callable(source, target_name=None):
-
-    ldict = {}
-    exec(source, globals(), ldict)
-
-    if target_name:
-        return ldict[target_name]
-    else:
-        for v in ldict.values():
-            if callable(v):
-                return v
-
 # pack args and kwargs into a list
-def listify(*args, **kwargs):
+def listify(*args, **kwargs) -> List:
     return [*args, *kwargs.values()]
 
-# computes class_string for class object
-def get_class_string(_class):
-    return f'{_class.__module__}.{_class.__name__}'
-
 # recursively load config with superconfigs
-def load_config(yaml_file: str) -> DictConfig:
+def load_config(yaml_file: str|Path) -> DictConfig:
 
     config = OmegaConf.load(yaml_file)
 
     if SUPER_CONFIG_KEY in config:
         super_configs = []
         for super_config in config[SUPER_CONFIG_KEY]:
             super_configs.append(load_config(super_config))
@@ -56,42 +37,43 @@
 
     class_string = config.get(CLASS_STRING, None)
     if class_string is None:
         raise ValueError(f"Cannot instantiate object without '{CLASS_STRING}' key")
     
     module_name, class_name = class_string.rsplit(".", 1)
     module = import_module(module_name)
-    module_class = getattr(module, class_name)
+    module_attribute = getattr(module, class_name)
+
+    method_string = config.get(METHOD_KEY, "")
+    if method_string is None:
+        return module_attribute
 
     kwargs = {}
     if KWARGS in config:
         for k, v in config[KWARGS].items():
-            kwargs[k] = instantiate(v) if isinstance(config[KWARGS][k], DictConfig) else v
+            kwargs[k] = instantiate(v) if hasattr(v, CLASS_STRING) else v
  
     args = []
     if ARGS in config:
         for item in config[ARGS]:
-            args.append(instantiate(item)) if isinstance(item, DictConfig) else args.append(item)
-
+            item = instantiate(item) if hasattr(item, CLASS_STRING) else item
+            args.append(item)
 
-    # allow custom instantiation method
-    method_string = config.get(METHOD_KEY, '__init__')
-    if method_string is None:
-        return module_class
-
-    # have to invoke __init__ method as special case due to nuances of python compiler
-    if method_string == '__init__':
-        return module_class(*args, **kwargs)
+    if method_string == "":
+        return module_attribute(*args, **kwargs)
     else:
-        method = getattr(module_class, method_string)
+        method = getattr(module_attribute, method_string)
         return method(*args, **kwargs)
 
 # convenience method for running object from yaml
-def run(yaml_file: str, method_string: str=None, *args, **kwargs) -> Any:
-    sys.path.append(os.getcwd()) 
+def run(yaml_file: str|Path, method_string: str=None, *args, **kwargs) -> Any:
+
+    yaml_file = Path(yaml_file)
+    sys.path.append(str(Path.cwd()))
+    sys.path.append(str(yaml_file.parent.resolve()))
 
     config = load_config(yaml_file)
 
     metadata = dict(config.get(METADATA_KEY, {}))
     metadata["config_path"] = str(Path(yaml_file).resolve())
     metadata["time"] = time()
```

### Comparing `liteobj-0.0.3/setup.py` & `liteobj-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 00000060: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
 00000070: 6d65 6e74 7320 3d20 6f70 656e 2866 227b  ments = open(f"{
 00000080: 7265 706f 5f6e 616d 657d 2f7b 7265 7175  repo_name}/{requ
 00000090: 6972 656d 656e 7473 5f66 6e7d 2229 2e72  irements_fn}").r
 000000a0: 6561 6428 292e 7370 6c69 7428 290d 0a0d  ead().split()...
 000000b0: 0a73 6574 7570 286e 616d 653d 7265 706f  .setup(name=repo
 000000c0: 5f6e 616d 652c 0d0a 2020 2020 2020 7665  _name,..      ve
-000000d0: 7273 696f 6e3d 2730 2e30 2e33 272c 0d0a  rsion='0.0.3',..
+000000d0: 7273 696f 6e3d 2730 2e30 2e34 272c 0d0a  rsion='0.0.4',..
 000000e0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
 000000f0: 6e3d 2743 7265 6174 6520 6c69 6768 7477  n='Create lightw
 00000100: 6569 6768 7420 636f 6e66 6967 7320 666f  eight configs fo
 00000110: 7220 696e 7374 616e 7469 6174 696e 6720  r instantiating 
 00000120: 4d4c 2065 7870 6572 696d 656e 7473 272c  ML experiments',
 00000130: 0d0a 2020 2020 2020 6175 7468 6f72 3d27  ..      author='
 00000140: 316c 696e 7427 2c0d 0a20 2020 2020 2061  1lint',..      a
```

