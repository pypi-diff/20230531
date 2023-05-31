# Comparing `tmp/bihc-0.0.8.0.tar.gz` & `tmp/bihc-0.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bihc-0.0.8.0.tar", last modified: Tue May 16 17:05:03 2023, max compression
+gzip compressed data, was "/home/edelafue/BIHC/dist/.tmp-ezemyt_h/bihc-0.0.8.1.tar", last modified: Wed May 31 14:43:34 2023, max compression
```

## Comparing `bihc-0.0.8.0.tar` & `bihc-0.0.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-16 17:05:03.948450 bihc-0.0.8.0/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      760 2023-05-04 17:43:24.000000 bihc-0.0.8.0/LICENSE
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      105 2023-05-04 17:43:24.000000 bihc-0.0.8.0/MANIFEST.in
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-16 17:05:03.941222 bihc-0.0.8.0/PKG-INFO
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     2686 2023-05-04 17:43:24.000000 bihc-0.0.8.0/README.md
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-16 17:05:03.496882 bihc-0.0.8.0/bihc/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      172 2023-05-04 17:43:24.000000 bihc-0.0.8.0/bihc/__init__.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)    27391 2023-05-16 11:07:39.000000 bihc-0.0.8.0/bihc/beam.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     6330 2023-05-16 13:35:53.000000 bihc-0.0.8.0/bihc/impedance.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     9072 2023-05-04 17:43:24.000000 bihc-0.0.8.0/bihc/plot.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     4157 2023-05-04 17:43:24.000000 bihc-0.0.8.0/bihc/power.py
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-16 17:05:03.753240 bihc-0.0.8.0/bihc.egg-info/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/PKG-INFO
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      334 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/SOURCES.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        1 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/dependency_links.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       23 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/requires.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        5 2023-05-16 17:05:02.000000 bihc-0.0.8.0/bihc.egg-info/top_level.txt
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)      128 2023-05-04 17:43:25.000000 bihc-0.0.8.0/pyproject.toml
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)       38 2023-05-16 17:05:03.950495 bihc-0.0.8.0/setup.cfg
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1082 2023-05-16 17:02:58.000000 bihc-0.0.8.0/setup.py
-drwxrwxrwx   0 edelafue  (1000) edelafue  (1000)        0 2023-05-16 17:05:03.865760 bihc-0.0.8.0/tests/
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     1886 2023-05-04 17:43:26.000000 bihc-0.0.8.0/tests/test_analyticBunchShapes.py
--rwxrwxrwx   0 edelafue  (1000) edelafue  (1000)     3008 2023-05-04 17:43:26.000000 bihc-0.0.8.0/tests/test_numericBunchShapes.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-05-31 14:43:34.000000 bihc-0.0.8.1/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      760 2022-12-08 10:22:14.000000 bihc-0.0.8.1/LICENSE
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      105 2022-12-08 10:22:14.000000 bihc-0.0.8.1/MANIFEST.in
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-31 14:43:34.000000 bihc-0.0.8.1/PKG-INFO
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     2686 2023-01-20 08:26:47.000000 bihc-0.0.8.1/README.md
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      172 2023-03-28 09:04:32.000000 bihc-0.0.8.1/bihc/__init__.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)    28294 2023-05-31 14:41:18.000000 bihc-0.0.8.1/bihc/beam.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     6330 2023-05-19 11:33:18.000000 bihc-0.0.8.1/bihc/impedance.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     9085 2023-05-31 14:26:46.000000 bihc-0.0.8.1/bihc/plot.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     4157 2023-03-08 15:02:48.000000 bihc-0.0.8.1/bihc/power.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/PKG-INFO
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      334 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/SOURCES.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        1 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/dependency_links.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       23 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/requires.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        5 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/top_level.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      128 2022-12-16 15:42:39.000000 bihc-0.0.8.1/pyproject.toml
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       38 2023-05-31 14:43:34.000000 bihc-0.0.8.1/setup.cfg
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1082 2023-05-31 14:42:25.000000 bihc-0.0.8.1/setup.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-05-31 14:43:34.000000 bihc-0.0.8.1/tests/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1886 2023-03-23 17:54:24.000000 bihc-0.0.8.1/tests/test_analyticBunchShapes.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3008 2023-03-23 17:41:58.000000 bihc-0.0.8.1/tests/test_numericBunchShapes.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `bihc-0.0.8.0/LICENSE` & `bihc-0.0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.0/PKG-INFO` & `bihc-0.0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.8.0
+Version: 0.0.8.1
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.8.0/README.md` & `bihc-0.0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.0/bihc/beam.py` & `bihc-0.0.8.1/bihc/beam.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,20 +580,44 @@
         For more information check the tool documentation:
         https://lpc.web.cern.ch/schemeEditor.html
         '''
         import csv
 
         self.isATimberFill = False
         self._fillingScheme = np.zeros(self.M, dtype=bool)
+        francesco_style = False 
 
         with open(self._beamFile) as f:
             data = csv.reader(f)
-            for row in data:
-                if row[0]: #avoid empty rows
-                    self._fillingScheme[int((int(row[0])-1)/10)] = True
+
+            for i, row in enumerate(data):
+                if i == 0:
+                    if row[0].isdigit():  #reading francesco modified files
+                        francesco_style = True
+                        break
+                else:
+                     break
+
+            if francesco_style:
+                for row in data:
+                    if row[0]: #avoid empty rows
+                        self._fillingScheme[int((int(row[0])-1)/10)] = True #Takes only beam 1
+
+            else: #reading files from LPC web format
+                start_line = False
+                for i, row in enumerate(data):
+                    if 'B1 bucket number' in row:
+                        start_line = True
+                        continue
+
+                    if start_line:
+                        try:
+                            self._fillingScheme[int((int(row[0])-1)/10)] = True #we take beam one
+                        except: #this breaks when an empty cell is reached
+                            break
 
         self._bunchLength[self._fillingScheme]=self.BUNCH_LENGTH_GLOBAL  #std vector of a single turn in the machine
         self.phi=np.ones(self.M)*self.PHI_GLOBAL
 
         self._setBunches()
 
     def setCustomBeamWithFillingScheme(self):
```

### Comparing `bihc-0.0.8.0/bihc/impedance.py` & `bihc-0.0.8.1/bihc/impedance.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.0/bihc/plot.py` & `bihc-0.0.8.1/bihc/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,26 +212,27 @@
         f=f[mask3]
         S=S[mask3]   
         Zreal=Zreal[mask3]
         Zf=f
 
         plt.figure()
         #spectrum
-        plt.plot(f/1e9,S,label='Spectrum')
+        plt.plot(f/1e9,S, color='r', label='Spectrum')
         ax = plt.gca()
         plt.xlim(0,self.fmax/1e9)
         plt.ylim(0,)
         plt.tick_params(axis='both', which='major')
         plt.xlabel("frequency [GHz]")
         plt.ylabel("Normalized Spectrum [a.u.]")
         plt.grid(True, color='gray', linestyle=':')
         plt.legend()
+
         #impedance
         axx = ax.twinx()
-        axx.plot(f/1e9,Zreal, color='r', label='Impedance')
+        axx.plot(f/1e9,Zreal, color='k', label='Impedance')
         axx.set_ylabel('Impedance [$\Omega$]')
         plt.show()
 
     def plotCollide(beam1, beam2):
         
         [t1,s1]=beam1.longitudinalProfile
         [t2,s2]=beam2.longitudinalProfile
```

### Comparing `bihc-0.0.8.0/bihc/power.py` & `bihc-0.0.8.1/bihc/power.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.0/bihc.egg-info/PKG-INFO` & `bihc-0.0.8.1/bihc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.8.0
+Version: 0.0.8.1
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.8.0/setup.py` & `bihc-0.0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name="bihc",
-    version="0.0.8.0",
+    version="0.0.8.1",
     description="BIHC: Beam-Induced Heating Computation package",
     author="Francesco Giordano",
     author_email="benoit.salvant@cern.ch", 
     packages=['bihc'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LeonardoSito/BIHC",
```

### Comparing `bihc-0.0.8.0/tests/test_analyticBunchShapes.py` & `bihc-0.0.8.1/tests/test_analyticBunchShapes.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.0/tests/test_numericBunchShapes.py` & `bihc-0.0.8.1/tests/test_numericBunchShapes.py`

 * *Files identical despite different names*

