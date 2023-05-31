# Comparing `tmp/pysurfex-0.0.4.tar.gz` & `tmp/pysurfex-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysurfex-0.0.4.tar", max compression
+gzip compressed data, was "pysurfex-0.0.4.1.tar", max compression
```

## Comparing `pysurfex-0.0.4.tar` & `pysurfex-0.0.4.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     3318 2023-05-23 10:11:39.709958 pysurfex-0.0.4/README.rst
--rw-r--r--   0        0        0     5200 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      142 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/__init__.py
--rw-r--r--   0        0        0    25713 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/binary_input.py
--rw-r--r--   0        0        0    27141 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/binary_input_legacy.py
--rw-r--r--   0        0        0    18837 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/bufr.py
--rw-r--r--   0        0        0    10460 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cache.py
--rw-r--r--   0        0        0    19335 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/config.yml
--rw-r--r--   0        0        0     8835 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/config_exp_surfex.toml
--rw-r--r--   0        0        0      135 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/default_thredds.cfg
--rw-r--r--   0        0        0     5253 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/first_guess.yml
--rw-r--r--   0        0        0      192 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/qc_codes.json
--rw-r--r--   0        0        0      370 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/user.yml
--rw-r--r--   0        0        0    65246 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/cli.py
--rw-r--r--   0        0        0    61684 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/cmd_parsing.py
--rw-r--r--   0        0        0    32484 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/configuration.py
--rw-r--r--   0        0        0     1291 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/datetime_utils.py
--rw-r--r--   0        0        0     8730 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/ecoclimap.py
--rw-r--r--   0        0        0     3891 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/fa.py
--rw-r--r--   0        0        0    58096 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/file.py
--rw-r--r--   0        0        0    35668 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/forcing.py
--rw-r--r--   0        0        0    32941 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/geo.py
--rw-r--r--   0        0        0    22471 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/grib.py
--rw-r--r--   0        0        0    14928 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/input_methods.py
--rw-r--r--   0        0        0    18924 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/interpolation.py
--rw-r--r--   0        0        0    24223 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/namelist.py
--rw-r--r--   0        0        0   100554 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/namelist_legacy.py
--rw-r--r--   0        0        0    34770 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/netcdf.py
--rw-r--r--   0        0        0    37729 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/obs.py
--rw-r--r--   0        0        0     4483 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/observation.py
--rw-r--r--   0        0        0    12016 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/obsmon.py
--rw-r--r--   0        0        0     6415 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/obsoul.py
--rw-r--r--   0        0        0    18146 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/platform_deps.py
--rw-r--r--   0        0        0       20 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/plot.py
--rw-r--r--   0        0        0    17168 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/read.py
--rw-r--r--   0        0        0    11679 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/run.py
--rw-r--r--   0        0        0     2254 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/assimilation.json
--rw-r--r--   0        0        0        0 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/filetype.json
--rw-r--r--   0        0        0     1075 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/forecast.json
--rw-r--r--   0        0        0     1305 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/pgd.json
--rw-r--r--   0        0        0      952 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/prep.json
--rw-r--r--   0        0        0     3499 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/timeseries.py
--rw-r--r--   0        0        0    67688 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/titan.py
--rw-r--r--   0        0        0     3463 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/util.py
--rw-r--r--   0        0        0    19977 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/variable.py
--rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 pysurfex-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3318 2023-05-31 17:25:52.357264 pysurfex-0.0.4.1/README.rst
+-rw-r--r--   0        0        0     5202 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/__init__.py
+-rw-r--r--   0        0        0    28033 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/binary_input.py
+-rw-r--r--   0        0        0    27141 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/binary_input_legacy.py
+-rw-r--r--   0        0        0    18837 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/bufr.py
+-rw-r--r--   0        0        0    10460 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/cache.py
+-rw-r--r--   0        0        0    19335 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/cfg/config.yml
+-rw-r--r--   0        0        0     8836 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/cfg/config_exp_surfex.toml
+-rw-r--r--   0        0        0      135 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/cfg/default_thredds.cfg
+-rw-r--r--   0        0        0     5253 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/cfg/first_guess.yml
+-rw-r--r--   0        0        0      192 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/cfg/qc_codes.json
+-rw-r--r--   0        0        0      370 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/cfg/user.yml
+-rw-r--r--   0        0        0    65246 2023-05-31 17:25:52.361264 pysurfex-0.0.4.1/pysurfex/cli.py
+-rw-r--r--   0        0        0    61684 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/cmd_parsing.py
+-rw-r--r--   0        0        0    32484 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/configuration.py
+-rw-r--r--   0        0        0     1484 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/datetime_utils.py
+-rw-r--r--   0        0        0     8730 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/ecoclimap.py
+-rw-r--r--   0        0        0     3891 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/fa.py
+-rw-r--r--   0        0        0    58305 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/file.py
+-rw-r--r--   0        0        0    35668 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/forcing.py
+-rw-r--r--   0        0        0    32941 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/geo.py
+-rw-r--r--   0        0        0    22471 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/grib.py
+-rw-r--r--   0        0        0    14928 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/input_methods.py
+-rw-r--r--   0        0        0    18924 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/interpolation.py
+-rw-r--r--   0        0        0    23376 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/namelist.py
+-rw-r--r--   0        0        0   100554 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/namelist_legacy.py
+-rw-r--r--   0        0        0    34853 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/netcdf.py
+-rw-r--r--   0        0        0    37729 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/obs.py
+-rw-r--r--   0        0        0     4483 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/observation.py
+-rw-r--r--   0        0        0    12016 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/obsmon.py
+-rw-r--r--   0        0        0     6415 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/obsoul.py
+-rw-r--r--   0        0        0    18146 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/platform_deps.py
+-rw-r--r--   0        0        0       20 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/plot.py
+-rw-r--r--   0        0        0    17168 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/read.py
+-rw-r--r--   0        0        0    11394 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/run.py
+-rw-r--r--   0        0        0     2254 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/settings/assimilation.json
+-rw-r--r--   0        0        0        0 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/settings/filetype.json
+-rw-r--r--   0        0        0     1075 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/settings/forecast.json
+-rw-r--r--   0        0        0     1305 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/settings/pgd.json
+-rw-r--r--   0        0        0      952 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/settings/prep.json
+-rw-r--r--   0        0        0     3499 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/timeseries.py
+-rw-r--r--   0        0        0    67688 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/titan.py
+-rw-r--r--   0        0        0     3463 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/util.py
+-rw-r--r--   0        0        0    19977 2023-05-31 17:25:52.365264 pysurfex-0.0.4.1/pysurfex/variable.py
+-rw-r--r--   0        0        0     4606 1970-01-01 00:00:00.000000 pysurfex-0.0.4.1/PKG-INFO
```

### Comparing `pysurfex-0.0.4/README.rst` & `pysurfex-0.0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pyproject.toml` & `pysurfex-0.0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "pysurfex"
-    version = "0.0.4"
+    version = "0.0.4.1"
     description = "Python API to SURFEX"
     authors = ["Trygve Aspelien"]
     license = "MIT"
     readme = "README.rst"
     repository = "https://github.com/metno/pysurfex"
     documentation = "https://metno.github.io/pysurfex/"
```

### Comparing `pysurfex-0.0.4/pysurfex/binary_input.py` & `pysurfex-0.0.4.1/pysurfex/binary_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,14 @@
 """Input data for surfex binaries."""
 import json
 import logging
 import os
 import subprocess
 from abc import ABC, abstractmethod
 
-"""
-def binary_input_data():
-    return {
-        "pgd": {
-            "NAM_FRAC#LECOSG": {
-                "True": {
-                    "macros": {
-                        "VTYPE": {"fmt": "02d"},
-                        "DECADE": {"ntime": "NAM_DATA_ISBA#NTIME"},
-                    },
-                    "NAM_DATA_ISBA#CFTYP_ALBNIR_SOIL": {
-                        "DIRTYP": {
-                            "NAM_DATA_ISBA#CFNAM_ALBNIR_SOIL": "@ecoclimap_sg@/ALB_@VTYPE@_@DECADE@"
-                        }
-                    },
-                },
-                "False": {
-                    "ecoclimapI_covers_param.bin": "@ecoclimap_bin_dir@/ecoclimapI_covers_param.bin",
-                    "ecoclimapII_eu_covers_param.bin": "@ecoclimap_bin_dir@/ecoclimapII_eu_covers_param.bin",
-                    "ecoclimapII_af_covers_param.bin": "@ecoclimap_bin_dir@/ecoclimapII_af_covers_param.bin",
-                },
-            },
-            "NAM_ZS#YFILETYPE": {"DIRECT": {"NAM_ZS#YFILE": "@gmted@/gmted2010"}},
-        },
-        "prep": {},
-    }
-"""
-
 
 class InputDataToSurfexBinaries(ABC):
     """Abstract input data."""
 
     @abstractmethod
     def __init__(self):
         """Construct."""
@@ -205,15 +177,15 @@
             self.data = input_data[program]
         except KeyError:
             raise RuntimeError(f"Could not find program {program}") from KeyError
         data = self.process_data()
         JsonInputData.__init__(self, data)
 
     @staticmethod
-    def get_nml_value(nml, block, key, indices=None):
+    def get_nml_value2(nml, block, key, indices=None):
         """Get namelist value.
 
         Args:
             nml (nmlf90.Namelist): Namelist
             block (str): Namelist block
             key (str): Namelist key
             indices (list, optional): Indices to read. Defaults to None.
@@ -244,14 +216,95 @@
                     val = nml[block][key]
 
                 logging.debug("Found: %s Indices=%s", val, indices)
                 return val
         return None
 
     @staticmethod
+    def get_nml_value(nml, block, key, indices=None):
+        """Get namelist value.
+
+        Args:
+            nml (nmlf90.Namelist): Namelist
+            block (str): Namelist block
+            key (str): Namelist key
+            indices (list, optional): Indices to read. Defaults to None.
+
+        Returns:
+            setting (any): Namelist setting
+
+        """
+        logging.debug("Checking block=%s key=%s", block, key)
+        if block in nml:
+            if key in nml[block]:
+                vals = []
+                val_dict = {}
+                val = nml[block][key]
+                logging.debug("namelist type=%s", type(val))
+                if indices is not None:
+                    logging.debug("indices=%s", indices)
+                    if len(indices) == 2:
+                        val = nml[block][key][indices[1]][indices[0]]
+                    else:
+                        val = nml[block][key][indices[0]]
+                        logging.debug("Found 1D value %s", val)
+                        if isinstance(val, list):
+                            return None
+                    val_dict.update({"value": val, "indices": None})
+                    vals.append(val_dict)
+
+                else:
+                    if isinstance(val, list):
+                        dim_size = len(val)
+                        dims = []
+                        tval = val
+                        while dim_size != 1:
+                            logging.debug("tval=%s", tval)
+                            if isinstance(tval, int):
+                                dim_size = 1
+                            else:
+                                dim_size = len(tval)
+                                if dim_size != 1:
+                                    dims.append(dim_size)
+                                tval = tval[0]
+
+                        logging.debug("dims=%s", dims)
+                        logging.debug("type(val)=%s", type(val))
+                        if len(dims) - 1 == 2:
+                            for i in range(0, dims[0]):
+                                for j in range(0, dims[1]):
+                                    val_dict = {}
+                                    indices = [j, i]
+                                    lval = val[i][j]
+                                    val_dict.update({"value": lval, "indices": indices})
+                                    logging.debug("value=%s indices=%s", lval, indices)
+                                    vals.append(val_dict)
+                        elif len(dims) - 1 == 1:
+                            for i in range(0, dims[0]):
+                                val_dict = {}
+                                indices = [i]
+                                val_dict.update({"value": val[i], "indices": indices})
+                                logging.debug("value=%s indices=%s", val[i], indices)
+                                vals.append(val_dict)
+                        elif len(dims) - 1 == 0:
+                            val_dict = {}
+                            val_dict.update({"value": val, "indices": None})
+                            vals.append(val_dict)
+                    else:
+                        val_dict = {}
+                        if isinstance(val, bool):
+                            val = str(val)
+                        val_dict.update({"value": val, "indices": None})
+                        vals.append(val_dict)
+
+                logging.debug("Found: value=%s", val_dict["value"])
+                return vals
+        return None
+
+    @staticmethod
     def get_nml_value_from_string(nml, string, sep="#", indices=None):
         """Get namelist value from a string.
 
         Args:
             nml (nmlf90.Namelist): Namelist
             string (str): Namelist identifier
             sep (str, optional): _description_. Defaults to "#".
@@ -302,15 +355,15 @@
         )
         pval = self.platform.parse_setting(
             pval,
             validtime=self.validtime,
             basedtg=self.basetime,
             check_parsing=check_parsing,
         )
-        return {pkey: pval}
+        return pkey, pval
 
     def read_macro_setting(self, macro_defs, key, default=None, sep="#"):
         """Read a macro setting.
 
         Args:
             macro_defs (dict): Macro definition
             key (str): Macro setting to get.
@@ -322,14 +375,16 @@
         """
         try:
             setting = macro_defs[key]
             if isinstance(setting, str):
                 if setting.find(sep) > 0:
                     logging.debug("Read macro setting from namelist %s", setting)
                     setting = self.get_nml_value_from_string(self.nml, setting)
+                    if isinstance(setting, list):
+                        setting = setting[0]["value"]
             return setting
         except KeyError:
             return default
 
     def extend_macro(self, key, val, macros, sep="#"):
         """Extend entries from macro.
 
@@ -342,15 +397,15 @@
         Raises:
             NotImplementedError: _description_
             NotImplementedError: _description_
 
         Returns:
             dict: Key, value dictionary
         """
-        logging.debug("macros=%s", macros)
+        logging.debug("extenders=%s", macros)
         if macros is None:
             return {key: val}
 
         processed_data = {}
         for macro, macro_types in macros.items():
             loop = {}
             for macro_type, macro_defs in macro_types.items():
@@ -369,15 +424,15 @@
                         if nncv == 1:
                             loop.update({str(icounter1): str(icounter2)})
                             icounter1 += 1
                         icounter2 += 1
                 elif macro_type == "dict":
                     values = self.get_nml_value_from_string(self.nml, macro_defs)
                     counter = 0
-                    for key, val in values.items():
+                    for key, val in values[0].items():
                         loop.update({str(key): str(val)})
                         counter += 1
 
                 elif macro_type == "iterator":
                     start = self.read_macro_setting(macro_defs, "start", sep=sep)
                     end = self.read_macro_setting(macro_defs, "end", sep=sep)
                     fmt = self.read_macro_setting(
@@ -417,48 +472,47 @@
         logging.debug("Processed data=%s", processed_data)
         return processed_data
 
     def process_macro(self, key, val, macros, sep="#", indices=None):
         """Process macro.
 
         Args:
-            key (_type_): _description_
-            val (_type_): _description_
+            key (str): Key
+            val (str): Value
             macros (dict): Macros
             sep (str, optional): Namelist key separator. Defaults to "#".
             indices (list, optional): Process macro from namelist indices.
 
         Raises:
-            NotImplementedError: _description_
-            NotImplementedError: _description_
+            NotImplementedError: Only 2 dimensions are implemented
 
         Returns:
             dict: Key, value dictionary
         """
         logging.debug("macros=%s", macros)
         if macros is None:
-            return {key: val}
+            return key, val
 
         logging.debug("indices=%s", indices)
         if indices is None:
-            return {key: val}
+            return key, val
 
         pkey = key
         pval = val
         for macro in macros:
             lindex = None
             if len(indices) == 2:
                 if macro == "DECADE":
                     lindex = indices[1]
                 else:
                     lindex = indices[0]
             elif len(indices) == 1:
                 lindex = indices[0]
             elif len(indices) > 2:
-                raise NotImplementedError
+                raise NotImplementedError("Only 2 dimensions are implemented")
 
             vmacro = None
             if lindex is not None:
                 try:
                     macro_defs = macros[macro]
                     logging.debug("macro_defs=%s", macro_defs)
                 except KeyError:
@@ -480,198 +534,195 @@
                         month = int(day / 30) + 1
                         mday = int(day % 30)
                         if dec == lindex:
                             vmacro = f"{month:02d}{mday:02d}"
                         dec += 1
 
                 logging.debug("Substitute @%s@ with %s", macro, vmacro)
-                pkey = pkey.replace(f"@{macro}@", vmacro)
-                pval = pval.replace(f"@{macro}@", vmacro)
-        return {pkey: pval}
+                if isinstance(pkey, str):
+                    pkey = pkey.replace(f"@{macro}@", vmacro)
+                if isinstance(pval, str):
+                    pval = pval.replace(f"@{macro}@", vmacro)
+        return pkey, pval
 
     def matching_value(self, data, val, sep="#", indices=None):
         """Match the value. Possibly also read namelist value.
 
         Args:
             data (dict): Data to check keys for
             val (str): Key to find
             sep (str, optional): Namelist separator. Defaults to "#".
             indices(list, optional): Indices in namelist
 
         Raises:
-            TypeError: Data must be a dict or string
+            RuntimeError: "Malformed input data"
 
         Returns:
             dict: Matching entry in data.
+
         """
-        if val is not None:
-            val = str(val)
+        if val == "macro" or val == "extenders":
+            return None
         if isinstance(data, dict):
-            skeys = list(data.keys())
-        elif isinstance(data, str):
-            skeys = [data]
+            mdata = data.keys()
         else:
-            raise TypeError
-
-        logging.debug("Check for val=%s in skeys=%s", val, skeys)
-        for skey in skeys:
-            skey_ms = [skey]
-            if skey.find(sep) > 0:
-                logging.debug("skey=%s is a namelist variable", skey)
-                skey_m = self.get_nml_value_from_string(self.nml, skey, indices=indices)
-
-                if isinstance(skey_m, list):
-                    skey_ms = skey_m
-                else:
-                    skey_ms = [skey_m]
-
-            found_data = []
-            for skey_m in skey_ms:
-                logging.debug("matching val=%s skey=%s skey_m=%s", val, skey, skey_m)
-                if val is not None and val == skey_m:
-                    logging.debug("Found %s. data=%s", val, data)
-                    if skey.find(sep) > 0:
-                        if isinstance(data[skey], dict):
-                            found_data.append(data[skey][skey_m])
-                        elif isinstance(data[skey], str):
-                            found_data.append(data[skey])
-                        else:
-                            found_data.append({skey_m: data[skey]})
-                    else:
-                        found_data.append(data[skey])
-
-            logging.debug("found_data=%s", found_data)
-            if len(found_data) > 0:
-                if len(found_data) == 1:
-                    return found_data[0]
-                return found_data
+            mdata = [data]
+        val = str(val)
+        logging.debug("Check if val=%s matches mdata=%s", val, mdata)
+        sval = None
+        for mval in mdata:
+            if val.find(sep) > 0:
+                logging.debug("val=%s is a namelist variable", val)
+                sval = self.get_nml_value_from_string(self.nml, val, indices=indices)
+                logging.debug("Got sval=%s", sval)
+                if sval is None:
+                    return None
+                indices = sval[0]["indices"]
+                sval = sval[0]["value"]
+            if mval == val:
+                logging.debug("Found matching data. val=%s data=%s", val, data)
+                try:
+                    rval = data[val]
+                except TypeError:
+                    raise RuntimeError("Malformed input data") from TypeError
+                if sval is not None:
+                    rval = {sval: rval}
+                logging.debug("Return data rval=%s", rval)
+                return rval
         logging.warning("Value=%s not found in data", val)
         return None
 
     def process_data(self, sep="#"):
-        """Process input definitions on files to map."""
-        data = {}
+        """Process input definitions on files to map.
+
+        Args:
+            sep (str, optional): Namelist separator. Defaults to "#".
+
+        Returns:
+            mapped_data (dict): A dict with mapped local names and target files.
+
+        """
         logging.debug("Process data: %s", self.data)
-        for key, value in self.data.items():
-            logging.debug("key=%s", key)
-            # Required namelist variable
-            if key.find(sep) > 0:
-                val = self.get_nml_value_from_string(self.nml, key)
-                setting = self.matching_value(value, val, sep=sep)
-                if setting is not None:
-
-                    unprocessed_data = {}
-                    macros = None
-                    if "macros" in setting:
-                        macros = setting["macros"]
-                    extenders = None
-                    if "extenders" in setting:
-                        extenders = setting["extenders"]
-                    for key1, value1 in setting.items():
-                        logging.debug("key1 %s value1 %s", key1, value1)
-                        # Macro definition
-                        if key1 == "macros" or key1 == "extenders":
-                            pass
-                        # Extra namelist level
-                        elif key1.find(sep) > 0:
-                            logging.debug("Key1=%s is a namelist variable", key1)
-                            val1 = self.get_nml_value_from_string(self.nml, key1)
-                            indices = None
-                            if isinstance(val1, list):
-
-                                logging.debug("Got a namelist list variable")
-                                indices = []
-                                vals1 = []
-                                for i, vals in enumerate(val1):
-                                    if isinstance(vals, list):
-                                        logging.debug(
-                                            "i=%s len(vals)=%s val1=%s",
-                                            i,
-                                            len(vals),
-                                            val1,
-                                        )
-                                        for j in range(0, len(vals)):
-                                            ind = [j, i]
-                                            vals1.append(val1[i][j])
-                                            indices.append(ind)
-                                    else:
-                                        vals1.append(val1[i])
-                                        indices.append([i])
+
+        def _process_data(mapped_data, data, indices=None, macros=None, extenders=None):
+            for key, value in data.items():
+                logging.debug(".................. key=%s", key)
+                # Required namelist variable
+                if key.find(sep) > 0:
+                    vals = self.get_nml_value_from_string(self.nml, key, indices=indices)
+                else:
+                    vals = [{"value": value, "indices": None}]
+
+                if isinstance(vals, list):
+                    for val_dict in vals:
+                        logging.debug("=========== val_dict=%s", val_dict)
+                        val = val_dict["value"]
+                        indices = val_dict["indices"]
+
+                        setting = self.matching_value(
+                            value, val, sep=sep, indices=indices
+                        )
+                        logging.debug("Setting=%s", setting)
+                        if setting is not None:
+                            if "macros" in setting:
+                                macros = setting.copy()
+                                macros = macros["macros"]
+                            if "extenders" in setting:
+                                extenders = setting.copy()
+                                extenders = extenders["extenders"]
+
+                            last_dict = True
+                            if isinstance(setting, dict):
+                                for __, tval in setting.items():
+                                    if isinstance(tval, dict):
+                                        last_dict = False
                             else:
-                                vals1 = [val1]
-                            for ind, val1 in enumerate(vals1):
+                                print(setting)
+                            if not last_dict:
                                 logging.debug(
-                                    "ind=%s Checking for val1=%s in setting=%s",
-                                    ind,
-                                    val1,
-                                    setting,
+                                    "------ Call next loop. setting=%s", setting
                                 )
-                                if indices is not None:
-                                    lindices = indices[ind]
-                                else:
-                                    lindices = None
-                                setting1 = self.matching_value(
-                                    setting, val1, sep=sep, indices=lindices
+                                _process_data(
+                                    mapped_data,
+                                    setting,
+                                    indices=indices,
+                                    macros=macros,
+                                    extenders=extenders,
                                 )
-                                if setting1 is not None:
+                            else:
+                                for key2, value2 in setting.items():
+                                    logging.debug(
+                                        "Setting1 key=%s value=%s indices=%s",
+                                        key2,
+                                        value2,
+                                        indices,
+                                    )
+                                    if key2.find(sep) > 0:
+                                        keys = self.get_nml_value_from_string(
+                                            self.nml, key2, indices=indices
+                                        )
+                                        key2 = keys[0]["value"]
+
+                                    processed = False
                                     logging.debug(
-                                        "key1=%s val1=%s Setting1=%s",
-                                        key1,
-                                        val1,
-                                        setting1,
+                                        "Setting2 key=%s value=%s indices=%s",
+                                        key2,
+                                        value2,
+                                        indices,
                                     )
-                                    if isinstance(setting1, str):
-                                        unprocessed_data.update({val1: setting1})
-                                    else:
-                                        logging.debug(
-                                            "setting1=%s, lindices=%s", setting1, lindices
+                                    if macros is not None:
+                                        processed = True
+                                        key3, value3 = self.process_macro(
+                                            key2, value2, macros, indices=indices
                                         )
-                                        for key2, value2 in setting1.items():
-                                            if key2.find(sep) > 0:
-                                                key2 = self.get_nml_value_from_string(
-                                                    self.nml, key2, indices=lindices
-                                                )
-
-                                            logging.debug("key2=%s", key2)
-                                            sub_macros = self.process_macro(
-                                                key2, value2, macros, indices=lindices
+                                        if value3.endswith(".dir"):
+                                            dir_key = key3 + ".dir"
+                                            dir_val = value3
+                                            hdr_key = key3 + ".hdr"
+                                            hdr_val = value3.replace(".dir", ".hdr")
+                                            hdr_key, hdr_val = self.substitute(
+                                                hdr_key, hdr_val
                                             )
+                                            dir_key, dir_val = self.substitute(
+                                                dir_key, dir_val
+                                            )
+                                            mapped_data.update({hdr_key: hdr_val})
+                                            mapped_data.update({dir_key: dir_val})
+                                        else:
+                                            mapped_data.update({key3: setting})
+
+                                    if extenders is not None:
+                                        processed = True
+                                        processed_values = self.extend_macro(
+                                            key2, value2, extenders
+                                        )
+                                        for pkey3, pval3 in processed_values.items():
                                             logging.debug(
-                                                "Substituted macros %s", sub_macros
+                                                "pkey3=%s pval3=%s", pkey3, pval3
                                             )
-                                            unprocessed_data.update(sub_macros)
-                                else:
-                                    logging.warning(
-                                        "Could not match namelist variable %s", key1
-                                    )
-                        # Direct defintions
-                        else:
-                            if isinstance(value1, str):
-                                logging.debug("key1=%s value1=%s", key1, value1)
-                                unprocessed_data.update({key1: value1})
-                            else:
-                                logging.warning("Did not find a string %s", type(value1))
+                                            pkey3, pval3 = self.substitute(pkey3, pval3)
+                                            logging.debug(
+                                                "pkey3=%s pval3=%s", pkey3, pval3
+                                            )
+                                            mapped_data.update({pkey3: pval3})
 
-                    logging.debug(
-                        "Manipulate unprocesessed values with general"
-                        " or user-defined macros %s",
-                        unprocessed_data,
-                    )
-                    for key, value in unprocessed_data.items():
-                        logging.debug("key=%s value=%s", key, value)
-                        if isinstance(value, str):
-                            if value.endswith(".dir"):
-                                hdr_key = key + ".hdr"
-                                hdr_val = value.replace(".dir", ".hdr")
-                                sub_values = self.substitute(hdr_key, hdr_val)
-                                data.update(sub_values)
-                                key = key + ".dir"
-
-                        processed_values = self.extend_macro(key, value, extenders)
-                        for key, val in processed_values.items():
-                            sub_values = self.substitute(key, val)
-                            data.update(sub_values)
+                                    if not processed:
+                                        pkey3 = key2
+                                        pval3 = value2
+                                        logging.debug("pkey3=%s pval3=%s", pkey3, pval3)
+                                        pkey3, pval3 = self.substitute(pkey3, pval3)
+                                        mapped_data.update({pkey3: pval3})
+
+                                indices = None
+                        else:
+                            if key not in ["macros", "extenders"]:
+                                logging.warning(
+                                    "Could not match key=%s value=%s", key, val
+                                )
                 else:
-                    logging.warning("Could not find the namelist value=%s", val)
-            else:
-                logging.warning("Expected a namelist variable")
-        return data
+                    logging.warning("Could not find namelist key=%s", key)
+                    indices = None
+
+        mapped_data = {}
+        _process_data(mapped_data, self.data)
+        logging.debug("Mapped data=%s", mapped_data)
+        return mapped_data
```

### Comparing `pysurfex-0.0.4/pysurfex/binary_input_legacy.py` & `pysurfex-0.0.4.1/pysurfex/binary_input_legacy.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/bufr.py` & `pysurfex-0.0.4.1/pysurfex/bufr.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/cache.py` & `pysurfex-0.0.4.1/pysurfex/cache.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/cfg/config.yml` & `pysurfex-0.0.4.1/pysurfex/cfg/config.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/cfg/config_exp_surfex.toml` & `pysurfex-0.0.4.1/pysurfex/cfg/config_exp_surfex.toml`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 YSOC_SUB = "soc_sub"                # Soil organic carbon data. Options: "soc_sub"
 
 YSAND = 'sand_fao'                  # Soil texture input data: "sand_fao"|"SAND_HWSD_MOY_V2"|"sand_SOILGRID"
                                     # suffix json assumes namelist values provided as a json file
 
 YCLAY = "clay_fao"                  # Soil texture input data: "clay_fao"|"CLAY_HWSD_MOY_V2"|"clay_SOILGRID"
                                     # suffix json assumes namelist values provided as a json file
-PERTSURF = true                    # Perturb surface parameters
+PERTSURF = false                    # Perturb surface parameters
 XCGMAX = 2.0E-5                     # Maximum value for soil heat capacity; default=2.0E-5
 XCSMAX = 2.0E-4                     # Maximum value for snow heat capacity; default=2.0E-4
 
 # Sub-grid-scale orography settings
 [SURFEX.SSO]
 SCHEME = "NONE"                     # SSO scheme used in SURFEX "NONE"|"'Z01D'"|"'BE04'"|"'OROT'"
```

### Comparing `pysurfex-0.0.4/pysurfex/cfg/first_guess.yml` & `pysurfex-0.0.4.1/pysurfex/cfg/first_guess.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/cli.py` & `pysurfex-0.0.4.1/pysurfex/cli.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/cmd_parsing.py` & `pysurfex-0.0.4.1/pysurfex/cmd_parsing.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/configuration.py` & `pysurfex-0.0.4.1/pysurfex/configuration.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/datetime_utils.py` & `pysurfex-0.0.4.1/pysurfex/datetime_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 #!/usr/bin/env python3
 """Implement helper routines to deal with dates and times."""
-from datetime import date, datetime, timedelta
+from datetime import date, datetime, timedelta, timezone
 
 
 # TODO use ISO times
 def as_datetime(dtg):
     """Convert string to datetime."""
     if len(dtg) == 10:
         fmt = "%Y%m%d%H"
     elif len(dtg) == 12:
         fmt = "%Y%m%d%H%M"
     elif len(dtg) == 14:
         fmt = "%Y%m%d%H%M%S"
     else:
         raise RuntimeError(f"dtg={dtg} len(dtg) is {len(dtg)}")
-
-    return datetime.strptime(dtg, fmt)
+    return datetime.strptime(dtg, fmt).replace(tzinfo=timezone.utc)
 
 
 def as_datetime_string(dtg):
     """Convert string to datetime."""
     fmt = "%Y%m%d%H%M%S"
     return dtg.strftime(fmt)
 
 
+def offsetaware(dtg):
+    """Make offset aware."""
+    return dtg.replace(tzinfo=timezone.utc)
+
+
 def as_timedelta(seconds=0):
     """Convert seconds to timedelta."""
     return timedelta(seconds=seconds)
 
 
 def fromtimestamp(validtime):
     """Convert timestamp to validtime."""
     return datetime.fromtimestamp(validtime)
 
 
 def utcfromtimestamp(epochtime):
     """Convert timestamp to validtime."""
-    return datetime.utcfromtimestamp(epochtime)
+    return datetime.utcfromtimestamp(epochtime).replace(tzinfo=timezone.utc)
 
 
 def isdatetime(obj):
     """Check if is a datetime objects."""
     return isinstance(obj, date)
 
 
 def as_datetime_args(year=None, month=None, day=None, hour=0, minute=0, second=0):
     """Set datetime object from args."""
     return datetime(
         year=year, month=month, day=day, hour=hour, minute=minute, second=second
-    )
+    ).replace(tzinfo=timezone.utc)
```

### Comparing `pysurfex-0.0.4/pysurfex/ecoclimap.py` & `pysurfex-0.0.4.1/pysurfex/ecoclimap.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/fa.py` & `pysurfex-0.0.4.1/pysurfex/fa.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/file.py` & `pysurfex-0.0.4.1/pysurfex/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -911,15 +911,21 @@
                     year=year, month=month, day=day, hour=hour
                 )
             except IndexError:
                 logging.warning("Could not checking time")
 
             if time_in_file is not None:
                 if validtime != time_in_file:
-                    logging.error("%s %s", time_in_file, validtime)
+                    logging.error(
+                        "time_in_file=%s validtime=%s %s %s",
+                        time_in_file,
+                        validtime,
+                        type(time_in_file),
+                        type(validtime),
+                    )
                     raise RuntimeError("Mismatch in times in file and the wanted time")
 
         geo_in = self.get_geo()
         field = f_h[var.varname][:]
         fillvalue = f_h[var.varname].getncattr("_FillValue")
         logging.info("Set %s to nan", fillvalue)
         field = field.filled(np.nan)
```

### Comparing `pysurfex-0.0.4/pysurfex/forcing.py` & `pysurfex-0.0.4.1/pysurfex/forcing.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/geo.py` & `pysurfex-0.0.4.1/pysurfex/geo.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/grib.py` & `pysurfex-0.0.4.1/pysurfex/grib.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/input_methods.py` & `pysurfex-0.0.4.1/pysurfex/input_methods.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/interpolation.py` & `pysurfex-0.0.4.1/pysurfex/interpolation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/namelist.py` & `pysurfex-0.0.4.1/pysurfex/namelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,14 @@
             definitions (dict): Namelist definitions
             assemble(dict, optional): Assembly order. Default to None.
             consistency (bool, optional): Check configuration consistency. Defaults to True.
         """
         self.program = program
         self.config = config
         self.nldict = definitions
-        macros_defs = {
-            "CPGDFILE": "SURFEX#IO#CPGDFILE",
-            "CPREPFILE": "SURFEX#IO#CPREPFILE",
-            "CSURFFILE": "SURFEX#IO#CSURFFILE",
-            "CSURF_FILETYPE": "SURFEX#IO#CSURF_FILETYPE",
-            "CFORCING_FILETYPE": "SURFEX#IO#CFORCING_FILETYPE",
-            "CTIMESERIES_FILETYPE": "SURFEX#IO#CTIMESERIES_FILETYPE",
-            "XRIMAX": "SURFEX#PARAMETERS#XRIMAX",
-            "LSPLIT_PATCH": "SURFEX#IO#LSPLIT_PATCH",
-            "LFAKETREE": "SURFEX#TREEDRAG#FAKETREES",
-            "LECOSG": "SURFEX#COVER#SG",
-            "XTSTEP": "SURFEX#IO#XTSTEP",
-            "XTSTEP_OUTPUT ": "SURFEX#IO#XTSTEP_OUTPUT",
-        }
-        macros = {}
-        for macro, setting in macros_defs.items():
-            vmacro = config.get_setting(setting)
-            logging.debug("Mapping macro %s = %s", macro, vmacro)
-            if vmacro is not None:
-                macros.update({macro: vmacro})
 
         nobstype = 0
         if program == "soda" or program == "offline":
             nnco = self.config.get_setting("SURFEX#ASSIM#OBS#NNCO")
             nobstype = 0
             for __, obs_val in enumerate(nnco):
                 if obs_val == 1:
@@ -109,14 +89,16 @@
 
         def _flatten_dict_gen(dic, parent_key, sep):
             for key, val in dic.items():
                 new_key = parent_key + sep + key if parent_key else key
                 if isinstance(val, collections.abc.MutableMapping):
                     yield from flatten_dict(val, new_key, sep=sep).items()
                 else:
+                    if isinstance(val, tuple):
+                        val = list(val)
                     yield new_key, val
 
         def flatten_dict(
             d: collections.abc.MutableMapping, parent_key: str = "", sep: str = "#"
         ):
             return dict(_flatten_dict_gen(d, parent_key, sep))
```

### Comparing `pysurfex-0.0.4/pysurfex/namelist_legacy.py` & `pysurfex-0.0.4.1/pysurfex/namelist_legacy.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/netcdf.py` & `pysurfex-0.0.4.1/pysurfex/netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     cfunits = None
 except AssertionError:
     cfunits = None
 except:  # noqa
     cfunits = None
 
 
-from .datetime_utils import fromtimestamp, isdatetime, utcfromtimestamp
+from .datetime_utils import fromtimestamp, isdatetime, offsetaware, utcfromtimestamp
 from .geo import ConfProj, Geo
 from .interpolation import Interpolation
 
 
 class Netcdf(object):
     """Netcdf input."""
 
@@ -98,23 +98,24 @@
         else:
             if not isinstance(times, (list, tuple)):
                 raise ValueError("Times must be a list!")
             if isdatetime(times[0]):
                 logging.debug("Time provided in call as datetime objects")
                 times_in_var = var.datetimes
                 for i, times_in_var_val in enumerate(times_in_var):
+                    times_in_var_val = offsetaware(times_in_var_val)
                     logging.debug(
                         "i %s times_in_var %s times %s", i, times_in_var_val, times
                     )
                     for tval in times:
                         # Time steps requested
                         logging.debug(
                             "i=%s, times_in_var_val=%s tval=%s", i, times_in_var_val, tval
                         )
-                        if times_in_var[i] == tval:
+                        if times_in_var_val == tval:
                             times_to_read.append(i)
                             if i > 0:
                                 prev_time_steps.append(i - 1)
                             else:
                                 prev_time_steps.append(0)
 
             else:
```

### Comparing `pysurfex-0.0.4/pysurfex/obs.py` & `pysurfex-0.0.4.1/pysurfex/obs.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/observation.py` & `pysurfex-0.0.4.1/pysurfex/observation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/obsmon.py` & `pysurfex-0.0.4.1/pysurfex/obsmon.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/obsoul.py` & `pysurfex-0.0.4.1/pysurfex/obsoul.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/platform_deps.py` & `pysurfex-0.0.4.1/pysurfex/platform_deps.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/read.py` & `pysurfex-0.0.4.1/pysurfex/read.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/run.py` & `pysurfex-0.0.4.1/pysurfex/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,35 +192,27 @@
             surfout (_type_, optional): _description_. Defaults to None.
             archive_data (_type_, optional): _description_. Defaults to None.
             pgdfile (str, optional): _description_. Defaults to None.
             print_namelist (bool, optional): _description_. Defaults to False.
             negpert (bool, optional): _description_. Defaults to False.
 
         """
-        self.pert_number = pert_number
+        pert_number = int(pert_number)
         settings["nam_io_varassim"]["LPRT"] = True
-        settings["nam_var"]["nivar"] = int(pert_number)
+        settings["nam_var"]["nivar"] = pert_number
         # Handle negative pertubations
         if negpert:
-            nvar = int(settings["nam_var"]["nvar"])
-            ipert = 0
-            npert = 1
-            for nvi in range(0, nvar):
-                key = "nncv(" + str(nvi + 1) + ")"
-                val = int(settings["nam_var"][key])
-                # Check if active
-                if val == 1:
-                    npert = 1
-                else:
-                    npert = npert + 1
-                for __ in range(0, npert):
-                    ipert = ipert + 1
-                    key = "xtprt_m(" + str(ipert) + ")"
-                    val = settings["nam_var"][key]
-                    settings["nam_var"][key] = -val
+            nncv = settings["nam_var"]["nncv"]
+            nind = 0
+            for nvi, nval in enumerate(nncv):
+                if nval == 1:
+                    nind += 1
+                    if nind == pert_number:
+                        val = settings["nam_var"]["xtprt_m"][nvi]
+                        settings["nam_var"]["xtprt_m"][nvi] = -val
         SURFEXBinary.__init__(
             self,
             binary,
             batch,
             io,
             settings,
             input_data,
```

### Comparing `pysurfex-0.0.4/pysurfex/settings/assimilation.json` & `pysurfex-0.0.4.1/pysurfex/settings/assimilation.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/settings/forecast.json` & `pysurfex-0.0.4.1/pysurfex/settings/forecast.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/settings/pgd.json` & `pysurfex-0.0.4.1/pysurfex/settings/pgd.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/settings/prep.json` & `pysurfex-0.0.4.1/pysurfex/settings/prep.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/timeseries.py` & `pysurfex-0.0.4.1/pysurfex/timeseries.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/titan.py` & `pysurfex-0.0.4.1/pysurfex/titan.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/util.py` & `pysurfex-0.0.4.1/pysurfex/util.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/pysurfex/variable.py` & `pysurfex-0.0.4.1/pysurfex/variable.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.4/PKG-INFO` & `pysurfex-0.0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysurfex
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Python API to SURFEX
 Home-page: https://github.com/metno/pysurfex
 License: MIT
 Author: Trygve Aspelien
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

