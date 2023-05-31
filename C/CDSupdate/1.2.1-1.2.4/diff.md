# Comparing `tmp/CDSupdate-1.2.1.tar.gz` & `tmp/CDSupdate-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CDSupdate-1.2.1.tar", last modified: Mon May  8 10:03:39 2023, max compression
+gzip compressed data, was "CDSupdate-1.2.4.tar", last modified: Wed May 31 14:48:35 2023, max compression
```

## Comparing `CDSupdate-1.2.1.tar` & `CDSupdate-1.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.371984 CDSupdate-1.2.1/
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.366754 CDSupdate-1.2.1/CDSupdate/
--rw-r--r--   0 yrobin     (501) staff       (20)     9431 2023-05-08 10:02:58.000000 CDSupdate-1.2.1/CDSupdate/__CDSUParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     5131 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/__CVarsParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.2.1/CDSupdate/__curses_doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)     3744 2023-05-05 06:01:11.000000 CDSupdate-1.2.1/CDSupdate/__doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)      847 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/__exceptions.py
--rw-r--r--   0 yrobin     (501) staff       (20)     4268 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/__exec.py
--rw-r--r--   0 yrobin     (501) staff       (20)    12881 2023-05-08 10:02:58.000000 CDSupdate-1.2.1/CDSupdate/__extracvars.py
--rw-r--r--   0 yrobin     (501) staff       (20)      974 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)    14464 2023-05-03 12:54:20.000000 CDSupdate-1.2.1/CDSupdate/__io.py
--rw-r--r--   0 yrobin     (501) staff       (20)     1912 2023-05-08 10:02:58.000000 CDSupdate-1.2.1/CDSupdate/__release.py
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.371371 CDSupdate-1.2.1/CDSupdate/data/
--rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-dptas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)     2027 2023-05-08 10:02:58.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-name.csv
--rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-pr-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-ps-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-psl-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      858 2023-05-05 06:01:11.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-rlds-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)     1280 2023-05-05 06:01:11.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-rsds-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-tas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-uas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-vas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-zg-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      723 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.2.1/CDSupdate/data/areas.csv
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.367621 CDSupdate-1.2.1/CDSupdate.egg-info/
--rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)      935 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/SOURCES.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/dependency_links.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       42 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/requires.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/top_level.txt
--rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.2.1/LICENSE
--rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.2.1/MANIFEST.in
--rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-08 10:03:39.371833 CDSupdate-1.2.1/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)     1568 2023-05-04 08:04:46.000000 CDSupdate-1.2.1/README.md
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.371649 CDSupdate-1.2.1/scripts/
--rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/scripts/cdsupdate
--rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-08 10:03:39.372027 CDSupdate-1.2.1/setup.cfg
--rwxr-xr-x   0 yrobin     (501) staff       (20)     2417 2023-05-04 08:04:46.000000 CDSupdate-1.2.1/setup.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.986013 CDSupdate-1.2.4/
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.982017 CDSupdate-1.2.4/CDSupdate/
+-rw-r--r--   0 yrobin     (501) staff       (20)     9506 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__CDSUParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     5145 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__CVarsParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.2.4/CDSupdate/__curses_doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3744 2023-05-05 06:01:11.000000 CDSupdate-1.2.4/CDSupdate/__doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      969 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__exceptions.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4471 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__exec.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    16235 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__extracvars.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      988 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    14922 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__io.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1983 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__release.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.985525 CDSupdate-1.2.4/CDSupdate/data/
+-rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-dptas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     1918 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-name.csv
+-rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-pr-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-ps-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-psl-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      858 2023-05-05 06:01:11.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-rlds-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     1280 2023-05-05 06:01:11.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-rsds-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-tas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-uas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-vas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-zg-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      737 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/data/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.2.4/CDSupdate/data/areas.csv
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.983009 CDSupdate-1.2.4/CDSupdate.egg-info/
+-rw-r--r--   0 yrobin     (501) staff       (20)     2552 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)      935 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/SOURCES.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/dependency_links.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       42 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/requires.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/top_level.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.2.4/LICENSE
+-rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.2.4/MANIFEST.in
+-rw-r--r--   0 yrobin     (501) staff       (20)     2552 2023-05-31 14:48:35.985859 CDSupdate-1.2.4/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)     1753 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/README.md
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.985681 CDSupdate-1.2.4/scripts/
+-rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/scripts/cdsupdate
+-rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-31 14:48:35.986050 CDSupdate-1.2.4/setup.cfg
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     2431 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/setup.py
```

### Comparing `CDSupdate-1.2.1/CDSupdate/__CDSUParams.py` & `CDSupdate-1.2.4/CDSupdate/__CDSUParams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-## Copyright(c) 2023 Yoann Robin
+## Copyright(c) 2023 Yoann Robin, Andreia Hisi
 ## 
 ## This file is part of CDSupdate.
 ## 
 ## CDSupdate is free software: you can redistribute it and/or modify
 ## it under the terms of the GNU General Public License as published by
 ## the Free Software Foundation, either version 3 of the License, or
 ## (at your option) any later version.
@@ -32,14 +32,15 @@
 import dataclasses
 
 import numpy  as np
 import xarray as xr
 import pandas as pd
 
 from .__exceptions  import AbortForHelpException
+from .__exceptions  import  NoUserInputException
 
 from .__CVarsParams import CVarsParams
 from .__CVarsParams import cvarsParams
 
 
 ###############
 ## Variables ##
@@ -70,15 +71,21 @@
 	keep_hourly : bool                   = False
 	
 	cvarsParams  : CVarsParams   = cvarsParams
 	cdsApiParams : dict | None = None
 	
 	def init_from_user_input( self , *argv ):##{{{
 		
+		## In list
 		argv = list(argv)
+		
+		## Special case, no user input
+		if len(argv) == 0:
+			raise NoUserInputException
+		
 		## Special case of area
 		if "--area" in argv:
 			idx = argv.index("--area") + 1
 			if len(argv) > idx and argv[idx][0] == "-":
 				argv[idx] = " " + argv[idx]
 		
 		## Parser for user input
@@ -95,16 +102,14 @@
 		parser.add_argument( "--keep-hourly" , action = "store_const" , const = True , default = False )
 		
 		## Transform in dict
 		kwargs = vars(parser.parse_args(argv))
 		
 		## And store in the class
 		for key in kwargs:
-			if key not in self.__dict__:
-				raise Exception("Parameter not present in the class")
 			self.__dict__[key] = kwargs[key]
 			
 		
 	##}}}
 	
 	def init_tmp(self):##{{{
 		
@@ -170,19 +175,19 @@
 			## If help, stop
 			if self.help:
 				raise AbortForHelpException
 			
 			## Test of the output dir exist
 			if self.output_dir is None:
 				raise Exception("Output directory must be given!")
-			self.output_dir = os.path.split(self.output_dir)[0]
-			if not os.path.isdir(self.output_dir):
-				raise Exception( f"Output directory {self.output_dir} is not a path!" )
+			self.output_dir = os.path.abspath(self.output_dir)
 			if self.output_dir.split(os.path.sep)[-1] == "ERA5":
 				self.output_dir = os.path.sep.join( self.output_dir.split(os.path.sep)[:-1] )
+			if not os.path.isdir(self.output_dir):
+				raise Exception( f"Output directory {self.output_dir} is not a path!" )
 			
 			## Test if the tmp directory exists
 			if self.tmp is not None:
 				if not os.path.isdir(self.tmp):
 					raise Exception( f"The temporary directory {self.tmp} is given, but doesn't exists!" )
 			
 			## Now cvars
```

### Comparing `CDSupdate-1.2.1/CDSupdate/__CVarsParams.py` & `CDSupdate-1.2.4/CDSupdate/__CVarsParams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-## Copyright(c) 2022, 2023 Yoann Robin
+## Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 ## 
 ## This file is part of CDSupdate.
 ## 
 ## CDSupdate is free software: you can redistribute it and/or modify
 ## it under the terms of the GNU General Public License as published by
 ## the Free Software Foundation, either version 3 of the License, or
 ## (at your option) any later version.
```

### Comparing `CDSupdate-1.2.1/CDSupdate/__curses_doc.py` & `CDSupdate-1.2.4/CDSupdate/__curses_doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/__doc.py` & `CDSupdate-1.2.4/CDSupdate/__doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/__exceptions.py` & `CDSupdate-1.2.4/CDSupdate/__exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,12 +12,17 @@
 ## but WITHOUT ANY WARRANTY; without even the implied warranty of
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 ## 
 ## You should have received a copy of the GNU General Public License
 ## along with CDSupdate.  If not, see <https://www.gnu.org/licenses/>.
 
+
+class NoUserInputException(Exception):
+	def __init__( self , *args , **kwargs ):
+		super().__init__( *args , **kwargs )
+
 class AbortForHelpException(Exception):
 	def __init__( self , *args , **kwargs ):
 		super().__init__( *args , **kwargs )
```

### Comparing `CDSupdate-1.2.1/CDSupdate/__exec.py` & `CDSupdate-1.2.4/CDSupdate/__exec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-## Copyright(c) 2022, 2023 Yoann Robin
+## Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 ## 
 ## This file is part of CDSupdate.
 ## 
 ## CDSupdate is free software: you can redistribute it and/or modify
 ## it under the terms of the GNU General Public License as published by
 ## the Free Software Foundation, either version 3 of the License, or
 ## (at your option) any later version.
@@ -36,14 +36,15 @@
 ## Imports ##
 #############
 
 from .__CDSUParams import cdsuParams
 from .__release    import version
 
 from .__exceptions import AbortForHelpException
+from .__exceptions import NoUserInputException
 
 from .__io import load_data_CDS
 from .__io import BRUT_to_AMIP_format
 from .__io import merge_AMIP_CF_format
 from .__extracvars import build_EXTRA_cvars
 
 from .__curses_doc import print_doc
@@ -101,15 +102,20 @@
 	"""
 	
 	
 	## Time counter
 	walltime0 = dt.datetime.utcnow()
 	
 	## Read input
-	cdsuParams.init_from_user_input(*argv)
+	try:
+		cdsuParams.init_from_user_input(*argv)
+	except NoUserInputException as e:
+		print("No user input, abort!")
+		print("Read the documentation with 'cdsupdate --help'")
+		return
 	
 	## Init logs
 	cdsuParams.init_logging()
 	
 	## Logging
 	logger.info(cdsuParams.LINE)
 	logger.info( r"   ____ ____  ____                  _       _        " )
```

### Comparing `CDSupdate-1.2.1/CDSupdate/__extracvars.py` & `CDSupdate-1.2.4/CDSupdate/__extracvars.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,14 +43,36 @@
 logger.addHandler(logging.NullHandler())
 
 
 ###############
 ## Functions ##
 ###############
 
+## Temperature units conversion ##{{{
+
+def kelvin2celcius(T):
+	return T - 273.15
+
+def celcius2kelvin(T):
+	return T + 273.15
+
+def fahrenheit2celcius(T):
+	return (T - 32.) * 5. / 9.
+
+def celcius2fahrenheit(T):
+	return T * 9. / 5. + 32
+
+def fahrenheit2kelvin(T):
+	return celcius2kelvin( fahrenheit2celcius(T) )
+
+def kelvin2fahrenheit(T):
+	return celcius2fahrenheit( kelvin2celcius(T) )
+
+##}}}
+
 def build_sfcWind():##{{{
 	
 	area_name = cdsuParams.area_name
 	
 	## files
 	ipathu  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "uas" )
 	ipathv  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "vas" )
@@ -206,40 +228,38 @@
 		target = os.path.join( opath , ofile )
 		if not os.path.isdir(opath):
 			os.makedirs(opath)
 		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
 		odatad.to_netcdf( os.path.join( opath , ofile ) )
 ##}}}
 
-def build_heatIndex():##{{{
-	
-	cvar = "heatIndex"
+def _build_HI_method_blazejczyk():##{{{
+	cvar = "HI"
 	area_name = cdsuParams.area_name
 	
 	## files
 	cvar0   = "tas"
 	ipath0  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar0 )
 	ifiles0 = os.listdir(ipath0)
 	ifiles0.sort()
 	cvar1   = "hurs"
 	ipath1  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar1 )
 	ifiles1 = os.listdir(ipath1)
 	ifiles1.sort()
 	
-	
 	for ifile0,ifile1 in zip(ifiles0,ifiles1):
 		
 		idata0 = xr.open_dataset( os.path.join( ipath0 , ifile0 ) )
 		idata1 = xr.open_dataset( os.path.join( ipath1 , ifile1 ) )
 		
+		## Build hourly HI
+		odatah = idata0.copy( deep = True ).rename( { cvar0 : cvar } )
 		year  = idata0.time.dt.year[0].values
 		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata0.time.dt.dayofyear.values)]
 		
-		## Build hourly heatIndex
-		odatah = idata0.copy( deep = True ).rename( { cvar0 : cvar } )
 		c0     = -8.784695
 		c1     = 1.61139411
 		c2     = 2.338549
 		c3     = -0.14611605
 		c4     = -1.2308094e-2
 		c5     = -1.6424828e-2
 		c6     = 2.211732e-3
@@ -273,14 +293,103 @@
 		target = os.path.join( opath , ofile )
 		if not os.path.isdir(opath):
 			os.makedirs(opath)
 		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
 		odatad.to_netcdf( os.path.join( opath , ofile ) )
 ##}}}
 
+def _build_HI_method_noaa():##{{{
+	cvar = "HI"
+	area_name = cdsuParams.area_name
+	
+	## files
+	cvar0   = "tas"
+	ipath0  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar0 )
+	ifiles0 = os.listdir(ipath0)
+	ifiles0.sort()
+	cvar1   = "hurs"
+	ipath1  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar1 )
+	ifiles1 = os.listdir(ipath1)
+	ifiles1.sort()
+	
+	for ifile0,ifile1 in zip(ifiles0,ifiles1):
+		
+		idata0 = xr.open_dataset( os.path.join( ipath0 , ifile0 ) )
+		idata1 = xr.open_dataset( os.path.join( ipath1 , ifile1 ) )
+		
+		## Build hourly HI
+		odatah = idata0.copy( deep = True ).rename( { cvar0 : cvar } )
+		year  = idata0.time.dt.year[0].values
+		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata0.time.dt.dayofyear.values)]
+		
+		## Variables
+		T = kelvin2fahrenheit(idata0[cvar0])
+		H = idata1[cvar1].round(0)
+		
+		## Constants
+		c0 = -42.379
+		c1 =   2.04901523
+		c2 =  10.14333127
+		c3 =  -0.22475541
+		c4 =  -0.00683783
+		c5 =  -0.05481717
+		c6 =   0.00122874
+		c7 =   0.00085282
+		c8 =  -0.00000199
+		
+		## Heat Index
+		HI = c0 + c1 * T + c2 * H + c3 * T * H + c4 * T**2 + c5 * H**2 + c6 * T**2 * H + c7 * T * H**2 + c8 * T**2 * H**2
+		
+		## Correction for extremes
+		HIA1 = ( 13 - H ) /  4 * np.sqrt( ( 17 - np.abs( T - 95 ) ) / 17 )
+		HIA2 = ( H - 85 ) / 10 * ( ( 87 - T ) / 5 )
+		HIL  = 0.5 * ( T + 61 + 1.2 * (T - 68) + 0.094 * H )
+		
+		HI = HI.where( ~( ( H < 13. ) & (T > 80.) & (T < 112) ) , HI - HIA1 )
+		HI = HI.where( ~( ( H > 85. ) & (T > 80.) & (T <  87) ) , HI + HIA2 )
+		HI = HI.where( HIL > 80. , HIL )
+		
+		odatah[cvar] = fahrenheit2kelvin(HI)
+		
+		## Build daily
+		odatad = odatah.groupby("time.dayofyear").mean().rename( dayofyear = "time" ).assign_coords( time = dtime )
+		
+		## Save hourly
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
+		t0    = str(odatah.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatah.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvar}_hr_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/hr/{cvar}/{ofile}'" )
+		odatah.to_netcdf( os.path.join( opath , ofile ) )
+		
+		## Save daily
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
+		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
+		odatad.to_netcdf( os.path.join( opath , ofile ) )
+		
+##}}}
+
+def build_HI( method = "noaa" ):##{{{
+	
+	if method == "noaa":
+		_build_HI_method_noaa()
+	else:
+		_build_HI_method_blazejczyk()
+	
+##}}}
+
 def build_cvarmin( cvar ):##{{{
 	
 	cvarN = f"{cvar}min"
 	area_name = cdsuParams.area_name
 	
 	## files
 	ipath  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
@@ -355,13 +464,13 @@
 			build_cvarmax( cvar[:-3] )
 		if cvar == "sfcWind":
 			build_sfcWind()
 		if cvar == "hurs":
 			build_hurs()
 		if cvar == "huss":
 			build_huss()
-		if cvar == "heatIndex":
-			build_heatIndex()
+		if cvar == "HI":
+			build_HI()
 	
 ##}}}
```

### Comparing `CDSupdate-1.2.1/CDSupdate/__init__.py` & `CDSupdate-1.2.4/CDSupdate/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-## Copyright(c) 2022, 2023 Yoann Robin
+## Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 ## 
 ## This file is part of CDSupdate.
 ## 
 ## CDSupdate is free software: you can redistribute it and/or modify
 ## it under the terms of the GNU General Public License as published by
 ## the Free Software Foundation, either version 3 of the License, or
 ## (at your option) any later version.
```

### Comparing `CDSupdate-1.2.1/CDSupdate/__io.py` & `CDSupdate-1.2.4/CDSupdate/__io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-## Copyright(c) 2023 Yoann Robin
+## Copyright(c) 2023 Yoann Robin, Andreia Hisi
 ## 
 ## This file is part of CDSupdate.
 ## 
 ## CDSupdate is free software: you can redistribute it and/or modify
 ## it under the terms of the GNU General Public License as published by
 ## the Free Software Foundation, either version 3 of the License, or
 ## (at your option) any later version.
@@ -317,15 +317,15 @@
 			if len(cvarattrs[att]) == 0:
 				continue
 			if att == "long_name" and not (level == "single"):
 				ncv_cvar.setncattr( att , cvarattrs[att].replace("__CHANGE__",level) )
 			else:
 				ncv_cvar.setncattr( att , cvarattrs[att] )
 		
-		ncv_cvar.setncattr( "coordinates" , "height lat lon" )
+		ncv_cvar.setncattr( "coordinates" , "height" )
 		if level == "single":
 			ncv_height[:] = float(cdsuParams.cvarsParams.height(cvar))
 		else:
 			ncv_height[:] = float(level)
 		
 		## Add global attrs
 		gattrs = build_gattrs( cvar , level )
@@ -386,16 +386,20 @@
 				if ifileN is None:
 					continue
 				
 				## Case 2, new file, but no old data
 				if ifileO is None:
 					logger.info( f" * No old data to merge" )
 					idataN = xr.open_dataset( os.path.join( ipath , ifileN ) )
-					t0    = str(idataN.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
-					t1    = str(idataN.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
+					if freq == "hr":
+						t0    = str(idataN.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+						t1    = str(idataN.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+					else:
+						t0    = str(idataN.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
+						t1    = str(idataN.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
 					ofile  = f"ERA5_{cvar}_{freq}_{area_name}_{t0}-{t1}.nc"
 					logger.info( f" * Save '{ofile}'" )
 					save_netcdf( idataN , cvar , freq , os.path.join( opath , ofile ) )
 				
 				## Case 3, must merge the two files
 				if ifileO is not None and ifileN is not None:
 					logger.info( f" * Require merge" )
@@ -403,15 +407,19 @@
 					idataO = xr.open_dataset( os.path.join( opath , ifileO ) ).expand_dims("version").assign_coords( version = [0] )
 					idata  = xr.concat( [idataN,idataO] , dim = "version" )
 					idata  = idata.sel( version = 1 ).combine_first( idata.sel( version = 0 ) ).compute()
 					del idataN
 					del idataO
 					os.remove( os.path.join( opath , ifileO ) )
 					
-					t0    = str(idata.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
-					t1    = str(idata.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
+					if freq == "hr":
+						t0    = str(idataN.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+						t1    = str(idataN.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+					else:
+						t0    = str(idataN.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
+						t1    = str(idataN.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
 					ofile  = f"ERA5_{cvar}_{freq}_{area_name}_{t0}-{t1}.nc"
 					logger.info( f" * Save '{ofile}'" )
 					save_netcdf( idata , cvar , freq , os.path.join( opath , ofile ) )
 ##}}}
```

### Comparing `CDSupdate-1.2.1/CDSupdate/__release.py` & `CDSupdate-1.2.4/CDSupdate/__release.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-## Copyright(c) 2022, 2023 Yoann Robin
+## Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 ## 
 ## This file is part of CDSupdate.
 ## 
 ## CDSupdate is free software: you can redistribute it and/or modify
 ## it under the terms of the GNU General Public License as published by
 ## the Free Software Foundation, either version 3 of the License, or
 ## (at your option) any later version.
@@ -15,31 +15,31 @@
 ## 
 ## You should have received a copy of the GNU General Public License
 ## along with CDSupdate.  If not, see <https://www.gnu.org/licenses/>.
 
 
 version_major = "1"
 version_minor = "2"
-version_patch = "1"
+version_patch = "4"
 version_extra = ""
 version       = f"{version_major}.{version_minor}.{version_patch}{version_extra}"
 
 name = "CDSupdate"
 
 description = "Auto-updater of data from the Climate Data Store"
 
-authors       = ["Yoann Robin"]
-authors_email = ["yoann.robin.k@gmail.com"]
+authors       = ["Yoann Robin","Andreia Hisi"]
+authors_email = ["yoann.robin.k@gmail.com","andreia.hisi@lsce.ipsl.fr"]
 authors_doc   = ", ".join( [ f"{ath} ({athm})" for ath,athm in zip(authors,authors_email) ] )
 
 src_url = "https://github.com/yrobink/CDSupdate"
 
 license = "GNU-GPL3"
 license_txt = """\
-Copyright(c) 2022, 2023 Yoann Robin
+Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 
 This file is part of CDSupdate.
 
 CDSupdate is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-dptas-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-dptas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-pr-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-pr-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-ps-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-ps-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-psl-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-psl-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-rlds-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-rlds-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-rsds-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-rsds-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-uas-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-uas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-vas-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-vas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/ERA5-zg-description.txt` & `CDSupdate-1.2.4/CDSupdate/data/ERA5-zg-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/CDSupdate/data/__init__.py` & `CDSupdate-1.2.4/CDSupdate/data/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-## Copyright(c) 2022, 2023 Yoann Robin
+## Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 ## 
 ## This file is part of CDSupdate.
 ## 
 ## CDSupdate is free software: you can redistribute it and/or modify
 ## it under the terms of the GNU General Public License as published by
 ## the Free Software Foundation, either version 3 of the License, or
 ## (at your option) any later version.
```

### Comparing `CDSupdate-1.2.1/CDSupdate.egg-info/PKG-INFO` & `CDSupdate-1.2.4/CDSupdate.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.2.1
+Version: 1.2.4
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
-Author: Yoann Robin
-Author-email: yoann.robin.k@gmail.com
+Author: Yoann Robin, Andreia Hisi
+Author-email: yoann.robin.k@gmail.com, andreia.hisi@lsce.ipsl.fr
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
 Platform: macosx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -42,14 +42,16 @@
 ~~~shell
 pip3 install CDSupdate
 ~~~
 
 Or from source:
 
 ~~~shell
+git clone https://github.com/yrobink/CDSupdate.git
+cd CDSupdaye
 pip3 install .
 ~~~
 
 This adds the `CDSupdate` package in your python installation, and the command
 `cdsupdate`.
 
 ## How to use ?
@@ -63,18 +65,21 @@
 As example, to download the daily mean temperature over the North Atlantic
 (80W-50E,5N,72N) between 2019-11-09 and 2022-01-17 in the directory `odir`, just run:
 
 ~~~shell
 cdsupdate --log info test.log --period 2019-11-09/2022-01-17 --cvar tas --area NorthAtlantic --odir odir
 ~~~
 
+## How to cite it ?
+
+You can use this [DOI:10.5281/zenodo.7991332](https://doi.org/10.5281/zenodo.7991332)
 
 ## License
 
-Copyright(c) 2022, 2023 Yoann Robin
+Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 
 This file is part of CDSupdate.
 
 CDSupdate is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `CDSupdate-1.2.1/CDSupdate.egg-info/SOURCES.txt` & `CDSupdate-1.2.4/CDSupdate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/LICENSE` & `CDSupdate-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/PKG-INFO` & `CDSupdate-1.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.2.1
+Version: 1.2.4
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
-Author: Yoann Robin
-Author-email: yoann.robin.k@gmail.com
+Author: Yoann Robin, Andreia Hisi
+Author-email: yoann.robin.k@gmail.com, andreia.hisi@lsce.ipsl.fr
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
 Platform: macosx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -42,14 +42,16 @@
 ~~~shell
 pip3 install CDSupdate
 ~~~
 
 Or from source:
 
 ~~~shell
+git clone https://github.com/yrobink/CDSupdate.git
+cd CDSupdaye
 pip3 install .
 ~~~
 
 This adds the `CDSupdate` package in your python installation, and the command
 `cdsupdate`.
 
 ## How to use ?
@@ -63,18 +65,21 @@
 As example, to download the daily mean temperature over the North Atlantic
 (80W-50E,5N,72N) between 2019-11-09 and 2022-01-17 in the directory `odir`, just run:
 
 ~~~shell
 cdsupdate --log info test.log --period 2019-11-09/2022-01-17 --cvar tas --area NorthAtlantic --odir odir
 ~~~
 
+## How to cite it ?
+
+You can use this [DOI:10.5281/zenodo.7991332](https://doi.org/10.5281/zenodo.7991332)
 
 ## License
 
-Copyright(c) 2022, 2023 Yoann Robin
+Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 
 This file is part of CDSupdate.
 
 CDSupdate is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `CDSupdate-1.2.1/README.md` & `CDSupdate-1.2.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 ~~~shell
 pip3 install CDSupdate
 ~~~
 
 Or from source:
 
 ~~~shell
+git clone https://github.com/yrobink/CDSupdate.git
+cd CDSupdaye
 pip3 install .
 ~~~
 
 This adds the `CDSupdate` package in your python installation, and the command
 `cdsupdate`.
 
 ## How to use ?
@@ -42,18 +44,21 @@
 As example, to download the daily mean temperature over the North Atlantic
 (80W-50E,5N,72N) between 2019-11-09 and 2022-01-17 in the directory `odir`, just run:
 
 ~~~shell
 cdsupdate --log info test.log --period 2019-11-09/2022-01-17 --cvar tas --area NorthAtlantic --odir odir
 ~~~
 
+## How to cite it ?
+
+You can use this [DOI:10.5281/zenodo.7991332](https://doi.org/10.5281/zenodo.7991332)
 
 ## License
 
-Copyright(c) 2022, 2023 Yoann Robin
+Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 
 This file is part of CDSupdate.
 
 CDSupdate is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
```

### Comparing `CDSupdate-1.2.1/scripts/cdsupdate` & `CDSupdate-1.2.4/scripts/cdsupdate`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.1/setup.py` & `CDSupdate-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-## Copyright(c) 2022, 2023 Yoann Robin
+## Copyright(c) 2022, 2023 Yoann Robin, Andreia Hisi
 ## 
 ## This file is part of CDSupdate.
 ## 
 ## CDSupdate is free software: you can redistribute it and/or modify
 ## it under the terms of the GNU General Public License as published by
 ## the Free Software Foundation, either version 3 of the License, or
 ## (at your option) any later version.
```

