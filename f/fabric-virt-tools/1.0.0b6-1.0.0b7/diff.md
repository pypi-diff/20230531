# Comparing `tmp/fabric-virt-tools-1.0.0b6.tar.gz` & `tmp/fabric-virt-tools-1.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-virt-tools-1.0.0b6.tar", last modified: Wed May 31 20:51:45 2023, max compression
+gzip compressed data, was "fabric-virt-tools-1.0.0b7.tar", last modified: Wed May 31 21:05:27 2023, max compression
```

## Comparing `fabric-virt-tools-1.0.0b6.tar` & `fabric-virt-tools-1.0.0b7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b6/LICENSE
--rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b6/README.md
--rw-r--r--   0        0        0       24 2023-05-31 20:50:50.138436 fabric-virt-tools-1.0.0b6/fabric_virt_tools/__init__.py
--rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric-virt-tools-1.0.0b6/fabric_virt_tools/cpu_tune.py
--rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b6/fabric_virt_tools/numa_tune.py
--rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b6/fabric_virt_tools/utils.py
--rw-r--r--   0        0        0     3838 2023-05-31 19:48:41.435763 fabric-virt-tools-1.0.0b6/fabric_virt_tools/virt_tools_cli.py
--rw-r--r--   0        0        0      954 2023-05-31 19:08:35.841733 fabric-virt-tools-1.0.0b6/pyproject.toml
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b7/LICENSE
+-rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b7/README.md
+-rw-r--r--   0        0        0       24 2023-05-31 21:05:00.042394 fabric-virt-tools-1.0.0b7/fabric_virt_tools/__init__.py
+-rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric-virt-tools-1.0.0b7/fabric_virt_tools/cpu_tune.py
+-rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b7/fabric_virt_tools/numa_tune.py
+-rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b7/fabric_virt_tools/utils.py
+-rw-r--r--   0        0        0     3838 2023-05-31 19:48:41.435763 fabric-virt-tools-1.0.0b7/fabric_virt_tools/virt_tools_cli.py
+-rw-r--r--   0        0        0      955 2023-05-31 21:04:53.032899 fabric-virt-tools-1.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b7/PKG-INFO
```

### Comparing `fabric-virt-tools-1.0.0b6/LICENSE` & `fabric-virt-tools-1.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b6/fabric_virt_tools/cpu_tune.py` & `fabric-virt-tools-1.0.0b7/fabric_virt_tools/cpu_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b6/fabric_virt_tools/numa_tune.py` & `fabric-virt-tools-1.0.0b7/fabric_virt_tools/numa_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b6/fabric_virt_tools/utils.py` & `fabric-virt-tools-1.0.0b7/fabric_virt_tools/utils.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b6/fabric_virt_tools/virt_tools_cli.py` & `fabric-virt-tools-1.0.0b7/fabric_virt_tools/virt_tools_cli.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b6/pyproject.toml` & `fabric-virt-tools-1.0.0b7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                "Operating System :: OS Independent"]
 description = "Fabric Virtual Machine Tools"
 dynamic = ["version"]
 
 keywords = ["Fabric Virtual Machine Tools"]
 
 
-scripts = {"fabric-virt-tools-cli" = "fabric_virt_tools.virt_tools_cli:vir_tools_cli"}
+scripts = {"fabric-virt-tools-cli" = "fabric_virt_tools.virt_tools_cli:virt_tools_cli"}
 
 requires-python = '>=3.6'
 dependencies = [
                 "libvirt-python",
                 "psutil",
                 "click"
                ]
```

### Comparing `fabric-virt-tools-1.0.0b6/PKG-INFO` & `fabric-virt-tools-1.0.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-virt-tools
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: Fabric Virtual Machine Tools
 Keywords: Fabric Virtual Machine Tools
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

