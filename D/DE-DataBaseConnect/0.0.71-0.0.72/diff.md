# Comparing `tmp/DE_DataBaseConnect-0.0.71.tar.gz` & `tmp/DE_DataBaseConnect-0.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DE_DataBaseConnect-0.0.71.tar", last modified: Wed May 31 17:06:42 2023, max compression
+gzip compressed data, was "DE_DataBaseConnect-0.0.72.tar", last modified: Wed May 31 17:13:12 2023, max compression
```

## Comparing `DE_DataBaseConnect-0.0.71.tar` & `DE_DataBaseConnect-0.0.72.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 17:06:42.865261 DE_DataBaseConnect-0.0.71/
--rw-rw-rw-   0        0        0    17319 2023-05-31 17:06:36.000000 DE_DataBaseConnect-0.0.71/DE_DataBase.py
-drwxrwxrwx   0        0        0        0 2023-05-31 17:06:42.853288 DE_DataBaseConnect-0.0.71/DE_DataBaseConnect.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-31 17:06:41.000000 DE_DataBaseConnect-0.0.71/DE_DataBaseConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-31 17:06:41.000000 DE_DataBaseConnect-0.0.71/DE_DataBaseConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 17:06:41.000000 DE_DataBaseConnect-0.0.71/DE_DataBaseConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 17:06:41.000000 DE_DataBaseConnect-0.0.71/DE_DataBaseConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.71/Licence.txt
--rw-rw-rw-   0        0        0      307 2023-05-31 17:06:42.866258 DE_DataBaseConnect-0.0.71/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.71/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 17:06:42.872237 DE_DataBaseConnect-0.0.71/setup.cfg
--rw-rw-rw-   0        0        0      327 2023-05-31 17:06:36.000000 DE_DataBaseConnect-0.0.71/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:13:12.004668 DE_DataBaseConnect-0.0.72/
+-rw-rw-rw-   0        0        0    17318 2023-05-31 17:13:05.000000 DE_DataBaseConnect-0.0.72/DE_DataBase.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:13:11.994668 DE_DataBaseConnect-0.0.72/DE_DataBaseConnect.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-31 17:13:10.000000 DE_DataBaseConnect-0.0.72/DE_DataBaseConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-31 17:13:11.000000 DE_DataBaseConnect-0.0.72/DE_DataBaseConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 17:13:10.000000 DE_DataBaseConnect-0.0.72/DE_DataBaseConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 17:13:10.000000 DE_DataBaseConnect-0.0.72/DE_DataBaseConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.72/Licence.txt
+-rw-rw-rw-   0        0        0      307 2023-05-31 17:13:12.005643 DE_DataBaseConnect-0.0.72/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.72/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 17:13:12.013620 DE_DataBaseConnect-0.0.72/setup.cfg
+-rw-rw-rw-   0        0        0      327 2023-05-31 17:13:05.000000 DE_DataBaseConnect-0.0.72/setup.py
```

### Comparing `DE_DataBaseConnect-0.0.71/DE_DataBase.py` & `DE_DataBaseConnect-0.0.72/DE_DataBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             # Efetuando a conexao com a instancia do BANCO
             conn = ora.connect(string_connect["username"], string_connect["password"], dnsName, threaded=True)
             self._connection_is_valid = True
             self._nome_database = string_connect["database"]
         except Exception as error:
             self._connection_is_valid = False
             msg = f"""Falha ao tentar se conectar com o banco de dados ORACLE [{string_connect["name_conection"]}].\nDataBase Erro: {conn.DatabaseError}\n exception Error: {error} """
-            self._DATABASE_ERROR = conn
+            self._DATABASE_ERROR = msg
             conn = msg
         finally:
             return conn
 
     def SQLITE(self, database, **kwargs):
         DATABASE_NAME, result, msg, conn = None, False, None, None
         try:
```

### Comparing `DE_DataBaseConnect-0.0.71/Licence.txt` & `DE_DataBaseConnect-0.0.72/Licence.txt`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.71/README.md` & `DE_DataBaseConnect-0.0.72/README.md`

 * *Files identical despite different names*

