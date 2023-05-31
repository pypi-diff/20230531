# Comparing `tmp/fabric-virt-tools-1.0.0b1.tar.gz` & `tmp/fabric-virt-tools-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-virt-tools-1.0.0b1.tar", last modified: Wed May 31 18:44:46 2023, max compression
+gzip compressed data, was "fabric-virt-tools-1.0.0b2.tar", last modified: Wed May 31 18:48:13 2023, max compression
```

## Comparing `fabric-virt-tools-1.0.0b1.tar` & `fabric-virt-tools-1.0.0b2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b1/LICENSE
--rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b1/README.md
--rw-r--r--   0        0        0       24 2023-05-31 18:41:55.153563 fabric-virt-tools-1.0.0b1/fabric_virt_tools/__init__.py
--rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric-virt-tools-1.0.0b1/fabric_virt_tools/cpu_tune.py
--rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b1/fabric_virt_tools/numa_tune.py
--rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b1/fabric_virt_tools/utils.py
--rw-r--r--   0        0        0     3706 2023-05-31 18:41:27.926288 fabric-virt-tools-1.0.0b1/fabric_virt_tools/vir_tools_cli.py
--rw-r--r--   0        0        0      870 2023-05-31 17:30:19.445680 fabric-virt-tools-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b2/README.md
+-rw-r--r--   0        0        0       24 2023-05-31 18:48:05.419991 fabric-virt-tools-1.0.0b2/fabric_virt_tools/__init__.py
+-rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric-virt-tools-1.0.0b2/fabric_virt_tools/cpu_tune.py
+-rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b2/fabric_virt_tools/numa_tune.py
+-rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b2/fabric_virt_tools/utils.py
+-rw-r--r--   0        0        0     3706 2023-05-31 18:41:27.926288 fabric-virt-tools-1.0.0b2/fabric_virt_tools/vir_tools_cli.py
+-rw-r--r--   0        0        0      960 2023-05-31 18:47:59.135000 fabric-virt-tools-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b2/PKG-INFO
```

### Comparing `fabric-virt-tools-1.0.0b1/LICENSE` & `fabric-virt-tools-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b1/fabric_virt_tools/cpu_tune.py` & `fabric-virt-tools-1.0.0b2/fabric_virt_tools/cpu_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b1/fabric_virt_tools/numa_tune.py` & `fabric-virt-tools-1.0.0b2/fabric_virt_tools/numa_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b1/fabric_virt_tools/utils.py` & `fabric-virt-tools-1.0.0b2/fabric_virt_tools/utils.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b1/fabric_virt_tools/vir_tools_cli.py` & `fabric-virt-tools-1.0.0b2/fabric_virt_tools/vir_tools_cli.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b1/pyproject.toml` & `fabric-virt-tools-1.0.0b2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,17 @@
                "License :: OSI Approved :: MIT License",
                "Operating System :: OS Independent"]
 description = "Fabric Aggregate Manager Handlers"
 dynamic = ["version"]
 
 keywords = ["Fabric Virtual Machine Tools"]
 
+
+scripts = {"fabric-virt-tools-cli" = "fabric_virt_tools.virt_tools_cli:virt_tools_cli"}
+
 requires-python = '>=3.6'
 dependencies = [
                 "libvirt-python",
                 "psutil",
                 "click"
                ]
```

### Comparing `fabric-virt-tools-1.0.0b1/PKG-INFO` & `fabric-virt-tools-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-virt-tools
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Fabric Aggregate Manager Handlers
 Keywords: Fabric Virtual Machine Tools
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

