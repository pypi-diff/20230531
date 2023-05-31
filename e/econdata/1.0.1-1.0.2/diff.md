# Comparing `tmp/econdata-1.0.1.tar.gz` & `tmp/econdata-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econdata-1.0.1.tar", last modified: Mon Apr 17 03:29:58 2023, max compression
+gzip compressed data, was "econdata-1.0.2.tar", last modified: Wed May 31 03:02:46 2023, max compression
```

## Comparing `econdata-1.0.1.tar` & `econdata-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 03:29:58.819703 econdata-1.0.1/
--rw-rw-rw-   0        0        0     1781 2023-04-17 03:29:58.818712 econdata-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1303 2023-04-17 03:22:50.000000 econdata-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 03:29:58.819703 econdata-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-04-17 03:23:35.000000 econdata-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:29:58.790780 econdata-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 03:29:58.797789 econdata-1.0.1/src/econdata/
--rw-rw-rw-   0        0        0     6359 2023-04-17 03:28:28.000000 econdata-1.0.1/src/econdata/BCRP.py
--rw-rw-rw-   0        0        0     2820 2023-04-14 08:10:41.000000 econdata-1.0.1/src/econdata/BM.py
--rw-rw-rw-   0        0        0     3554 2023-04-14 08:10:41.000000 econdata-1.0.1/src/econdata/FRED.py
--rw-rw-rw-   0        0        0     2112 2023-04-15 23:34:08.000000 econdata-1.0.1/src/econdata/OECD.py
--rw-rw-rw-   0        0        0     3592 2023-04-17 03:28:40.000000 econdata-1.0.1/src/econdata/YFinance.py
--rw-rw-rw-   0        0        0        0 2023-04-17 03:16:12.000000 econdata-1.0.1/src/econdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 03:29:58.817708 econdata-1.0.1/src/econdata.egg-info/
--rw-rw-rw-   0        0        0     1781 2023-04-17 03:29:58.000000 econdata-1.0.1/src/econdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-17 03:29:58.000000 econdata-1.0.1/src/econdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 03:29:58.000000 econdata-1.0.1/src/econdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-17 03:29:58.000000 econdata-1.0.1/src/econdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 03:29:58.000000 econdata-1.0.1/src/econdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 03:02:46.262250 econdata-1.0.2/
+-rw-rw-rw-   0        0        0     2092 2023-05-31 03:02:46.261277 econdata-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1620 2023-05-31 02:58:39.000000 econdata-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 03:02:46.262250 econdata-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-05-31 03:00:02.000000 econdata-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 03:02:46.033038 econdata-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 03:02:46.226983 econdata-1.0.2/src/econdata/
+-rw-rw-rw-   0        0        0     6259 2023-05-31 02:58:39.000000 econdata-1.0.2/src/econdata/BCRP.py
+-rw-rw-rw-   0        0        0     2820 2023-05-31 02:58:39.000000 econdata-1.0.2/src/econdata/BM.py
+-rw-rw-rw-   0        0        0     4008 2023-05-31 02:58:39.000000 econdata-1.0.2/src/econdata/FRED.py
+-rw-rw-rw-   0        0        0     2112 2023-05-31 02:58:39.000000 econdata-1.0.2/src/econdata/OECD.py
+-rw-rw-rw-   0        0        0     3592 2023-05-31 02:58:39.000000 econdata-1.0.2/src/econdata/YFinance.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 02:58:39.000000 econdata-1.0.2/src/econdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 03:02:46.260261 econdata-1.0.2/src/econdata.egg-info/
+-rw-rw-rw-   0        0        0     2092 2023-05-31 03:02:46.000000 econdata-1.0.2/src/econdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-31 03:02:46.000000 econdata-1.0.2/src/econdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 03:02:46.000000 econdata-1.0.2/src/econdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-31 03:02:46.000000 econdata-1.0.2/src/econdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 03:02:46.000000 econdata-1.0.2/src/econdata.egg-info/top_level.txt
```

### Comparing `econdata-1.0.1/PKG-INFO` & `econdata-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: econdata
-Version: 1.0.1
-Summary: Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú
+Version: 1.0.2
+Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/econdata
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -21,36 +21,37 @@
 ```
 # Instalación mediante PyPI
 !pip install econdata==1.0.1
 
 # o simplemente:
 !pip install econdata
 ```
-
+El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
 ## Versión 1.0.1
 * Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
 * Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
 
-La segunda sirve para conseguir la metadata, principalmente, los códigos de las series:
+La segunda sirve para conseguir la metadata:
 ```
 search()
 ```
 El resultado incluye los nombres, códigos y fechas que servirán como complemento con la función anterior: `get_data()`.
 
 
 ## Test !
 El código guía para usar las funciones está disponible [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
+El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
 
 
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo)
 * [Andrei Romero](https://github.com/Ixtalia)
```

### Comparing `econdata-1.0.1/README.md` & `econdata-1.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -9,36 +9,37 @@
 ```
 # Instalación mediante PyPI
 !pip install econdata==1.0.1
 
 # o simplemente:
 !pip install econdata
 ```
-
+El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
 ## Versión 1.0.1
 * Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
 * Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
 
-La segunda sirve para conseguir la metadata, principalmente, los códigos de las series:
+La segunda sirve para conseguir la metadata:
 ```
 search()
 ```
 El resultado incluye los nombres, códigos y fechas que servirán como complemento con la función anterior: `get_data()`.
 
 
 ## Test !
 El código guía para usar las funciones está disponible [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
+El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
 
 
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo)
 * [Andrei Romero](https://github.com/Ixtalia)
```

### Comparing `econdata-1.0.1/setup.py` & `econdata-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='econdata',
-    version = '1.0.1',
+    version = '1.0.2',
     author = 'Mauricio Alvarado, Andrei Romero',
-    description = 'Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú',
+    description = 'Extracción de series de tiempo de las principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mauricioalvaradoo/econdata',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
@@ -19,12 +19,13 @@
     package_dir={'':'src'},
     # packages=setuptools.find_packages(),
     python_requires='>=3.6',
     install_requires = [
         'pandas',
         'numpy',
         'yfinance',
-        'requests'
+        'requests',
+        'warnings'
     ]
 )
```

### Comparing `econdata-1.0.1/src/econdata/BCRP.py` & `econdata-1.0.2/src/econdata/BCRP.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,19 +89,17 @@
     df.set_index("time", inplace=True)
     df.rename(series, axis=1, inplace=True)
 
 
     # Formatos de fechas
     if keys[0][-1] == 'D':
         df.index = pd.to_datetime(df.index, format="%d.%b.%y")
-        df.index = df.index.strftime("%Y-%m-%d")
     if keys[0][-1] == 'M':
         df.index = df.index.str.replace('Set', 'Sep')
         df.index = pd.to_datetime(df.index, format="%b.%Y")
-        df.index = df.index.strftime("%Y-%m-%d")
     if keys[0][-1] == 'Q':
         try:
             df.index = pd.period_range(fechaini, fechafin, freq="Q")
         except: 
             try: # Hasta fecha fin Q4
                 df.index = pd.period_range(fechaini, fechafin[:4]+'Q4', freq="Q")
             except: # Aumentando un año para series en var. %
```

### Comparing `econdata-1.0.1/src/econdata/BM.py` & `econdata-1.0.2/src/econdata/BM.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.1/src/econdata/FRED.py` & `econdata-1.0.2/src/econdata/FRED.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pandas as pd
 import numpy as np
 import requests 
 
+import warnings
+warnings.simplefilter('ignore')
 
 
 def get_data(series, api_key, fechaini, fechafin):
     
     """ Importar múltiples series de la API del FRED
     
     Parámetros
@@ -77,30 +79,39 @@
     for i in df.columns:
         try:
             df.loc[df[i] == '.', i] = np.nan
             df[i] = df[i].astype('float')
         except:
             pass
     
+    # index to datetime
+    df.index = pd.to_datetime(df.index)
+
     return df
 
 
 
 
-def search(consulta, api_key):
+def search(consulta, api_key, frecuencia=None):
     
     """ Extraer metadatos de las consultas
 
     Parámetros
     ----------
     consulta: list
         Palabras claves de las consultas  
     api_key: str
         API Key del desarrollador: https://fred.stlouisfed.org/docs/api/api_key.html
-    
+    frecuencia: str
+        Frecuencia de la serie consultada. Default: None.
+        >>> "Daily"
+        >>> "Monthly"
+        >>> "Quarterly"
+        >>> "Annual"
+            
     Retorno
     ----------
     df: pd.DataFrame
        Series consultadas
     
 
     @authors: Norbert Andrei Romero Escobedo, Mauricio Alvarado
@@ -135,11 +146,17 @@
         "title": list_title,
         "start": list_start,
         "end": list_end,
         "frequency": list_frequency,
         "seasonal_adjusment": list_seasonal_adjusment
     })
 
+    if frecuencia is not None:
+        try:
+            df = df[df["frequency"] == str(frecuencia)]
+        except:
+            pass
+
     df.set_index("id", inplace=True) 
 
     return df
```

### Comparing `econdata-1.0.1/src/econdata/OECD.py` & `econdata-1.0.2/src/econdata/OECD.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.1/src/econdata/YFinance.py` & `econdata-1.0.2/src/econdata/YFinance.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.1/src/econdata.egg-info/PKG-INFO` & `econdata-1.0.2/src/econdata.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: econdata
-Version: 1.0.1
-Summary: Extracción de series de tiempo de las cinco principales instituciones económicas para el Perú
+Version: 1.0.2
+Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/econdata
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -21,36 +21,37 @@
 ```
 # Instalación mediante PyPI
 !pip install econdata==1.0.1
 
 # o simplemente:
 !pip install econdata
 ```
-
+El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
 ## Versión 1.0.1
 * Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
 * Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
 
-La segunda sirve para conseguir la metadata, principalmente, los códigos de las series:
+La segunda sirve para conseguir la metadata:
 ```
 search()
 ```
 El resultado incluye los nombres, códigos y fechas que servirán como complemento con la función anterior: `get_data()`.
 
 
 ## Test !
 El código guía para usar las funciones está disponible [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
+El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
 
 
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo)
 * [Andrei Romero](https://github.com/Ixtalia)
```

