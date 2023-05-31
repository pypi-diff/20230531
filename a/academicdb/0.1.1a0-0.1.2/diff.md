# Comparing `tmp/academicdb-0.1.1a0.tar.gz` & `tmp/academicdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "academicdb-0.1.1a0.tar", max compression
+gzip compressed data, was "academicdb-0.1.2.tar", max compression
```

## Comparing `academicdb-0.1.1a0.tar` & `academicdb-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     1070 2023-03-31 20:59:16.841096 academicdb-0.1.1a0/LICENSE
--rw-r--r--   0        0        0     7380 2023-04-01 15:53:49.731611 academicdb-0.1.1a0/README.md
--rw-r--r--   0        0        0      668 2023-04-01 15:56:14.182912 academicdb-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       20 2023-03-31 22:40:28.945142 academicdb-0.1.1a0/src/academicdb/__about__.py
--rw-r--r--   0        0        0        0 2023-03-31 17:39:51.516988 academicdb-0.1.1a0/src/academicdb/__init__.py
--rw-r--r--   0        0        0     2519 2023-03-31 22:40:29.005142 academicdb-0.1.1a0/src/academicdb/coauthor_setup.py
--rw-r--r--   0        0        0     6731 2023-03-31 22:40:29.125141 academicdb-0.1.1a0/src/academicdb/crossref_utils.py
--rw-r--r--   0        0        0        0 2023-03-31 20:35:22.725982 academicdb-0.1.1a0/src/academicdb/data/__init__.py
--rw-r--r--   0        0        0      163 2023-03-31 20:53:00.979235 academicdb-0.1.1a0/src/academicdb/data/latex_footer.tex
--rw-r--r--   0        0        0     1710 2023-03-31 17:39:51.520988 academicdb-0.1.1a0/src/academicdb/data/latex_header.tex
--rw-r--r--   0        0        0     5635 2023-03-31 22:40:29.025142 academicdb-0.1.1a0/src/academicdb/database.py
--rwxr-xr-x   0        0        0     8219 2023-04-01 14:38:53.741958 academicdb-0.1.1a0/src/academicdb/dbbuilder.py
--rw-r--r--   0        0        0      463 2023-03-31 22:40:28.957142 academicdb-0.1.1a0/src/academicdb/fix_conference_file.py
--rw-r--r--   0        0        0     7038 2023-03-31 22:40:29.125141 academicdb-0.1.1a0/src/academicdb/orcid.py
--rw-r--r--   0        0        0     5922 2023-03-31 22:40:29.077141 academicdb-0.1.1a0/src/academicdb/publication.py
--rw-r--r--   0        0        0      995 2023-03-31 22:40:28.969142 academicdb-0.1.1a0/src/academicdb/publication_utils.py
--rw-r--r--   0        0        0     4071 2023-03-31 22:40:29.049141 academicdb-0.1.1a0/src/academicdb/pubmed.py
--rw-r--r--   0        0        0     1620 2023-04-01 15:26:23.756619 academicdb-0.1.1a0/src/academicdb/query.py
--rw-r--r--   0        0        0     1684 2023-03-31 22:40:28.985142 academicdb-0.1.1a0/src/academicdb/recordConverter.py
--rwxr-xr-x   0        0        0    13363 2023-04-01 15:18:40.258125 academicdb-0.1.1a0/src/academicdb/render_cv.py
--rw-r--r--   0        0        0    13412 2023-04-01 15:32:55.130810 academicdb-0.1.1a0/src/academicdb/researcher.py
--rw-r--r--   0        0        0     9579 2023-03-31 22:40:29.121141 academicdb-0.1.1a0/src/academicdb/utils.py
--rw-r--r--   0        0        0     8265 1970-01-01 00:00:00.000000 academicdb-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-31 20:59:16.841096 academicdb-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7593 2023-04-04 22:52:14.081020 academicdb-0.1.2/README.md
+-rw-r--r--   0        0        0      677 2023-05-31 17:25:34.908865 academicdb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-03-31 22:40:28.945142 academicdb-0.1.2/src/academicdb/__about__.py
+-rw-r--r--   0        0        0        0 2023-03-31 17:39:51.516988 academicdb-0.1.2/src/academicdb/__init__.py
+-rw-r--r--   0        0        0     2719 2023-04-03 22:30:47.671692 academicdb-0.1.2/src/academicdb/coauthor_setup.py
+-rw-r--r--   0        0        0     6899 2023-04-04 19:46:38.212799 academicdb-0.1.2/src/academicdb/crossref_utils.py
+-rw-r--r--   0        0        0        0 2023-03-31 20:35:22.725982 academicdb-0.1.2/src/academicdb/data/__init__.py
+-rw-r--r--   0        0        0      163 2023-03-31 20:53:00.979235 academicdb-0.1.2/src/academicdb/data/latex_footer.tex
+-rw-r--r--   0        0        0     1710 2023-03-31 17:39:51.520988 academicdb-0.1.2/src/academicdb/data/latex_header.tex
+-rw-r--r--   0        0        0     5696 2023-04-04 22:52:14.081020 academicdb-0.1.2/src/academicdb/database.py
+-rwxr-xr-x   0        0        0     8219 2023-04-01 14:38:53.741958 academicdb-0.1.2/src/academicdb/dbbuilder.py
+-rw-r--r--   0        0        0      463 2023-03-31 22:40:28.957142 academicdb-0.1.2/src/academicdb/fix_conference_file.py
+-rwxr-xr-x   0        0        0     1553 2023-04-04 17:06:53.782307 academicdb-0.1.2/src/academicdb/get_collaborators.py
+-rw-r--r--   0        0        0     7120 2023-04-04 22:52:14.081020 academicdb-0.1.2/src/academicdb/orcid.py
+-rw-r--r--   0        0        0    95796 2023-05-29 14:26:47.869466 academicdb-0.1.2/src/academicdb/output/publications.md
+-rw-r--r--   0        0        0     5922 2023-03-31 22:40:29.077141 academicdb-0.1.2/src/academicdb/publication.py
+-rw-r--r--   0        0        0      995 2023-03-31 22:40:28.969142 academicdb-0.1.2/src/academicdb/publication_utils.py
+-rw-r--r--   0        0        0     5504 2023-04-03 23:06:48.958356 academicdb-0.1.2/src/academicdb/pubmed.py
+-rw-r--r--   0        0        0     1620 2023-04-01 15:26:23.756619 academicdb-0.1.2/src/academicdb/query.py
+-rw-r--r--   0        0        0     1684 2023-03-31 22:40:28.985142 academicdb-0.1.2/src/academicdb/recordConverter.py
+-rwxr-xr-x   0        0        0    13778 2023-04-04 22:52:14.081020 academicdb-0.1.2/src/academicdb/render_cv.py
+-rwxr-xr-x   0        0        0     5598 2023-05-29 14:38:54.424618 academicdb-0.1.2/src/academicdb/render_pubs.py
+-rw-r--r--   0        0        0    13466 2023-04-04 20:04:37.068467 academicdb-0.1.2/src/academicdb/researcher.py
+-rw-r--r--   0        0        0     9579 2023-03-31 22:40:29.121141 academicdb-0.1.2/src/academicdb/utils.py
+-rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 academicdb-0.1.2/PKG-INFO
```

### Comparing `academicdb-0.1.1a0/LICENSE` & `academicdb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `academicdb-0.1.1a0/README.md` & `academicdb-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 - [Install MongoDB](https://www.mongodb.com/docs/manual/installation/) on your own system. 
 - Create a free cloud MongoDB instance [here](https://www.mongodb.com/cloud).
 
 The former is easier, but I prefer the latter because it allows the database to accessed from any system. 
 
 Rendering the CV after building the database requires that LaTeX be installed on your system and available from the command line.  There are various LaTeX distributions depending on your operating system.
 
+_Note: If you get an error that the font Tex Gyre Termes is not installed when executing `render_cv`, you can install it using Homebrew like so:_
+```{bash}
+$ brew tap homebrew/cask-fonts
+$ brew install --cask font-tex-gyre-termes
+```
+
 ### Configuring academicdb
 
 To use academicdb, you must first set up some configuration files, which will reside in `~/.academicdb`.  The most important is `config.toml`, which contains all of the details about you that are used to retrieve your information.  Here are the contents of mine as an example:
 
 ```
 [researcher]
 lastname = "poldrack"
@@ -46,32 +52,32 @@
 ]
 ```
 
 Most of this should be self-explanatory. There are several identifiers that you need to specify:
 
 - **ORCID**: This is a unique identifier for researchers.  If you don't already have an ORCID you can get one [here](http://orcid.org).  You will need to enter information about your education, employment, invited position and distinctions, and memberships and service into your ORCID account since that is where academicdb looks for that information.
 - **Google Scholar**: You will also need to retrieve your Google Scholar ID.  Once you have set up your profile, go to the "My Profile" page.  The URL from that page contains your id: for example, my URL is *https://scholar.google.com/citations?user=RbmLvDIAAAAJ&hl=en* and the ID is *RbmLvDIAAAAJ*.  
-- **Scopus**: Scopus is a service run by Elsevier.  I know that they are the bad guys, but Scopus provides a service that is not available from anywhere else: For each reference it provides a set of unique identifiers for the coauthors, which can be used to retreive their affilation information.  This is essential for generating the NSF collaborators spreadsheet.
+- **Scopus**: Scopus is a service run by Elsevier. It provides a service that is not available from anywhere else: For each reference it provides a set of unique identifiers for the coauthors, which can be used to retreive their affilation information.  This is essential for generating the NSF collaborators spreadsheet.
 
 ### cloud MongoDB setup
 
 If you are going to use a cloud MongoDB server, you will need to add the following lines to your `config.toml`:
 
 ```
 [mongo]
 CONNECT_STRING = 'mongodb+srv://<username>:<password>@<server>'
 ```
 
 The cloud provider should provide you with the connection string that you can paste into this variable.
 
 ## Obtaining an API key for Scopus
 
-  You will need to obtain an API key to access the Scopus database, which you can obtain from [http://dev.elsevier.com/myapikey.html](http://dev.elsevier.com/myapikey.html).  This is used by the [pybliometrics](https://pybliometrics.readthedocs.io/en/stable/) package to access the APIs; note that there are [weekly limits](https://dev.elsevier.com/api_key_settings.html) on the number of records one can access from these APIs without a subscription. If your institution has a subscription and you are on the institution's network, you may be able to bypass these. 
+  You will need to obtain an API key to access the Scopus database, which you can obtain from [http://dev.elsevier.com/myapikey.html](http://dev.elsevier.com/myapikey.html).  This is used by the [pybliometrics](https://pybliometrics.readthedocs.io/en/stable/) package to access the APIs. Note that this key will only work if you are on your institution's network and the institution has the appropriate license with Elsevier.  You can also request an institutional token from Elsevier if you wish to use the APIs from outside of your institution's network.
 
-  The first time you use the package, you will be asked by pybliometrics to enter your API key, which will be stored in `~/.pybliometrics/config.ini` for reuse.
+  The first time you use the package, you will be asked by pybliometrics to enter your API key (and InstToken if you have one), which will be stored in `~/.pybliometrics/config.ini` for reuse.
 
 ## specifying additional information
 
 There are a number of pieces of information that are difficult to reliably obtain from ORCID or other APIs, so they must be specified in a set of text files, which should be saved in the base directory that is specified when the command line `dbbuilder` tool is used.  See the `examples` directory for examples of each of these.
 
 - `editorial.csv`: information about editorial roles
 - `talks.csv`: information about non-conference talks at other institutions
```

### Comparing `academicdb-0.1.1a0/pyproject.toml` & `academicdb-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "academicdb"
-version = "0.1.1a0"
+version = "0.1.2"
 description = "Database for an academic CV"
 authors = ["Russ Poldrack <poldrack@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.5.3"
 numpy = "^1.23"
 biopython = "^1.81"
 scholarly = "^1.7.11"
 crossrefapi = "^1.5.0"
 toml = "^0.10.2"
+tomli = { version = "^2.0.1", python = "<3.11" }
 pybliometrics = "^3.4.0"
 pymongo = "^4.3.3"
 orcid = "^1.0.3"
 tomli-w = "^1.0.0"
-
-[tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 
 [tool.poetry.scripts]
 dbbuilder = "academicdb.dbbuilder:main"
 render_cv = "academicdb.render_cv:main"
 
 [build-system]
```

### Comparing `academicdb-0.1.1a0/src/academicdb/coauthor_setup.py` & `academicdb-0.1.2/src/academicdb/coauthor_setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -45,28 +45,37 @@
                     }
                 else:
                     if pub['year'] > coauthors[coauthor]['year']:
                         coauthors[coauthor]['year'] = pub['year']
     return coauthors
 
 
-if os.path.exists(dbconfigfile):
-    dbconfig = load_config(dbconfigfile)
-    assert dbconfig['mongo'][
+if os.path.exists(configfile):
+    config = load_config(configfile)
+    assert config['mongo'][
         'CONNECT_STRING'
     ], 'CONNECT_STRING must be specified in dbconfig'
     db = database.Database(
         database.MongoDatabase(
-            connect_string=dbconfig['mongo']['CONNECT_STRING']
+            connect_string=config['mongo']['CONNECT_STRING']
         )
     )
 else:
-    db = database.Database(database.MongoDatabase(overwrite=args.overwrite))
-
-if db.get_collection('coauthors') is not None:
-    db.drop_collection('coauthors')
+    db = database.Database(database.MongoDatabase(overwrite=False))
 
 publications = db.get_collection('publications')
 
-coauthors = get_coauthors(publications)
+#coauthors = get_coauthors(publications)
+
+#db.add('coauthors', list(coauthors.values()))
 
-db.add('coauthors', list(coauthors.values()))
+dois = [i['DOI'] for i in publications if i['DOI'].find('nodoi') == -1]
+recs = [Works().doi(doi) for doi in dois]
+print(len(recs))
+goodrecs = [rec for rec in recs if rec is not None]
+print(len(goodrecs))
+
+dep_ctr = 0
+for rec in goodrecs:
+    if 'published' in rec:
+        dep_ctr += 1
+print(dep_ctr)
```

### Comparing `academicdb-0.1.1a0/src/academicdb/crossref_utils.py` & `academicdb-0.1.2/src/academicdb/crossref_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,16 @@
     # don't replace pubmed info if it already exists
     for field in ['title', 'volume', 'page', 'type', 'publisher']:
         if field in record:
             f = record[field]
             if isinstance(f, list):
                 f = f[0]
             pub[field] = f
-
+    if 'published' in record and 'date-parts' in record['published']:
+        pub['publication-date'] = '-'.join([str(i) for i in record['published']['date-parts'][0]])
     # filter out pages with n/a
     if 'page' in pub and pub['page'].find('n/a') > -1:
         del pub['page']
 
     # get the title
     if len(record['container-title']) > 0:
         pub['journal'] = record['container-title'][0]
```

### Comparing `academicdb-0.1.1a0/src/academicdb/data/latex_header.tex` & `academicdb-0.1.2/src/academicdb/data/latex_header.tex`

 * *Files identical despite different names*

### Comparing `academicdb-0.1.1a0/src/academicdb/database.py` & `academicdb-0.1.2/src/academicdb/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,21 +134,22 @@
 
     def list_collections(self, **kwargs):
         return self.client[self.dbname].list_collection_names()
 
     def get_collection(self, collection_name: str, **kwargs):
         # deal with some tables that don't use $set
         testitem = self.client[self.dbname][collection_name].find_one({})
-        if '$set' not in testitem:
-            return list(self.client[self.dbname][collection_name].find({}))
-        else:
-            return [
-                item['$set']
-                for item in self.client[self.dbname][collection_name].find({})
-            ]
+        if testitem is not None:
+            if '$set' not in testitem:
+                return list(self.client[self.dbname][collection_name].find({}))
+            else:
+                return [
+                    item['$set']
+                    for item in self.client[self.dbname][collection_name].find({})
+                ]
 
     def drop_collection(self, collection_name: str, **kwargs):
         self.client[self.dbname].drop_collection(collection_name)
 
 
 # dependency inversion
 class Database:
```

### Comparing `academicdb-0.1.1a0/src/academicdb/dbbuilder.py` & `academicdb-0.1.2/src/academicdb/dbbuilder.py`

 * *Files identical despite different names*

### Comparing `academicdb-0.1.1a0/src/academicdb/orcid.py` & `academicdb-0.1.2/src/academicdb/orcid.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,18 @@
     institution = record['organization']['name']
     city = (
         record['organization']['address']['city']
         + ', '
         + record['organization']['address']['region']
     )
     start_date = record['start-date']['year']['value']
-    end_date = record['end-date']['year']['value']
+    if record['end-date'] is not None:
+        end_date = record['end-date']['year']['value']
+    else:
+        end_date = 'present'
     degree = record['role-title']
     dept = record['department-name']
     return [institution, degree, dept, city, start_date, end_date]
 
 
 def get_orcid_funding(orcid_data):
     funding_df = pd.DataFrame(
```

### Comparing `academicdb-0.1.1a0/src/academicdb/publication.py` & `academicdb-0.1.2/src/academicdb/publication.py`

 * *Files identical despite different names*

### Comparing `academicdb-0.1.1a0/src/academicdb/publication_utils.py` & `academicdb-0.1.2/src/academicdb/publication_utils.py`

 * *Files identical despite different names*

### Comparing `academicdb-0.1.1a0/src/academicdb/query.py` & `academicdb-0.1.2/src/academicdb/query.py`

 * *Files identical despite different names*

### Comparing `academicdb-0.1.1a0/src/academicdb/recordConverter.py` & `academicdb-0.1.2/src/academicdb/recordConverter.py`

 * *Files identical despite different names*

### Comparing `academicdb-0.1.1a0/src/academicdb/render_cv.py` & `academicdb-0.1.2/src/academicdb/render_cv.py`

 * *Files 3% similar despite different names*

```diff
@@ -304,15 +304,15 @@
 def get_heading(metadata):
 
     address = ''
     for addr_line in metadata['address']:
         address += f'{addr_line}\\\\\n'
     heading = f"""
 \\reversemarginpar 
-{{\\LARGE Russell A. Poldrack}}\\\\[4mm] 
+{{\\LARGE {metadata['firstname'].capitalize()} {metadata['middlename'][0].capitalize()}. {metadata['lastname'].capitalize()}}}\\\\[4mm] 
 \\vspace{{-1cm}} 
 
 \\begin{{multicols}}{{2}} 
 {address}
 \\columnbreak 
 
 Phone: {metadata['phone']} \\\\
@@ -373,14 +373,23 @@
         )
     db = setup_db(configfile)
 
     metadata = db.get_collection('metadata')
     assert len(metadata) == 1, 'There should be only one metadata document'
     metadata = metadata[0]
 
+    parsed_twitter_handle = ""
+    for char in metadata['twitter']:
+        # handle parsing of underscores from twitter handles in latex
+        if char == "_":
+            parsed_twitter_handle += "\char`" + char
+        else:
+            parsed_twitter_handle += char
+    metadata['twitter'] = parsed_twitter_handle
+
     header = pkgutil.get_data('academicdb', 'data/latex_header.tex').decode(
         'utf-8'
     )
     footer = pkgutil.get_data('academicdb', 'data/latex_footer.tex').decode(
         'utf-8'
     )
```

### Comparing `academicdb-0.1.1a0/src/academicdb/researcher.py` & `academicdb-0.1.2/src/academicdb/researcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -352,21 +352,24 @@
                                 for aff in coauthor_info.affiliation_current
                             ]
                         self.coauthors[coauthor] = {
                             'scopus_id': coauthor,
                             'name': coauthor_info.indexed_name,
                             'affiliation': affil,
                             'affiliation_id': affil_id,
-                            'latest_year': pub['year'],
+                            'dates': [pub['publication-date']],
                             'num_pubs': 1,
                         }
                     else:
-                        if pub['year'] > self.coauthors[coauthor]['latest_year']:
-                            self.coauthors[coauthor]['latest_year'] = pub['year']
                         self.coauthors[coauthor]['num_pubs'] += 1
+                        self.coauthors[coauthor]['dates'].append(
+                            pub['publication-date']
+                        )
+                        self.coauthors[coauthor]['dates'].sort()
+
 
     def to_database(self, db: database.Database):
         """
         add this researcher record to the database
         """
         for table in database_fields:
             logging.info(f'adding {table} to database')
```

### Comparing `academicdb-0.1.1a0/src/academicdb/utils.py` & `academicdb-0.1.2/src/academicdb/utils.py`

 * *Files identical despite different names*

### Comparing `academicdb-0.1.1a0/PKG-INFO` & `academicdb-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: academicdb
-Version: 0.1.1a0
+Version: 0.1.2
 Summary: Database for an academic CV
 License: MIT
 Author: Russ Poldrack
 Author-email: poldrack@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,16 +14,18 @@
 Requires-Dist: biopython (>=1.81,<2.0)
 Requires-Dist: crossrefapi (>=1.5.0,<2.0.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: orcid (>=1.0.3,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pybliometrics (>=3.4.0,<4.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
+Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: scholarly (>=1.7.11,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ## *academicdb*: An academic database builder
 
 Why build your CV by hand when you can create it programmatically?  This package uses a set of APIs (including Scopus, ORCID, CrossRef, and Pubmed) to generate a database of academic acheivements, and provides a tool to render those into a professional-looking CV.  Perhaps more importantly, it provides a database of collaborators, which can be used to generate the notorious NSF collaborators spreadsheet. 
 
@@ -40,14 +42,20 @@
 - [Install MongoDB](https://www.mongodb.com/docs/manual/installation/) on your own system. 
 - Create a free cloud MongoDB instance [here](https://www.mongodb.com/cloud).
 
 The former is easier, but I prefer the latter because it allows the database to accessed from any system. 
 
 Rendering the CV after building the database requires that LaTeX be installed on your system and available from the command line.  There are various LaTeX distributions depending on your operating system.
 
+_Note: If you get an error that the font Tex Gyre Termes is not installed when executing `render_cv`, you can install it using Homebrew like so:_
+```{bash}
+$ brew tap homebrew/cask-fonts
+$ brew install --cask font-tex-gyre-termes
+```
+
 ### Configuring academicdb
 
 To use academicdb, you must first set up some configuration files, which will reside in `~/.academicdb`.  The most important is `config.toml`, which contains all of the details about you that are used to retrieve your information.  Here are the contents of mine as an example:
 
 ```
 [researcher]
 lastname = "poldrack"
@@ -71,32 +79,32 @@
 ]
 ```
 
 Most of this should be self-explanatory. There are several identifiers that you need to specify:
 
 - **ORCID**: This is a unique identifier for researchers.  If you don't already have an ORCID you can get one [here](http://orcid.org).  You will need to enter information about your education, employment, invited position and distinctions, and memberships and service into your ORCID account since that is where academicdb looks for that information.
 - **Google Scholar**: You will also need to retrieve your Google Scholar ID.  Once you have set up your profile, go to the "My Profile" page.  The URL from that page contains your id: for example, my URL is *https://scholar.google.com/citations?user=RbmLvDIAAAAJ&hl=en* and the ID is *RbmLvDIAAAAJ*.  
-- **Scopus**: Scopus is a service run by Elsevier.  I know that they are the bad guys, but Scopus provides a service that is not available from anywhere else: For each reference it provides a set of unique identifiers for the coauthors, which can be used to retreive their affilation information.  This is essential for generating the NSF collaborators spreadsheet.
+- **Scopus**: Scopus is a service run by Elsevier. It provides a service that is not available from anywhere else: For each reference it provides a set of unique identifiers for the coauthors, which can be used to retreive their affilation information.  This is essential for generating the NSF collaborators spreadsheet.
 
 ### cloud MongoDB setup
 
 If you are going to use a cloud MongoDB server, you will need to add the following lines to your `config.toml`:
 
 ```
 [mongo]
 CONNECT_STRING = 'mongodb+srv://<username>:<password>@<server>'
 ```
 
 The cloud provider should provide you with the connection string that you can paste into this variable.
 
 ## Obtaining an API key for Scopus
 
-  You will need to obtain an API key to access the Scopus database, which you can obtain from [http://dev.elsevier.com/myapikey.html](http://dev.elsevier.com/myapikey.html).  This is used by the [pybliometrics](https://pybliometrics.readthedocs.io/en/stable/) package to access the APIs; note that there are [weekly limits](https://dev.elsevier.com/api_key_settings.html) on the number of records one can access from these APIs without a subscription. If your institution has a subscription and you are on the institution's network, you may be able to bypass these. 
+  You will need to obtain an API key to access the Scopus database, which you can obtain from [http://dev.elsevier.com/myapikey.html](http://dev.elsevier.com/myapikey.html).  This is used by the [pybliometrics](https://pybliometrics.readthedocs.io/en/stable/) package to access the APIs. Note that this key will only work if you are on your institution's network and the institution has the appropriate license with Elsevier.  You can also request an institutional token from Elsevier if you wish to use the APIs from outside of your institution's network.
 
-  The first time you use the package, you will be asked by pybliometrics to enter your API key, which will be stored in `~/.pybliometrics/config.ini` for reuse.
+  The first time you use the package, you will be asked by pybliometrics to enter your API key (and InstToken if you have one), which will be stored in `~/.pybliometrics/config.ini` for reuse.
 
 ## specifying additional information
 
 There are a number of pieces of information that are difficult to reliably obtain from ORCID or other APIs, so they must be specified in a set of text files, which should be saved in the base directory that is specified when the command line `dbbuilder` tool is used.  See the `examples` directory for examples of each of these.
 
 - `editorial.csv`: information about editorial roles
 - `talks.csv`: information about non-conference talks at other institutions
```

