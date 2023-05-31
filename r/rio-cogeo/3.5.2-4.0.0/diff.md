# Comparing `tmp/rio_cogeo-3.5.2.tar.gz` & `tmp/rio_cogeo-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio_cogeo-3.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rio_cogeo-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rio_cogeo-3.5.2.tar` & `rio_cogeo-4.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      213 2023-05-22 21:41:00.779658 rio_cogeo-3.5.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1172 2023-05-22 21:41:00.779658 rio_cogeo-3.5.2/.gitignore
--rw-r--r--   0        0        0      740 2023-05-22 21:41:00.779658 rio_cogeo-3.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1517 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/LICENSE
--rw-r--r--   0        0        0     3373 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/README.md
--rw-r--r--   0        0        0     2305 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/__init__.py
--rw-r--r--   0        0        0    29058 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/cogeo.py
--rw-r--r--   0        0        0      406 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/errors.py
--rw-r--r--   0        0        0     1950 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/models.py
--rw-r--r--   0        0        0     4521 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/profiles.py
--rw-r--r--   0        0        0       21 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/scripts/__init__.py
--rw-r--r--   0        0        0    13693 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/scripts/cli.py
--rw-r--r--   0        0        0     4595 2023-05-22 21:41:00.783659 rio_cogeo-3.5.2/rio_cogeo/utils.py
--rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 rio_cogeo-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0      213 2023-05-31 08:38:21.946849 rio_cogeo-4.0.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1172 2023-05-31 08:38:21.946849 rio_cogeo-4.0.0/.gitignore
+-rw-r--r--   0        0        0      740 2023-05-31 08:38:21.946849 rio_cogeo-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1517 2023-05-31 08:38:21.946849 rio_cogeo-4.0.0/LICENSE
+-rw-r--r--   0        0        0     3373 2023-05-31 08:38:21.946849 rio_cogeo-4.0.0/README.md
+-rw-r--r--   0        0        0     2324 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/rio_cogeo/__init__.py
+-rw-r--r--   0        0        0    28480 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/rio_cogeo/cogeo.py
+-rw-r--r--   0        0        0      406 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/rio_cogeo/errors.py
+-rw-r--r--   0        0        0     1950 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/rio_cogeo/models.py
+-rw-r--r--   0        0        0     4521 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/rio_cogeo/profiles.py
+-rw-r--r--   0        0        0       21 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/rio_cogeo/scripts/__init__.py
+-rw-r--r--   0        0        0    13775 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/rio_cogeo/scripts/cli.py
+-rw-r--r--   0        0        0     4615 2023-05-31 08:38:21.950849 rio_cogeo-4.0.0/rio_cogeo/utils.py
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 rio_cogeo-4.0.0/PKG-INFO
```

### Comparing `rio_cogeo-3.5.2/.gitignore` & `rio_cogeo-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rio_cogeo-3.5.2/.pre-commit-config.yaml` & `rio_cogeo-4.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rio_cogeo-3.5.2/LICENSE` & `rio_cogeo-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rio_cogeo-3.5.2/README.md` & `rio_cogeo-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `rio_cogeo-3.5.2/pyproject.toml` & `rio_cogeo-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "click>=7.0",
     "rasterio>=1.3.3",
     "numpy~=1.15",
-    "morecantile>=3.1,<4.0",
+    "morecantile>=4.0,<5.0",
     "pydantic",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
@@ -88,14 +88,15 @@
 ignore_missing_imports = "True"
 
 [tool.ruff]
 select = [
     "D1",  # pydocstyle errors
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
+    "F",  # flake8
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
```

### Comparing `rio_cogeo-3.5.2/rio_cogeo/cogeo.py` & `rio_cogeo-4.0.0/rio_cogeo/cogeo.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import pathlib
 import sys
 import tempfile
 import warnings
 from contextlib import ExitStack, contextmanager
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union
 
 import click
 import morecantile
 import rasterio
 from rasterio.enums import ColorInterp
 from rasterio.enums import Resampling as ResamplingEnums
 from rasterio.env import GDALVersion
@@ -38,30 +38,59 @@
     fileobj.close()
     try:
         yield fileobj
     finally:
         os.remove(fileobj.name)
 
 
+# RasterIO() resampling method.
+# ref: https://gdal.org/api/raster_c_api.html#_CPPv418GDALRIOResampleAlg
+RIOResampling = Literal[
+    "nearest",
+    "bilinear",
+    "cubic",
+    "cubic_spline",
+    "lanczos",
+    "average",
+    "mode",
+    "gauss",
+    "rms",
+]
+
+# WarpKernel resampling method.
+# ref: https://gdal.org/api/gdalwarp_cpp.html#_CPPv4N14GDALWarpKernel9eResampleE
+WarpResampling = Literal[
+    "nearest",
+    "bilinear",
+    "cubic",
+    "cubic_spline",
+    "lanczos",
+    "average",
+    "mode",
+    "sum",
+    "rms",
+]
+
+
 def cog_translate(  # noqa: C901
     source: Union[str, pathlib.PurePath, DatasetReader, DatasetWriter, WarpedVRT],
     dst_path: Union[str, pathlib.PurePath],
     dst_kwargs: Dict,
     indexes: Optional[Sequence[int]] = None,
     nodata: Optional[Union[str, int, float]] = None,
     dtype: Optional[str] = None,
     add_mask: bool = False,
     overview_level: Optional[int] = None,
-    overview_resampling: str = "nearest",
+    overview_resampling: RIOResampling = "nearest",
     web_optimized: bool = False,
     tms: Optional[morecantile.TileMatrixSet] = None,
     zoom_level_strategy: str = "auto",
     zoom_level: Optional[int] = None,
     aligned_levels: Optional[int] = None,
-    resampling: str = "nearest",
+    resampling: WarpResampling = "nearest",
     in_memory: Optional[bool] = None,
     config: Optional[Dict] = None,
     allow_intermediate_compression: bool = False,
     forward_band_tags: bool = False,
     forward_ns_tags: bool = False,
     quiet: bool = False,
     temporary_compression: str = "DEFLATE",
@@ -89,15 +118,15 @@
     dtype: str, optional
         Overwrite output data type. Default will be the input data type.
     add_mask, bool, optional
         Force output dataset creation with a mask.
     overview_level : int, optional (default: None)
         COGEO overview (decimation) level. By default, inferred from data size.
     overview_resampling : str, optional (default: "nearest")
-        Resampling algorithm for overviews
+        RasterIO Resampling algorithm for overviews
     web_optimized: bool, optional (default: False)
         Create web-optimized cogeo.
     tms: morecantile.TileMatrixSet, optional (default: "WebMercatorQuad")
         TileMatrixSet to use for reprojection, resolution and alignment.
     zoom_level_strategy: str, optional (default: auto)
         Strategy to determine zoom level (same as in GDAL 3.2).
         LOWER will select the zoom level immediately below the theoretical computed non-integral zoom level, leading to subsampling.
@@ -106,15 +135,15 @@
         ref: https://gdal.org/drivers/raster/cog.html#raster-cog
     zoom_level: int, optional.
         Zoom level number (starting at 0 for coarsest zoom level). If this option is specified, `--zoom-level-strategy` is ignored.
     aligned_levels: int, optional.
         Number of overview levels for which GeoTIFF tile and tiles defined in the tiling scheme match.
         Default is to use the maximum overview levels. Note: GDAL use number of resolution levels instead of overview levels.
     resampling : str, optional (default: "nearest")
-        Resampling algorithm.
+        Warp Resampling algorithm.
     in_memory: bool, optional
         Force processing raster in memory (default: process in memory if small)
     config : dict
         Rasterio Env options.
     allow_intermediate_compression: bool, optional (default: False)
         Allow intermediate file compression to reduce memory/disk footprint.
         Note: This could reduce the speed of the process.
@@ -191,23 +220,23 @@
                 vrt_params.update(
                     {"nodata": nodata, "add_alpha": False, "src_nodata": nodata}
                 )
 
             if alpha:
                 vrt_params.update({"add_alpha": False})
 
-            if web_optimized and not use_cog_driver:
-                params = utils.get_web_optimized_params(
+            if web_optimized:
+                wo_params = utils.get_web_optimized_params(
                     src_dst,
                     zoom_level_strategy=zoom_level_strategy,
                     zoom_level=zoom_level,
                     aligned_levels=aligned_levels,
                     tms=tms,
                 )
-                vrt_params.update(**params)
+                vrt_params.update(**wo_params)
 
             with WarpedVRT(src_dst, **vrt_params) as vrt_dst:
                 meta = vrt_dst.meta
                 meta["count"] = len(indexes)
 
                 if add_mask:
                     meta.pop("nodata", None)
@@ -306,43 +335,40 @@
                 tags.update(
                     {
                         "OVR_RESAMPLING_ALG": ResamplingEnums[
                             overview_resampling
                         ].name.upper()
                     }
                 )
-                if additional_cog_metadata:
-                    tags.update(**additional_cog_metadata)
-
-                if forward_ns_tags:
-                    namespaces = src_dst.tag_namespaces()
-                    for ns in namespaces:
-                        if ns in ["DERIVED_SUBDATASETS", "IMAGE_STRUCTURE"]:
-                            continue
-                        tmp_dst.update_tags(ns=ns, **src_dst.tags(ns=ns))
-
-                if web_optimized and not use_cog_driver:
+                if web_optimized:
                     default_zoom = tms.zoom_for_res(
                         max(tmp_dst.res),
                         max_z=30,
                         zoom_level_strategy=zoom_level_strategy,
                     )
-                    dst_kwargs.update(
+                    tags.update(
                         {
-                            "@TILING_SCHEME_NAME": tms.identifier,
-                            "@TILING_SCHEME_ZOOM_LEVEL": zoom_level
+                            "TILING_SCHEME_NAME": tms.id or "CUSTOM",
+                            "TILING_SCHEME_ZOOM_LEVEL": zoom_level
                             if zoom_level is not None
                             else default_zoom,
                         }
                     )
-
                     if aligned_levels:
-                        dst_kwargs.update(
-                            {"@TILING_SCHEME_ALIGNED_LEVELS": aligned_levels}
-                        )
+                        tags["TILING_SCHEME_ALIGNED_LEVELS"] = aligned_levels
+
+                if additional_cog_metadata:
+                    tags.update(**additional_cog_metadata)
+
+                if forward_ns_tags:
+                    namespaces = src_dst.tag_namespaces()
+                    for ns in namespaces:
+                        if ns in ["DERIVED_SUBDATASETS", "IMAGE_STRUCTURE"]:
+                            continue
+                        tmp_dst.update_tags(ns=ns, **src_dst.tags(ns=ns))
 
                 tmp_dst.update_tags(**tags)
                 tmp_dst._set_all_scales([vrt_dst.scales[b - 1] for b in indexes])
                 tmp_dst._set_all_offsets([vrt_dst.offsets[b - 1] for b in indexes])
 
                 if not quiet:
                     click.echo("Writing output to: {}".format(dst_path), err=True)
@@ -350,35 +376,14 @@
                 if use_cog_driver:
                     if not GDALVersion.runtime().at_least("3.1"):
                         raise Exception(
                             "GDAL 3.1 or above required to use the COG driver."
                         )
 
                     dst_kwargs["driver"] = "COG"
-                    if web_optimized:
-                        dst_kwargs["TILING_SCHEME"] = (
-                            "GoogleMapsCompatible"
-                            if tms.identifier == "WebMercatorQuad"
-                            else tms.identifier
-                        )
-
-                        if zoom_level is not None:
-                            if not GDALVersion.runtime().at_least("3.5"):
-                                warnings.warn(
-                                    "ZOOM_LEVEL option is only available with GDAL >3.5."
-                                )
-
-                            dst_kwargs["ZOOM_LEVEL"] = zoom_level
-
-                        dst_kwargs["ZOOM_LEVEL_STRATEGY"] = zoom_level_strategy
-
-                        if aligned_levels is not None:
-                            # GDAL uses Number of resolution (not overviews)
-                            # See https://github.com/OSGeo/gdal/issues/5336#issuecomment-1042946603
-                            dst_kwargs["aligned_levels"] = aligned_levels + 1
 
                     if add_mask and dst_kwargs.get("compress", "") != "JPEG":
                         warnings.warn(
                             "With GDAL COG driver, mask band will be translated to an alpha band."
                         )
 
                     dst_kwargs["overview_resampling"] = overview_resampling
```

### Comparing `rio_cogeo-3.5.2/rio_cogeo/models.py` & `rio_cogeo-4.0.0/rio_cogeo/models.py`

 * *Files identical despite different names*

### Comparing `rio_cogeo-3.5.2/rio_cogeo/profiles.py` & `rio_cogeo-4.0.0/rio_cogeo/profiles.py`

 * *Files identical despite different names*

### Comparing `rio_cogeo-3.5.2/rio_cogeo/scripts/cli.py` & `rio_cogeo-4.0.0/rio_cogeo/scripts/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Rio_cogeo.scripts.cli."""
 
+import json
 import os
+import typing
 
 import click
 import numpy
-from rasterio.enums import Resampling as ResamplingEnums
-from rasterio.env import GDALVersion
+from morecantile import TileMatrixSet
 from rasterio.rio import options
-from rasterio.warp import SUPPORTED_RESAMPLING as WarpResampling
 
 from rio_cogeo import __version__ as cogeo_version
-from rio_cogeo.cogeo import cog_info, cog_translate, cog_validate
+from rio_cogeo.cogeo import (
+    RIOResampling,
+    WarpResampling,
+    cog_info,
+    cog_translate,
+    cog_validate,
+)
 from rio_cogeo.profiles import cog_profiles
 
-OverviewResampling = [r for r in ResamplingEnums if r.value < 8]
-if GDALVersion.runtime().at_least("3.3"):
-    OverviewResampling.append(ResamplingEnums.rms)
-
 IN_MEMORY_THRESHOLD = int(os.environ.get("IN_MEMORY_THRESHOLD", 10980 * 10980))
 
 
 class BdxParamType(click.ParamType):
     """Band index type."""
 
     name = "bidx"
@@ -117,15 +119,15 @@
     help="Overview level (if not provided, appropriate overview level will be "
     "selected until the smallest overview is smaller than the value of the "
     "internal blocksize)",
 )
 @click.option(
     "--overview-resampling",
     help="Overview creation resampling algorithm.",
-    type=click.Choice([it.name for it in OverviewResampling]),
+    type=click.Choice(list(typing.get_args(RIOResampling))),
     default="nearest",
     show_default=True,
 )
 @click.option(
     "--overview-blocksize",
     default=lambda: os.environ.get("GDAL_TIFF_OVR_BLOCKSIZE", 128),
     help="Overview's internal tile size (default defined by "
@@ -152,15 +154,15 @@
     type=int,
     help="Number of overview levels for which GeoTIFF tile and tiles defined in the tiling scheme match.",
 )
 @click.option(
     "--resampling",
     "-r",
     help="Resampling algorithm. Will only be applied with the `--web-optimized` option.",
-    type=click.Choice([it.name for it in WarpResampling]),
+    type=click.Choice(list(typing.get_args(WarpResampling))),
     default="nearest",
     show_default=True,
 )
 @click.option(
     "--in-memory/--no-in-memory",
     default=None,
     help="Force processing raster in memory / not in memory (default: process in memory "
@@ -197,14 +199,19 @@
 @click.option(
     "--use-cog-driver",
     help="Use GDAL COG Driver (require GDAL>=3.1).",
     is_flag=True,
     default=False,
     show_default=True,
 )
+@click.option(
+    "--tms",
+    help="Path to TileMatrixSet JSON file.",
+    type=click.Path(),
+)
 @options.creation_options
 @click.option(
     "--config",
     "config",
     metavar="NAME=VALUE",
     multiple=True,
     callback=options._cb_key_val,
@@ -232,14 +239,15 @@
     resampling,
     in_memory,
     allow_intermediate_compression,
     forward_band_tags,
     forward_ns_tags,
     threads,
     use_cog_driver,
+    tms,
     creation_options,
     config,
     quiet,
 ):
     """Create Cloud Optimized Geotiff."""
     output_profile = cog_profiles.get(cogeo_profile)
     output_profile.update({"BIGTIFF": os.environ.get("BIGTIFF", "IF_SAFER")})
@@ -257,14 +265,21 @@
         {
             "GDAL_NUM_THREADS": threads,
             "GDAL_TIFF_INTERNAL_MASK": os.environ.get("GDAL_TIFF_INTERNAL_MASK", True),
             "GDAL_TIFF_OVR_BLOCKSIZE": str(overview_blocksize),
         }
     )
 
+    if tms:
+        with open(tms, "r") as f:
+            tilematrixset = TileMatrixSet(**json.load(f))
+
+    else:
+        tilematrixset = None
+
     cog_translate(
         input,
         output,
         output_profile,
         indexes=bidx,
         nodata=nodata,
         dtype=dtype,
@@ -277,14 +292,15 @@
         aligned_levels=aligned_levels,
         resampling=resampling,
         in_memory=in_memory,
         config=config,
         allow_intermediate_compression=allow_intermediate_compression,
         forward_band_tags=forward_band_tags,
         forward_ns_tags=forward_ns_tags,
+        tms=tilematrixset,
         use_cog_driver=use_cog_driver,
         quiet=quiet,
     )
 
 
 @cogeo.command(short_help="Validate COGEO")
 @options.file_in_arg
```

### Comparing `rio_cogeo-3.5.2/rio_cogeo/utils.py` & `rio_cogeo-4.0.0/rio_cogeo/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,18 +49,19 @@
     src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT],
     tilesize: int = 256,
     tms: morecantile.TileMatrixSet = morecantile.tms.get("WebMercatorQuad"),
     zoom_level_strategy: str = "auto",
 ) -> Tuple[int, int]:
     """Calculate raster min/max zoom level."""
     # If the raster is not in the TMS CRS we calculate its projected properties (height, width, resolution)
-    if src_dst.crs != tms.rasterio_crs:
+    tms_crs = tms.rasterio_crs
+    if src_dst.crs != tms_crs:
         aff, w, h = calculate_default_transform(
             src_dst.crs,
-            tms.rasterio_crs,
+            tms_crs,
             src_dst.width,
             src_dst.height,
             *src_dst.bounds,
         )
     else:
         aff = list(src_dst.transform)
         w = src_dst.width
@@ -88,31 +89,35 @@
     src_dst,
     zoom_level_strategy: str = "auto",
     zoom_level: Optional[int] = None,
     aligned_levels: Optional[int] = None,
     tms: morecantile.TileMatrixSet = morecantile.tms.get("WebMercatorQuad"),
 ) -> Dict:
     """Return VRT parameters for a WebOptimized COG."""
-    if src_dst.crs != tms.rasterio_crs:
-        with WarpedVRT(src_dst, crs=tms.rasterio_crs) as vrt:
+    tms_crs = tms.rasterio_crs
+
+    if src_dst.crs != tms_crs:
+        with WarpedVRT(src_dst, crs=tms_crs) as vrt:
             bounds = vrt.bounds
             aff = list(vrt.transform)
+
     else:
         bounds = src_dst.bounds
         aff = list(src_dst.transform)
 
     resolution = max(abs(aff[0]), abs(aff[4]))
 
     if zoom_level is None:
         # find max zoom (closest to the raster resolution)
         max_zoom = tms.zoom_for_res(
             resolution,
             max_z=30,
             zoom_level_strategy=zoom_level_strategy,
         )
+
     else:
         max_zoom = zoom_level
 
     # defined the zoom level we want to align the raster
     aligned_levels = aligned_levels or 0
     base_zoom = max_zoom - aligned_levels
 
@@ -131,12 +136,12 @@
         morecantile.Tile(lr_tile.x + 1, lr_tile.y + 1, lr_tile.z)
     )
 
     vrt_width = max(1, round((e - w) / vrt_transform.a))
     vrt_height = max(1, round((s - n) / vrt_transform.e))
 
     return {
-        "crs": tms.rasterio_crs,
+        "crs": tms_crs,
         "transform": vrt_transform,
         "width": vrt_width,
         "height": vrt_height,
     }
```

### Comparing `rio_cogeo-3.5.2/PKG-INFO` & `rio_cogeo-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-cogeo
-Version: 3.5.2
+Version: 4.0.0
 Summary: Cloud Optimized GeoTIFF (COGEO) creation plugin for rasterio
 Keywords: COGEO,CloudOptimized Geotiff,rasterio
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: click>=7.0
 Requires-Dist: rasterio>=1.3.3
 Requires-Dist: numpy~=1.15
-Requires-Dist: morecantile>=3.1,<4.0
+Requires-Dist: morecantile>=4.0,<5.0
 Requires-Dist: pydantic
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: cogdumper ; extra == "test"
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: rio-cogeo Version: 3.5.2 Summary: Cloud Optimized
+Metadata-Version: 2.1 Name: rio-cogeo Version: 4.0.0 Summary: Cloud Optimized
 GeoTIFF (COGEO) creation plugin for rasterio Keywords: COGEO,CloudOptimized
 Geotiff,rasterio Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: GIS Requires-Dist: click>=7.0 Requires-Dist:
-rasterio>=1.3.3 Requires-Dist: numpy~=1.15 Requires-Dist: morecantile>=3.1,<4.0
+rasterio>=1.3.3 Requires-Dist: numpy~=1.15 Requires-Dist: morecantile>=4.0,<5.0
 Requires-Dist: pydantic Requires-Dist: pre-commit ; extra == "dev" Requires-
 Dist: mkdocs ; extra == "docs" Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: pytest ; extra == "test" Requires-Dist: pytest-cov ; extra ==
 "test" Requires-Dist: cogdumper ; extra == "test" Project-URL: Documentation,
 https://cogeotiff.github.io/rio-cogeo/ Project-URL: Source, https://github.com/
 cogeotiff/rio-cogeo Provides-Extra: dev Provides-Extra: docs Provides-Extra:
 test # rio-cogeo
```

