# Comparing `tmp/simply_nwb-0.0.7.tar.gz` & `tmp/simply_nwb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply_nwb-0.0.7.tar", last modified: Fri May 26 15:53:59 2023, max compression
+gzip compressed data, was "simply_nwb-0.1.0.tar", last modified: Wed May 31 21:16:56 2023, max compression
```

## Comparing `simply_nwb-0.0.7.tar` & `simply_nwb-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:53:59.001367 simply_nwb-0.0.7/
--rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      566 2023-05-26 15:53:59.000367 simply_nwb-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-26 15:53:59.001367 simply_nwb-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-05-26 15:53:51.000000 simply_nwb-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.988346 simply_nwb-0.0.7/simply_nwb/
--rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.992344 simply_nwb-0.0.7/simply_nwb/acquisition/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/acquisition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.998361 simply_nwb-0.0.7/simply_nwb/acquisition/tools/
--rw-rw-rw-   0        0        0      181 2023-05-19 17:18:00.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/__init__.py
--rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/blackrock.py
--rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/csv.py
--rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/labjack.py
--rw-rw-rw-   0        0        0     2601 2023-05-23 15:16:58.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/mp4.py
--rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/p_erg.py
--rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/plaintext.py
--rw-rw-rw-   0        0        0     3874 2023-05-24 18:25:41.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/tif.py
--rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.0.7/simply_nwb/acquisition/tools/yaml.py
--rw-rw-rw-   0        0        0    24781 2023-05-23 18:43:23.000000 simply_nwb-0.0.7/simply_nwb/simple_nwb.py
--rw-rw-rw-   0        0        0    12850 2023-05-25 20:43:09.000000 simply_nwb-0.0.7/simply_nwb/testing.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.999367 simply_nwb-0.0.7/simply_nwb/transferring/
--rw-rw-rw-   0        0        0       31 2023-05-25 16:13:35.000000 simply_nwb-0.0.7/simply_nwb/transferring/__init__.py
--rw-rw-rw-   0        0        0     7693 2023-05-26 15:53:17.000000 simply_nwb-0.0.7/simply_nwb/transferring/nwb_transfer.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:53:59.000367 simply_nwb-0.0.7/simply_nwb/transforms/
--rw-rw-rw-   0        0        0        0 2023-05-18 16:57:25.000000 simply_nwb-0.0.7/simply_nwb/transforms/__init__.py
--rw-rw-rw-   0        0        0     7110 2023-05-25 18:00:05.000000 simply_nwb-0.0.7/simply_nwb/util.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:53:58.991345 simply_nwb-0.0.7/simply_nwb.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 15:53:58.000000 simply_nwb-0.0.7/simply_nwb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.477912 simply_nwb-0.1.0/
+-rw-rw-rw-   0        0        0    35819 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      566 2023-05-31 21:16:56.477912 simply_nwb-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-31 21:16:56.477912 simply_nwb-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-05-31 18:00:34.000000 simply_nwb-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.463890 simply_nwb-0.1.0/simply_nwb/
+-rw-rw-rw-   0        0        0       35 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/simply_nwb/__init__.py
+-rw-rw-rw-   0        0        0    27237 2023-05-31 18:00:34.000000 simply_nwb-0.1.0/simply_nwb/simple_nwb.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.469890 simply_nwb-0.1.0/simply_nwb/transferring/
+-rw-rw-rw-   0        0        0      514 2023-05-31 21:15:34.000000 simply_nwb-0.1.0/simply_nwb/transferring/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.470889 simply_nwb-0.1.0/simply_nwb/transferring/filesync/
+-rw-rw-rw-   0        0        0       38 2023-05-31 20:09:28.000000 simply_nwb-0.1.0/simply_nwb/transferring/filesync/__init__.py
+-rw-rw-rw-   0        0        0     7061 2023-05-31 21:13:35.000000 simply_nwb-0.1.0/simply_nwb/transferring/filesync/oneway.py
+-rw-rw-rw-   0        0        0     7339 2023-05-31 20:19:57.000000 simply_nwb-0.1.0/simply_nwb/transferring/nwb_transfer.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.476912 simply_nwb-0.1.0/simply_nwb/transforms/
+-rw-rw-rw-   0        0        0      179 2023-05-31 18:00:34.000000 simply_nwb-0.1.0/simply_nwb/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2971 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/simply_nwb/transforms/blackrock.py
+-rw-rw-rw-   0        0        0      565 2023-05-19 20:07:34.000000 simply_nwb-0.1.0/simply_nwb/transforms/csv.py
+-rw-rw-rw-   0        0        0     2607 2023-05-19 16:01:27.000000 simply_nwb-0.1.0/simply_nwb/transforms/labjack.py
+-rw-rw-rw-   0        0        0     1789 2023-05-31 15:31:44.000000 simply_nwb-0.1.0/simply_nwb/transforms/mp4.py
+-rw-rw-rw-   0        0        0     3827 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/simply_nwb/transforms/p_erg.py
+-rw-rw-rw-   0        0        0      705 2023-05-18 16:57:25.000000 simply_nwb-0.1.0/simply_nwb/transforms/plaintext.py
+-rw-rw-rw-   0        0        0     3874 2023-05-24 18:25:41.000000 simply_nwb-0.1.0/simply_nwb/transforms/tif.py
+-rw-rw-rw-   0        0        0      464 2023-05-19 20:07:49.000000 simply_nwb-0.1.0/simply_nwb/transforms/yaml.py
+-rw-rw-rw-   0        0        0     7593 2023-05-31 16:44:20.000000 simply_nwb-0.1.0/simply_nwb/util.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:16:56.467902 simply_nwb-0.1.0/simply_nwb.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 21:16:56.000000 simply_nwb-0.1.0/simply_nwb.egg-info/top_level.txt
```

### Comparing `simply_nwb-0.0.7/LICENSE` & `simply_nwb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.7/PKG-INFO` & `simply_nwb-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply_nwb
-Version: 0.0.7
+Version: 0.1.0
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.0.7/setup.py` & `simply_nwb-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.7"
+VERSION = "0.1.0"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

### Comparing `simply_nwb-0.0.7/simply_nwb/acquisition/tools/blackrock.py` & `simply_nwb-0.1.0/simply_nwb/transforms/blackrock.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.7/simply_nwb/acquisition/tools/csv.py` & `simply_nwb-0.1.0/simply_nwb/transforms/csv.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.7/simply_nwb/acquisition/tools/labjack.py` & `simply_nwb-0.1.0/simply_nwb/transforms/labjack.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.7/simply_nwb/acquisition/tools/p_erg.py` & `simply_nwb-0.1.0/simply_nwb/transforms/p_erg.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.7/simply_nwb/acquisition/tools/plaintext.py` & `simply_nwb-0.1.0/simply_nwb/transforms/plaintext.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.7/simply_nwb/acquisition/tools/tif.py` & `simply_nwb-0.1.0/simply_nwb/transforms/tif.py`

 * *Files identical despite different names*

### Comparing `simply_nwb-0.0.7/simply_nwb/simple_nwb.py` & `simply_nwb-0.1.0/simply_nwb/simple_nwb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from uuid import uuid4
 import os
-import sys
 import glob
 
 import numpy as np
 import pandas as pd
-import pendulum
+from hdmf.backends.hdf5 import H5DataIO
 from hdmf.common.table import DynamicTable
 from hdmf.common.table import VectorData
 from pynwb import NWBFile, TimeSeries
 from pynwb.behavior import BehavioralEvents
 from pynwb.device import Device
 from pynwb.ecephys import ElectrodeGroup
 from pynwb.file import Subject
 from pynwb.ophys import OpticalChannel, TwoPhotonSeries
 
-from .acquisition.tools import labjack_load_file
-from .acquisition.tools import blackrock_all_spiketrains, perg_parse_to_table
+from transforms import labjack_load_file
+from transforms import blackrock_all_spiketrains, perg_parse_to_table
 from .util import warn_on_name_format, inspect_nwb_obj, nwb_write, panda_df_to_dyn_table, \
     panda_df_to_list_of_timeseries, dict_to_dyn_tables
 
 
 class SimpleNWB(object):
     _REQUIRED_ARGS = [
         "session_description",
@@ -33,34 +32,50 @@
     @staticmethod
     def create_nwb(
             session_description=None,
             session_start_time=None,
             experimenter=None,
             lab=None,
             experiment_description=None,
+            institution=None,
             # Optional
             identifier=None,
             subject=None,
             session_id=None,
-            institution=None,
             keywords=None,
             related_publications=None
     ):
+        """
+        Create a new nwbfile from the given params. More infor here https://pynwb.readthedocs.io/en/stable/pynwb.file.html#pynwb.file.NWBFile
+
+        :param session_description: description of the session
+        :param session_start_time: start date and time of recording session
+        :param experimenter: name of experimenter, list of form ["Lastname, Firstname"]
+        :param lab: name of lab
+        :param experiment_description: experiment description
+        :param institution: institution
+        :param identifier: Optional identifier for the file, if not supplied will be generated
+        :param subject: Optional pynwb.file.Subject object for metadata
+        :param session_id: Optional lab-specific session id, if not supplied will be generated
+        :param keywords: Optional list of keywords e.g ["keyword1", "keyword2", ...]
+        :param related_publications: Optional related publications in a list of the DOI, URL, PMID etc ["DOI:1234/asdf"]
+        :return:
+        """
         for arg in SimpleNWB._REQUIRED_ARGS:
             # Required args
             if locals()[arg] is None:
                 raise ValueError("Did not provide '{}' to SimpleNWB()!".format(arg))
+            if institution is None:
+                raise ValueError("Must provide institution!")
 
             # Optional args
             if identifier is None:
                 identifier = str(uuid4())
             if session_id is None:
                 session_id = str(uuid4())
-            if institution is None:
-                institution = "CU Anschutz"
             if isinstance(subject, dict):
                 subject = Subject(**subject)
             elif not isinstance(subject, Subject) and not subject is None:
                 raise ValueError("'subject' argument must either be a dict or a pynwb.file.Subject type!")
 
             if keywords is None:
                 keywords = []
@@ -81,40 +96,82 @@
 
             return NWBFile(**nwb_kwargs)
 
     @staticmethod
     def inspect(nwbfile):
         """
         Inspect the given NWBFile
+
         :param nwbfile: NWBFile object
         :return: List of issues with the file, if empty, inspection passed
         """
 
         results = inspect_nwb_obj(nwbfile)
         return results
 
     @staticmethod
     def write(nwbfile, filename=None):
         """
         Write the give NWBFile object to file
+
         :param nwbfile: NWBFile object to write
         :param filename: path to file to write, WILL OVERWRITE!
         :return: None
         """
         nwb_write(nwbfile, filename)
 
     @staticmethod
+    def mp4_add_as_behavioral(
+            nwbfile,
+            name=None,
+            numpy_data=None,
+            frame_count=None,
+            sampling_rate=None,
+            description=None,
+            chunking=True,
+            compression=True
+    ):
+        """
+        Add a numpy array as behavioral data, meant to work in conjunction with the mp4
+
+        :param nwbfile: NWBFile to add the mp4 data to
+        :param name: Name of the movie
+        :param numpy_data: data, can be np.memmap
+        :param frame_count: number of total frames
+        :param sampling_rate: frames per second
+        :param description: description of the movie
+        :param chunking: Optional chunking for large files, defaults to True
+        :param compression: Optional compression for large files, defaults to True
+        :return: None
+        """
+
+        behavior_module = nwbfile.create_processing_module(name="behavior", description="test desc")
+        mp4_timeseries = TimeSeries(
+            name=name,
+            data=H5DataIO(
+                data=numpy_data[:frame_count],
+                compression=compression,
+                chunks=chunking
+            ),
+            description=description,
+            unit="mp4 video frame images",
+            rate=sampling_rate
+        )
+
+        behavior_module.add(mp4_timeseries)
+
+    @staticmethod
     def processing_add_dict(
             nwbfile,
             processed_name=None,
             processed_description=None,
             data_dict=None,
             uneven_columns=False):
         """
-        Add a processed dict into the NWB that doesn't fit in any other part of the NWB. MAKE SURE YOU CANT ADD IT ELSEWHERE BEFORE USING THIS FUNC!
+        Add a processed dict into the NWB that doesn't fit in any other part of the NWB. MAKE SURE YOU CANNOT ADD IT ELSEWHERE BEFORE USING THIS FUNC!
 
         :param nwbfile: NWBFile to add data to
         :param processed_name: Name of the processing module
         :param processed_description: description of the processed data
         :param data_dict: dict data to add
         :param uneven_columns: Set this to True if the keys of the dict have different lengths
         """
@@ -146,15 +203,15 @@
     def processing_add_dataframe(
             nwbfile,
             processed_name=None,
             processed_description=None,
             data=None
     ):
         """
-        Add a processed pandas Dataframe into the NWB that doesn't fit in any other part of the NWB. MAKE SURE YOU CANT ADD IT ELSEWHERE BEFORE USING THIS FUNC!
+        Add a processed pandas Dataframe into the NWB that doesn't fit in any other part of the NWB. MAKE SURE YOU CANNOT ADD IT ELSEWHERE BEFORE USING THIS FUNC!
 
         :param nwbfile: NWBFile to add data to
         :param processed_name: Name of the processing module
         :param processed_description: description of the processed data
         :param data: Pandas Dataframe data to add
         :return: None
         """
@@ -318,15 +375,15 @@
         """
         Add LabJack data to the NWBFile as a behavioral entry
 
         :param nwbfile: NWBFile to add the data to
         :param labjack_filename: LabJack filename to read from
         :param name: Name of this behavioral unit
         :param measured_unit_list: List of SI unit strings corresponding to the columns of the labjack data
-        :param start_time: start time float
+        :param start_time: start time float in Hz
         :param sampling_rate: sampling rate in Hz
         :param description: description of the behavioral data
         :param behavior_module: Optional NWB behavior module to add this data to, otherwise will create a new one e.g. nwbfile.processing["behavior"]
         :param behavior_module_name: optional module name to add this behavior to, if exists will append. will ignore if behavior_module arg is supplied
         :param comments: additional comments about the data
         :return:
         """
```

### Comparing `simply_nwb-0.0.7/simply_nwb/transferring/nwb_transfer.py` & `simply_nwb-0.1.0/simply_nwb/transferring/nwb_transfer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 import os
 import shutil
 import pendulum
 from simply_nwb.util import is_camel_case, is_snake_case, is_filesystem_safe, _print
 import glob
 
 
-# shutil Hack to increase the buffer size for copying large files faster
-def _copyfileobj_patched(fsrc, fdst, length=0):
-    """Patches shutil method to hugely improve copy speed"""
-    length = 256 * 1024 * 1024  # 256MB buffer size
-    while 1:
-        buf = fsrc.read(length)
-        if not buf:
-            break
-        fdst.write(buf)
-
-
-# Overwrite the shutil.copyfilyobj method
-shutil.copyfileobj = _copyfileobj_patched
-
-
 class NWBTransfer(object):
+    """
+    Class to aid in transferring data around in a structured way
+    """
+    
     TIMESTAMP_SUFFIX = "{day}_{month}_{year}-{hour}_{minute}_{second}"
 
     def __init__(
             self,
             nwb_file_location=None,
             raw_data_folder_location=None,
             lab_name=None,
```

### Comparing `simply_nwb-0.0.7/simply_nwb/util.py` & `simply_nwb-0.1.0/simply_nwb/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,24 +145,37 @@
     return DynamicTable(
         name=table_name,
         description=description,
         columns=v_columns
     )
 
 
-def panda_df_to_list_of_timeseries(pd_df=None, measured_unit_list=None, series_name_suffix="",
+def panda_df_to_list_of_timeseries(pd_df=None, measured_unit_list=None, series_name_prefix="",
                                    start_time=None, sampling_rate=None, description=None, comments=None):
+    """
+    Turns a panda dataframe into a list of TimeSeries objects
+
+
+    :param pd_df: dataframe to transform
+    :param measured_unit_list: list of units for each column of the dataframe
+    :param series_name_prefix: optional series prefix
+    :param start_time: time the data started for each timeseries
+    :param sampling_rate: sampling rate in Hz
+    :param description: description of this dataframe
+    :param comments: optional comments
+    :return:
+    """
     timeseries_list = []
     if len(measured_unit_list) != len(pd_df.columns):
         raise ValueError(
             f"Invalid 'measured_unit_list' does not match number of columns '{len(measured_unit_list)}' != '{len(pd_df.columns)}' Units: '{measured_unit_list}' Cols: '{pd_df.columns}'")
 
     for idx, col_name in enumerate(pd_df.columns):
         timeseries_list.append(TimeSeries(
-            name=f"{series_name_suffix}{col_name}",
+            name=f"{series_name_prefix}{col_name}",
             data=pd_df[col_name].to_numpy(),
             unit=measured_unit_list[idx],
             starting_time=start_time,
             rate=sampling_rate,
             description=f"column {col_name} {description}",
             comments=comments,
         ))
```

### Comparing `simply_nwb-0.0.7/simply_nwb.egg-info/PKG-INFO` & `simply_nwb-0.1.0/simply_nwb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-nwb
-Version: 0.0.7
+Version: 0.1.0
 Summary: Common NWB use cases and simplified interface for common usage
 Author: Spencer Hanson
 Keywords: neuroscience,nwb,tools,science
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 ###########
```

### Comparing `simply_nwb-0.0.7/simply_nwb.egg-info/SOURCES.txt` & `simply_nwb-0.1.0/simply_nwb.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 LICENSE
 README.rst
 setup.py
 simply_nwb/__init__.py
 simply_nwb/simple_nwb.py
-simply_nwb/testing.py
 simply_nwb/util.py
 simply_nwb.egg-info/PKG-INFO
 simply_nwb.egg-info/SOURCES.txt
 simply_nwb.egg-info/dependency_links.txt
 simply_nwb.egg-info/requires.txt
 simply_nwb.egg-info/top_level.txt
-simply_nwb/acquisition/__init__.py
-simply_nwb/acquisition/tools/__init__.py
-simply_nwb/acquisition/tools/blackrock.py
-simply_nwb/acquisition/tools/csv.py
-simply_nwb/acquisition/tools/labjack.py
-simply_nwb/acquisition/tools/mp4.py
-simply_nwb/acquisition/tools/p_erg.py
-simply_nwb/acquisition/tools/plaintext.py
-simply_nwb/acquisition/tools/tif.py
-simply_nwb/acquisition/tools/yaml.py
 simply_nwb/transferring/__init__.py
 simply_nwb/transferring/nwb_transfer.py
-simply_nwb/transforms/__init__.py
+simply_nwb/transferring/filesync/__init__.py
+simply_nwb/transferring/filesync/oneway.py
+simply_nwb/transforms/__init__.py
+simply_nwb/transforms/blackrock.py
+simply_nwb/transforms/csv.py
+simply_nwb/transforms/labjack.py
+simply_nwb/transforms/mp4.py
+simply_nwb/transforms/p_erg.py
+simply_nwb/transforms/plaintext.py
+simply_nwb/transforms/tif.py
+simply_nwb/transforms/yaml.py
```

