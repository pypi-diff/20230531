# Comparing `tmp/fabric-virt-tools-1.0.0b3.tar.gz` & `tmp/fabric_virt_tools-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-virt-tools-1.0.0b3.tar", last modified: Wed May 31 18:51:38 2023, max compression
+gzip compressed data, was "fabric_virt_tools-1.0.0b4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fabric-virt-tools-1.0.0b3.tar` & `fabric_virt_tools-1.0.0b4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b3/LICENSE
--rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b3/README.md
--rw-r--r--   0        0        0       24 2023-05-31 18:51:26.714254 fabric-virt-tools-1.0.0b3/fabric_virt_tools/__init__.py
--rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric-virt-tools-1.0.0b3/fabric_virt_tools/cpu_tune.py
--rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b3/fabric_virt_tools/numa_tune.py
--rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b3/fabric_virt_tools/utils.py
--rw-r--r--   0        0        0     3706 2023-05-31 18:41:27.926288 fabric-virt-tools-1.0.0b3/fabric_virt_tools/vir_tools_cli.py
--rw-r--r--   0        0        0      960 2023-05-31 18:47:59.135000 fabric-virt-tools-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric_virt_tools-1.0.0b4/LICENSE
+-rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric_virt_tools-1.0.0b4/README.md
+-rw-r--r--   0        0        0       24 2023-05-31 18:53:13.392937 fabric_virt_tools-1.0.0b4/fabric_virt_tools/__init__.py
+-rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric_virt_tools-1.0.0b4/fabric_virt_tools/cpu_tune.py
+-rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric_virt_tools-1.0.0b4/fabric_virt_tools/numa_tune.py
+-rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric_virt_tools-1.0.0b4/fabric_virt_tools/utils.py
+-rw-r--r--   0        0        0     3706 2023-05-31 18:41:27.926288 fabric_virt_tools-1.0.0b4/fabric_virt_tools/vir_tools_cli.py
+-rw-r--r--   0        0        0      960 2023-05-31 18:47:59.135000 fabric_virt_tools-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 fabric_virt_tools-1.0.0b4/PKG-INFO
```

### Comparing `fabric-virt-tools-1.0.0b3/LICENSE` & `fabric_virt_tools-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b3/fabric_virt_tools/cpu_tune.py` & `fabric_virt_tools-1.0.0b4/fabric_virt_tools/cpu_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b3/fabric_virt_tools/numa_tune.py` & `fabric_virt_tools-1.0.0b4/fabric_virt_tools/numa_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b3/fabric_virt_tools/utils.py` & `fabric_virt_tools-1.0.0b4/fabric_virt_tools/utils.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b3/fabric_virt_tools/vir_tools_cli.py` & `fabric_virt_tools-1.0.0b4/fabric_virt_tools/vir_tools_cli.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b3/pyproject.toml` & `fabric_virt_tools-1.0.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b3/PKG-INFO` & `fabric_virt_tools-1.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-virt-tools
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Fabric Aggregate Manager Handlers
 Keywords: Fabric Virtual Machine Tools
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

