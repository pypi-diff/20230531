# Comparing `tmp/ODAMNet-1.0.2.tar.gz` & `tmp/ODAMNet-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ODAMNet-1.0.2.tar", last modified: Tue Mar  7 10:10:28 2023, max compression
+gzip compressed data, was "ODAMNet-1.1.0.tar", last modified: Wed May 31 07:54:35 2023, max compression
```

## Comparing `ODAMNet-1.0.2.tar` & `ODAMNet-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 morgane   (1000) morgane   (1000)        0 2023-03-07 10:10:28.876909 ODAMNet-1.0.2/
--rw-rw-r--   0 morgane   (1000) morgane   (1000)     1074 2023-02-10 13:52:21.000000 ODAMNet-1.0.2/LICENSE
--rw-rw-r--   0 morgane   (1000) morgane   (1000)     6405 2023-03-07 10:10:28.876909 ODAMNet-1.0.2/PKG-INFO
--rw-rw-r--   0 morgane   (1000) morgane   (1000)     4401 2023-03-07 10:01:18.000000 ODAMNet-1.0.2/README.md
--rw-rw-r--   0 morgane   (1000) morgane   (1000)     1343 2023-03-07 10:10:09.000000 ODAMNet-1.0.2/pyproject.toml
--rw-rw-r--   0 morgane   (1000) morgane   (1000)       38 2023-03-07 10:10:28.876909 ODAMNet-1.0.2/setup.cfg
-drwxrwxr-x   0 morgane   (1000) morgane   (1000)        0 2023-03-07 10:10:28.876909 ODAMNet-1.0.2/src/
-drwxrwxr-x   0 morgane   (1000) morgane   (1000)        0 2023-03-07 10:10:28.876909 ODAMNet-1.0.2/src/ODAMNet.egg-info/
--rw-rw-r--   0 morgane   (1000) morgane   (1000)     6405 2023-03-07 10:10:28.000000 ODAMNet-1.0.2/src/ODAMNet.egg-info/PKG-INFO
--rw-rw-r--   0 morgane   (1000) morgane   (1000)      408 2023-03-07 10:10:28.000000 ODAMNet-1.0.2/src/ODAMNet.egg-info/SOURCES.txt
--rw-rw-r--   0 morgane   (1000) morgane   (1000)        1 2023-03-07 10:10:28.000000 ODAMNet-1.0.2/src/ODAMNet.egg-info/dependency_links.txt
--rw-rw-r--   0 morgane   (1000) morgane   (1000)       49 2023-03-07 10:10:28.000000 ODAMNet-1.0.2/src/ODAMNet.egg-info/entry_points.txt
--rw-rw-r--   0 morgane   (1000) morgane   (1000)      208 2023-03-07 10:10:28.000000 ODAMNet-1.0.2/src/ODAMNet.egg-info/requires.txt
--rw-rw-r--   0 morgane   (1000) morgane   (1000)        8 2023-03-07 10:10:28.000000 ODAMNet-1.0.2/src/ODAMNet.egg-info/top_level.txt
-drwxrwxr-x   0 morgane   (1000) morgane   (1000)        0 2023-03-07 10:10:28.876909 ODAMNet-1.0.2/src/odamnet/
--rwxrwxr-x   0 morgane   (1000) morgane   (1000)     8504 2023-02-13 10:02:12.000000 ODAMNet-1.0.2/src/odamnet/CTD_functions.py
--rwxrwxr-x   0 morgane   (1000) morgane   (1000)     9013 2023-02-20 09:40:09.000000 ODAMNet-1.0.2/src/odamnet/WP_functions.py
--rw-rw-r--   0 morgane   (1000) morgane   (1000)        0 2023-02-10 13:52:21.000000 ODAMNet-1.0.2/src/odamnet/__init__.py
--rwxr-xr-x   0 morgane   (1000) morgane   (1000)     1538 2023-02-10 13:52:21.000000 ODAMNet-1.0.2/src/odamnet/customClick.py
--rwxrwxr-x   0 morgane   (1000) morgane   (1000)    18811 2023-02-10 13:52:21.000000 ODAMNet-1.0.2/src/odamnet/methods_functions.py
--rwxr-xr-x   0 morgane   (1000) morgane   (1000)    17898 2023-02-13 10:51:35.000000 ODAMNet-1.0.2/src/odamnet/odamnet.py
+drwxrwxr-x   0 morgane   (1000) morgane   (1000)        0 2023-05-31 07:54:35.385061 ODAMNet-1.1.0/
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)     1074 2023-02-10 13:52:21.000000 ODAMNet-1.1.0/LICENSE
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)     6640 2023-05-31 07:54:35.385061 ODAMNet-1.1.0/PKG-INFO
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)     4633 2023-05-30 08:50:20.000000 ODAMNet-1.1.0/README.md
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)     1346 2023-05-31 07:53:16.000000 ODAMNet-1.1.0/pyproject.toml
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)       38 2023-05-31 07:54:35.385061 ODAMNet-1.1.0/setup.cfg
+drwxrwxr-x   0 morgane   (1000) morgane   (1000)        0 2023-05-31 07:54:35.317060 ODAMNet-1.1.0/src/
+drwxrwxr-x   0 morgane   (1000) morgane   (1000)        0 2023-05-31 07:54:35.317060 ODAMNet-1.1.0/src/ODAMNet.egg-info/
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)     6640 2023-05-31 07:54:35.000000 ODAMNet-1.1.0/src/ODAMNet.egg-info/PKG-INFO
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)      408 2023-05-31 07:54:35.000000 ODAMNet-1.1.0/src/ODAMNet.egg-info/SOURCES.txt
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)        1 2023-05-31 07:54:35.000000 ODAMNet-1.1.0/src/ODAMNet.egg-info/dependency_links.txt
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)       49 2023-05-31 07:54:35.000000 ODAMNet-1.1.0/src/ODAMNet.egg-info/entry_points.txt
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)      208 2023-05-31 07:54:35.000000 ODAMNet-1.1.0/src/ODAMNet.egg-info/requires.txt
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)        8 2023-05-31 07:54:35.000000 ODAMNet-1.1.0/src/ODAMNet.egg-info/top_level.txt
+drwxrwxr-x   0 morgane   (1000) morgane   (1000)        0 2023-05-31 07:54:35.377061 ODAMNet-1.1.0/src/odamnet/
+-rwxrwxr-x   0 morgane   (1000) morgane   (1000)     8522 2023-05-04 13:05:41.000000 ODAMNet-1.1.0/src/odamnet/CTD_functions.py
+-rwxrwxr-x   0 morgane   (1000) morgane   (1000)     8989 2023-05-10 09:47:46.000000 ODAMNet-1.1.0/src/odamnet/WP_functions.py
+-rw-rw-r--   0 morgane   (1000) morgane   (1000)        0 2023-02-10 13:52:21.000000 ODAMNet-1.1.0/src/odamnet/__init__.py
+-rwxr-xr-x   0 morgane   (1000) morgane   (1000)     1570 2023-05-04 13:07:47.000000 ODAMNet-1.1.0/src/odamnet/customClick.py
+-rwxrwxr-x   0 morgane   (1000) morgane   (1000)    19843 2023-05-04 13:16:44.000000 ODAMNet-1.1.0/src/odamnet/methods_functions.py
+-rwxrwxr-x   0 morgane   (1000) morgane   (1000)    19072 2023-05-10 13:46:21.000000 ODAMNet-1.1.0/src/odamnet/odamnet.py
```

### Comparing `ODAMNet-1.0.2/LICENSE` & `ODAMNet-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ODAMNet-1.0.2/PKG-INFO` & `ODAMNet-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ODAMNet
-Version: 1.0.2
-Summary: Study the link between environmental factors and rare diseases
+Version: 1.1.0
+Summary: Study molecular relationships between chemicals and rare diseases
 Author: Morgane Térézol
 License: MIT License
         
         Copyright (c) 2022 Morgane Térézol
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,23 +46,23 @@
 
 This tool was created within the framework of the [EJRP-RD project][EJPRD].
 
 ## Installation 
 
 ### From PyPI
 
-ODAMNet is available as [Python package][pypi]. You can easily install it using `pip`.
+ODAMNet is available in [Python package][pypi]. You can easily install it using `pip`.
 
 ```console
 $ python3 -m pip install odamnet
 ```
 
-### From Conda - *It's ongoing*
+### From Conda
 
-It is available in [bioconda][bioconda] too.
+ODAMNet is also available in [bioconda][bioconda] using ``conda``.
 
 ```console
 $ conda install odamnet
 ```
 
 ### From Github
 
@@ -85,26 +85,27 @@
 Three different approaches are available: 
 
 - Overlap analysis
 - Active Modules Identification (AMI, using [DOMINO][DOMINO])
 - Random Walk with Restart (RWR, using [multiXrank][multiXrank])
 
 ```console
-$ odamnet [overlap|domino|multixrank|networkCreation] [ARGS]
+$ odamnet [overlap|domino|multixrank|networkCreation|networkDownloading] [ARGS]
 ```
 
 ## Examples
 
-Three approaches are implemented to study relationships between genes targeted by chemicals (extracted automatically 
-from [CTD database][CTD]) and rare diseases (extracted automatically from [WikiPathways][WikiPathways]).
+Three approaches are implemented to study relationships between genes targeted by chemicals (retrieved automatically 
+from the [Comparative Toxicogenomics Database][CTD] (CTD)) and rare diseases (retrieved automatically from 
+[WikiPathways][WikiPathways]).
 
 ### Overlap analysis
 
-This method computes the overlap between target genes and rare disease pathways. It is looking for direct associations, 
-i.e., target genes that are part of rare disease pathways.
+The first approach computes the overlap between chemical target genes and rare disease pathways. It is looking for 
+direct associations, i.e. chemical target genes that are part of rare disease pathways.
 
 Give your chemicals list into `--chemicalsFile` input. 
 
 ```console
 $ odamnet overlap --chemicalsFile FILENAME
 ```
 
@@ -120,53 +121,57 @@
 
 ```console
 $ odamnet domino --chemicalsFile FILENAME --networkFile FILENAME
 ```
 
 ### Random Walk with Restart (RWR)
 
-The Random Walk with Restart is performed using multiXrank Python package.
+The Random Walk with Restart is performed using multiXrank Python package. This approach mesures the proximity of every node 
+(e.g. genes and diseases) to the target genes within a multilayer network. The multilayer network is composed of genes networks 
+and rare disease pathway network. Diseases and genes are linked using a bipartite.  
 
-#### Network and bipartite creation
-
-MultiXrank need networks as input. You need to create a network with the rare disease pathways. This network will not 
-have any connection between disease nodes (i.e. disconnected network). Disease nodes will be only connected with gene 
-nodes that are involved in disease pathways using a bipartite.  
+Give your chemicals list into `--chemicalsFile` input. 
 
-Give a path to save generated disease network and disease-gene bipartite using `--networksPath` and `--bipartitePath` 
-respectively.
+MultiXrank needs a configuration file (`--configPath`), networks directory (`--networksPath`),
+the target genes file (`--seedsFile`) and a name to write the result into network file (`--sifFileName`). 
 
 ```console
-$ odamnet networkCreation --networksPath PATH --bipartitePath PATH
+$ odamnet multixrank --chemicalsFile FILENAME --configPath PATH --networksPath PATH --seedsFile FILENAME --sifFileName FILENAME
 ```
 
-*Rare disease pathways are extracted automatically from WikiPathways.*
+*You can have more details about the configuration file in the [documentation page][doc].*
 
-#### multiXrank
+### Other functions
 
-Random Walk with Restart mesures the proximity of every node (e.g. genes and diseases) to the target genes within a 
-multilayer network. The multilayer network is composed of molecular multiplex and rare disease pathway network (the one 
-created previously). 
+#### Network and bipartite creation
 
-Give your chemicals list into `--chemicalsFile` input. 
+For the RWR, you should need to create a rare disease pathways network to integrate disease information into the multilayer.
+ODAMNet creates a disconnected network (no connection between disease nodes) and its corresponding bipartite that connects 
+diseases with genes that are involved in. 
 
-MultiXrank needs a configuration file (`--configPath`), networks directory (`--networksPath`),
-the target genes file (`--seedsFile`) and a name to write the result into network file (`--sifFileName`). 
+Give a path to save generated disease network and disease-gene bipartite using `--networksPath` and `--bipartitePath`
+respectively.
 
 ```console
-$ odamnet multixrank --chemicalsFile FILENAME --configPath PATH --networksPath PATH --seedsFile FILENAME --sifFileName FILENAME
+$ odamnet networkCreation --networksPath PATH --bipartitePath PATH
 ```
+*Rare disease pathways are retrieved automatically from WikiPathways.*
+
+#### Network downloading
 
-*We provide a molecular multiplex into the useCases directory in the [GitHub page][git].*
+ODAMNet allows you to download automatically biological networks from [NDEx][NDEx] using the network ID (`--netUUID`). 
+You can choose the network name file with `--networkFile`.
 
-*You can also have more details about the configuration file in the [documentation page][doc].*
+```console
+$ odamnet networkDownloading --netUUID TEXT --networkFile FILENAME
+```
 
 [ODAMNet documentation]: https://odamnet.readthedocs.io/
 [pypi]: https://pypi.org/project/ODAMNet/
 [bioconda]: https://bioconda.github.io/index.html
 [EJPRD]: https://www.ejprarediseases.org/
 [DOMINO]: http://domino.cs.tau.ac.il
 [multiXrank]: https://multixrank-doc.readthedocs.io/en/latest/index.html
 [WikiPathways]: https://www.wikipathways.org/
 [CTD]: https://ctdbase.org/
+[NDEx]: https://www.ndexbio.org/
 [doc]: https://odamnet.readthedocs.io/en/latest/pages/formats/Input.html#configuration-file
-[git]: https://github.com/MOohTus/ODAMNet/tree/main/useCases/InputData
```

### Comparing `ODAMNet-1.0.2/README.md` & `ODAMNet-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 This tool was created within the framework of the [EJRP-RD project][EJPRD].
 
 ## Installation 
 
 ### From PyPI
 
-ODAMNet is available as [Python package][pypi]. You can easily install it using `pip`.
+ODAMNet is available in [Python package][pypi]. You can easily install it using `pip`.
 
 ```console
 $ python3 -m pip install odamnet
 ```
 
-### From Conda - *It's ongoing*
+### From Conda
 
-It is available in [bioconda][bioconda] too.
+ODAMNet is also available in [bioconda][bioconda] using ``conda``.
 
 ```console
 $ conda install odamnet
 ```
 
 ### From Github
 
@@ -46,26 +46,27 @@
 Three different approaches are available: 
 
 - Overlap analysis
 - Active Modules Identification (AMI, using [DOMINO][DOMINO])
 - Random Walk with Restart (RWR, using [multiXrank][multiXrank])
 
 ```console
-$ odamnet [overlap|domino|multixrank|networkCreation] [ARGS]
+$ odamnet [overlap|domino|multixrank|networkCreation|networkDownloading] [ARGS]
 ```
 
 ## Examples
 
-Three approaches are implemented to study relationships between genes targeted by chemicals (extracted automatically 
-from [CTD database][CTD]) and rare diseases (extracted automatically from [WikiPathways][WikiPathways]).
+Three approaches are implemented to study relationships between genes targeted by chemicals (retrieved automatically 
+from the [Comparative Toxicogenomics Database][CTD] (CTD)) and rare diseases (retrieved automatically from 
+[WikiPathways][WikiPathways]).
 
 ### Overlap analysis
 
-This method computes the overlap between target genes and rare disease pathways. It is looking for direct associations, 
-i.e., target genes that are part of rare disease pathways.
+The first approach computes the overlap between chemical target genes and rare disease pathways. It is looking for 
+direct associations, i.e. chemical target genes that are part of rare disease pathways.
 
 Give your chemicals list into `--chemicalsFile` input. 
 
 ```console
 $ odamnet overlap --chemicalsFile FILENAME
 ```
 
@@ -81,53 +82,57 @@
 
 ```console
 $ odamnet domino --chemicalsFile FILENAME --networkFile FILENAME
 ```
 
 ### Random Walk with Restart (RWR)
 
-The Random Walk with Restart is performed using multiXrank Python package.
+The Random Walk with Restart is performed using multiXrank Python package. This approach mesures the proximity of every node 
+(e.g. genes and diseases) to the target genes within a multilayer network. The multilayer network is composed of genes networks 
+and rare disease pathway network. Diseases and genes are linked using a bipartite.  
 
-#### Network and bipartite creation
-
-MultiXrank need networks as input. You need to create a network with the rare disease pathways. This network will not 
-have any connection between disease nodes (i.e. disconnected network). Disease nodes will be only connected with gene 
-nodes that are involved in disease pathways using a bipartite.  
+Give your chemicals list into `--chemicalsFile` input. 
 
-Give a path to save generated disease network and disease-gene bipartite using `--networksPath` and `--bipartitePath` 
-respectively.
+MultiXrank needs a configuration file (`--configPath`), networks directory (`--networksPath`),
+the target genes file (`--seedsFile`) and a name to write the result into network file (`--sifFileName`). 
 
 ```console
-$ odamnet networkCreation --networksPath PATH --bipartitePath PATH
+$ odamnet multixrank --chemicalsFile FILENAME --configPath PATH --networksPath PATH --seedsFile FILENAME --sifFileName FILENAME
 ```
 
-*Rare disease pathways are extracted automatically from WikiPathways.*
+*You can have more details about the configuration file in the [documentation page][doc].*
 
-#### multiXrank
+### Other functions
 
-Random Walk with Restart mesures the proximity of every node (e.g. genes and diseases) to the target genes within a 
-multilayer network. The multilayer network is composed of molecular multiplex and rare disease pathway network (the one 
-created previously). 
+#### Network and bipartite creation
 
-Give your chemicals list into `--chemicalsFile` input. 
+For the RWR, you should need to create a rare disease pathways network to integrate disease information into the multilayer.
+ODAMNet creates a disconnected network (no connection between disease nodes) and its corresponding bipartite that connects 
+diseases with genes that are involved in. 
 
-MultiXrank needs a configuration file (`--configPath`), networks directory (`--networksPath`),
-the target genes file (`--seedsFile`) and a name to write the result into network file (`--sifFileName`). 
+Give a path to save generated disease network and disease-gene bipartite using `--networksPath` and `--bipartitePath`
+respectively.
 
 ```console
-$ odamnet multixrank --chemicalsFile FILENAME --configPath PATH --networksPath PATH --seedsFile FILENAME --sifFileName FILENAME
+$ odamnet networkCreation --networksPath PATH --bipartitePath PATH
 ```
+*Rare disease pathways are retrieved automatically from WikiPathways.*
+
+#### Network downloading
 
-*We provide a molecular multiplex into the useCases directory in the [GitHub page][git].*
+ODAMNet allows you to download automatically biological networks from [NDEx][NDEx] using the network ID (`--netUUID`). 
+You can choose the network name file with `--networkFile`.
 
-*You can also have more details about the configuration file in the [documentation page][doc].*
+```console
+$ odamnet networkDownloading --netUUID TEXT --networkFile FILENAME
+```
 
 [ODAMNet documentation]: https://odamnet.readthedocs.io/
 [pypi]: https://pypi.org/project/ODAMNet/
 [bioconda]: https://bioconda.github.io/index.html
 [EJPRD]: https://www.ejprarediseases.org/
 [DOMINO]: http://domino.cs.tau.ac.il
 [multiXrank]: https://multixrank-doc.readthedocs.io/en/latest/index.html
 [WikiPathways]: https://www.wikipathways.org/
 [CTD]: https://ctdbase.org/
+[NDEx]: https://www.ndexbio.org/
 [doc]: https://odamnet.readthedocs.io/en/latest/pages/formats/Input.html#configuration-file
-[git]: https://github.com/MOohTus/ODAMNet/tree/main/useCases/InputData
```

### Comparing `ODAMNet-1.0.2/pyproject.toml` & `ODAMNet-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ['setuptools>=59.8.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'ODAMNet'
 authors = [{name = "Morgane Térézol"}]
-version = '1.0.2'
-description = 'Study the link between environmental factors and rare diseases'
+version = '1.1.0'
+description = 'Study molecular relationships between chemicals and rare diseases'
 readme = {file = 'README.md', content-type = 'text/markdown'}
 requires-python = '>=3.9'
 license = {file = 'LICENSE'}
 keywords = [
 	'rare diseases',
         'overlap',
         'WikiPathways',
```

### Comparing `ODAMNet-1.0.2/src/ODAMNet.egg-info/PKG-INFO` & `ODAMNet-1.1.0/src/ODAMNet.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ODAMNet
-Version: 1.0.2
-Summary: Study the link between environmental factors and rare diseases
+Version: 1.1.0
+Summary: Study molecular relationships between chemicals and rare diseases
 Author: Morgane Térézol
 License: MIT License
         
         Copyright (c) 2022 Morgane Térézol
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,23 +46,23 @@
 
 This tool was created within the framework of the [EJRP-RD project][EJPRD].
 
 ## Installation 
 
 ### From PyPI
 
-ODAMNet is available as [Python package][pypi]. You can easily install it using `pip`.
+ODAMNet is available in [Python package][pypi]. You can easily install it using `pip`.
 
 ```console
 $ python3 -m pip install odamnet
 ```
 
-### From Conda - *It's ongoing*
+### From Conda
 
-It is available in [bioconda][bioconda] too.
+ODAMNet is also available in [bioconda][bioconda] using ``conda``.
 
 ```console
 $ conda install odamnet
 ```
 
 ### From Github
 
@@ -85,26 +85,27 @@
 Three different approaches are available: 
 
 - Overlap analysis
 - Active Modules Identification (AMI, using [DOMINO][DOMINO])
 - Random Walk with Restart (RWR, using [multiXrank][multiXrank])
 
 ```console
-$ odamnet [overlap|domino|multixrank|networkCreation] [ARGS]
+$ odamnet [overlap|domino|multixrank|networkCreation|networkDownloading] [ARGS]
 ```
 
 ## Examples
 
-Three approaches are implemented to study relationships between genes targeted by chemicals (extracted automatically 
-from [CTD database][CTD]) and rare diseases (extracted automatically from [WikiPathways][WikiPathways]).
+Three approaches are implemented to study relationships between genes targeted by chemicals (retrieved automatically 
+from the [Comparative Toxicogenomics Database][CTD] (CTD)) and rare diseases (retrieved automatically from 
+[WikiPathways][WikiPathways]).
 
 ### Overlap analysis
 
-This method computes the overlap between target genes and rare disease pathways. It is looking for direct associations, 
-i.e., target genes that are part of rare disease pathways.
+The first approach computes the overlap between chemical target genes and rare disease pathways. It is looking for 
+direct associations, i.e. chemical target genes that are part of rare disease pathways.
 
 Give your chemicals list into `--chemicalsFile` input. 
 
 ```console
 $ odamnet overlap --chemicalsFile FILENAME
 ```
 
@@ -120,53 +121,57 @@
 
 ```console
 $ odamnet domino --chemicalsFile FILENAME --networkFile FILENAME
 ```
 
 ### Random Walk with Restart (RWR)
 
-The Random Walk with Restart is performed using multiXrank Python package.
+The Random Walk with Restart is performed using multiXrank Python package. This approach mesures the proximity of every node 
+(e.g. genes and diseases) to the target genes within a multilayer network. The multilayer network is composed of genes networks 
+and rare disease pathway network. Diseases and genes are linked using a bipartite.  
 
-#### Network and bipartite creation
-
-MultiXrank need networks as input. You need to create a network with the rare disease pathways. This network will not 
-have any connection between disease nodes (i.e. disconnected network). Disease nodes will be only connected with gene 
-nodes that are involved in disease pathways using a bipartite.  
+Give your chemicals list into `--chemicalsFile` input. 
 
-Give a path to save generated disease network and disease-gene bipartite using `--networksPath` and `--bipartitePath` 
-respectively.
+MultiXrank needs a configuration file (`--configPath`), networks directory (`--networksPath`),
+the target genes file (`--seedsFile`) and a name to write the result into network file (`--sifFileName`). 
 
 ```console
-$ odamnet networkCreation --networksPath PATH --bipartitePath PATH
+$ odamnet multixrank --chemicalsFile FILENAME --configPath PATH --networksPath PATH --seedsFile FILENAME --sifFileName FILENAME
 ```
 
-*Rare disease pathways are extracted automatically from WikiPathways.*
+*You can have more details about the configuration file in the [documentation page][doc].*
 
-#### multiXrank
+### Other functions
 
-Random Walk with Restart mesures the proximity of every node (e.g. genes and diseases) to the target genes within a 
-multilayer network. The multilayer network is composed of molecular multiplex and rare disease pathway network (the one 
-created previously). 
+#### Network and bipartite creation
 
-Give your chemicals list into `--chemicalsFile` input. 
+For the RWR, you should need to create a rare disease pathways network to integrate disease information into the multilayer.
+ODAMNet creates a disconnected network (no connection between disease nodes) and its corresponding bipartite that connects 
+diseases with genes that are involved in. 
 
-MultiXrank needs a configuration file (`--configPath`), networks directory (`--networksPath`),
-the target genes file (`--seedsFile`) and a name to write the result into network file (`--sifFileName`). 
+Give a path to save generated disease network and disease-gene bipartite using `--networksPath` and `--bipartitePath`
+respectively.
 
 ```console
-$ odamnet multixrank --chemicalsFile FILENAME --configPath PATH --networksPath PATH --seedsFile FILENAME --sifFileName FILENAME
+$ odamnet networkCreation --networksPath PATH --bipartitePath PATH
 ```
+*Rare disease pathways are retrieved automatically from WikiPathways.*
+
+#### Network downloading
 
-*We provide a molecular multiplex into the useCases directory in the [GitHub page][git].*
+ODAMNet allows you to download automatically biological networks from [NDEx][NDEx] using the network ID (`--netUUID`). 
+You can choose the network name file with `--networkFile`.
 
-*You can also have more details about the configuration file in the [documentation page][doc].*
+```console
+$ odamnet networkDownloading --netUUID TEXT --networkFile FILENAME
+```
 
 [ODAMNet documentation]: https://odamnet.readthedocs.io/
 [pypi]: https://pypi.org/project/ODAMNet/
 [bioconda]: https://bioconda.github.io/index.html
 [EJPRD]: https://www.ejprarediseases.org/
 [DOMINO]: http://domino.cs.tau.ac.il
 [multiXrank]: https://multixrank-doc.readthedocs.io/en/latest/index.html
 [WikiPathways]: https://www.wikipathways.org/
 [CTD]: https://ctdbase.org/
+[NDEx]: https://www.ndexbio.org/
 [doc]: https://odamnet.readthedocs.io/en/latest/pages/formats/Input.html#configuration-file
-[git]: https://github.com/MOohTus/ODAMNet/tree/main/useCases/InputData
```

### Comparing `ODAMNet-1.0.2/src/odamnet/CTD_functions.py` & `ODAMNet-1.1.0/src/odamnet/CTD_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-@author: Morgane T.
+@author: Morgane Térézol.
 
 CTD functions
 
-Script to manage the input genes list reading.
-Genes list could come from
-- a chemical list and requested from CTD
+Manage the target genes list retrieval.
+Target genes list could come from:
+- a chemicals file and requested from CTD
 - a CTD file (file created by request CTD)
-- a list of interested genes
-
+- a list of target genes
 """
 
 # Libraries
 import requests
 import re
 from datetime import datetime
 from alive_progress import alive_bar
@@ -41,15 +40,15 @@
 
 
 def readCTDFile(CTDFile, nbPub, outputPath):
     """
     Read CTD file, created from a request.
 
     :param FILE CTDFile: Content of the CTD file
-    :param int nbPub: Minimum number of publications to keep an interaction
+    :param int nbPub: Minimum number of publications to keep a chemical-gene interaction
     :param PATH outputPath: Output path directory name
     :return:
         - **targetGenesDict** (*dict*) – Dictionary of genes for each chemical as query
     """
     # Parameters
     targetGenesList = []
     targetGenesDict = {}
@@ -86,25 +85,25 @@
 
     # Return
     return targetGenesDict
 
 
 def CTDrequest(chemName, association, outputPath, nbPub):
     """
-    Function to request CTD database.
+    Request CTD database.
 
-    Search all genes which interact with the chemical given in input.
+    Search all genes which interact with chemicals given in input.
     Could be several chemicals names in the same line. Analysis will be done like if it's only one chemical.
     If hierarchicalAssociations is used, chemical related to the chemical given in input are used as query.
     Focus on genes present in Homo sapiens.
 
-    :param str chemName: Chemical name of MeSH ids string
+    :param str chemName: Chemical name in MeSH ids string
     :param str association: Association name (hierarchicalAssociations or directAssociations)
     :param str outputPath: Folder path to save the results
-    :param int nbPub: Minimum number of publications to keep an interaction
+    :param int nbPub: Minimum number of publications to keep a chemical-gene interaction
 
     :return:
         - **homoGenesList** (*list*) – List of genes which interact with chemicals given in input (only Homo sapiens)
         - **chemMeSH** (*str*) – Composition of MeSH ID from chemicals given in input
     """
     # Parameters
     URL = 'http://ctdbase.org/tools/batchQuery.go'
@@ -173,15 +172,15 @@
     Make CTD request for each chemical present in the list given in input.
     Each element can be composed of one or more element.
     If several element, the analysis will be done like if there is only one chemical.
 
     :param list chemList: List of chemical to request to CTD (MeSH IDs or chemical names)
     :param str association: Association name (hierarchicalAssociations or directAssociations)
     :param str outputPath: Folder path to save the results
-    :param int nbPub: Minimum number of publications to keep an interaction
+    :param int nbPub: Minimum number of publications to keep a chemical-gene interaction
 
     :return:
         - **chemTargetsDict** (*dict*) – Dict composed of interaction genes list for each chemical
     """
     # Parameters
     chemTargetsDict = {}
 
@@ -195,15 +194,15 @@
 
     # Return
     return chemTargetsDict
 
 
 def targetGenesExtraction(chemicalsFile, directAssociations, outputPath, nbPub):
     """
-    Read environmental factor file
+    Read chemicals file
     Request CTD and extract target genes
     Save results into output file
     Return the gene targets list
 
     :param FILE chemicalsFile: Content of the chemicals file list
     :param bool directAssociations: Chemical only or descendants too
     :param PATH outputPath: Folder path name to save results
```

### Comparing `ODAMNet-1.0.2/src/odamnet/WP_functions.py` & `ODAMNet-1.1.0/src/odamnet/WP_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 @author: Morgane T.
 
 WikiPathways functions
 """
 
 # Libraries
 import os.path
-import shutil as shutil
 from SPARQLWrapper import SPARQLWrapper, TSV
 from datetime import datetime
 from alive_progress import alive_bar
 
 
 # Functions
 def readRequestResultsWP(WPrequestResult):
```

### Comparing `ODAMNet-1.0.2/src/odamnet/customClick.py` & `ODAMNet-1.1.0/src/odamnet/customClick.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-@author: Morgane T.
+@author: Morgane Térézol.
 
 Custom click class to add some functionalities.
 """
 
+# Libraries
 import click
 
 # From : https://stackoverflow.com/questions/44247099/click-command-line-interfaces-make-options-required-if-other-optional-option-is
 # From : https://github.com/pallets/click/issues/513
 
 
+# Functions
 class RequiredIf(click.Option):
     """
     Add new parameter : RequiredIf
     Check if two parameters are given together.
     """
     def __init__(self, *args, **kwargs):
         self.required_if = kwargs.pop('required_if')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ODAMNet-1.0.2/src/odamnet/methods_functions.py` & `ODAMNet-1.1.0/src/odamnet/methods_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-@author: Morgane T. and Ozan O.
+@author: Morgane Térézol. and Ozan Ozisik.
 
-Script of methods that we can apply to CTD and WP lists
-Adapted from overlapAnalysis.py from Ozan O. (Paper vitamin A)
+Methods can be applied to CTD and WP lists
+Adapted from overlapAnalysis.py from Ozisik et al., 2021
 """
 
 # Libraries
 import json
 import ndex2
 import requests
 import os
@@ -111,15 +111,15 @@
     # print('\tOverlap analysis done!')
     # return df
 
 
 def overlapAnalysis(targetGenesDict, pathOfInterestGenesDict, pathOfInterestNamesDict, pathwaysOfInterestList,
                     backgroundGenesDict, outputPath, analysisName):
     """
-    For each chemical given in input, calculate overlap.rst with RD WP.
+    Calculate overlap between target genes and pathways of interest.
 
     :param dict targetGenesDict: Dict composed of interaction genes list for each chemical
     :param dict pathOfInterestGenesDict: Dict of pathways of interest genes
     :param dict pathOfInterestNamesDict: Dict of pathways of interest names
     :param list pathwaysOfInterestList: Pathways of interest list and their associated background name
     :param list backgroundGenesDict: Dict of background genes
     :param str outputPath: Folder path to save the results
@@ -135,42 +135,51 @@
                 featureName=chem,
                 outputPath=outputPath,
                 analysisName=analysisName)
 
 
 def RWR(configPath, networksPath, outputPath, sifPathName, top):
     """
-    Perform a Random Walk with Restart analysis on different multiplex and networks.
+    Perform a Random Walk with Restart analysis using multilayers.
     You have to specify seeds and networks.
 
     :param str configPath: Configuration file name path
     :param str networksPath: Networks path name
     :param str outputPath: Output folder path name
     :param str sifPathName: Result file name path to write SIF result file
-    :param int top: Number of results to report in SIF file
+    :param int top: Number of top results to report
     """
+    # Parameters
+    outputFileName = outputPath + "/RWR_top" + str(top) + ".txt"
+
     # Analysis
     with alive_bar(title='Random walks through the networks', theme='musical') as bar:
         multixrank_obj = multixrank.Multixrank(config=configPath, wdir=networksPath)
         ranking_df = multixrank_obj.random_walk_rank()
         multixrank_obj.write_ranking(ranking_df, path=outputPath)
         multixrank_obj.to_sif(ranking_df, path=sifPathName, top=top)
         bar()
 
+    # Select top of disease
+    disease_df = ranking_df[ranking_df['multiplex'] == "2"]
+    disease_df_sort = disease_df.sort_values(by=['score'], ascending=False)
+    disease_df_sort = disease_df_sort.drop(columns=['multiplex', 'layer'])
+    disease_df_sort[0:top].to_csv(outputFileName, index=False, sep='\t')
+
 
 def DOMINO(genesFileName, networkFileName, outputPath, featureName):
     """
     Run active modules identification analysis on the DOMINO server
 
     :param genesFileName: Active genes file name (g.e. list of genes of interest)
     :param networkFileName: Network file name
     :param outputPath: Output path name to save the results
     :param featureName: Feature name (g.e. chemical name)
     :return:
-        - **activeModulesDict** (*dict*) – Dict of active modules identified
+        - **activeModules_list** (*list*) – list of active modules identified
     """
     # Input file names
     data_dict = {
         'Network file name': os.path.basename(networkFileName),
         'Active gene file name': os.path.basename(genesFileName)
     }
     # Input file contents
@@ -215,16 +224,16 @@
     # Return
     return activeModules_list
 
 
 def DOMINOandOverlapAnalysis(featuresDict, networkFileName, pathOfInterestGenesDict, pathOfInterestNamesDict,
                              pathwaysOfInterestList, backgroundGenesDict, outputPath, analysisName):
     """
-    For each genes list, run an active module identification.
-    For each AM identified, run an overlap analysis against the pathways of interest.
+    Run an active module identification for each target genes list
+    Run an overlap analysis between identified active module and pathways of interest.
 
     :param featuresDict: Dict of list of genes
     :param networkFileName: Content of network file
     :param pathOfInterestGenesDict: Genes dict of pathways of interest
     :param pathOfInterestNamesDict: Names dict of pathways of interest
     :param pathwaysOfInterestList: List of pathways of interest and their bg name associated
     :param backgroundGenesDict: Dict of background genes
@@ -261,17 +270,25 @@
         # Output
         AMIFileName = outputPath + '/DOMINO_' + featureName + '_activeModules.txt'
         DOMINOOutput(networkFileName, AMIFileName, featureName, outputPath)
         print(featureName + ' analysis done!\n')
 
 
 def DOMINOOutput(networkFileName, AMIFileName, featureName, outputPath):
+    """
+    Create output file of the active module identification analysis
+
+    :param networkFileName: Content of network file
+    :param AMIFileName: AMI results file name
+    :param featureName: chemical ID
+    :param outputPath: Output path name to save results
+    """
     # Output file name
     AMoutput = outputPath + '/DOMINO_' + featureName + '_activeModules.txt'
-    metricsOutput = outputPath + '/DOMINO_' + featureName + '_activeModulesNetworkMetrics.txt'
+    metricsOutput = outputPath + '/DOMINO_' + featureName + '_activeModulesMetrics.txt'
     networkOutput = outputPath + '/DOMINO_' + featureName + '_activeModulesNetwork.txt'
     overlapOutput = outputPath + '/DOMINO_' + featureName + '_overlapAMresults4Cytoscape.txt'
     pathwaysOverlapOutput = outputPath + '/DOMINO_' + featureName + '_signOverlap.txt'
     # Parameters
     AM_dict = {}
     edges_df = pd.DataFrame(columns=['source', 'target', 'link', 'AMI_number'])
     AMNumbersList = []
@@ -379,15 +396,15 @@
                                    'ActiveGenesNumber': list(activeGenesDict.values())})
     metrics_df = pd.merge(metrics_df, activeGenes_df, on='AMINumber')
     metrics_df.to_csv(metricsOutput, index=False, sep='\t')
 
 
 def createNetworkandBipartiteFiles(bipartiteName, networkName, pathOfInterestGenesDict):
     """
-    Create a bipartite between genes symbols and pathways of interest
+    Create a bipartite between target genes and pathways of interest
     Create a disconnected network between pathways of interest
 
     :param filename bipartiteName: Bipartite file name
     :param FILENAME networkName: Network file name
     :param dict pathOfInterestGenesDict: Dict of pathways of interest
     """
     # Parameters
@@ -409,29 +426,38 @@
     # Write ID and ID into network file
     with open(networkName, 'w') as networkOutputFile:
         for ID in pathwayIDs:
             networkOutputFile.write('\t'.join([ID, ID]))
             networkOutputFile.write('\n')
 
 
-def downloadNDExNetwork(networkUUID, outputFileName):
+def downloadNDExNetwork(networkUUID, outputFileName, simplify):
     """
     Download network from NDEx website
+    Create a tab separated file with three columns: node1, interaction type and node2
+    With header (SIF format)
 
     :param str networkUUID: Network ID
     :param FILENAME outputFileName: SIF file name to write network
+    :param boolean simplify: if True, remove header and the interaction column
     """
     # Create NDEx2 python client
     client = ndex2.client.Ndex2()
 
     # Download
     client_resp = client.get_network_as_cx_stream(networkUUID)
 
     # Convert downloaded network to NiceCXNetwork object
+    print('\nExtract network with UUID : ' + networkUUID)
     net_cx = ndex2.create_nice_cx_from_raw_cx(json.loads(client_resp.content))
-    print('Extract network with UUID : ' + networkUUID)
     net_cx.print_summary()
 
     # Convert to pandas dataframe
     df = net_cx.to_pandas_dataframe()
     df.columns = ['node_1', 'link', 'node_2']
-    df.to_csv(outputFileName, index=False, sep='\t', na_rep='linked')
+
+    # True - Remove interaction columns + header
+    if simplify:
+        df = df.drop(columns=['link'])
+        df.to_csv(outputFileName, index=False, header=False, sep='\t')
+    else:
+        df.to_csv(outputFileName, index=False, sep='\t', na_rep='linked')
```

### Comparing `ODAMNet-1.0.2/src/odamnet/odamnet.py` & `ODAMNet-1.1.0/src/odamnet/odamnet.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,34 +17,41 @@
 # Libraries
 import os
 import click
 from click_option_group import optgroup, RequiredMutuallyExclusiveOptionGroup
 import odamnet.customClick as customClick
 from alive_progress import alive_bar
 import shutil as shutil
-import importlib.metadata
+from importlib import metadata
 
 # Script version
-__version__ = importlib.metadata.version(__package__ or __name__)
+__version__ = metadata.version(__package__ or __name__)
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
 @click.group(context_settings=CONTEXT_SETTINGS, cls=customClick.NaturalOrderGroup)
 @click.version_option(__version__)
 def main():
     """
-    [OPTIONS] = overlap | domino | multixrank | networkCreation
+    [OPTIONS] =
+    overlap | domino | multixrank | networkCreation | networkDownloading
 
-    Analyse the relationship between chemicals and Rare Diseases.
+    Analyse the molecular relationships between chemicals and rare diseases.
     Select the approach you want to perform:
 
-    overlap | domino | multixrank
+    odamnet [overlap | domino | multixrank] -h
 
-    If you need to create a network with the pathways of interest, select : networkCreation
+    To create a pathways/processes network and its bipartite network:
+
+    odamnet networkCreation -h
+
+    To download networks from NDEx:
+
+    odamnet networkDownloading -h
     """
     pass
 
 
 @main.command(short_help='Overlap analysis', context_settings=CONTEXT_SETTINGS)
 @optgroup.group('Extract target genes list from', cls=RequiredMutuallyExclusiveOptionGroup, help='Choice the way to extract target genes')
 @optgroup.option('-c', '--chemicalsFile', 'chemicalsFile', type=click.File(), help='Chemicals file name')
@@ -59,15 +66,15 @@
               help='Pathways of interest file name (GMT file)\n')
 @click.option('--backgroundFile', 'backgroundFile', type=click.File(), cls=customClick.RequiredIf,
               required_if='pathOfInterestGMT', help='Background genes file name\n')
 @click.option('-o', '--outputPath', 'outputPath', type=click.Path(), default='OutputResults', show_default=True,
               help='Output folder name to save results')
 def overlap(chemicalsFile, CTD_file, targetGenesFile, directAssociation, nbPub, pathOfInterestGMT, backgroundFile, outputPath):
     """
-    Perform overlap analysis between genes targeted by chemicals and Rare Diseases pathways.
+    Perform Overlap analysis between genes targeted by chemicals and rare diseases pathways.
     """
     # Parameters
     outputPath = os.path.join(outputPath, 'OutputOverlapResults')
     featuresDict = {}
     pathwaysOfInterestList = []
 
     # Check if outputPath exist and create it if it does not exist
@@ -129,16 +136,19 @@
 @click.option('--backgroundFile', 'backgroundFile', type=click.File(), cls=customClick.RequiredIf,
               required_if='pathOfInterestGMT', help='Background genes file name\n')
 @click.option('-o', '--outputPath', 'outputPath', type=click.Path(), default='OutputResults', show_default=True,
               help='Output folder name to save results')
 def DOMINO(chemicalsFile, CTD_file, targetGenesFile, networkFileName, networkUUID, directAssociation, nbPub, pathOfInterestGMT, backgroundFile,
            outputPath):
     """
-    DOMINO defines target genes as active genes and search active modules (AM) through a given network.
-    For each AM, an overlap analysis is performed against RD pathways (or pathways of interest).
+    Perform Active module identification analysis between genes targeted by chemicals and rare diseases pathways using
+    DOMINO.
+
+    1. DOMINO on network using target genes as seed
+    2. Overlap analysis between identified active modules and rare disease pahtways
     """
     # Parameters
     outputPath = os.path.join(outputPath, 'OutputDOMINOResults')
     featuresDict = {}
     pathwaysOfInterestList = []
 
     # Check if outputPath exist and create it if it does not exist
@@ -148,15 +158,15 @@
     # Extract network from NDEx website
     if os.path.exists(networkFileName):
         if networkUUID:
             print('Network File already exists. Give only file name (without network UUID) or rename/remove file.')
             exit()
     else:
         if networkUUID:
-            methods.downloadNDExNetwork(networkUUID=networkUUID, outputFileName=networkFileName)
+            methods.downloadNDExNetwork(networkUUID=networkUUID, outputFileName=networkFileName, simplify=False)
         else:
             print('Network file doesn\'t exist. Add the network UUID to request NEDx or give another network file.')
             exit()
 
     # Extract genes from background and pathways of interest
     if pathOfInterestGMT:
         # Files reading
@@ -192,60 +202,14 @@
                                      pathOfInterestNamesDict=pathOfInterestNamesDict,
                                      pathwaysOfInterestList=pathwaysOfInterestList,
                                      backgroundGenesDict=backgroundGenesDict,
                                      outputPath=outputPath,
                                      analysisName=analysisName)
 
 
-@main.command('networkCreation', short_help='Network and its bipartite creation', context_settings=CONTEXT_SETTINGS)
-@click.option('--networksPath', 'networksPath', type=click.Path(), required=True,
-              help='Output path to save the network')
-@click.option('--networksName', 'networksName', type=str, default='WP_RareDiseasesNetwork.sif', show_default=True,
-              metavar='FILENAME', help='Network output name')
-@click.option('--bipartitePath', 'bipartitePath', type=click.Path(), required=True,
-              help='Output path to save the bipartite')
-@click.option('--bipartiteName', 'bipartiteName', type=str, default='Bipartite_WP_RareDiseases_geneSymbols.tsv',
-              show_default=True, metavar='FILENAME', help='Bipartite output name')
-@click.option('--GMT', 'pathOfInterestGMT', type=click.File(),
-              help='Pathways of interest in GMT like format (e.g. from WP request).')
-@click.option('-o', '--outputPath', 'outputPath', type=click.Path(), default='OutputResults', show_default=True,
-              help='Output path name (for complementary output files)')
-def createNetworkFiles(pathOfInterestGMT, networksPath, networksName, bipartitePath, bipartiteName, outputPath):
-    """
-    Creates network SIF file from WP request or pathways of interest given in GMT file.
-    """
-    # Parameters
-    outputPath = os.path.join(outputPath, 'OutputCreateNetwork')
-    networkFileName = networksPath + '/' + networksName
-    bipartiteFileName = bipartitePath + '/' + bipartiteName
-
-    # Check if outputPath exist and create it if it does not exist
-    if not os.path.exists(outputPath):
-        os.makedirs(outputPath, exist_ok=True)
-    # Check if networksPath exist and create it if it does not exist
-    if not os.path.exists(networksPath):
-        os.makedirs(networksPath, exist_ok=True)
-    # Check if bipartitePath exist and create it if it does not exist
-    if not os.path.exists(bipartitePath):
-        os.makedirs(bipartitePath, exist_ok=True)
-
-    # Extract pathways of interest
-    if pathOfInterestGMT:
-        # From file
-        pathOfInterestGenesDict, pathOfInterestNamesDict, pathwaysOfInterestList = WP.readGMTFile(GMTFile=pathOfInterestGMT)
-    else:
-        # From request
-        pathOfInterestGenesDict, pathOfInterestNamesDict, pathwayOfInterestList = WP.rareDiseasesWPrequest(outputPath=outputPath)
-
-    # Create network and bipartite
-    methods.createNetworkandBipartiteFiles(bipartiteName=bipartiteFileName,
-                                           networkName=networkFileName,
-                                           pathOfInterestGenesDict=pathOfInterestGenesDict)
-
-
 @main.command(short_help='Random Walk with Restart analysis', context_settings=CONTEXT_SETTINGS)
 @optgroup.group('Extract target genes list from', cls=RequiredMutuallyExclusiveOptionGroup, help='Choice the way to extract target genes')
 @optgroup.option('-c', '--chemicalsFile', 'chemicalsFile', type=click.File(), help='Chemicals file name')
 @optgroup.option('-r', '--CTD_file', 'CTD_file', type=click.File(), help='CTD file name')
 @optgroup.option('-t', '--targetGenesFile', 'targetGenesFile', type=click.File(), help='Target genes file name')
 @click.option('--directAssociation', 'directAssociation', default=True, type=bool, show_default=True,
               help='True: Extract target genes from chemicals \n False: Extract target genes from chemicals + its child chemicals')
@@ -258,15 +222,15 @@
 @click.option('--top', 'top', type=int, default=10, show_default=True,
               help='Top number of results to write into output file')
 @click.option('-o', '--outputPath', 'outputPath', type=click.Path(), default='OutputResults', show_default=True,
               help='Output folder name to save results')
 def multiXrank(chemicalsFile, CTD_file, targetGenesFile, directAssociation, nbPub, configPath,
                networksPath, seedsFileName, outputPath, sifFileName, top):
     """
-    Performs a Random Walk with Restart analysis through heterogeneous multilayer using the target genes as seeds.
+    Performs a Random Walk with Restart analysis using multiXrank with genes and diseases multilayers.
     """
     # Parameters
     outputPath = os.path.join(outputPath, 'OutputMultiXRankResults')
     featuresDict = {}
     nodesList = []
 
     # Check if outputPath exist and create it if it does not exist
@@ -326,9 +290,73 @@
         # Run multiXrank
         shutil.copyfile(seedsFileName, analysisOutputPath + '/' + os.path.basename(seedsFileName))
         shutil.copyfile(configPath, analysisOutputPath + '/' + os.path.basename(configPath))
         methods.RWR(configPath=configPath, networksPath=networksPath, outputPath=analysisOutputPath,
                     sifPathName=sifPathName, top=top)
 
 
+@main.command('networkCreation', short_help='Network and its bipartite creation', context_settings=CONTEXT_SETTINGS)
+@click.option('--networksPath', 'networksPath', type=click.Path(), required=True,
+              help='Output path to save the network')
+@click.option('--networksName', 'networksName', type=str, default='WP_RareDiseasesNetwork.gr', show_default=True,
+              metavar='FILENAME', help='Network output name')
+@click.option('--bipartitePath', 'bipartitePath', type=click.Path(), required=True,
+              help='Output path to save the bipartite')
+@click.option('--bipartiteName', 'bipartiteName', type=str, default='Bipartite_WP_RareDiseases_geneSymbols.gr',
+              show_default=True, metavar='FILENAME', help='Bipartite output name')
+@click.option('--GMT', 'pathOfInterestGMT', type=click.File(),
+              help='Pathways of interest in GMT like format (e.g. from WP request).')
+@click.option('-o', '--outputPath', 'outputPath', type=click.Path(), default='OutputResults', show_default=True,
+              help='Output path name (for complementary output files)')
+def createNetworkFiles(pathOfInterestGMT, networksPath, networksName, bipartitePath, bipartiteName, outputPath):
+    """
+    Creates network (GR format) from WikiPathways request or pathways of interest given in GMT file.
+    """
+    # Parameters
+    outputPath = os.path.join(outputPath, 'OutputCreateNetwork')
+    networkFileName = networksPath + '/' + networksName
+    bipartiteFileName = bipartitePath + '/' + bipartiteName
+
+    # Check if outputPath exist and create it if it does not exist
+    if not os.path.exists(outputPath):
+        os.makedirs(outputPath, exist_ok=True)
+    # Check if networksPath exist and create it if it does not exist
+    if not os.path.exists(networksPath):
+        os.makedirs(networksPath, exist_ok=True)
+    # Check if bipartitePath exist and create it if it does not exist
+    if not os.path.exists(bipartitePath):
+        os.makedirs(bipartitePath, exist_ok=True)
+
+    # Extract pathways of interest
+    if pathOfInterestGMT:
+        # From file
+        pathOfInterestGenesDict, pathOfInterestNamesDict, pathwaysOfInterestList = WP.readGMTFile(GMTFile=pathOfInterestGMT)
+    else:
+        # From request
+        pathOfInterestGenesDict, pathOfInterestNamesDict, pathwayOfInterestList = WP.rareDiseasesWPrequest(outputPath=outputPath)
+
+    # Create network and bipartite
+    methods.createNetworkandBipartiteFiles(bipartiteName=bipartiteFileName,
+                                           networkName=networkFileName,
+                                           pathOfInterestGenesDict=pathOfInterestGenesDict)
+
+
+@main.command('networkDownloading', short_help='Download networks from NDEx', context_settings=CONTEXT_SETTINGS)
+@click.option('--netUUID', 'networkUUID', type=str, help='NDEx network ID', required=True)
+@click.option('--networkFile', 'networkFileName', type=str, metavar='FILENAME', required=True, help='Network file name')
+@click.option('--simple', 'simple', type=bool, default=False, help='Remove interaction column and header')
+def networkDownloading(networkUUID, networkFileName, simple):
+    """
+    Download networks from NDEx using the UUID network.
+    Create SIF (3 columns with header) or GR (2 columns without header) network
+    """
+    # Check if network already exist
+    if os.path.exists(networkFileName):
+        print('\nNetwork file already exists. Rename or remove network file.')
+        exit()
+
+    # Extract network from NDEx website
+    methods.downloadNDExNetwork(networkUUID=networkUUID, outputFileName=networkFileName, simplify=simple)
+
+
 if __name__ == '__main__':
     main()
```

