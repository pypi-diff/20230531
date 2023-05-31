# Comparing `tmp/bioumlsim-0.4.1.tar.gz` & `tmp/bioumlsim-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.4.1.tar", last modified: Tue May 30 09:22:49 2023, max compression
+gzip compressed data, was "bioumlsim-0.4.2.tar", last modified: Wed May 31 12:22:05 2023, max compression
```

## Comparing `bioumlsim-0.4.1.tar` & `bioumlsim-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:22:49.861918 bioumlsim-0.4.1/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.4.1/LICENSE
--rw-rw-rw-   0        0        0      771 2023-05-30 09:22:49.862916 bioumlsim-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 09:22:49.776742 bioumlsim-0.4.1/bioumlsim/
--rw-rw-rw-   0        0        0     2348 2023-05-30 09:21:29.000000 bioumlsim-0.4.1/bioumlsim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:22:49.858917 bioumlsim-0.4.1/bioumlsim/jars/
--rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
--rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
--rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/biouml.workbench_0.9.10.jar
--rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/colt.jar
--rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
--rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.4.1/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
--rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
--rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
--rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.4.1/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
--rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/org.apache.velocity_1.6.2.jar
--rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.4.1/bioumlsim/jars/org.json-20170516.jar
--rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
--rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
--rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
--rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
--rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
--rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
--rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/src.jar
--rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.4.1/bioumlsim/jars/streamex-0.7.0.jar
--rw-rw-rw-   0        0        0      323 2023-05-30 05:53:42.000000 bioumlsim-0.4.1/bioumlsim/test.py
--rw-rw-rw-   0        0        0     1496 2023-05-30 07:46:26.000000 bioumlsim-0.4.1/bioumlsim/test.xml
-drwxrwxrwx   0        0        0        0 2023-05-30 09:22:49.802368 bioumlsim-0.4.1/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-05-30 09:22:49.000000 bioumlsim-0.4.1/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-05-30 09:22:49.000000 bioumlsim-0.4.1/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:22:49.000000 bioumlsim-0.4.1/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 09:12:26.000000 bioumlsim-0.4.1/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-05-30 09:22:49.000000 bioumlsim-0.4.1/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 09:22:49.000000 bioumlsim-0.4.1/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      895 2023-05-30 09:22:49.874962 bioumlsim-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 12:22:05.582103 bioumlsim-0.4.2/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-05-31 12:22:05.582103 bioumlsim-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 12:22:05.491844 bioumlsim-0.4.2/bioumlsim/
+-rw-rw-rw-   0        0        0     2437 2023-05-31 12:06:12.000000 bioumlsim-0.4.2/bioumlsim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:22:05.580090 bioumlsim-0.4.2/bioumlsim/jars/
+-rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
+-rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
+-rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/biouml.workbench_0.9.10.jar
+-rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/colt.jar
+-rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
+-rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.4.2/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
+-rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
+-rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
+-rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.4.2/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
+-rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/org.apache.velocity_1.6.2.jar
+-rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.4.2/bioumlsim/jars/org.json-20170516.jar
+-rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
+-rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
+-rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
+-rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
+-rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
+-rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
+-rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/src.jar
+-rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.4.2/bioumlsim/jars/streamex-0.7.0.jar
+-rw-rw-rw-   0        0        0      323 2023-05-30 05:53:42.000000 bioumlsim-0.4.2/bioumlsim/test.py
+-rw-rw-rw-   0        0        0     1496 2023-05-30 07:46:26.000000 bioumlsim-0.4.2/bioumlsim/test.xml
+drwxrwxrwx   0        0        0        0 2023-05-31 12:22:05.523089 bioumlsim-0.4.2/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-05-31 12:22:05.000000 bioumlsim-0.4.2/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2023-05-31 12:22:05.000000 bioumlsim-0.4.2/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:22:05.000000 bioumlsim-0.4.2/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-31 12:22:04.000000 bioumlsim-0.4.2/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-05-31 12:22:05.000000 bioumlsim-0.4.2/bioumlsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 12:22:05.000000 bioumlsim-0.4.2/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0      895 2023-05-31 12:22:05.595743 bioumlsim-0.4.2/setup.cfg
```

### Comparing `bioumlsim-0.4.1/LICENSE` & `bioumlsim-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/PKG-INFO` & `bioumlsim-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.4.1/bioumlsim/__init__.py` & `bioumlsim-0.4.2/bioumlsim/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 
     def __init__(self):
         path = os.path.dirname(__file__)+'/jars'
         self.bioUMLPath = path
         print("JVM is starting up")
         jpype.startJVM(classpath=[path+'/*'], convertStrings=True)
         
-    def load(self, file):
+    def load(self, file, verbose = False):
         """
         Loads SBML file and transforms it into object which represents mathematical model.
         Args:
             file (str): path to file
         Returns:
             model
         """
-        print(f"SBML file is loading: {file}")
+        if (verbose):
+             print(f"SBML file is loading: {file}")
         diagram = jpype.JClass("biouml.plugins.sbml.SbmlModelFactory").readDiagram(file, False)
         self.engine = jpype.JClass("biouml.plugins.simulation.java.JavaSimulationEngine")()
         self.engine.setDiagram(diagram)
         self.engine.setClassPath(self.bioUMLPath +'/src.jar')
         self.engine.disableLog()
         self.engine.setAbsTolerance(self.atol)
         self.engine.setRelTolerance(self.rtol)
@@ -46,24 +47,25 @@
          
 class Model:
     
     def __init__(self, engine, model):
         self.engine = engine
         self.model = model
         
-    def simulate(self, tend, numpoints):
+    def simulate(self, tend, numpoints, verbose = False):
         """
         Simulates SBML model and returns results.
         Args:
             tend: final time for simulation
             numpoints: number of time points
         Returns:
             simulation results
         """
-        print(f"Simulating model: {self.engine.getDiagram().getName()}")
+        if (verbose):
+            print(f"Simulating model: {self.engine.getDiagram().getName()}")
         self.engine.setCompletionTime(tend)
         self.engine.setTimeIncrement(tend / numpoints)
         result = self.engine.simulateSimple(self.model)
         species = self.engine.getFloatingSpecies()
         values = np.array(result.getValuesTransposed(species))
         names = np.array(species)
         times = np.array(result.getTimes());
```

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar` & `bioumlsim-0.4.2/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar` & `bioumlsim-0.4.2/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/biouml.workbench_0.9.10.jar` & `bioumlsim-0.4.2/bioumlsim/jars/biouml.workbench_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/colt.jar` & `bioumlsim-0.4.2/bioumlsim/jars/colt.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar` & `bioumlsim-0.4.2/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar` & `bioumlsim-0.4.2/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar` & `bioumlsim-0.4.2/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar` & `bioumlsim-0.4.2/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar` & `bioumlsim-0.4.2/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/org.apache.velocity_1.6.2.jar` & `bioumlsim-0.4.2/bioumlsim/jars/org.apache.velocity_1.6.2.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/org.json-20170516.jar` & `bioumlsim-0.4.2/bioumlsim/jars/org.json-20170516.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.access_0.9.10.jar` & `bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.access_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar` & `bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar` & `bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar` & `bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar` & `bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/ru.biosoft.math_0.9.10.jar` & `bioumlsim-0.4.2/bioumlsim/jars/ru.biosoft.math_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/src.jar` & `bioumlsim-0.4.2/bioumlsim/jars/src.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/jars/streamex-0.7.0.jar` & `bioumlsim-0.4.2/bioumlsim/jars/streamex-0.7.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim/test.xml` & `bioumlsim-0.4.2/bioumlsim/test.xml`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.4.2/bioumlsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.4.1/bioumlsim.egg-info/SOURCES.txt` & `bioumlsim-0.4.2/bioumlsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.4.1/setup.cfg` & `bioumlsim-0.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696f 756d 6c73 696d 0d0a 7665   = bioumlsim..ve
-00000020: 7273 696f 6e20 3d20 302e 342e 310d 0a61  rsion = 0.4.1..a
+00000020: 7273 696f 6e20 3d20 302e 342e 320d 0a61  rsion = 0.4.2..a
 00000030: 7574 686f 7220 3d20 496c 7961 204b 6973  uthor = Ilya Kis
 00000040: 656c 6576 2c20 4269 6f73 6f66 742e 7275  elev, Biosoft.ru
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2034 7833 6375 7430 7240 676d 6169 6c2e   4x3cut0r@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2050 7974 686f 6e20 696e 7465 7266   = Python interf
 00000090: 6163 6520 666f 7220 7369 6d75 6c61 7469  ace for simulati
```

