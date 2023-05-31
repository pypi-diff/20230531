# Comparing `tmp/pydrs-2.2.0.tar.gz` & `tmp/pydrs-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrs-2.2.0.tar", last modified: Fri Mar  3 12:57:49 2023, max compression
+gzip compressed data, was "pydrs-2.3.0.tar", last modified: Wed May 31 12:18:36 2023, max compression
```

## Comparing `pydrs-2.2.0.tar` & `pydrs-2.3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 12:57:49.107663 pydrs-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-03 12:57:33.000000 pydrs-2.2.0/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-03 12:57:33.000000 pydrs-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-03 12:57:33.000000 pydrs-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-03-03 12:57:49.107663 pydrs-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-03-03 12:57:33.000000 pydrs-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-03 12:57:33.000000 pydrs-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-03 12:57:49.107663 pydrs-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 12:57:33.000000 pydrs-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 12:57:49.103664 pydrs-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 12:57:49.103664 pydrs-2.2.0/src/pydrs/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95763 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 12:57:49.103664 pydrs-2.2.0/src/pydrs/bsmp/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/command.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 12:57:49.103664 pydrs-2.2.0/src/pydrs/bsmp/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/entities/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/entities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/bsmp/pwrsupply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 12:57:49.107663 pydrs-2.2.0/src/pydrs/consts/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/consts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/consts/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    24259 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/consts/fac.py
--rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/consts/fap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/consts/fbp.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/consts/resonant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/pydrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-03-03 12:57:33.000000 pydrs-2.2.0/src/pydrs/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 12:57:49.103664 pydrs-2.2.0/src/pydrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-03-03 12:57:49.000000 pydrs-2.2.0/src/pydrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-03 12:57:49.000000 pydrs-2.2.0/src/pydrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 12:57:49.000000 pydrs-2.2.0/src/pydrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 12:57:48.000000 pydrs-2.2.0/src/pydrs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-03 12:57:49.000000 pydrs-2.2.0/src/pydrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-03 12:57:49.000000 pydrs-2.2.0/src/pydrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:36.715774 pydrs-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-31 12:18:17.000000 pydrs-2.3.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-31 12:18:17.000000 pydrs-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 12:18:17.000000 pydrs-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-31 12:18:36.715774 pydrs-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-05-31 12:18:17.000000 pydrs-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-31 12:18:17.000000 pydrs-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-31 12:18:36.715774 pydrs-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:18:17.000000 pydrs-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:36.711774 pydrs-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:36.715774 pydrs-2.3.0/src/pydrs/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96407 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:36.715774 pydrs-2.3.0/src/pydrs/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:36.715774 pydrs-2.3.0/src/pydrs/bsmp/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/entities/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/entities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/bsmp/pwrsupply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:36.715774 pydrs-2.3.0/src/pydrs/consts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/consts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/consts/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24259 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/consts/fac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/consts/fap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/consts/fbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/consts/resonant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/pydrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-31 12:18:17.000000 pydrs-2.3.0/src/pydrs/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:18:36.715774 pydrs-2.3.0/src/pydrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-31 12:18:36.000000 pydrs-2.3.0/src/pydrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-31 12:18:36.000000 pydrs-2.3.0/src/pydrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:18:36.000000 pydrs-2.3.0/src/pydrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:18:36.000000 pydrs-2.3.0/src/pydrs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-31 12:18:36.000000 pydrs-2.3.0/src/pydrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 12:18:36.000000 pydrs-2.3.0/src/pydrs.egg-info/top_level.txt
```

### Comparing `pydrs-2.2.0/CHANGES.md` & `pydrs-2.3.0/CHANGES.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## [2.3.0] - 2023-05-09
+### Changed:
+- SWLS resonant converter BSMP specification, including new variables, alarms and interlocks
+
 ## [2.2.0] - 2023-02-27
 ### Changed:
 - ID of BSMP variables in FAC-DCDC and FAC-DCDC-EMA 
 - ID of BSMP variables in FAP-4P and FAP-2P2S 
 
 ### Removed:
 - "Ground Leakage Overcurrent" from FAC-DCDC and FAC-DCDC-EMA module alarm and interlock lists
```

### Comparing `pydrs-2.2.0/LICENSE` & `pydrs-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/PKG-INFO` & `pydrs-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrs
-Version: 2.2.0
+Version: 2.3.0
 License: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydrs-2.2.0/README.md` & `pydrs-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/pyproject.toml` & `pydrs-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/base.py` & `pydrs-2.3.0/src/pydrs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2194,30 +2194,48 @@
         """
         return self._read_vars_generic(
             fac.bsmp_2p_dcdc_imas,
             fac.list_2p_dcdc_imas_soft_interlocks,
             fac.list_2p_dcdc_imas_hard_interlocks,
         )
 
-    def read_vars_swls_resonant_converter(self) -> dict:
+    def read_vars_swls_resonant_converter(self, iib=True) -> dict:
         """
         Reads SWLS resonant converter power supply variables
 
+        Parameters
+        -------
+        iib
+            Whether or not IIB interlocks should be parsed and returned alongside other data
 
         Returns
         -------
         dict
             Dictionary with power supply variables
         """
-        return self._read_vars_generic(
+        vars_dict = self._read_vars_generic(
             resonant.bsmp,
             resonant.list_soft_interlocks,
             resonant.list_hard_interlocks,
         )
 
+        if iib:
+            vars_dict["iib_interlocks_raw"] = vars_dict["iib_interlocks"]
+            vars_dict["iib_alarms_raw"] = vars_dict["iib_alarms"]
+
+            vars_dict["iib_interlocks"] = self.decode_interlocks(
+                vars_dict["iib_interlocks_raw"], resonant.list_iib_interlocks
+            )
+
+            vars_dict["iib_alarms"] = self.decode_interlocks(
+                vars_dict["iib_alarms_raw"], resonant.list_iib_alarms
+            )
+
+        return vars_dict
+
     def check_param_bank(self, param_file: str):
 
         ps_param_list = []
 
         # max_sampling_freq = 600000
         # c28_sysclk = 150e6
```

### Comparing `pydrs-2.2.0/src/pydrs/bsmp/command.py` & `pydrs-2.3.0/src/pydrs/bsmp/command.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/bsmp/entities/parameters.py` & `pydrs-2.3.0/src/pydrs/bsmp/entities/parameters.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/bsmp/entities/ps.py` & `pydrs-2.3.0/src/pydrs/bsmp/entities/ps.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/bsmp/exceptions.py` & `pydrs-2.3.0/src/pydrs/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/bsmp/interface.py` & `pydrs-2.3.0/src/pydrs/bsmp/interface.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/bsmp/pwrsupply.py` & `pydrs-2.3.0/src/pydrs/bsmp/pwrsupply.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/consts/__init__.py` & `pydrs-2.3.0/src/pydrs/consts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 WRITE_FLOAT_SIZE_PAYLOAD = "\x00\x05"
 WRITE_DOUBLE_SIZE_PAYLOAD = "\x00\x03"
 COM_READ_VAR = "\x10\x00\x01"
 COM_REQUEST_CURVE = "\x40"
 COM_SEND_WFM_REF = "\x41"
 
-UDC_FIRMWARE_VERSION = "0.45.00    01/23"
+UDC_FIRMWARE_VERSION = "0.45.00    05/23"
 
 ufm_offset = {
     "serial": 0,
     "calibdate": 4,
     "variant": 9,
     "rburden": 10,
     "calibtemp": 12,
```

### Comparing `pydrs-2.2.0/src/pydrs/consts/common.py` & `pydrs-2.3.0/src/pydrs/consts/common.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/consts/fac.py` & `pydrs-2.3.0/src/pydrs/consts/fac.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/consts/fap.py` & `pydrs-2.3.0/src/pydrs/consts/fap.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/consts/fbp.py` & `pydrs-2.3.0/src/pydrs/consts/fbp.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/pydrs.py` & `pydrs-2.3.0/src/pydrs/pydrs.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/utils.py` & `pydrs-2.3.0/src/pydrs/utils.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs/validation.py` & `pydrs-2.3.0/src/pydrs/validation.py`

 * *Files identical despite different names*

### Comparing `pydrs-2.2.0/src/pydrs.egg-info/PKG-INFO` & `pydrs-2.3.0/src/pydrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrs
-Version: 2.2.0
+Version: 2.3.0
 License: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydrs-2.2.0/src/pydrs.egg-info/SOURCES.txt` & `pydrs-2.3.0/src/pydrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

