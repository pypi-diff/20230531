# Comparing `tmp/exergenics-etl-1.0.5.tar.gz` & `tmp/exergenics-etl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.0.5.tar", last modified: Fri May 26 06:43:02 2023, max compression
+gzip compressed data, was "exergenics-etl-1.0.6.tar", last modified: Wed May 31 03:25:23 2023, max compression
```

## Comparing `exergenics-etl-1.0.5.tar` & `exergenics-etl-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48486 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    35894 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-26 06:43:00.000000 exergenics-etl-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.090276 exergenics-etl-1.0.6/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.090276 exergenics-etl-1.0.6/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49892 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35886 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 03:25:18.000000 exergenics-etl-1.0.6/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 03:25:23.000000 exergenics-etl-1.0.6/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 03:25:23.094276 exergenics-etl-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-31 03:25:21.000000 exergenics-etl-1.0.6/setup.py
```

### Comparing `exergenics-etl-1.0.5/LICENSE` & `exergenics-etl-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.5/app/exergenics_etl/__init__.py` & `exergenics-etl-1.0.6/app/exergenics_etl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .src.exergenics_etl import (
+    EtlError,
     hello,
     create_api,
     create_sql_engine,
     get_time_now,
     structure_slack_message,
     create_tmp_folder,
     generate_CSV_name,
```

### Comparing `exergenics-etl-1.0.5/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.0.6/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,22 @@
                    'min', '25%', '50%', '75%', 'max']
 
 
 logger = Logger(loggerName='Exergenics-ETL',
                 component='python_package', subComponent='exergenics_etl')
 
 
+class EtlError(Exception):
+    """Exception raised for errors in ETL function."""
+
+    def __init__(self, message=""):
+        self.message = message
+        super().__init__(self.message)
+
+
 def hello(name: str) -> None:
     """Says hello to someone.
 
     Args:
         name (str): The name of the person to greet.
 
     Returns:
@@ -337,33 +345,36 @@
         A header should be a non-nan string only, ideally with a length greater than 5,
         and not a string of numbers.
 
         Args:
             df0 (pd.DataFrame): Pandas DataFrame for header validation.
 
         Raises:
-            AttributeError: Headers containing numbers cannot be skipped.
+            EtlError: If invalid column headers are found.
         """
 
         # Drop rows with NA in timestamps (the 1st column)
         df = df0[~pd.isna(df0[df0.columns[0]])]
 
         # Get all headers
         headers = df.iloc[0]
 
         # Validate each header
         for v in headers:
 
             try:
                 # Check header is a string but not a string of numbers
                 pd.to_numeric(v)
+
+                # Raise and log error
                 errorMessage = f"Test Failed: Can do to_numeric on header: {v} of type {type(v)}; \
                     the header can't be numbers, a string of numbers, an empty string, None, np.nan or boolean."
                 self.logger.error(errorMessage)
-                raise AttributeError(errorMessage)
+                userMessage = "Column names cannot be numbers, empty strings or True/False."
+                raise EtlError(userMessage)
 
             except ValueError as e:
                 pass
 
             try:
                 assert len(v) > 5, f'Expected the length of header to be ideally greater than 5 \
                     but the actual length of header "{v}" was {len(v)}'
@@ -403,17 +414,17 @@
                 self.logger.info(
                     f'Found skiprows value = {skiprowsTrial}')
                 return df, skiprows, headerRowID
 
             except:
                 continue
 
-        errorMessage = f"Table in data file should start at the first 10 rows. Faulty file: {fileName}."
+        errorMessage = f"Table in the data file should start at the first 10 rows."
         self.logger.error(errorMessage)
-        raise Exception(errorMessage)
+        raise EtlError(errorMessage)
 
     def _auto_skiprows_excel(self, fileName: str, zf: zipfile.ZipFile) -> Tuple[pd.DataFrame, int, int]:
         """Skip rows before headers for DataFrame read from an Excel sheet.
         Assume redundant stuffs in excel sheets are in the first column above timestamps.
         That is, the header of a data point is the first non-NA string in that column.
         Verify after skipping rows.
 
@@ -446,43 +457,48 @@
             fileName (str): File name of the file to apply skip rows.
             zf (zipfile.ZipFile): Zipped folder where the file is.
 
         Returns:
             pd.DataFrame: Pandas DataFrame of the input CSV file with skipped rows.  
         """
 
-        # Get the filename extension of the current data file
-        extension = [
-            extension for extension in EXTENSIONS if fileName.endswith(extension)][0]
-
-        if self.skiprows is None:
-            # Find skiprows value to read the data file
-            if extension == 'xlsx':
-                df, self.skiprows, headerRowId = self._auto_skiprows_excel(fileName, zf)
-            elif extension == 'csv':
-                df, self.skiprows, headerRowId = self._auto_skiprows_csv(fileName, zf)
-
-        else:
-            # Read the data file with the last skiprows value
-            if extension == 'csv':
-                df = pd.read_csv(zf.open(fileName), skiprows=self.skiprows, header=None)
-            elif extension == 'xlsx':
-                df = pd.read_excel(zf.open(fileName), skiprows=self.skiprows, header=None)
-            
-            headerRowId = 0
-
-        # Validate that headers are strings
-        self.validate_headers(df)
-
-        # Set header as column names
-        df.columns = df.loc[headerRowId].values
+        try:
+            # Get the filename extension of the current data file
+            extension = [
+                extension for extension in EXTENSIONS if fileName.endswith(extension)][0]
+
+            if self.skiprows is None:
+                # Find skiprows value to read the data file
+                if extension == 'xlsx':
+                    df, self.skiprows, headerRowId = self._auto_skiprows_excel(fileName, zf)
+                elif extension == 'csv':
+                    df, self.skiprows, headerRowId = self._auto_skiprows_csv(fileName, zf)
 
-        # Remove headers from values
-        df.drop(labels=headerRowId, inplace=True)
-        df.reset_index(inplace=True, drop=True)  # Replace and reset index
+            else:
+                # Read the data file with the last skiprows value
+                if extension == 'csv':
+                    df = pd.read_csv(zf.open(fileName), skiprows=self.skiprows, header=None)
+                elif extension == 'xlsx':
+                    df = pd.read_excel(zf.open(fileName), skiprows=self.skiprows, header=None)
+                
+                headerRowId = 0
+
+            # Validate that headers are strings
+            self.validate_headers(df)
+
+            # Set header as column names
+            df.columns = df.loc[headerRowId].values
+
+            # Remove headers from values
+            df.drop(labels=headerRowId, inplace=True)
+            df.reset_index(inplace=True, drop=True)  # Replace and reset index
+        
+        except Exception as e:
+            self.logger.error(e)
+            raise EtlError('Error in opening data file.')
 
         return df
 
 
 def convertable_to_float(string: str) -> bool:
     """Checks if a given string can be converted to a float.
 
@@ -514,15 +530,15 @@
         self.genericColumnHeaders = genericColumnHeaders
 
     def _validate_timestamp_column_header(self, df: pd.DataFrame) -> bool:
         """Assuming the first column is always timestamps,
         validate auto skiprows by checking if the first header is a valid header for timestamps.
 
         Raises:
-            AssertionError: Cannot find exact match for the timestamp column header.
+            EtlError: Cannot find exact match for the timestamp column header.
 
         Returns:
             bool: True if timestamp is in a correct format. 
         """
 
         logger = Logger()
 
@@ -532,21 +548,21 @@
             assert timestampHeader.lower() in self.validTimestampHeaders
         except AssertionError as e:
             logger.warn(
                 f"Cannot find exact match for this timestamp column header: {timestampHeader}.")
 
             try:
                 # Check if the timestamp column header of the current df is similar to any valid timestamp headers
-                msg = f"Cannot recognise this timestamp column header: {timestampHeader}. Either auto-skiprows is broken, or we should add this one into Column Header tree."
                 assert min([levenshtein_distance(timestampHeader.lower(), validTimestampHeader)
-                            for validTimestampHeader in self.validTimestampHeaders]) <= TIMESTAMP_HEADER_DISTANCE, msg
-            except AssertionError as e:
+                            for validTimestampHeader in self.validTimestampHeaders]) <= TIMESTAMP_HEADER_DISTANCE
+            except AssertionError:
                 logger.error(
                     f"Cannot find similar match for this timestamp column header: {timestampHeader}.")
-                raise AssertionError(e)
+                userMessage = "Cannot find timestamp column."
+                raise EtlError(userMessage)
 
         logger.info(
             'Verifying timestamp column header ... Timestamp header is VALID!')
         return True
 
     def _check_for_wide_format(self, df: pd.DataFrame) -> bool:
         """Method check whether input file is in a wide format.
@@ -575,33 +591,33 @@
         """Validate the format of a dataframe read from a data file.
 
         Args:
             df (pd.DataFrame): Pandas DataFrame to validate timestamp and 
             wide format. 
 
         Raises:
-            AssertionError: If any validation failed.
+            EtlError: If any validation failed.
             Exception: For unknown errors.
 
         Returns:
             bool: True if all validations are passed.
         """
 
         logger = Logger()
 
         try:
             self._validate_timestamp_column_header(df)
             assert self._check_for_wide_format(
-                df), 'This data file looks like in a long format. PreMerged can only accept datasets in a wide format.'
-        except AssertionError as e:
-            raise AssertionError(e)
+                df), 'This data file looks like in a long format. We currently only accept datasets in a wide format.'
+        except (AssertionError, EtlError) as e:
+            raise EtlError(e)
         except Exception as e:
             msg = f'Unknown error: {e}'
             logger.error(msg)
-            raise Exception(msg)
+            raise e
 
         return True
 
     def check_for_generic_header(self, pointName: str, dfSameName: pd.DataFrame, dfNew: pd.DataFrame) -> bool:
         """Check if the point name of a dataframe is from a generic header
         by comparing the time intervals (i.e. the modes of timestamp gaps)
         of the dataframes before and after concatenation.
@@ -614,52 +630,56 @@
             pointName (str): Point name to verify whether it is a generic header.
             dfSameName (pd.DataFrame): Pandas Dataframe in a long format containing values that have the same 
                 column header in the original data file as dfNew.
             dfNew (pd.DataFrame): Pandas Dataframe in a long format containing values that have the same 
                 column header in the original data file as dfSameName.
 
         Raises:
-            AssertionError: If the point name is considered generic.
+            EtlError: If the point name is considered generic.
 
         Returns:
             bool: False if the point name is not considered generic.
         """
 
         logger = Logger()
 
-        # Check if this is a generic column header we have seen before
-        assert pointName.lower(
-        ) not in self.genericColumnHeaders, f'A generic column header found: "{pointName}"'
-
-        # Check if this could be a generic column header we haven't seen before
-        if len(pointName) <= LENGTH_THRESHOLD:
-
-            msg = f'This point name has a length less than 10, which is possibly not a valid point name: "{pointName}"'
-            logger.warn(msg)
-
-            # If values are recorded in a similar behaviour in terms of time interval
-            oldTimeInterval = calculate_time_interval(dfSameName[TIME])
-            newTimeInterval = calculate_time_interval(dfNew[TIME])
-            if oldTimeInterval == newTimeInterval:
-
-                # Concatenate the two dataframes with the same point name
-                dfConcat = pd.concat([dfSameName, dfNew],
-                                     axis=0, ignore_index=True)
-                dfConcat.drop_duplicates(inplace=True, ignore_index=True)
-
-                # Check for a drop in time interval
-                timeIntervalAfterConcat = calculate_time_interval(
-                    dfConcat[TIME])
-                if timeIntervalAfterConcat < oldTimeInterval:
-                    msg = f'It\'s likely that there are two different points sharing the same column header: "{pointName}".'
-                    logger.error(
-                        f"{msg} because the time interval dropped after concatenating two dataframes.")
-                    raise AssertionError(msg)
+        try:
+            # Check if this is a generic column header we have seen before
+            assert pointName.lower(
+            ) not in self.genericColumnHeaders, f'Generic column name found: "{pointName}".'
+
+            # Check if this could be a generic column header we haven't seen before
+            if len(pointName) <= LENGTH_THRESHOLD:
+
+                msg = f'This point name has a length less than 10, which is possibly not a valid point name: "{pointName}"'
+                logger.warn(msg)
+
+                # If values are recorded in a similar behaviour in terms of time interval
+                oldTimeInterval = calculate_time_interval(dfSameName[TIME])
+                newTimeInterval = calculate_time_interval(dfNew[TIME])
+                if oldTimeInterval == newTimeInterval:
+
+                    # Concatenate the two dataframes with the same point name
+                    dfConcat = pd.concat([dfSameName, dfNew],
+                                        axis=0, ignore_index=True)
+                    dfConcat.drop_duplicates(inplace=True, ignore_index=True)
+
+                    # Check for a drop in time interval
+                    timeIntervalAfterConcat = calculate_time_interval(
+                        dfConcat[TIME])
+                    if timeIntervalAfterConcat < oldTimeInterval:
+                        msg = f'It\'s likely that there are two different points sharing the same column header: "{pointName}".'
+                        logger.error(
+                            f"{msg} because the time interval dropped after concatenating two dataframes.")
+                        raise EtlError(msg)
+            
+            return False
 
-        return False
+        except (AssertionError, EtlError) as e:
+            raise EtlError(str(e))
 
 
 def calculate_time_interval(dtSeries: pd.Series) -> str:
     """Calculate the time interval of a datetime series.
 
     Args:
         dtSeries (pandas.Series): A pandas series of datetime objects.
@@ -776,30 +796,30 @@
             # GET its year
             year = str(dtDf.loc[idx]["Dt Objects"].year)
 
             # SET the last two digits of year as shortYear
             shortYear = str(year)[-2:]
 
             # SPLIT the corresponding datetime string into chunks of strings by delimiters into a list
-            dateParts = self.delim.split(dtDf.loc[idx]['Dt Strings'])
+            dtString = dtDf.loc[idx]['Dt Strings']
+            dateParts = self.delim.split(dtString)
 
-            # GET the position of year in the list
+            # GET the positions of year in dateParts
             positions = [i for i, x in enumerate(dateParts) if x == year]
 
             # If year is not found
             if not positions:
 
-                # GET the position of shortYear in the list
+                # GET the position of shortYear in dateParts
                 positions = [i for i, x in enumerate(
                     dateParts) if x == shortYear]
 
                 if not positions:
-                    errorMessage = "Can't find year position!"
+                    errorMessage = f"Can't find year position in the current timestamp = {dtString}, neither 4-digit year or 2-digit year."
                     self.logger.warn(errorMessage)
-                    raise Exception(errorMessage)
 
                 else:
                     self.isShortYear = True
 
             # STORE the position to list positionsShortYears
             positionsYears += positions
 
@@ -807,17 +827,17 @@
 
         # GET the most common position of short year
         if positionsYears:
             countPositionsYears = Counter(positionsYears)
             self.positionYear = sorted(countPositionsYears.items(),
                                        key=lambda item: item[1], reverse=True)[0][0]
         else:
-            errorMessage = f"Cannot find where the position of year is."
+            errorMessage = f"Cannot find the position of year in timestamps."
             self.logger.error(errorMessage)
-            raise AttributeError(errorMessage)
+            raise EtlError(errorMessage)
 
         return
 
     def _find_day_position(self, dtSeries: pd.Series) -> int:
         """Find 50 timestamps with day > 12 as test cases and
         find the position of day.
 
@@ -889,16 +909,17 @@
                         self.formats['hm'])] = self.formats['hm_12']
                 except ValueError:
                     try:
                         formatCodeList[formatCodeList.index(
                             self.formats['hmsf'])] = self.formats['hmsf_12']
                     except ValueError:
                         errorMessage = 'AM/PM in timestamp but cannot find time!'
-                        self.logger.warn(errorMessage)
-                        raise ValueError(errorMessage)
+                        self.logger.error(errorMessage)
+                        userMessage = 'Cannot find time in timestamps.'
+                        raise EtlError(userMessage)
 
         return formatCodeList
 
     def _guess_one_format(self, datestring: str) -> str:
         """ Guess and return the timestamp format for a timestamp string. 
 
         Args:
@@ -953,15 +974,15 @@
 
                     # Append the format code for the current timestamp part to output
                     out.append(item)
 
                 except AttributeError:
                     errorMessage = f"Can't find a time part regex brick that matches with {part}"
                     self.logger.error(errorMessage)
-                    raise AttributeError(errorMessage)
+                    raise EtlError('Cannot recognise date parts.')
 
         out = self._correct_format_code_for_AMPM(out)
 
         # Check and filter out time zone from datetime format code
         out = self._check_and_remove_time_zone(parts, out)
 
         return "".join(out)
@@ -969,45 +990,44 @@
     def _find_final_format(self, dtSeries: pd.Series) -> str:
         """Get the format for the whole timestamp series. 
 
         Args:
             dtSeries (pd.Series): Pandas Series containing timestamp strings.
 
         Raises:
-            AttributeError: Unable to find datetime format.
+            EtlError: Unable to find datetime format.
 
         Returns:
             str: Most common time format as a string.
         """
 
         # FIND the most common format
         # FIND the positions of year and day
         try:
             self._find_short_year_position(dtSeries)
             self._find_day_position(dtSeries)
-        except Exception as e:
-            self.logger.error(e)
-            raise e
 
-        # SELECT self.nTests timestamps randomly as tests to find the format
-        dtTests = dtSeries.sample(n=self.nTests, replace=True)
-        try:
+            # SELECT self.nTests timestamps randomly as tests to find the format
+            dtTests = dtSeries.sample(n=self.nTests, replace=True)
             dtFormats = dtTests.apply(lambda x: self._guess_one_format(x))
-        except Exception as e:
-            errorMessage = f"Finding datetime format failed: {e}"
-            self.logger.error(errorMessage)
-            raise AttributeError(errorMessage)
 
-        countPossibleFormats = Counter(dtFormats)
+            countPossibleFormats = Counter(dtFormats)
 
-        # SAVE the most common format
-        self.dtFinalFormat = sorted(countPossibleFormats.items(),
-                                    key=lambda item: item[1], reverse=True)[0][0]
-        self.logger.info(
-            f'Datetime format found: {self.dtFinalFormat}')
+            # SAVE the most common format
+            self.dtFinalFormat = sorted(countPossibleFormats.items(),
+                                        key=lambda item: item[1], reverse=True)[0][0]
+            self.logger.info(
+                f'Datetime format found: {self.dtFinalFormat}')
+            
+        except EtlError as e:
+            self.logger.error(e)
+            raise EtlError(f'Unable to find datetime format. {str(e)}')
+        except Exception as e:
+            self.logger.error(e)
+            raise e
 
         # RETURN the most common format as a string
         return self.dtFinalFormat
 
     def _check_and_remove_time_zone(self, dateParts: list, out: str) -> str:
         """Check if time zones exist in timestamps. 
 
@@ -1042,15 +1062,16 @@
     def parse(self, dtSeries: pd.Series) -> pd.Series:
         """Parse input datetime string.
 
         Args:
             dtSeries (pd.Series): Pandas Seires of Datetime string to apply parsing.
 
         Raises:
-            Exception: Failed datetime parsing.
+            EtlError: Failed datetime parsing.
+            Exception: For unknown errors.
 
         Returns:
             pd.Series: Panda Series of parsed datetime objects.
         """
         self.dtSeriesTemp = dtSeries
         self.logger.info(
             f'Showing the first and the last 2 of the timestamps BEFORE parsing: \n{pd.concat([self.dtSeriesTemp.head(2), self.dtSeriesTemp.tail(2)])}')
@@ -1079,18 +1100,21 @@
                 self.isShortYear = False
                 self.containsTimeZone = False
 
                 self._find_final_format(self.dtSeriesTemp)
                 dtObjects = pd.to_datetime(
                     self.dtSeriesTemp, format=self.dtFinalFormat, exact=(not self.containsTimeZone))
                 self.logger.info('Second Parsing done')
-            except Exception as e:
+            except EtlError as e:
                 errorMessage = f'Second parsing failed: {e}'
                 self.logger.error(errorMessage)
-                raise Exception(errorMessage)
+                raise EtlError(f'Parsing timestamps failed. {str(e)}')
+            except Exception as e:
+                self.logger.error(e)
+                raise e
 
         # TODO: Check that the numbers of NaN in dtSeries and dtObjects are the same
 
         if self.containsTimeZone:
             self.logger.warn('Timestamps contain time zones!')
 
         # RETURN a pd.Series of datetime objects
@@ -1104,39 +1128,53 @@
     """Transform each column in the input dataframe to a new dataframe in long format.
 
     Args:
         wideDf (pd.DataFrame): Pandas Dataframe of a dataset with wide format.
         filesWithNanColumn (set): Set of files with NaN column.
         fileName (str): Absolute file path of dataset to be processed.
 
+    Raises:
+            EtlError: If duplicate column headers are found in a single data file and for unknown errors.
+
     Returns:
         Tuple[dict, set]: Dictionary of the new dataframe(s) and a set of files with NaN column.
     """
+    
+    logger = Logger()
+
+    try:
+        dfDictFile = {}
+
+        # Loop through all columns (point values) except the first column (where the timestamps should be)
+        for point in wideDf.columns[1:]:
 
-    dfDictFile = {}
+            # Get all non-na values for selected column as temp dataframe
+            tempDf = wideDf[wideDf[point].notna()][[TIME, point]].rename(
+                columns={point: VALUE})
 
-    # Loop through all columns (point values) except the first column (where the timestamps should be)
-    for point in wideDf.columns[1:]:
+            # Log the file name if the whole column is NaN
+            if not wideDf[point].notna().any():
+                filesWithNanColumn.add(fileName)
 
-        # Get all non-na values for selected column as temp dataframe
-        tempDf = wideDf[wideDf[point].notna()][[TIME, point]].rename(
-            columns={point: VALUE})
+            # Rename and reorder to fit raw data format
+            tempDf[NAME] = point  # point for every row
+            tempDf = tempDf[LOG_HEADER]  # Reorder the columns
 
-        # Log the file name if the whole column is NaN
-        if not wideDf[point].notna().any():
-            filesWithNanColumn.add(fileName)
+            tempDf.sort_values(TIME, inplace=True, ignore_index=True)
 
-        # Rename and reorder to fit raw data format
-        tempDf[NAME] = point  # point for every row
-        tempDf = tempDf[LOG_HEADER]  # Reorder the columns
+            assert point not in dfDictFile.keys(), f'Duplicate column header in a single data file.'
+            dfDictFile[point] = tempDf
 
-        tempDf.sort_values(TIME, inplace=True, ignore_index=True)
+    except AssertionError as e:
+        logger.error(e)
+        raise EtlError(str(e))
 
-        assert point not in dfDictFile.keys(), f'Duplicate column header in a single data file.'
-        dfDictFile[point] = tempDf
+    except Exception as e:
+        logger.error(e)
+        raise EtlError('Failed to preprocess columns.')
 
     return dfDictFile, filesWithNanColumn
 
 
 def get_point_summary(point: str, df: pd.DataFrame) -> pd.DataFrame:
     """Generate summary statistics of a point based on its trend log.
 
@@ -1279,19 +1317,26 @@
     Args:
         api (exergenics.ExergenicsApi): Exergenics Api object
         filePath (str): A local path for file needed to be uploaded
         jobId (int): The Id of selected job
         nodeName (str): The name of node in jobData
         removeFile (bool, optional): Remove local file after uploading or not. Defaults to True.
 
+    Raises:
+        EtlError: If no file exist in input file path.
     Returns:
         str: url for file uploaded
     """
+
+    logger = Logger()
+
     # Error out if no file exist in input file path
     if not os.path.isfile(filePath):
-        raise ValueError(f'No file existing in local path: {filePath}.')
+
+        logger.error(f'No file existing in local path: {filePath}.')
+        raise EtlError(f'No file existing in local path.')
 
     url2s3 = api.sendToBucket(filePath)
     if removeFile is True:
         os.remove(filePath)
     api.setJobData(jobId, nodeName, url2s3)
     return url2s3
```

### Comparing `exergenics-etl-1.0.5/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.0.6/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.5/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.0.6/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.5/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.0.6/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 import shutil
 import zipfile
 from ..src.logger import ETLLogger as Logger
 from dotenv import load_dotenv
 
 from ..src.exergenics_etl import (
+    EtlError,
     create_api,
     create_sql_engine,
     get_time_now,
     create_tmp_folder,
     generate_CSV_name,
     strftime_for_NaT,
     generate_one_manifest_row,
@@ -334,27 +335,27 @@
     def test_check_for_generic_header2(self, my_inputValidation_object):
         myDfSameName = pd.read_csv(
             'app/exergenics_etl/test/testData/dfSameName_genericHeader.csv', parse_dates=['timepretty'])
         myDfNew = pd.read_csv(
             'app/exergenics_etl/test/testData/dfNew_genericHeader.csv', parse_dates=['timepretty'])
         myPointName = 'Value'
 
-        with pytest.raises(AssertionError):
+        with pytest.raises(EtlError):
             my_inputValidation_object.check_for_generic_header(
                 myPointName, myDfSameName, myDfNew)
 
     def test_check_for_generic_header_new(self, my_inputValidation_object):
         """Check if the two dataframes share a generic name that is not in our known, generic header name list."""
         myDfSameName = pd.read_csv(
             'app/exergenics_etl/test/testData/dfSameName_newGenericHeader.csv', parse_dates=['timepretty'])
         myDfNew = pd.read_csv(
             'app/exergenics_etl/test/testData/dfNew_newGenericHeader.csv', parse_dates=['timepretty'])
         myPointName = 'Value'
 
-        with pytest.raises(AssertionError):
+        with pytest.raises(EtlError):
             my_inputValidation_object.check_for_generic_header(
                 myPointName, myDfSameName, myDfNew)
 
     @pytest.mark.parametrize("myTestTimestampHeader", ['timestamp', 'time stamp', 'ui::timestamp', 'ts', 'date', 'time', 'datetime', 'date/time'])
     def test_validate_timestamp_column_header(self, my_inputValidation_object, myTestTimestampHeader):
         myDf = pd.DataFrame(
             {myTestTimestampHeader: [],
@@ -553,15 +554,15 @@
 
     def test_parse_for_time_zone_handling(self, my_datetimeParser, my_test_case_time_zone_parsing):
         dtSeries, expected_output = my_test_case_time_zone_parsing
         dtObjects = my_datetimeParser.parse(dtSeries)
         assert expected_output.equals(dtObjects.astype(str))
 
     def test_parse_for_timestamps_with_unrecognisable_time_parts(self, my_datetimeParser, my_test_dtSeries_with_unrecognisable_time_parts):
-        with pytest.raises(AttributeError):
+        with pytest.raises(EtlError):
             my_datetimeParser.parse(
                 my_test_dtSeries_with_unrecognisable_time_parts)
 
     def test_correct_format_code_for_AMPM_with_seconds(self, my_datetimeParser, my_test_case_for_correcting_format_code_with_AMPM_and_seconds):
         """
         Test for the method, _correct_format_code_for_AMPM, in DatetimeParser.
         The method should be able replace %H:%M:%S with %I:%M:%S if %H:%M:%S and %p are parts of the datetime format.
@@ -584,15 +585,15 @@
     def test_correct_format_code_for_AMPM_but_no_time(self, my_datetimeParser, my_format_code_with_AMPM_but_no_time):
         """
         Test for the method, _correct_format_code_for_AMPM, in DatetimeParser.
         The method should raise error if %p is part of the datetime format
         but neither %H:%M:%S nor %H:%M can't be found.
         """
         my_format_code_list = my_format_code_with_AMPM_but_no_time
-        with pytest.raises(ValueError):
+        with pytest.raises(EtlError):
             my_datetimeParser._correct_format_code_for_AMPM(
                 my_format_code_list)
 
     @pytest.mark.parametrize("myTestMilliseconds", [".1", ".11", ".111", ".1111", ".11111", ".111111"])
     def test_parse_timestamp_with_milliseconds(self, my_datetimeParser, myTestMilliseconds):
         myTestTimestamp = "2022-05-15 05:05:01" + myTestMilliseconds
         myTestDtSeries = pd.Series([myTestTimestamp for i in range(10)])
@@ -765,10 +766,10 @@
 
     @pytest.fixture(scope='class')
     def my_removeFile(self):
         return False
 
     def test_save_missing_file_to_portal(self, my_api, my_filePath, my_jobId, my_nodeName, my_removeFile):
         """Test saving missing file to portal"""
-        with pytest.raises(ValueError):
+        with pytest.raises(EtlError):
             url2s3 = save_file_to_portal(
                 my_api, my_filePath, my_jobId, my_nodeName, my_removeFile)
```

### Comparing `exergenics-etl-1.0.5/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.0.6/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.5/setup.py` & `exergenics-etl-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.0.5",
+    version="v1.0.6",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

