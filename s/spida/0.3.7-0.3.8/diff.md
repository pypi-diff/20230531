# Comparing `tmp/spida-0.3.7.tar.gz` & `tmp/spida-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.3.7.tar", last modified: Wed May 31 20:12:34 2023, max compression
+gzip compressed data, was "spida-0.3.8.tar", last modified: Wed May 31 20:54:22 2023, max compression
```

## Comparing `spida-0.3.7.tar` & `spida-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 20:12:34.421445 spida-0.3.7/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.3.7/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6148 2023-05-31 20:12:34.420431 spida-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.3.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 20:12:34.421445 spida-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-31 20:11:33.000000 spida-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:12:34.373299 spida-0.3.7/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.3.7/spida/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:12:34.410936 spida-0.3.7/spida/data/
--rw-rw-rw-   0        0        0        2 2023-05-31 02:38:32.000000 spida-0.3.7/spida/data/config.json
--rw-rw-rw-   0        0        0    18541 2023-05-31 02:36:49.000000 spida-0.3.7/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:12:34.418355 spida-0.3.7/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.3.7/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5949 2023-05-31 20:09:12.000000 spida-0.3.7/spida/utils/img.py
--rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.3.7/spida/utils/misc.py
--rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.3.7/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-31 20:12:34.408911 spida-0.3.7/spida.egg-info/
--rw-rw-rw-   0        0        0     6148 2023-05-31 20:12:34.000000 spida-0.3.7/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-31 20:12:34.000000 spida-0.3.7/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 20:12:34.000000 spida-0.3.7/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-31 20:12:34.000000 spida-0.3.7/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-31 20:12:34.000000 spida-0.3.7/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.833371 spida-0.3.8/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6148 2023-05-31 20:54:22.832350 spida-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.3.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 20:54:22.834381 spida-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-05-31 20:53:06.000000 spida-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.790923 spida-0.3.8/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.3.8/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.823669 spida-0.3.8/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-31 02:38:32.000000 spida-0.3.8/spida/data/config.json
+-rw-rw-rw-   0        0        0    18541 2023-05-31 02:36:49.000000 spida-0.3.8/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.831337 spida-0.3.8/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.3.8/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     5970 2023-05-31 20:52:48.000000 spida-0.3.8/spida/utils/img.py
+-rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.3.8/spida/utils/misc.py
+-rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.3.8/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:54:22.821575 spida-0.3.8/spida.egg-info/
+-rw-rw-rw-   0        0        0     6148 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 20:54:22.000000 spida-0.3.8/spida.egg-info/top_level.txt
```

### Comparing `spida-0.3.7/LICENSE` & `spida-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.3.7/PKG-INFO` & `spida-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `spida-0.3.7/README.md` & `spida-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `spida-0.3.7/setup.py` & `spida-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.3.7",
+    version="0.3.8",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
```

### Comparing `spida-0.3.7/spida/stable_diffusion.py` & `spida-0.3.8/spida/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.7/spida/utils/img.py` & `spida-0.3.8/spida/utils/img.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     vmin, vmax : scalar, optional
         When using scalar data and no explicit norm, vmin and vmax define the data range that the colormap covers. Default is None.
     """
     if use_matplot:
         plt.imshow(img, cmap, vmin=vmin, vmax=vmax)
         plt.show()
     else:
-        Image.fromarray(img, mode="RGB").show()
+        Image.fromarray(np.uint8(img)).show()
 
 
 def save(img: np.ndarray, file_name: str = None):
     """
     Save the image to a file. If no filename is given, it will generate one.
 
     Parameters
@@ -53,15 +53,15 @@
         png_files = glob.glob("img_*.png")
         if png_files:
             nums = [int(i[4:-4]) for i in png_files]
             fnum = max(nums) + 1
             file_name = f"img_{fnum}.png"
         else:
             file_name = "img_0.png"
-    Image.fromarray(img, mode="RGB").save(file_name)
+    Image.fromarray(np.uint8(img)).save(file_name)
 
 
 def open(path: str = None):
     """
     Open an image file and return the image array.
 
     Parameters
@@ -72,15 +72,15 @@
     Returns
     -------
     numpy.ndarray
         The image array.
     """
     if path is None:
         path = filedialog.askopenfilename()
-    return plt.imread(path)
+    return np.asarray(Image.open(path).convert("RGB"))
 
 
 def grid_img(imgs: np.ndarray, grid_shape: tuple = None, fill_value: int = 255):
     """
     Creates a grid of images from a provided set of images.
 
     Parameters
@@ -140,15 +140,15 @@
 
     Returns
     -------
     str
         The base64 string of the image.
     """
     with io.BytesIO() as output_bytes:
-        Image.fromarray(img, mode="RGB").save(output_bytes, format="PNG")
+        Image.fromarray(np.uint8(img)).save(output_bytes, format="PNG")
         bytes_data = output_bytes.getvalue()
     return base64.b64encode(bytes_data).decode(encoding="utf-8")
 
 
 def imgs2b64strs(imgs: np.ndarray):
     """
     Convert multiple image arrays to a list of base64 strings.
```

### Comparing `spida-0.3.7/spida/utils/misc.py` & `spida-0.3.8/spida/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.7/spida/utils/net.py` & `spida-0.3.8/spida/utils/net.py`

 * *Files identical despite different names*

### Comparing `spida-0.3.7/spida.egg-info/PKG-INFO` & `spida-0.3.8/spida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

