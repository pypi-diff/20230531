# Comparing `tmp/pard-0.6.0.0.tar.gz` & `tmp/pard-0.7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pard-0.6.0.0.tar", max compression
+gzip compressed data, was "pard-0.7.0.0.tar", max compression
```

## Comparing `pard-0.6.0.0.tar` & `pard-0.7.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      182 2022-10-23 20:05:25.206355 pard-0.6.0.0/pard/__init__.py
--rw-r--r--   0        0        0     1430 2022-10-23 20:03:40.655460 pard-0.6.0.0/pard/_handling_3_letter_code_decorator.py
--rw-r--r--   0        0        0   270377 2023-05-16 14:17:43.476006 pard-0.6.0.0/pard/_raw_python_dictionaries.py
--rw-r--r--   0        0        0     1124 2023-05-16 14:19:41.213205 pard-0.6.0.0/pard/empar.py
--rw-r--r--   0        0        0      845 2022-10-23 20:10:27.038271 pard-0.6.0.0/pard/epstein.py
--rw-r--r--   0        0        0     1722 2023-05-16 13:23:51.722407 pard-0.6.0.0/pard/experimental_exchangeability.py
--rw-r--r--   0        0        0      532 2022-10-23 20:10:27.034177 pard-0.6.0.0/pard/grantham.py
--rw-r--r--   0        0        0     1085 2023-05-16 13:25:23.144824 pard-0.6.0.0/pard/kolaskar.py
--rw-r--r--   0        0        0     5498 2023-02-27 17:05:25.237415 pard-0.6.0.0/pard/koshi_goldstein.py
--rw-r--r--   0        0        0      528 2022-10-23 20:10:27.053363 pard-0.6.0.0/pard/miyata.py
--rw-r--r--   0        0        0      526 2022-10-23 20:10:27.043726 pard-0.6.0.0/pard/sneath.py
--rw-r--r--   0        0        0      548 2023-05-16 14:23:09.261771 pard-0.6.0.0/pyproject.toml
--rw-r--r--   0        0        0    10177 2023-05-16 14:23:09.261771 pard-0.6.0.0/README.md
--rw-r--r--   0        0        0    10762 1970-01-01 00:00:00.000000 pard-0.6.0.0/setup.py
--rw-r--r--   0        0        0    10320 1970-01-01 00:00:00.000000 pard-0.6.0.0/PKG-INFO
+-rw-r--r--   0        0        0      268 2023-05-31 20:01:42.968972 pard-0.7.0.0/pard/__init__.py
+-rw-r--r--   0        0        0     1430 2022-10-23 20:03:40.655460 pard-0.7.0.0/pard/_handling_3_letter_code_decorator.py
+-rw-r--r--   0        0        0   270377 2023-05-16 14:17:43.476006 pard-0.7.0.0/pard/_raw_python_dictionaries.py
+-rw-r--r--   0        0        0     1124 2023-05-16 14:19:41.213205 pard-0.7.0.0/pard/empar.py
+-rw-r--r--   0        0        0      845 2022-10-23 20:10:27.038271 pard-0.7.0.0/pard/epstein.py
+-rw-r--r--   0        0        0     1722 2023-05-16 13:23:51.722407 pard-0.7.0.0/pard/experimental_exchangeability.py
+-rw-r--r--   0        0        0      532 2022-10-23 20:10:27.034177 pard-0.7.0.0/pard/grantham.py
+-rw-r--r--   0        0        0     1085 2023-05-16 13:25:23.144824 pard-0.7.0.0/pard/kolaskar.py
+-rw-r--r--   0        0        0     5498 2023-02-27 17:05:25.237415 pard-0.7.0.0/pard/koshi_goldstein.py
+-rw-r--r--   0        0        0      528 2022-10-23 20:10:27.053363 pard-0.7.0.0/pard/miyata.py
+-rw-r--r--   0        0        0      805 2023-05-31 20:03:00.605364 pard-0.7.0.0/pard/pairwise_distance.py
+-rw-r--r--   0        0        0      526 2022-10-23 20:10:27.043726 pard-0.7.0.0/pard/sneath.py
+-rw-r--r--   0        0        0      548 2023-05-31 20:13:11.223887 pard-0.7.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10177 2023-05-31 20:13:11.222877 pard-0.7.0.0/README.md
+-rw-r--r--   0        0        0    10762 1970-01-01 00:00:00.000000 pard-0.7.0.0/setup.py
+-rw-r--r--   0        0        0    10320 1970-01-01 00:00:00.000000 pard-0.7.0.0/PKG-INFO
```

### Comparing `pard-0.6.0.0/pard/_handling_3_letter_code_decorator.py` & `pard-0.7.0.0/pard/_handling_3_letter_code_decorator.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/_raw_python_dictionaries.py` & `pard-0.7.0.0/pard/_raw_python_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/empar.py` & `pard-0.7.0.0/pard/empar.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/epstein.py` & `pard-0.7.0.0/pard/epstein.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/experimental_exchangeability.py` & `pard-0.7.0.0/pard/experimental_exchangeability.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/grantham.py` & `pard-0.7.0.0/pard/grantham.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/kolaskar.py` & `pard-0.7.0.0/pard/kolaskar.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/koshi_goldstein.py` & `pard-0.7.0.0/pard/koshi_goldstein.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/miyata.py` & `pard-0.7.0.0/pard/miyata.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pard/sneath.py` & `pard-0.7.0.0/pard/sneath.py`

 * *Files identical despite different names*

### Comparing `pard-0.6.0.0/pyproject.toml` & `pard-0.7.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pard"
-version = "0.6.0.0"
+version = "0.7.0.0"
 description = "Physicochemical Amino acid Replacement Distances"
 authors = ["JasonMendoza2008 <lhotteromain@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "pard"},
 ]
```

### Comparing `pard-0.6.0.0/README.md` & `pard-0.7.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -211,27 +211,27 @@
 ### Citation
 If you use this software, please cite it as below.
 
 - APA:
 
 `
 Lhotte, R. & Taupin, J. (2022).
-Physicochemical Amino acid Replacement Distances (PARD) package (Version 0.6.0.0) [Computer software].
+Physicochemical Amino acid Replacement Distances (PARD) package (Version 0.7.0.0) [Computer software].
 https://doi.org/10.5281/zenodo.7013169
 `
 
 - BibTeX:
 
 ```
 @software{lhotte_pard_2022,
     author = {Lhotte, Romain and Taupin, Jean-Luc},
     doi = {10.5281/zenodo.7013169},
     month = {8},
     title = {{Physicochemical Amino acid Replacement Distances (PARD) package}},
-    version = {0.6.0.0},
+    version = {0.7.0.0},
     year = {2022}
 }
 ```
 
 
 ### References
 - [1] Grantham, R., 1974. Amino acid difference formula to help explain protein evolution. science, 185(4154),
```

### Comparing `pard-0.6.0.0/setup.py` & `pard-0.7.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['pard']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pard',
-    'version': '0.6.0.0',
+    'version': '0.7.0.0',
     'description': 'Physicochemical Amino acid Replacement Distances',
-    'long_description': '## PARD (Physicochemical Amino acid Replacement Distances)\n[![DOI](https://zenodo.org/badge/526882024.svg)](https://zenodo.org/badge/latestdoi/526882024)\n![Coverage](\nreadme_resources/coverage.svg\n)\n[![Downloads](https://pepy.tech/badge/pard)](https://pepy.tech/project/pard)\n\n### Overview\nAmino acid replacements (also referred to as substitutions) are changes from one amino acid to a different one in a\nprotein - and there are different ways to assess the difference between the two amino acids that come into play in an\namino acid replacement.\n\nOne can look at one or several properties\' discrepancy between two amino acids.\nTo list only a few: polarity\n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862) [[3]](https://www.nature.com/articles/215355a0) \n[[4]](https://link.springer.com/article/10.1007/BF01732340) \n[[8]](https://onlinelibrary.wiley.com/doi/10.1111/j.1399-3011.1987.tb02254.x),\nmolecular volume / relative sizes of amino-acid side chains \n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862) [[3]](https://www.nature.com/articles/215355a0)\n[[4]](https://link.springer.com/article/10.1007/BF01732340), \nmean number of lone pair electrons on the side-chain\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123),\nmaximum moment of inertia for rotation at the α―β bond\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\nor at the β―γ bond [[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\nor at the γ―δ bond [[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123), \npresence of a pyrrolidine ring (proline (P))\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123), \nexperimental protein activity and stability after exchanging one amino acid into another\n[[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/), Chou-Fasman alpha helical, beta strand and reverse turn\npropensity parameters [[8]](https://onlinelibrary.wiley.com/doi/10.1111/j.1399-3011.1987.tb02254.x), etc.\n\n`pard` is a package designed to make those **P**hysicochemical **A**mino acid **R**eplacement **D**istances calculations\nstraightforward with Python.\n\nOne typical use is to establish a \'distance\' between a wild-type protein and its mutated version. Sometimes, rather\nthan a distance, a similarity is outputted (e.g. with `the Conformational similarity weight matrix`\n[[7]](https://www.sciencedirect.com/science/article/abs/pii/002228369290261H) or `EMPAR` \n[[8]](https://onlinelibrary.wiley.com/doi/10.1111/j.1399-3011.1987.tb02254.x)). The higher the distance, the more\ndifferent the two amino acids are. The higher the similarity, the more similar the two amino acids are. Whenever\na distance is not outputted but rather a similarity, a warning (that the user can turn off) will be raised.\n\n\n### Getting started\n#### Install from PyPI (recommended)\nTo use `pard`, run `pip install pard` in your terminal.\n\n#### Usage\n```py\n## Imports\nfrom pard.grantham import grantham\nfrom pard.sneath import sneath\nfrom pard.experimental_exchangeability import experimental_exchangeability\nfrom pard.koshi_goldstein import koshi_goldstein, MatrixType\n\n\n## Basic examples\namino_acid_1: str = "W"  # Tryptophan\namino_acid_2: str = "L"  # Leucine\ndistance_grantham: int = grantham(amino_acid_1, amino_acid_2)\nprint(distance_grantham)\n\ndistance_sneath: int   = sneath(amino_acid_1, amino_acid_2)\nprint(distance_sneath)\n\ndistance_ee: float     = experimental_exchangeability(\n    amino_acid_1, \n    amino_acid_2, \n    False, \n    warning=True\n)\nprint(distance_ee)\n\n\n## More subtle examples\n# Koshi-Goldstein has several scores and can estimate the likelihood of InDels\ndistance_koshi_goldstein_all: float = koshi_goldstein(\n    "-",\n    "A",\n    MatrixType.ALL_RESIDUES,\n    False,\n    warning=True\n)\nprint(distance_koshi_goldstein_all)\n```\nor equivalently\n```py\n## Imports\nimport pard\n\n\n## Basic examples\namino_acid_1: str = "W"  # Tryptophan\namino_acid_2: str = "L"  # Leucine\ndistance_grantham: int = pard.grantham.grantham(amino_acid_1, amino_acid_2)\nprint(distance_grantham)\n\ndistance_sneath: int   = pard.sneath.sneath(amino_acid_1, amino_acid_2)\nprint(distance_sneath)\n\ndistance_ee: float     = pard.experimental_exchangeability.experimental_exchangeability(\n    amino_acid_1,\n    amino_acid_2,\n    False,\n    warning=True\n)\nprint(distance_ee)\n\n\n## More subtle examples\n# Koshi-Goldstein has several scores and can estimate the likelihood of InDels\ndistance_koshi_goldstein_all: float = pard.koshi_goldstein.koshi_goldstein(\n    "-",\n    "A",\n    pard.koshi_goldstein.MatrixType.ALL_RESIDUES,\n    False,\n    warning=True\n)\nprint(distance_koshi_goldstein_all)\n```\nwill output:\n```\n>>> 61\n>>> 30\n>>> 177\n>>> 1.6\n```\nwhich are the correct values \n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862)\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\n[[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/)\n[[6]](https://academic.oup.com/peds/article-abstract/8/7/641/1465446)\n.\n\n#### Exit codes:\n```\n- 1: Argument amino_acid_1 or amino_acid_2 is neither of length 1 nor length 3. See error message.\n```\n\n### About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/6.2.x/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n#### Unit tests details\nCoverage\n```\nName                                         Stmts   Miss  Cover\n----------------------------------------------------------------\npard\\__init__.py                                 3      0   100%\npard\\_handling_3_letter_code_decorator.py       18      2    89%\npard\\_raw_python_dictionaries.py                71      0   100%\npard\\empar.py                                    8      0   100%\npard\\epstein.py                                  7      0   100%\npard\\experimental_exchangeability.py            10      0   100%\npard\\grantham.py                                 5      0   100%\npard\\kolaskar.py                                 8      0   100%\npard\\koshi_goldstein.py                         55      2    96%\npard\\miyata.py                                   5      0   100%\npard\\sneath.py                                   5      0   100%\ntests\\__init__.py                                0      0   100%\ntests\\test_empar.py                             26      0   100%\ntests\\test_epstein.py                           46      0   100%\ntests\\test_experimental_exchangeability.py      30      0   100%\ntests\\test_grantham.py                          25      0   100%\ntests\\test_kolaskar.py                          26      0   100%\ntests\\test_koshi_goldstein.py                  108      0   100%\ntests\\test_miyata.py                            25      0   100%\ntests\\test_pard.py                               3      0   100%\ntests\\test_raw_python_dictionaries.py           24      0   100%\ntests\\test_sneath.py                            21      0   100%\nunit_tests_simple.py                             5      0   100%\n----------------------------------------------------------------\nTOTAL                                          534      4    99%\n```\n\n#### pytest\n```\nplatform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 16 items\n\ntests\\test_empar.py .                                     [  6%] \ntests\\test_epstein.py .                                   [ 12%] \ntests\\test_experimental_exchangeability.py .              [ 18%] \ntests\\test_grantham.py .                                  [ 25%]\ntests\\test_kolaskar.py .                                  [ 31%] \ntests\\test_koshi_goldstein.py .......                     [ 75%]\ntests\\test_miyata.py .                                    [ 81%] \ntests\\test_pard.py .                                      [ 87%] \ntests\\test_raw_python_dictionaries.py .                   [ 93%] \ntests\\test_sneath.py .                                    [100%] \n\n====================== 16 passed in 0.11s ====================== \n```\n\n#### mypy detail\n```\n================================== mypy ==================================\nSuccess: no issues found in 24 source files\n```\n\n### Useful links:\n- [Corresponding GitHub repository](https://github.com/MICS-Lab/pard)\n- [Corresponding PyPI page](https://pypi.org/project/pard/)\n\n\n### Citation\nIf you use this software, please cite it as below.\n\n- APA:\n\n`\nLhotte, R. & Taupin, J. (2022).\nPhysicochemical Amino acid Replacement Distances (PARD) package (Version 0.6.0.0) [Computer software].\nhttps://doi.org/10.5281/zenodo.7013169\n`\n\n- BibTeX:\n\n```\n@software{lhotte_pard_2022,\n    author = {Lhotte, Romain and Taupin, Jean-Luc},\n    doi = {10.5281/zenodo.7013169},\n    month = {8},\n    title = {{Physicochemical Amino acid Replacement Distances (PARD) package}},\n    version = {0.6.0.0},\n    year = {2022}\n}\n```\n\n\n### References\n- [1] Grantham, R., 1974. Amino acid difference formula to help explain protein evolution. science, 185(4154), \npp.862-864.\n- [2] Sneath, P.H.A., 1966. Relations between chemical structure and biological activity in peptides. Journal of\ntheoretical biology, 12(2), pp.157-195.\n- [3] Epstein, C.J., 1967. Non-randomness of ammo-acid changes in the evolution of homologous proteins. Nature,\n215(5099), pp.355-359.\n- [4] Miyata, T., Miyazawa, S. and Yasunaga, T., 1979. Two types of amino acid substitutions in protein evolution. \nJournal of molecular evolution, 12(3), pp.219-236.\n- [5] Yampolsky, L.Y. and Stoltzfus, A., 2005. The exchangeability of amino acids in proteins. Genetics, 170(4), \npp.1459-1472.\n- [6] Koshi, J.M. and Goldstein, R.A., 1995. Context-dependent optimal substitution matrices. Protein Engineering,\nDesign and Selection, 8(7), pp.641-645.\n',
+    'long_description': '## PARD (Physicochemical Amino acid Replacement Distances)\n[![DOI](https://zenodo.org/badge/526882024.svg)](https://zenodo.org/badge/latestdoi/526882024)\n![Coverage](\nreadme_resources/coverage.svg\n)\n[![Downloads](https://pepy.tech/badge/pard)](https://pepy.tech/project/pard)\n\n### Overview\nAmino acid replacements (also referred to as substitutions) are changes from one amino acid to a different one in a\nprotein - and there are different ways to assess the difference between the two amino acids that come into play in an\namino acid replacement.\n\nOne can look at one or several properties\' discrepancy between two amino acids.\nTo list only a few: polarity\n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862) [[3]](https://www.nature.com/articles/215355a0) \n[[4]](https://link.springer.com/article/10.1007/BF01732340) \n[[8]](https://onlinelibrary.wiley.com/doi/10.1111/j.1399-3011.1987.tb02254.x),\nmolecular volume / relative sizes of amino-acid side chains \n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862) [[3]](https://www.nature.com/articles/215355a0)\n[[4]](https://link.springer.com/article/10.1007/BF01732340), \nmean number of lone pair electrons on the side-chain\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123),\nmaximum moment of inertia for rotation at the α―β bond\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\nor at the β―γ bond [[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\nor at the γ―δ bond [[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123), \npresence of a pyrrolidine ring (proline (P))\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123), \nexperimental protein activity and stability after exchanging one amino acid into another\n[[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/), Chou-Fasman alpha helical, beta strand and reverse turn\npropensity parameters [[8]](https://onlinelibrary.wiley.com/doi/10.1111/j.1399-3011.1987.tb02254.x), etc.\n\n`pard` is a package designed to make those **P**hysicochemical **A**mino acid **R**eplacement **D**istances calculations\nstraightforward with Python.\n\nOne typical use is to establish a \'distance\' between a wild-type protein and its mutated version. Sometimes, rather\nthan a distance, a similarity is outputted (e.g. with `the Conformational similarity weight matrix`\n[[7]](https://www.sciencedirect.com/science/article/abs/pii/002228369290261H) or `EMPAR` \n[[8]](https://onlinelibrary.wiley.com/doi/10.1111/j.1399-3011.1987.tb02254.x)). The higher the distance, the more\ndifferent the two amino acids are. The higher the similarity, the more similar the two amino acids are. Whenever\na distance is not outputted but rather a similarity, a warning (that the user can turn off) will be raised.\n\n\n### Getting started\n#### Install from PyPI (recommended)\nTo use `pard`, run `pip install pard` in your terminal.\n\n#### Usage\n```py\n## Imports\nfrom pard.grantham import grantham\nfrom pard.sneath import sneath\nfrom pard.experimental_exchangeability import experimental_exchangeability\nfrom pard.koshi_goldstein import koshi_goldstein, MatrixType\n\n\n## Basic examples\namino_acid_1: str = "W"  # Tryptophan\namino_acid_2: str = "L"  # Leucine\ndistance_grantham: int = grantham(amino_acid_1, amino_acid_2)\nprint(distance_grantham)\n\ndistance_sneath: int   = sneath(amino_acid_1, amino_acid_2)\nprint(distance_sneath)\n\ndistance_ee: float     = experimental_exchangeability(\n    amino_acid_1, \n    amino_acid_2, \n    False, \n    warning=True\n)\nprint(distance_ee)\n\n\n## More subtle examples\n# Koshi-Goldstein has several scores and can estimate the likelihood of InDels\ndistance_koshi_goldstein_all: float = koshi_goldstein(\n    "-",\n    "A",\n    MatrixType.ALL_RESIDUES,\n    False,\n    warning=True\n)\nprint(distance_koshi_goldstein_all)\n```\nor equivalently\n```py\n## Imports\nimport pard\n\n\n## Basic examples\namino_acid_1: str = "W"  # Tryptophan\namino_acid_2: str = "L"  # Leucine\ndistance_grantham: int = pard.grantham.grantham(amino_acid_1, amino_acid_2)\nprint(distance_grantham)\n\ndistance_sneath: int   = pard.sneath.sneath(amino_acid_1, amino_acid_2)\nprint(distance_sneath)\n\ndistance_ee: float     = pard.experimental_exchangeability.experimental_exchangeability(\n    amino_acid_1,\n    amino_acid_2,\n    False,\n    warning=True\n)\nprint(distance_ee)\n\n\n## More subtle examples\n# Koshi-Goldstein has several scores and can estimate the likelihood of InDels\ndistance_koshi_goldstein_all: float = pard.koshi_goldstein.koshi_goldstein(\n    "-",\n    "A",\n    pard.koshi_goldstein.MatrixType.ALL_RESIDUES,\n    False,\n    warning=True\n)\nprint(distance_koshi_goldstein_all)\n```\nwill output:\n```\n>>> 61\n>>> 30\n>>> 177\n>>> 1.6\n```\nwhich are the correct values \n[[1]](https://www.science.org/doi/10.1126/science.185.4154.862)\n[[2]](https://www.sciencedirect.com/science/article/abs/pii/0022519366901123)\n[[5]](https://pubmed.ncbi.nlm.nih.gov/15944362/)\n[[6]](https://academic.oup.com/peds/article-abstract/8/7/641/1465446)\n.\n\n#### Exit codes:\n```\n- 1: Argument amino_acid_1 or amino_acid_2 is neither of length 1 nor length 3. See error message.\n```\n\n### About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/6.2.x/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n#### Unit tests details\nCoverage\n```\nName                                         Stmts   Miss  Cover\n----------------------------------------------------------------\npard\\__init__.py                                 3      0   100%\npard\\_handling_3_letter_code_decorator.py       18      2    89%\npard\\_raw_python_dictionaries.py                71      0   100%\npard\\empar.py                                    8      0   100%\npard\\epstein.py                                  7      0   100%\npard\\experimental_exchangeability.py            10      0   100%\npard\\grantham.py                                 5      0   100%\npard\\kolaskar.py                                 8      0   100%\npard\\koshi_goldstein.py                         55      2    96%\npard\\miyata.py                                   5      0   100%\npard\\sneath.py                                   5      0   100%\ntests\\__init__.py                                0      0   100%\ntests\\test_empar.py                             26      0   100%\ntests\\test_epstein.py                           46      0   100%\ntests\\test_experimental_exchangeability.py      30      0   100%\ntests\\test_grantham.py                          25      0   100%\ntests\\test_kolaskar.py                          26      0   100%\ntests\\test_koshi_goldstein.py                  108      0   100%\ntests\\test_miyata.py                            25      0   100%\ntests\\test_pard.py                               3      0   100%\ntests\\test_raw_python_dictionaries.py           24      0   100%\ntests\\test_sneath.py                            21      0   100%\nunit_tests_simple.py                             5      0   100%\n----------------------------------------------------------------\nTOTAL                                          534      4    99%\n```\n\n#### pytest\n```\nplatform win32 -- Python 3.11.1, pytest-7.2.0, pluggy-1.0.0\nplugins: anyio-3.6.2, mypy-0.10.3\ncollected 16 items\n\ntests\\test_empar.py .                                     [  6%] \ntests\\test_epstein.py .                                   [ 12%] \ntests\\test_experimental_exchangeability.py .              [ 18%] \ntests\\test_grantham.py .                                  [ 25%]\ntests\\test_kolaskar.py .                                  [ 31%] \ntests\\test_koshi_goldstein.py .......                     [ 75%]\ntests\\test_miyata.py .                                    [ 81%] \ntests\\test_pard.py .                                      [ 87%] \ntests\\test_raw_python_dictionaries.py .                   [ 93%] \ntests\\test_sneath.py .                                    [100%] \n\n====================== 16 passed in 0.11s ====================== \n```\n\n#### mypy detail\n```\n================================== mypy ==================================\nSuccess: no issues found in 24 source files\n```\n\n### Useful links:\n- [Corresponding GitHub repository](https://github.com/MICS-Lab/pard)\n- [Corresponding PyPI page](https://pypi.org/project/pard/)\n\n\n### Citation\nIf you use this software, please cite it as below.\n\n- APA:\n\n`\nLhotte, R. & Taupin, J. (2022).\nPhysicochemical Amino acid Replacement Distances (PARD) package (Version 0.7.0.0) [Computer software].\nhttps://doi.org/10.5281/zenodo.7013169\n`\n\n- BibTeX:\n\n```\n@software{lhotte_pard_2022,\n    author = {Lhotte, Romain and Taupin, Jean-Luc},\n    doi = {10.5281/zenodo.7013169},\n    month = {8},\n    title = {{Physicochemical Amino acid Replacement Distances (PARD) package}},\n    version = {0.7.0.0},\n    year = {2022}\n}\n```\n\n\n### References\n- [1] Grantham, R., 1974. Amino acid difference formula to help explain protein evolution. science, 185(4154), \npp.862-864.\n- [2] Sneath, P.H.A., 1966. Relations between chemical structure and biological activity in peptides. Journal of\ntheoretical biology, 12(2), pp.157-195.\n- [3] Epstein, C.J., 1967. Non-randomness of ammo-acid changes in the evolution of homologous proteins. Nature,\n215(5099), pp.355-359.\n- [4] Miyata, T., Miyazawa, S. and Yasunaga, T., 1979. Two types of amino acid substitutions in protein evolution. \nJournal of molecular evolution, 12(3), pp.219-236.\n- [5] Yampolsky, L.Y. and Stoltzfus, A., 2005. The exchangeability of amino acids in proteins. Genetics, 170(4), \npp.1459-1472.\n- [6] Koshi, J.M. and Goldstein, R.A., 1995. Context-dependent optimal substitution matrices. Protein Engineering,\nDesign and Selection, 8(7), pp.641-645.\n',
     'author': 'JasonMendoza2008',
     'author_email': 'lhotteromain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pard-0.6.0.0/PKG-INFO` & `pard-0.7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pard
-Version: 0.6.0.0
+Version: 0.7.0.0
 Summary: Physicochemical Amino acid Replacement Distances
 Author: JasonMendoza2008
 Author-email: lhotteromain@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -223,27 +223,27 @@
 ### Citation
 If you use this software, please cite it as below.
 
 - APA:
 
 `
 Lhotte, R. & Taupin, J. (2022).
-Physicochemical Amino acid Replacement Distances (PARD) package (Version 0.6.0.0) [Computer software].
+Physicochemical Amino acid Replacement Distances (PARD) package (Version 0.7.0.0) [Computer software].
 https://doi.org/10.5281/zenodo.7013169
 `
 
 - BibTeX:
 
 ```
 @software{lhotte_pard_2022,
     author = {Lhotte, Romain and Taupin, Jean-Luc},
     doi = {10.5281/zenodo.7013169},
     month = {8},
     title = {{Physicochemical Amino acid Replacement Distances (PARD) package}},
-    version = {0.6.0.0},
+    version = {0.7.0.0},
     year = {2022}
 }
 ```
 
 
 ### References
 - [1] Grantham, R., 1974. Amino acid difference formula to help explain protein evolution. science, 185(4154),
```

