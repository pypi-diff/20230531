# Comparing `tmp/DE_DataBaseConnect-0.0.73.tar.gz` & `tmp/DE_DataBaseConnect-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DE_DataBaseConnect-0.0.73.tar", last modified: Wed May 31 17:18:57 2023, max compression
+gzip compressed data, was "DE_DataBaseConnect-0.0.74.tar", last modified: Wed May 31 17:22:04 2023, max compression
```

## Comparing `DE_DataBaseConnect-0.0.73.tar` & `DE_DataBaseConnect-0.0.74.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:57.363238 DE_DataBaseConnect-0.0.73/
--rw-rw-rw-   0        0        0    17280 2023-05-31 17:18:50.000000 DE_DataBaseConnect-0.0.73/DE_DataBase.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:18:57.352263 DE_DataBaseConnect-0.0.73/DE_DataBaseConnect.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-31 17:18:56.000000 DE_DataBaseConnect-0.0.73/DE_DataBaseConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-31 17:18:56.000000 DE_DataBaseConnect-0.0.73/DE_DataBaseConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 17:18:56.000000 DE_DataBaseConnect-0.0.73/DE_DataBaseConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 17:18:56.000000 DE_DataBaseConnect-0.0.73/DE_DataBaseConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.73/Licence.txt
--rw-rw-rw-   0        0        0      307 2023-05-31 17:18:57.365228 DE_DataBaseConnect-0.0.73/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.73/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 17:18:57.374205 DE_DataBaseConnect-0.0.73/setup.cfg
--rw-rw-rw-   0        0        0      327 2023-05-31 17:18:50.000000 DE_DataBaseConnect-0.0.73/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:22:04.553067 DE_DataBaseConnect-0.0.74/
+-rw-rw-rw-   0        0        0    17270 2023-05-31 17:21:53.000000 DE_DataBaseConnect-0.0.74/DE_DataBase.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:22:04.540102 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-31 17:22:03.000000 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-31 17:22:03.000000 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 17:22:03.000000 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 17:22:03.000000 DE_DataBaseConnect-0.0.74/DE_DataBaseConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.74/Licence.txt
+-rw-rw-rw-   0        0        0      307 2023-05-31 17:22:04.553067 DE_DataBaseConnect-0.0.74/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.74/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 17:22:04.562044 DE_DataBaseConnect-0.0.74/setup.cfg
+-rw-rw-rw-   0        0        0      327 2023-05-31 17:21:59.000000 DE_DataBaseConnect-0.0.74/setup.py
```

### Comparing `DE_DataBaseConnect-0.0.73/DE_DataBase.py` & `DE_DataBaseConnect-0.0.74/DE_DataBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
             # Efetuando a conexao com a instancia do BANCO
             conn = ora.connect(string_connect["username"], string_connect["password"], dnsName, threaded=True)
             self._connection_is_valid = True
             self._nome_database = string_connect["database"]
         except Exception as error:
             self._connection_is_valid = False
-            msg = f"""Falha ao tentar se conectar com o banco de dados ORACLE [{string_connect["name_conection"]}].\nException Error: {error} """
+            msg = f"""Falha ao tentar se conectar com o banco de dados ORACLE [{string_connect["name"]}].\nException Error: {error} """
             self._DATABASE_ERROR = msg
             conn = msg
         finally:
             return conn
 
     def SQLITE(self, database, **kwargs):
         DATABASE_NAME, result, msg, conn = None, False, None, None
```

### Comparing `DE_DataBaseConnect-0.0.73/Licence.txt` & `DE_DataBaseConnect-0.0.74/Licence.txt`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.73/README.md` & `DE_DataBaseConnect-0.0.74/README.md`

 * *Files identical despite different names*

