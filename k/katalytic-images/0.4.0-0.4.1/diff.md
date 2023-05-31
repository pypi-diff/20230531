# Comparing `tmp/katalytic-images-0.4.0.tar.gz` & `tmp/katalytic_images-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-images-0.4.0.tar", last modified: Sun May  7 10:08:38 2023, max compression
+gzip compressed data, was "katalytic_images-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic-images-0.4.0.tar` & `katalytic_images-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-images-0.4.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic-images-0.4.0/.gitignore
--rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic-images-0.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     2111 2023-05-07 10:08:33.713105 katalytic-images-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-images-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2130 2023-04-30 14:20:54.475497 katalytic-images-0.4.0/README.md
--rw-r--r--   0        0        0     1549 2023-05-07 10:08:33.713105 katalytic-images-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    10015 2023-05-07 10:03:19.751524 katalytic-images-0.4.0/src/katalytic/images.py
--rw-r--r--   0        0        0    14584 2023-05-07 10:06:02.709954 katalytic-images-0.4.0/tests/test_images.py
--rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 katalytic-images-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.4.1/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.4.1/.gitignore
+-rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.4.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2716 2023-05-31 06:43:54.787954 katalytic_images-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.4.1/README.md
+-rw-r--r--   0        0        0     1549 2023-05-31 06:43:54.787954 katalytic_images-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    21782 2023-05-31 06:26:00.533837 katalytic_images-0.4.1/src/katalytic/images.py
+-rw-r--r--   0        0        0    15603 2023-05-31 06:18:31.089140 katalytic_images-0.4.1/tests/test_images.py
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.4.1/PKG-INFO
```

### Comparing `katalytic-images-0.4.0/.gitignore` & `katalytic_images-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.4.0/.gitlab-ci.yml` & `katalytic_images-0.4.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.4.0/CHANGELOG.md` & `katalytic_images-0.4.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 0.4.1 (2023-05-31)
+### fix
+- [[`dc2fff6`](https://gitlab.com/katalytic/katalytic-images/commit/dc2fff66953ee47de40d78702ab6b55079800969)] ValueError -> TypeError
+- [[`44c3801`](https://gitlab.com/katalytic/katalytic-images/commit/44c38013096021262cdb3c5e8da0ff50972468cb)] convert types to what opencv expects
+- [[`c6fe7fa`](https://gitlab.com/katalytic/katalytic-images/commit/c6fe7fae2868c1340929704ba20cbcd303647aa1)] readme
+- [[`ecaef54`](https://gitlab.com/katalytic/katalytic-images/commit/ecaef54965aaaec043b8fd170a5d82c15071a8df)] remove unnecessary function and convert circle radius to int
+
+
 ## 0.4.0 (2023-05-07)
 ### feat
 - [[`dca7f3e`](https://gitlab.com/katalytic/katalytic-images/commit/dca7f3eb1ee463393fa8c872fcebe8f101b5f73c)] add create_{rectangle,circle,line,text,mask,polylines}
 
 
 ## 0.3.0 (2023-05-04)
 ### feat
```

### Comparing `katalytic-images-0.4.0/LICENSE.txt` & `katalytic_images-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.4.0/README.md` & `katalytic_images-0.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# Not fit for public use yet
+- I will probably introduce backwards incompatible changes
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-images)](https://pypi.org/project/katalytic-images/)
 [![tests](https://gitlab.com/katalytic/katalytic-images/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-images/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-images/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-images/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-images.svg)](https://katalytic-images.readthedocs.io/en/latest/)
@@ -35,8 +38,7 @@
 - Propose new features
 - Propose packaging, building, or deployment improvements
 - Report and fix bugs
 	- you can also submit an xfail test
 - Submit code and tests
 - Tell me what I'm doing wrong or when I'm not following best practices
 - Update the documentation
-
```

### Comparing `katalytic-images-0.4.0/pyproject.toml` & `katalytic_images-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.4.0"
+version = "0.4.1"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-images-0.4.0/tests/test_images.py` & `katalytic_images-0.4.1/tests/test_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,49 +125,72 @@
             _ = convert_image(img, 'RGB', 'unknown')
 
     def test_convert_from_unknown(self):
         img = np.array([[[0, 0, 0], [255, 255, 255]]])
         with pytest.raises(ValueError):
             _ = convert_image(img, 'unknown', 'RGB')
 
-    @pytest.mark.parametrize('before', [1, True, None, [], {}, (), object()])
-    def test_save_raises_ValueError_for_before(self, before):
-        with pytest.raises(ValueError):
+    @pytest.mark.parametrize('before', all_types_besides('str'))
+    def test_save_raises_TypeError_for_before(self, before):
+        with pytest.raises(TypeError):
             convert_image(_create_RGB(), before, 'RGB')
 
-    @pytest.mark.parametrize('after', [1, True, None, [], {}, (), object()])
-    def test_save_raises_ValueError_for_after(self, after):
-        with pytest.raises(ValueError):
+    @pytest.mark.parametrize('after', all_types_besides('str'))
+    def test_save_raises_TypeError_for_after(self, after):
+        with pytest.raises(TypeError):
             convert_image(_create_RGB(), 'RGB', after)
 
 
 class Test_draw:
     @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             draw(np.zeros((5, 5)), wrong_type)
 
     def test_draws_on_a_copy(self):
         img = np.zeros((5, 5, 3), dtype=np.uint8)
         img_copy = img.copy()
         shapes = [
             create_line((0,0), (0,3), (0, 255, 0), thickness=1),
-            create_rectangle((1,1), (3,3), (255, 0, 0), thickness=-1),
+            create_rectangle([1,1], (3,3), (255, 0, 0), thickness=-1),
             create_circle((4,4), 2, (0, 0, 255))
         ]
 
         img = draw(img, shapes)
         assert (img == [255, 0, 0]).all(axis=2).any()
         assert (img == [0, 255, 0]).all(axis=2).any()
         assert (img == [0, 0, 255]).all(axis=2).any()
 
         assert not (img_copy == [255, 0, 0]).all(axis=2).any()
         assert not (img_copy == [0, 255, 0]).all(axis=2).any()
         assert not (img_copy == [0, 0, 255]).all(axis=2).any()
 
+    def test_converts_to_type_expected_by_opencv(self):
+        line = create_line([0.0, 0.0], [0.0, 3.0], (0, 255, 0), thickness=1)
+        assert isinstance(line['p1'], tuple)
+        assert isinstance(line['p2'], tuple)
+        assert all([isinstance(x, int) for x in line['p1'] + line['p2']])
+
+        rect = create_rectangle([1.0, 1.0], [3.0, 3.0], (255, 0, 0), thickness=-1)
+        assert isinstance(rect['p1'], tuple)
+        assert isinstance(rect['p2'], tuple)
+        assert all([isinstance(x, int) for x in rect['p1'] + rect['p2']])
+
+        circle = create_circle([4.0, 4.0], 2, (0, 0, 255))
+        assert isinstance(circle['center'], tuple)
+        assert all([isinstance(x, int) for x in circle['center']])
+
+        text = create_text('hello', [0.0, 50.0], (0, 255, 0))
+        assert isinstance(text['origin'], tuple)
+        assert all([isinstance(x, int) for x in text['origin']])
+
+        # This will raise an error if anything else goes wrong
+        img = np.zeros((100, 100, 3), dtype=np.uint8)
+        draw(img, [line, rect, circle, text])
+
     def test_maintains_order_if_sequence(self):
         data = [
             create_line((0,0), (0,2), (0, 255, 0), thickness=1),
             create_line((0,1), (0,3), (0, 0, 255), thickness=1),
         ]
         expected = np.array([
             [[0, 255, 0]],
@@ -375,16 +398,16 @@
             save_image(_create_RGB(), path)
 
     @pytest.mark.parametrize('image', [1, True, None, [], {}, (), object()])
     def test_save_raises_TypeError_for_image(self, image):
         with pytest.raises(TypeError):
             save_image(image, get_unique_path('{}.png'))
 
-    @pytest.mark.parametrize('mode', ['unkonwn', '', 1, True, None, [], {}, (), object()])
+    @pytest.mark.parametrize('mode', [1, True, None, [], {}, (), object()])
     def test_save_raises_ValueError_for_mode(self, mode):
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             save_image(_create_RGB(), get_unique_path('{}.png'), mode=mode)
 
     @pytest.mark.parametrize('exists', ['unkonwn', '', 1, True, None, [], {}, (), object()])
     def test_save_raises_ValueError_for_exists(self, exists):
         with pytest.raises(ValueError):
             save_image(_create_RGB(), get_unique_path('{}.png'), exists=exists)
```

### Comparing `katalytic-images-0.4.0/PKG-INFO` & `katalytic_images-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.4.0
+Version: 0.4.1
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -28,14 +28,17 @@
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-images.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-images.git
 Provides-Extra: dev
 
+# Not fit for public use yet
+- I will probably introduce backwards incompatible changes
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-images)](https://pypi.org/project/katalytic-images/)
 [![tests](https://gitlab.com/katalytic/katalytic-images/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-images/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-images/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-images/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-images.svg)](https://katalytic-images.readthedocs.io/en/latest/)
@@ -70,8 +73,7 @@
 - Propose packaging, building, or deployment improvements
 - Report and fix bugs
 	- you can also submit an xfail test
 - Submit code and tests
 - Tell me what I'm doing wrong or when I'm not following best practices
 - Update the documentation
 
-
```

