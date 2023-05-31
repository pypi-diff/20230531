# Comparing `tmp/serialdatalog-0.1.6.tar.gz` & `tmp/serialdatalog-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialdatalog-0.1.6.tar", max compression
+gzip compressed data, was "serialdatalog-0.1.7.tar", max compression
```

## Comparing `serialdatalog-0.1.6.tar` & `serialdatalog-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.6/README.md
--rw-r--r--   0        0        0      364 2023-05-31 10:19:42.063041 serialdatalog-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.6/serialdatalog/__init__.py
--rw-r--r--   0        0        0     5871 2023-05-31 10:17:07.920329 serialdatalog-0.1.6/serialdatalog/datalog.py
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.7/README.md
+-rw-r--r--   0        0        0      364 2023-05-31 10:45:55.747388 serialdatalog-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.7/serialdatalog/__init__.py
+-rw-r--r--   0        0        0     5752 2023-05-31 10:33:23.030800 serialdatalog-0.1.7/serialdatalog/datalog.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.7/PKG-INFO
```

### Comparing `serialdatalog-0.1.6/README.md` & `serialdatalog-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `serialdatalog-0.1.6/serialdatalog/datalog.py` & `serialdatalog-0.1.7/serialdatalog/datalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,37 +46,36 @@
 
         # Connects to database
         con = connect_to_database(dest)
         table_dict["Time_Stamp"] = "REAL"
         table_name = create_database(con, table_dict)
 
         # Loops over reading serial input
-        with open(dest, "a") as f:
-            run = True
-            while run:
-                try:
-                    line = ser.readline().decode(encoding)
-                    clogger.info(line)
-                    line = line.rstrip().split(",")
-                    line.append(datetime.now().strftime('%y%m%d%H%M%S'))
-                    data_dict = {
-                        h : liteval(line[i]) for i, h in enumerate(list(table_dict.keys()))
-                    }
-                    add_to_database(con, data_dict, table_name)
+        run = True
+        while run:
+            if trigger is not None:
+                run = trigger.value
+            try:
+                line = ser.readline().decode(encoding)
+                clogger.info(line)
+                line = line.rstrip().split(",")
+                line.append(datetime.now().strftime('%y%m%d%H%M%S'))
+                data_dict = {
+                    h : liteval(line[i]) for i, h in enumerate(list(table_dict.keys()))
+                }
+                add_to_database(con, data_dict, table_name)
 
-                except IndexError as error:
-                    clogger.debug(error)
-                except SyntaxError as error:
-                    clogger.debug(error)
-                except UnicodeDecodeError as error:
-                    clogger.debug(error)
-                except KeyboardInterrupt as error:
-                    clogger.debug(error)
-                if trigger is not None:
-                    run = trigger.value
+            except IndexError as error:
+                clogger.debug(error)
+            except SyntaxError as error:
+                clogger.debug(error)
+            except UnicodeDecodeError as error:
+                clogger.debug(error)
+            except KeyboardInterrupt as error:
+                clogger.debug(error)
     clogger.info("Finished reading data.")
     return True
 
 def connect_to_database(database):
     """Connects to the SQLite database.
 
     Args:
```

### Comparing `serialdatalog-0.1.6/PKG-INFO` & `serialdatalog-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialdatalog
-Version: 0.1.6
+Version: 0.1.7
 Summary: Logs data coming from a serial port
 Author: Alex
 Author-email: adrysdale@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

