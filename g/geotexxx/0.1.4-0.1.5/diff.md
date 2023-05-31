# Comparing `tmp/geotexxx-0.1.4.tar.gz` & `tmp/geotexxx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geotexxx-0.1.4.tar", last modified: Wed May 31 11:27:11 2023, max compression
+gzip compressed data, was "geotexxx-0.1.5.tar", last modified: Wed May 31 14:19:51 2023, max compression
```

## Comparing `geotexxx-0.1.4.tar` & `geotexxx-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 11:27:11.682188 geotexxx-0.1.4/
--rw-rw-rw-   0        0        0    13954 2022-04-20 15:29:56.000000 geotexxx-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3831 2023-05-31 11:27:11.681188 geotexxx-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3573 2023-04-04 15:09:05.000000 geotexxx-0.1.4/README.md
--rw-rw-rw-   0        0        0      405 2023-05-31 11:26:31.000000 geotexxx-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 11:27:11.682188 geotexxx-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 11:27:11.660220 geotexxx-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 11:27:11.668915 geotexxx-0.1.4/src/geotexxx/
--rw-rw-rw-   0        0        0        0 2023-02-24 15:44:18.000000 geotexxx-0.1.4/src/geotexxx/__init__.py
--rw-rw-rw-   0        0        0   103525 2023-05-31 10:28:47.000000 geotexxx-0.1.4/src/geotexxx/gefxml_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:27:11.679181 geotexxx-0.1.4/src/geotexxx.egg-info/
--rw-rw-rw-   0        0        0     3831 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 11:27:11.000000 geotexxx-0.1.4/src/geotexxx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 14:19:51.455959 geotexxx-0.1.5/
+-rw-rw-rw-   0        0        0    13954 2022-04-20 15:29:56.000000 geotexxx-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3831 2023-05-31 14:19:51.454963 geotexxx-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3573 2023-04-04 15:09:05.000000 geotexxx-0.1.5/README.md
+-rw-rw-rw-   0        0        0      405 2023-05-31 14:19:37.000000 geotexxx-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 14:19:51.455959 geotexxx-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 14:19:51.431904 geotexxx-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 14:19:51.442969 geotexxx-0.1.5/src/geotexxx/
+-rw-rw-rw-   0        0        0        0 2023-02-24 15:44:18.000000 geotexxx-0.1.5/src/geotexxx/__init__.py
+-rw-rw-rw-   0        0        0   103425 2023-05-31 14:17:40.000000 geotexxx-0.1.5/src/geotexxx/gefxml_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:19:51.452959 geotexxx-0.1.5/src/geotexxx.egg-info/
+-rw-rw-rw-   0        0        0     3831 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 14:19:51.000000 geotexxx-0.1.5/src/geotexxx.egg-info/top_level.txt
```

### Comparing `geotexxx-0.1.4/LICENSE.txt` & `geotexxx-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geotexxx-0.1.4/PKG-INFO` & `geotexxx-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotexxx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package om geotechnisch grondonderzoek te verwerken
 Author-email: Thomas van der Linden <t.van.der.linden@amsterdam.nl>
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gefxml_reader
```

### Comparing `geotexxx-0.1.4/README.md` & `geotexxx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `geotexxx-0.1.4/src/geotexxx/gefxml_reader.py` & `geotexxx-0.1.5/src/geotexxx/gefxml_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1924,16 +1924,14 @@
 
         aantal_boringen = len(properties['bore'].unique())
         
         for boreId, boreData in properties.groupby('bore'): 
 
             if type(boreId) != float: # er kan een nan inzitten, dat is data type float
                 try: 
-                    print(f'{boreId} van {aantal_boringen} boringen')
-
                     # TODO: zou dit beter zijn als method voor de class Bore?
                     bore = Bore()
                     bore.soillayers = {}
 
                     layers = {}
                     for layerNr, layerData in boreData.groupby('layer'):
                         layerData = layerData.max(skipna=True)
@@ -1999,16 +1997,16 @@
                     xs.append(bore.easting)
                     ys.append(bore.northing)
                     fs.append(f'{bore.testid}_{boreId}')
                     groundlevels.append(bore.groundlevel)
                     depths.append(onderkant)
                     peilbuizen.append(peilbuisAanwezig)
                     boorbeschrijvingen.append(boorbeschrijving)
-                except Exception as e:
-                    print(boreId, e)
+                except:
+                    pass
 
         # maak een csv met locaties en bestandsnamen en of er een boorbeschrijving en een peilbuis aanwezig is
         kaart = pd.DataFrame()
         kaart['x'] = xs
         kaart['y'] = ys
         kaart['boring'] = fs
         kaart['maaiveld'] = groundlevels
```

### Comparing `geotexxx-0.1.4/src/geotexxx.egg-info/PKG-INFO` & `geotexxx-0.1.5/src/geotexxx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geotexxx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package om geotechnisch grondonderzoek te verwerken
 Author-email: Thomas van der Linden <t.van.der.linden@amsterdam.nl>
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gefxml_reader
```

