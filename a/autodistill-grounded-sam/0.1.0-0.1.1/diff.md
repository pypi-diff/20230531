# Comparing `tmp/autodistill_grounded_sam-0.1.0.tar.gz` & `tmp/autodistill_grounded_sam-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autodistill_grounded_sam-0.1.0.tar", last modified: Sat May 27 02:59:42 2023, max compression
+gzip compressed data, was "autodistill_grounded_sam-0.1.1.tar", last modified: Wed May 31 06:40:06 2023, max compression
```

## Comparing `autodistill_grounded_sam-0.1.0.tar` & `autodistill_grounded_sam-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      599 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/PKG-INFO
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     3157 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/README.md
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       85 2023-05-27 02:59:06.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/__init__.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     2352 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/grounded_sam.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     4642 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/helpers.py
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      599 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/PKG-INFO
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      390 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/SOURCES.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)        1 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/dependency_links.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      155 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/requires.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       25 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/top_level.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       38 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/setup.cfg
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     1592 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/setup.py
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 02:59:42.000000 autodistill_grounded_sam-0.1.0/test/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       41 2023-05-27 02:55:23.000000 autodistill_grounded_sam-0.1.0/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:40:06.969679 autodistill_grounded_sam-0.1.1/
+-rw-r--r--   0 james      (501) staff       (20)      599 2023-05-31 06:40:06.969537 autodistill_grounded_sam-0.1.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     3157 2023-05-30 17:09:40.000000 autodistill_grounded_sam-0.1.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:40:06.968001 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam/
+-rw-r--r--   0 james      (501) staff       (20)       85 2023-05-31 06:38:30.000000 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2337 2023-05-30 17:44:48.000000 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam/grounded_sam.py
+-rw-r--r--   0 james      (501) staff       (20)     4642 2023-05-30 17:10:07.000000 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam/helpers.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:40:06.969003 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)      599 2023-05-31 06:40:06.000000 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      390 2023-05-31 06:40:06.000000 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-05-31 06:40:06.000000 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      155 2023-05-31 06:40:06.000000 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       25 2023-05-31 06:40:06.000000 autodistill_grounded_sam-0.1.1/autodistill_grounded_sam.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-05-31 06:40:06.969728 autodistill_grounded_sam-0.1.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1669 2023-05-31 06:39:52.000000 autodistill_grounded_sam-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:40:06.969175 autodistill_grounded_sam-0.1.1/test/
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-05-30 17:09:40.000000 autodistill_grounded_sam-0.1.1/test/test_hello.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autodistill_grounded_sam-0.1.0/PKG-INFO` & `autodistill_grounded_sam-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill_grounded_sam
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill_grounded_sam-0.1.0/README.md` & `autodistill_grounded_sam-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/grounded_sam.py` & `autodistill_grounded_sam-0.1.1/autodistill_grounded_sam/grounded_sam.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 torch.use_deterministic_algorithms(False)
 
 import supervision as sv
 from groundingdino.util.inference import Model
 from segment_anything import SamPredictor
 
 import numpy as np
-from autodistill.core import BaseModel
-from autodistill.detection import CaptionOntology
+from autodistill.detection import CaptionOntology, DetectionBaseModel
 
 from autodistill_grounded_sam.helpers import (
     combine_detections,
     load_grounding_dino,
     load_SAM
 )
 
 HOME = os.path.expanduser("~")
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 @dataclass
-class GroundedSAM(BaseModel):
+class GroundedSAM(DetectionBaseModel):
     ontology: CaptionOntology
     grounding_dino_model: Model
     sam_predictor: SamPredictor
     box_threshold: float
     text_threshold: float
 
     def __init__(self, ontology: CaptionOntology, box_threshold=0.35, text_threshold=0.25):
@@ -43,15 +42,15 @@
 
     def predict(self, input: str) -> sv.Detections:
         image = cv2.imread(input)
 
         # GroundingDINO predictions
         detections_list = []
 
-        for i, description in enumerate(self.ontology.descriptions()):
+        for i, description in enumerate(self.ontology.prompts()):
             # detect objects
             detections = self.grounding_dino_model.predict_with_classes(
                 image=image,
                 classes=[description],
                 box_threshold=self.box_threshold,
                 text_threshold=self.text_threshold,
             )
```

### Comparing `autodistill_grounded_sam-0.1.0/autodistill_grounded_sam/helpers.py` & `autodistill_grounded_sam-0.1.1/autodistill_grounded_sam/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill_grounded_sam-0.1.0/autodistill_grounded_sam.egg-info/PKG-INFO` & `autodistill_grounded_sam-0.1.1/autodistill_grounded_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-grounded-sam
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill_grounded_sam-0.1.0/setup.py` & `autodistill_grounded_sam-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,28 +14,33 @@
 with open("./autodistill_grounded_sam/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
-    
-with open("requirements.txt", "r") as fh:
-    install_requires = fh.read().split('\n')
 
 setuptools.setup(
     name="autodistill_grounded_sam", 
     version=version,
     author="Roboflow",
     author_email="jacob@roboflow.com",
     description="Automatically distill large foundational models into smaller, in-domain models for deployment",
     long_description="Automatically distill large foundational models into smaller, in-domain models for deployment",
     long_description_content_type="text/markdown",
     url="https://github.com/autodistill/autodistill",
-    install_requires=install_requires,
+    install_requires=[
+        "torch",
+        "autodistill",
+        "numpy>=1.20.0",
+        "opencv-python>=4.6.0",
+        "rf_groundingdino",
+        "rf_segment_anything",
+        "supervision"
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

