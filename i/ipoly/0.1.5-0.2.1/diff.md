# Comparing `tmp/ipoly-0.1.5.tar.gz` & `tmp/ipoly-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipoly-0.1.5.tar", last modified: Tue Apr  4 08:35:31 2023, max compression
+gzip compressed data, was "ipoly-0.2.1.tar", max compression
```

## Comparing `ipoly-0.1.5.tar` & `ipoly-0.2.1.tar`

### file list

```diff
@@ -1,86 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.263961 ipoly-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.251961 ipoly-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.255961 ipoly-0.1.5/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-04 08:35:21.000000 ipoly-0.1.5/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.255961 ipoly-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-04 08:35:21.000000 ipoly-0.1.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-04 08:35:21.000000 ipoly-0.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-04 08:35:21.000000 ipoly-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-04 08:35:21.000000 ipoly-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-04 08:35:21.000000 ipoly-0.1.5/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.255961 ipoly-0.1.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-04 08:35:21.000000 ipoly-0.1.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-04 08:35:21.000000 ipoly-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-04 08:35:21.000000 ipoly-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-04 08:35:31.263961 ipoly-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-04 08:35:21.000000 ipoly-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    58885 2023-04-04 08:35:21.000000 ipoly-0.1.5/banner_transparent_background.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:21.000000 ipoly-0.1.5/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.255961 ipoly-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.255961 ipoly-0.1.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/ipoly.LaTeX.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/ipoly.communication.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/ipoly.file_management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/ipoly.logger.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/ipoly.ml.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/ipoly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/ipoly.scraping.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/ipoly.traceback.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 08:35:21.000000 ipoly-0.1.5/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.259961 ipoly-0.1.5/ipoly/
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/LaTeX.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    20979 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/file_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.259961 ipoly-0.1.5/ipoly/img/
--rw-r--r--   0 runner    (1001) docker     (123)    21662 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/img/ipoly.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    25346 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/scraping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/traceback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-04 08:35:21.000000 ipoly-0.1.5/ipoly/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.259961 ipoly-0.1.5/ipoly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-04 08:35:31.000000 ipoly-0.1.5/ipoly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-04 08:35:31.000000 ipoly-0.1.5/ipoly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:35:31.000000 ipoly-0.1.5/ipoly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-04 08:35:31.000000 ipoly-0.1.5/ipoly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 08:35:31.000000 ipoly-0.1.5/ipoly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.259961 ipoly-0.1.5/logo/
--rw-r--r--   0 runner    (1001) docker     (123)    58885 2023-04-04 08:35:21.000000 ipoly-0.1.5/logo/banner_transparent_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    62353 2023-04-04 08:35:21.000000 ipoly-0.1.5/logo/banner_white_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    66249 2023-04-04 08:35:21.000000 ipoly-0.1.5/logo/logo+name_transparent_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    68879 2023-04-04 08:35:21.000000 ipoly-0.1.5/logo/logo+name_white_background.png
--rw-r--r--   0 runner    (1001) docker     (123)   140930 2023-04-04 08:35:21.000000 ipoly-0.1.5/logo/logo_ipoly_transparent_background.png
--rw-r--r--   0 runner    (1001) docker     (123)   151573 2023-04-04 08:35:21.000000 ipoly-0.1.5/logo/logo_ipoly_white_background.png
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-04 08:35:21.000000 ipoly-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-04 08:35:21.000000 ipoly-0.1.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-04 08:35:21.000000 ipoly-0.1.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-04 08:35:21.000000 ipoly-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-04 08:35:31.263961 ipoly-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.263961 ipoly-0.1.5/source/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/conftest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/ipoly.LaTeX.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/ipoly.communication.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/ipoly.file_management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/ipoly.logger.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/ipoly.ml.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/ipoly.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/ipoly.scraping.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/ipoly.traceback.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-04 08:35:21.000000 ipoly-0.1.5/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.263961 ipoly-0.1.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.263961 ipoly-0.1.5/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)   191709 2023-04-04 08:35:21.000000 ipoly-0.1.5/tests/test_files/image2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:35:31.263961 ipoly-0.1.5/tests/test_files/test_folder/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-04-04 08:35:21.000000 ipoly-0.1.5/tests/test_files/test_folder/image1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 08:35:21.000000 ipoly-0.1.5/tests/test_files/test_folder/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-04 08:35:21.000000 ipoly-0.1.5/tests/test_ipoly.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-04 08:35:21.000000 ipoly-0.1.5/unix_env.sh
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-04 08:35:21.000000 ipoly-0.1.5/windows_env.cmd
+-rw-r--r--   0        0        0     1074 2023-05-31 13:51:25.170964 ipoly-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2689 2023-05-31 13:51:25.170964 ipoly-0.2.1/README.md
+-rw-r--r--   0        0        0    13323 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/LaTeX.py
+-rw-r--r--   0        0        0      405 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/__init__.py
+-rw-r--r--   0        0        0     3908 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/communication.py
+-rw-r--r--   0        0        0    51143 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/file_management.py
+-rw-r--r--   0        0        0    21662 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/img/ipoly.ico
+-rw-r--r--   0        0        0     6181 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/logger.py
+-rw-r--r--   0        0        0    26520 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/ml.py
+-rw-r--r--   0        0        0    13890 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/scraping.py
+-rw-r--r--   0        0        0     2350 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/traceback.py
+-rw-r--r--   0        0        0     9665 2023-05-31 13:51:25.174964 ipoly-0.2.1/ipoly/visualisation.py
+-rw-r--r--   0        0        0     2656 2023-05-31 13:51:25.182964 ipoly-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 ipoly-0.2.1/PKG-INFO
```

### Comparing `ipoly-0.1.5/LICENSE` & `ipoly-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipoly-0.1.5/ipoly/img/ipoly.ico` & `ipoly-0.2.1/ipoly/img/ipoly.ico`

 * *Files identical despite different names*

### Comparing `ipoly-0.1.5/ipoly/logger.py` & `ipoly-0.2.1/ipoly/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,37 @@
-from abc import abstractmethod
+"""Module proposing a custom loger."""
+import logging
 from logging.handlers import RotatingFileHandler
 from os import remove
 from threading import Thread
 from time import sleep
-from traceback import extract_stack, walk_stack
-import logging
+from traceback import extract_stack
+from traceback import walk_stack
 from typing import Literal
+from typing import TypeVar  # TODO waiting for PEP 673 to be released
+
+# from typing import Self
+
+Self_Logger = TypeVar("Self_Logger", bound="Logger")
+
+from ipoly.traceback import raiser
 
 available_log_levels = Literal[
-    "PROD", "NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"
+    "PROD",
+    "NOTSET",
+    "DEBUG",
+    "INFO",
+    "WARNING",
+    "ERROR",
+    "CRITICAL",
 ]
 
 
 class Logger:
-    """Abstract class to implement a configurable logger to a specific class
+    """Abstract class to implement a configurable logger to a specific class.
 
     The logger automatically creates a log file named like the class implementing this class
 
     :param debug: bool, default False
 
     :param log: str, default "PROD"
         Level of the logger among :
@@ -30,25 +44,22 @@
         CRITICAL: Level 50
     :param log_stdout: bool, default False
         Print the logs if enabled, however in both cases save the logs in the log file
     :param keep_log: bool, default False
         Overwrite the previous log file if False
     """
 
-    @abstractmethod
-    def _raiser(self, exception: str):
-        raise NotImplementedError
-
     def __init__(
-        self,
-        debug=False,
+        self: Self_Logger,
+        debug: bool = False,
         log: available_log_levels = "PROD",
-        log_stdout=False,
-        keep_log=False,
+        log_stdout: bool = False,
+        keep_log: bool = False,
     ):
+        """Initialisation of the Logger."""
         self._DEBUG = debug
         self._LOG = log
         self._log_stdout = log_stdout
         self._keep_log = keep_log
 
         if self._LOG != "PROD":
             frame = None
@@ -59,15 +70,15 @@
                 if frame.f_locals[variable_names[0]] not in (self, self.__class__):
                     break
                     # if the frame is inside a method of this instance,
                     # the first argument usually contains either the instance
                     # or its class, we want to find the first frame, where
                     # this is not the case
             else:
-                self._raiser("No suitable outer frame found.")
+                raiser("No suitable outer frame found.")
             self._outer_frame = frame
             self.creation_module = frame.f_globals["__name__"]
             (
                 self.creation_file,
                 self.creation_line,
                 self.creation_function,
                 self.creation_text,
@@ -79,15 +90,16 @@
                 if not keep_log:
                     remove(self._creation_name + ".log")
             except OSError:
                 pass
             self._logger = logging.getLogger()
             self._logger.setLevel(logging.DEBUG)
             formatter = logging.Formatter(
-                "%(asctime)s :: %(levelname)s :: %(message)s", "%d: %H:%M:%S"
+                "%(asctime)s :: %(levelname)s :: %(message)s",
+                "%d: %H:%M:%S",
             )
             file_handler = RotatingFileHandler(
                 self._creation_name + ".log",
                 "a",
                 1000000,
                 1,
                 encoding="utf-8",
@@ -106,54 +118,51 @@
             # creation of a second handler which redirect every log of self.logging on the console
             if log_stdout:
                 stream_handler = logging.StreamHandler()
                 stream_handler.setLevel(log_type)
                 self._logger.addHandler(stream_handler)
             self._log("Initialization of a new object of this instance", log="INFO")
 
-    def _log(self, message, condition: bool = True, log="DEBUG"):
-        """
-        Create a log message
-        :param message: str
-            Content of the log message
-        :param condition: bool, default True
-            Condition to create the log
-        :param log: str
-            Log level (PROD, NOTSET, DEBUG, INFO, WARNING, ERROR, CRITICAL)
-        :return: None
-        """
+    def _log(
+        self: Self_Logger,
+        message: str,
+        condition: bool = True,
+        log: available_log_levels = "DEBUG",
+    ):
+        """Create a log message.
 
+        Args:
+            message: Content of the log message
+            condition: Condition to create the log
+            log: Log level (PROD, NOTSET, DEBUG, INFO, WARNING, ERROR, CRITICAL)
+        """
         if condition and self._LOG != "PROD":
             logging_levels = {
                 "NOTSET": logging.NOTSET,
                 "DEBUG": logging.DEBUG,
                 "INFO": logging.INFO,
                 "WARNING": logging.WARNING,
                 "ERROR": logging.ERROR,
                 "CRITICAL": logging.CRITICAL,
             }[log]
             self._logger.log(logging_levels, message)
             logging.shutdown()
 
     def _check_existence_after_creation(self):
-        """
-        Check if the log file has been created, else raise an error
-        :return: None
-        """
-
+        """Check if the log file has been created, else raise an error."""
         while self._outer_frame.f_lineno == self.creation_line:
             sleep(0.01)
         # this is executed as soon as the line number changes
         # now we can be sure the instance was actually created
 
         def error():
-            self._raiser(
+            raiser(
                 "The creation name hasn't be found, the "
                 "probable cause may be that you declared "
-                "several variables at the same time."
+                "several variables at the same time.",
             )
 
         nameparts = self._creation_name.split(".")
         var = None
         try:
             var = self._outer_frame.f_locals[nameparts[0]]
         except KeyError:
```

### Comparing `ipoly-0.1.5/ipoly/ml.py` & `ipoly-0.2.1/ipoly/ml.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,50 @@
 import pandas as pd
 import tensorflow as tf
 
 from ipoly.file_management import caster
 from ipoly.traceback import raiser
 
 
+def get_driver_details() -> dict | None:
+    """Returns details of GPU's driver, CUDA version and Tensorflow version.
+
+    Uses nvsmi library to get GPU information. If no Nvidia-smi is installed or no GPU info is found,
+    'N/A' is assigned to the driver and CUDA version.
+
+    Returns:
+        A dictionary with the driver version, CUDA version, and Tensorflow version.
+    """
+    from nvsmi import get_gpus
+
+    # Get GPU information
+    try:
+        gpu_info = get_gpus()
+    except FileNotFoundError:
+        print("No Nvidia-smi installed")
+        return None
+
+    # Get the first GPU's driver and CUDA version (assuming all GPUs have the same driver and CUDA version)
+    if gpu_info:
+        first_gpu = gpu_info[0]
+        driver_version = first_gpu.driver_version
+        cuda_version = first_gpu.cuda_version
+    else:
+        driver_version = "N/A"
+        cuda_version = "N/A"
+
+    version_information = {
+        "Driver Version": driver_version,
+        "Cuda Version": cuda_version,
+        "Tensorflow Version": tf.__version__,
+    }
+
+    return version_information
+
+
 def set_seed(seed: int = 42) -> None:
     """Set the seed fot NumPy, TensorFlow and PyTorch.
 
     Args:
         seed: The seed value to set.
     """
     from tensorflow import random as tfr
@@ -159,15 +195,15 @@
         correlation_threshold : The column is removed if its correlation with another is higher than this threshold.
         missing_rows_threshold : The row is removed if the proportion of its non-empty cells is lower than this threshold.
         missing_columns_threshold : The column is removed if its proportion of non-empty cells is lower than this threshold.
         categories_ratio_threshold : The column is removed if its proportion of non unique values is higher than this threshold.
         id_correlation_threshold : The column is removed if all its values are unique the mean correlation with other columns is less than this threshold.
         verbose : Print realised actions if True.
     """
-    y = [y] if not y is list else y
+    y = [y] if not isinstance(y, list) else y
     if len(y) != len(subfinder(y, train_df.columns)):
         raiser("y variable is not in df columns", Exception)
 
     train_df = caster(train_df)
     if test_df is not None:
         test_df = caster(
             test_df,
@@ -380,30 +416,30 @@
     from transformers import logging
     from transformers.utils import CONFIG_NAME, TF2_WEIGHTS_NAME
     from os import listdir
     from os.path import isdir
 
     logging.set_verbosity_error()
     if not processor_name:
-        processor_name = model_name_or_path
+        processor_name = str(model_name_or_path)
     if not config_name:
-        config_name = model_name_or_path
+        config_name = str(model_name_or_path)
 
     checkpoint = None
     if isdir(output_dir) and len(listdir(output_dir)) > 0 and not overwrite_output_dir:
         if (output_dir / CONFIG_NAME).is_file() and (
             output_dir / TF2_WEIGHTS_NAME
         ).is_file():
             checkpoint = output_dir
         else:
             raise ValueError(
                 f"Output directory ({output_dir}) already exists and is not empty. "
                 "Use --overwrite_output_dir to continue regardless.",
             )
-
+    config_path: str | PathLike
     if checkpoint is not None:
         config_path = output_dir
     elif config_name:
         config_path = config_name
     else:
         config_path = model_name_or_path
     if num_labels is not None:
@@ -656,15 +692,16 @@
         # calculate the accuracy
         acc = accuracy_score(Y_test, Y_pred)
 
         # update the best model if necessary
         if acc > best_acc:
             best_acc = acc
             best_model = model
-    best_model = best_model.fit(X, y)
+    if best_model is not None:
+        best_model = best_model.fit(X, y)
     return best_model
 
 
 def binary_focal_loss(gamma=2.0, alpha=0.25):
     """Binary form of focal loss.
 
     FL(p_t) = -alpha * (1 - p_t)**gamma * log(p_t)
```

### Comparing `ipoly-0.1.5/ipoly/visualisation.py` & `ipoly-0.2.1/ipoly/visualisation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 """Provide routines for visualising data."""
 from typing import Any
 from typing import Iterable
 from typing import Tuple
 
-import matplotlib.pyplot as plt
-import seaborn as sns
-import tensorflow as tf
 from nptyping import Int
 from nptyping import NDArray
 from numpy import set_printoptions
 from pandas import DataFrame
-from sklearn import metrics
 
 # numpy and matplotlib defaults
 set_printoptions(threshold=15, linewidth=80)
 
 
 def plot(
-    title: str = None,
-    xlabel: str = None,
-    ylabel: str = None,
+    title: str | None = None,
+    xlabel: str | None = None,
+    ylabel: str | None = None,
     figsize: Any = None,
     grid: bool = False,
-    xticks: Tuple[int] = None,
-    yticks: Tuple[int] = None,
+    xticks: Tuple[int] | None = None,
+    yticks: Tuple[int] | None = None,
 ):
     """Set the main parameters value."""
     from numpy import arange
+    import matplotlib.pyplot as plt
 
     fig = plt.figure(figsize=figsize, dpi=100)
     fig.patch.set_facecolor("xkcd:white")
     plt.xticks(rotation=45, ha="right")
 
     plt.legend(bbox_to_anchor=(1.05, 1))
     if xticks:
@@ -40,29 +37,31 @@
     plt.grid(grid)
     if ylabel:
         plt.ylabel(ylabel)
     if xlabel:
         plt.xlabel(xlabel)
     if title:
         plt.title(title)
-    if ".png" in title:
+    if title is not None and ".png" in title:
         plt.savefig(title)
     else:
         plt.show()
     plt.close()
 
 
-def plot_history(history, keys: list[str] = None) -> None:
+def plot_history(history, keys: list[str] | None = None) -> None:
     """Plot the history of a Tensorflow training for each metrics.
 
     Args:
         history: The history to plot.
         keys: List of all metrics that will be plot.Plot all metrics
             if not specified.
     """
+    import matplotlib.pyplot as plt
+
     if keys is None:
         keys = history.history.keys()
     for key in keys:
         plt.plot(history.history[key])
         plt.plot(history.history["val_accuracy"])
         plt.legend(["train", "val"], loc="upper left")
         plot("model accuracy", "epoch", "accuracy")
@@ -72,44 +71,49 @@
     """Plot the correlation matrix of your DataFrame.
 
     Args:
         df: The input DataFrame.
     """
     from numpy import triu
     from numpy import ones_like
+    from seaborn import heatmap as sns_heatmap
+    from seaborn import diverging_palette
+    import matplotlib.pyplot as plt
 
     corr = df.corr()
     # Generate a mask for the upper triangle
     mask = triu(ones_like(corr, dtype=bool))
     # Set up the matplotlib figure
     f, ax = plt.subplots(figsize=(11, 9))
     # Generate a custom diverging colormap
-    cmap = sns.diverging_palette(230, 20, as_cmap=True)
+    cmap = diverging_palette(230, 20, as_cmap=True)
     # Draw the heatmap with the mask and correct aspect ratio
-    sns.heatmap(
+    sns_heatmap(
         corr,
         mask=mask,
         cmap=cmap,
         vmax=0.3,
         center=0,
         square=True,
         linewidths=0.5,
         cbar_kws={"shrink": 0.5},
     )
 
 
 def _confusion_matrix(confusion_matrix, axes, class_names, fontsize=14):
+    from seaborn import heatmap as sns_heatmap
+
     df_cm = DataFrame(
         confusion_matrix,
         index=class_names,
         columns=class_names,
     )
 
     try:
-        heatmap = sns.heatmap(df_cm, annot=True, fmt="d", cbar=False, ax=axes)
+        heatmap = sns_heatmap(df_cm, annot=True, fmt="d", cbar=False, ax=axes)
     except ValueError:
         raise ValueError("Confusion matrix values must be integers.")
     heatmap.yaxis.set_ticklabels(
         heatmap.yaxis.get_ticklabels(),
         rotation=0,
         ha="right",
         fontsize=fontsize,
@@ -123,41 +127,44 @@
     axes.set_ylabel("True label")
     axes.set_xlabel("Predicted label")
 
 
 def plot_confusion_matrix(
     y_pred: NDArray[Any, Int],
     y_true: NDArray[Any, Int],
-    labels: Iterable[str] = None,
+    labels: Iterable[str] | None = None,
 ):
     """Plot the confusion matrix.
 
     It determines by itself if it has to plot a simple confusion matrix
     or multiple  ones in case of multilabel classification.
 
     Args:
         y_pred: Predicted logits.
         y_true: True labels.
         labels: Labels name. Need to be specified only if it is a
             multilabel classification.
     """
     from numpy import unique
+    from sklearn import metrics
+    import matplotlib.pyplot as plt
 
     fig, ax = plt.subplots(2, 2, figsize=(10, 7))
     if ((unique(y_true.sum(axis=1)) == 1).all()) or (len(y_true.shape) == 1):
         if len(y_true.shape) == 2:
             y_true = y_true.argmax(axis=1)
             y_pred = y_pred.argmax(axis=1)
         _confusion_matrix(
             metrics.confusion_matrix(y_true, y_pred),
             ax.flatten(),
             ["N", "Y"],
         )
     else:
         confusion_matrix = metrics.multilabel_confusion_matrix(y_true, y_pred)
+        labels = labels or []  # replace None with an empty list
         for axes, cfs_matrix, label in zip(ax.flatten(), confusion_matrix, labels):
             _confusion_matrix(cfs_matrix, axes, ["N", "Y"])
             axes.set_title("Confusion Matrix for the class - " + label)
 
         fig.tight_layout()
         plt.show()
 
@@ -256,14 +263,15 @@
     Usage:
         display_batch_of_images(images)
         display_batch_of_images(images, predictions)
         display_batch_of_images((images, labels))
         display_batch_of_images((images,labels), predictions)
     """
     import matplotlib.pyplot as plt
+    import tensorflow as tf
     from math import sqrt
 
     # data
     images, labels = batch_to_numpy_images_and_labels(databatch)
     labels = [tf.argmax(label, axis=0) for label in labels]  # One hot to index
     if labels is None:
         labels = [None for _ in enumerate(images)]
```

