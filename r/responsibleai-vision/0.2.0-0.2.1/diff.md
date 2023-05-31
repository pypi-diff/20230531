# Comparing `tmp/responsibleai_vision-0.2.0.tar.gz` & `tmp/responsibleai_vision-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_vision-0.2.0.tar", last modified: Fri May  5 17:33:40 2023, max compression
+gzip compressed data, was "responsibleai_vision-0.2.1.tar", last modified: Wed May 31 18:48:38 2023, max compression
```

## Comparing `responsibleai_vision-0.2.0.tar` & `responsibleai_vision-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.199850 responsibleai_vision-0.2.0/
--rw-rw-rw-   0        0        0     1403 2023-05-05 17:33:40.199850 responsibleai_vision-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      691 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 17:33:39.862868 responsibleai_vision-0.2.0/responsibleai_vision/
--rw-rw-rw-   0        0        0      367 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:33:39.966630 responsibleai_vision-0.2.0/responsibleai_vision/common/
--rw-rw-rw-   0        0        0      127 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/common/__init__.py
--rw-rw-rw-   0        0        0     2518 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.0/responsibleai_vision/common/constants.py
--rw-rw-rw-   0        0        0      223 2022-09-01 02:31:14.000000 responsibleai_vision-0.2.0/responsibleai_vision/common/interfaces.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.016699 responsibleai_vision-0.2.0/responsibleai_vision/managers/
--rw-rw-rw-   0        0        0      109 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/managers/__init__.py
--rw-rw-rw-   0        0        0    13897 2023-05-05 17:29:08.000000 responsibleai_vision-0.2.0/responsibleai_vision/managers/error_analysis_manager.py
--rw-rw-rw-   0        0        0    26315 2023-05-04 17:50:06.000000 responsibleai_vision-0.2.0/responsibleai_vision/managers/explainer_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.055076 responsibleai_vision-0.2.0/responsibleai_vision/rai_vision_insights/
--rw-rw-rw-   0        0        0      253 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/rai_vision_insights/__init__.py
--rw-rw-rw-   0        0        0    46976 2023-05-05 17:29:08.000000 responsibleai_vision-0.2.0/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.131971 responsibleai_vision-0.2.0/responsibleai_vision/utils/
--rw-rw-rw-   0        0        0      129 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/utils/__init__.py
--rw-rw-rw-   0        0        0     2329 2023-05-05 17:29:08.000000 responsibleai_vision-0.2.0/responsibleai_vision/utils/feature_extractors.py
--rw-rw-rw-   0        0        0     2824 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.0/responsibleai_vision/utils/image_reader.py
--rw-rw-rw-   0        0        0     2568 2023-04-13 17:35:46.000000 responsibleai_vision-0.2.0/responsibleai_vision/utils/image_utils.py
--rw-rw-rw-   0        0        0      194 2023-05-05 17:31:42.000000 responsibleai_vision-0.2.0/responsibleai_vision/version.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:33:39.927458 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/
--rw-rw-rw-   0        0        0     1403 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 17:33:40.199850 responsibleai_vision-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1417 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.199850 responsibleai_vision-0.2.0/tests/
--rw-rw-rw-   0        0        0     4575 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.0/tests/test_rai_vision_automl_images_insights.py
--rw-rw-rw-   0        0        0     7899 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.0/tests/test_rai_vision_insights.py
--rw-rw-rw-   0        0        0     3082 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.0/tests/test_rai_vision_insights_save_and_load_scenarios.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:48:38.051345 responsibleai_vision-0.2.1/
+-rw-rw-rw-   0        0        0     1403 2023-05-31 18:48:38.050342 responsibleai_vision-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      691 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.797791 responsibleai_vision-0.2.1/responsibleai_vision/
+-rw-rw-rw-   0        0        0      367 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.871887 responsibleai_vision-0.2.1/responsibleai_vision/common/
+-rw-rw-rw-   0        0        0      127 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/common/__init__.py
+-rw-rw-rw-   0        0        0     2518 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.1/responsibleai_vision/common/constants.py
+-rw-rw-rw-   0        0        0      223 2022-09-01 02:31:14.000000 responsibleai_vision-0.2.1/responsibleai_vision/common/interfaces.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.908697 responsibleai_vision-0.2.1/responsibleai_vision/managers/
+-rw-rw-rw-   0        0        0      109 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/managers/__init__.py
+-rw-rw-rw-   0        0        0    13897 2023-05-05 19:17:38.000000 responsibleai_vision-0.2.1/responsibleai_vision/managers/error_analysis_manager.py
+-rw-rw-rw-   0        0        0    26315 2023-05-04 17:50:06.000000 responsibleai_vision-0.2.1/responsibleai_vision/managers/explainer_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.932563 responsibleai_vision-0.2.1/responsibleai_vision/rai_vision_insights/
+-rw-rw-rw-   0        0        0      253 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/rai_vision_insights/__init__.py
+-rw-rw-rw-   0        0        0    46805 2023-05-31 14:23:26.000000 responsibleai_vision-0.2.1/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.981601 responsibleai_vision-0.2.1/responsibleai_vision/utils/
+-rw-rw-rw-   0        0        0      129 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/responsibleai_vision/utils/__init__.py
+-rw-rw-rw-   0        0        0     2443 2023-05-12 20:02:09.000000 responsibleai_vision-0.2.1/responsibleai_vision/utils/feature_extractors.py
+-rw-rw-rw-   0        0        0     2824 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.1/responsibleai_vision/utils/image_reader.py
+-rw-rw-rw-   0        0        0     2880 2023-05-30 17:49:11.000000 responsibleai_vision-0.2.1/responsibleai_vision/utils/image_utils.py
+-rw-rw-rw-   0        0        0      194 2023-05-31 18:43:36.000000 responsibleai_vision-0.2.1/responsibleai_vision/version.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:48:37.839844 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/
+-rw-rw-rw-   0        0        0     1403 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-31 18:48:37.000000 responsibleai_vision-0.2.1/responsibleai_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 18:48:38.052494 responsibleai_vision-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1417 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:48:38.046193 responsibleai_vision-0.2.1/tests/
+-rw-rw-rw-   0        0        0     4575 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.1/tests/test_rai_vision_automl_images_insights.py
+-rw-rw-rw-   0        0        0     8318 2023-05-30 17:49:11.000000 responsibleai_vision-0.2.1/tests/test_rai_vision_insights.py
+-rw-rw-rw-   0        0        0     3401 2023-05-31 14:23:26.000000 responsibleai_vision-0.2.1/tests/test_rai_vision_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_vision-0.2.0/PKG-INFO` & `responsibleai_vision-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_vision
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_vision-0.2.0/README.md` & `responsibleai_vision-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision/common/constants.py` & `responsibleai_vision-0.2.1/responsibleai_vision/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision/managers/error_analysis_manager.py` & `responsibleai_vision-0.2.1/responsibleai_vision/managers/error_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision/managers/explainer_manager.py` & `responsibleai_vision-0.2.1/responsibleai_vision/managers/explainer_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision/rai_vision_insights/rai_vision_insights.py` & `responsibleai_vision-0.2.1/responsibleai_vision/rai_vision_insights/rai_vision_insights.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                                                    ModelTask)
 from responsibleai_vision.managers.explainer_manager import ExplainerManager
 from responsibleai_vision.managers.error_analysis_manager import (
     ErrorAnalysisManager)
 from responsibleai_vision.utils.feature_extractors import extract_features
 from responsibleai_vision.utils.image_reader import (
     get_base64_string_from_path, get_image_from_path, is_automl_image_model)
-from responsibleai_vision.utils.image_utils import get_images
+from responsibleai_vision.utils.image_utils import convert_images, get_images
 
 IMAGE = ImageColumns.IMAGE.value
 IMAGE_URL = ImageColumns.IMAGE_URL.value
 _IMAGE_MODE = 'image_mode'
 _IMAGE_DOWNLOADER = 'image_downloader'
 _PREDICTIONS = 'predictions'
 _TEST = 'test'
@@ -178,15 +178,15 @@
             task_type=task_type,
             test=test,
             target_column=target_column,
             classes=classes
         )
         self.predict_output = None
         super(RAIVisionInsights, self).__init__(
-            model, test, test, target_column, task_type,
+            model, None, test, target_column, task_type,
             serializer)
 
         ext_test, ext_features = extract_features(
             self.test, self.target_column, self.task_type,
             self.image_mode,
             self._feature_metadata.dropped_features)
         self._ext_test = ext_test
@@ -719,18 +719,15 @@
         returned as is.
 
         :param dataset: The dataset to convert.
         :type dataset: numpy.ndarray
         :return: The converted dataset.
         :rtype: numpy.ndarray
         """
-        if len(dataset) > 0 and isinstance(dataset[0], str):
-            dataset = np.array([get_image_from_path(
-                x, self.image_mode) for x in dataset])
-        return dataset
+        return convert_images(dataset, self.image_mode)
 
     def _convert_images_base64_df(self, dataset: pd.DataFrame) -> pd.DataFrame:
         """Converts the images to the format required by the model.
 
         If the images are base64 encoded, they are decoded and converted to
         numpy arrays. If the images are already numpy arrays, they are
         returned as is.
@@ -914,16 +911,15 @@
            task type and the classes (if any).
 
         :param path: The directory path to save the RAIVisionInsights to.
         :type path: str
         """
         top_dir = Path(path)
         classes = convert_to_list(self._classes)
-        if self._feature_metadata is not None:
-            feature_metadata_dict = self._feature_metadata.to_dict()
+        feature_metadata_dict = self._feature_metadata.to_dict()
         meta = {
             _TARGET_COLUMN: self.target_column,
             _TASK_TYPE: self.task_type,
             _CLASSES: classes,
             _IMAGE_MODE: self.image_mode,
             _FEATURE_METADATA: feature_metadata_dict,
         }
```

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision/utils/feature_extractors.py` & `responsibleai_vision-0.2.1/responsibleai_vision/utils/feature_extractors.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     :type target_column: str or list[str]
     :param task_type: The type of task to be performed.
     :type task_type: str
     :param image_mode: The mode to open the image in.
         See pillow documentation for all modes:
         https://pillow.readthedocs.io/en/stable/handbook/concepts.html
     :type image_mode: str
+    :param dropped_features: The list of features to drop from the dataset.
+    :type dropped_features: list[str]
     :return: The list of extracted features and the feature names.
     :rtype: list, list
     '''
     results = []
     feature_names = ["mean_pixel_value"]
     column_names = image_dataset.columns
     has_dropped_features = dropped_features is not None
```

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision/utils/image_reader.py` & `responsibleai_vision-0.2.1/responsibleai_vision/utils/image_reader.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision/utils/image_utils.py` & `responsibleai_vision-0.2.1/responsibleai_vision/utils/image_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,23 @@
         See pillow documentation for all modes:
         https://pillow.readthedocs.io/en/stable/handbook/concepts.html
     :type image_mode: str
     :return: The converted dataset.
     :rtype: numpy.ndarray
     """
     if len(dataset) > 0 and isinstance(dataset[0], str):
-        dataset = np.array([get_image_from_path(
-            x, image_mode) for x in dataset])
+        try:
+            dataset = np.array([get_image_from_path(
+                x, image_mode) for x in dataset])
+        except ValueError:
+            # if images of different sizes, try to convert one by one
+            jagged = np.empty(len(dataset), dtype=object)
+            for i, x in enumerate(dataset):
+                jagged[i] = get_image_from_path(x, image_mode)
+            dataset = jagged
     return dataset
 
 
 def get_images(dataset, image_mode, transformations=None):
     """Get the images from the dataset.
 
     If transformations are provided as a callable, the images
```

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision.egg-info/PKG-INFO` & `responsibleai_vision-0.2.1/responsibleai_vision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-vision
-Version: 0.2.0
+Version: 0.2.1
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_vision-0.2.0/responsibleai_vision.egg-info/SOURCES.txt` & `responsibleai_vision-0.2.1/responsibleai_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.0/setup.py` & `responsibleai_vision-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.0/tests/test_rai_vision_automl_images_insights.py` & `responsibleai_vision-0.2.1/tests/test_rai_vision_automl_images_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.2.0/tests/test_rai_vision_insights.py` & `responsibleai_vision-0.2.1/tests/test_rai_vision_insights.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     load_fridge_object_detection_dataset,
     load_mnist_dataset,
     create_image_classification_pipeline,
     load_imagenet_labels, retrieve_or_train_fridge_model,
     retrieve_fridge_object_detection_model,
     FRIDGE_MULTILABEL_TARGETS,
     ImageTransforms,
-    ImageTransformEnum)
+    ImageTransformEnum,
+    load_flowers_dataset,
+    create_dummy_model)
 from responsibleai_vision.common.constants import ImageColumns
 from rai_vision_insights_validator import validate_rai_vision_insights
 
 
 class TestRAIVisionInsights(object):
 
     def test_rai_insights_image_classification_imagenet(self):
@@ -145,14 +147,23 @@
         class_names = np.array(['can', 'carton',
                                 'milk_bottle', 'water_bottle'])
         dropped_features = [i for i in range(0, 10)]
         run_rai_insights(model, data[:3], ImageColumns.LABEL,
                          task_type, class_names,
                          dropped_features=dropped_features)
 
+    def test_jagged_image_sizes(self):
+        data = load_flowers_dataset()
+        model = create_dummy_model(data)
+        test_data = data
+        class_names = data[ImageColumns.LABEL.value].unique()
+        task_type = ModelTask.IMAGE_CLASSIFICATION
+        run_rai_insights(model, test_data, ImageColumns.LABEL,
+                         task_type, class_names)
+
 
 def run_rai_insights(model, test_data, target_column,
                      task_type, classes=None, test_explainer=False,
                      test_error_analysis=False,
                      image_mode=None, dropped_features=None):
     feature_metadata = None
     if dropped_features:
```

