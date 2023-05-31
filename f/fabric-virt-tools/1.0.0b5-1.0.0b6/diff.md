# Comparing `tmp/fabric-virt-tools-1.0.0b5.tar.gz` & `tmp/fabric-virt-tools-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-virt-tools-1.0.0b5.tar", last modified: Wed May 31 18:59:34 2023, max compression
+gzip compressed data, was "fabric-virt-tools-1.0.0b6.tar", last modified: Wed May 31 20:51:45 2023, max compression
```

## Comparing `fabric-virt-tools-1.0.0b5.tar` & `fabric-virt-tools-1.0.0b6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b5/LICENSE
--rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b5/README.md
--rw-r--r--   0        0        0       24 2023-05-31 18:59:21.250276 fabric-virt-tools-1.0.0b5/fabric_virt_tools/__init__.py
--rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric-virt-tools-1.0.0b5/fabric_virt_tools/cpu_tune.py
--rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b5/fabric_virt_tools/numa_tune.py
--rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b5/fabric_virt_tools/utils.py
--rw-r--r--   0        0        0     3706 2023-05-31 18:41:27.926288 fabric-virt-tools-1.0.0b5/fabric_virt_tools/vir_tools_cli.py
--rw-r--r--   0        0        0      959 2023-05-31 18:59:17.779498 fabric-virt-tools-1.0.0b5/pyproject.toml
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 18:44:31.383234 fabric-virt-tools-1.0.0b6/LICENSE
+-rw-r--r--   0        0        0      279 2023-05-31 18:44:17.271476 fabric-virt-tools-1.0.0b6/README.md
+-rw-r--r--   0        0        0       24 2023-05-31 20:50:50.138436 fabric-virt-tools-1.0.0b6/fabric_virt_tools/__init__.py
+-rw-r--r--   0        0        0     8485 2023-05-31 17:54:08.507450 fabric-virt-tools-1.0.0b6/fabric_virt_tools/cpu_tune.py
+-rw-r--r--   0        0        0    12229 2023-05-31 18:39:32.027641 fabric-virt-tools-1.0.0b6/fabric_virt_tools/numa_tune.py
+-rw-r--r--   0        0        0     1559 2023-05-31 17:39:04.855580 fabric-virt-tools-1.0.0b6/fabric_virt_tools/utils.py
+-rw-r--r--   0        0        0     3838 2023-05-31 19:48:41.435763 fabric-virt-tools-1.0.0b6/fabric_virt_tools/virt_tools_cli.py
+-rw-r--r--   0        0        0      954 2023-05-31 19:08:35.841733 fabric-virt-tools-1.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 fabric-virt-tools-1.0.0b6/PKG-INFO
```

### Comparing `fabric-virt-tools-1.0.0b5/LICENSE` & `fabric-virt-tools-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b5/fabric_virt_tools/cpu_tune.py` & `fabric-virt-tools-1.0.0b6/fabric_virt_tools/cpu_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b5/fabric_virt_tools/numa_tune.py` & `fabric-virt-tools-1.0.0b6/fabric_virt_tools/numa_tune.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b5/fabric_virt_tools/utils.py` & `fabric-virt-tools-1.0.0b6/fabric_virt_tools/utils.py`

 * *Files identical despite different names*

### Comparing `fabric-virt-tools-1.0.0b5/fabric_virt_tools/vir_tools_cli.py` & `fabric-virt-tools-1.0.0b6/fabric_virt_tools/virt_tools_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 #
 import json
+import traceback
 from typing import List, Dict
 
 import click
 
 from fabric_virt_tools.cpu_tune import CpuTune
 from fabric_virt_tools.numa_tune import NumaTune
 
 
 @click.group()
 @click.option('-v', '--verbose', is_flag=True)
 @click.pass_context
-def vir_tools_cli(ctx, verbose):
+def virt_tools_cli(ctx, verbose):
     ctx.ensure_object(dict)
     ctx.obj['VERBOSE'] = verbose
 
 
 @click.group()
 @click.pass_context
 def cpu(ctx):
@@ -55,29 +56,31 @@
     """ Query CPU Info for VM Guest and relevant host information as well
     """
     try:
         cpu_tune = CpuTune()
         cpu_info = cpu_tune.info(domain_name=domain_name)
         print(json.dumps(cpu_info))
     except Exception as e:
-        raise click.ClickException(f"vir_tools_cli: {e}")
+        traceback.print_exc()
+        raise click.ClickException(f"virt_tools_cli: {e}")
 
 
 @cpu.command()
 @click.option('--domain_name', help='Virtual Guest Domain Name', required=True)
 @click.option('--vcpu_cpu_map', help='Virtual CPU to Host Cpu Map', required=True)
 @click.pass_context
 def tune(ctx, domain_name: str, vcpu_cpu_map: List[Dict[str, str]]):
     """ Query CPU Info for VM Guest and relevant host information as well
     """
     try:
         cpu_tune = CpuTune()
         cpu_tune.vcpu_pin(domain_name=domain_name, vcpu_cpu_map=vcpu_cpu_map)
     except Exception as e:
-        raise click.ClickException(f"vir_tools_cli: {e}")
+        traceback.print_exc()
+        raise click.ClickException(f"virt_tools_cli: {e}")
 
 
 @click.group()
 @click.pass_context
 def numa(ctx):
     """ Numa Tuning
     """
@@ -90,26 +93,28 @@
     """ Query Numa Info for VM Guest and relevant host information as well
     """
     try:
         numa_tune = NumaTune()
         numa_info = numa_tune.info(domain_name=domain_name)
         print(json.dumps(numa_info))
     except Exception as e:
-        raise click.ClickException(f"vir_tools_cli: {e}")
+        traceback.print_exc()
+        raise click.ClickException(f"virt_tools_cli: {e}")
 
 
 @numa.command()
 @click.option('--domain_name', help='Virtual Guest Domain Name', required=True)
 @click.option('--node_set', help='List of the nodes to be assigned', required=True)
 @click.pass_context
 def tune(ctx, domain_name: str, node_set: List[str]):
     """ Pin Numa Node to the VM Guest
     """
     try:
         numa_tune = NumaTune()
-        numa_info = numa_tune.numa_tune(domain_name=domain_name, node_set=node_set)
+        numa_tune.numa_tune(domain_name=domain_name, node_set=node_set)
     except Exception as e:
-        raise click.ClickException(f"vir_tools_cli: {e}")
+        traceback.print_exc()
+        raise click.ClickException(f"virt_tools_cli: {e}")
 
 
-vir_tools_cli.add_command(cpu)
-vir_tools_cli.add_command(numa)
+virt_tools_cli.add_command(cpu)
+virt_tools_cli.add_command(numa)
```

### Comparing `fabric-virt-tools-1.0.0b5/pyproject.toml` & `fabric-virt-tools-1.0.0b6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "fabric-virt-tools"
 authors = [{name="Komal Thareja", email="kthare10@renci.org"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["Programming Language :: Python :: 3",
                "License :: OSI Approved :: MIT License",
                "Operating System :: OS Independent"]
-description = "Fabric Aggregate Manager Handlers"
+description = "Fabric Virtual Machine Tools"
 dynamic = ["version"]
 
 keywords = ["Fabric Virtual Machine Tools"]
 
 
 scripts = {"fabric-virt-tools-cli" = "fabric_virt_tools.virt_tools_cli:vir_tools_cli"}
```

### Comparing `fabric-virt-tools-1.0.0b5/PKG-INFO` & `fabric-virt-tools-1.0.0b6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fabric-virt-tools
-Version: 1.0.0b5
-Summary: Fabric Aggregate Manager Handlers
+Version: 1.0.0b6
+Summary: Fabric Virtual Machine Tools
 Keywords: Fabric Virtual Machine Tools
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

