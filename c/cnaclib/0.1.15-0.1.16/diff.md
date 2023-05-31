# Comparing `tmp/cnaclib-0.1.15.tar.gz` & `tmp/cnaclib-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnaclib-0.1.15.tar", last modified: Tue May 30 11:27:40 2023, max compression
+gzip compressed data, was "cnaclib-0.1.16.tar", last modified: Wed May 31 08:07:16 2023, max compression
```

## Comparing `cnaclib-0.1.15.tar` & `cnaclib-0.1.16.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 11:27:40.100839 cnaclib-0.1.15/
--rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.15/LICENSE.txt
--rw-rw-rw-   0        0        0     2879 2023-05-30 11:27:40.093838 cnaclib-0.1.15/PKG-INFO
--rw-rw-rw-   0        0        0     1956 2023-05-30 11:25:19.000000 cnaclib-0.1.15/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 11:27:40.021831 cnaclib-0.1.15/cnaclib/
--rw-rw-rw-   0        0        0       17 2023-05-18 14:22:52.000000 cnaclib-0.1.15/cnaclib/__init__.py
--rw-rw-rw-   0        0        0     7931 2023-05-22 15:45:17.000000 cnaclib-0.1.15/cnaclib/lSix.py
--rw-rw-rw-   0        0        0    23582 2023-05-30 10:39:35.000000 cnaclib-0.1.15/cnaclib/rac.py
--rw-rw-rw-   0        0        0       36 2023-05-22 15:54:04.000000 cnaclib-0.1.15/cnaclib/test.py
--rw-rw-rw-   0        0        0    21837 2023-05-25 10:53:32.000000 cnaclib-0.1.15/cnaclib/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-30 11:27:40.085837 cnaclib-0.1.15/cnaclib.egg-info/
--rw-rw-rw-   0        0        0     2879 2023-05-30 11:27:38.000000 cnaclib-0.1.15/cnaclib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-30 11:27:38.000000 cnaclib-0.1.15/cnaclib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 11:27:38.000000 cnaclib-0.1.15/cnaclib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-05-30 11:27:38.000000 cnaclib-0.1.15/cnaclib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 11:27:38.000000 cnaclib-0.1.15/cnaclib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 11:27:40.103839 cnaclib-0.1.15/setup.cfg
--rw-rw-rw-   0        0        0     1192 2023-05-30 11:22:54.000000 cnaclib-0.1.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 08:07:16.588306 cnaclib-0.1.16/
+-rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.16/LICENSE.txt
+-rw-rw-rw-   0        0        0     2879 2023-05-31 08:07:16.584306 cnaclib-0.1.16/PKG-INFO
+-rw-rw-rw-   0        0        0     1956 2023-05-30 11:25:19.000000 cnaclib-0.1.16/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 08:07:16.547302 cnaclib-0.1.16/cnaclib/
+-rw-rw-rw-   0        0        0       17 2023-05-18 14:22:52.000000 cnaclib-0.1.16/cnaclib/__init__.py
+-rw-rw-rw-   0        0        0     7931 2023-05-22 15:45:17.000000 cnaclib-0.1.16/cnaclib/lSix.py
+-rw-rw-rw-   0        0        0    23585 2023-05-31 07:35:47.000000 cnaclib-0.1.16/cnaclib/rac.py
+-rw-rw-rw-   0        0        0       36 2023-05-22 15:54:04.000000 cnaclib-0.1.16/cnaclib/test.py
+-rw-rw-rw-   0        0        0    21531 2023-05-31 07:37:31.000000 cnaclib-0.1.16/cnaclib/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-31 08:07:16.576305 cnaclib-0.1.16/cnaclib.egg-info/
+-rw-rw-rw-   0        0        0     2879 2023-05-31 08:07:14.000000 cnaclib-0.1.16/cnaclib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-31 08:07:15.000000 cnaclib-0.1.16/cnaclib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 08:07:14.000000 cnaclib-0.1.16/cnaclib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-05-31 08:07:14.000000 cnaclib-0.1.16/cnaclib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 08:07:14.000000 cnaclib-0.1.16/cnaclib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 08:07:16.590306 cnaclib-0.1.16/setup.cfg
+-rw-rw-rw-   0        0        0     1192 2023-05-31 07:31:23.000000 cnaclib-0.1.16/setup.py
```

### Comparing `cnaclib-0.1.15/LICENSE.txt` & `cnaclib-0.1.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.15/PKG-INFO` & `cnaclib-0.1.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnaclib
-Version: 0.1.15
+Version: 0.1.16
 Summary: Simulateur RAC
 Home-page: UNKNOWN
 Author: BENHAMADA Nadir
 Author-email: aistatendz@gmail.com
 License: UNKNOWN
 Description: # cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC.
```

### Comparing `cnaclib-0.1.15/README.md` & `cnaclib-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.15/cnaclib/lSix.py` & `cnaclib-0.1.16/cnaclib/lSix.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.15/cnaclib/rac.py` & `cnaclib-0.1.16/cnaclib/rac.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         Date : str.
         Une date au format texte --> "dd/mm/yyyy".
         
         Returns
         -------
         Le Salaire National Minimum Garanti.
         '''
-        return SNMG(Date)
+        return SNMG(Date)[0]
 
 
     def Cal_SalRef(self, snmg):
         '''
         Calcul le Salaire de référence qui est calculé sur la base du Salaire mensuel moyen et le Salaire National Minimum Garanti.
```

### Comparing `cnaclib-0.1.15/cnaclib/tools.py` & `cnaclib-0.1.16/cnaclib/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 from datetime import datetime
+from dateutil import relativedelta
+import pandas as pd
 
 ##########################################################################################################################################
 #                                                       TOOLS
 ##########################################################################################################################################
 
 
 def listeCodewils():
@@ -538,47 +540,60 @@
 
     elif langue == 1:
         for code in listeCodewils():
             if not os.path.exists(code+'-'+NomWil(code, langue)):
                 os.mkdir(chemin+code+'-'+NomWil(code, langue))
 
 
-def SNMG(Date):
-    Date = datetime.strptime(Date, "%d/%m/%Y")
-    if Date < datetime.strptime('01/01/1990', "%d/%m/%Y"):
-        SNMG = 0
-    elif Date >= datetime.strptime('01/01/1990', "%d/%m/%Y") and  Date <= datetime.strptime('31/12/1990', "%d/%m/%Y") :
-        SNMG = 1000
-    elif  Date >= datetime.strptime('01/01/1991', "%d/%m/%Y") and Date <= datetime.strptime('30/06/1991', "%d/%m/%Y"):
-        SNMG = 1800
-    elif  Date >= datetime.strptime('01/07/1991', "%d/%m/%Y") and Date <= datetime.strptime('31/03/1992', "%d/%m/%Y"):
-        SNMG = 2000
-    elif  Date >= datetime.strptime('01/04/1992', "%d/%m/%Y") and Date <= datetime.strptime('30/04/1997', "%d/%m/%Y"):
-        SNMG = 2500
-    elif  Date >= datetime.strptime('01/05/1997', "%d/%m/%Y") and Date <= datetime.strptime('31/12/1997', "%d/%m/%Y"):
-        SNMG = 4800
-    elif  Date >= datetime.strptime('01/01/1998', "%d/%m/%Y") and Date <= datetime.strptime('31/08/1998', "%d/%m/%Y"):
-        SNMG = 5400
-    elif  Date >= datetime.strptime('01/09/1998', "%d/%m/%Y") and Date <= datetime.strptime('31/12/2000', "%d/%m/%Y"):
-        SNMG = 6000
-    elif  Date >= datetime.strptime('01/01/2001', "%d/%m/%Y") and Date <= datetime.strptime('31/12/2003', "%d/%m/%Y"):
-        SNMG = 8000
-    elif  Date >= datetime.strptime('01/01/2004', "%d/%m/%Y") and Date <= datetime.strptime('31/12/2006', "%d/%m/%Y"):
-        SNMG = 10000
-    elif  Date >= datetime.strptime('01/01/2007', "%d/%m/%Y") and Date <= datetime.strptime('31/12/2009', "%d/%m/%Y"):
-        SNMG = 12000
-    elif  Date >= datetime.strptime('01/01/2010', "%d/%m/%Y") and Date <= datetime.strptime('31/12/2011', "%d/%m/%Y"):
-        SNMG = 15000
-    elif  Date >= datetime.strptime('01/01/2012', "%d/%m/%Y") and Date <= datetime.strptime('31/05/2020', "%d/%m/%Y"):
-        SNMG = 18000
-    elif  Date >= datetime.strptime('01/06/2020', "%d/%m/%Y"):
-        SNMG = 20000
-    return SNMG
+def SNMG(date_saisie):
+    date_saisie = datetime.strptime(date_saisie, "%d/%m/%Y").date()
+
+    listeDatesFinStr = ['31/12/1990','30/06/1991','31/03/1992', 
+                   '30/04/1997','31/12/1997','31/08/1998',
+                   '31/12/2000','31/12/2003','31/12/2006', 
+                   '31/12/2009','31/12/2011','31/05/2020', 
+                    ]
+    dateDebut = datetime.strptime('01/01/1990', "%d/%m/%Y").date()
+
+    listeDatesFin = [datetime.strptime(i, "%d/%m/%Y").date() for i in listeDatesFinStr]
+
+    jourPlus = relativedelta.relativedelta(days=1)
+    anneePlus =relativedelta.relativedelta(years=1)
+    
+    valeurs = [1000.0, 1800.0, 2000.0, 2500.0, 4800.0, 5400.0, 6000.0, 8000.0, 10000.0, 12000.0, 15000.0, 18000.0, 20000.0]
+    
+    snmg_dict = {
+        '0': {"DateDebut":dateDebut,
+            "DateFin":listeDatesFin[0],
+            "SNMG":valeurs[0]
+        }
+    }
+    
+    for index, date  in enumerate(listeDatesFin):
+
+        snmg_dict[str(index+1)] = {
+            "DateDebut":date + jourPlus,
+            "DateFin":listeDatesFin[index+1],
+            "SNMG":valeurs[index+1]
+        }
+
+        if index == 10:
+            snmg_dict['12'] = {"DateDebut":listeDatesFin[index+1] + jourPlus,
+                "DateFin":datetime.today().date()+anneePlus,
+                "SNMG":valeurs[12]}      
+            break
+     
+    for dict in snmg_dict:
+        debut = snmg_dict[dict].get('DateDebut')
+        fin = snmg_dict[dict].get('DateFin')   
+        if date_saisie >= debut and date_saisie <= fin:
+            snmg = snmg_dict[dict].get('SNMG')
+            break
+        else:
+            snmg = 0
+    snmg_tbl = pd.DataFrame(snmg_dict.values(), snmg_dict.keys())
+    return snmg, snmg_dict, snmg_tbl
+
 
 
 
 
-#[print(NomWil(p,0)) for p in listeCodewils()]
-#[print(NomWil(p,1)) for p in listeCodewils()]
-#[print(Region(NomWil(p,0),0)) for p in listeCodewils()]
-#GenererDossiers(1)
-#print(SNMG('23/11/1995'))
```

### Comparing `cnaclib-0.1.15/cnaclib.egg-info/PKG-INFO` & `cnaclib-0.1.16/cnaclib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnaclib
-Version: 0.1.15
+Version: 0.1.16
 Summary: Simulateur RAC
 Home-page: UNKNOWN
 Author: BENHAMADA Nadir
 Author-email: aistatendz@gmail.com
 License: UNKNOWN
 Description: # cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC.
```

### Comparing `cnaclib-0.1.15/setup.py` & `cnaclib-0.1.16/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 chemin = Path(__file__).parent
 long_description = (chemin / "README.md").read_text()
 
 
 setuptools.setup(
     name = 'cnaclib',
-    version = '0.1.15',
+    version = '0.1.16',
     author= 'BENHAMADA Nadir',
     author_email='aistatendz@gmail.com',
     description='Simulateur RAC',
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=["certifi >=2023.5.7",
```

