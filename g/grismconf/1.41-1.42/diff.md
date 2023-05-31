# Comparing `tmp/grismconf-1.41.tar.gz` & `tmp/grismconf-1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grismconf-1.41.tar", last modified: Mon May  8 18:18:46 2023, max compression
+gzip compressed data, was "grismconf-1.42.tar", last modified: Wed May 31 13:21:26 2023, max compression
```

## Comparing `grismconf-1.41.tar` & `grismconf-1.42.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 npirzkal   (501) staff       (20)        0 2023-05-08 18:18:46.978433 grismconf-1.41/
--rw-r--r--   0 npirzkal   (501) staff       (20)      368 2023-05-08 18:18:46.977897 grismconf-1.41/PKG-INFO
--rw-r--r--   0 npirzkal   (501) staff       (20)     2553 2020-05-14 03:46:06.000000 grismconf-1.41/README.md
--rw-------   0 npirzkal   (501) staff       (20)   167467 2016-10-12 16:12:10.000000 grismconf-1.41/Updated_GRISM_Configuration.pdf
-drwxr-xr-x   0 npirzkal   (501) staff       (20)        0 2023-05-08 18:18:46.974561 grismconf-1.41/grismconf/
--rw-------   0 npirzkal   (501) staff       (20)       72 2023-05-08 18:18:39.000000 grismconf-1.41/grismconf/__init__.py
--rw-------   0 npirzkal   (501) staff       (20)    21405 2023-05-08 18:06:43.000000 grismconf-1.41/grismconf/grismconf.py
--rw-------   0 npirzkal   (501) staff       (20)     4854 2020-11-02 22:16:37.000000 grismconf-1.41/grismconf/poly.py
-drwxr-xr-x   0 npirzkal   (501) staff       (20)        0 2023-05-08 18:18:46.976931 grismconf-1.41/grismconf.egg-info/
--rw-------   0 npirzkal   (501) staff       (20)      368 2023-05-08 18:18:46.000000 grismconf-1.41/grismconf.egg-info/PKG-INFO
--rw-------   0 npirzkal   (501) staff       (20)      245 2023-05-08 18:18:46.000000 grismconf-1.41/grismconf.egg-info/SOURCES.txt
--rw-------   0 npirzkal   (501) staff       (20)        1 2023-05-08 18:18:46.000000 grismconf-1.41/grismconf.egg-info/dependency_links.txt
--rw-------   0 npirzkal   (501) staff       (20)       10 2023-05-08 18:18:46.000000 grismconf-1.41/grismconf.egg-info/top_level.txt
--rw-r--r--   0 npirzkal   (501) staff       (20)       38 2023-05-08 18:18:46.978611 grismconf-1.41/setup.cfg
--rw-------   0 npirzkal   (501) staff       (20)      843 2023-05-08 18:18:23.000000 grismconf-1.41/setup.py
+drwxr-xr-x   0 npirzkal   (501) staff       (20)        0 2023-05-31 13:21:26.000000 grismconf-1.42/
+-rw-r--r--   0 npirzkal   (501) staff       (20)      368 2023-05-31 13:21:26.000000 grismconf-1.42/PKG-INFO
+-rw-r--r--   0 npirzkal   (501) staff       (20)     2553 2020-05-14 03:46:07.000000 grismconf-1.42/README.md
+-rw-r--r--   0 npirzkal   (501) staff       (20)   167467 2016-10-12 16:12:10.000000 grismconf-1.42/Updated_GRISM_Configuration.pdf
+drwxr-xr-x   0 npirzkal   (501) staff       (20)        0 2023-05-31 13:21:26.000000 grismconf-1.42/grismconf/
+-rw-r--r--   0 npirzkal   (501) staff       (20)       72 2023-05-31 13:20:11.000000 grismconf-1.42/grismconf/__init__.py
+-rw-r--r--   0 npirzkal   (501) staff       (20)    21444 2023-05-31 13:19:46.000000 grismconf-1.42/grismconf/grismconf.py
+-rw-r--r--   0 npirzkal   (501) staff       (20)     4854 2020-11-02 22:16:38.000000 grismconf-1.42/grismconf/poly.py
+drwxr-xr-x   0 npirzkal   (501) staff       (20)        0 2023-05-31 13:21:26.000000 grismconf-1.42/grismconf.egg-info/
+-rw-r--r--   0 npirzkal   (501) staff       (20)      368 2023-05-31 13:21:26.000000 grismconf-1.42/grismconf.egg-info/PKG-INFO
+-rw-r--r--   0 npirzkal   (501) staff       (20)      245 2023-05-31 13:21:26.000000 grismconf-1.42/grismconf.egg-info/SOURCES.txt
+-rw-r--r--   0 npirzkal   (501) staff       (20)        1 2023-05-31 13:21:26.000000 grismconf-1.42/grismconf.egg-info/dependency_links.txt
+-rw-r--r--   0 npirzkal   (501) staff       (20)       10 2023-05-31 13:21:26.000000 grismconf-1.42/grismconf.egg-info/top_level.txt
+-rw-r--r--   0 npirzkal   (501) staff       (20)       38 2023-05-31 13:21:26.000000 grismconf-1.42/setup.cfg
+-rw-r--r--   0 npirzkal   (501) staff       (20)      843 2023-05-31 13:20:22.000000 grismconf-1.42/setup.py
```

### Comparing `grismconf-1.41/README.md` & `grismconf-1.42/README.md`

 * *Files identical despite different names*

### Comparing `grismconf-1.41/Updated_GRISM_Configuration.pdf` & `grismconf-1.42/Updated_GRISM_Configuration.pdf`

 * *Files identical despite different names*

### Comparing `grismconf-1.41/grismconf/grismconf.py` & `grismconf-1.42/grismconf/grismconf.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,16 +113,17 @@
             pass
 
         try:
             self.POMY = np.array(self._get_value("POMY")).astype(float)
         except:
             pass
 
+        print(self.POMX)
         if self.POMX is not None and self.POMY is not None:
-            if np.isfinite(self.POMX) and np.isfinite(self.POMY):
+            if np.isfinite(self.POMX).all() and np.isfinite(self.POMY).all():
                 self.POM_POLYGON = np.array([self.POMX,self.POMY]).transpose()
 
         # Load the name of a dispersed background model file
         self.BCK = None
         try:
             self.BCK = os.path.join(self.GRISM_CONF_PATH,self._get_value("BACKGROUND"))
         except:
@@ -196,17 +197,17 @@
         rot = np.dot(np.array([dx-origin[0], dy-origin[1]]).T, _mat)
         dxr = rot[:,0]+origin[0]
         dyr = rot[:,1]+origin[1]
         return dxr, dyr
 
     def is_inside_POM(self,order,xs,ys,XRANGE=False):
         """Check if points xs,ys are within the POM. Uses self.POM_POLYGON is availanle, otherwise XRANGE,YRANGE"""
-        print("is_inside:",self.POM_POLYGON)
+        #print("is_inside:",self.POM_POLYGON)
         if self.POM_POLYGON is not None and XRANGE is not True:
-            print("use polygon")
+            #print("use polygon")
             import matplotlib.path as mpltPath
             points = np.array([xs,ys]).transpose()
             path = mpltPath.Path(self.POM_POLYGON)
             ok = path.contains_points(points)
             return ok
         if self.XRANGE[order] is not None and self.YRANGE[order] is not None:
             #print("use xrange")
```

### Comparing `grismconf-1.41/grismconf/poly.py` & `grismconf-1.42/grismconf/poly.py`

 * *Files identical despite different names*

### Comparing `grismconf-1.41/setup.py` & `grismconf-1.42/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
 	name='grismconf',
-	version='1.41',
+	version='1.42',
 	description='GRISM Configuration python code, described in ISR 2017-01: A More Generalized Coordinate Transformation Approach for Grisms, Pirzkal & Ryan 2017 http://www.stsci.edu/hst/wfc3/documents/ISRs/WFC3-2017-01.pdf',
 	url='https://github.com/npirzkal/GRISMCONF',
 	author='Nor Pirzkal',
 	author_email='npirzkal@mac.com',
     package_dir = {
         'grismconf': 'grismconf',
         },
```

