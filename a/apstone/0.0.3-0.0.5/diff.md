# Comparing `tmp/apstone-0.0.3.tar.gz` & `tmp/apstone-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apstone-0.0.3.tar", last modified: Mon Nov 14 08:28:00 2022, max compression
+gzip compressed data, was "apstone-0.0.5.tar", last modified: Wed May 31 08:24:43 2023, max compression
```

## Comparing `apstone-0.0.3.tar` & `apstone-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2051 2022-11-14 08:28:00.670556 apstone-0.0.3/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1557 2022-11-11 09:51:48.000000 apstone-0.0.3/README.md
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2022-11-14 03:45:05.000000 apstone-0.0.3/apstone/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1833 2022-11-14 08:26:24.000000 apstone-0.0.3/apstone/model_base.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone/model_convert/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      154 2022-11-11 10:19:16.000000 apstone-0.0.3/apstone/model_convert/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     9481 2022-11-11 08:06:23.000000 apstone-0.0.3/apstone/model_convert/detectron2_model_export.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      578 2022-11-11 08:34:17.000000 apstone-0.0.3/apstone/model_convert/modelscope_ali_2_onnx.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3016 2021-10-12 09:30:00.000000 apstone-0.0.3/apstone/model_convert/onnx2simple2trt.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2620 2021-10-12 09:30:48.000000 apstone-0.0.3/apstone/model_convert/onnx2trt.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      824 2022-11-11 08:34:17.000000 apstone-0.0.3/apstone/model_convert/tf2pb2onnx.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      712 2022-11-11 10:20:15.000000 apstone-0.0.3/apstone/model_convert/torch2any.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone/model_edit/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      108 2022-11-11 08:34:17.000000 apstone-0.0.3/apstone/model_edit/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      450 2022-11-11 08:34:17.000000 apstone-0.0.3/apstone/model_edit/torch_model_edit.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone/wrappers/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      109 2022-11-14 08:24:11.000000 apstone-0.0.3/apstone/wrappers/__init__.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone/wrappers/mmlab_wrapper/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      205 2022-11-11 08:34:17.000000 apstone-0.0.3/apstone/wrappers/mmlab_wrapper/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2413 2022-11-14 06:16:11.000000 apstone-0.0.3/apstone/wrappers/mmlab_wrapper/bbox_detector_mmdet.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6984 2022-11-14 06:30:44.000000 apstone-0.0.3/apstone/wrappers/mmlab_wrapper/kp_detector_mmpose.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5386 2022-11-11 10:10:08.000000 apstone-0.0.3/apstone/wrappers/mmlab_wrapper/utils.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone/wrappers/onnx_wrapper/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       86 2022-11-14 03:43:14.000000 apstone-0.0.3/apstone/wrappers/onnx_wrapper/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5834 2022-11-11 08:34:17.000000 apstone-0.0.3/apstone/wrappers/onnx_wrapper/onnx_model.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3990 2022-11-14 06:05:04.000000 apstone-0.0.3/apstone/wrappers/onnx_wrapper/onnx_model_picklable.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone/wrappers/tjm_wrapper/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      143 2022-11-14 05:56:11.000000 apstone-0.0.3/apstone/wrappers/tjm_wrapper/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      830 2022-11-11 08:34:17.000000 apstone-0.0.3/apstone/wrappers/tjm_wrapper/tjm_model.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone/wrappers/trt_wrapper/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      199 2022-11-14 06:22:41.000000 apstone-0.0.3/apstone/wrappers/trt_wrapper/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5089 2022-11-14 03:38:26.000000 apstone-0.0.3/apstone/wrappers/trt_wrapper/trt_wrapper_mmdeploy.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3729 2022-11-11 08:34:17.000000 apstone-0.0.3/apstone/wrappers/trt_wrapper/trt_wrapper_self.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2022-11-14 08:28:00.670556 apstone-0.0.3/apstone.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2051 2022-11-14 08:28:00.000000 apstone-0.0.3/apstone.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1145 2022-11-14 08:28:00.000000 apstone-0.0.3/apstone.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2022-11-14 08:28:00.000000 apstone-0.0.3/apstone.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       54 2022-11-14 08:28:00.000000 apstone-0.0.3/apstone.egg-info/requires.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2022-11-14 08:28:00.000000 apstone-0.0.3/apstone.egg-info/top_level.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2022-11-14 08:28:00.670556 apstone-0.0.3/setup.cfg
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1040 2022-11-14 08:27:56.000000 apstone-0.0.3/setup.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.115399 apstone-0.0.5/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2051 2023-05-31 08:24:43.115399 apstone-0.0.5/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1557 2022-11-11 09:51:48.000000 apstone-0.0.5/README.md
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.107399 apstone-0.0.5/apstone/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2022-11-14 03:45:05.000000 apstone-0.0.5/apstone/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1976 2023-05-24 08:54:03.000000 apstone-0.0.5/apstone/model_base.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.111399 apstone-0.0.5/apstone/model_convert/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      154 2022-11-11 10:19:16.000000 apstone-0.0.5/apstone/model_convert/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     9481 2022-11-11 08:06:23.000000 apstone-0.0.5/apstone/model_convert/detectron2_model_export.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      578 2022-11-11 08:34:17.000000 apstone-0.0.5/apstone/model_convert/modelscope_ali_2_onnx.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3016 2021-10-12 09:30:00.000000 apstone-0.0.5/apstone/model_convert/onnx2simple2trt.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2620 2021-10-12 09:30:48.000000 apstone-0.0.5/apstone/model_convert/onnx2trt.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      824 2022-11-22 01:24:31.000000 apstone-0.0.5/apstone/model_convert/tf2pb2onnx.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      712 2022-11-11 10:20:15.000000 apstone-0.0.5/apstone/model_convert/torch2any.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.111399 apstone-0.0.5/apstone/model_edit/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      108 2022-11-11 08:34:17.000000 apstone-0.0.5/apstone/model_edit/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      450 2022-11-11 08:34:17.000000 apstone-0.0.5/apstone/model_edit/torch_model_edit.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.111399 apstone-0.0.5/apstone/onnx_tools/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      671 2022-11-11 08:34:17.000000 apstone-0.0.5/apstone/onnx_tools/convert_onnx_input_shape.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1151 2023-02-21 07:06:09.000000 apstone-0.0.5/apstone/onnx_tools/onnx_merge.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      992 2022-11-11 08:34:17.000000 apstone-0.0.5/apstone/onnx_tools/remove_initializer_from_input.py
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)   107494 2022-11-11 08:06:23.000000 apstone-0.0.5/apstone/onnx_tools/symbolic_shape_infer.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.111399 apstone-0.0.5/apstone/wrappers/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      109 2022-11-14 08:24:11.000000 apstone-0.0.5/apstone/wrappers/__init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.111399 apstone-0.0.5/apstone/wrappers/llm_wrapper/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      758 2023-05-06 02:26:28.000000 apstone-0.0.5/apstone/wrappers/llm_wrapper/llm_model.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.111399 apstone-0.0.5/apstone/wrappers/mmlab_wrapper/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      205 2022-11-11 08:34:17.000000 apstone-0.0.5/apstone/wrappers/mmlab_wrapper/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2413 2022-11-14 06:16:11.000000 apstone-0.0.5/apstone/wrappers/mmlab_wrapper/bbox_detector_mmdet.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6984 2022-11-14 06:30:44.000000 apstone-0.0.5/apstone/wrappers/mmlab_wrapper/kp_detector_mmpose.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5386 2022-11-11 10:10:08.000000 apstone-0.0.5/apstone/wrappers/mmlab_wrapper/utils.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.111399 apstone-0.0.5/apstone/wrappers/onnx_wrapper/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       86 2022-11-14 03:43:14.000000 apstone-0.0.5/apstone/wrappers/onnx_wrapper/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7603 2023-05-24 08:53:25.000000 apstone-0.0.5/apstone/wrappers/onnx_wrapper/onnx_model.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3990 2022-11-14 06:05:04.000000 apstone-0.0.5/apstone/wrappers/onnx_wrapper/onnx_model_picklable.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.111399 apstone-0.0.5/apstone/wrappers/tjm_wrapper/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      143 2022-11-14 05:56:11.000000 apstone-0.0.5/apstone/wrappers/tjm_wrapper/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      830 2022-11-11 08:34:17.000000 apstone-0.0.5/apstone/wrappers/tjm_wrapper/tjm_model.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.115399 apstone-0.0.5/apstone/wrappers/trt_wrapper/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      199 2022-11-14 06:22:41.000000 apstone-0.0.5/apstone/wrappers/trt_wrapper/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5089 2022-11-14 03:38:26.000000 apstone-0.0.5/apstone/wrappers/trt_wrapper/trt_wrapper_mmdeploy.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3729 2022-11-11 08:34:17.000000 apstone-0.0.5/apstone/wrappers/trt_wrapper/trt_wrapper_self.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 08:24:43.107399 apstone-0.0.5/apstone.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2051 2023-05-31 08:24:43.000000 apstone-0.0.5/apstone.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1387 2023-05-31 08:24:43.000000 apstone-0.0.5/apstone.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-31 08:24:43.000000 apstone-0.0.5/apstone.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       54 2023-05-31 08:24:43.000000 apstone-0.0.5/apstone.egg-info/requires.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-05-31 08:24:43.000000 apstone-0.0.5/apstone.egg-info/top_level.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      933 2023-05-19 09:49:55.000000 apstone-0.0.5/onnx_model_speed_test.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2023-05-31 08:24:43.115399 apstone-0.0.5/setup.cfg
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1040 2023-05-31 08:24:09.000000 apstone-0.0.5/setup.py
```

### Comparing `apstone-0.0.3/PKG-INFO` & `apstone-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apstone
-Version: 0.0.3
+Version: 0.0.5
 Summary: ai_power base stone
 Home-page: https://github.com/ykk648/apstone
 Author: ykk648
 Author-email: ykk648@gmail.com
 Project-URL: Bug Tracker, https://github.com/ykk648/apstone/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `apstone-0.0.3/README.md` & `apstone-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/model_base.py` & `apstone-0.0.5/apstone/model_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,17 @@
 
         if 'input_dynamic_shape' in model_info.keys():
             self.input_dynamic_shape = model_info['input_dynamic_shape']
         else:
             self.input_dynamic_shape = None
 
         if 'picklable' in model_info.keys():
-            ONNXModelWrapper = OnnxModelPickable
+            picklable = model_info['picklable']
         else:
-            ONNXModelWrapper = ONNXModel
-
-        if 'encrypt' in model_info.keys():
-            from .utils.data_encrypt import load_encrypt_model
-            self.model_path = load_encrypt_model(self.model_path, key=model_info['encrypt'])
+            picklable = False
 
         # init model
         if Path(self.model_path).suffix == '.engine':
             if 'trt_wrapper_self' in model_info.keys():
                 from .wrappers.trt_wrapper import TRTWrapperSelf
                 TRTWrapper = TRTWrapperSelf
             else:
@@ -36,11 +32,18 @@
             self.model = TRTWrapper(self.model_path)
         elif Path(self.model_path).suffix == '.tjm':
             from .wrappers.tjm_wrapper import TJMWrapper
             self.model_type = 'tjm'
             self.model = TJMWrapper(self.model_path, provider=provider)
         elif Path(self.model_path).suffix in ['.onnx', '.bin']:
             self.model_type = 'onnx'
-            self.model = ONNXModelWrapper(self.model_path, provider=provider,
-                                          input_dynamic_shape=self.input_dynamic_shape)
+            if not picklable:
+                if 'encrypt' in model_info.keys():
+                    from cv2box.utils.encrypt import CVEncrypt
+                    self.model_path = CVEncrypt(model_info['encrypt']).load_encrypt_file(self.model_path)
+                self.model = ONNXModel(self.model_path, provider=provider,
+                                              input_dynamic_shape=self.input_dynamic_shape)
+            else:
+                self.model = OnnxModelPickable(self.model_path, provider=provider, )
+
         else:
             raise 'check model suffix , support engine/tjm/onnx/bin now.'
```

### Comparing `apstone-0.0.3/apstone/model_convert/detectron2_model_export.py` & `apstone-0.0.5/apstone/model_convert/detectron2_model_export.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/model_convert/modelscope_ali_2_onnx.py` & `apstone-0.0.5/apstone/model_convert/modelscope_ali_2_onnx.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/model_convert/onnx2simple2trt.py` & `apstone-0.0.5/apstone/model_convert/onnx2simple2trt.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/model_convert/onnx2trt.py` & `apstone-0.0.5/apstone/model_convert/onnx2trt.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/model_convert/tf2pb2onnx.py` & `apstone-0.0.5/apstone/model_convert/tf2pb2onnx.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/model_convert/torch2any.py` & `apstone-0.0.5/apstone/model_convert/torch2any.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/wrappers/mmlab_wrapper/bbox_detector_mmdet.py` & `apstone-0.0.5/apstone/wrappers/mmlab_wrapper/bbox_detector_mmdet.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/wrappers/mmlab_wrapper/kp_detector_mmpose.py` & `apstone-0.0.5/apstone/wrappers/mmlab_wrapper/kp_detector_mmpose.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/wrappers/mmlab_wrapper/utils.py` & `apstone-0.0.5/apstone/wrappers/mmlab_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/wrappers/onnx_wrapper/onnx_model.py` & `apstone-0.0.5/apstone/wrappers/onnx_wrapper/onnx_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -- coding: utf-8 --
 # @Time : 2021/11/29
 # @Author : ykk648
 # @Project : https://github.com/ykk648/apstone
 
-"""
-todo: io_binding https://onnxruntime.ai/docs/api/python/api_summary.html
-"""
 
 import onnxruntime
 import numpy as np
 from cv2box import MyFpsCounter
 import os
+from pathlib import Path
+import re
 
 
 def get_output_info(onnx_session):
     output_name = []
     output_shape = []
     for node in onnx_session.get_outputs():
         output_name.append(node.name)
@@ -43,46 +42,62 @@
         input_feed[name] = image_tensor[index]
     return input_feed
 
 
 class ONNXModel:
     def __init__(self, onnx_path, provider='gpu', debug=False, input_dynamic_shape=None):
         self.provider = provider
+        try:
+            onnx_name = Path(onnx_path).stem
+            trt_cache_path = './cache/trt/' + onnx_name
+        except TypeError:
+            pass
 
         if self.provider == 'gpu':
             self.providers = (
                 "CUDAExecutionProvider",
                 {'device_id': 0, }
             )
         elif self.provider == 'trt':
-            os.makedirs('./cache/trt', exist_ok=True)
+            os.makedirs(trt_cache_path, exist_ok=True)
             self.providers = (
                 'TensorrtExecutionProvider',
-                {'trt_engine_cache_enable': True, 'trt_engine_cache_path': './cache/trt', 'trt_fp16_enable': False, }
+                {'trt_engine_cache_enable': True, 'trt_engine_cache_path': trt_cache_path, 'trt_fp16_enable': False, }
             )
         elif self.provider == 'trt16':
-            os.makedirs('./cache/trt', exist_ok=True)
+            os.makedirs(trt_cache_path, exist_ok=True)
             self.providers = (
                 'TensorrtExecutionProvider',
-                {'trt_engine_cache_enable': True, 'trt_engine_cache_path': './cache/trt', 'trt_fp16_enable': True,
+                {'trt_engine_cache_enable': True, 'trt_engine_cache_path': trt_cache_path, 'trt_fp16_enable': True,
                  'trt_dla_enable': False, }
             )
         elif self.provider == 'trt8':
-            os.makedirs('./cache/trt', exist_ok=True)
+            os.makedirs(trt_cache_path, exist_ok=True)
             self.providers = (
                 'TensorrtExecutionProvider',
                 {'trt_engine_cache_enable': True, 'trt_int8_enable': True, }
             )
         else:
             self.providers = "CPUExecutionProvider"
 
         # onnxruntime.set_default_logger_severity(3)
         session_options = onnxruntime.SessionOptions()
         session_options.log_severity_level = 3
-        self.onnx_session = onnxruntime.InferenceSession(onnx_path, session_options, providers=[self.providers])
+
+        # When env change leads to trt cache load fail, auto generate new cache
+        try:
+            self.onnx_session = onnxruntime.InferenceSession(onnx_path, session_options, providers=[self.providers])
+        except Exception as e:
+            if type(e.args[0])==str and 'TensorRT EP could not deserialize engine from cache' in e.args[0]:
+                res = re.match('.*TensorRT EP could not deserialize engine from cache: (.*)', e.args[0])
+                os.remove(res.group(1))
+                print('waiting generate new model...')
+                self.onnx_session = onnxruntime.InferenceSession(onnx_path, session_options, providers=[self.providers])
+            else:
+                raise e
 
         # sessionOptions.intra_op_num_threads = 3
         self.input_name, self.input_shape = get_input_info(self.onnx_session)
         self.output_name, self.output_shape = get_output_info(self.onnx_session)
 
         self.input_dynamic_shape = input_dynamic_shape
 
@@ -144,7 +159,34 @@
         return self.onnx_session.run(self.output_name, input_feed=input_feed)
 
     def batch_forward(self, bach_image_tensor, trans=False):
         if trans:
             bach_image_tensor = bach_image_tensor.transpose(0, 3, 1, 2)
         input_feed = get_input_feed(self.input_name, bach_image_tensor)
         return self.onnx_session.run(self.output_name, input_feed=input_feed)
+
+    def binding_forward(self, binding):
+        """
+        ref io_binding https://onnxruntime.ai/docs/api/python/api_summary.html
+        do io_binding outside this func and pass it in
+        example(cuda in&out):
+            import torch
+            binding = self.model.onnx_session.io_binding()
+            image_tensor_in = image_tensor_in.contiguous()
+            binding.bind_input(
+                name='X',
+                device_type='cuda',
+                device_id=0,
+                element_type=np.float32,
+                shape=tuple(image_tensor_in.shape),
+                buffer_ptr=image_tensor_in.data_ptr(),)
+
+            Y_tensor = torch.empty(Y_shape, dtype=torch.float32, device='cuda:0').contiguous()
+            binding.bind_output(
+                name='Y',
+                device_type='cuda',
+                device_id=0,
+                element_type=np.float32,
+                shape=tuple(Y_tensor.shape),
+                buffer_ptr=Y_tensor.data_ptr(),)
+        """
+        self.onnx_session.run_with_iobinding(binding)
```

### Comparing `apstone-0.0.3/apstone/wrappers/onnx_wrapper/onnx_model_picklable.py` & `apstone-0.0.5/apstone/wrappers/onnx_wrapper/onnx_model_picklable.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/wrappers/tjm_wrapper/tjm_model.py` & `apstone-0.0.5/apstone/wrappers/tjm_wrapper/tjm_model.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/wrappers/trt_wrapper/trt_wrapper_mmdeploy.py` & `apstone-0.0.5/apstone/wrappers/trt_wrapper/trt_wrapper_mmdeploy.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone/wrappers/trt_wrapper/trt_wrapper_self.py` & `apstone-0.0.5/apstone/wrappers/trt_wrapper/trt_wrapper_self.py`

 * *Files identical despite different names*

### Comparing `apstone-0.0.3/apstone.egg-info/PKG-INFO` & `apstone-0.0.5/apstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apstone
-Version: 0.0.3
+Version: 0.0.5
 Summary: ai_power base stone
 Home-page: https://github.com/ykk648/apstone
 Author: ykk648
 Author-email: ykk648@gmail.com
 Project-URL: Bug Tracker, https://github.com/ykk648/apstone/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `apstone-0.0.3/apstone.egg-info/SOURCES.txt` & `apstone-0.0.5/apstone.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+onnx_model_speed_test.py
 setup.py
 apstone/__init__.py
 apstone/model_base.py
 apstone.egg-info/PKG-INFO
 apstone.egg-info/SOURCES.txt
 apstone.egg-info/dependency_links.txt
 apstone.egg-info/requires.txt
@@ -12,15 +13,20 @@
 apstone/model_convert/modelscope_ali_2_onnx.py
 apstone/model_convert/onnx2simple2trt.py
 apstone/model_convert/onnx2trt.py
 apstone/model_convert/tf2pb2onnx.py
 apstone/model_convert/torch2any.py
 apstone/model_edit/__init__.py
 apstone/model_edit/torch_model_edit.py
+apstone/onnx_tools/convert_onnx_input_shape.py
+apstone/onnx_tools/onnx_merge.py
+apstone/onnx_tools/remove_initializer_from_input.py
+apstone/onnx_tools/symbolic_shape_infer.py
 apstone/wrappers/__init__.py
+apstone/wrappers/llm_wrapper/llm_model.py
 apstone/wrappers/mmlab_wrapper/__init__.py
 apstone/wrappers/mmlab_wrapper/bbox_detector_mmdet.py
 apstone/wrappers/mmlab_wrapper/kp_detector_mmpose.py
 apstone/wrappers/mmlab_wrapper/utils.py
 apstone/wrappers/onnx_wrapper/__init__.py
 apstone/wrappers/onnx_wrapper/onnx_model.py
 apstone/wrappers/onnx_wrapper/onnx_model_picklable.py
```

### Comparing `apstone-0.0.3/setup.py` & `apstone-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='apstone',  # 项目的名称
-    version='0.0.3',  # 项目版本
+    version='0.0.5',  # 项目版本
     author='ykk648',  # 项目作者
     author_email='ykk648@gmail.com',  # 作者email
     url='https://github.com/ykk648/apstone',  # 项目代码仓库
     project_urls={
         "Bug Tracker": "https://github.com/ykk648/apstone/issues",
     },
     description='ai_power base stone',  # 项目描述
```

