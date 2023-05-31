# Comparing `tmp/pynir-0.7.6.tar.gz` & `tmp/pynir-0.7.7.tar.gz`

## Comparing `pynir-0.7.6.tar` & `pynir-0.7.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynir-0.7.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/Makefile
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/conf.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/make.bat
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/modules.rst
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/pynir.rst
--rw-r--r--   0        0        0   530403 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/doctrees/modules.doctree
--rw-r--r--   0        0        0   279145 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/doctrees/pynir.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0    21444 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/index.html
--rw-r--r--   0        0        0    26832 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/modules.html
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0   118287 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/pynir.html
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/search.html
--rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_modules/index.html
--rw-r--r--   0        0        0   102728 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_modules/pynir/Calibration.html
--rw-r--r--   0        0        0    73899 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_modules/pynir/CalibrationTransfer.html
--rw-r--r--   0        0        0    53422 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_modules/pynir/FeatureSelection.html
--rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_modules/pynir/OutlierDection.html
--rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_modules/pynir/Preprocessing.html
--rw-r--r--   0        0        0    25985 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_modules/pynir/utils.html
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_sources/pynir.rst.txt
--rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pynir-0.7.6/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0  1215471 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Data_Corn.mat
--rw-r--r--   0        0        0  5505213 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Data_Tablet.mat
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo11_calibrationTransfer_PFCE_Tablet.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo12_calibrationTransfer_PFCE_Corn.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo1_SimulateNIR.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo2_Regression.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo3_Binary_Classification.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo4_Multiclass_Classification.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo5_dataPreprocessing.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo6_outierDection.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo7_FeatureSelection_oneStep.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo8_FeatureSelection_multiSteps.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pynir-0.7.6/examples/Demo9_calibrationTransfer.py
--rw-r--r--   0        0        0    19671 2020-02-02 00:00:00.000000 pynir-0.7.6/src/pynir/Calibration.py
--rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 pynir-0.7.6/src/pynir/CalibrationTransfer.py
--rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pynir-0.7.6/src/pynir/FeatureSelection.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pynir-0.7.6/src/pynir/OutlierDection.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 pynir-0.7.6/src/pynir/Preprocessing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynir-0.7.6/src/pynir/__init__.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 pynir-0.7.6/src/pynir/utils.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pynir-0.7.6/LICENSE.txt
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 pynir-0.7.6/README.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynir-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     9025 2020-02-02 00:00:00.000000 pynir-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynir-0.7.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/Makefile
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/conf.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/make.bat
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/modules.rst
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/pynir.rst
+-rw-r--r--   0        0        0   530403 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/doctrees/modules.doctree
+-rw-r--r--   0        0        0   279145 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/doctrees/pynir.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0    21444 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/index.html
+-rw-r--r--   0        0        0    26832 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/modules.html
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0   118287 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/pynir.html
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/search.html
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/index.html
+-rw-r--r--   0        0        0   102728 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/Calibration.html
+-rw-r--r--   0        0        0    73899 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/CalibrationTransfer.html
+-rw-r--r--   0        0        0    53422 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/FeatureSelection.html
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/OutlierDection.html
+-rw-r--r--   0        0        0    24364 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/Preprocessing.html
+-rw-r--r--   0        0        0    25985 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_modules/pynir/utils.html
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_sources/pynir.rst.txt
+-rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pynir-0.7.7/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0  1215471 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Data_Corn.mat
+-rw-r--r--   0        0        0  5505213 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Data_Tablet.mat
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo11_calibrationTransfer_PFCE_Tablet.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo12_calibrationTransfer_PFCE_Corn.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo1_SimulateNIR.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo2_Regression.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo3_Binary_Classification.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo4_Multiclass_Classification.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo5_dataPreprocessing.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo6_outierDection.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo7_FeatureSelection_oneStep.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo8_FeatureSelection_multiSteps.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 pynir-0.7.7/examples/Demo9_calibrationTransfer.py
+-rw-r--r--   0        0        0    20004 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/Calibration.py
+-rw-r--r--   0        0        0    11020 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/CalibrationTransfer.py
+-rw-r--r--   0        0        0     8536 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/FeatureSelection.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/OutlierDection.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/Preprocessing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/__init__.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 pynir-0.7.7/src/pynir/utils.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pynir-0.7.7/LICENSE.txt
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 pynir-0.7.7/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynir-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     9025 2020-02-02 00:00:00.000000 pynir-0.7.7/PKG-INFO
```

### Comparing `pynir-0.7.6/.github/workflows/python-publish.yml` & `pynir-0.7.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/Makefile` & `pynir-0.7.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/conf.py` & `pynir-0.7.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/make.bat` & `pynir-0.7.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/pynir.rst` & `pynir-0.7.7/docs/pynir.rst`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/doctrees/environment.pickle` & `pynir-0.7.7/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/doctrees/index.doctree` & `pynir-0.7.7/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/doctrees/modules.doctree` & `pynir-0.7.7/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/doctrees/pynir.doctree` & `pynir-0.7.7/docs/_build/doctrees/pynir.doctree`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/genindex.html` & `pynir-0.7.7/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/index.html` & `pynir-0.7.7/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/modules.html` & `pynir-0.7.7/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/objects.inv` & `pynir-0.7.7/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/py-modindex.html` & `pynir-0.7.7/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/pynir.html` & `pynir-0.7.7/docs/_build/html/pynir.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/search.html` & `pynir-0.7.7/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/searchindex.js` & `pynir-0.7.7/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_modules/index.html` & `pynir-0.7.7/docs/_build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_modules/pynir/Calibration.html` & `pynir-0.7.7/docs/_build/html/_modules/pynir/Calibration.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_modules/pynir/CalibrationTransfer.html` & `pynir-0.7.7/docs/_build/html/_modules/pynir/CalibrationTransfer.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_modules/pynir/FeatureSelection.html` & `pynir-0.7.7/docs/_build/html/_modules/pynir/FeatureSelection.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_modules/pynir/OutlierDection.html` & `pynir-0.7.7/docs/_build/html/_modules/pynir/OutlierDection.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_modules/pynir/Preprocessing.html` & `pynir-0.7.7/docs/_build/html/_modules/pynir/Preprocessing.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_modules/pynir/utils.html` & `pynir-0.7.7/docs/_build/html/_modules/pynir/utils.html`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_sources/pynir.rst.txt` & `pynir-0.7.7/docs/_build/html/_sources/pynir.rst.txt`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_static/alabaster.css` & `pynir-0.7.7/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_static/basic.css` & `pynir-0.7.7/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_static/doctools.js` & `pynir-0.7.7/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_static/language_data.js` & `pynir-0.7.7/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_static/pygments.css` & `pynir-0.7.7/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_static/searchtools.js` & `pynir-0.7.7/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/docs/_build/html/_static/sphinx_highlight.js` & `pynir-0.7.7/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/examples/Data_Corn.mat` & `pynir-0.7.7/examples/Data_Corn.mat`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/examples/Data_Tablet.mat` & `pynir-0.7.7/examples/Data_Tablet.mat`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py` & `pynir-0.7.7/examples/Demo10_calibrationTransfer_PFCE_simulateNIR.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,18 @@
+import os
+import sys
+
+current_dir = os.path.dirname(__file__)
+parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
+pynir_dir = os.path.join(parent_dir, 'src')
+if pynir_dir not in sys.path:
+    sys.path.insert(0, pynir_dir)
+    
 from pynir.utils import simulateNIR_calibrationTransfer
-from pynir.Calibration import pls, regresssionReport
+from pynir.Calibration import pls, regressionReport
 from pynir.CalibrationTransfer import NS_PFCE,SS_PFCE,FS_PFCE,MT_PFCE
 import matplotlib.pyplot as plt
 import numpy as np
 
 from sklearn.model_selection import train_test_split
 
 import time
```

### Comparing `pynir-0.7.6/examples/Demo11_calibrationTransfer_PFCE_Tablet.py` & `pynir-0.7.7/examples/Demo11_calibrationTransfer_PFCE_Tablet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
+import os
 import sys
-from pathlib import Path
 
-pynir_path = str(Path(__file__).parent.parent / 'src')
-
-if pynir_path not in sys.path:
-    sys.path.append(pynir_path)
-    print("add pynir path")
+current_dir = os.path.dirname(__file__)
+parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
+pynir_dir = os.path.join(parent_dir, 'src')
+if pynir_dir not in sys.path:
+    sys.path.insert(0, pynir_dir)
 
 from pynir.utils import simulateNIR_calibrationTransfer
-from pynir.Calibration import pls, regresssionReport
+from pynir.Calibration import pls, regressionReport
 from pynir.CalibrationTransfer import NS_PFCE,SS_PFCE,FS_PFCE,MT_PFCE
 import matplotlib.pyplot as plt
 import numpy as np
 
 from scipy.io import loadmat
 
 from sklearn.model_selection import train_test_split
 
 import time
 
 
-RawData = loadmat("./Data_Tablet.mat")
+RawData = loadmat(os.path.join(current_dir, "Data_Tablet.mat"))
 wv = RawData["wv"].ravel()
 Xcal1 = RawData["Xcal1"]
 Xcal2 = RawData["Xcal2"]
 Xtrans1 = RawData["Xtrans1"]
 Xtrans2 = RawData["Xtrans2"]
 Xtest1 = RawData["Xtest1"]
 Xtest2 = RawData["Xtest2"]
```

### Comparing `pynir-0.7.6/examples/Demo12_calibrationTransfer_PFCE_Corn.py` & `pynir-0.7.7/examples/Demo12_calibrationTransfer_PFCE_Corn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
+import os
 import sys
-from pathlib import Path
 
-pynir_path = str(Path(__file__).parent.parent / 'src')
-
-if pynir_path not in sys.path:
-    sys.path.append(pynir_path)
-    print("add pynir path")
+current_dir = os.path.dirname(__file__)
+parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
+pynir_dir = os.path.join(parent_dir, 'src')
+if pynir_dir not in sys.path:
+    sys.path.insert(0, pynir_dir)
 
 from pynir.utils import simulateNIR_calibrationTransfer
-from pynir.Calibration import pls, regresssionReport
+from pynir.Calibration import pls, regressionReport
 from pynir.CalibrationTransfer import NS_PFCE,SS_PFCE,FS_PFCE,MT_PFCE
 import matplotlib.pyplot as plt
 import numpy as np
 
 from scipy.io import loadmat
 
 from sklearn.model_selection import train_test_split
 
 import time
 
 
-RawData = loadmat("./Data_Corn.mat")
+RawData = loadmat(os.path.join(current_dir, "Data_Corn.mat"))
 wv = RawData["wv"].ravel()
 Xcal1 = RawData["Xcal1"]
 Xcal2 = RawData["Xcal2"]
 Xcal3 = RawData["Xcal3"]
 Xtrans1 = RawData["Xtrans1"]
 Xtrans2 = RawData["Xtrans2"]
 Xtrans3 = RawData["Xtrans3"]
@@ -46,20 +46,20 @@
 ax[2].plot(wv, np.transpose(Xcal3))
 ax[2].set_title("Third")
 
 fig.supxlabel("Wavelength (nm)")
 fig.supylabel("Intensity(A.U.)")
 plt.show()
 
-nComp = 4
-plsModel1 = pls(nComp=nComp).fit(Xcal1, ycal)
+n_components = 4
+plsModel1 = pls(n_components=n_components).fit(Xcal1, ycal)
 
-yhat1 = plsModel1.predict(Xtest1,nComp=nComp)
-yhat2= plsModel1.predict(Xtest2,nComp=nComp)
-yhat3= plsModel1.predict(Xtest3,nComp=nComp)
+yhat1 = plsModel1.predict(Xtest1,n_components=n_components)
+yhat2= plsModel1.predict(Xtest2,n_components=n_components)
+yhat3= plsModel1.predict(Xtest3,n_components=n_components)
 
 fig, ax = plt.subplots(3,sharex=True,figsize=(8,16))
 plsModel1.plot_prediction(ytest, yhat1,title = "First", ax = ax[0])
 plsModel1.plot_prediction(ytest, yhat2, title= "Second", ax = ax[1])
 plsModel1.plot_prediction(ytest, yhat3, title= "Third", ax = ax[2])
 
 fig, ax = plt.subplots()
@@ -123,18 +123,18 @@
 ax.set_ylabel("Regression Coefficients")
 ax.set_title("FS-PFCE")
 print("cost {:.2f} seconds for FS-PFCE".format(time.time()-tic))
 
 
 ## MT-PFCE
 tic = time.time()
-plsModel_global = pls(nComp=nComp).fit(np.vstack((Xcal1,Xtrans2,Xtrans3)),
+plsModel_global = pls(n_components=n_components).fit(np.vstack((Xcal1,Xtrans2,Xtrans3)),
                                        np.vstack((ycal,ytrans,ytrans)))
 optLV_global = plsModel_global.get_optLV()
-plsModel_global = pls(nComp=optLV_global).fit(np.vstack((Xcal1,Xtrans2,Xtrans3)),
+plsModel_global = pls(n_components=optLV_global).fit(np.vstack((Xcal1,Xtrans2,Xtrans3)),
                                        np.vstack((ycal,ytrans,ytrans)))
 
 bglb = plsModel_global.model['B'][:,-1]
 MT_PFCE_model = MT_PFCE(thres=thres, constrType=constrType)
 MT_PFCE_model.fit([Xcal1,Xtrans2,Xtrans3],(ycal,ytrans,ytrans),bglb)
 yhat1_MT_PFCE = MT_PFCE_model.transform(Xtest1,0) # task 1
 yhat2_MT_PFCE = MT_PFCE_model.transform(Xtest2,1) # task 2
```

### Comparing `pynir-0.7.6/examples/Demo2_Regression.py` & `pynir-0.7.7/examples/Demo2_Regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from pynir.utils import simulateNIR
 from pynir.Calibration import pls
-from pynir.Calibration import regresssionReport
+from pynir.Calibration import regressionReport
 
 from sklearn.model_selection import train_test_split
 
 # simulate NIR data
 X,y,wv = simulateNIR(nSample=200,n_components=10,noise=1e-5)
 
 Xtrain, Xtest, ytrain,ytest = train_test_split(X,y,test_size=0.2)
@@ -37,17 +37,17 @@
 rmsep = []
 
 r2c = []
 r2cv = []
 r2p = []
 
 for i in range(n_components):
-    report_train = regresssionReport(ytrain, yhat_train[:,i])
-    report_cv = regresssionReport(ytrain, yhat_cv[:,i])
-    report_test = regresssionReport(ytest, yhat_test[:,i])
+    report_train = regressionReport(ytrain, yhat_train[:,i])
+    report_cv = regressionReport(ytrain, yhat_cv[:,i])
+    report_test = regressionReport(ytest, yhat_test[:,i])
 
     rmsec.append(report_train["rmse"])
     rmsecv.append(report_cv["rmse"])
     rmsep.append(report_test["rmse"])
 
     r2c.append(report_train["r2"])
     r2cv.append(report_cv["r2"])
```

### Comparing `pynir-0.7.6/examples/Demo3_Binary_Classification.py` & `pynir-0.7.7/examples/Demo3_Binary_Classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 from pynir.Calibration import binaryClassificationReport,plot_confusion_matrix
 
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import confusion_matrix
 
 
 # simulate NIR data
-X,y,wv = simulateNIR(nSample=200,nComp=10,refType=2, noise=1e-5)
+X,y,wv = simulateNIR(nSample=200,n_components=10,refType=2, noise=1e-5)
 
 Xtrain, Xtest, ytrain,ytest = train_test_split(X,y,test_size=0.2)
 
 # estabilish PLS model
-nComp = 10
-plsdaModel = plsda(n_components = nComp).fit(Xtrain,ytrain)
+n_components = 10
+plsdaModel = plsda(n_components = n_components).fit(Xtrain,ytrain)
 
 # 10 fold cross validation for selecting optimal nlv
 accuracy_cv = []
 yhat_cv  = plsdaModel.crossValidation_predict(nfold = 10)
-for i in range(nComp):
+for i in range(n_components):
     report_cv = binaryClassificationReport(ytrain, yhat_cv[:,i])
     accuracy_cv.append(report_cv["accuracy"])
 
 
 fig,ax = plt.subplots()
-ax.plot(np.arange(nComp)+1,accuracy_cv, marker = "*",label = "Accuracy$_c$$_v$")
+ax.plot(np.arange(n_components)+1,accuracy_cv, marker = "*",label = "Accuracy$_c$$_v$")
 ax.set_xlabel("nLV")
 ax.set_ylabel("Accuracy")
 ax.legend()
 plt.show()
 
 
 optLV = plsdaModel.get_optLV()  # optimized nLV based on cross validation
```

### Comparing `pynir-0.7.6/examples/Demo4_Multiclass_Classification.py` & `pynir-0.7.7/examples/Demo4_Multiclass_Classification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+import os
+import sys
+
+current_dir = os.path.dirname(__file__)
+parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
+pynir_dir = os.path.join(parent_dir, 'src')
+if pynir_dir not in sys.path:
+    sys.path.insert(0, pynir_dir)
+
 import numpy as np
 import matplotlib.pyplot as plt
 
 from pynir.utils import simulateNIR
 from pynir.Calibration import plsda
 from pynir.Calibration import multiClassificationReport,plot_confusion_matrix
```

### Comparing `pynir-0.7.6/examples/Demo5_dataPreprocessing.py` & `pynir-0.7.7/examples/Demo5_dataPreprocessing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+import os
+import sys
+
+current_dir = os.path.dirname(__file__)
+parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
+pynir_dir = os.path.join(parent_dir, 'src')
+if pynir_dir not in sys.path:
+    sys.path.insert(0, pynir_dir)
+    
 import numpy as np
 import matplotlib.pyplot as plt
 
 from pynir.utils import simulateNIR
 
 from pynir.Preprocessing import snv,cwt,msc,SG_filtering
```

### Comparing `pynir-0.7.6/examples/Demo7_FeatureSelection_oneStep.py` & `pynir-0.7.7/examples/Demo7_FeatureSelection_oneStep.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Time    : 2019.4.30
-# @Author  : FrankEl
+# @Author  : Jin Zhang
 # @File    : Feature_selection_demo_mcuve.py
+import os
+import sys
+
+current_dir = os.path.dirname(__file__)
+parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
+pynir_dir = os.path.join(parent_dir, 'src')
+if pynir_dir not in sys.path:
+    sys.path.insert(0, pynir_dir)
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from pynir.utils import simulateNIR
 from pynir.Calibration import pls
 from pynir.FeatureSelection import MCUVE,RT,VC,plotFeatureSelection
```

### Comparing `pynir-0.7.6/examples/Demo8_FeatureSelection_multiSteps.py` & `pynir-0.7.7/examples/Demo8_FeatureSelection_multiSteps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Time    : 2019.4.30
-# @Author  : FrankEl
+# @Author  : Jin Zhang
 # @File    : Feature_selection_demo_rt.py
+import os
+import sys
+
+current_dir = os.path.dirname(__file__)
+parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
+pynir_dir = os.path.join(parent_dir, 'src')
+if pynir_dir not in sys.path:
+    sys.path.insert(0, pynir_dir)
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.io as scio
 from sklearn.cross_decomposition import PLSRegression
 from sklearn.model_selection import train_test_split
 from numpy.linalg import matrix_rank as rank
```

### Comparing `pynir-0.7.6/examples/Demo9_calibrationTransfer.py` & `pynir-0.7.7/examples/Demo9_calibrationTransfer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,18 @@
+import os
+import sys
+
+current_dir = os.path.dirname(__file__)
+parent_dir = os.path.abspath(os.path.join(current_dir, os.pardir))
+pynir_dir = os.path.join(parent_dir, 'src')
+if pynir_dir not in sys.path:
+    sys.path.insert(0, pynir_dir)
+
 from pynir.utils import simulateNIR_calibrationTransfer
-from pynir.Calibration import pls, regresssionReport
+from pynir.Calibration import pls, regressionReport
 from pynir.CalibrationTransfer import PDS,SST, BS
 import matplotlib.pyplot as plt
 import numpy as np
 
 from sklearn.model_selection import train_test_split
 
 # Simulate NIR spectra for calibration transfer
```

### Comparing `pynir-0.7.6/src/pynir/Calibration.py` & `pynir-0.7.7/src/pynir/Calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         return yhat
 
     def get_optLV(self, nfold=10):
         yhat_cv = self.crossValidation_predict(nfold)
         rmsecv = []
         r2cv = []
         for i in range(yhat_cv.shape[1]):
-            reportcv = regresssionReport(self.y, yhat_cv[:, i])
+            reportcv = regressionReport(self.y, yhat_cv[:, i])
             rmsecv.append(reportcv["rmse"])
             r2cv.append(reportcv["r2"])
         optLV = int(np.argmin(rmsecv)+1)
         self.optLV = optLV
         return optLV
 
     def transform(self, Xnew):
@@ -127,15 +127,15 @@
         W0 = x_weights / np.sqrt(np.sum(x_weights**2, axis=0))
         p = x_loadings.shape[0]
         sumSq = np.sum(x_scores**2, axis=0) * np.sum(y_loadings**2, axis=1)
         vipScore = np.sqrt(p * np.sum(sumSq * (W0**2), axis=1) / np.sum(sumSq))
         return vipScore
 
     def plot_prediction(self, y, yhat, xlabel="Reference", ylabel="Prediction", title="", ax=None):
-        report = regresssionReport(y, yhat)
+        report = regressionReport(y, yhat)
         if ax == None:
             fig, ax = plt.subplots()
         ax.plot([np.min(y)*0.95, np.max(y)*1.05], [np.min(y)*0.95, np.max(y)*1.05],
                 color='black', label="y=x")
         ax.scatter(y, yhat, color='tab:green', marker='*', label='Prediction')
         ax.text(0.7, 0.03,
                 "RMSEP = {:.4f}\nR$^2$ = {:.2}".format(
@@ -397,15 +397,25 @@
         report["accuracy"] = accuracy_score(ytrue, ypred)
         report["sensitivity"] = recall_score(ytrue, ypred)  # recall
         report["specificity"] = tn/(tn+fp)
         report["f1"] = f1_score(ytrue, ypred)
         return report
 
 
-def regresssionReport(ytrue, ypred):
+def regressionReport(ytrue, ypred):
+    '''
+    Computes the root mean squared error (RMSE) and R-squared (R2) for regression models.
+
+    Parameters:
+    ytrue (array-like): True values of the dependent variable.
+    ypred (array-like): Predicted values of the dependent variable.
+
+    Returns:
+    dict: A dictionary containing the RMSE and R2 values.
+    '''
     report = dict()
     report["rmse"] = mean_squared_error(ytrue, ypred, squared=False)
     report["r2"] = r2_score(ytrue, ypred)
     return report
 
 
 def simpls(X, y, n_components):
```

### Comparing `pynir-0.7.6/src/pynir/CalibrationTransfer.py` & `pynir-0.7.7/src/pynir/CalibrationTransfer.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/src/pynir/FeatureSelection.py` & `pynir-0.7.7/src/pynir/FeatureSelection.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/src/pynir/OutlierDection.py` & `pynir-0.7.7/src/pynir/OutlierDection.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/src/pynir/Preprocessing.py` & `pynir-0.7.7/src/pynir/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/src/pynir/utils.py` & `pynir-0.7.7/src/pynir/utils.py`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/LICENSE.txt` & `pynir-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/README.md` & `pynir-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pynir-0.7.6/pyproject.toml` & `pynir-0.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pynir"
-version = "0.7.6"
+version = "0.7.7"
 authors = [{ name = "Jin Zhang", email = "jinzhang@nankai.edu.cn" }]
 description = "NIR calibration toolbox in python"
 readme = "README.md"
 requires-python = ">=3.7"
 
 dependencies = [
   "numpy",
```

### Comparing `pynir-0.7.6/PKG-INFO` & `pynir-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynir
-Version: 0.7.6
+Version: 0.7.7
 Summary: NIR calibration toolbox in python
 Project-URL: Homepage, https://github.com/JinZhangLab/pynir
 Project-URL: Bug Tracker, https://github.com/JinZhangLab/pynir/issues
 Project-URL: Documentation, https://pynir.readthedocs.io/en/latest/
 Author-email: Jin Zhang <jinzhang@nankai.edu.cn>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
```

