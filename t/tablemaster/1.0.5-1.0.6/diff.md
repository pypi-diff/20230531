# Comparing `tmp/tablemaster-1.0.5.tar.gz` & `tmp/tablemaster-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.0.5.tar", last modified: Tue Apr  4 12:35:34 2023, max compression
+gzip compressed data, was "tablemaster-1.0.6.tar", last modified: Wed May 31 07:21:49 2023, max compression
```

## Comparing `tablemaster-1.0.5.tar` & `tablemaster-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-04-04 12:35:34.410934 tablemaster-1.0.5/
--rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.0.5/LICENSE
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-04-04 12:35:34.410788 tablemaster-1.0.5/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)     1346 2023-03-31 02:43:20.000000 tablemaster-1.0.5/README.md
--rw-r--r--   0 livid      (501) staff       (20)       38 2023-04-04 12:35:34.410971 tablemaster-1.0.5/setup.cfg
--rw-r--r--   0 livid      (501) staff       (20)      521 2023-04-04 12:35:21.000000 tablemaster-1.0.5/setup.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-04-04 12:35:34.409960 tablemaster-1.0.5/tablemaster/
--rw-r--r--   0 livid      (501) staff       (20)      490 2023-03-31 02:40:15.000000 tablemaster-1.0.5/tablemaster/__init__.py
--rw-r--r--   0 livid      (501) staff       (20)      559 2023-03-31 02:38:51.000000 tablemaster-1.0.5/tablemaster/gspread.py
--rw-r--r--   0 livid      (501) staff       (20)     3395 2023-04-04 12:32:12.000000 tablemaster-1.0.5/tablemaster/mysql.py
--rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.0.5/tablemaster/utils.py
-drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-04-04 12:35:34.410620 tablemaster-1.0.5/tablemaster.egg-info/
--rw-r--r--   0 livid      (501) staff       (20)      239 2023-04-04 12:35:34.000000 tablemaster-1.0.5/tablemaster.egg-info/PKG-INFO
--rw-r--r--   0 livid      (501) staff       (20)      289 2023-04-04 12:35:34.000000 tablemaster-1.0.5/tablemaster.egg-info/SOURCES.txt
--rw-r--r--   0 livid      (501) staff       (20)        1 2023-04-04 12:35:34.000000 tablemaster-1.0.5/tablemaster.egg-info/dependency_links.txt
--rw-r--r--   0 livid      (501) staff       (20)       92 2023-04-04 12:35:34.000000 tablemaster-1.0.5/tablemaster.egg-info/requires.txt
--rw-r--r--   0 livid      (501) staff       (20)       12 2023-04-04 12:35:34.000000 tablemaster-1.0.5/tablemaster.egg-info/top_level.txt
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-05-31 07:21:49.181111 tablemaster-1.0.6/
+-rw-r--r--   0 livid      (501) staff       (20)    11357 2023-03-29 11:23:27.000000 tablemaster-1.0.6/LICENSE
+-rw-r--r--   0 livid      (501) staff       (20)      239 2023-05-31 07:21:49.180986 tablemaster-1.0.6/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)     1484 2023-05-24 06:49:43.000000 tablemaster-1.0.6/README.md
+-rw-r--r--   0 livid      (501) staff       (20)       38 2023-05-31 07:21:49.181155 tablemaster-1.0.6/setup.cfg
+-rw-r--r--   0 livid      (501) staff       (20)      521 2023-05-31 07:21:36.000000 tablemaster-1.0.6/setup.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-05-31 07:21:49.180172 tablemaster-1.0.6/tablemaster/
+-rw-r--r--   0 livid      (501) staff       (20)      490 2023-03-31 02:40:15.000000 tablemaster-1.0.6/tablemaster/__init__.py
+-rw-r--r--   0 livid      (501) staff       (20)     1009 2023-05-31 07:12:09.000000 tablemaster-1.0.6/tablemaster/gspread.py
+-rw-r--r--   0 livid      (501) staff       (20)     3395 2023-04-04 12:32:12.000000 tablemaster-1.0.6/tablemaster/mysql.py
+-rw-r--r--   0 livid      (501) staff       (20)      810 2023-03-29 11:23:27.000000 tablemaster-1.0.6/tablemaster/utils.py
+drwxr-xr-x   0 livid      (501) staff       (20)        0 2023-05-31 07:21:49.180835 tablemaster-1.0.6/tablemaster.egg-info/
+-rw-r--r--   0 livid      (501) staff       (20)      239 2023-05-31 07:21:49.000000 tablemaster-1.0.6/tablemaster.egg-info/PKG-INFO
+-rw-r--r--   0 livid      (501) staff       (20)      289 2023-05-31 07:21:49.000000 tablemaster-1.0.6/tablemaster.egg-info/SOURCES.txt
+-rw-r--r--   0 livid      (501) staff       (20)        1 2023-05-31 07:21:49.000000 tablemaster-1.0.6/tablemaster.egg-info/dependency_links.txt
+-rw-r--r--   0 livid      (501) staff       (20)       92 2023-05-31 07:21:49.000000 tablemaster-1.0.6/tablemaster.egg-info/requires.txt
+-rw-r--r--   0 livid      (501) staff       (20)       12 2023-05-31 07:21:49.000000 tablemaster-1.0.6/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.0.5/LICENSE` & `tablemaster-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.0.5/README.md` & `tablemaster-1.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 # Examples
 
 ## import
 ```
 import tablemaster as tm
 ```
 
-## Query from mysql
+## query from mysql
 ```
 sql_query = 'SELECT * FROM table_name LIMIT 20'
 df = tm.query(sql_query, tm.cfg.db_name)
 df
 ```
 
-## Change column name
+## change column name
 ```
 sql_query = ('ALTER TABLE table_name RENAME COLUMN column1 TO column2')
 tm.opt(sql_query, tm.cfg.db_name)
 ```
 
 ## create a table in mysql and upload data from dataframe df
 ```
@@ -48,14 +48,20 @@
 
 ## delete a table in mysql
 ```
 tb = tm.Manage_table('table_name_2', tm.cfg.db1)
 tb.delete_table()
 ```
 
+## delete rows in mysql with condition
+```
+tb = tm.Manage_table('table_name_2', tm.cfg.db1)
+tb.par_del("order_date > '2023-01-01' ")
+```
+
 ## read table from google sheet
 ```
 google_sheet = ('GoogleSheet Table Name', 'GoogleSheet Sheet Name')
 df = tm.gs_read_df(google_sheet)
 df
 ```
```

### Comparing `tablemaster-1.0.5/setup.py` & `tablemaster-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy==1.4.46',
         'pandas',
         'python-dateutil',
         'gspread',
```

### Comparing `tablemaster-1.0.5/tablemaster/mysql.py` & `tablemaster-1.0.6/tablemaster/mysql.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.0.5/tablemaster/utils.py` & `tablemaster-1.0.6/tablemaster/utils.py`

 * *Files identical despite different names*

