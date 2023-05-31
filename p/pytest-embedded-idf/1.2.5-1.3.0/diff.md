# Comparing `tmp/pytest-embedded-idf-1.2.5.tar.gz` & `tmp/pytest-embedded-idf-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-idf-1.2.5.tar", last modified: Tue Apr 11 05:40:51 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-idf-1.3.0.tar", last modified: Wed May 31 13:09:03 2023, max compression
```

## Comparing `pytest-embedded-idf-1.2.5.tar` & `pytest-embedded-idf-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf/unity_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 05:40:51.000000 pytest-embedded-idf-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 05:40:39.000000 pytest-embedded-idf-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24784 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf/unity_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:03.000000 pytest-embedded-idf-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-31 13:08:52.000000 pytest-embedded-idf-1.3.0/setup.py
```

### Comparing `pytest-embedded-idf-1.2.5/PKG-INFO` & `pytest-embedded-idf-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.2.5
+Version: 1.3.0
 Summary: pytest embedded plugin for esp-idf project
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-idf
```

### Comparing `pytest-embedded-idf-1.2.5/pytest_embedded_idf/__init__.py` & `pytest-embedded-idf-1.3.0/pytest_embedded_idf/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 
 from pytest_embedded.utils import lazy_load
 
 from .app import IdfApp
 from .linux import LinuxDut, LinuxSerial
-from .unity_tester import CaseTester
+from .unity_tester import CaseTester, UnittestMenuCase
 
 __getattr__ = lazy_load(
     importlib.import_module(__name__),
     {
         'IdfApp': IdfApp,
         'LinuxDut': LinuxDut,
         'LinuxSerial': LinuxSerial,
@@ -24,8 +24,9 @@
 __all__ = [
     'IdfApp',
     'IdfSerial',
     'IdfDut',
     'CaseTester',
     'LinuxSerial',
     'LinuxDut',
+    'UnittestMenuCase',
 ]
```

### Comparing `pytest-embedded-idf-1.2.5/pytest_embedded_idf/app.py` & `pytest-embedded-idf-1.3.0/pytest_embedded_idf/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     Attributes:
         elf_file (str): elf file path
         flash_args (dict[str, Any]): dict of flasher_args.json
         flash_files (list[FlashFile]): list of (offset, file path, encrypted) of files need to be flashed in
         flash_settings (dict[str, Any]): dict of flash settings
     """
 
+    XTENSA_TARGETS = ['esp32', 'esp32s2', 'esp32s3']
+    RISCV32_TARGETS = ['esp32c3', 'esp32h2', 'esp32c2', 'esp32c6']
+
     FLASH_ARGS_FILENAME = 'flash_args'
     FLASH_PROJECT_ARGS_FILENAME = 'flash_project_args'
     FLASH_ARGS_JSON_FILENAME = 'flasher_args.json'
 
     def __init__(
         self,
         part_tool: Optional[str] = None,
@@ -107,14 +110,34 @@
         """
         if self.sdkconfig:
             return self.sdkconfig.get('IDF_TARGET', 'esp32')
         else:
             return self.flash_args.get('extra_esptool_args', {}).get('chip', 'esp32')
 
     @property
+    def is_riscv32(self):
+        if self.sdkconfig.get('IDF_TARGET_ARCH_RISCV'):
+            return True
+
+        if self.target in self.RISCV32_TARGETS:
+            return True
+
+        return False
+
+    @property
+    def is_xtensa(self):
+        if self.sdkconfig.get('IDF_TARGET_ARCH_XTENSA'):
+            return True
+
+        if self.target in self.XTENSA_TARGETS:
+            return True
+
+        return False
+
+    @property
     def partition_table(self) -> Dict[str, Any]:
         """
         Returns:
             partition table dict generated by the partition tool
         """
         if self._partition_table is not None:
             return self._partition_table
```

### Comparing `pytest-embedded-idf-1.2.5/pytest_embedded_idf/linux.py` & `pytest-embedded-idf-1.3.0/pytest_embedded_idf/linux.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.2.5/pytest_embedded_idf/serial.py` & `pytest-embedded-idf-1.3.0/pytest_embedded_idf/serial.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-idf-1.2.5/pytest_embedded_idf.egg-info/PKG-INFO` & `pytest-embedded-idf-1.3.0/pytest_embedded_idf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-idf
-Version: 1.2.5
+Version: 1.3.0
 Summary: pytest embedded plugin for esp-idf project
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-idf
```

### Comparing `pytest-embedded-idf-1.2.5/setup.py` & `pytest-embedded-idf-1.3.0/setup.py`

 * *Files identical despite different names*

