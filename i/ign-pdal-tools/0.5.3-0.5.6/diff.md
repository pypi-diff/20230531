# Comparing `tmp/ign-pdal-tools-0.5.3.tar.gz` & `tmp/ign-pdal-tools-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-pdal-tools-0.5.3.tar", last modified: Wed May 24 14:50:33 2023, max compression
+gzip compressed data, was "ign-pdal-tools-0.5.6.tar", last modified: Wed May 31 15:11:39 2023, max compression
```

## Comparing `ign-pdal-tools-0.5.3.tar` & `ign-pdal-tools-0.5.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 GLiegard (16037) user_RDS (11150)        0 2023-05-24 14:50:33.037826 ign-pdal-tools-0.5.3/
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2716 2023-05-24 14:50:33.037826 ign-pdal-tools-0.5.3/PKG-INFO
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2497 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/README.md
-drwxr-xr-x   0 GLiegard (16037) user_RDS (11150)        0 2023-05-24 14:50:33.033826 ign-pdal-tools-0.5.3/ign_pdal_tools.egg-info/
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2716 2023-05-24 14:50:33.000000 ign-pdal-tools-0.5.3/ign_pdal_tools.egg-info/PKG-INFO
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)      566 2023-05-24 14:50:33.000000 ign-pdal-tools-0.5.3/ign_pdal_tools.egg-info/SOURCES.txt
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)        1 2023-05-24 14:50:33.000000 ign-pdal-tools-0.5.3/ign_pdal_tools.egg-info/dependency_links.txt
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)       10 2023-05-24 14:50:33.000000 ign-pdal-tools-0.5.3/ign_pdal_tools.egg-info/top_level.txt
-drwxr-xr-x   0 GLiegard (16037) user_RDS (11150)        0 2023-05-24 14:50:33.033826 ign-pdal-tools-0.5.3/pdaltools/
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)       74 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pdaltools/_version.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     8269 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pdaltools/color.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     5438 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pdaltools/las_add_buffer.py
--rwxr-xr-x   0 GLiegard (16037) user_RDS (11150)     1193 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pdaltools/las_clip.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     4880 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pdaltools/las_info.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     4183 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pdaltools/las_merge.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     4742 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pdaltools/replace_attribute_in_las.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2385 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pdaltools/standardize_format.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)      353 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/pyproject.toml
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)       38 2023-05-24 14:50:33.037826 ign-pdal-tools-0.5.3/setup.cfg
-drwxr-xr-x   0 GLiegard (16037) user_RDS (11150)        0 2023-05-24 14:50:33.037826 ign-pdal-tools-0.5.3/test/
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     3306 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/test/test_color.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2345 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/test/test_las_add_buffer.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     1873 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/test/test_las_clip.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2628 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/test/test_las_info.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     1853 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/test/test_las_merge.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2791 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/test/test_replace_attribute_in_las.py
--rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2595 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.3/test/test_standardize_format.py
+drwxr-xr-x   0 GLiegard (16037) user_RDS (11150)        0 2023-05-31 15:11:39.209094 ign-pdal-tools-0.5.6/
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2716 2023-05-31 15:11:39.209094 ign-pdal-tools-0.5.6/PKG-INFO
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2497 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/README.md
+drwxr-xr-x   0 GLiegard (16037) user_RDS (11150)        0 2023-05-31 15:11:39.205094 ign-pdal-tools-0.5.6/ign_pdal_tools.egg-info/
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2716 2023-05-31 15:11:39.000000 ign-pdal-tools-0.5.6/ign_pdal_tools.egg-info/PKG-INFO
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)      566 2023-05-31 15:11:39.000000 ign-pdal-tools-0.5.6/ign_pdal_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)        1 2023-05-31 15:11:39.000000 ign-pdal-tools-0.5.6/ign_pdal_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)       10 2023-05-31 15:11:39.000000 ign-pdal-tools-0.5.6/ign_pdal_tools.egg-info/top_level.txt
+drwxr-xr-x   0 GLiegard (16037) user_RDS (11150)        0 2023-05-31 15:11:39.205094 ign-pdal-tools-0.5.6/pdaltools/
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)       74 2023-05-31 15:11:06.000000 ign-pdal-tools-0.5.6/pdaltools/_version.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     8269 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/pdaltools/color.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     5438 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/pdaltools/las_add_buffer.py
+-rwxr-xr-x   0 GLiegard (16037) user_RDS (11150)     1193 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/pdaltools/las_clip.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     4880 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/pdaltools/las_info.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     4183 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/pdaltools/las_merge.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     5270 2023-05-31 09:01:28.000000 ign-pdal-tools-0.5.6/pdaltools/replace_attribute_in_las.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     3050 2023-05-31 13:00:07.000000 ign-pdal-tools-0.5.6/pdaltools/standardize_format.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)      353 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/pyproject.toml
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)       38 2023-05-31 15:11:39.209094 ign-pdal-tools-0.5.6/setup.cfg
+drwxr-xr-x   0 GLiegard (16037) user_RDS (11150)        0 2023-05-31 15:11:39.209094 ign-pdal-tools-0.5.6/test/
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     3306 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/test/test_color.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2345 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/test/test_las_add_buffer.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     1873 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/test/test_las_clip.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     2628 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/test/test_las_info.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     1853 2023-05-24 14:49:59.000000 ign-pdal-tools-0.5.6/test/test_las_merge.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     3133 2023-05-31 09:01:28.000000 ign-pdal-tools-0.5.6/test/test_replace_attribute_in_las.py
+-rw-r--r--   0 GLiegard (16037) user_RDS (11150)     3867 2023-05-31 09:01:28.000000 ign-pdal-tools-0.5.6/test/test_standardize_format.py
```

### Comparing `ign-pdal-tools-0.5.3/PKG-INFO` & `ign-pdal-tools-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-pdal-tools
-Version: 0.5.3
+Version: 0.5.6
 Summary: Library for common LAS files manipulation with PDAL
 Author-email: Guillaume Liegard <guillaume.liegard@ign.fr>
 Description-Content-Type: text/markdown
 
 # Pdal tools
 
 Bibliothèque python qui réalise des opérations simples en utilisant pdal:
```

### Comparing `ign-pdal-tools-0.5.3/README.md` & `ign-pdal-tools-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/ign_pdal_tools.egg-info/PKG-INFO` & `ign-pdal-tools-0.5.6/ign_pdal_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-pdal-tools
-Version: 0.5.3
+Version: 0.5.6
 Summary: Library for common LAS files manipulation with PDAL
 Author-email: Guillaume Liegard <guillaume.liegard@ign.fr>
 Description-Content-Type: text/markdown
 
 # Pdal tools
 
 Bibliothèque python qui réalise des opérations simples en utilisant pdal:
```

### Comparing `ign-pdal-tools-0.5.3/ign_pdal_tools.egg-info/SOURCES.txt` & `ign-pdal-tools-0.5.6/ign_pdal_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/pdaltools/color.py` & `ign-pdal-tools-0.5.6/pdaltools/color.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/pdaltools/las_add_buffer.py` & `ign-pdal-tools-0.5.6/pdaltools/las_add_buffer.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/pdaltools/las_clip.py` & `ign-pdal-tools-0.5.6/pdaltools/las_clip.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/pdaltools/las_info.py` & `ign-pdal-tools-0.5.6/pdaltools/las_info.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/pdaltools/las_merge.py` & `ign-pdal-tools-0.5.6/pdaltools/las_merge.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/pdaltools/replace_attribute_in_las.py` & `ign-pdal-tools-0.5.6/pdaltools/replace_attribute_in_las.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import argparse
 from collections import Counter
 import json
 import logging
 import os
 import pdal
-from pdaltools.standardize_format import get_writer_parameters
+from pdaltools.standardize_format import get_writer_parameters, exec_las2las
+import tempfile
 from typing import List, Dict
 
 
 
 def parse_args():
     parser = argparse.ArgumentParser("Replace values of a given attribute in a las/laz file.")
     parser.add_argument("--input_file",
@@ -107,20 +108,33 @@
             print("Invalid json string or file path, please check args.replacement_map input:")
             print(replacement_map)
             raise e
 
     return parsed_map
 
 
+def replace_values_clean(input_file: str,
+                   output_file: str,
+                   replacement_map: Dict,
+                   attribute: str="Classification",
+                   writer_parameters: Dict={}):
+
+    _, extension = os.path.splitext(output_file)
+    with tempfile.NamedTemporaryFile(suffix=extension) as tmp:
+        tmp.close()
+        replace_values(input_file, tmp.name, replacement_map, attribute, writer_parameters)
+        exec_las2las(tmp.name, output_file)
+
+
 def main():
     args = parse_args()
     writer_params_from_parser = dict(dataformat_id=args.record_format, a_srs=args.projection)
     writer_parameters = get_writer_parameters(writer_params_from_parser)
     replacement_map = parse_replacement_map_from_path_or_json_string(args.replacement_map)
 
-    replace_values(args.input_file, args.output_file,
+    replace_values_clean(args.input_file, args.output_file,
                    replacement_map, args.attribute, writer_parameters)
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     main()
```

### Comparing `ign-pdal-tools-0.5.3/pdaltools/standardize_format.py` & `ign-pdal-tools-0.5.6/pdaltools/standardize_format.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,32 @@
     - record format
     - global encoding
     - projection
     - precision
     - no extra-dims
 """
 import argparse
+import os
 import pdal
+import subprocess as sp
+import tempfile
 from typing import Dict
 
-
 STANDARD_PARAMETERS = dict(
     major_version="1",
     minor_version="4",  # Laz format version (pdal always write in 1.x format)
     global_encoding=17,  # store WKT projection in file
     compression="true",  # Save to compressed laz format
     extra_dims= [],  # Save no extra_dims
     scale_x=0.01, # Precision of the stored data
     scale_y=0.01,
     scale_z=0.01,
-    offset_x='auto',  # To be confirmed
-    offset_y='auto',  # To be confirmed
-    offset_z='auto',  # To be confirmed
+    offset_x=0, # No offset
+    offset_y=0,
+    offset_z=0,
     dataformat_id=6,  # No color by default
     a_srs="EPSG:2154"
 )
 
 
 def parse_args():
     parser = argparse.ArgumentParser("Rewrite laz file with standard format.")
@@ -63,14 +65,34 @@
     # Update parameters with command line values
     params = get_writer_parameters(params_from_parser)
     pipeline = pdal.Reader.las(input_file)
     pipeline |= pdal.Writer(filename=output_file, **params)
     pipeline.execute()
 
 
+def exec_las2las(input_file: str, output_file: str):
+    r = sp.run(["las2las", "-i", input_file, "-o", output_file], stderr=sp.PIPE, stdout=sp.PIPE)
+    if r.returncode == 1:
+        msg = r.stderr.decode()
+        print(msg)
+        raise RuntimeError(msg)
+
+    output = r.stdout.decode()
+    for line in output.splitlines():
+        print(line)
+
+
+def standardize(input_file: str, output_file: str, params_from_parser: Dict) -> None:
+    _, extension = os.path.splitext(output_file)
+    with tempfile.NamedTemporaryFile(suffix=extension) as tmp:
+        tmp.close()
+        rewrite_with_pdal(input_file, tmp.name, params_from_parser)
+        exec_las2las(tmp.name, output_file)
+
+
 if __name__ == "__main__":
     args = parse_args()
     params_from_parser = dict(
         dataformat_id=args.record_format,
         a_srs=args.projection)
-    rewrite_with_pdal(args.input_file, args.output_file, params_from_parser)
+    standardize(args.input_file, args.output_file, params_from_parser)
```

### Comparing `ign-pdal-tools-0.5.3/test/test_color.py` & `ign-pdal-tools-0.5.6/test/test_color.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/test/test_las_add_buffer.py` & `ign-pdal-tools-0.5.6/test/test_las_add_buffer.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/test/test_las_clip.py` & `ign-pdal-tools-0.5.6/test/test_las_clip.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/test/test_las_info.py` & `ign-pdal-tools-0.5.6/test/test_las_info.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/test/test_las_merge.py` & `ign-pdal-tools-0.5.6/test/test_las_merge.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.3/test/test_replace_attribute_in_las.py` & `ign-pdal-tools-0.5.6/test/test_replace_attribute_in_las.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from collections import Counter
 import json
 import os
-from pdaltools.replace_attribute_in_las import replace_values, parse_replacement_map_from_path_or_json_string
+from pdaltools.replace_attribute_in_las import replace_values, replace_values_clean, parse_replacement_map_from_path_or_json_string
 from pdaltools.count_occurences.count_occurences_for_attribute import compute_count_one_file
+from pdaltools.standardize_format import get_writer_parameters
 import pytest
 import shutil
 from test.utils import get_pdal_infos_summary
 from typing import Dict
-
+from test.test_standardize_format import assert_lasinfo_no_warning
 
 test_path = os.path.dirname(os.path.abspath(__file__))
 tmp_path = os.path.join(test_path, "tmp")
 input_dir = os.path.join(test_path, "data/classified_laz")
 input_file = os.path.join(input_dir, "test_data_77050_627755_LA93_IGN69.laz")
 output_file = os.path.join(tmp_path, "replaced.las")
 attribute = "Classification"
@@ -63,14 +64,19 @@
     replace_values(input_file, output_file, replacement_map_success, attribute)
     count = compute_count_one_file(output_file, attribute)
 
     assert count == expected_counts
     check_dimensions(input_file, output_file)
 
 
+def test_replace_values_clean():
+    replace_values_clean(input_file, output_file, replacement_map_success, attribute, get_writer_parameters({}))
+    assert_lasinfo_no_warning(output_file)
+
+
 def test_replace_values_duplicate_input():
     with pytest.raises(ValueError):
         replace_values(input_file, output_file, replacement_map_fail, attribute)
 
 
 def check_dimensions(input_file, output_file):
     input_summary = get_pdal_infos_summary(input_file)
```

### Comparing `ign-pdal-tools-0.5.3/test/test_standardize_format.py` & `ign-pdal-tools-0.5.6/test/test_standardize_format.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pytest
 import shutil
-from pdaltools.standardize_format import rewrite_with_pdal
+from pdaltools.standardize_format import rewrite_with_pdal, standardize, exec_las2las
 import logging
 from test.utils import get_pdal_infos_summary
 import pdal
-
+import subprocess as sp
 
 # Note: tile 77050_627760 is cropped to simulate missing data in neighbors during merge
 test_path = os.path.dirname(os.path.abspath(__file__))
 tmp_path = os.path.join(test_path, "tmp")
 input_dir = os.path.join(test_path, "data")
 
 coord_x = 77055
@@ -67,10 +67,49 @@
 
 
 def test_standardize_format():
     for params in multiple_params:
         _test_standardize_format_one_params_set(params)
 
 
+def exec_lasinfo(input_file: str):
+    r = sp.run(["lasinfo", "-stdout", input_file], stderr=sp.PIPE, stdout=sp.PIPE)
+    if r.returncode == 1:
+        msg = r.stderr.decode()
+        print(msg)
+        raise RuntimeError(msg)
+
+    output = r.stdout.decode()
+    return output
+
+
+def assert_lasinfo_no_warning(input_file: str):
+    errors = [ line for line in exec_lasinfo(input_file).splitlines() if 'WARNING' in line]
+
+    for line in errors:
+        print(line)
+
+    assert errors == [], errors
+
+
+def test_exec_las2las_error():
+    with pytest.raises(RuntimeError):
+        exec_las2las("not_existing_input_file", "output_file")
+
+
+def test_standardize_does_NOT_produce_any_warning_with_Lasinfo():
+    # bad file on the store (44 Mo)
+    # input_file = "/var/data/store-lidarhd/developpement/standaLAS/demo_standardization/Semis_2022_0584_6880_LA93_IGN69.laz"
+
+    input_file = "./test/data/classified_laz/test_data_77050_627755_LA93_IGN69.laz"
+    output_file = "./tmp/test_standardize_produce_no_warning_with_lasinfo.las"
+
+    # if you want to see input_file warnings
+    # assert_lasinfo_no_warning(input_file)
+
+    standardize(input_file, output_file, multiple_params[0])
+    assert_lasinfo_no_warning(output_file)
+
+
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
     test_standardize_format()
```

