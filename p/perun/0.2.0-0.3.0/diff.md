# Comparing `tmp/perun-0.2.0.tar.gz` & `tmp/perun-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun-0.2.0.tar", max compression
+gzip compressed data, was "perun-0.3.0.tar", max compression
```

## Comparing `perun-0.2.0.tar` & `perun-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1527 2023-03-28 10:16:42.052420 perun-0.2.0/LICENSE
--rw-r--r--   0        0        0     7909 2023-03-28 10:16:42.052420 perun-0.2.0/README.md
--rw-r--r--   0        0        0      319 2023-03-28 10:16:42.808419 perun-0.2.0/perun/__init__.py
--rw-r--r--   0        0        0       88 2023-03-28 10:16:42.052420 perun-0.2.0/perun/__main__.py
--rw-r--r--   0        0        0      190 2023-03-28 10:16:42.052420 perun-0.2.0/perun/backend/__init__.py
--rw-r--r--   0        0        0     1963 2023-03-28 10:16:42.052420 perun-0.2.0/perun/backend/backend.py
--rw-r--r--   0        0        0     7894 2023-03-28 10:16:42.052420 perun-0.2.0/perun/backend/intel_rapl.py
--rw-r--r--   0        0        0     3401 2023-03-28 10:16:42.052420 perun-0.2.0/perun/backend/nvml.py
--rw-r--r--   0        0        0     4435 2023-03-28 10:16:42.052420 perun-0.2.0/perun/backend/psutil.py
--rw-r--r--   0        0        0     6785 2023-03-28 10:16:42.052420 perun-0.2.0/perun/cli.py
--rw-r--r--   0        0        0     1992 2023-03-28 10:16:42.052420 perun-0.2.0/perun/comm.py
--rw-r--r--   0        0        0     2715 2023-03-28 10:16:42.052420 perun-0.2.0/perun/configuration.py
--rw-r--r--   0        0        0     3793 2023-03-28 10:16:42.052420 perun-0.2.0/perun/coordination.py
--rw-r--r--   0        0        0       26 2023-03-28 10:16:42.052420 perun-0.2.0/perun/data_model/__init__.py
--rw-r--r--   0        0        0     7213 2023-03-28 10:16:42.052420 perun-0.2.0/perun/data_model/data.py
--rw-r--r--   0        0        0     1943 2023-03-28 10:16:42.052420 perun-0.2.0/perun/data_model/measurement_type.py
--rw-r--r--   0        0        0      988 2023-03-28 10:16:42.052420 perun-0.2.0/perun/data_model/sensor.py
--rw-r--r--   0        0        0      837 2023-03-28 10:16:42.052420 perun-0.2.0/perun/decorator.py
--rw-r--r--   0        0        0       21 2023-03-28 10:16:42.052420 perun-0.2.0/perun/extras/__init__.py
--rw-r--r--   0        0        0     1863 2023-03-28 10:16:42.052420 perun-0.2.0/perun/extras/horeka.py
--rw-r--r--   0        0        0       18 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/__init__.py
--rw-r--r--   0        0        0     1516 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/bench.py
--rw-r--r--   0        0        0     6458 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/hdf5.py
--rw-r--r--   0        0        0     4352 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/io.py
--rw-r--r--   0        0        0     1414 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/json.py
--rw-r--r--   0        0        0     2612 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/pandas.py
--rw-r--r--   0        0        0      536 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/pickle.py
--rw-r--r--   0        0        0     3061 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/text_report.py
--rw-r--r--   0        0        0      889 2023-03-28 10:16:42.052420 perun-0.2.0/perun/io/yaml.py
--rw-r--r--   0        0        0      828 2023-03-28 10:16:42.052420 perun-0.2.0/perun/logging.py
--rw-r--r--   0        0        0    12299 2023-03-28 10:16:42.052420 perun-0.2.0/perun/perun.py
--rw-r--r--   0        0        0     7107 2023-03-28 10:16:42.052420 perun-0.2.0/perun/processing.py
--rw-r--r--   0        0        0     2857 2023-03-28 10:16:42.052420 perun-0.2.0/perun/util.py
--rw-r--r--   0        0        0     1557 2023-03-28 10:16:42.812419 perun-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8792 1970-01-01 00:00:00.000000 perun-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-05-31 09:51:29.914219 perun-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8486 2023-05-31 09:51:29.914219 perun-0.3.0/README.md
+-rw-r--r--   0        0        0      319 2023-05-31 09:51:30.662215 perun-0.3.0/perun/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-31 09:51:29.918220 perun-0.3.0/perun/__main__.py
+-rw-r--r--   0        0        0      190 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/__init__.py
+-rw-r--r--   0        0        0     1963 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/backend.py
+-rw-r--r--   0        0        0     7426 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/intel_rapl.py
+-rw-r--r--   0        0        0     3401 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/nvml.py
+-rw-r--r--   0        0        0     4435 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/psutil.py
+-rw-r--r--   0        0        0     7550 2023-05-31 09:51:29.918220 perun-0.3.0/perun/cli.py
+-rw-r--r--   0        0        0     1992 2023-05-31 09:51:29.918220 perun-0.3.0/perun/comm.py
+-rw-r--r--   0        0        0     3044 2023-05-31 09:51:29.918220 perun-0.3.0/perun/configuration.py
+-rw-r--r--   0        0        0     3793 2023-05-31 09:51:29.918220 perun-0.3.0/perun/coordination.py
+-rw-r--r--   0        0        0       26 2023-05-31 09:51:29.918220 perun-0.3.0/perun/data_model/__init__.py
+-rw-r--r--   0        0        0     7136 2023-05-31 09:51:29.918220 perun-0.3.0/perun/data_model/data.py
+-rw-r--r--   0        0        0     1900 2023-05-31 09:51:29.918220 perun-0.3.0/perun/data_model/measurement_type.py
+-rw-r--r--   0        0        0      988 2023-05-31 09:51:29.918220 perun-0.3.0/perun/data_model/sensor.py
+-rw-r--r--   0        0        0      878 2023-05-31 09:51:29.918220 perun-0.3.0/perun/decorator.py
+-rw-r--r--   0        0        0       21 2023-05-31 09:51:29.918220 perun-0.3.0/perun/extras/__init__.py
+-rw-r--r--   0        0        0     1863 2023-05-31 09:51:29.918220 perun-0.3.0/perun/extras/horeka.py
+-rw-r--r--   0        0        0       18 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/__init__.py
+-rw-r--r--   0        0        0     1544 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/bench.py
+-rw-r--r--   0        0        0     6458 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/hdf5.py
+-rw-r--r--   0        0        0     4384 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/io.py
+-rw-r--r--   0        0        0     1414 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/json.py
+-rw-r--r--   0        0        0     2612 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/pandas.py
+-rw-r--r--   0        0        0      536 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/pickle.py
+-rw-r--r--   0        0        0     3983 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/text_report.py
+-rw-r--r--   0        0        0      828 2023-05-31 09:51:29.918220 perun-0.3.0/perun/logging.py
+-rw-r--r--   0        0        0    12299 2023-05-31 09:51:29.918220 perun-0.3.0/perun/perun.py
+-rw-r--r--   0        0        0     7107 2023-05-31 09:51:29.918220 perun-0.3.0/perun/processing.py
+-rw-r--r--   0        0        0     4189 2023-05-31 09:51:29.918220 perun-0.3.0/perun/util.py
+-rw-r--r--   0        0        0     1873 2023-05-31 09:51:30.662215 perun-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9410 1970-01-01 00:00:00.000000 perun-0.3.0/PKG-INFO
```

### Comparing `perun-0.2.0/LICENSE` & `perun-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/README.md` & `perun-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 <div align="center">
-  <img src="https://raw.githubusercontent.com/Helmholtz-AI-Energy/perun/main/docs/images/perun.svg">
+  <img src="https://raw.githubusercontent.com/Helmholtz-AI-Energy/perun/main/docs/images/full_logo.svg">
 </div>
 
-Have you ever wondered how much energy is used when training your neural network on the MNIST dataset? Want to get scared because of impact you are having on the evironment while doing "valuable" research? Are you interested in knowing how much carbon you are burning playing with DALL-E just to get attention on twitter? If the thing that was missing from your machine learning workflow was existential dread, this is the correct package for you!
+&nbsp;
+&nbsp;
 
-perun is python package that calculates the energy consumption of your python scripts by sampling usage statistics from Intel RAPL, Nvidia-NVML and *psutil*. Unlike other energy measuring applications out there, this is the only one capable of handling MPI applications, being capable of gathering data from 100s of nodes at the same time, and accumulating it efficiently. This is posible without adding any line of code into your existing application, and without meaningfully extending the runtime of your application.
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B-orange)](https://fair-software.eu)
+![PyPI](https://img.shields.io/pypi/v/perun)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/perun)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![Documentation Status](https://readthedocs.org/projects/perun/badge/?version=latest)](https://perun.readthedocs.io/en/latest/?badge=latest)
+
+perun is a Python package that calculates the energy consumption of Python scripts by sampling usage statistics from Intel RAPL, Nvidia-NVML, and psutil. It can handle MPI applications, gather data from hundreds of nodes, and accumulate it efficiently. perun can be used as a command-line tool or as a function decorator in Python scripts.
+
+Check out the [docs](https://perun.readthedocs.io/en/latest/)!
+
+## Key Features
+
+ - Measures energy consumption of Python scripts using Intel RAPL, Nvidia-NVML, and psutil
+ - Handles MPI applications efficiently
+ - Gathers data from hundreds of nodes and accumulates it efficiently
+ - Can be used as a command-line tool or as a function decorator in Python scripts
 
 ## Installation
 
 From PyPI:
 
 ```console
 pip install perun
@@ -18,50 +36,55 @@
 
 ```console
 pip install git+https://github.com/Helmholtz-AI-Energy/perun
 ```
 
 ## Quick Start
 
-Perun has two usage methods, either using the command line, or using function decorators.
+### Command Line
 
-### Command line
-
-When using the command line, perun will output file containing runtime, energy and other information gathered while your script runs.
+To use perun as a command-line tool, run the monitor subcommand followed by the path to your Python script and its arguments:
 
 ```console
 $ perun monitor path/to/your/script.py [args]
-$ cat perun_results/script_2023-03-23T12:10:48.627214.txt
+```
+
+perun will output a file containing runtime, energy, and other information gathered while your script runs:
+
+
+```console
 PERUN REPORT
 
 App name: script
 Run ID: 2023-03-23T12:10:48.627214
 RUNTIME: 0:00:06.333626 s
 CPU_UTIL: 64.825 %
 MEM_UTIL: 0.563 %
 NET_READ: 1.401 kB
 NET_WRITE: 1.292 kB
 DISK_READ: 174.633 MB
 DISK_WRITE: 88.000 kB
+
 ```
 
-### Decorator
+### Function Decorator
 
-Perun can also monitor individual functions using a decorator:
+To use perun as a function decorator in your Python script, import the monitor decorator and add it to the function you want to monitor:
 
 ```python
+
 import time
 from perun.decorator import monitor
 
 @monitor()
-def your_sleep_function(n: int):
+def your_function(n: int):
     time.sleep(n)
 ```
 
-And then running your script like always:
+When you run your script, perun will output a report from the function:
 
 ```console
 python path/to/your/script.py
 ```
 
 > :exclamation: Each time the function is run, perun will output a new report from the function.
```

### Comparing `perun-0.2.0/perun/backend/backend.py` & `perun-0.3.0/perun/backend/backend.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/backend/intel_rapl.py` & `perun-0.3.0/perun/backend/intel_rapl.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,28 +34,18 @@
         """Init IntelRAPLBackend."""
         super().__init__()
         log.info("Initialized Intel RAPL")
 
     def setup(self):
         """Check Intel RAPL access."""
         cpuInfo = cpuinfo.get_cpu_info()
-        self.metadata = {
-            "vendor_id": cpuInfo["vendor_id_raw"],
-            "brand": cpuInfo["brand_raw"],
-            "arch": cpuInfo["arch_string_raw"],
-            "hz_advertised": cpuInfo["hz_advertised_friendly"],
-            "hz_actual": cpuInfo["hz_actual_friendly"],
-            "l1_data_cache_size": cpuInfo["l1_data_cache_size"],
-            "l1_instruction_cache_size": cpuInfo["l1_instruction_cache_size"],
-            "l2_cache_size": cpuInfo["l2_cache_size"],
-            "l2_cache_line_size": cpuInfo["l2_cache_line_size"],
-            "l2_cache_associativity": cpuInfo["l2_cache_associativity"],
-            "l3_cache_size": cpuInfo["l3_cache_size"],
-            "source": "Intel RAPL",
-        }
+        self.metadata = {}
+        for key, value in cpuInfo.items():
+            self.metadata[key] = value
+
         log.debug(f"CPU info metadata: {self.metadata}")
 
         raplPath = Path(RAPL_PATH)
 
         def getCallback(file: IOBase) -> Callable[[], np.number]:
             def func() -> np.number:
                 file.seek(0)
@@ -64,14 +54,15 @@
             return func
 
         if not raplPath.exists():
             raise ImportWarning("No powercap interface")
 
         self._files = []
         packageDevices = []
+        packageFiles = []
         foundPsys = False
         for child in raplPath.iterdir():
             log.debug(child)
             match = re.match(DIR_RGX, child.name)
             if match:
                 if os.access(child / "energy_uj", os.R_OK):
                     socket = match.groups()[0]
@@ -114,27 +105,29 @@
                             dataType,
                             getCallback(energy_file),
                         )
 
                         self.devices[device.id] = device
                         if "package" in device_name:
                             packageDevices.append(device)
+                            packageFiles.append(energy_file)
 
                         for grandchild in child.iterdir():
                             match = re.match(SUBDIR_RGX, grandchild.name)
                             if match:
                                 with open(grandchild / "name", "r") as file:
                                     device_name = file.readline().strip()
+
                                 if "dram" in device_name:
                                     devType = DeviceType.RAM
                                 elif "package" in device_name:
                                     devType = DeviceType.CPU
-                                elif "psys" in device_name:
-                                    devType = DeviceType.CPU
-                                    foundPsys = True
+                                # elif "psys" in device_name:
+                                #     devType = DeviceType.CPU
+                                #     foundPsys = True
                                 else:
                                     devType = DeviceType.OTHER
 
                                 if devType != DeviceType.OTHER:
                                     with open(
                                         child / "max_energy_range_uj", "r"
                                     ) as file:
@@ -162,15 +155,16 @@
                                     log.debug(device)
                                     self.devices[device.id] = device
 
                                     if "package" in device_name:
                                         packageDevices.append(device)
 
         if foundPsys:
-            for pkg in packageDevices:
+            for pkg, file in zip(packageDevices, packageFiles):
+                file.close()
                 del self.devices[pkg.id]
 
         log.debug(f"IntelRapl devices {self.devices}")
 
     def close(self) -> None:
         """Backend shutdown code (does nothing for intel rapl)."""
         log.debug("Closing files")
```

### Comparing `perun-0.2.0/perun/backend/nvml.py` & `perun-0.3.0/perun/backend/nvml.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/backend/psutil.py` & `perun-0.3.0/perun/backend/psutil.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/cli.py` & `perun-0.3.0/perun/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Command line api definition.
 
 Uses click https://click.palletsprojects.com/en/8.1.x/ to manage complex cmdline configurations.
 """
 from pathlib import Path
+from typing import Dict, List, Optional
 
 import click
 
 import perun
 from perun import log
 from perun.configuration import config, read_custom_config, save_to_config_callback
 from perun.io.io import IOFormat, exportTo, importFrom
+from perun.util import getHostMetadata
 
 
 @click.group()
 @click.version_option(version=perun.__version__)
 @click.option(
     "-c",
     "--configuration",
@@ -51,15 +53,15 @@
     type=click.Path(exists=False, dir_okay=True, file_okay=False),
     help="Where to save the output files, defaults to the current working directory.",
     callback=save_to_config_callback,
     expose_value=False,
 )
 @click.option(
     "--raw",
-    default=False,
+    default=True,
     help="Use the flag '--raw' if you need access to all the raw data collected by perun. The output will be saved on an hdf5 file on the perun data output location.",
     is_flag=True,
     callback=save_to_config_callback,
     expose_value=False,
 )
 # Sampling Options
 @click.option(
@@ -153,36 +155,59 @@
         config.read_dict(_default_config)
         config.write(sys.stdout)
     else:
         config.write(sys.stdout)
 
 
 @cli.command()
-def sensors():
+@click.option(
+    "-v",
+    "--verbose",
+    is_flag=True,
+    default=False,
+    help="Print all the available system information in json format.",
+)
+def sensors(verbose: bool):
     """Print sensors assigned to each rank by perun."""
     from perun import COMM_WORLD
     from perun.backend import backends
     from perun.coordination import getGlobalSensorRankConfiguration
 
     globalHostRank, globalSensorConfig = getGlobalSensorRankConfiguration(
         COMM_WORLD, backends
     )
-    if COMM_WORLD.Get_rank() == 0:
-        for rank, bes in enumerate(globalSensorConfig):
-            click.echo(f"Rank: {rank}")
-            for key, items in bes.items():
-                if len(items) > 0:
-                    click.echo(f"   {key}:")
-                    for device in items:
-                        click.echo(f"       {device}")
-                    click.echo("")
-
-        click.echo("Hostnames: ")
-        for host, ranks in globalHostRank.items():
-            click.echo(f"   {host}: {ranks}")
+
+    if verbose:
+        import json
+        import sys
+
+        hostMD = getHostMetadata(globalSensorConfig[0])
+        allHostsMD: Optional[List[Dict]] = COMM_WORLD.gather(hostMD, root=0)
+
+        if COMM_WORLD.Get_rank() == 0 and allHostsMD:
+            metadataDict = {}
+            for host, assignedRanks in globalHostRank.items():
+                metadataDict[host] = allHostsMD[assignedRanks[0]]
+
+            json.dump(metadataDict, sys.stdout, indent=4)
+
+    else:
+        if COMM_WORLD.Get_rank() == 0:
+            for rank, bes in enumerate(globalSensorConfig):
+                click.echo(f"Rank: {rank}")
+                for key, items in bes.items():
+                    if len(items) > 0:
+                        click.echo(f"   {key}:")
+                        for device in items:
+                            click.echo(f"       {device}")
+                        click.echo("")
+
+            click.echo("Hostnames: ")
+            for host, ranks in globalHostRank.items():
+                click.echo(f"   {host}: {ranks}")
 
     for b in backends:
         b.close()
 
 
 @cli.command()
 @click.argument("input_file", type=click.Path(exists=True))
```

### Comparing `perun-0.2.0/perun/comm.py` & `perun-0.3.0/perun/comm.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/configuration.py` & `perun-0.3.0/perun/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Configuration module."""
-# kgCO2eq/kWh - source https://www.nowtricity.com/country/germany/
-# cent/kWh (Euro) - source: https://www.stromauskunft.de/strompreise/ Baden-Württemberg lokare anbieter
-
+# gCO2eq/kWh - source: https://ourworldindata.org/grapher/carbon-intensity-electricity Global Average
+# cent/kWh (Euro) - source: https://www.stromauskunft.de/strompreise/ 03.05.2023
 import configparser
+import os
 from pathlib import Path
 from typing import Any, Mapping, Optional, Union
 
 import click
 
 _default_config: Mapping[str, Mapping[str, Any]] = {
     "post-processing": {
         "pue": 1.58,
-        "emissions_factor": 0.262,  # gCO2eq/kWh
-        "price_factor": 34.60,  # Cent/kWh
+        "emissions_factor": 417.80,  # gCO2eq/kWh
+        "price_factor": 32.51,  # Cent/kWh
     },
     "monitor": {
-        "sampling_rate": 1,
+        "sampling_rate": 5,
     },
     "output": {
         "app_name": None,
         "run_id": None,
-        "format": "text",
+        "format": "pickle",
         "data_out": "./perun_results",
         "depth": None,
-        "raw": False,
+        "raw": True,
     },
     "benchmarking": {
         "bench_enable": False,
         "bench_rounds": 10,
         "bench_warmup_rounds": 1,
         # "bench_metrics": ["ENERGY", "RUNTIME"],
     },
@@ -85,7 +85,16 @@
     Args:
         key (str): Option name
         value (Any): New option value
     """
     for section in config.sections():
         if config.has_option(section, key):
             config.set(section, key, str(value))
+
+
+def read_environ():
+    """Read perun environmental variables."""
+    for section, subconf in _default_config.items():
+        for option in subconf.keys():
+            envvar = f"PERUN_{option.upper()}"
+            if envvar in os.environ:
+                config.set(section, option, os.environ[envvar])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `perun-0.2.0/perun/coordination.py` & `perun-0.3.0/perun/coordination.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/data_model/data.py` & `perun-0.3.0/perun/data_model/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Storage Module."""
 import dataclasses
 import enum
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
-from typing_extensions import Self
 
 from perun import log
 from perun.data_model.measurement_type import MetricMetaData
 from perun.data_model.sensor import DeviceType
 
 
 class NodeType(enum.Enum):
@@ -51,15 +50,15 @@
 
     type: MetricType
     value: np.number
     metric_md: MetricMetaData
     agg: AggregateType
 
     @classmethod
-    def fromDict(cls, metricDict: Dict) -> Self:
+    def fromDict(cls, metricDict: Dict):
         """Create RawData object from a dictionary."""
         return cls(
             MetricType(metricDict["type"]),
             np.float32(metricDict["value"]),
             MetricMetaData.fromDict(metricDict["metric_md"]),
             AggregateType(metricDict["agg"]),
         )
@@ -73,15 +72,15 @@
     metric_md: MetricMetaData
     mean: np.number
     std: np.number
     max: np.number
     min: np.number
 
     @classmethod
-    def fromMetrics(cls, metrics: List[Metric]) -> Self:
+    def fromMetrics(cls, metrics: List[Metric]):
         """Create a stats object based on the metric's values."""
         type = metrics[0].type
         metric_md = metrics[0].metric_md
 
         for m in metrics:
             if m.type != type:
                 log.error("Metrics given to Stats class do not match")
@@ -100,15 +99,15 @@
         Value property.
 
         For compatibility with Metric dataclass.
         """
         return self.mean
 
     @classmethod
-    def fromDict(cls, statsDict: Dict) -> Self:
+    def fromDict(cls, statsDict: Dict):
         """Stats constructor from a dictionory."""
         return cls(
             MetricType(statsDict["type"]),
             MetricMetaData.fromDict(statsDict["metric_md"]),
             statsDict["mean"],
             statsDict["std"],
             statsDict["max"],
@@ -122,15 +121,15 @@
 
     timesteps: np.ndarray
     values: np.ndarray
     t_md: MetricMetaData
     v_md: MetricMetaData
 
     @classmethod
-    def fromDict(cls, rawDataDict: Dict) -> Self:
+    def fromDict(cls, rawDataDict: Dict):
         """Create RawData object from a dictionary."""
         t_md = MetricMetaData.fromDict(rawDataDict["t_md"])
         v_md = MetricMetaData.fromDict(rawDataDict["v_md"])
         return cls(
             np.array(rawDataDict["timesteps"], dtype=t_md.dtype),
             np.array(rawDataDict["values"], dtype=t_md.dtype),
             t_md,
@@ -142,15 +141,15 @@
     """Recursive data structure that contains all the information of a monitored application."""
 
     def __init__(
         self,
         id: str,
         type: NodeType,
         metadata: Dict,
-        nodes: Optional[Dict[str, Self]] = None,
+        nodes: Optional[Dict[str, Any]] = None,
         metrics: Optional[Dict[MetricType, Union[Metric, Stats]]] = None,
         deviceType: Optional[DeviceType] = None,
         raw_data: Optional[RawData] = None,
         processed: bool = False,
     ) -> None:
         """DataNode.
 
@@ -160,15 +159,15 @@
             metadata (Dict): Metadata
             nodes (Dict[str, Self], optional): Child DataNodes. Defaults to {}.
             raw_data (Optional[RawData], optional): If sensor, contains raw sensor values. Defaults to None.
         """
         self.id = id
         self.type = type
         self.metadata: Dict[str, Any] = metadata
-        self.nodes: Dict[str, Self] = nodes if nodes else {}
+        self.nodes: Dict[str, Any] = nodes if nodes else {}
         self.metrics: Dict[MetricType, Union[Metric, Stats]] = (
             metrics if metrics else {}
         )
         self.deviceType: Optional[DeviceType] = deviceType
         self.raw_data: Optional[RawData] = raw_data
         self.processed = processed
 
@@ -204,15 +203,15 @@
 
         if include_raw_data and self.raw_data:
             resultsDict["raw_data"] = dataclasses.asdict(self.raw_data)
 
         return resultsDict
 
     @classmethod
-    def fromDict(cls, resultsDict: Dict) -> Self:
+    def fromDict(cls, resultsDict: Dict):
         """Build object from dictionary."""
         type = NodeType(resultsDict["type"])
         newResults = cls(
             id=resultsDict["id"],
             type=type,
             metadata=resultsDict["metadata"],
             nodes={
```

### Comparing `perun-0.2.0/perun/data_model/measurement_type.py` & `perun-0.3.0/perun/data_model/measurement_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Unit module."""
 import dataclasses
 import enum
 from typing import Dict
 
 import numpy as np
-from typing_extensions import Self
 
 
 class Unit(str, enum.Enum):
     """Unit enum."""
 
     JOULE = "J"
     WATT = "W"
@@ -76,15 +75,15 @@
     mag: Magnitude
     dtype: np.dtype
     min: np.number
     max: np.number
     fill: np.number
 
     @classmethod
-    def fromDict(cls, mdDict: Dict) -> Self:
+    def fromDict(cls, mdDict: Dict):
         """Create MetricMetadata from a dictionary."""
         dtype = np.dtype(mdDict["dtype"])
         return cls(
             Unit(mdDict["unit"]),
             Magnitude(mdDict["mag"]),
             dtype,
             dtype.type(mdDict["min"]),
```

### Comparing `perun-0.2.0/perun/data_model/sensor.py` & `perun-0.3.0/perun/data_model/sensor.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/decorator.py` & `perun-0.3.0/perun/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Decorator module."""
 
 import functools
 
 from perun import config, log
-from perun.configuration import read_custom_config, save_to_config
+from perun.configuration import read_custom_config, read_environ, save_to_config
 from perun.perun import monitor_application
 
 
 def monitor(
     configuration: str = "./.perun.ini",
     **conf_kwargs,
 ):
     """Decorate function to monitor its energy usage."""
 
     def inner_function(func):
         @functools.wraps(func)
         def func_wrapper(*args, **kwargs):
             # Get custom config and kwargs
-
             read_custom_config(None, None, configuration)
             for key, value in conf_kwargs.items():
                 save_to_config(key, value)
 
+            read_environ()
             log.setLevel(f"{config.get('debug', 'log_lvl')}")
+
             func_result = monitor_application(func, args, kwargs)
 
             return func_result
 
         return func_wrapper
 
     return inner_function
```

### Comparing `perun-0.2.0/perun/extras/horeka.py` & `perun-0.3.0/perun/extras/horeka.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/io/bench.py` & `perun-0.3.0/perun/io/bench.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,23 +23,23 @@
         if metricType in lessIsBetterMetrics:
             metric_md = metric.metric_md
             value, tfactor, mag = value2str(metric.value, metric_md)
 
             if isinstance(metric, Stats):
                 metricDict.append(
                     {
-                        "name": f"{dataNode.metadata['app_name']} - {metricType.name}",
+                        "name": f"{dataNode.metadata['app_name']}_{dataNode.id} - {metricType.name}",
                         "unit": f"{mag.symbol}{metric_md.unit.symbol}",
                         "value": metric.mean / tfactor,
                         "range": metric.std / tfactor,
                     }
                 )
             else:
                 metricDict.append(
                     {
-                        "name": f"{dataNode.metadata['app_name']} - {metricType.name}",
+                        "name": f"{dataNode.metadata['app_name']}_{dataNode.id} - {metricType.name}",
                         "unit": f"{mag.symbol}{metric_md.unit.symbol}",
                         "value": metric.value / tfactor,
                     }
                 )
 
     return json.dumps(metricDict, indent=4)
```

### Comparing `perun-0.2.0/perun/io/hdf5.py` & `perun-0.3.0/perun/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/io/io.py` & `perun-0.3.0/perun/io/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from perun.io.json import exportJson, importJson
 from perun.io.pandas import exportCSV
 from perun.io.pickle import exportPickle, importPickle
 from perun.io.text_report import textReport
 
 _suffixes = {
     "text": "txt",
-    "yaml": "yaml",
     "json": "json",
     "hdf5": "hdf5",
     "pickle": "pkl",
     "csv": "csv",
     "bench": "json",
 }
 
@@ -29,15 +28,14 @@
 
     TEXT = "text"
     JSON = "json"
     HDF5 = "hdf5"
     PICKLE = "pickle"
     CSV = "csv"
     BENCH = "bench"
-    # YAML = "yaml"
 
     @property
     def suffix(self):
         """Return file suffix from format."""
         return _suffixes[self.value]
 
     @classmethod
@@ -74,14 +72,22 @@
     if format == IOFormat.BENCH and dataNode.type != NodeType.MULTI_RUN:
         log.warning(
             "BENCH format can only be used with 'bench' mode enabled. Using pickle instead."
         )
         format = IOFormat.PICKLE
 
     filename = f"{dataNode.metadata['app_name']}_{dataNode.id}"
+    output_path: Path = data_out / filename
+
+    existing_files = [path for path in output_path.parent.glob(f"{filename}*")]
+    if len(existing_files) > 0:
+        log.warning(f"File {output_path} already exists and will.")
+        idx = len(existing_files)
+        filename += f"_{idx}"
+        dataNode.id += f"_{idx}"
 
     reportStr: Union[str, bytes]
     if format == IOFormat.JSON:
         filename += ".json"
         fileType = "w"
         reportStr = exportJson(dataNode, depth, rawData)
         with open(data_out / filename, fileType) as file:
@@ -100,17 +106,14 @@
         exportCSV(data_out / filename, dataNode)
     elif format == IOFormat.BENCH:
         filename += ".json"
         fileType = "w"
         reportStr = exportBench(dataNode)
         with open(data_out / filename, fileType) as file:
             file.write(reportStr)
-    # elif format == IOFormat.YAML:
-    #     filename += ".yaml"
-    #     reportStr = exportYaml(dataNode, depth, rawData)
     else:
         filename += ".txt"
         fileType = "w"
         reportStr = textReport(dataNode)
         with open(data_out / filename, fileType) as file:
             file.write(reportStr)
 
@@ -121,17 +124,14 @@
     Args:
         filePath (Path): Path to file
         format (Optional[IOFormat], optional): File format. Defaults to None.
     """
     if format == IOFormat.JSON:
         with open(filePath, "r") as file:
             dataNode = importJson(file.read())
-    # elif format == IOFormat.YAML:
-    #     filename += ".yaml"
-    #     reportStr = exportYaml(dataNode, depth, rawData)
     elif format == IOFormat.HDF5:
         dataNode = importHDF5(filePath)
     elif format == IOFormat.PICKLE:
         with open(filePath, "rb") as file:
             dataNode = importPickle(file.read())
     else:
         raise ValueError("File format is not supported.")
```

### Comparing `perun-0.2.0/perun/io/json.py` & `perun-0.3.0/perun/io/json.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/io/pandas.py` & `perun-0.3.0/perun/io/pandas.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/io/pickle.py` & `perun-0.3.0/perun/io/pickle.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/io/text_report.py` & `perun-0.3.0/perun/io/text_report.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Text report module."""
 
-from prettytable import PrettyTable
 
 from perun import config, log
 from perun.data_model.data import DataNode, MetricType, NodeType, Stats
 from perun.util import value2str
 
 
 def textReport(dataNode: DataNode) -> str:
@@ -32,34 +31,60 @@
         "PERUN REPORT\n"
         "\n"
         f"App name: {dataNode.metadata['app_name']}\n"
         f"Run ID: {dataNode.id}\n"
     )
 
     if dataNode.type == NodeType.MULTI_RUN:
-        table = PrettyTable(float_format="1.3f")
-        table.field_names = ["Name", "mean", "std", "max", "min"]
-        table.align = "r"
-        table.align["Name"] = "l"  # type: ignore
+        columns = ["Name", "Unit", "mean", "std", "max", "min"]
+        column_widths = [4, 4, 8, 8, 8, 8]
+        entries = {}
         for metricType in MetricType:
             if metricType in dataNode.metrics:
                 metric = dataNode.metrics[metricType]
                 if isinstance(metric, Stats):
                     value, tfactor, mag = value2str(metric.value, metric.metric_md)
-                    table.add_row(
-                        [
-                            f"{metricType.name} [{mag.symbol}{metric.metric_md.unit.value}]",
-                            f"{metric.mean / tfactor:.3f}",
-                            f"{metric.std / tfactor:.3f}",
-                            f"{metric.max / tfactor:.3f}",
-                            f"{metric.min / tfactor:.3f}",
-                        ]
+                    unit_str = f"{mag.symbol}{metric.metric_md.unit.value}"
+                    column_widths[0] = (
+                        column_widths[0]
+                        if column_widths[0] > len(metricType.name)
+                        else len(metricType.name)
                     )
+                    column_widths[1] = (
+                        column_widths[1]
+                        if column_widths[1] > len(unit_str)
+                        else len(unit_str)
+                    )
+                    entries[metricType.name] = [
+                        unit_str,
+                        f"{metric.mean/tfactor:.3f}",
+                        f"{metric.std/tfactor:.3f}",
+                        f"{metric.max/tfactor:.3f}",
+                        f"{metric.min/tfactor:.3f}",
+                    ]
+
         reportStr += "\n"
-        reportStr += table.get_string(float_format=".3")
+        header_row: str = "|" + "".join(
+            [
+                " {0:^{width}} |".format(column, width=width)
+                for column, width in zip(columns, column_widths)
+            ]
+        )
+        table_width = len(header_row)
+        reportStr += header_row + "\n"
+        reportStr += ("-" * table_width) + "\n"
+        for key, values in entries.items():
+            name = "| {0:<{width}} |".format(key, width=column_widths[0])
+            values_str = "".join(
+                [
+                    " {0:>{w}} |".format(v, w=w)
+                    for v, w in zip(values, column_widths[1:])
+                ]
+            )
+            reportStr += name + values_str + "\n"
 
     else:
         for metricType in MetricType:
             if metricType in dataNode.metrics:
                 metric = dataNode.metrics[metricType]
                 value, _, mag = value2str(metric.value, metric.metric_md)
                 reportStr += f"{metricType.name}: {value} {mag.symbol}{metric.metric_md.unit.value}\n"
```

### Comparing `perun-0.2.0/perun/logging.py` & `perun-0.3.0/perun/logging.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/perun.py` & `perun-0.3.0/perun/perun.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/perun/processing.py` & `perun-0.3.0/perun/processing.py`

 * *Files identical despite different names*

### Comparing `perun-0.2.0/pyproject.toml` & `perun-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 [tool.poetry]
 name = "perun"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Gutiérrez Hermosillo Muriedas, Juan Pedro <juanpedroghm@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/Helmholtz-AI-Energy/perun"
 
 [tool.poetry.scripts]
 perun = "perun.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-pynvml = "*"
-click = "*"
-py-cpuinfo = "*"
-PyYAML = "*"
-numpy = "*"
-psutil = "*"
-h5py = "*"
-prettytable = "^3.6.0"
-pandas = "^1.5.3"
-typing-extensions = "^4.5.0"
+pynvml = "^11.0.0"
+click = "^8.0.0"
+py-cpuinfo = "^5.0.0"
+numpy = "^1.20.0"
+psutil = "^5.9.0"
+h5py = "^3.5.9"
+pandas = ">=1.3"
+
+[tool.poetry.extras]
+dev = ["pytest", "flake8", "mypy", "black", "pre-commit", "pytest-cov"]
+docs = ["sphinx", "sphinx-rtd-theme", "sphinx-autoapi"]
+mpi = ["mpi4py"]
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
+pytest-cov = "*"
 flake8 = "*"
 mypy = "*"
 black = "*"
 pre-commit = "*"
-pytest-cov = "*"
 
-[tool.poetry.group.mpi]
+[tool.poetry.group.docs]
 optional = true
 
-[tool.poetry.group.mpi.dependencies]
-mpi4py = "*"
+[tool.poetry.group.docs.dependencies]
+sphinx = "*"
+sphinx-rtd-theme = "*"
+sphinx-autoapi = "*"
 
-[tool.poetry.group.horeka]
+[tool.poetry.group.mpi]
 optional = true
 
-[tool.poetry.group.horeka.dependencies]
-influxdb-client = "*"
-pandas = "*"
+[tool.poetry.group.mpi.dependencies]
+mpi4py = "^3.1"
+
+# [tool.poetry.group.horeka]
+# optional = true
+#
+# [tool.poetry.group.horeka.dependencies]
+# influxdb-client = "*"
 
 [tool.semantic_release]
 version_variable = [
     "perun/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "release"
@@ -56,19 +68,21 @@
 build_command = "pip install poetry && poetry build"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.isort]
 skip = ["perun/__init__.py"]
-known_third_party = ["click", "cpuinfo", "h5py", "influxdb_client", "numpy", "pandas", "prettytable", "psutil", "pynvml", "pytest", "typing_extensions"]
+known_third_party = ["click", "cpuinfo", "h5py", "influxdb_client", "numpy", "pandas", "psutil", "pynvml", "pytest"]
 profile = "black"
 
 [tool.pydocstyle]
 match = '(test_)!.*\.py'
+match-dir = 'perun'
+convention = 'numpy'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 exclude = [
```

### Comparing `perun-0.2.0/PKG-INFO` & `perun-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,59 @@
 Metadata-Version: 2.1
 Name: perun
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/Helmholtz-AI-Energy/perun
 License: BSD-3-Clause
 Author: Gutiérrez Hermosillo Muriedas, Juan Pedro
 Author-email: juanpedroghm@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML
-Requires-Dist: click
-Requires-Dist: h5py
-Requires-Dist: numpy
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: prettytable (>=3.6.0,<4.0.0)
-Requires-Dist: psutil
-Requires-Dist: py-cpuinfo
-Requires-Dist: pynvml
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: mpi
+Requires-Dist: click (>=8.0.0,<9.0.0)
+Requires-Dist: h5py (>=3.5.9,<4.0.0)
+Requires-Dist: numpy (>=1.20.0,<2.0.0)
+Requires-Dist: pandas (>=1.3)
+Requires-Dist: psutil (>=5.9.0,<6.0.0)
+Requires-Dist: py-cpuinfo (>=5.0.0,<6.0.0)
+Requires-Dist: pynvml (>=11.0.0,<12.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <img src="https://raw.githubusercontent.com/Helmholtz-AI-Energy/perun/main/docs/images/perun.svg">
+  <img src="https://raw.githubusercontent.com/Helmholtz-AI-Energy/perun/main/docs/images/full_logo.svg">
 </div>
 
-Have you ever wondered how much energy is used when training your neural network on the MNIST dataset? Want to get scared because of impact you are having on the evironment while doing "valuable" research? Are you interested in knowing how much carbon you are burning playing with DALL-E just to get attention on twitter? If the thing that was missing from your machine learning workflow was existential dread, this is the correct package for you!
+&nbsp;
+&nbsp;
 
-perun is python package that calculates the energy consumption of your python scripts by sampling usage statistics from Intel RAPL, Nvidia-NVML and *psutil*. Unlike other energy measuring applications out there, this is the only one capable of handling MPI applications, being capable of gathering data from 100s of nodes at the same time, and accumulating it efficiently. This is posible without adding any line of code into your existing application, and without meaningfully extending the runtime of your application.
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B-orange)](https://fair-software.eu)
+![PyPI](https://img.shields.io/pypi/v/perun)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/perun)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
+[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
+[![Documentation Status](https://readthedocs.org/projects/perun/badge/?version=latest)](https://perun.readthedocs.io/en/latest/?badge=latest)
+
+perun is a Python package that calculates the energy consumption of Python scripts by sampling usage statistics from Intel RAPL, Nvidia-NVML, and psutil. It can handle MPI applications, gather data from hundreds of nodes, and accumulate it efficiently. perun can be used as a command-line tool or as a function decorator in Python scripts.
+
+Check out the [docs](https://perun.readthedocs.io/en/latest/)!
+
+## Key Features
+
+ - Measures energy consumption of Python scripts using Intel RAPL, Nvidia-NVML, and psutil
+ - Handles MPI applications efficiently
+ - Gathers data from hundreds of nodes and accumulates it efficiently
+ - Can be used as a command-line tool or as a function decorator in Python scripts
 
 ## Installation
 
 From PyPI:
 
 ```console
 pip install perun
@@ -45,50 +63,55 @@
 
 ```console
 pip install git+https://github.com/Helmholtz-AI-Energy/perun
 ```
 
 ## Quick Start
 
-Perun has two usage methods, either using the command line, or using function decorators.
+### Command Line
 
-### Command line
-
-When using the command line, perun will output file containing runtime, energy and other information gathered while your script runs.
+To use perun as a command-line tool, run the monitor subcommand followed by the path to your Python script and its arguments:
 
 ```console
 $ perun monitor path/to/your/script.py [args]
-$ cat perun_results/script_2023-03-23T12:10:48.627214.txt
+```
+
+perun will output a file containing runtime, energy, and other information gathered while your script runs:
+
+
+```console
 PERUN REPORT
 
 App name: script
 Run ID: 2023-03-23T12:10:48.627214
 RUNTIME: 0:00:06.333626 s
 CPU_UTIL: 64.825 %
 MEM_UTIL: 0.563 %
 NET_READ: 1.401 kB
 NET_WRITE: 1.292 kB
 DISK_READ: 174.633 MB
 DISK_WRITE: 88.000 kB
+
 ```
 
-### Decorator
+### Function Decorator
 
-Perun can also monitor individual functions using a decorator:
+To use perun as a function decorator in your Python script, import the monitor decorator and add it to the function you want to monitor:
 
 ```python
+
 import time
 from perun.decorator import monitor
 
 @monitor()
-def your_sleep_function(n: int):
+def your_function(n: int):
     time.sleep(n)
 ```
 
-And then running your script like always:
+When you run your script, perun will output a report from the function:
 
 ```console
 python path/to/your/script.py
 ```
 
 > :exclamation: Each time the function is run, perun will output a new report from the function.
```

