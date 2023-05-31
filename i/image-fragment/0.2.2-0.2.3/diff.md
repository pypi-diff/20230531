# Comparing `tmp/image_fragment-0.2.2.tar.gz` & `tmp/image_fragment-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\image_fragment-0.2.2.tar", last modified: Fri Oct  9 07:10:13 2020, max compression
+gzip compressed data, was "image_fragment-0.2.3.tar", last modified: Wed May 31 10:33:02 2023, max compression
```

## Comparing `image_fragment-0.2.2.tar` & `image_fragment-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2020-10-09 07:10:13.000000 image_fragment-0.2.2/
--rw-rw-rw-   0        0        0       20 2020-09-01 06:26:00.000000 image_fragment-0.2.2/CHANGES.txt
--rw-rw-rw-   0        0        0       76 2020-08-31 03:40:28.000000 image_fragment-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2768 2020-10-09 07:10:13.000000 image_fragment-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1880 2020-10-09 07:10:08.000000 image_fragment-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2020-10-09 07:10:13.000000 image_fragment-0.2.2/image_fragment/
--rw-rw-rw-   0        0        0        0 2020-08-30 20:01:54.000000 image_fragment-0.2.2/image_fragment/__init__.py
--rw-rw-rw-   0        0        0    11384 2020-09-24 12:39:04.000000 image_fragment-0.2.2/image_fragment/fragment.py
-drwxrwxrwx   0        0        0        0 2020-10-09 07:10:13.000000 image_fragment-0.2.2/image_fragment.egg-info/
--rw-rw-rw-   0        0        0     2768 2020-10-09 07:10:13.000000 image_fragment-0.2.2/image_fragment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2020-10-09 07:10:13.000000 image_fragment-0.2.2/image_fragment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-09 07:10:13.000000 image_fragment-0.2.2/image_fragment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2020-10-09 07:10:13.000000 image_fragment-0.2.2/image_fragment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2020-10-09 07:10:13.000000 image_fragment-0.2.2/image_fragment.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2020-10-09 07:10:13.000000 image_fragment-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      791 2020-10-09 07:10:08.000000 image_fragment-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:33:02.866722 image_fragment-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 10:32:51.000000 image_fragment-0.2.3/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 10:32:51.000000 image_fragment-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 10:32:51.000000 image_fragment-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-31 10:33:02.866722 image_fragment-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-31 10:32:51.000000 image_fragment-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:33:02.866722 image_fragment-0.2.3/image_fragment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:32:51.000000 image_fragment-0.2.3/image_fragment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-05-31 10:32:51.000000 image_fragment-0.2.3/image_fragment/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:33:02.866722 image_fragment-0.2.3/image_fragment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-31 10:33:02.000000 image_fragment-0.2.3/image_fragment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-31 10:33:02.000000 image_fragment-0.2.3/image_fragment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:33:02.000000 image_fragment-0.2.3/image_fragment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 10:33:02.000000 image_fragment-0.2.3/image_fragment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 10:33:02.000000 image_fragment-0.2.3/image_fragment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 10:33:02.866722 image_fragment-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-31 10:32:51.000000 image_fragment-0.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `image_fragment-0.2.2/PKG-INFO` & `image_fragment-0.2.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,47 @@
-Metadata-Version: 2.1
-Name: image_fragment
-Version: 0.2.2
-Summary: Data Section
-Home-page: https://github.com/fuzailpalnak/fragment
-Author: Fuzail Palnak
-Author-email: fuzailpalnak@gmail.com
-License: UNKNOWN
-Description: # Fragment
-        ![GitHub](https://img.shields.io/github/license/fuzailpalnak/fragment)
-        ![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
-        ![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
-        
-        Any extent is a set of smaller fragment extent , which can be as small as *1 x 1* to the *size* of the extent given.
-        This library will section the given extent in to specified smaller fragment extent
-        
-        
-        ## Installation
-        
-            pip install image-fragment
-        
-        
-        ## Image Fragments
-        
-        ![fragments](https://user-images.githubusercontent.com/24665570/91711219-2b7c8980-eba3-11ea-94d2-8239cf6713c4.gif)
-        
-        An image extent can be sectioned into many fragments, these fragments holds positional information to where it is located 
-        to the original extent
-        
-        Now this information can be used to extract selected fragments from the Image, perform operation, and transfer the new 
-        data to selected position.
-        
-        
-        ```python
-        import numpy as np
-        from image_fragment.fragment import ImageFragment
-        
-        image = np.zeros((1, 1024, 1024, 3))
-        new_image = np.zeros((1, 1024, 1024, 3))
-        image_fragment = ImageFragment.image_fragment_4d(fragment_size=(1, 512, 512, 3), org_size=(1, 1024, 1024, 3))
-        for fragment in image_fragment:
-            # GET DATA THAT BELONGS TO THE FRAGMENT
-            fragmented_image = fragment.get_fragment_data(image)
-            
-            # DO SOME OPERATION ON THE FRAGMENTED DATA
-            operation_done_on_fragmented_data = np.rot(fragmented_image)
-            
-            # TRANSFER OPERATED IMAGE ON NEW IMAGE ON THE FRAGMENT POSITION
-            new_image = fragment.transfer_fragment(transfer_from=operation_done_on_fragmented_data, transfer_to=new_image)
-            
-        ```
-        
-        If image is 3 Dimensional then switch to `image_fragment = ImageFragment.image_fragment_3d(fragment_size=(512, 512, 3), org_size=(1024, 1024, 3))`, 
-        this will provide fragments for 3 dimensional image
-        
-Keywords: numpy, Window, Section, Array, Stitch, Split
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: ~=3.6
-Description-Content-Type: text/markdown
+# Fragment
+![GitHub](https://img.shields.io/github/license/fuzailpalnak/fragment)
+![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
+![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
+![Downloads](https://pepy.tech/badge/image-fragment)
+
+Any extent is a set of smaller fragment extent , which can be as small as *1 x 1* to the *size* of the extent given.
+This library will section the given extent in to specified smaller fragment extent
+
+
+## Installation
+
+    pip install image-fragment
+
+
+## Image Fragments
+
+![fragments](https://user-images.githubusercontent.com/24665570/91711219-2b7c8980-eba3-11ea-94d2-8239cf6713c4.gif)
+
+An image extent can be sectioned into many fragments, these fragments holds positional information to where it is located 
+to the original extent
+
+Now this information can be used to extract selected fragments from the Image, perform operation, and transfer the new 
+data to selected position.
+
+
+```python
+import numpy as np
+from image_fragment.fragment import ImageFragment
+
+image = np.zeros((1, 1024, 1024, 3))
+new_image = np.zeros((1, 1024, 1024, 3))
+image_fragment = ImageFragment.image_fragment_4d(fragment_size=(1, 512, 512, 3), org_size=(1, 1024, 1024, 3))
+for fragment in image_fragment:
+    # GET DATA THAT BELONGS TO THE FRAGMENT
+    fragmented_image = fragment.get_fragment_data(image)
+    
+    # DO SOME OPERATION ON THE FRAGMENTED DATA
+    operation_done_on_fragmented_data = np.rot(fragmented_image)
+    
+    # TRANSFER OPERATED IMAGE ON NEW IMAGE ON THE FRAGMENT POSITION
+    new_image = fragment.transfer_fragment(transfer_from=operation_done_on_fragmented_data, transfer_to=new_image)
+    
+```
+
+If image is 3 Dimensional then switch to `image_fragment = ImageFragment.image_fragment_3d(fragment_size=(512, 512, 3), org_size=(1024, 1024, 3))`, 
+this will provide fragments for 3 dimensional image
```

### Comparing `image_fragment-0.2.2/README.md` & `image_fragment-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,62 @@
-# Fragment
-![GitHub](https://img.shields.io/github/license/fuzailpalnak/fragment)
-![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
-![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
-
-Any extent is a set of smaller fragment extent , which can be as small as *1 x 1* to the *size* of the extent given.
-This library will section the given extent in to specified smaller fragment extent
-
-
-## Installation
-
-    pip install image-fragment
-
-
-## Image Fragments
-
-![fragments](https://user-images.githubusercontent.com/24665570/91711219-2b7c8980-eba3-11ea-94d2-8239cf6713c4.gif)
-
-An image extent can be sectioned into many fragments, these fragments holds positional information to where it is located 
-to the original extent
-
-Now this information can be used to extract selected fragments from the Image, perform operation, and transfer the new 
-data to selected position.
-
-
-```python
-import numpy as np
-from image_fragment.fragment import ImageFragment
-
-image = np.zeros((1, 1024, 1024, 3))
-new_image = np.zeros((1, 1024, 1024, 3))
-image_fragment = ImageFragment.image_fragment_4d(fragment_size=(1, 512, 512, 3), org_size=(1, 1024, 1024, 3))
-for fragment in image_fragment:
-    # GET DATA THAT BELONGS TO THE FRAGMENT
-    fragmented_image = fragment.get_fragment_data(image)
-    
-    # DO SOME OPERATION ON THE FRAGMENTED DATA
-    operation_done_on_fragmented_data = np.rot(fragmented_image)
-    
-    # TRANSFER OPERATED IMAGE ON NEW IMAGE ON THE FRAGMENT POSITION
-    new_image = fragment.transfer_fragment(transfer_from=operation_done_on_fragmented_data, transfer_to=new_image)
-    
-```
-
-If image is 3 Dimensional then switch to `image_fragment = ImageFragment.image_fragment_3d(fragment_size=(512, 512, 3), org_size=(1024, 1024, 3))`, 
-this will provide fragments for 3 dimensional image
+Metadata-Version: 2.1
+Name: image_fragment
+Version: 0.2.3
+Summary: Data Section
+Home-page: https://github.com/fuzailpalnak/fragment
+Author: Fuzail Palnak
+Author-email: fuzailpalnak@gmail.com
+Keywords: numpy, Window, Section, Array, Stitch, Split
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: ~=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Fragment
+![GitHub](https://img.shields.io/github/license/fuzailpalnak/fragment)
+![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
+![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)
+![Downloads](https://pepy.tech/badge/image-fragment)
+
+Any extent is a set of smaller fragment extent , which can be as small as *1 x 1* to the *size* of the extent given.
+This library will section the given extent in to specified smaller fragment extent
+
+
+## Installation
+
+    pip install image-fragment
+
+
+## Image Fragments
+
+![fragments](https://user-images.githubusercontent.com/24665570/91711219-2b7c8980-eba3-11ea-94d2-8239cf6713c4.gif)
+
+An image extent can be sectioned into many fragments, these fragments holds positional information to where it is located 
+to the original extent
+
+Now this information can be used to extract selected fragments from the Image, perform operation, and transfer the new 
+data to selected position.
+
+
+```python
+import numpy as np
+from image_fragment.fragment import ImageFragment
+
+image = np.zeros((1, 1024, 1024, 3))
+new_image = np.zeros((1, 1024, 1024, 3))
+image_fragment = ImageFragment.image_fragment_4d(fragment_size=(1, 512, 512, 3), org_size=(1, 1024, 1024, 3))
+for fragment in image_fragment:
+    # GET DATA THAT BELONGS TO THE FRAGMENT
+    fragmented_image = fragment.get_fragment_data(image)
+    
+    # DO SOME OPERATION ON THE FRAGMENTED DATA
+    operation_done_on_fragmented_data = np.rot(fragmented_image)
+    
+    # TRANSFER OPERATED IMAGE ON NEW IMAGE ON THE FRAGMENT POSITION
+    new_image = fragment.transfer_fragment(transfer_from=operation_done_on_fragmented_data, transfer_to=new_image)
+    
+```
+
+If image is 3 Dimensional then switch to `image_fragment = ImageFragment.image_fragment_3d(fragment_size=(512, 512, 3), org_size=(1024, 1024, 3))`, 
+this will provide fragments for 3 dimensional image
```

### Comparing `image_fragment-0.2.2/image_fragment/fragment.py` & `image_fragment-0.2.3/image_fragment/fragment.py`

 * *Files identical despite different names*

### Comparing `image_fragment-0.2.2/setup.py` & `image_fragment-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 install_requires = [
-    "numpy == 1.19.1",
+    "numpy >= 1.19.1",
 ]
 
 setup(
     name="image_fragment",
-    version="0.2.2",
+    version="0.2.3",
     author="Fuzail Palnak",
     author_email="fuzailpalnak@gmail.com",
     url="https://github.com/fuzailpalnak/fragment",
     description="Data Section",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

