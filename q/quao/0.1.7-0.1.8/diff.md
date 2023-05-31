# Comparing `tmp/quao-0.1.7.tar.gz` & `tmp/quao-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.1.7.tar", last modified: Wed May 31 03:16:04 2023, max compression
+gzip compressed data, was "quao-0.1.8.tar", last modified: Wed May 31 04:10:54 2023, max compression
```

## Comparing `quao-0.1.7.tar` & `quao-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.313717 quao-0.1.7/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-05-31 03:16:04.312715 quao-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.7/README.md
--rw-rw-rw-   0        0        0      846 2023-05-31 03:15:37.000000 quao-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 03:16:04.314718 quao-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.205777 quao-0.1.7/src/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.229739 quao-0.1.7/src/quao/
--rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.7/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.269508 quao-0.1.7/src/quao/algorithms/
--rw-rw-rw-   0        0        0        2 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5305 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/algorithms/shor.py
--rw-rw-rw-   0        0        0     3605 2023-05-31 03:15:37.000000 quao-0.1.7/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.280752 quao-0.1.7/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.7/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      189 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/config/loggingConfig.py
--rw-rw-rw-   0        0        0      175 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/config/threadConfig.py
--rw-rw-rw-   0        0        0      529 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/dataUtils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.289212 quao-0.1.7/src/quao/enum/
--rw-rw-rw-   0        0        0      200 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/enum/providerType.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.300749 quao-0.1.7/src/quao/sdk/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.7/src/quao/sdk/__init__.py
--rw-rw-rw-   0        0        0     6402 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/sdk/qiskit.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.311956 quao-0.1.7/src/quao/status/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:57:12.000000 quao-0.1.7/src/quao/status/__init__.py
--rw-rw-rw-   0        0        0     2450 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/status/qiskit_status.py
--rw-rw-rw-   0        0        0     1636 2023-05-31 01:58:09.000000 quao-0.1.7/src/quao/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-31 03:16:04.257716 quao-0.1.7/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-05-31 03:16:04.000000 quao-0.1.7/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-31 03:16:04.000000 quao-0.1.7/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 03:16:04.000000 quao-0.1.7/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-31 03:16:04.000000 quao-0.1.7/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 03:16:04.000000 quao-0.1.7/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.651938 quao-0.1.8/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-05-31 04:10:54.650934 quao-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.8/README.md
+-rw-rw-rw-   0        0        0      846 2023-05-31 04:10:44.000000 quao-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 04:10:54.651938 quao-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.600936 quao-0.1.8/src/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.606938 quao-0.1.8/src/quao/
+-rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.8/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.636942 quao-0.1.8/src/quao/algorithms/
+-rw-rw-rw-   0        0        0        2 2023-05-31 01:58:09.000000 quao-0.1.8/src/quao/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-05-31 01:58:09.000000 quao-0.1.8/src/quao/algorithms/shor.py
+-rw-rw-rw-   0        0        0     3527 2023-05-31 04:10:04.000000 quao-0.1.8/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.641937 quao-0.1.8/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.8/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      189 2023-05-31 01:58:09.000000 quao-0.1.8/src/quao/config/loggingConfig.py
+-rw-rw-rw-   0        0        0      179 2023-05-31 04:07:43.000000 quao-0.1.8/src/quao/config/threadConfig.py
+-rw-rw-rw-   0        0        0      529 2023-05-31 01:58:09.000000 quao-0.1.8/src/quao/dataUtils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.643936 quao-0.1.8/src/quao/enum/
+-rw-rw-rw-   0        0        0      200 2023-05-31 01:58:09.000000 quao-0.1.8/src/quao/enum/providerType.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.646934 quao-0.1.8/src/quao/sdk/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.8/src/quao/sdk/__init__.py
+-rw-rw-rw-   0        0        0     6415 2023-05-31 03:35:27.000000 quao-0.1.8/src/quao/sdk/qiskit.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.649934 quao-0.1.8/src/quao/status/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:57:12.000000 quao-0.1.8/src/quao/status/__init__.py
+-rw-rw-rw-   0        0        0     2450 2023-05-31 01:58:09.000000 quao-0.1.8/src/quao/status/qiskit_status.py
+-rw-rw-rw-   0        0        0     1636 2023-05-31 01:58:09.000000 quao-0.1.8/src/quao/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:10:54.632971 quao-0.1.8/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-05-31 04:10:54.000000 quao-0.1.8/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-31 04:10:54.000000 quao-0.1.8/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 04:10:54.000000 quao-0.1.8/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-31 04:10:54.000000 quao-0.1.8/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 04:10:54.000000 quao-0.1.8/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.1.7/LICENSE` & `quao-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.1.7/PKG-INFO` & `quao-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.7
+Version: 0.1.8
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.1.7/README.md` & `quao-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.1.7/pyproject.toml` & `quao-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.1.7"
+version = "0.1.8"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.1.7/src/quao/algorithms/shor.py` & `quao-0.1.8/src/quao/algorithms/shor.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.7/src/quao/backend.py` & `quao-0.1.8/src/quao/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
     QuaO Project backend.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 from .dataUtils import RequestData
 from .utilities import JobResponse
 from .config.threadConfig import pool
+from .config.loggingConfig import logging
 from json import JSONDecodeError
 
 import requests
 import io
 
 
 class Backend:
@@ -17,15 +18,15 @@
         self.sdk = request_data.sdk
         self.input = request_data.input
         self.shots = request_data.shots
         self.required_qubit = self.get_qubit_number(circuit)
         self.backend_request = self.generate_backend_request(request_data.device_id)
         self.backend_data = self.get_backend_data()
         self.circuit_export_url = request_data.circuit_export_url
-        pool.apply_async(self.__export_circuit, (circuit,))
+        pool.submit(self.__export_circuit, circuit)
 
     def get_qubit_number(self, circuit) -> int:
 
         if self.sdk == "qiskit":
             return int(circuit.num_qubits)
         return 0
 
@@ -78,18 +79,14 @@
 
     def __export_circuit(self, circuit):
         """
             Export circuit to svg file then send to QuaO server for saving
             Args:
                 circuit: circuit will be exported
         """
-        import logging
-
-        logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
-
         logging.info("Preparing circuit figure...")
         circuit_figure = circuit.draw(output='mpl', fold=-1)
 
         logging.info("Converting circuit figure to svg file...")
         figure_buffer = io.BytesIO()
         circuit_figure.savefig(figure_buffer, format='svg')
```

### Comparing `quao-0.1.7/src/quao/dataUtils.py` & `quao-0.1.8/src/quao/dataUtils.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.7/src/quao/sdk/qiskit.py` & `quao-0.1.8/src/quao/sdk/qiskit.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 job_status = job.status().name
                 job_result = result.to_dict()
                 content_type = APPLICATION_JSON
                 job_histogram = self.__get_histogram(result=result)
 
             # handle job result has Statevector Object
             if self.device_name == 'statevector_simulator':
-                job_result = json.dumps(job_result)
+                job_result = json.dumps(job_result, default=str)
 
         except Exception as exception:
             job_result = {
                 "error": "Exception when invoke job on IBM Quantum provider",
                 "exception": str(exception)
             }
             job_status = "ERROR"
```

### Comparing `quao-0.1.7/src/quao/status/qiskit_status.py` & `quao-0.1.8/src/quao/status/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.7/src/quao/utilities.py` & `quao-0.1.8/src/quao/utilities.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.7/src/quao.egg-info/PKG-INFO` & `quao-0.1.8/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.7
+Version: 0.1.8
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.1.7/src/quao.egg-info/SOURCES.txt` & `quao-0.1.8/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

