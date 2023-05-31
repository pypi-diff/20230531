# Comparing `tmp/DE_DataBaseConnect-0.0.66.tar.gz` & `tmp/DE_DataBaseConnect-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DE_DataBaseConnect-0.0.66.tar", last modified: Thu Feb 16 17:55:45 2023, max compression
+gzip compressed data, was "DE_DataBaseConnect-0.0.67.tar", last modified: Wed May 31 15:45:07 2023, max compression
```

## Comparing `DE_DataBaseConnect-0.0.66.tar` & `DE_DataBaseConnect-0.0.67.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 17:55:45.482072 DE_DataBaseConnect-0.0.66/
--rw-rw-rw-   0        0        0    17237 2023-02-16 17:55:08.000000 DE_DataBaseConnect-0.0.66/DE_DataBase.py
-drwxrwxrwx   0        0        0        0 2023-02-16 17:55:45.466114 DE_DataBaseConnect-0.0.66/DE_DataBaseConnect.egg-info/
--rw-rw-rw-   0        0        0      307 2023-02-16 17:55:43.000000 DE_DataBaseConnect-0.0.66/DE_DataBaseConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-02-16 17:55:43.000000 DE_DataBaseConnect-0.0.66/DE_DataBaseConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 17:55:43.000000 DE_DataBaseConnect-0.0.66/DE_DataBaseConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 17:55:43.000000 DE_DataBaseConnect-0.0.66/DE_DataBaseConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.66/Licence.txt
--rw-rw-rw-   0        0        0      307 2023-02-16 17:55:45.476089 DE_DataBaseConnect-0.0.66/PKG-INFO
--rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.66/README.md
--rw-rw-rw-   0        0        0       42 2023-02-16 17:55:45.483068 DE_DataBaseConnect-0.0.66/setup.cfg
--rw-rw-rw-   0        0        0      327 2023-02-16 17:55:08.000000 DE_DataBaseConnect-0.0.66/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:45:07.928088 DE_DataBaseConnect-0.0.67/
+-rw-rw-rw-   0        0        0    17247 2023-05-31 15:43:36.000000 DE_DataBaseConnect-0.0.67/DE_DataBase.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:45:07.918112 DE_DataBaseConnect-0.0.67/DE_DataBaseConnect.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-31 15:45:05.000000 DE_DataBaseConnect-0.0.67/DE_DataBaseConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-31 15:45:05.000000 DE_DataBaseConnect-0.0.67/DE_DataBaseConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:45:05.000000 DE_DataBaseConnect-0.0.67/DE_DataBaseConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:45:05.000000 DE_DataBaseConnect-0.0.67/DE_DataBaseConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.67/Licence.txt
+-rw-rw-rw-   0        0        0      307 2023-05-31 15:45:07.929087 DE_DataBaseConnect-0.0.67/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2022-08-23 21:32:43.000000 DE_DataBaseConnect-0.0.67/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 15:45:07.936065 DE_DataBaseConnect-0.0.67/setup.cfg
+-rw-rw-rw-   0        0        0      327 2023-05-31 15:44:09.000000 DE_DataBaseConnect-0.0.67/setup.py
```

### Comparing `DE_DataBaseConnect-0.0.66/DE_DataBase.py` & `DE_DataBaseConnect-0.0.67/DE_DataBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 dnsName = ora.makedsn(host=string_connect["host"], port=string_connect["port"], service_name=string_connect["instance"])
 
             # Efetuando a conexao com a instancia do BANCO
             conn = ora.connect(string_connect["username"], string_connect["password"], dnsName, threaded=True)
             self._connection_is_valid = True
             self._nome_database = string_connect["database"]
         except Exception as error:
-            msg = f"""Falha ao tentar se conectar com o banco de dados ORACLE [{string_connect["name"]}].\nErro: {error} """
+            msg = f"""Falha ao tentar se conectar com o banco de dados ORACLE [{string_connect["name_conection"]}].\nErro: {error} """
             conn = msg
             self._connection_is_valid = False
             self._DATABASE_ERROR = conn.DatabaseError
         finally:
             return conn
 
     def SQLITE(self, database, **kwargs):
```

### Comparing `DE_DataBaseConnect-0.0.66/Licence.txt` & `DE_DataBaseConnect-0.0.67/Licence.txt`

 * *Files identical despite different names*

### Comparing `DE_DataBaseConnect-0.0.66/README.md` & `DE_DataBaseConnect-0.0.67/README.md`

 * *Files identical despite different names*

