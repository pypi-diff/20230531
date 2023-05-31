# Comparing `tmp/lavlab-python-utils-1.0.1.tar.gz` & `tmp/lavlab-python-utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.0.1.tar", last modified: Fri May 26 16:05:19 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.0.2.tar", last modified: Wed May 31 19:36:31 2023, max compression
```

## Comparing `lavlab-python-utils-1.0.1.tar` & `lavlab-python-utils-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/src/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/src/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/src/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    19120 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/src/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/src/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:36:31.481476 lavlab-python-utils-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 19:36:31.481476 lavlab-python-utils-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:36:31.477476 lavlab-python-utils-1.0.2/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26962 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:36:31.481476 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:36:31.000000 lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-31 19:36:20.000000 lavlab-python-utils-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:36:31.481476 lavlab-python-utils-1.0.2/setup.cfg
```

### Comparing `lavlab-python-utils-1.0.1/PKG-INFO` & `lavlab-python-utils-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+
+TODO: this readme
+=================
+for more info goto: https://lavlab-python-utils.readthedocs.io/en/latest/
```

### Comparing `lavlab-python-utils-1.0.1/pyproject.toml` & `lavlab-python-utils-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 [project]
 name = "lavlab-python-utils"
-version = "1.0.1"
+description = "LaViolette Lab utility package"
+version = "1.0.2"
+
 authors = [
   { name="Michael Barrett", email="mjbarrett@mcw.edu" },
 ]
-description = "LaViolette Lab utility package"
-readme = "README.md"
-requires-python = ">=3.7"
+
+readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+
+requires-python = ">=3.6"
 dependencies = [
   'omero-py >= 5.13.1',
   'omero-scripts >= 5.7.1',
   'scikit-image >= 0.19.3'
 ]
+
+[project.optional-dependencies]
+docs = ["sphinx>=6.2.1","docutils >= 0.18.1"]
+
 [project.urls]
 "Homepage" = "https://github.com/laviolette-lab/lavlab-python-utils"
 "Bug Tracker" = "https://github.com/laviolette-lab/lavlab-python-utils/issues"
+
+[build-system]
+requires = ["setuptools", "wheel"]
```

### Comparing `lavlab-python-utils-1.0.1/src/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.0.2/lavlab/omero_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+"""This module can be tricky to work with and requires decent python experience. Primarily a dependency for omero_util"""
 # written by manics https://github.com/microscopepony/omero-asyncio/commits?author=manics
 import asyncio
 from functools import partial, update_wrapper
 import logging
 import Ice
 import omero.clients
```

### Comparing `lavlab-python-utils-1.0.1/src/lavlab/omero_util.py` & `lavlab-python-utils-1.0.2/lavlab/omero_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,131 @@
 """
 Helper functions that handle high-level operations and translating asynchronous requests for easy development.
 """
 import os
 import asyncio
-from collections.abc import AsyncGenerator
+import tempfile
 
 import numpy as np
 from skimage import draw
-from PIL import Image
-from omero.gateway import _BlitzGateway, ImageWrapper, FileAnnotationWrapper
+
+from collections.abc import AsyncGenerator
+
+from omero.gateway import _BlitzGateway, ImageWrapper, FileAnnotationWrapper, ShapeWrapper
+import omero.model.enums as omero_enums
+from omero.rtypes import rint, rstring
+
+from omero_model_RoiI import RoiI
+from omero_model_PolygonI import PolygonI
 from omero_model_EllipseI import EllipseI
 from omero_model_PolygonI import PolygonI
 from omero_model_RectangleI import RectangleI
 from omero_model_FileAnnotationI import FileAnnotationI
-import omero.model.enums as omero_enums
 
 from lavlab import omero_asyncio
-from lavlab.python_util import chunkify, merge_async_iters, interlaceLists, lookup_filetype_by_name, FILETYPE_DICTIONARY
+from lavlab.python_util import chunkify, merge_async_iters, interlace_lists, lookup_filetype_by_name, FILETYPE_DICTIONARY, save_image_binary, rgba_to_int, resize_image_array
 
 PARALLEL_STORE_COUNT=4
-"""Number of pixel stores to be created for an image"""
+"""Number of pixel stores to be created for an image."""
 
 OMERO_DICTIONARY = {
     # TODO add real pixeltype support
     "PIXEL_TYPES": {
         omero_enums.PixelsTypeint8: np.int8,
         omero_enums.PixelsTypeuint8: np.uint8,
         omero_enums.PixelsTypeint16: np.int16,
         omero_enums.PixelsTypeuint16: np.uint16,
         omero_enums.PixelsTypeint32: np.int32,
         omero_enums.PixelsTypeuint32: np.uint32,
         omero_enums.PixelsTypefloat: np.float32,
         omero_enums.PixelsTypedouble: np.float64,
     },
     "BYTE_MASKS": {
-        "UINT_8": {
+        np.uint8: {
             "RED": 0xFF000000, 
             "GREEN": 0xFF0000, 
             "BLUE": 0xFF00,  
             "ALPHA": 0xFF
         }
     },
     "SKIMAGE_FORMATS": FILETYPE_DICTIONARY["SKIMAGE_FORMATS"]
 }
 """
-Dictionary for dealing with omero/pixel datatypes.\n
-PIXEL_TYPES: { omero.PixelType: numpy.datatype }\n
-BYTE_MASKS: { "UINT_8": { "RED": 0x... } }\n
-SKIMAGE_FORMATS: alias FILETYPE_DICTIONARY["SKIMAGE_FORMATS"]
+Dictionary for converting omero info into python equivalents.
+
+```
+OMERO_DICTIONARY = {
+"PIXEL_TYPES": {
+    omero_enums.PixelsTypeint8: np.int8,
+    omero_enums.PixelsTypeuint8: np.uint8,
+    omero_enums.PixelsTypeint16: np.int16,
+    omero_enums.PixelsTypeuint16: np.uint16,
+    omero_enums.PixelsTypeint32: np.int32,
+    omero_enums.PixelsTypeuint32: np.uint32,
+    omero_enums.PixelsTypefloat: np.float32,
+    omero_enums.PixelsTypedouble: np.float64,
+},
+"BYTE_MASKS": {
+    np.uint8: {
+        "RED": 0xFF000000, 
+        "GREEN": 0xFF0000, 
+        "BLUE": 0xFF00,  
+        "ALPHA": 0xFF
+    }
+},
+"SKIMAGE_FORMATS": FILETYPE_DICTIONARY["SKIMAGE_FORMATS"]
+}
+```
+
+See Also
+--------
+lavlab.python_utils.FILETYPE_DICTIONARY : Contains file extensions and mimetypes for commonly used files.
 """
 
 
 #
 ## IMAGE DATA
 #
 def getTiles(img: ImageWrapper, tiles: list[tuple[int,int,int,tuple[int,int,int,int]]],
             resLvl: int=None, rps_bypass=True) -> AsyncGenerator[tuple[np.ndarray,tuple[int,int,int,tuple[int,int,int,int]]]]:
     """
-Asynchronous tile generator. Creates and destroys parallel RawPixelsStores to request tiles.\n
-img: omero.gateway.ImageWrapper\n
-tiles: list of tiles (z,c,t,(x,y,w,h))\n
-resLvl: what resolution level are these tiles on, default highest res\n
-rps_bypass: alias for rawPixelsStore.setPixelsId(pixels.id, rps_bypass)\n
-returns: async generator. \n
-usage: async for nparray, zctxywh in getTiles(img, [zctxywh,...]):
+Asynchronous tile generator. 
+
+Creates and destroys parallel asynchronous RawPixelsStores to await multiple tiles at once.
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects().
+tiles: list[ (z,c,t,(x,y,w,h) ]), ... ]
+    list of tiles to gather.
+resLvl: default: -1
+    what resolution level are these tiles on, default highest res
+rps_bypass: default: True
+    passthrough for rawPixelsStore.setPixelsId(pixels.id, rps_bypass)
+
+Returns
+-------
+Async tile generator
+    python async generator that yields omero tiles as numpy arrays
+
+Examples
+--------
+```
+import asyncio
+async def work(img, tiles, res_lvl, dims):
+    bin = np.zeros(dims, np.uint8)
+    async for tile, (z,c,t,coord) in getTiles(img,tiles,res_lvl):
+        bin [
+            coord[1]:coord[1]+coord[3],
+            coord[0]:coord[0]+coord[2], 
+            c ] = tile 
+    return bin
+asyncio.run(work(img, tiles, res_lvl, dims))
+```
 """
     # tile request group
     async def work(id, tiles, resLvl):
         # create and init rps for this group
         rps = await session.createRawPixelsStore()
         await rps.setPixelsId(id,rps_bypass)
 
@@ -92,31 +150,80 @@
 
     # create parallel raw pixels stores
     jobs=[]
     for chunk in chunkify(tiles, int(len(tiles)/PARALLEL_STORE_COUNT)+1):
         jobs.append(work(img.getPrimaryPixels().getId(), chunk, resLvl))
     return merge_async_iters(*jobs)
 
-def getDownsampledYXDimensions(img: ImageWrapper, downsample_factor: int):
-    """Returns img yx dimensions after being divided by downsample factor"""
+def getDownsampledYXDimensions(img: ImageWrapper, downsample_factor: int) -> tuple[int,int]:
+    """
+Returns yx (rows,columns) dimensions of given image at the downsample.
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects().
+downsample_factor: int
+    Takes every nth pixel from the base resolution.
+
+Returns
+-------
+int
+    img.getSizeY() / downsample_factor
+int 
+    img.getSizeX() / downsample_factor
+"""
     return (int(img.getSizeY() / downsample_factor),
             int(img.getSizeX() / downsample_factor))
 
 def getDownsampleFromDimensions(base_shape:tuple[int,...], sample_shape:tuple[int,...]) -> tuple[float,...]:
-    """Essentially an alias for np.divide()"""
+    """
+Essentially an alias for np.divide().
+
+Finds the ratio between a base array shape and a sample array shape by dividing each axis.
+
+Parameters
+----------
+base_shape: tuple(int)*x
+    Shape of the larger image. (base_nparray.shape)
+sample_shape: tuple(int)*x
+    Shape of the smaller image. (sample_nparray.shape)
+
+Raises
+------
+AssertionError
+    Asserts that the input shapes have the same amount of axes
+
+Returns
+-------
+tuple(int)*x
+    Returns a tuple containing the downsample factor of each axis for the sample array.
+
+""" 
     assert len(base_shape) == len(sample_shape)
     return np.divide(base_shape, sample_shape)
 
 
-def getClosestResolutionLevel(img: ImageWrapper, dim: tuple[int,int]
-                              ) -> tuple[int,tuple[int,int,int,int]]:
+def getClosestResolutionLevel(img: ImageWrapper, dim: tuple[int,int]) -> tuple[int,tuple[int,int,int,int]]:
     """
-Finds the closest resolution to desired resolution.\n
-Returns resolution level to be used in store.setResolution() and actual y,x dimensions of that resolution.\n
-return value schema: ( level, (width,height,x_tile_size,y_tile_size) )
+Finds the closest resolution to desired resolution.
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper or RawPixelsStore
+    Omero Image object from conn.getObjects() or initialized rps
+dim: tuple[int, int]
+    tuple containing desired y,x dimensions. 
+
+Returns
+-------
+int
+    resolution level to be used in rps.setResolution() 
+tuple[int,int,int,int]
+    height, width, tilesize_y, tilesize_x of closest resolution
     """
     # if has getResolutionLevels method it's a rawpixelstore
     if type(img) is hasattr(img, 'getResolutionLevels'): rps = img
     # else assume it's an ImageWrapper obj and use it to create an rps
     else:
         rps = img._conn.createRawPixelsStore()
         rps.setPixelsId(img.getPrimaryPixels().getId(), True)
@@ -137,44 +244,47 @@
             tileSize=rps.getTileSize()
 
             if close_rps is True: rps.close()
 
             return (lvls-i, (resolutions[i-1].sizeY,resolutions[i-1].sizeX,
                              tileSize[1], tileSize[0]))
         
-# https://docs.scipy.org/doc/scipy-1.2.1/reference/generated/scipy.misc.imresize.html
-def resizeImage(input_array: np.ndarray, shape_xy: tuple[int,int], interpolation=Image.NEAREST):
-    """
-Resizes input image array to desired xy dimensions using PIL.Image.resize.\n
-input_array: 2-3(+?) dimensional numpy array.\n
-shape_xy: desired width and height of output.\n
-interpolation: default nearest neighbor, PIL.Image.INTERPOLATION_TYPE\n
-Returns: smaller np.ndarray
-    """
-    return np.asarray(Image.fromarray(input_array).
-                      resize(shape_xy, interpolation), input_array.dtype)
 
 def getImageAtResolution(img: ImageWrapper, yx_dim: tuple[int,int], channels:list[int]=None) -> np.ndarray:
     """
-Gathers tiles and scales down to desired resolution.\n
-Out of Memory issues ahead! Request a reasonable resolution!\n
-img: ImageWrapper\n
-yx_dim: tuple of desired dimensions (row, col)\n
-channels: array of channels to gather, to grab only blue channel: channels=(2) default: all channels\n
-returns: np array of color values for given img
+Gathers tiles and scales down to desired resolution.
+
+Warns
+-------
+Out of Memory issues ahead! Request a reasonable resolution!
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects().
+yx_dim: tuple(y,x)
+    Tuple of desired dimensions (row, col)
+channels: tuple(int,...), default: all channels
+    Array of channels to gather.
+    To grab only blue channel: channels=(2) 
+
+Returns
+-------
+np.ndarray 
+    Array of rbg values for given img.
     """
     async def work(img, tiles, res_lvl, current_dims, des_shape):
         bin = np.zeros(current_dims, np.uint8)
         async for tile, (z,c,t,coord) in getTiles(img,tiles,res_lvl):
             bin [
                 coord[1]:coord[1]+coord[3],
                 coord[0]:coord[0]+coord[2], 
                 c ] = tile 
         if bin.shape != des_shape:
-            bin = resizeImage(bin,(yx_dim[1],yx_dim[0]))
+            bin = resize_image_array(bin,(yx_dim[1],yx_dim[0]))
         return bin
     
     res_lvl, dims = getClosestResolutionLevel(img, yx_dim)
 
     if channels is None:
         channels = range(img.getSizeC())
     
@@ -184,34 +294,99 @@
     else: 
         des_shape = yx_dim
         current_dims = dims[:1]
         
     tiles = createFullTileList([0,],channels,[0,],dims[1],dims[0],(dims[3],dims[2]))
     return asyncio.run(work(img, tiles, res_lvl, current_dims, des_shape))
 
-def applyMask(img_bin: np.ndarray, mask_bin: np.ndarray, where=None):
-    """Essentially an alias for np.where()"""
-    if where is None:
-        where=mask_bin!=0
-    return np.where(where, mask_bin, img_bin)
+
+def getLargeRecon(img:ImageWrapper, downsample_factor, workdir='./', save_format="JPEG"):
+    """
+Checks OMERO for a pregenerated large recon, if none are found, it will generate and upload one.
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects().
+downsample_factor: int
+    Which large recon size to get.
+
+Returns
+-------
+omero.gateway.AnnotationWrapper
+    remote large recon object
+str
+    local path to large recon
+    """
+    NS = "LargeRecon."+str(downsample_factor)
+    EXT, MIME = OMERO_DICTIONARY["SKIMAGE_FORMATS"][save_format]
+    recon = img.getAnnotation(NS)
+    if recon is None:
+        name = img.getName()
+        sizeX = img.getSizeX()
+        sizeY = img.getSizeY()
+
+        print(f"No large recon {downsample_factor} for img: {name} Generating...")
+
+        yx_dim=getDownsampledYXDimensions(img, downsample_factor)
+        reconPath = workdir + os.sep + f"LR{downsample_factor}_{name.replace('.ome.tiff',EXT)}"
+        recon = img.getAnnotation(NS)
+        
+        if recon is None: 
+                print(f"Downsampling: {name} from {(sizeY,sizeX)} to {yx_dim}")
+                reconBin = getImageAtResolution(img, yx_dim)
+                
+                if save_format == 'JPEG': 
+                    jpeg=True 
+                else: 
+                    jpeg=False
+
+                save_image_binary(reconPath,reconBin, jpeg)
+                
+                print("Downsampling Complete! Uploading to OMERO...")
+                recon = img._conn.createFileAnnfromLocalFile(reconPath, mimetype=MIME, ns=NS)
+                img.linkAnnotation(recon)
+        else:
+            reconPath = downloadFileAnnotation(recon, workdir)
+
+    return recon, reconPath
 
 #
 ## TILES
 #
-def createTileList2D(z:int, c:int, t:int, size_x:int, size_y:int, 
+def createTileList2D(z:int, c:int, t:int, size_x:int, size_y:int,
         tile_size:tuple[int,int]) -> list[tuple[int,int,int,tuple[int,int,int,int]]]:
     """
-Creates a list of tile coords for a given plane (z,c,t)\n
-z: z index\n
-c: channel\n
-t: timepoint\n
-size_x: width of full image\n
-size_y: height of full image\n
-tile_size: tuple(desired_tile_width, desired_tile_height)\n
-Return: [(z,c,t(0,0,tile_size[0],tile_size[1])), ...]
+Creates a list of tile coords for a given 2D plane (z,c,t)
+
+Notes
+-----
+Tiles are outputed as (z,c,t,(x,y,w,h)) as this is the expected format by omero python bindings.\n
+This may cause confusion as numpy uses rows,cols (y,x) instead of x,y. \n
+Tile lists generated by lavlab.omero_utils are compatible with omero_util and official omero functions.
+
+Parameters
+----------
+z: int
+    z index
+c: int
+    channel
+t: int
+    timepoint
+size_x: int
+    width of full image in pixels
+size_y: int
+    height of full image in pixels
+tile_size: tuple(int, int)
+    size of tile to gather (x,y)
+
+Returns
+-------
+list 
+    list of (z,c,t,(x,y,w,h)) tiles for use in getTiles 
     """ 
     tileList = []
     width, height = tile_size 
     for y in range(0, size_y, height):
         width, height = tile_size # reset tile size
         # if tileheight is greater than remaining pixels, get remaining pixels
         if size_y-y < height: height = size_y-y
@@ -221,56 +396,94 @@
             tileList.append((z,c,t,(x,y,width,height)))
     return tileList
 
 
 def createFullTileList(z_indexes: int, channels: int, timepoints: int, width: int, height:int, 
         tile_size:tuple[int,int], weave=False) -> list[tuple[int,int,int,tuple[int,int,int,int]]]:
     """
-Creates a list of all tiles for given dimensions.\n
-size_z: z index\n
-size_c: channel\n
-size_t: timepoint\n
-size_x: width of full image\n
-size_y: height of full image\n
-tile_size: tuple(desired_tile_width, desired_tile_height)\n
-rgb: Interlace tiles from each channel vs default seperate channels.\n
-    Default: False. \n
-    Example False: [0,0,0,tile],[0,0,0,tile2],...[0,1,0,tile],...\n
-    Example True: [0,0,0,tile],[0,1,0,tile],[0,2,0,tile]... \n
-Return: [(z,c,t(0,0,tile_size[0],tile_size[1])), ...]
-    """
+Creates a list of all tiles for given dimensions.
+
+Parameters
+----------
+z_indexes: list[int]
+    list containing z_indexes to gather
+channels: list[int]
+    list containing channels to gather
+timepoints: list[int]
+    list containing timepoints to gather
+width: int
+    width of full image in pixels
+height: int
+    height of full image in pixels
+tile_size: tuple(int, int)
+weave: bool, Default: False
+    Interlace tiles from each channel vs default seperate channels.
+
+Returns
+-------
+list 
+    list of (z,c,t,(x,y,w,h)) tiles for use in getTiles 
+    
 
+Examples
+--------
+```
+>>> createFullTileList((0),(0,2),(0),1000,1000,10,10)
+list[
+(0,0,0,(0,0,10,10)), (0,0,0,(10,0,10,10))...
+(0,2,0,(0,0,10,10)), (0,2,0,(10,0,10,10))...
+]
+
+Default will gather each channel separately.
+
+>>> createFullTileList((0),(0,2),(0),1000,1000,10,10, weave=True)
+list[
+(0,0,0,(0,0,10,10)), (0,2,0,(0,0,10,10)),
+(0,0,0,(10,0,10,10)), (0,2,0,(10,0,10,10))...
+]
+
+Setting weave True will mix the channels together. Used  for writing RGB images
+```
+"""
     tileList = []
     if weave is True: 
         origC = channels
         channels = (0)
     for z in z_indexes:
         for c in channels:
             for t in timepoints:
                 if weave is True:
                     tileChannels = []
                     for channel in origC:
                         tileChannels.append(createTileList2D(z,channel,t,width, height, tile_size)) 
-                    tileList.extend(interlaceLists(tileChannels))
+                    tileList.extend(interlace_lists(tileChannels))
                 else:
                     tileList.extend(createTileList2D(z,c,t,width, height, tile_size))
         
     return tileList
 
 def createTileListFromImage(img: ImageWrapper, rgb=False, include_z=True, include_t=True) -> list[int,int,int,tuple[int,int,int,int]]:
     """
-Generates a list of tiles from an omero:model:Image object.
-img: omero.model.ImageWrapper
-rgb: Puts tile channels next to each other.
-    Default: False.\n
-    Example False: [0,0,0,tile],[0,0,0,tile2],...[0,1,0,tile],...\n
-    Example True: [0,0,0,tile],[0,1,0,tile],[0,2,0,tile]... \n
-include_z: get tiles for z indexes\n
-include_t: get tiles for timepoints\n
-returns: [(z,c,t(0,0,tile_size[0],tile_size[1])), ...]
+Generates a list of tiles from an omero.model.Image object.
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects().
+rgb: bool, Default: False.
+    Puts tile channels next to each other. 
+include_z: bool, Default: True
+    get tiles for z indexes
+include_t: bool, Default: True
+    get tiles for timepoints
+
+Returns
+-------
+list 
+    List of (z,c,t,(x,y,w,h)) tiles for use in getTiles.
     """
     width = range(img.getSizeX()) 
     height = range(img.getSizeY())
     z_indexes = range(img.getSizeZ())
     timepoints = range(img.getSizeT())
     channels = range(img.getSizeC())
 
@@ -286,20 +499,31 @@
 
 #
 ## ROIS
 #
 def getShapesAsPoints(img: ImageWrapper, point_downsample=4, img_downsample=1, 
                       roi_service=None) -> list[tuple[int, tuple[int,int,int], tuple[np.ndarray, np.ndarray]]]:
     """
-Gathers Rectangles, Polygons, and Ellipses as a tuple containing the shapeId, its rgb val, and a tuple of yx points of its bounds.\n
-img: ImageWrapper\n
-point_downsample: grab every nth point, default: 4\n
-img_downsample: how much to scale roi points\n
-roi_service: allows roiservice passthrough for performance\n
-returns: [(shape.id, (r,g,b), (row_points, column_points)),...]
+Gathers Rectangles, Polygons, and Ellipses as a tuple containing the shapeId, its rgb val, and a tuple of yx points of its bounds.
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects().
+point_downsample: int, Default: 4
+    Grabs every nth point for faster computation.
+img_downsample: int, Default: 1
+    How much to scale roi points.
+roi_service: omero.RoiService, optional
+    Allows roiservice passthrough for performance.
+
+Returns
+-------
+returns: list[shape.id, (r,g,b), (row_points, column_points))]
+    list of tuples containing a shape's id, rgb value, and a tuple of row and column points
     """
     if roi_service is None:
         roi_service=img._conn.getRoiService()
         close_roi=True
 
     sizeX = img.getSizeX() / img_downsample
     sizeY = img.getSizeY() / img_downsample
@@ -333,15 +557,15 @@
                     y.append(float(coordList[1]) / img_downsample)
                     x.append(float(coordList[0]) / img_downsample)
 
                 points = draw.polygon_perimeter(y, x, shape=yx_shape)
 
             if points is not None:
                 color_val = shape.getStrokeColor()._val
-                masks = OMERO_DICTIONARY["BYTE_MASKS"]["UINT_8"]
+                masks = OMERO_DICTIONARY["BYTE_MASKS"][np.uint8]
                 red = (color_val & masks["RED"]) >> 24  
                 green = (color_val & masks["GREEN"]) >> 16  
                 blue = (color_val & masks["BLUE"]) >> 8 
                 points=(points[0][::point_downsample], points[1][::point_downsample])
                 
                 shapes.append((shape.getId()._val, (red,green,blue), points))
 
@@ -349,30 +573,120 @@
         return None
     
     if close_roi: roi_service.close()
 
     # make sure is in correct order
     return sorted(shapes)
 
-def drawShapes(input_img, shape_points):
-    """
-Draws a list of shape points (from getShapesAsPoints) onto a given numpy array.\n
-NO SAFETY CHECKS! MAKE SURE input_img AND shape_points ARE FOR THE SAME DOWNSAMPLE FACTOR!\n
-input_img: 3 channel numpy array\n
-shape_points: [(shape.id, (r,g,b), (row_points, column_points)),...]
+
+def createPolygon(contour:tuple[np.ndarray, np.ndarray], x_offset=0, y_offset=0, z=None, t=None, comment=None, rgb=(0,0,0)) -> PolygonI:
+    """ 
+Creates a local omero polygon obj from a list of points, and parameters.
+    
+Parameters
+----------
+contour: tuple[rows, cols]
+    Expects contour as outputed by skimage.measure.find_contours
+x_offset: int, Default: 0
+    Inherited from where I ripped this code. Lets you shift coords I guess.
+y_offset: int, Default: 0
+    Inherited from where I ripped this code. Lets you shift coords I guess.
+z: int, optional
+    Allows polygon to exist in a specific z_index for multi dimensional ROIs.
+t: int, optional
+    Allows polygon to exist in a specific timepoint for multi dimensional ROIs.
+comment: str, optional
+    Description of polygon, recommended to use to keep track of which programs generate which shapes.
+rgb: tuple[int,int,int], Default: (0,0,0) 
+    What color contour should this polygon's contour be.
+    
+Returns
+-------
+omero_model_PolygonI.PolygonI
+    Local Omero Polygon object, likely needs to linked to an ROI
+    """
+    stride = 64
+    coords = []
+    # points in contour are adjacent pixels, which is too verbose
+    # take every nth point
+    for count, xy in enumerate(contour):
+        if count%stride == 0:
+            coords.append(xy)
+    if len(coords) < 2:
+        return
+    points = ["%s,%s" % (xy[1] + x_offset, xy[0] + y_offset) for xy in coords]
+    points = ", ".join(points)
+    polygon = PolygonI()
+    if z is not None:
+        polygon.theZ = rint(z)
+    if t is not None:
+        polygon.theT = rint(t)
+    if comment is not None:
+        polygon.setTextValue(rstring(comment))
+    polygon.strokeColor = rint(rgba_to_int(*rgb))
+    polygon.points = rstring(points)
+    return polygon
+
+def createRoi(img: ImageWrapper, shapes: list[ShapeWrapper]):
+    """
+Creates an omero RoiI object for an image from an array of shapes.
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects().
+shapes: list[omero_model_ShapeI.ShapeI]
+    List of omero shape objects (Polygon, Rectangle, etc).
+
+Returns
+omero_model_RoiI.RoiI
+    Local Omero ROI object, needs to be saved
+-------
+
+    """
+    # create an ROI, link it to Image
+    roi = RoiI()
+    # use the omero.model.ImageI that underlies the 'image' wrapper
+    roi.setImage(img._obj)
+    for shape in shapes:
+        roi.addShape(shape)
+    return roi
+
+
+def drawShapes(input_img: np.ndarray, shape_points:tuple[int,tuple[int,int,int],tuple[np.ndarray, np.ndarray]]) -> None:
+    """
+Draws a list of shape points onto the input numpy array.
+
+Warns
+-------
+NO SAFETY CHECKS! MAKE SURE input_img AND shape_points ARE FOR THE SAME DOWNSAMPLE FACTOR!
+
+Parameters
+----------
+input_img: np.ndarray
+    3 channel numpy array
+shape_points: tuple(int, tuple(int,int,int), tuple(row, col))
+    output from getShapesAsPoints
+
+Returns
+-------
+``None``
     """
     for id, rgb, points in shape_points:
         rr,cc = draw.polygon(*points)
         input_img[rr,cc]=rgb
 
+
+
+
 # TODO SLOW AND broken for rgb = 0,0,0 annotations
 # def getShapesAsMasks(img: ImageWrapper, downsample: int, bool_mask=True, 
 #                      point_downsample=4, roi_service=None) -> list[np.ndarray]:
 #     """
-# Gathers Rectangles, Polygons, and Ellipses as masks for the image at the given downsampling\n
+# Gathers Rectangles, Polygons, and Ellipses as masks for the image at the given downsampling
 # Converts rectangles and ellipses into polygons (4 rectangle points into an array of points on the outline)
 #     """
 #     sizeX = int(img.getSizeX() / downsample)
 #     sizeY = int(img.getSizeY() / downsample)
 
 #     masks=[]
 #     for id, rgb, points in getShapesAsPoints(img, point_downsample, downsample, roi_service):
@@ -401,58 +715,88 @@
 
 # 
 ## FILES
 #  
 
 def downloadFileAnnotation(file_annot: FileAnnotationWrapper, outdir=".") -> str:
     """
-Downloads FileAnnotation from OMERO into a local directory.\n
-file_annot: file annotation from previous processing script.\n
-out_dir: where to download this file.\n
-return: string path to downloaded file
+Downloads FileAnnotation from OMERO into a local directory.
+
+Parameters
+----------
+file_annot: omero.gateway.FileAnnotationWrapper
+    Remote Omero File Annotation object.
+out_dir: str, Default: '.' 
+    Where to download this file.
+
+Returns
+-------
+str 
+    String path to downloaded file.
     """
     path = os.path.abspath(outdir) + os.sep + file_annot.getFile().getName()
     print(f"Downloading {path}...")
     with open(path, 'wb') as f:
         for chunk in file_annot.getFileInChunks():
             f.write(chunk)
     print(f"{path} downloaded!")
     return path
 
 
 # TODO checkUserScripts
-def getScriptByName(conn: _BlitzGateway, fn: str, absolute=False, checkUserScripts=True) -> int:
+def getScriptByName(conn: _BlitzGateway, fn: str, absolute=False, checkUserScripts=False) -> int:
     """
-Searches for an omero script in the host with the given name.\n
-conn
+Searches for an omero script in the host with the given name.
+
+Parameters
+----------
+conn: omero.gateway.BlitzGateway
+    An Omero BlitzGateway with a session.
+fn: str
+    Name of remote Omero.Script
+absolute: bool, Default: False
+    Absolute uses omero's getScriptID(). This method does not accept wildcards and requires a path.
+    Default will get all remote script names and compare the filename using python equivelency (allows wildcards).
+checkUserScripts: bool, Default: False
+    Not implemented.
+
+Returns
+-------
+int
+    Omero.Script Id
     """
     if checkUserScripts: print("getScriptByName not fully implemented! May cause unexpected results!")
     scriptService=conn.getScriptService()
     try:
         if absolute is True: return scriptService.getScriptID(fn)
         for script in scriptService.getScripts():
             if script.getName().getValue() == fn:
                 return script.getId().getValue()
     finally:
         scriptService.close()
 
 def uploadFileAsAnnotation(parent_obj: ImageWrapper, file_path: str, namespace:str, 
-        mime:str=None, conn:_BlitzGateway=None, overwrite=True) -> FileAnnotationI:
+        mime:str=None, overwrite=True) -> FileAnnotationI:
     """
-Uploads a given filepath to omero as an annotation for parent_obj under namespace.\n
-parent_obj: object that should own an annotation (typically an ImageWrapper)\n
-file_path: path of file for uploading\n
-namespace: namespace to put future file annotation\n
-mime: mimetype for filetype. if None this will be guessed based on file extension and filetype dictionary\n
-conn: conn passthrough\n
-overwrite: overwrite existing file annotation in this namespace.\n
-return: created FileAnnotation object
+Uploads a given filepath to omero as an annotation for parent_obj under namespace.
+
+parent_obj: omero.gateway.ParentWrapper
+    Object that should own the annotation. (typically an ImageWrapper)
+file_path: str
+    Local path of file to upload as annotation.
+namespace: str 
+    Remote namespace to put the file annotation
+mime: str, optional 
+    Mimetype for filetype. If None this will be guessed based on file extension and filetype dictionary
+overwrite: bool, Default: True
+    Overwrites existing file annotation in this namespace.
+return: omero.gateway.FileAnnotationWrapper
+    Uploaded FileAnnotation object.
     """
-    if conn is None:
-        conn = parent_obj._conn
+    conn = parent_obj._conn
 
     # if no mime provided try to parse from filename, if cannot, assume plaintext
     if mime is None:
         mime = FILETYPE_DICTIONARY.get(
             lookup_filetype_by_name(file_path),
             FILETYPE_DICTIONARY["GENERIC_FILES"]["TXT"]
         )["MIME"]
@@ -469,20 +813,26 @@
     return annot_obj
 
 #
 ## PARSING
 #
 def idsToImageIds(conn: _BlitzGateway, dType: str, rawIds: list[int]) -> list[int]:
     """
-Gathers image ids from given OMERO objects.\n
-For Project and Dataset ids. Takes Image ids too for compatibility.\n
-conn: connected BlitzGateway\n
-dType: string data type, should be one of: 'Image','Dataset', or 'Project'\n
-rawIds: ids for datatype\n
-return: [imageId,...]
+Gathers image ids from given OMERO objects. For Project and Dataset ids. Takes Image ids too for compatibility.
+
+Parameters
+----------
+conn: omero.gateway.BlitzGateway
+    An Omero BlitzGateway with a session.
+dType: str 
+    String data type, should be one of: 'Image','Dataset', or 'Project'
+rawIds: list[int]
+    ids for datatype
+return: list[int]
+    List of all found Image ids
     """
     if dType != "Image" :
         # project to dataset
         if dType == "Project" :
             projectIds = rawIds; rawIds = []
             for projectId in projectIds :
                 for dataset in conn.getObjects('dataset', opts={'project' : projectId}) :
```

### Comparing `lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/PKG-INFO` & `lavlab-python-utils-1.0.2/lavlab_python_utils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+
+TODO: this readme
+=================
+for more info goto: https://lavlab-python-utils.readthedocs.io/en/latest/
```

