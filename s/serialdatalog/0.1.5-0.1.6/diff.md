# Comparing `tmp/serialdatalog-0.1.5.tar.gz` & `tmp/serialdatalog-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialdatalog-0.1.5.tar", max compression
+gzip compressed data, was "serialdatalog-0.1.6.tar", max compression
```

## Comparing `serialdatalog-0.1.5.tar` & `serialdatalog-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.5/README.md
--rw-r--r--   0        0        0      364 2023-05-30 21:01:24.762753 serialdatalog-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.5/serialdatalog/__init__.py
--rw-r--r--   0        0        0     5401 2023-05-30 21:01:19.519333 serialdatalog-0.1.5/serialdatalog/datalog.py
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.6/README.md
+-rw-r--r--   0        0        0      364 2023-05-31 10:19:42.063041 serialdatalog-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.6/serialdatalog/__init__.py
+-rw-r--r--   0        0        0     5871 2023-05-31 10:17:07.920329 serialdatalog-0.1.6/serialdatalog/datalog.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.6/PKG-INFO
```

### Comparing `serialdatalog-0.1.5/README.md` & `serialdatalog-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `serialdatalog-0.1.5/serialdatalog/datalog.py` & `serialdatalog-0.1.6/serialdatalog/datalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,32 @@
 clogger = logging.getLogger(__name__)
 def logger(
         table_dict,
         source="/dev/ttyACM0",
         dest="datalog.sqlite3",
         encoding='utf-8',
         timeout=10,
+        trigger=None,
     ):
     """Logs serial readings
 
     Args:
         table_dict (dict) : A dictionary containing the "table header" : "data type".
         source (string, optional) : Source port of the serial device.
             Defaults to "/dev/ttyACM0".
         dest (string, optional) : Destination database to write serial output to.
             Defaults to 'datalog.db'
         encoding (string, optional) : Encoding of serial device. 
             Defaults to 'utf-8'.
         timeout (float, optional) : Timeout for reading from the serial port.
             Defaults to 10.
+        trigger (bool object, optional) : An external trigger object that will only collect data if True.
+            It is expected to have the property value. That is, if trigger.value == True, the logger will
+            run. If trigger.value == False then the logger will stop.
+            Defaults to None. If None, no trigger will be used.
 
     Returns:
         return val (bool) : True if successful. False otherwise.
     """
 
     # Connects to source
     with serial.Serial(source, timeout=timeout) as ser:
@@ -42,15 +47,16 @@
         # Connects to database
         con = connect_to_database(dest)
         table_dict["Time_Stamp"] = "REAL"
         table_name = create_database(con, table_dict)
 
         # Loops over reading serial input
         with open(dest, "a") as f:
-            while True:
+            run = True
+            while run:
                 try:
                     line = ser.readline().decode(encoding)
                     clogger.info(line)
                     line = line.rstrip().split(",")
                     line.append(datetime.now().strftime('%y%m%d%H%M%S'))
                     data_dict = {
                         h : liteval(line[i]) for i, h in enumerate(list(table_dict.keys()))
@@ -61,14 +67,16 @@
                     clogger.debug(error)
                 except SyntaxError as error:
                     clogger.debug(error)
                 except UnicodeDecodeError as error:
                     clogger.debug(error)
                 except KeyboardInterrupt as error:
                     clogger.debug(error)
+                if trigger is not None:
+                    run = trigger.value
     clogger.info("Finished reading data.")
     return True
 
 def connect_to_database(database):
     """Connects to the SQLite database.
 
     Args:
```

### Comparing `serialdatalog-0.1.5/PKG-INFO` & `serialdatalog-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialdatalog
-Version: 0.1.5
+Version: 0.1.6
 Summary: Logs data coming from a serial port
 Author: Alex
 Author-email: adrysdale@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

