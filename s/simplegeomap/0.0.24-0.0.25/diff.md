# Comparing `tmp/simplegeomap-0.0.24.tar.gz` & `tmp/simplegeomap-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplegeomap-0.0.24.tar", last modified: Tue May 30 13:07:03 2023, max compression
+gzip compressed data, was "dist/simplegeomap-0.0.25.tar", last modified: Wed May 31 05:51:12 2023, max compression
```

## Comparing `simplegeomap-0.0.24.tar` & `simplegeomap-0.0.25.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.24/README.md
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/simplegeomap.egg-info/
--rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/simplegeomap.egg-info/dependency_links.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/simplegeomap.egg-info/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/simplegeomap.egg-info/top_level.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/simplegeomap.egg-info/requires.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/simplegeomap.egg-info/SOURCES.txt
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/simplegeomap/
--rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.24/simplegeomap/__init__.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     6774 2023-05-30 12:14:00.000000 simplegeomap-0.0.24/simplegeomap/simplegeomap.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     5459 2023-05-30 12:11:42.000000 simplegeomap-0.0.24/simplegeomap/util.py
--rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-05-30 13:05:28.000000 simplegeomap-0.0.24/setup.py
--rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-05-30 13:07:03.000000 simplegeomap-0.0.24/setup.cfg
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.25/README.md
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/simplegeomap.egg-info/
+-rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/simplegeomap.egg-info/dependency_links.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/simplegeomap.egg-info/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/simplegeomap.egg-info/top_level.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/simplegeomap.egg-info/requires.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/simplegeomap.egg-info/SOURCES.txt
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/simplegeomap/
+-rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.25/simplegeomap/__init__.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     6776 2023-05-30 14:07:40.000000 simplegeomap-0.0.25/simplegeomap/simplegeomap.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     5459 2023-05-30 12:11:42.000000 simplegeomap-0.0.25/simplegeomap/util.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-05-30 14:10:17.000000 simplegeomap-0.0.25/setup.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-05-31 05:51:12.000000 simplegeomap-0.0.25/setup.cfg
```

### Comparing `simplegeomap-0.0.24/PKG-INFO` & `simplegeomap-0.0.25/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.24
+Version: 0.0.25
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.24/README.md` & `simplegeomap-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.24/simplegeomap.egg-info/PKG-INFO` & `simplegeomap-0.0.25/simplegeomap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.24
+Version: 0.0.25
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.24/simplegeomap/simplegeomap.py` & `simplegeomap-0.0.25/simplegeomap/simplegeomap.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     ridx = np.random.choice(range(len(interpx)), size=8*1000, replace=False)
 
     interpx = interpx[ridx]
     interpy = interpy[ridx]
     interpz = interpz[ridx]
 
     q = QuadTreeInterpolator(interpx, interpy, interpz)
-    interp = np.vectorize(q.interpolate,otypes=[np.float])
+    interp = np.vectorize(q.interpolate,otypes=[np.float64])
 
     newx,newy = np.meshgrid(glon,glat)
     newz = interp(newx,newy)
     if not levels:
         CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=[500,1000,1500,2000,3000])
     else:
         CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=levels)
```

### Comparing `simplegeomap-0.0.24/simplegeomap/util.py` & `simplegeomap-0.0.25/simplegeomap/util.py`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.24/setup.py` & `simplegeomap-0.0.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 readme=open("README.md").read()
 
 setuptools.setup(
     name='simplegeomap',    
-    version='0.0.24',
+    version='0.0.25',
     description="Simple offline map plot utility, for country borders, elevation, water",
     long_description=readme,
     long_description_content_type="text/markdown",    
     install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','scipy','zarr'],
     include_package_data=True,
     url="https://github.com/burakbayramli/simplegeomap",
     author="Burak Bayramli",
```

