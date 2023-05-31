# Comparing `tmp/pytest-embedded-qemu-1.2.5.tar.gz` & `tmp/pytest-embedded-qemu-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-qemu-1.2.5.tar", last modified: Tue Apr 11 05:40:52 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-qemu-1.3.0.tar", last modified: Wed May 31 13:09:03 2023, max compression
```

## Comparing `pytest-embedded-qemu-1.2.5.tar` & `pytest-embedded-qemu-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/qemu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 05:40:52.000000 pytest-embedded-qemu-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-11 05:40:39.000000 pytest-embedded-qemu-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/qemu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/setup.py
```

### Comparing `pytest-embedded-qemu-1.2.5/PKG-INFO` & `pytest-embedded-qemu-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.2.5
+Version: 1.3.0
 Summary: pytest embedded plugin for qemu, not target chip
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-qemu
```

### Comparing `pytest-embedded-qemu-1.2.5/README.md` & `pytest-embedded-qemu-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/app.py` & `pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import os
 from typing import Optional
 
 from pytest_embedded.log import MessageQueue, live_print_call
 from pytest_embedded_idf.app import IdfApp
 
-from . import DEFAULT_IMAGE_FN
+from . import DEFAULT_IMAGE_FN, ENCRYPTED_IMAGE_FN
 
 
 class IdfFlashImageMaker:
     """
     Create a single image for QEMU based on the `IdfApp`'s partition table and all the flash files.
     """
 
@@ -27,18 +27,20 @@
         """
         Create a single image file for qemu.
         """
         # flash_files is sorted, if the first offset is not 0x0, we need to fill it with empty bin
         if self.app.flash_files[0][0] != 0x0:
             self._write_empty_bin(count=self.app.flash_files[0][0])
         for offset, file_path, encrypted in self.app.flash_files:
-            if encrypted:
-                raise NotImplementedError('will implement later')
-            else:
-                self._write_bin(file_path, seek=offset)
+            self._write_bin(file_path, seek=offset)
+
+        if self.app.encrypt:
+            if self.app.keyfile is None or not os.path.exists(self.app.keyfile):
+                raise ValueError('Flash Encryption key file doesn\'t exist')
+            self._write_encrypted_bin(self.image_path)
 
     def _write_empty_bin(self, count: int, bs: int = 1024, seek: int = 0):
         live_print_call(
             f'dd if=/dev/zero bs={bs} count={count} seek={seek} of={self.image_path}',
             shell=True,
         )
 
@@ -46,23 +48,18 @@
         live_print_call(
             f'dd if={binary_filepath} bs={bs} seek={seek} of={self.image_path} conv=notrunc',
             shell=True,
         )
 
     def _write_encrypted_bin(self, binary_filepath, bs: int = 1, seek: int = 0):
         live_print_call(
-            'dd if=/dev/zero bs=1 count=32 of=key.bin',
-            shell=True,
-        )  # generate a fake key bin
-        live_print_call(
-            f'espsecure.py encrypt_flash_data --keyfile key.bin --output decrypted.bin --address {seek} '
-            f'{binary_filepath}',
+            f'espsecure.py encrypt_flash_data --keyfile {self.app.keyfile} '
+            f'--output {self.app.encrypted_image_path} --address {seek} {binary_filepath}',
             shell=True,
         )
-        self._write_bin('decrypted.bin', bs=bs, seek=seek)
 
     def _burn_efuse(self):
         pass
 
 
 class QemuApp(IdfApp):
     """
@@ -73,25 +70,29 @@
     """
 
     def __init__(
         self,
         msg_queue: MessageQueue,
         qemu_image_path: Optional[str] = None,
         skip_regenerate_image: Optional[bool] = False,
+        encrypt: Optional[bool] = False,
+        keyfile: Optional[str] = None,
         **kwargs,
     ):
         self._q = msg_queue
 
         super().__init__(**kwargs)
 
         self.image_path = qemu_image_path or os.path.join(self.binary_path, DEFAULT_IMAGE_FN)
         self.skip_regenerate_image = skip_regenerate_image
+        self.encrypt = encrypt
+        self.keyfile = keyfile
 
-        if self.target != 'esp32':
-            raise ValueError('For now on QEMU we only support ESP32')
+        if self.encrypt:
+            self.encrypted_image_path = os.path.join(self.binary_path, ENCRYPTED_IMAGE_FN)
 
         self.create_image()
 
     def create_image(self) -> None:
         """
         Create the image, if it doesn't exist.
         """
```

### Comparing `pytest-embedded-qemu-1.2.5/pytest_embedded_qemu/qemu.py` & `pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/qemu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,78 @@
 import os
 import shlex
 from typing import Optional
 
 from pytest_embedded.log import DuplicateStdoutPopen
 
-from . import DEFAULT_IMAGE_FN
+from . import DEFAULT_IMAGE_FN, QemuApp
 
 
 class Qemu(DuplicateStdoutPopen):
     """
     QEMU class
     """
 
     SOURCE = 'QEMU'
 
     QEMU_PROG_PATH = 'qemu-system-xtensa'
-    QEMU_DEFAULT_ARGS = '-nographic -no-reboot -machine esp32'
+    QEMU_PROG_FMT = 'qemu-system-{}'
+
+    QEMU_DEFAULT_ARGS = '-nographic -machine esp32'
+    QEMU_DEFAULT_FMT = '-nographic -machine {}'
 
     QEMU_STRAP_MODE_FMT = '-global driver=esp32.gpio,property=strap_mode,value={}'
     QEMU_SERIAL_TCP_FMT = '-serial tcp::{},server,nowait'
 
     def __init__(
         self,
         qemu_image_path: Optional[str] = None,
         qemu_prog_path: Optional[str] = None,
         qemu_cli_args: Optional[str] = None,
         qemu_extra_args: Optional[str] = None,
+        app: Optional[QemuApp] = None,
         **kwargs,
     ):
         """
         Args:
             qemu_image_path: QEMU image path
             qemu_prog_path: QEMU program path
             qemu_cli_args: QEMU CLI arguments
             qemu_extra_args: QEMU CLI extra arguments, will be appended to `qemu_cli_args`
         """
+        self.app = app
+
         image_path = qemu_image_path or DEFAULT_IMAGE_FN
         if not os.path.exists(image_path):
             raise ValueError(f'QEMU image path doesn\'t exist: {image_path}')
 
-        qemu_prog_path = qemu_prog_path or self.QEMU_PROG_PATH
-        qemu_cli_args = shlex.split(qemu_cli_args or self.QEMU_DEFAULT_ARGS)
+        qemu_prog_path = qemu_prog_path or self.qemu_prog_name
+        qemu_cli_args = shlex.split(qemu_cli_args or self.qemu_default_args)
         qemu_extra_args = shlex.split(qemu_extra_args or '')
 
         super().__init__(
             cmd=[qemu_prog_path, *qemu_cli_args, *qemu_extra_args] + ['-drive', f'file={image_path},if=mtd,format=raw'],
             **kwargs,
         )
+
+    @property
+    def qemu_prog_name(self):
+        if self.app:
+            return self.QEMU_PROG_FMT.format('xtensa' if self.app.is_xtensa else 'riscv32')
+
+        return self.QEMU_PROG_PATH
+
+    @property
+    def qemu_default_args(self):
+        if self.app:
+            return self.QEMU_DEFAULT_FMT.format(self.app.target)
+
+        return self.QEMU_DEFAULT_ARGS
+
+    def _hard_reset(self):
+        """
+        This is a fake hard_reset. Keep this API to keep the consistency.
+        """
+        # TODO: implement with QMP
+        #  https://gitlab.com/qemu-project/python-qemu-qmp/-/issues/6
+        #  for now got so many unexpected exceptions while __del__
+        raise NotImplementedError
```

### Comparing `pytest-embedded-qemu-1.2.5/pytest_embedded_qemu.egg-info/PKG-INFO` & `pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.2.5
+Version: 1.3.0
 Summary: pytest embedded plugin for qemu, not target chip
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-qemu
```

### Comparing `pytest-embedded-qemu-1.2.5/setup.py` & `pytest-embedded-qemu-1.3.0/setup.py`

 * *Files identical despite different names*

