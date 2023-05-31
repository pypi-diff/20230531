# Comparing `tmp/db2ixf-0.1.0.tar.gz` & `tmp/db2ixf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2ixf-0.1.0.tar", last modified: Mon May 29 22:04:33 2023, max compression
+gzip compressed data, was "db2ixf-0.1.1.tar", last modified: Wed May 31 00:52:55 2023, max compression
```

## Comparing `db2ixf-0.1.0.tar` & `db2ixf-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:04:33.652548 db2ixf-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-29 22:03:22.000000 db2ixf-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-05-29 22:03:22.000000 db2ixf-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46701 2023-05-29 22:04:33.652548 db2ixf-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-29 22:03:22.000000 db2ixf-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-29 22:03:22.000000 db2ixf-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:04:33.652548 db2ixf-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-29 22:03:22.000000 db2ixf-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:04:33.648548 db2ixf-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:04:33.652548 db2ixf-0.1.0/src/db2ixf/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 22:04:33.000000 db2ixf-0.1.0/src/db2ixf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/ixf.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-29 22:03:22.000000 db2ixf-0.1.0/src/db2ixf/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:04:33.652548 db2ixf-0.1.0/src/db2ixf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46701 2023-05-29 22:04:33.000000 db2ixf-0.1.0/src/db2ixf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-29 22:04:33.000000 db2ixf-0.1.0/src/db2ixf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:04:33.000000 db2ixf-0.1.0/src/db2ixf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 22:04:33.000000 db2ixf-0.1.0/src/db2ixf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:04:32.000000 db2ixf-0.1.0/src/db2ixf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 22:04:33.000000 db2ixf-0.1.0/src/db2ixf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 22:04:33.000000 db2ixf-0.1.0/src/db2ixf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:52:55.524495 db2ixf-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-31 00:51:31.000000 db2ixf-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-05-31 00:51:31.000000 db2ixf-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-31 00:52:55.524495 db2ixf-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-05-31 00:51:31.000000 db2ixf-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-31 00:51:31.000000 db2ixf-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:52:55.524495 db2ixf-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 00:51:31.000000 db2ixf-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:52:55.524495 db2ixf-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:52:55.524495 db2ixf-0.1.1/src/db2ixf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/ixf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:52:55.524495 db2ixf-0.1.1/src/db2ixf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:52:54.000000 db2ixf-0.1.1/src/db2ixf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/top_level.txt
```

### Comparing `db2ixf-0.1.0/LICENSE` & `db2ixf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.0/pyproject.toml` & `db2ixf-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 name = 'db2ixf'
 authors = [
     { name = 'Ismail Hammounou', email = 'ismail.hammounou@gmail.com' },
 ]
 maintainers = [
     { name = 'Ismail Hammounou', email = 'ismail.hammounou@gmail.com' },
 ]
-description = 'Parsing and processing of IBM eXchange formats (IXF)'
+description = 'Parsing and processing of IBM eXchange format (IXF)'
 keywords = [
     'PC', 'IXF', 'IBM', 'DB2', 'Development', 'Tools', 'Package', 'Parsing',
     'Format'
 ]
-license = { file = "LICENSE" }
+license = { text = "AGPL-3.0" }
 requires-python = '>=3.7'
 dynamic = ['version', 'readme']
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU Affero General Public License v3',
     'Programming Language :: Python :: 3.7',
@@ -64,14 +64,15 @@
 include = ['db2ixf*']
 exclude = ['tests*', 'db2ixf.tests*']
 namespaces = true
 
 
 
 [tool.setuptools_scm]
+root = '.'
 write_to = 'src/db2ixf/_version.py'
 version_scheme = 'release-branch-semver'
 
 
 
 [tool.disutils]
 bdist_wheel.universal = true
```

### Comparing `db2ixf-0.1.0/src/db2ixf/__init__.py` & `db2ixf-0.1.1/src/db2ixf/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 """
 Helps the user to parse PC/IXF file format of IBM DB2.
 
 IXF file is organised in a sequence of records.
 these records have 5 main types: Header, Table, Column Descriptor, Data and Application.
 
 Inside the IXF file, these records are ordered which means that it starts with a header record,
-table one, set of column descriptors where each column descriptor is also a record
-then it ends with the set of data records.
+table one, set of column descriptors - where each column descriptor is also a record -
+ant it ends with the set of data records.
 
 IXF = H + T + Set(C) + Set(D).
 
 Each record type is represented by a list of fields and each field has a length in bytes that
 we will use to read data from the IXF file.
 
 For more information about record types; Please visit this
 [link](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-record-types).
 
 
-
-Data records stores the data we want to extract, which means that for each column we need
-to extract its content from the data record. Each column has its data type.
+Data records [Set(D)] stores the data we want to extract, which means that
+for each column we need to extract its content from the data record.
+Each column has its data type.
 
 For more information about data types; Please visit this
 [link](https://www.ibm.com/docs/en/db2/11.5?topic=format-pcixf-data-types).
 """
 from db2ixf.ixf import IXFParser
 
-
 __all__ = ['IXFParser']
```

### Comparing `db2ixf-0.1.0/src/db2ixf/cli.py` & `db2ixf-0.1.1/src/db2ixf/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,45 +21,46 @@
     name='db2ixf',
     rich_markup_mode="markdown",
     epilog='Made with heart :D'
 )
 
 
 @app.command(epilog='Made with heart :D')
-def json(file: Annotated[Path,
-                         typer.Argument(
-                             help='Path to the ixf FILE.',
-                             exists=True,
-                             dir_okay=False,
-                             resolve_path=True,
-                             rich_help_panel='Required Arguments',
-                         )],
-         output: Annotated[Union[Path, None],
-                           typer.Argument(
-                               help='Path to the `json` OUTPUT file.',
-                               dir_okay=False,
-                               readable=False,
-                               resolve_path=True,
-                               rich_help_panel='Optional Arguments',
-                           )] = None,
-         encoding: Annotated[Union[str, None],
-                             typer.Option(
-                                 '--encoding',
-                                 '-e',
-                                 help='IXF file encoding.',
-                                 rich_help_panel='Command Options',
-                             )] = 'latin-1',
-         verbose: Annotated[int,
+def json(
+        file: Annotated[Path,
+                        typer.Argument(
+                            help='Path to the ixf FILE.',
+                            exists=True,
+                            dir_okay=False,
+                            resolve_path=True,
+                            rich_help_panel='Required Arguments',
+                        )],
+        output: Annotated[Union[Path, None],
+                          typer.Argument(
+                              help='Path to the `json` OUTPUT file.',
+                              dir_okay=False,
+                              readable=False,
+                              resolve_path=True,
+                              rich_help_panel='Optional Arguments',
+                          )] = None,
+        encoding: Annotated[Union[str, None],
                             typer.Option(
-                                '--verbose',
-                                '-v',
-                                help='Verbosity level.',
-                                count=True,
-                            )] = 0,
-         ):
+                                '--encoding',
+                                '-e',
+                                help='IXF file encoding.',
+                                rich_help_panel='Command Options',
+                            )] = 'latin-1',
+        verbose: Annotated[int,
+                           typer.Option(
+                               '--verbose',
+                               '-v',
+                               help='Verbosity level.',
+                               count=True,
+                           )] = 0,
+):
     """
     Parse ixf ``FILE`` and convert it to a **json** ``OUTPUT``.
     """
     if output is None:
         output = Path.cwd()
         filename = file.name.lower().removesuffix('.ixf') + '.json'
         output /= filename
@@ -78,15 +79,16 @@
 
     parser = IXFParser(file, encoding)
     parser.to_json(output)
     raise typer.Exit()
 
 
 @app.command(epilog='Made with heart :D')
-def csv(file: Annotated[Path,
+def csv(
+        file: Annotated[Path,
                         typer.Argument(
                             help='Path to the ixf FILE.',
                             exists=True,
                             dir_okay=False,
                             resolve_path=True,
                             rich_help_panel='Required Arguments',
                         )],
@@ -115,15 +117,15 @@
         verbose: Annotated[int,
                            typer.Option(
                                '--verbose',
                                '-v',
                                help='Verbosity level.',
                                count=True,
                            )] = 0,
-        ):
+):
     """
     Parse ixf ``FILE`` and convert it to a **csv** ``OUTPUT``.
     """
     if output is None:
         output = Path.cwd()
         filename = file.name.lower().removesuffix('.ixf') + '.csv'
         output /= filename
@@ -146,62 +148,63 @@
 
     parser = IXFParser(file, encoding)
     parser.to_csv(output, str(sep))
     raise typer.Exit()
 
 
 @app.command(epilog='Made with heart :D')
-def parquet(file: Annotated[Path,
-                            typer.Argument(
-                                help='Path to the ixf FILE.',
-                                exists=True,
-                                dir_okay=False,
-                                resolve_path=True,
-                                rich_help_panel='Required Arguments',
-                            )],
-            output: Annotated[Union[Path, None],
-                              typer.Argument(
-                                  help='Path to the `parquet` OUTPUT file.',
-                                  dir_okay=False,
-                                  readable=False,
-                                  resolve_path=True,
-                                  rich_help_panel='Optional Arguments',
-                              )] = None,
-            encoding: Annotated[Union[str, None],
-                                typer.Option(
-                                    '--encoding',
-                                    '-e',
-                                    help='IXF file encoding.',
-                                    rich_help_panel='Command Options',
-                                )] = 'latin-1',
-            version: Annotated[Union[str, None],
-                               typer.Option(
-                                   '--version',
-                                   help='Parquet version. Please look '
-                                        'at pyarrow documentation.',
-                                   rich_help_panel='Command Options',
-                               )] = '1.0',
-            batch_size: Annotated[Union[int, None],
-                                  typer.Option(
-                                      '--batch-size',
-                                      '-s',
-                                      help='Size of the batch: number of '
-                                           'rows to extract before writing '
-                                           'to the parquet file, It is used '
-                                           'for memory optimization.',
-                                      rich_help_panel='Command Options',
-                                  )] = 500,
-            verbose: Annotated[int,
-                               typer.Option(
-                                   '--verbose',
-                                   '-v',
-                                   help='Verbosity level.',
-                                   count=True,
-                               )] = 0,
-            ):
+def parquet(
+        file: Annotated[Path,
+                        typer.Argument(
+                            help='Path to the ixf FILE.',
+                            exists=True,
+                            dir_okay=False,
+                            resolve_path=True,
+                            rich_help_panel='Required Arguments',
+                        )],
+        output: Annotated[Union[Path, None],
+                          typer.Argument(
+                              help='Path to the `parquet` OUTPUT file.',
+                              dir_okay=False,
+                              readable=False,
+                              resolve_path=True,
+                              rich_help_panel='Optional Arguments',
+                          )] = None,
+        encoding: Annotated[Union[str, None],
+                            typer.Option(
+                                '--encoding',
+                                '-e',
+                                help='IXF file encoding.',
+                                rich_help_panel='Command Options',
+                            )] = 'latin-1',
+        version: Annotated[Union[str, None],
+                           typer.Option(
+                               '--version',
+                               help='Parquet version. Please look '
+                                    'at pyarrow documentation.',
+                               rich_help_panel='Command Options',
+                           )] = '1.0',
+        batch_size: Annotated[Union[int, None],
+                              typer.Option(
+                                  '--batch-size',
+                                  '-s',
+                                  help='Size of the batch: number of '
+                                       'rows to extract before writing '
+                                       'to the parquet file, It is used '
+                                       'for memory optimization.',
+                                  rich_help_panel='Command Options',
+                              )] = 500,
+        verbose: Annotated[int,
+                           typer.Option(
+                               '--verbose',
+                               '-v',
+                               help='Verbosity level.',
+                               count=True,
+                           )] = 0,
+):
     """
     Parse ixf ``FILE`` and convert it to a **parquet** ``OUTPUT``.
     """
     if output is None:
         output = Path.cwd()
         filename = file.name.lower().removesuffix('.ixf') + '.parquet'
         output /= filename
@@ -234,24 +237,25 @@
 def version_callback(value: bool):
     if value:
         print(f"{__version__}")
         raise typer.Exit()
 
 
 @app.callback(invoke_without_command=True)
-def main(ctx: typer.Context,
-         version: Annotated[Optional[bool],
-                            typer.Option(
-                                '--version',
-                                '-v',
-                                help='Show the version of the CLI.',
-                                callback=version_callback,
-                                is_eager=True,
-                            )] = None
-         ):
+def main(
+        ctx: typer.Context,
+        version: Annotated[Optional[bool],
+                           typer.Option(
+                               '--version',
+                               '-v',
+                               help='Show the version of the CLI.',
+                               callback=version_callback,
+                               is_eager=True,
+                           )] = None
+):
     """
     A command-line tool (**CLI**) for parsing and converting IXF (IBM DB2
     Import/Export Format) files to various formats such as JSON, CSV, and
     Parquet. Easily parse and convert IXF files to meet your data processing
     needs.
     """
     cli = ctx.info_name
```

### Comparing `db2ixf-0.1.0/src/db2ixf/collectors.py` & `db2ixf-0.1.1/src/db2ixf/collectors.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.0/src/db2ixf/constants.py` & `db2ixf-0.1.1/src/db2ixf/constants.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.0/src/db2ixf/helpers.py` & `db2ixf-0.1.1/src/db2ixf/helpers.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.0/src/db2ixf/ixf.py` & `db2ixf-0.1.1/src/db2ixf/ixf.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.0/src/db2ixf/logger.py` & `db2ixf-0.1.1/src/db2ixf/logger.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.0/src/db2ixf.egg-info/SOURCES.txt` & `db2ixf-0.1.1/src/db2ixf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

