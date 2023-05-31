# Comparing `tmp/ail_typo_squatting-2.4.0.tar.gz` & `tmp/ail_typo_squatting-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ail_typo_squatting-2.4.0.tar", max compression
+gzip compressed data, was "ail_typo_squatting-2.4.1.tar", max compression
```

## Comparing `ail_typo_squatting-2.4.0.tar` & `ail_typo_squatting-2.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1480 2022-10-10 06:31:40.879541 ail_typo_squatting-2.4.0/LICENSE
--rw-r--r--   0        0        0    15567 2023-02-13 09:09:27.990105 ail_typo_squatting-2.4.0/README.md
--rw-r--r--   0        0        0     1349 2023-02-13 09:13:36.349977 ail_typo_squatting-2.4.0/ail_typo_squatting/__init__.py
--rw-r--r--   0        0        0    74127 2023-02-13 09:00:45.438395 ail_typo_squatting-2.4.0/ail_typo_squatting/typo.py
--rw-r--r--   0        0        0   130949 2022-10-10 06:31:40.879541 ail_typo_squatting-2.4.0/etc/common-misspellings.json
--rw-r--r--   0        0        0    11077 2022-12-01 07:44:18.868804 ail_typo_squatting-2.4.0/etc/dynamic-dns.json
--rw-r--r--   0        0        0     6028 2022-10-10 06:31:40.879541 ail_typo_squatting-2.4.0/etc/homophones.txt
--rw-r--r--   0        0        0     9889 2022-10-27 12:02:28.815614 ail_typo_squatting-2.4.0/etc/tlds-alpha-by-domain.txt
--rw-r--r--   0        0        0      783 2023-02-13 09:18:59.573815 ail_typo_squatting-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    16784 1970-01-01 00:00:00.000000 ail_typo_squatting-2.4.0/setup.py
--rw-r--r--   0        0        0    16714 1970-01-01 00:00:00.000000 ail_typo_squatting-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1480 2022-10-10 06:31:40.879541 ail_typo_squatting-2.4.1/LICENSE
+-rw-r--r--   0        0        0    14736 2023-05-15 09:40:02.694386 ail_typo_squatting-2.4.1/README.md
+-rw-r--r--   0        0        0     1349 2023-02-13 09:13:36.349977 ail_typo_squatting-2.4.1/ail_typo_squatting/__init__.py
+-rw-r--r--   0        0        0    53442 2023-05-16 13:15:00.510028 ail_typo_squatting-2.4.1/ail_typo_squatting/typo.py
+-rw-r--r--   0        0        0   130949 2022-10-10 06:31:40.879541 ail_typo_squatting-2.4.1/etc/common-misspellings.json
+-rw-r--r--   0        0        0    11077 2023-05-16 08:48:07.685635 ail_typo_squatting-2.4.1/etc/dynamic-dns.json
+-rw-r--r--   0        0        0     6028 2022-10-10 06:31:40.879541 ail_typo_squatting-2.4.1/etc/homophones.txt
+-rw-r--r--   0        0        0     9889 2022-10-27 12:02:28.815614 ail_typo_squatting-2.4.1/etc/tlds-alpha-by-domain.txt
+-rw-r--r--   0        0        0      784 2023-05-31 06:36:40.363342 ail_typo_squatting-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0    15951 1970-01-01 00:00:00.000000 ail_typo_squatting-2.4.1/setup.py
+-rw-r--r--   0        0        0    15885 1970-01-01 00:00:00.000000 ail_typo_squatting-2.4.1/PKG-INFO
```

### Comparing `ail_typo_squatting-2.4.0/LICENSE` & `ail_typo_squatting-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ail_typo_squatting-2.4.0/README.md` & `ail_typo_squatting-2.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: ail-typo-squatting
+Version: 2.4.1
+Summary: Generate list of domain name using Domain name permutation engine to feed AIL
+Home-page: https://github.com/typosquatter/ail-typo-squatting
+License: BSD-2-Clause
+Keywords: typo-squatting,typosquatting
+Author: David Cruciani
+Author-email: david.cruciani@securitymadein.lu
+Maintainer: Alexandre Dulaunoy
+Maintainer-email: a@foo.be
+Requires-Python: >=3.6,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dnspython (>=2.2.0,<3.0.0)
+Requires-Dist: inflect (>=5.3.0,<6.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: tldextract (>=3.1.2,<4.0.0)
+Project-URL: Repository, https://github.com/typosquatter/ail-typo-squatting
+Description-Content-Type: text/markdown
+
 # ail-typo-squatting
 
 ail-typo-squatting is a Python library to generate list of potential typo squatting domains with domain name permutation engine to feed AIL and other systems. 
 
 The tool can be used as a stand-alone tool or to feed other systems.
 
 # Requirements
@@ -33,65 +61,65 @@
 $ pip3 install ail-typo-squatting
 ```
 
 # Usage
 
 ```bash
 dacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py --help  
-usage: typo.py [-h] [-v] [-dn DOMAINNAME [DOMAINNAME ...]] [-fdn FILEDOMAINNAME] [-o OUTPUT] [-fo FORMATOUTPUT] [-dnsr] [-l LIMIT] [-var] [-ko] [-a] [-om] [-repe] [-tra] [-repl] [-drepl] [-cho] [-ki] [-add] [-md] [-sd]
-               [-vs] [-ada] [-bs] [-hg] [-ahg] [-cm] [-hp] [-wt] [-at] [-sub] [-sp] [-cdd]
+usage: typo.py [-h] [-v] [-dn DOMAINNAME [DOMAINNAME ...]] [-fdn FILEDOMAINNAME] [-o OUTPUT] [-fo FORMATOUTPUT] [-dnsr] [-dnsl] [-l LIMIT] [-var] [-ko] [-a] [-om] [-repe] [-repl] [-drepl] [-cho] [-add]
+               [-md] [-sd] [-vs] [-ada] [-hg] [-ahg] [-cm] [-hp] [-wt] [-wsld] [-at] [-sub] [-sp] [-cdd] [-addns] [-ns]
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -v                    verbose, more display
   -dn DOMAINNAME [DOMAINNAME ...], --domainName DOMAINNAME [DOMAINNAME ...]
                         list of domain name
   -fdn FILEDOMAINNAME, --filedomainName FILEDOMAINNAME
                         file containing list of domain name
   -o OUTPUT, --output OUTPUT
                         path to ouput location
   -fo FORMATOUTPUT, --formatoutput FORMATOUTPUT
                         format for the output file, yara - regex - yaml - text. Default: text
   -dnsr, --dnsresolving
                         resolve all variation of domain name to see if it's up or not
+  -dnsl, --dnslimited   resolve all variation of domain name but keep only up domain in final result json
   -l LIMIT, --limit LIMIT
                         limit of variations for a domain name
   -var, --givevariations
                         give the algo that generate variations
   -ko, --keeporiginal   Keep in the result list the original domain name
   -a, --all             Use all algo
   -om, --omission       Leave out a letter of the domain name
   -repe, --repetition   Character Repeat
-  -tra, --transposition
-                        Swappe the order of adjacent letters in the domain name
-  -repl, --replacement  Adjacent character replacement to the immediate left and right on the keyboard
+  -repl, --replacement  Character replacement
   -drepl, --doublereplacement
                         Double Character Replacement
   -cho, --changeorder   Change the order of letters in word
-  -ki, --keyboardinsertion
-                        Adjacent character insertion of letters to the immediate left and right on the keyboard of each letter
   -add, --addition      Add a character in the domain name
   -md, --missingdot     Delete a dot from the domain name
   -sd, --stripdash      Delete of a dash from the domain name
   -vs, --vowelswap      Swap vowels within the domain name
   -ada, --adddash       Add a dash between the first and last character in a string
-  -bs, --bitsquatting   The character is substituted with the set of valid characters that can be made after a single bit flip
   -hg, --homoglyph      One or more characters that look similar to another character but are different are called homogylphs
   -ahg, --all_homoglyph
                         generate all possible homoglyph permutations. Ex: circl.lu, e1rc1.lu
   -cm, --commonmisspelling
                         Change a word by is misspellings
   -hp, --homophones     Change word by an other who sound the same when spoken
   -wt, --wrongtld       Change the original top level domain to another
+  -wsld, --wrongsld     Change the original second level domain to another
   -at, --addtld         Adding a tld before the original tld
   -sub, --subdomain     Insert a dot at varying positions to create subdomain
   -sp, --singularpluralize
                         Create by making a singular domain plural and vice versa
   -cdd, --changedotdash
                         Change dot to dash
+  -addns, --adddynamicdns
+                        Add dynamic dns at the end of the domain
+  -ns, --numeralswap    Change a numbers to words and vice versa. Ex: circlone.lu, circl1.lu
 ```
 
 # Usage example
 
 1. Creation of variations for `ail-project.org` and `circl.lu`, using all algorithm.
 
 ```bash
@@ -288,33 +316,31 @@
 
 | Algo               | Description                                                                                                                                                                                                                               |
 |:------------------ |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | AddDash            | These typos are created by adding a dash between the first and last character in a string.                                                                                                                                                |
 | Addition           | These typos are created by add a characters in the domain name.                                                                                                                                                                           |
 | AddDynamicDns      | These typos are created by adding a dynamic dns at the end of the original domain.                                                                                                                                                        |
 | AddTld             | These typos are created by adding a tld before the right tld. Example: google.com becomes google.com.it                                                                                                                                   |
-| Bitsquatting       | These typos are created by substituting a character with the set of valid characters that can be made after a single bit flip. For example, facebook.com becomes bacebook.com, dacebook.com, faaebook.com,fabebook.com,facabook.com, etc. |
 | ChangeDotDash      | These typos are created by changing a dot to a dash.                                                                                                                                                                                      |
 | ChangeOrder        | These typos are created by changing the order of letters in the each part of the domain.                                                                                                                                                  |
 | CommonMisspelling  | These typos are created by changing a word by is misspelling. Over 8000 common misspellings from Wikipedia. For example, www.youtube.com becomes www.youtub.com and www.abseil.com becomes www.absail.com.                                |
-| Double Replacement | These typos are created by replacing identical, consecutive letters of the domain name with letters to the immediate left and right on the keyboard.                                                                                      |
+| Double Replacement | These typos are created by replacing identical, consecutive letters of the domain name.                                                                                                                                                   |
 | Homoglyph          | These typos are created by replacing characters to another character that look similar but are different.  An example is that the lower case l looks similar to the numeral one, e.g. l vs 1. For example, google.com becomes goog1e.com. |
 | Homophones         | These typos are created by changing word by an other who sound the same when spoken. Over 450 sets of words that sound the same when spoken. For example, www.base.com becomes www.bass.com.                                              |
-| KeyboardInsertion  | These typos are created by inserting letters to the immediate left and right on the keyboard of each letter.                                                                                                                              |
 | MissingDot         | These typos are created by deleting a dot from the domain name.                                                                                                                                                                           |
 | NumeralSwap        | These typos are created by changing a number to words and vice versa. For example, circlone.lu becomes circl1.lu.                                                                                                                         |
 | Omission           | These typos are created by leaving out a letter of the domain name, one letter at a time.                                                                                                                                                 |
 | Repetition         | These typos are created by repeating a letter of the domain name.                                                                                                                                                                         |
-| Replacement        | These typos are created by replacing each letter of the domain name with letters to the immediate left and right on the keyboard. (QWERTY, AZERTY, QWERTZ, DVORAK)                                                                        |
+| Replacement        | These typos are created by replacing each letter of the domain name.                                                                                                                                                                      |
 | StripDash          | These typos are created by deleting a dash from the domain name.                                                                                                                                                                          |
 | SingularPluralize  | These typos are created by making a singular domain plural and vice versa.                                                                                                                                                                |
 | Subdomain          | These typos are created by placing a dot in the domain name in order to create subdomain. Example: google.com becomes goo.gle.com                                                                                                         |
-| Transposition      | These typos are created by swapping the order of adjacent letters in the domain name.                                                                                                                                                     |
 | VowelSwap          | These typos are created by swapping vowels within the domain name except for the first letter. For example, www.google.com becomes www.gaagle.com.                                                                                        |
 | WrongTld           | These typos are created by changing the original top level domain to another. For example, www.trademe.co.nz becomes www.trademe.co.mz and www.google.com becomes www.google.org Uses the 19 most common top level domains.               |
 | WrongSld           | These typos are created by changing the original second level domain to another. For example, www.trademe.co.uk becomes www.trademe.ac.uk and www.google.com will still be www.google.com .                                               |
 
 # Acknowledgment
 
 ![](./img/cef.png)
 
 The project has been co-funded by CEF-TC-2020-2 - 2020-EU-IA-0260 - JTAN - Joint Threat Analysis Network.
+
```

### Comparing `ail_typo_squatting-2.4.0/ail_typo_squatting/__init__.py` & `ail_typo_squatting-2.4.1/ail_typo_squatting/__init__.py`

 * *Files identical despite different names*

### Comparing `ail_typo_squatting-2.4.0/etc/common-misspellings.json` & `ail_typo_squatting-2.4.1/etc/common-misspellings.json`

 * *Files identical despite different names*

### Comparing `ail_typo_squatting-2.4.0/etc/dynamic-dns.json` & `ail_typo_squatting-2.4.1/etc/dynamic-dns.json`

 * *Files identical despite different names*

### Comparing `ail_typo_squatting-2.4.0/etc/homophones.txt` & `ail_typo_squatting-2.4.1/etc/homophones.txt`

 * *Files identical despite different names*

### Comparing `ail_typo_squatting-2.4.0/etc/tlds-alpha-by-domain.txt` & `ail_typo_squatting-2.4.1/etc/tlds-alpha-by-domain.txt`

 * *Files identical despite different names*

### Comparing `ail_typo_squatting-2.4.0/pyproject.toml` & `ail_typo_squatting-2.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "ail-typo-squatting"
-version = "2.4.0"
+version = "2.4.1"
 description = "Generate list of domain name using Domain name permutation engine to feed AIL"
 authors = [
 	"David Cruciani <david.cruciani@securitymadein.lu>"
 ]
 maintainers = [
 	"Alexandre Dulaunoy <a@foo.be>",
 	"Aurelien Thirion (terrtia) <aurelien.thirion@circl.lu>"
 ]
 license = "BSD-2-Clause"
-repository = "https://github.com/ail-project/ail-typo-squatting"
+repository = "https://github.com/typosquatter/ail-typo-squatting"
 
 readme = "README.md"
 
 keywords = [
 	"typo-squatting",
 	"typosquatting"
 ]
```

### Comparing `ail_typo_squatting-2.4.0/setup.py` & `ail_typo_squatting-2.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,22 @@
  'inflect>=5.3.0,<6.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.27.1,<3.0.0',
  'tldextract>=3.1.2,<4.0.0']
 
 setup_kwargs = {
     'name': 'ail-typo-squatting',
-    'version': '2.4.0',
+    'version': '2.4.1',
     'description': 'Generate list of domain name using Domain name permutation engine to feed AIL',
-    'long_description': '# ail-typo-squatting\n\nail-typo-squatting is a Python library to generate list of potential typo squatting domains with domain name permutation engine to feed AIL and other systems. \n\nThe tool can be used as a stand-alone tool or to feed other systems.\n\n# Requirements\n\n- Python 3.6+\n- [inflect](https://github.com/jaraco/inflect) library\n- [pyyaml](https://pyyaml.org/wiki/PyYAMLDocumentation)\n\n## Optional\n\n- [dnspython](https://github.com/rthalley/dnspython)\n\n# Installation\n\n## Source install\n\nail-typo-squatting can be install with poetry. If you don\'t have poetry installed, you can do the following `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python`.\n\n```bash\n$ poetry install\n$ poetry shell\n$ cd ail-typo-squatting\n$ python typo.py -h\n```\n\n## pip installation\n\n```bash\n$ pip3 install ail-typo-squatting\n```\n\n# Usage\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py --help  \nusage: typo.py [-h] [-v] [-dn DOMAINNAME [DOMAINNAME ...]] [-fdn FILEDOMAINNAME] [-o OUTPUT] [-fo FORMATOUTPUT] [-dnsr] [-l LIMIT] [-var] [-ko] [-a] [-om] [-repe] [-tra] [-repl] [-drepl] [-cho] [-ki] [-add] [-md] [-sd]\n               [-vs] [-ada] [-bs] [-hg] [-ahg] [-cm] [-hp] [-wt] [-at] [-sub] [-sp] [-cdd]\n\noptions:\n  -h, --help            show this help message and exit\n  -v                    verbose, more display\n  -dn DOMAINNAME [DOMAINNAME ...], --domainName DOMAINNAME [DOMAINNAME ...]\n                        list of domain name\n  -fdn FILEDOMAINNAME, --filedomainName FILEDOMAINNAME\n                        file containing list of domain name\n  -o OUTPUT, --output OUTPUT\n                        path to ouput location\n  -fo FORMATOUTPUT, --formatoutput FORMATOUTPUT\n                        format for the output file, yara - regex - yaml - text. Default: text\n  -dnsr, --dnsresolving\n                        resolve all variation of domain name to see if it\'s up or not\n  -l LIMIT, --limit LIMIT\n                        limit of variations for a domain name\n  -var, --givevariations\n                        give the algo that generate variations\n  -ko, --keeporiginal   Keep in the result list the original domain name\n  -a, --all             Use all algo\n  -om, --omission       Leave out a letter of the domain name\n  -repe, --repetition   Character Repeat\n  -tra, --transposition\n                        Swappe the order of adjacent letters in the domain name\n  -repl, --replacement  Adjacent character replacement to the immediate left and right on the keyboard\n  -drepl, --doublereplacement\n                        Double Character Replacement\n  -cho, --changeorder   Change the order of letters in word\n  -ki, --keyboardinsertion\n                        Adjacent character insertion of letters to the immediate left and right on the keyboard of each letter\n  -add, --addition      Add a character in the domain name\n  -md, --missingdot     Delete a dot from the domain name\n  -sd, --stripdash      Delete of a dash from the domain name\n  -vs, --vowelswap      Swap vowels within the domain name\n  -ada, --adddash       Add a dash between the first and last character in a string\n  -bs, --bitsquatting   The character is substituted with the set of valid characters that can be made after a single bit flip\n  -hg, --homoglyph      One or more characters that look similar to another character but are different are called homogylphs\n  -ahg, --all_homoglyph\n                        generate all possible homoglyph permutations. Ex: circl.lu, e1rc1.lu\n  -cm, --commonmisspelling\n                        Change a word by is misspellings\n  -hp, --homophones     Change word by an other who sound the same when spoken\n  -wt, --wrongtld       Change the original top level domain to another\n  -at, --addtld         Adding a tld before the original tld\n  -sub, --subdomain     Insert a dot at varying positions to create subdomain\n  -sp, --singularpluralize\n                        Create by making a singular domain plural and vice versa\n  -cdd, --changedotdash\n                        Change dot to dash\n```\n\n# Usage example\n\n1. Creation of variations for `ail-project.org` and `circl.lu`, using all algorithm.\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py -dn ail-project.org circl.lu -a -o .\n```\n\n2. Creation of variations for a file who contains domain name, using character omission - subdomain - hyphenation.\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py -fdn domain.txt -co -sub -hyp -o . -fo yara\n```\n\n3. Creation of variations for `ail-project.org` and `circl.lu`, using all algorithm and using dns resolution.\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py -dn ail-project.org circl.lu -a -dnsr -o .\n```\n\n4. Creation of variations for `ail-project.org`  and give the algorithm that generate the variation (**only for text format**).\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py -dn ail-project.org -a -o - -var\n```\n\n# Used as a library\n\n## To run all algorithms\n\n```python\nfrom ail_typo_squatting import runAll\nimport math\n\nresultList = list()\ndomainList = ["google.com"]\nformatoutput = "yara"\npathOutput = "."\nfor domain in domainList:\n    resultList = runAll(\n        domain=domain, \n        limit=math.inf, \n        formatoutput=formatoutput, \n        pathOutput=pathOutput, \n        verbose=False, \n        givevariations=False,\n        keeporiginal=False\n    )\n\n    print(resultList)\n    resultList = list()\n```\n\n## To run specific algorithm\n\n```python\nfrom ail_typo_squatting import formatOutput, omission, subdomain, addDash\nimport math\n\nresultList = list()\ndomainList = ["google.com"]\nlimit = math.inf\nformatoutput = "yara"\npathOutput = "."\nfor domain in domainList:\n    resultList = omission(domain=domain, resultList=resultList, verbose=False, limit=limit, givevariations=False,  keeporiginal=False)\n\n    resultList = subdomain(domain=domain, resultList=resultList, verbose=False, limit=limit, givevariations=False,  keeporiginal=False)\n\n    resultList = addDash(domain=domain, resultList=resultList, verbose=False, limit=limit, givevariations=False,  keeporiginal=False)\n\n    print(resultList)\n    formatOutput(format=formatoutput, resultList=resultList, domain=domain, pathOutput=pathOutput, givevariations=False)\n\n    resultList = list()\n```\n\n# Sample output\n\nThere\'s **4 format** possible for the output file:\n\n- text\n- yara\n- regex\n- sigma\n\nFor **Text** file, each line is a variation.\n\n```\nail-project.org\nil-project.org\nal-project.org\nai-project.org\nailproject.org\nail-roject.org\nail-poject.org\nail-prject.org\nail-proect.org\nail-projct.org\nail-projet.org\nail-projec.org\naail-project.org\naiil-project.org\n...\n```\n\nFor **Yara** file, each rule is a variation.\n\n```\nrule ail-project_org {\n    meta:\n        domain = "ail-project.org"\n    strings: \n        $s0 = "ail-project.org"\n        $s1 = "il-project.org"\n        $s2 = "al-project.org"\n        $s3 = "ai-project.org"\n        $s4 = "ailproject.org"\n        $s5 = "ail-roject.org"\n        $s6 = "ail-poject.org"\n        $s7 = "ail-prject.org"\n        $s8 = "ail-proect.org"\n        $s9 = "ail-projct.org"\n        $s10 = "ail-projet.org"\n        $s11 = "ail-projec.org"\n    condition:\n         any of ($s*)\n}\n```\n\nFor **Regex** file, each variations is transform into regex and concatenate with other to do only one big regex.\n\n```\nail\\-project\\.org|il\\-project\\.org|al\\-project\\.org|ai\\-project\\.org|ailproject\\.org|ail\\-roject\\.org|ail\\-poject\\.org|ail\\-prject\\.org|ail\\-proect\\.org|ail\\-projct\\.org|ail\\-projet\\.org|ail\\-projec\\.org\n```\n\nFor **Sigma** file, each variations are list under `variations` key.\n\n```\ntitle: ail-project.org\nvariations:\n- ail-project.org\n- il-project.org\n- al-project.org\n- ai-project.org\n- ailproject.org\n- ail-roject.org\n- ail-poject.org\n- ail-prject.org\n- ail-proect.org\n- ail-projct.org\n- ail-projet.org\n- ail-projec.org\n```\n\n## DNS output\n\nIn case DNS resolve is selected, an additional file will be created in JSON format\n\neach keys are variations and may have a field "ip" if the domain name have been resolved. The filed "NotExist" will be there each time with a Boolean value to determine if the domain is existing or not.\n\n```json\n{\n    "circl.lu": {\n        "NotExist": false,\n        "ip": [\n            "185.194.93.14"\n        ]\n    },\n    "ircl.lu": {\n        "NotExist": true\n    },\n    "crcl.lu": {\n        "NotExist": true\n    },\n    "cicl.lu": {\n        "NotExist": true\n    },\n    "cirl.lu": {\n        "NotExist": true\n    },\n    "circ.lu": {\n        "NotExist": true\n    },\n    "ccircl.lu": {\n        "NotExist": true\n    },\n    "ciircl.lu": {\n        "NotExist": true\n    },\n    ...\n}\n```\n\n# List of algorithms used\n\n| Algo               | Description                                                                                                                                                                                                                               |\n|:------------------ |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| AddDash            | These typos are created by adding a dash between the first and last character in a string.                                                                                                                                                |\n| Addition           | These typos are created by add a characters in the domain name.                                                                                                                                                                           |\n| AddDynamicDns      | These typos are created by adding a dynamic dns at the end of the original domain.                                                                                                                                                        |\n| AddTld             | These typos are created by adding a tld before the right tld. Example: google.com becomes google.com.it                                                                                                                                   |\n| Bitsquatting       | These typos are created by substituting a character with the set of valid characters that can be made after a single bit flip. For example, facebook.com becomes bacebook.com, dacebook.com, faaebook.com,fabebook.com,facabook.com, etc. |\n| ChangeDotDash      | These typos are created by changing a dot to a dash.                                                                                                                                                                                      |\n| ChangeOrder        | These typos are created by changing the order of letters in the each part of the domain.                                                                                                                                                  |\n| CommonMisspelling  | These typos are created by changing a word by is misspelling. Over 8000 common misspellings from Wikipedia. For example, www.youtube.com becomes www.youtub.com and www.abseil.com becomes www.absail.com.                                |\n| Double Replacement | These typos are created by replacing identical, consecutive letters of the domain name with letters to the immediate left and right on the keyboard.                                                                                      |\n| Homoglyph          | These typos are created by replacing characters to another character that look similar but are different.  An example is that the lower case l looks similar to the numeral one, e.g. l vs 1. For example, google.com becomes goog1e.com. |\n| Homophones         | These typos are created by changing word by an other who sound the same when spoken. Over 450 sets of words that sound the same when spoken. For example, www.base.com becomes www.bass.com.                                              |\n| KeyboardInsertion  | These typos are created by inserting letters to the immediate left and right on the keyboard of each letter.                                                                                                                              |\n| MissingDot         | These typos are created by deleting a dot from the domain name.                                                                                                                                                                           |\n| NumeralSwap        | These typos are created by changing a number to words and vice versa. For example, circlone.lu becomes circl1.lu.                                                                                                                         |\n| Omission           | These typos are created by leaving out a letter of the domain name, one letter at a time.                                                                                                                                                 |\n| Repetition         | These typos are created by repeating a letter of the domain name.                                                                                                                                                                         |\n| Replacement        | These typos are created by replacing each letter of the domain name with letters to the immediate left and right on the keyboard. (QWERTY, AZERTY, QWERTZ, DVORAK)                                                                        |\n| StripDash          | These typos are created by deleting a dash from the domain name.                                                                                                                                                                          |\n| SingularPluralize  | These typos are created by making a singular domain plural and vice versa.                                                                                                                                                                |\n| Subdomain          | These typos are created by placing a dot in the domain name in order to create subdomain. Example: google.com becomes goo.gle.com                                                                                                         |\n| Transposition      | These typos are created by swapping the order of adjacent letters in the domain name.                                                                                                                                                     |\n| VowelSwap          | These typos are created by swapping vowels within the domain name except for the first letter. For example, www.google.com becomes www.gaagle.com.                                                                                        |\n| WrongTld           | These typos are created by changing the original top level domain to another. For example, www.trademe.co.nz becomes www.trademe.co.mz and www.google.com becomes www.google.org Uses the 19 most common top level domains.               |\n| WrongSld           | These typos are created by changing the original second level domain to another. For example, www.trademe.co.uk becomes www.trademe.ac.uk and www.google.com will still be www.google.com .                                               |\n\n# Acknowledgment\n\n![](./img/cef.png)\n\nThe project has been co-funded by CEF-TC-2020-2 - 2020-EU-IA-0260 - JTAN - Joint Threat Analysis Network.\n',
+    'long_description': '# ail-typo-squatting\n\nail-typo-squatting is a Python library to generate list of potential typo squatting domains with domain name permutation engine to feed AIL and other systems. \n\nThe tool can be used as a stand-alone tool or to feed other systems.\n\n# Requirements\n\n- Python 3.6+\n- [inflect](https://github.com/jaraco/inflect) library\n- [pyyaml](https://pyyaml.org/wiki/PyYAMLDocumentation)\n\n## Optional\n\n- [dnspython](https://github.com/rthalley/dnspython)\n\n# Installation\n\n## Source install\n\nail-typo-squatting can be install with poetry. If you don\'t have poetry installed, you can do the following `curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python`.\n\n```bash\n$ poetry install\n$ poetry shell\n$ cd ail-typo-squatting\n$ python typo.py -h\n```\n\n## pip installation\n\n```bash\n$ pip3 install ail-typo-squatting\n```\n\n# Usage\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py --help  \nusage: typo.py [-h] [-v] [-dn DOMAINNAME [DOMAINNAME ...]] [-fdn FILEDOMAINNAME] [-o OUTPUT] [-fo FORMATOUTPUT] [-dnsr] [-dnsl] [-l LIMIT] [-var] [-ko] [-a] [-om] [-repe] [-repl] [-drepl] [-cho] [-add]\n               [-md] [-sd] [-vs] [-ada] [-hg] [-ahg] [-cm] [-hp] [-wt] [-wsld] [-at] [-sub] [-sp] [-cdd] [-addns] [-ns]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -v                    verbose, more display\n  -dn DOMAINNAME [DOMAINNAME ...], --domainName DOMAINNAME [DOMAINNAME ...]\n                        list of domain name\n  -fdn FILEDOMAINNAME, --filedomainName FILEDOMAINNAME\n                        file containing list of domain name\n  -o OUTPUT, --output OUTPUT\n                        path to ouput location\n  -fo FORMATOUTPUT, --formatoutput FORMATOUTPUT\n                        format for the output file, yara - regex - yaml - text. Default: text\n  -dnsr, --dnsresolving\n                        resolve all variation of domain name to see if it\'s up or not\n  -dnsl, --dnslimited   resolve all variation of domain name but keep only up domain in final result json\n  -l LIMIT, --limit LIMIT\n                        limit of variations for a domain name\n  -var, --givevariations\n                        give the algo that generate variations\n  -ko, --keeporiginal   Keep in the result list the original domain name\n  -a, --all             Use all algo\n  -om, --omission       Leave out a letter of the domain name\n  -repe, --repetition   Character Repeat\n  -repl, --replacement  Character replacement\n  -drepl, --doublereplacement\n                        Double Character Replacement\n  -cho, --changeorder   Change the order of letters in word\n  -add, --addition      Add a character in the domain name\n  -md, --missingdot     Delete a dot from the domain name\n  -sd, --stripdash      Delete of a dash from the domain name\n  -vs, --vowelswap      Swap vowels within the domain name\n  -ada, --adddash       Add a dash between the first and last character in a string\n  -hg, --homoglyph      One or more characters that look similar to another character but are different are called homogylphs\n  -ahg, --all_homoglyph\n                        generate all possible homoglyph permutations. Ex: circl.lu, e1rc1.lu\n  -cm, --commonmisspelling\n                        Change a word by is misspellings\n  -hp, --homophones     Change word by an other who sound the same when spoken\n  -wt, --wrongtld       Change the original top level domain to another\n  -wsld, --wrongsld     Change the original second level domain to another\n  -at, --addtld         Adding a tld before the original tld\n  -sub, --subdomain     Insert a dot at varying positions to create subdomain\n  -sp, --singularpluralize\n                        Create by making a singular domain plural and vice versa\n  -cdd, --changedotdash\n                        Change dot to dash\n  -addns, --adddynamicdns\n                        Add dynamic dns at the end of the domain\n  -ns, --numeralswap    Change a numbers to words and vice versa. Ex: circlone.lu, circl1.lu\n```\n\n# Usage example\n\n1. Creation of variations for `ail-project.org` and `circl.lu`, using all algorithm.\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py -dn ail-project.org circl.lu -a -o .\n```\n\n2. Creation of variations for a file who contains domain name, using character omission - subdomain - hyphenation.\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py -fdn domain.txt -co -sub -hyp -o . -fo yara\n```\n\n3. Creation of variations for `ail-project.org` and `circl.lu`, using all algorithm and using dns resolution.\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py -dn ail-project.org circl.lu -a -dnsr -o .\n```\n\n4. Creation of variations for `ail-project.org`  and give the algorithm that generate the variation (**only for text format**).\n\n```bash\ndacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py -dn ail-project.org -a -o - -var\n```\n\n# Used as a library\n\n## To run all algorithms\n\n```python\nfrom ail_typo_squatting import runAll\nimport math\n\nresultList = list()\ndomainList = ["google.com"]\nformatoutput = "yara"\npathOutput = "."\nfor domain in domainList:\n    resultList = runAll(\n        domain=domain, \n        limit=math.inf, \n        formatoutput=formatoutput, \n        pathOutput=pathOutput, \n        verbose=False, \n        givevariations=False,\n        keeporiginal=False\n    )\n\n    print(resultList)\n    resultList = list()\n```\n\n## To run specific algorithm\n\n```python\nfrom ail_typo_squatting import formatOutput, omission, subdomain, addDash\nimport math\n\nresultList = list()\ndomainList = ["google.com"]\nlimit = math.inf\nformatoutput = "yara"\npathOutput = "."\nfor domain in domainList:\n    resultList = omission(domain=domain, resultList=resultList, verbose=False, limit=limit, givevariations=False,  keeporiginal=False)\n\n    resultList = subdomain(domain=domain, resultList=resultList, verbose=False, limit=limit, givevariations=False,  keeporiginal=False)\n\n    resultList = addDash(domain=domain, resultList=resultList, verbose=False, limit=limit, givevariations=False,  keeporiginal=False)\n\n    print(resultList)\n    formatOutput(format=formatoutput, resultList=resultList, domain=domain, pathOutput=pathOutput, givevariations=False)\n\n    resultList = list()\n```\n\n# Sample output\n\nThere\'s **4 format** possible for the output file:\n\n- text\n- yara\n- regex\n- sigma\n\nFor **Text** file, each line is a variation.\n\n```\nail-project.org\nil-project.org\nal-project.org\nai-project.org\nailproject.org\nail-roject.org\nail-poject.org\nail-prject.org\nail-proect.org\nail-projct.org\nail-projet.org\nail-projec.org\naail-project.org\naiil-project.org\n...\n```\n\nFor **Yara** file, each rule is a variation.\n\n```\nrule ail-project_org {\n    meta:\n        domain = "ail-project.org"\n    strings: \n        $s0 = "ail-project.org"\n        $s1 = "il-project.org"\n        $s2 = "al-project.org"\n        $s3 = "ai-project.org"\n        $s4 = "ailproject.org"\n        $s5 = "ail-roject.org"\n        $s6 = "ail-poject.org"\n        $s7 = "ail-prject.org"\n        $s8 = "ail-proect.org"\n        $s9 = "ail-projct.org"\n        $s10 = "ail-projet.org"\n        $s11 = "ail-projec.org"\n    condition:\n         any of ($s*)\n}\n```\n\nFor **Regex** file, each variations is transform into regex and concatenate with other to do only one big regex.\n\n```\nail\\-project\\.org|il\\-project\\.org|al\\-project\\.org|ai\\-project\\.org|ailproject\\.org|ail\\-roject\\.org|ail\\-poject\\.org|ail\\-prject\\.org|ail\\-proect\\.org|ail\\-projct\\.org|ail\\-projet\\.org|ail\\-projec\\.org\n```\n\nFor **Sigma** file, each variations are list under `variations` key.\n\n```\ntitle: ail-project.org\nvariations:\n- ail-project.org\n- il-project.org\n- al-project.org\n- ai-project.org\n- ailproject.org\n- ail-roject.org\n- ail-poject.org\n- ail-prject.org\n- ail-proect.org\n- ail-projct.org\n- ail-projet.org\n- ail-projec.org\n```\n\n## DNS output\n\nIn case DNS resolve is selected, an additional file will be created in JSON format\n\neach keys are variations and may have a field "ip" if the domain name have been resolved. The filed "NotExist" will be there each time with a Boolean value to determine if the domain is existing or not.\n\n```json\n{\n    "circl.lu": {\n        "NotExist": false,\n        "ip": [\n            "185.194.93.14"\n        ]\n    },\n    "ircl.lu": {\n        "NotExist": true\n    },\n    "crcl.lu": {\n        "NotExist": true\n    },\n    "cicl.lu": {\n        "NotExist": true\n    },\n    "cirl.lu": {\n        "NotExist": true\n    },\n    "circ.lu": {\n        "NotExist": true\n    },\n    "ccircl.lu": {\n        "NotExist": true\n    },\n    "ciircl.lu": {\n        "NotExist": true\n    },\n    ...\n}\n```\n\n# List of algorithms used\n\n| Algo               | Description                                                                                                                                                                                                                               |\n|:------------------ |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| AddDash            | These typos are created by adding a dash between the first and last character in a string.                                                                                                                                                |\n| Addition           | These typos are created by add a characters in the domain name.                                                                                                                                                                           |\n| AddDynamicDns      | These typos are created by adding a dynamic dns at the end of the original domain.                                                                                                                                                        |\n| AddTld             | These typos are created by adding a tld before the right tld. Example: google.com becomes google.com.it                                                                                                                                   |\n| ChangeDotDash      | These typos are created by changing a dot to a dash.                                                                                                                                                                                      |\n| ChangeOrder        | These typos are created by changing the order of letters in the each part of the domain.                                                                                                                                                  |\n| CommonMisspelling  | These typos are created by changing a word by is misspelling. Over 8000 common misspellings from Wikipedia. For example, www.youtube.com becomes www.youtub.com and www.abseil.com becomes www.absail.com.                                |\n| Double Replacement | These typos are created by replacing identical, consecutive letters of the domain name.                                                                                                                                                   |\n| Homoglyph          | These typos are created by replacing characters to another character that look similar but are different.  An example is that the lower case l looks similar to the numeral one, e.g. l vs 1. For example, google.com becomes goog1e.com. |\n| Homophones         | These typos are created by changing word by an other who sound the same when spoken. Over 450 sets of words that sound the same when spoken. For example, www.base.com becomes www.bass.com.                                              |\n| MissingDot         | These typos are created by deleting a dot from the domain name.                                                                                                                                                                           |\n| NumeralSwap        | These typos are created by changing a number to words and vice versa. For example, circlone.lu becomes circl1.lu.                                                                                                                         |\n| Omission           | These typos are created by leaving out a letter of the domain name, one letter at a time.                                                                                                                                                 |\n| Repetition         | These typos are created by repeating a letter of the domain name.                                                                                                                                                                         |\n| Replacement        | These typos are created by replacing each letter of the domain name.                                                                                                                                                                      |\n| StripDash          | These typos are created by deleting a dash from the domain name.                                                                                                                                                                          |\n| SingularPluralize  | These typos are created by making a singular domain plural and vice versa.                                                                                                                                                                |\n| Subdomain          | These typos are created by placing a dot in the domain name in order to create subdomain. Example: google.com becomes goo.gle.com                                                                                                         |\n| VowelSwap          | These typos are created by swapping vowels within the domain name except for the first letter. For example, www.google.com becomes www.gaagle.com.                                                                                        |\n| WrongTld           | These typos are created by changing the original top level domain to another. For example, www.trademe.co.nz becomes www.trademe.co.mz and www.google.com becomes www.google.org Uses the 19 most common top level domains.               |\n| WrongSld           | These typos are created by changing the original second level domain to another. For example, www.trademe.co.uk becomes www.trademe.ac.uk and www.google.com will still be www.google.com .                                               |\n\n# Acknowledgment\n\n![](./img/cef.png)\n\nThe project has been co-funded by CEF-TC-2020-2 - 2020-EU-IA-0260 - JTAN - Joint Threat Analysis Network.\n',
     'author': 'David Cruciani',
     'author_email': 'david.cruciani@securitymadein.lu',
     'maintainer': 'Alexandre Dulaunoy',
     'maintainer_email': 'a@foo.be',
-    'url': 'https://github.com/ail-project/ail-typo-squatting',
+    'url': 'https://github.com/typosquatter/ail-typo-squatting',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `ail_typo_squatting-2.4.0/PKG-INFO` & `ail_typo_squatting-2.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: ail-typo-squatting
-Version: 2.4.0
-Summary: Generate list of domain name using Domain name permutation engine to feed AIL
-Home-page: https://github.com/ail-project/ail-typo-squatting
-License: BSD-2-Clause
-Keywords: typo-squatting,typosquatting
-Author: David Cruciani
-Author-email: david.cruciani@securitymadein.lu
-Maintainer: Alexandre Dulaunoy
-Maintainer-email: a@foo.be
-Requires-Python: >=3.6,<4.0
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dnspython (>=2.2.0,<3.0.0)
-Requires-Dist: inflect (>=5.3.0,<6.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: tldextract (>=3.1.2,<4.0.0)
-Project-URL: Repository, https://github.com/ail-project/ail-typo-squatting
-Description-Content-Type: text/markdown
-
 # ail-typo-squatting
 
 ail-typo-squatting is a Python library to generate list of potential typo squatting domains with domain name permutation engine to feed AIL and other systems. 
 
 The tool can be used as a stand-alone tool or to feed other systems.
 
 # Requirements
@@ -61,65 +33,65 @@
 $ pip3 install ail-typo-squatting
 ```
 
 # Usage
 
 ```bash
 dacru@dacru:~/git/ail-typo-squatting/bin$ python3 typo.py --help  
-usage: typo.py [-h] [-v] [-dn DOMAINNAME [DOMAINNAME ...]] [-fdn FILEDOMAINNAME] [-o OUTPUT] [-fo FORMATOUTPUT] [-dnsr] [-l LIMIT] [-var] [-ko] [-a] [-om] [-repe] [-tra] [-repl] [-drepl] [-cho] [-ki] [-add] [-md] [-sd]
-               [-vs] [-ada] [-bs] [-hg] [-ahg] [-cm] [-hp] [-wt] [-at] [-sub] [-sp] [-cdd]
+usage: typo.py [-h] [-v] [-dn DOMAINNAME [DOMAINNAME ...]] [-fdn FILEDOMAINNAME] [-o OUTPUT] [-fo FORMATOUTPUT] [-dnsr] [-dnsl] [-l LIMIT] [-var] [-ko] [-a] [-om] [-repe] [-repl] [-drepl] [-cho] [-add]
+               [-md] [-sd] [-vs] [-ada] [-hg] [-ahg] [-cm] [-hp] [-wt] [-wsld] [-at] [-sub] [-sp] [-cdd] [-addns] [-ns]
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -v                    verbose, more display
   -dn DOMAINNAME [DOMAINNAME ...], --domainName DOMAINNAME [DOMAINNAME ...]
                         list of domain name
   -fdn FILEDOMAINNAME, --filedomainName FILEDOMAINNAME
                         file containing list of domain name
   -o OUTPUT, --output OUTPUT
                         path to ouput location
   -fo FORMATOUTPUT, --formatoutput FORMATOUTPUT
                         format for the output file, yara - regex - yaml - text. Default: text
   -dnsr, --dnsresolving
                         resolve all variation of domain name to see if it's up or not
+  -dnsl, --dnslimited   resolve all variation of domain name but keep only up domain in final result json
   -l LIMIT, --limit LIMIT
                         limit of variations for a domain name
   -var, --givevariations
                         give the algo that generate variations
   -ko, --keeporiginal   Keep in the result list the original domain name
   -a, --all             Use all algo
   -om, --omission       Leave out a letter of the domain name
   -repe, --repetition   Character Repeat
-  -tra, --transposition
-                        Swappe the order of adjacent letters in the domain name
-  -repl, --replacement  Adjacent character replacement to the immediate left and right on the keyboard
+  -repl, --replacement  Character replacement
   -drepl, --doublereplacement
                         Double Character Replacement
   -cho, --changeorder   Change the order of letters in word
-  -ki, --keyboardinsertion
-                        Adjacent character insertion of letters to the immediate left and right on the keyboard of each letter
   -add, --addition      Add a character in the domain name
   -md, --missingdot     Delete a dot from the domain name
   -sd, --stripdash      Delete of a dash from the domain name
   -vs, --vowelswap      Swap vowels within the domain name
   -ada, --adddash       Add a dash between the first and last character in a string
-  -bs, --bitsquatting   The character is substituted with the set of valid characters that can be made after a single bit flip
   -hg, --homoglyph      One or more characters that look similar to another character but are different are called homogylphs
   -ahg, --all_homoglyph
                         generate all possible homoglyph permutations. Ex: circl.lu, e1rc1.lu
   -cm, --commonmisspelling
                         Change a word by is misspellings
   -hp, --homophones     Change word by an other who sound the same when spoken
   -wt, --wrongtld       Change the original top level domain to another
+  -wsld, --wrongsld     Change the original second level domain to another
   -at, --addtld         Adding a tld before the original tld
   -sub, --subdomain     Insert a dot at varying positions to create subdomain
   -sp, --singularpluralize
                         Create by making a singular domain plural and vice versa
   -cdd, --changedotdash
                         Change dot to dash
+  -addns, --adddynamicdns
+                        Add dynamic dns at the end of the domain
+  -ns, --numeralswap    Change a numbers to words and vice versa. Ex: circlone.lu, circl1.lu
 ```
 
 # Usage example
 
 1. Creation of variations for `ail-project.org` and `circl.lu`, using all algorithm.
 
 ```bash
@@ -316,34 +288,30 @@
 
 | Algo               | Description                                                                                                                                                                                                                               |
 |:------------------ |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | AddDash            | These typos are created by adding a dash between the first and last character in a string.                                                                                                                                                |
 | Addition           | These typos are created by add a characters in the domain name.                                                                                                                                                                           |
 | AddDynamicDns      | These typos are created by adding a dynamic dns at the end of the original domain.                                                                                                                                                        |
 | AddTld             | These typos are created by adding a tld before the right tld. Example: google.com becomes google.com.it                                                                                                                                   |
-| Bitsquatting       | These typos are created by substituting a character with the set of valid characters that can be made after a single bit flip. For example, facebook.com becomes bacebook.com, dacebook.com, faaebook.com,fabebook.com,facabook.com, etc. |
 | ChangeDotDash      | These typos are created by changing a dot to a dash.                                                                                                                                                                                      |
 | ChangeOrder        | These typos are created by changing the order of letters in the each part of the domain.                                                                                                                                                  |
 | CommonMisspelling  | These typos are created by changing a word by is misspelling. Over 8000 common misspellings from Wikipedia. For example, www.youtube.com becomes www.youtub.com and www.abseil.com becomes www.absail.com.                                |
-| Double Replacement | These typos are created by replacing identical, consecutive letters of the domain name with letters to the immediate left and right on the keyboard.                                                                                      |
+| Double Replacement | These typos are created by replacing identical, consecutive letters of the domain name.                                                                                                                                                   |
 | Homoglyph          | These typos are created by replacing characters to another character that look similar but are different.  An example is that the lower case l looks similar to the numeral one, e.g. l vs 1. For example, google.com becomes goog1e.com. |
 | Homophones         | These typos are created by changing word by an other who sound the same when spoken. Over 450 sets of words that sound the same when spoken. For example, www.base.com becomes www.bass.com.                                              |
-| KeyboardInsertion  | These typos are created by inserting letters to the immediate left and right on the keyboard of each letter.                                                                                                                              |
 | MissingDot         | These typos are created by deleting a dot from the domain name.                                                                                                                                                                           |
 | NumeralSwap        | These typos are created by changing a number to words and vice versa. For example, circlone.lu becomes circl1.lu.                                                                                                                         |
 | Omission           | These typos are created by leaving out a letter of the domain name, one letter at a time.                                                                                                                                                 |
 | Repetition         | These typos are created by repeating a letter of the domain name.                                                                                                                                                                         |
-| Replacement        | These typos are created by replacing each letter of the domain name with letters to the immediate left and right on the keyboard. (QWERTY, AZERTY, QWERTZ, DVORAK)                                                                        |
+| Replacement        | These typos are created by replacing each letter of the domain name.                                                                                                                                                                      |
 | StripDash          | These typos are created by deleting a dash from the domain name.                                                                                                                                                                          |
 | SingularPluralize  | These typos are created by making a singular domain plural and vice versa.                                                                                                                                                                |
 | Subdomain          | These typos are created by placing a dot in the domain name in order to create subdomain. Example: google.com becomes goo.gle.com                                                                                                         |
-| Transposition      | These typos are created by swapping the order of adjacent letters in the domain name.                                                                                                                                                     |
 | VowelSwap          | These typos are created by swapping vowels within the domain name except for the first letter. For example, www.google.com becomes www.gaagle.com.                                                                                        |
 | WrongTld           | These typos are created by changing the original top level domain to another. For example, www.trademe.co.nz becomes www.trademe.co.mz and www.google.com becomes www.google.org Uses the 19 most common top level domains.               |
 | WrongSld           | These typos are created by changing the original second level domain to another. For example, www.trademe.co.uk becomes www.trademe.ac.uk and www.google.com will still be www.google.com .                                               |
 
 # Acknowledgment
 
 ![](./img/cef.png)
 
 The project has been co-funded by CEF-TC-2020-2 - 2020-EU-IA-0260 - JTAN - Joint Threat Analysis Network.
-
```

