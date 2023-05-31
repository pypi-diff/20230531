# Comparing `tmp/pyrsig-0.3.1.tar.gz` & `tmp/pyrsig-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrsig-0.3.1.tar", last modified: Fri May 12 20:31:01 2023, max compression
+gzip compressed data, was "dist/pyrsig-0.4.0.tar", last modified: Wed May 31 14:53:41 2023, max compression
```

## Comparing `pyrsig-0.3.1.tar` & `pyrsig-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-12 20:31:01.000000 pyrsig-0.3.1/
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.3.1/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-05-12 20:31:01.000000 pyrsig-0.3.1/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.3.1/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-12 20:31:01.000000 pyrsig-0.3.1/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      357 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/requires.txt
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-12 20:31:01.000000 pyrsig-0.3.1/pyrsig/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-12 20:31:01.000000 pyrsig-0.3.1/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)      800 2023-03-29 20:44:48.000000 pyrsig-0.3.1/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.3.1/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2058 2023-03-29 20:31:50.000000 pyrsig-0.3.1/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-03-29 20:35:02.000000 pyrsig-0.3.1/pyrsig/tests/test_misc.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.3.1/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.3.1/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)    37717 2023-05-12 20:28:38.000000 pyrsig-0.3.1/pyrsig/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-05-12 20:31:01.000000 pyrsig-0.3.1/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.3.1/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-31 14:53:41.000000 pyrsig-0.4.0/
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.4.0/setup.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-05-31 14:53:41.000000 pyrsig-0.4.0/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.4.0/LICENSE
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-31 14:53:41.000000 pyrsig-0.4.0/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)      382 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-05-31 14:53:40.000000 pyrsig-0.4.0/pyrsig.egg-info/requires.txt
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-31 14:53:41.000000 pyrsig-0.4.0/pyrsig/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-31 14:53:41.000000 pyrsig-0.4.0/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)     1739 2023-05-31 14:41:16.000000 pyrsig-0.4.0/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.4.0/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2058 2023-03-29 20:31:50.000000 pyrsig-0.4.0/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-05-31 14:34:48.000000 pyrsig-0.4.0/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.4.0/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.4.0/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-05-31 14:48:57.000000 pyrsig-0.4.0/pyrsig/tests/test_gui.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    46992 2023-05-31 14:29:01.000000 pyrsig-0.4.0/pyrsig/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-05-31 14:53:41.000000 pyrsig-0.4.0/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.4.0/README.md
```

### Comparing `pyrsig-0.3.1/setup.py` & `pyrsig-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.3.1/PKG-INFO` & `pyrsig-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.3.1/LICENSE` & `pyrsig-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.3.1/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.4.0/pyrsig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.3.1/pyrsig/tests/test_ioapi.py` & `pyrsig-0.4.0/pyrsig/tests/test_ioapi.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.3.1/pyrsig/tests/test_dataframes.py` & `pyrsig-0.4.0/pyrsig/tests/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.3.1/pyrsig/tests/test_coards.py` & `pyrsig-0.4.0/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.3.1/pyrsig/__init__.py` & `pyrsig-0.4.0/pyrsig/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-__all__ = ['RsigApi', 'open_ioapi']
-__version__ = '0.3.1'
+__all__ = ['RsigApi', 'RsigGui', 'open_ioapi']
+__version__ = '0.4.0'
 
 import pandas as pd
 
+
 _def_grid_kw = {
     '12US1': dict(
         GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
         XORIG=-2556000.0, YORIG=-1728000.0, XCELL=12000., YCELL=12000.,
         P_ALP=33., P_BET=45., P_GAM=-97., XCENT=-97., YCENT=40.
     ),
     '4US1': dict(
@@ -111,14 +112,43 @@
     'tropomi.offl.ch4.methane_mixing_ratio_bias_corrected',
     'viirsnoaa.jrraod.AOD550', 'viirsnoaa.vaooo.AerosolOpticalDepth_at_550nm',
 )
 
 _point_prefixes = ('airnow', 'aqs', 'purpleair', 'pandora')
 
 
+def _actionf(msg, action, ErrorTyp=None):
+    """
+    Convenience function for warning or raising an error.
+
+    Arguments
+    ---------
+    msg : str
+        Message to raise or warn.
+    action : str
+        If 'error', raise ErrorTyp(msg)
+        If 'warn', warnings.warn using msg
+        Else do nothing.
+    ErrorTyp : Exception
+        Defaults to ErrorTyp
+
+    Returns
+    -------
+    None
+    """
+    import warnings
+
+    if ErrorTyp is None:
+        ErrorTyp = ValueError
+    if action == 'error':
+        raise ErrorTyp(msg)
+    elif action == 'warn':
+        warnings.warn(msg)
+
+
 def parsexml(root):
     """Recursive xml parsing:
     Given a root, return dictionaries for each element and its children.
     Each element has children, attributes (attr), tag, and text.
     If any of these has no elements, it will be removed.
     """
     out = {}
@@ -176,14 +206,16 @@
         out.append(record)
 
     return out
 
 
 def _progress(blocknum, readsize, totalsize):
     """
+    Display progress using dots or % indicator.
+
     Arguments
     ---------
     blocknum : int
         block number of blocks to be read
     readsize : int
         chunksize read
     totalsize : int
@@ -203,25 +235,34 @@
             print('Retrieving .', end='', flush=True)
         if (blocknum % pblocks) == 0:
             print('.', end='', flush=True)
 
 
 def _getfile(url, outpath, maxtries=5, verbose=1, overwrite=False):
     """
+    Download file from RSIG using fault tolerance and optional caching
+    when overwrite is False.
+
     Arguments
     ---------
     url : str
         path to retrieve
     outpath : str
         path to save file to
     maxtries : int
         try this many times before quitting
+    verbose : int
+        Level of verbosity
     overwrite : bool
         If True, overwrite existing files.
         If False, reuse existing files.
+
+    Returns
+    -------
+    None
     """
     import time
     from urllib.request import urlretrieve
     import ssl
     import os
 
     ssl._create_default_https_context = ssl._create_unverified_context
@@ -267,17 +308,129 @@
             print('Failed', url, t1 - t0)
         tries += 1
 
         if verbose > 0:
             print('')
 
 
+def get_proj4(attrs, earth_radius=6370000.):
+    """
+    Create a proj4 formatted grid definition using IOAPI attrs and earth_radius
+
+    Arguments
+    ---------
+    attrs : dict-like
+        Mappable of IOAPI properties that supports the items method
+    earth_radius : float
+        Assumed radius of the earth. 6370000 is the WRF default.
+
+    Returns
+    -------
+    projstr : str
+        proj4 formatted string such that the domain southwest corner starts at
+        (0, 0) and ends at (NCOLS, NROWS)
+    """
+    props = {k: v for k, v in attrs.items()}
+    props['x_0'] = -props['XORIG']
+    props['y_0'] = -props['YORIG']
+    props.setdefault('earth_radius', earth_radius)
+
+    if props['GDTYP'] == 2:
+        projstr = (
+            '+proj=lcc +lat_1={P_ALP} +lat_2={P_BET} +lat_0={YCENT}'
+            ' +lon_0={XCENT} +R={earth_radius} +x_0={x_0} +y_0={y_0}'
+            ' +to_meter={XCELL} +no_defs'
+        ).format(**props)
+    elif props['GDTYP'] == 6:
+        projstr = (
+            '+proj=stere +lat_0={P_ALP * 90} +lat_ts={P_BET} +lon_0={XCENT} '
+            + '+x_0={x_0} +y_0={y_0} +R={earth_radius} +to_meter={XCELL} '
+            + '+no_defs'
+        ).format(**props)
+    else:
+        raise ValueError('GDTYPE {GDTYP} not implemented'.format(**props))
+
+    return projstr
+
+
+def customize_grid(grid_kw, bbox, clip=True):
+    """
+    Redefine grid_kw to cover bbox by removing extra rows and columns and
+    redefining XORIG, YORIG, NCOLS and NROWS.
+
+    Arguments
+    ---------
+    grid_kw : dict or str
+        If str, must be a known grid in default grids.
+        If dict, must include all IOAPI grid metadata properties
+    bbox : tuple
+        wlon, slat, elon, nlat in decimal degrees (-180 to 180)
+    clip : bool
+        If True, limit grid to original grid bounds
+
+    Returns
+    -------
+    ogrid_kw : dict
+        IOAPI grid metadata properties with XORIG/YORIG and NCOLS/NROWS
+        adjusted such that it only covers bbox or (if clip) only covers
+        the portion of bbox covered by the original grid_kw.
+    """
+    import pyproj
+    import numpy as np
+
+    if isinstance(grid_kw, str):
+        grid_kw = _def_grid_kw[grid_kw]
+
+    ogrid_kw = {k: v for k, v in grid_kw.items()}
+    proj4str = get_proj4(grid_kw)
+    proj = pyproj.Proj(proj4str)
+    llx, lly = proj(*bbox[:2])
+    urx, ury = proj(*bbox[2:])
+    midx, midy = proj((bbox[0] + bbox[2]) / 2, (bbox[1] + bbox[3]) / 2)
+    maxy = np.max([lly, ury, midy])
+    miny = np.min([lly, ury, midy])
+    maxx = np.max([llx, urx, midx])
+    minx = np.min([llx, urx, midx])
+
+    lli, llj = np.floor([minx, miny]).astype('i')
+    uri, urj = np.ceil([maxx, maxy]).astype('i')
+    if clip:
+        lli, llj = np.maximum(0, [lli, llj])
+        uri = np.minimum(grid_kw['NCOLS'], uri)
+        urj = np.minimum(grid_kw['NROWS'], urj)
+    ogrid_kw['XORIG'] = grid_kw['XORIG'] + lli * grid_kw['XCELL']
+    ogrid_kw['YORIG'] = grid_kw['YORIG'] + llj * grid_kw['YCELL']
+    ogrid_kw['NCOLS'] = uri - lli
+    ogrid_kw['NROWS'] = urj - llj
+    return ogrid_kw
+
+
 def open_ioapi(path, metapath=None, earth_radius=6370000.):
+    """
+    Open an IOAPI file, add coordinate data, and optionally add RSIG metadata.
+
+    Arguments
+    ---------
+    path : str
+        Path to IOAPI formatted files.
+    metapath : str
+        Path to metadata associated with the RSIG query. The metadata will be
+        added as metadata global property.
+    earth_radius : float
+        Assumed radius of the earth. 6370000 is the WRF default.
+
+    Returns
+    -------
+    ds : xarray.Dataset
+        Dataset with IOAPI metadata
+    """
     import xarray as xr
     import numpy as np
+    import warnings
+
     f = xr.open_dataset(path, engine='netcdf4')
     lvls = f.attrs['VGLVLS']
     tflag = f['TFLAG'][:, 0, :].astype('i').values
     yyyyjjj = tflag[:, 0]
     yyyyjjj = np.where(yyyyjjj < 1, 1970001, yyyyjjj)
     HHMMSS = tflag[:, 1]
     tstrs = []
@@ -289,25 +442,19 @@
         f.coords['TSTEP'] = time
     except Exception:
         pass
 
     f.coords['LAY'] = (lvls[:-1] + lvls[1:]) / 2.
     f.coords['ROW'] = np.arange(f.attrs['NROWS']) + 0.5
     f.coords['COL'] = np.arange(f.attrs['NCOLS']) + 0.5
-    props = {k: v for k, v in f.attrs.items()}
-    props['x_0'] = -props['XORIG']
-    props['y_0'] = -props['YORIG']
-    props.setdefault('earth_radius', earth_radius)
-
-    if f.attrs['GDTYP'] == 2:
-        f.attrs['crs_proj4'] = (
-            '+proj=lcc +lat_1={P_ALP} +lat_2={P_BET} +lat_0={YCENT}'
-            ' +lon_0={XCENT} +R={earth_radius} +x_0={x_0} +y_0={y_0}'
-            ' +to_meter={XCELL} +no_defs'
-        ).format(**props)
+    try:
+        proj4str = get_proj4(f.attrs, earth_radius=earth_radius)
+        f.attrs['crs_proj4'] = proj4str
+    except ValueError as e:
+        warnings.warn(str(e))
 
     if metapath is None:
         import os
         if os.path.exists(path + '.txt'):
             metapath = path + '.txt'
 
     if metapath is False:
@@ -322,15 +469,15 @@
 
 
 class RsigApi:
     def __init__(
         self, key=None, bdate=None, edate=None, bbox=None, grid_kw=None,
         tropomi_kw=None, purpleair_kw=None, viirsnoaa_kw=None,
         server='ofmpub.epa.gov', compress=1, corners=1, encoding=None,
-        overwrite=False, workdir='.'
+        overwrite=False, workdir='.', gridfit=False
     ):
         """
         RsigApi is a python-based interface to RSIG's web-based API
 
         Arguments
         ---------
         key : str
@@ -372,14 +519,17 @@
           with encoding for all variables. If _FillValue is provided, it will
           not be applied to TFLAG and COUNT.
         overwrite : bool
           If True, overwrite downloaded files in workdir.
           If False, reuse downloaded files in workdir.
         workdir : str
           Working directory (must exist) defaults to '.'
+        gridfit : bool
+          Default (False) keep grid as supplied.
+          If True, redefine grid to remove cells outside the bbox.
 
         Properties
         ----------
         grid_kw : dict
           Dictionary of regridding IOAPI properties. Defaults to 12US1
 
         viirsnoaa_kw : dict
@@ -427,14 +577,17 @@
             grid_kw = '12US1'
 
         if isinstance(grid_kw, str):
             if grid_kw not in _def_grid_kw:
                 raise KeyError('unknown grid, you must specify properites')
             grid_kw = _def_grid_kw[grid_kw].copy()
 
+        if gridfit:
+            grid_kw = customize_grid(grid_kw, self.bbox)
+
         self.grid_kw = grid_kw
 
         if tropomi_kw is None:
             tropomi_kw = {'minimum_quality': 75, 'maximum_cloud_fraction': 1.0}
 
         self.tropomi_kw = tropomi_kw
 
@@ -1081,7 +1234,165 @@
                 metatxt = metaf.read()
             f.attrs['metadata'] = metatxt
 
         if removegz:
             os.remove(outpath)
 
         return f
+
+
+class RsigGui:
+    @classmethod
+    def from_api(cls, api):
+        gui = cls()
+        (
+            gui._bbw.value,
+            gui._bbs.value,
+            gui._bbe.value,
+            gui._bbn.value,
+        ) = api.bbox
+        if api.bdate is not None:
+            gui._dates.value = api.bdate
+        if api.edate is not None:
+            gui._datee.value = api.edate
+        if api.key is not None:
+            gui._prodd.value = api.key
+        if api.grid_kw is not None:
+            gui._gridd.value = api.grid_kw['GDNAM']
+        if api.workdir is not None:
+            gui._workd.value = api.workdir
+
+        return gui
+
+    def __init__(self):
+        """
+        RsigGui Object designed for IPython with ipywidgets in Jupyter
+
+        Example:
+        gui = RsigGui()
+        gui.form  # As last line in cell, displays controls for user
+        gui.plotopts()  # Plots current options
+        gui.check()  # Check bounding box and date options make sense
+        rsigapi = gui.get_api() # Convert gui to standard api
+        # proceed with normal RsigApi usage
+        """
+        from datetime import date
+        from ipywidgets import Layout, Box, Dropdown, Label, FloatSlider
+        from ipywidgets import DatePicker, Textarea
+        form_item_layout = Layout(
+            display='flex', flex_flow='row', justify_content='space-between'
+        )
+
+        prodopts = RsigApi().keys()
+        self._prodd = prodd = Dropdown(options=prodopts)
+        self._gridd = gridd = Dropdown(
+            options=list(_def_grid_kw), value='12US1'
+        )
+        self._dates = datesa = DatePicker(
+            description='Start Date', disabled=False,
+            value=(
+                date.today()
+                - pd.to_timedelta('7d')
+            )
+        )
+        self._datee = dateea = DatePicker(
+            description='End Date', disabled=False, value=datesa.value
+        )
+        self._bbw = bbw = FloatSlider(min=-180, max=180, value=-126)
+        self._bbe = bbe = FloatSlider(min=-180, max=180, value=-66)
+        self._bbs = bbs = FloatSlider(min=-90, max=90, value=24)
+        self._bbn = bbn = FloatSlider(min=-90, max=90, value=50)
+        self._workd = workd = Textarea(value='.')
+        form_items = [
+            Box([Label(value='RSIG Options')], layout=form_item_layout),
+            Box([
+                Label(value='Data Product'), prodd
+            ], layout=form_item_layout),
+            Box([Label(value='Southest'), bbs, Label(value='Northest'), bbn]),
+            Box([Label(value='Westest'), bbw, Label(value='Eastest'), bbe]),
+            Box([
+                Label(value='Date Start'), datesa,
+                Label(value='End'), dateea
+            ], layout=form_item_layout),
+            Box([Label(value='Grid Option'), gridd], layout=form_item_layout),
+            Box([
+                Label(value='Working Directory'), workd
+            ], layout=form_item_layout),
+        ]
+
+        self._form = Box(form_items, layout=Layout(
+            display='flex', flex_flow='column', border='solid 2px',
+            align_items='stretch', width='50%'
+        ))
+
+    def date_range(self):
+        import pandas as pd
+        return pd.date_range(self.bdate, self.edate)
+
+    @property
+    def form(self):
+        return self._form
+
+    @property
+    def key(self):
+        return self._prodd.value
+
+    @property
+    def bdate(self):
+        return self._dates.value
+
+    @property
+    def edate(self):
+        return self._datee.value
+
+    @property
+    def grid_kw(self):
+        return self._gridd.value
+
+    @property
+    def bbox(self):
+        return tuple([
+            v.value
+            for v in [self._bbw, self._bbs, self._bbe, self._bbn]
+        ])
+
+    @property
+    def workdir(self):
+        return self._workd.value
+
+    def plotopts(self):
+        import pycno
+        import matplotlib.pyplot as plt
+
+        fig, ax = plt.subplots()
+        bbw, bbs, bbe, bbn = self.bbox
+        ax.plot(
+            [bbw, bbe, bbe, bbw, bbw],
+            [bbs, bbs, bbn, bbn, bbs],
+            color='r'
+        )
+        fig.suptitle(f'Query Options: {self.key}, {self.grid_kw}')
+        ax.set(title=f'{self.bdate:%FT%H:%M:%S} {self.edate:%FT%H:%M:%S}')
+        pycno.cno().drawstates(ax=ax)
+        return fig
+
+    def get_api(self):
+        rsigapi = RsigApi(
+            key=self.key, bdate=self.bdate, edate=self.edate,
+            bbox=self.bbox, grid_kw=self.grid_kw, workdir=self.workdir
+        )
+        return rsigapi
+
+    def check(self, action='return'):
+        bbw, bbs, bbe, bbn = self.bbox
+        iswe = bbw < bbe
+        issn = bbs < bbn
+        isbe = self.bdate <= self.edate
+
+        if not iswe:
+            _actionf('West is East of East', action)
+        if not issn:
+            _actionf('South is North of North', action)
+        if not isbe:
+            _actionf('bdate is later than edate', action)
+
+        return iswe & issn & isbe
```

### Comparing `pyrsig-0.3.1/README.md` & `pyrsig-0.4.0/README.md`

 * *Files identical despite different names*

