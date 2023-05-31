# Comparing `tmp/relativedate-1.3.2.tar.gz` & `tmp/relativedate-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relativedate-1.3.2.tar", last modified: Mon May 29 20:15:27 2023, max compression
+gzip compressed data, was "relativedate-1.3.3.tar", last modified: Wed May 31 16:36:13 2023, max compression
```

## Comparing `relativedate-1.3.2.tar` & `relativedate-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 20:15:27.054959 relativedate-1.3.2/
--rw-rw-rw-   0        0        0     2414 2023-05-29 20:15:27.053961 relativedate-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2254 2023-05-24 11:24:35.000000 relativedate-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 20:15:27.043987 relativedate-1.3.2/relativedate/
--rw-rw-rw-   0        0        0     2030 2023-05-29 20:11:29.000000 relativedate-1.3.2/relativedate/__init__.py
--rw-rw-rw-   0        0        0     1095 2023-05-29 20:12:04.000000 relativedate-1.3.2/relativedate/dtget.py
--rw-rw-rw-   0        0        0     1243 2023-05-25 11:28:49.000000 relativedate-1.3.2/relativedate/dtmath.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:15:27.052965 relativedate-1.3.2/relativedate.egg-info/
--rw-rw-rw-   0        0        0     2414 2023-05-29 20:15:26.000000 relativedate-1.3.2/relativedate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-29 20:15:26.000000 relativedate-1.3.2/relativedate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 20:15:26.000000 relativedate-1.3.2/relativedate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 20:15:26.000000 relativedate-1.3.2/relativedate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 20:15:27.054959 relativedate-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      455 2023-05-29 20:15:24.000000 relativedate-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:36:13.277414 relativedate-1.3.3/
+-rw-rw-rw-   0        0        0     2414 2023-05-31 16:36:13.277414 relativedate-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2254 2023-05-24 11:24:35.000000 relativedate-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 16:36:13.263453 relativedate-1.3.3/relativedate/
+-rw-rw-rw-   0        0        0     2030 2023-05-29 20:11:29.000000 relativedate-1.3.3/relativedate/__init__.py
+-rw-rw-rw-   0        0        0     1095 2023-05-29 20:12:04.000000 relativedate-1.3.3/relativedate/dtget.py
+-rw-rw-rw-   0        0        0     1378 2023-05-31 16:34:33.000000 relativedate-1.3.3/relativedate/dtmath.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:36:13.276417 relativedate-1.3.3/relativedate.egg-info/
+-rw-rw-rw-   0        0        0     2414 2023-05-31 16:36:13.000000 relativedate-1.3.3/relativedate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-31 16:36:13.000000 relativedate-1.3.3/relativedate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 16:36:13.000000 relativedate-1.3.3/relativedate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 16:36:13.000000 relativedate-1.3.3/relativedate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 16:36:13.278411 relativedate-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-05-31 16:34:51.000000 relativedate-1.3.3/setup.py
```

### Comparing `relativedate-1.3.2/PKG-INFO` & `relativedate-1.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relativedate
-Version: 1.3.2
+Version: 1.3.3
 Summary: Pacote Python para tabalhar com Datas Relativas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: relativedate Version: 1.3.2 Summary: Pacote Python
+Metadata-Version: 2.1 Name: relativedate Version: 1.3.3 Summary: Pacote Python
 para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
```

### Comparing `relativedate-1.3.2/README.md` & `relativedate-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `relativedate-1.3.2/relativedate/__init__.py` & `relativedate-1.3.3/relativedate/__init__.py`

 * *Files identical despite different names*

### Comparing `relativedate-1.3.2/relativedate/dtget.py` & `relativedate-1.3.3/relativedate/dtget.py`

 * *Files identical despite different names*

### Comparing `relativedate-1.3.2/relativedate/dtmath.py` & `relativedate-1.3.3/relativedate/dtmath.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,21 @@
         # Tratamento do Mês
         if month < 1: 
             month += 12
             year -= 1
         elif month > 12: 
             month -= 12
             year += 1
-        return dt.replace(year=year, month=month)
+        
+        day = dt.day
+        while True:
+            try:
+                return dt.replace(year=year, month=month, day=day)
+            except:
+                day -= 1
 
 def addDay(dt, relative_day):
      return dt + timedelta(days=relative_day)
 
 
 def add(dt, year=0, month=0, day=0, hour=0, minute=0, second=0):
     dt = dt
```

### Comparing `relativedate-1.3.2/relativedate.egg-info/PKG-INFO` & `relativedate-1.3.3/relativedate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relativedate
-Version: 1.3.2
+Version: 1.3.3
 Summary: Pacote Python para tabalhar com Datas Relativas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: relativedate Version: 1.3.2 Summary: Pacote Python
+Metadata-Version: 2.1 Name: relativedate Version: 1.3.3 Summary: Pacote Python
 para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
```

