# Comparing `tmp/DE_DataBaseConnect-0.0.68.tar.gz` & `tmp/DE_DataBaseConnect-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DE_DataBaseConnect-0.0.68.tar", last modified: Wed May 31 16:47:33 2023, max compression
+gzip compressed data, was "DE_DataBaseConnect-0.0.69.tar", last modified: Wed May 31 16:54:06 2023, max compression
```

## Comparing `DE_DataBaseConnect-0.0.68.tar` & `DE_DataBaseConnect-0.0.69.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 16:47:33.369650 DE_DataBaseConnect-0.0.68/
--rw-rw-rw-   0        0        0    17233 2023-05-31 16:46:37.000000 DE_DataBaseConnect-0.0.68/DE_DataBase.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:47:33.359675 DE_DataBaseConnect-0.0.68/DE_DataBaseConnect.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-31 16:47:32.000000 DE_DataBaseConnect-0.0.68/DE_DataBaseConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-05-31 16:47:32.000000 DE_DataBaseConnect-0.0.68/DE_DataBaseConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 16:47:32.000000 DE_DataBaseConnect-0.0.68/DE_DataBaseConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 16:47:32.000000 DE_DataBaseConnect-0.0.68/DE_DataBaseConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.68/Licence.txt
--rw-rw-rw-   0        0        0      307 2023-05-31 16:47:33.370647 DE_DataBaseConnect-0.0.68/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.68/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 16:47:33.379622 DE_DataBaseConnect-0.0.68/setup.cfg
--rw-rw-rw-   0        0        0      327 2023-05-31 16:47:14.000000 DE_DataBaseConnect-0.0.68/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:54:06.410942 DE_DataBaseConnect-0.0.69/
+-rw-rw-rw-   0        0        0    17233 2023-05-31 16:53:42.000000 DE_DataBaseConnect-0.0.69/DE_DataBase.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:54:06.400968 DE_DataBaseConnect-0.0.69/DE_DataBaseConnect.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-31 16:54:05.000000 DE_DataBaseConnect-0.0.69/DE_DataBaseConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-31 16:54:05.000000 DE_DataBaseConnect-0.0.69/DE_DataBaseConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 16:54:05.000000 DE_DataBaseConnect-0.0.69/DE_DataBaseConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 16:54:05.000000 DE_DataBaseConnect-0.0.69/DE_DataBaseConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.69/Licence.txt
+-rw-rw-rw-   0        0        0      307 2023-05-31 16:54:06.411940 DE_DataBaseConnect-0.0.69/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.69/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 16:54:06.417924 DE_DataBaseConnect-0.0.69/setup.cfg
+-rw-rw-rw-   0        0        0      327 2023-05-31 16:53:58.000000 DE_DataBaseConnect-0.0.69/setup.py
```

### Comparing `DE_DataBaseConnect-0.0.68/DE_DataBase.py` & `DE_DataBaseConnect-0.0.69/DE_DataBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,17 +84,17 @@
                 dnsName = ora.makedsn(host=string_connect["host"], port=string_connect["port"], service_name=string_connect["instance"])
 
             # Efetuando a conexao com a instancia do BANCO
             conn = ora.connect(string_connect["username"], string_connect["password"], dnsName, threaded=True)
             self._connection_is_valid = True
             self._nome_database = string_connect["database"]
         except Exception as error:
-            msg = f"""Falha ao tentar se conectar com o banco de dados ORACLE [{string_connect["name_conection"]}].\nErro: {error} """
-            conn = msg
             self._connection_is_valid = False
+            msg = error
+            conn = f"""Falha ao tentar se conectar com o banco de dados ORACLE [{string_connect["name_conection"]}].\nErro: {msg} """
             self._DATABASE_ERROR = conn
         finally:
             return conn
 
     def SQLITE(self, database, **kwargs):
         DATABASE_NAME, result, msg, conn = None, False, None, None
         try:
```

### Comparing `DE_DataBaseConnect-0.0.68/Licence.txt` & `DE_DataBaseConnect-0.0.69/Licence.txt`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.68/README.md` & `DE_DataBaseConnect-0.0.69/README.md`

 * *Files identical despite different names*

