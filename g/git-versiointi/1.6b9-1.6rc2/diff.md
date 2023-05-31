# Comparing `tmp/git-versiointi-1.6b9.tar.gz` & `tmp/git-versiointi-1.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-versiointi-1.6b9.tar", last modified: Fri Jan 20 15:11:49 2023, max compression
+gzip compressed data, was "git-versiointi-1.6rc2.tar", last modified: Wed May 31 12:56:57 2023, max compression
```

## Comparing `git-versiointi-1.6b9.tar` & `git-versiointi-1.6rc2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-20 15:11:49.471157 git-versiointi-1.6b9/
--rw-r--r--   0 aha        (501) staff       (20)     6655 2023-01-20 15:11:49.471023 git-versiointi-1.6b9/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)     6306 2023-01-20 12:41:07.000000 git-versiointi-1.6b9/README.md
--rw-r--r--   0 aha        (501) staff       (20)      100 2022-06-20 07:59:54.000000 git-versiointi-1.6b9/_versiointi_setuptools_build_meta.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-20 15:11:49.468791 git-versiointi-1.6b9/git_versiointi.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)     6655 2023-01-20 15:11:49.000000 git-versiointi-1.6b9/git_versiointi.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      547 2023-01-20 15:11:49.000000 git-versiointi-1.6b9/git_versiointi.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-01-20 15:11:49.000000 git-versiointi-1.6b9/git_versiointi.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      247 2023-01-20 15:11:49.000000 git-versiointi-1.6b9/git_versiointi.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     8994 2023-01-20 15:11:33.000000 git-versiointi-1.6b9/git_versiointi.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)       25 2023-01-20 15:11:49.000000 git-versiointi-1.6b9/git_versiointi.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)       45 2023-01-20 15:11:49.000000 git-versiointi-1.6b9/git_versiointi.egg-info/top_level.txt
--rw-r--r--   0 aha        (501) staff       (20)      140 2023-01-20 14:59:29.000000 git-versiointi-1.6b9/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-01-20 15:11:49.471207 git-versiointi-1.6b9/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)     1160 2023-01-20 15:06:37.000000 git-versiointi-1.6b9/setup.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-01-20 15:11:49.470742 git-versiointi-1.6b9/versiointi/
--rw-r--r--   0 aha        (501) staff       (20)     4015 2023-01-20 15:11:25.000000 git-versiointi-1.6b9/versiointi/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      566 2022-06-08 07:34:13.000000 git-versiointi-1.6b9/versiointi/egg_info.py
--rw-r--r--   0 aha        (501) staff       (20)     5174 2023-01-20 15:11:25.000000 git-versiointi-1.6b9/versiointi/kaytanto.py
--rw-r--r--   0 aha        (501) staff       (20)     1142 2023-01-20 12:41:07.000000 git-versiointi-1.6b9/versiointi/oletus.py
--rw-r--r--   0 aha        (501) staff       (20)     1815 2022-06-08 07:34:13.000000 git-versiointi-1.6b9/versiointi/parametrit.py
--rw-r--r--   0 aha        (501) staff       (20)     5491 2023-01-20 15:11:25.000000 git-versiointi-1.6b9/versiointi/repo.py
--rw-r--r--   0 aha        (501) staff       (20)     2530 2022-06-08 07:51:15.000000 git-versiointi-1.6b9/versiointi/tiedostot.py
--rw-r--r--   0 aha        (501) staff       (20)      654 2022-06-08 07:34:13.000000 git-versiointi-1.6b9/versiointi/vaatimukset.py
--rw-r--r--   0 aha        (501) staff       (20)     3325 2023-01-20 12:41:07.000000 git-versiointi-1.6b9/versiointi/versiointi.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-31 12:56:57.461923 git-versiointi-1.6rc2/
+-rw-r--r--   0 aha        (501) staff       (20)     6656 2023-05-31 12:56:57.461802 git-versiointi-1.6rc2/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)     6306 2023-01-20 12:41:07.000000 git-versiointi-1.6rc2/README.md
+-rw-r--r--   0 aha        (501) staff       (20)      100 2022-06-20 07:59:54.000000 git-versiointi-1.6rc2/_versiointi_setuptools_build_meta.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-31 12:56:57.459659 git-versiointi-1.6rc2/git_versiointi.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)     6656 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      509 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      247 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)       25 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)       45 2023-05-31 12:56:57.000000 git-versiointi-1.6rc2/git_versiointi.egg-info/top_level.txt
+-rw-r--r--   0 aha        (501) staff       (20)      140 2023-05-15 12:45:13.000000 git-versiointi-1.6rc2/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-05-31 12:56:57.461959 git-versiointi-1.6rc2/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)     1143 2023-05-15 12:45:03.000000 git-versiointi-1.6rc2/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-31 12:56:57.461524 git-versiointi-1.6rc2/versiointi/
+-rw-r--r--   0 aha        (501) staff       (20)     5262 2023-05-15 13:01:31.000000 git-versiointi-1.6rc2/versiointi/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      566 2022-06-08 07:34:13.000000 git-versiointi-1.6rc2/versiointi/egg_info.py
+-rw-r--r--   0 aha        (501) staff       (20)     5174 2023-01-20 15:11:25.000000 git-versiointi-1.6rc2/versiointi/kaytanto.py
+-rw-r--r--   0 aha        (501) staff       (20)     1051 2023-05-31 12:55:13.000000 git-versiointi-1.6rc2/versiointi/oletus.py
+-rw-r--r--   0 aha        (501) staff       (20)     1815 2022-06-08 07:34:13.000000 git-versiointi-1.6rc2/versiointi/parametrit.py
+-rw-r--r--   0 aha        (501) staff       (20)     5491 2023-01-20 15:11:25.000000 git-versiointi-1.6rc2/versiointi/repo.py
+-rw-r--r--   0 aha        (501) staff       (20)     2530 2022-06-08 07:51:15.000000 git-versiointi-1.6rc2/versiointi/tiedostot.py
+-rw-r--r--   0 aha        (501) staff       (20)      654 2022-06-08 07:34:13.000000 git-versiointi-1.6rc2/versiointi/vaatimukset.py
+-rw-r--r--   0 aha        (501) staff       (20)     3325 2023-01-20 12:41:07.000000 git-versiointi-1.6rc2/versiointi/versiointi.py
```

### Comparing `git-versiointi-1.6b9/PKG-INFO` & `git-versiointi-1.6rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-versiointi
-Version: 1.6b9
+Version: 1.6rc2
 Summary: Asennettavan pakettiversion haku git-leimojen mukaan
 Home-page: https://github.com/an7oine/git-versiointi.git
 Author: Antti Hautaniemi
 Author-email: antti.hautaniemi@pispalanit.fi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `git-versiointi-1.6b9/README.md` & `git-versiointi-1.6rc2/README.md`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6b9/git_versiointi.egg-info/PKG-INFO` & `git-versiointi-1.6rc2/git_versiointi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-versiointi
-Version: 1.6b9
+Version: 1.6rc2
 Summary: Asennettavan pakettiversion haku git-leimojen mukaan
 Home-page: https://github.com/an7oine/git-versiointi.git
 Author: Antti Hautaniemi
 Author-email: antti.hautaniemi@pispalanit.fi
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `git-versiointi-1.6b9/setup.py` & `git-versiointi-1.6rc2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from versiointi import _versionumero
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(
   name='git-versiointi',
-  version=_versionumero(os.path.dirname(__file__)),
+  version=_versionumero(__file__),
   description='Asennettavan pakettiversion haku git-leimojen mukaan',
   long_description=long_description,
   long_description_content_type='text/markdown',
   url='https://github.com/an7oine/git-versiointi.git',
   author='Antti Hautaniemi',
   author_email='antti.hautaniemi@pispalanit.fi',
   licence='MIT',
@@ -30,9 +30,9 @@
     'setuptools.finalize_distribution_options': [
       'versiointi = versiointi:finalize_distribution_options',
     ]
   },
   classifiers=[
     'Programming Language :: Python :: 3',
   ],
-  install_requires=['GitPython', 'setuptools>=42'],
+  install_requires=['GitPython', 'setuptools>=63'],
 )
```

### Comparing `git-versiointi-1.6b9/versiointi/__init__.py` & `git-versiointi-1.6rc2/versiointi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,74 +37,122 @@
   requirements = asennusvaatimukset(setup_py)
   return {
     **({'install_requires': requirements} if requirements else {})
   }
   # def asennustiedot
 
 
+def _versiointi(setup_py):
+  ''' Muodosta versiointiolio setup.py-tiedoston sijainnin mukaan. '''
+  from .versiointi import Versiointi
+
+  # Poimi setup.py-tiedoston hakemisto.
+  polku = os.path.dirname(setup_py)
+
+  # Lataa oletusparametrit `setup.cfg`-tiedostosta, jos on.
+  parametrit = configparser.ConfigParser()
+  parametrit.read(os.path.join(polku, 'setup.cfg'))
+
+  # Palauta versiointiolio.
+  return Versiointi(
+    polku,
+    kaytanto=(
+      parametrit['versiointi']
+      if 'versiointi' in parametrit
+      else VERSIOKAYTANTO
+    )
+  )
+  # def _versiointi
+
+
+def _poimi_sdist_versio(setup_py):
+  ''' Poimi `sdist`-pakettiin tallennettu versionumero. '''
+  with open(os.path.join(
+    os.path.dirname(setup_py),
+    'PKG-INFO'
+  )) as pkg_info:
+    for rivi in pkg_info:
+      tulos = PKG_INFO_VERSIO.match(rivi)
+      if tulos:
+        return tulos.group(1)
+  return None
+  # def _poimi_sdist_versio
+
+
 def _versionumero(setup_py):
   ''' Sisäinen käyttö: palauta pelkkä versionumero. '''
-  dist = Distribution()
   try:
-    tarkista_git_versiointi(dist, 'git_versiointi', setup_py)
-    return dist.git_versiointi.versionumero(ref=dist.git_ref)
-  except:
-    return None
+    dist = Distribution(attrs={'git_versiointi': setup_py})
+  except DistutilsSetupError:
+    return _poimi_sdist_versio(setup_py)
+  else:
+    return _versiointi(setup_py).versionumero(ref=dist.git_ref)
   # def _versionumero
 
 
 def tarkista_git_versiointi(dist, attr, value):
-  ''' Hae Git-tietovarasto määritetyn setup.py-tiedoston polusta. '''
+  '''
+  Sisääntulopiste setup-komentosarjalle silloin, kun parametri
+  `setup_requires='git-versiointi'` on määritetty.
+
+  Huomaa, että `attr` on aina `git_versiointi`. Arvo
+  `value` on git-jakelun juurihakemisto.
+
+  Versiointiolio muodostetaan git-tietojen perusteella ja
+  asetetaan `dist.git_versiointi`-määreeseen.
+  '''
   # pylint: disable=unused-argument, protected-access
   from .versiointi import Versiointi
 
   if isinstance(value, Versiointi):
     # Hyväksytään aiemmin asetettu versiointiolio (tupla-ajo).
-    return
+    dist.git_versiointi = value
   elif not isinstance(value, str):
     raise DistutilsSetupError(
       f'virheellinen parametri: {attr}={value!r}'
     )
-
-  # Poimi setup.py-tiedoston hakemisto.
-  polku = os.path.dirname(value)
-
-  # Lataa oletusparametrit `setup.cfg`-tiedostosta, jos on.
-  parametrit = configparser.ConfigParser()
-  parametrit.read(os.path.join(polku, 'setup.cfg'))
-
-  # Alusta versiointiolio ja aseta se jakelun tietoihin.
-  try:
-    dist.git_versiointi = Versiointi(
-      polku,
-      kaytanto=(
-        parametrit['versiointi']
-        if 'versiointi' in parametrit
-        else VERSIOKAYTANTO
+  else:
+    # Alusta versiointiolio ja aseta se jakelun tietoihin.
+    try:
+      dist.git_versiointi = _versiointi(value)
+    except ValueError:
+      raise DistutilsSetupError(
+        f'git-tietovarastoa ei löydy hakemistosta {value!r}'
       )
-    )
-  except ValueError:
-    raise DistutilsSetupError(
-      f'git-tietovarastoa ei löydy hakemistosta {polku!r}'
-    )
-    # except ValueError
-
+  return value
   # def tarkista_git_versiointi
 
 
 def finalize_distribution_options(dist):
+  '''
+  Viimeistelyfunktio jakelun tietojen asettamisen jälkeen.
+
+  – Puukotetaan setuptools-jakelun tyyppi, jotta voidaan käyttää
+  tämän paketin tarjoamia laajennettuja komentoriviparametrejä.
+  – Asetetaan paketin versionumero ja -historia git-tietovaraston
+    mukaisesti.
+  – Tallennetaan versiointiolio tiedostokohtaista versiointia varten.
+  – Viimekätisenä ratkaisuna (git-tietovarastoa ei löytynyt)
+    poimitaan pelkkä versionumero `sdist`-jakelun metatiedoista.
+  '''
   # pylint: disable=protected-access
+  from .versiointi import Versiointi
+
   if dist.version != 0:
     return
-  elif getattr(dist, 'git_versiointi', None) is not None:
+
+  asetettu_versiointi = getattr(dist, 'git_versiointi', None)
+  if isinstance(asetettu_versiointi, Versiointi):
     pass
   else:
     try:
-      tarkista_git_versiointi(dist, 'git_versiointi', sys.argv[0])
-    except (ModuleNotFoundError, DistutilsSetupError):
+      dist.git_versiointi = _versiointi(
+        asetettu_versiointi or sys.argv[0]
+      )
+    except:
       dist.git_versiointi = None
 
   # Aseta jakelun tyyppi; tarvitaan komentoriviparametrien lisäämiseksi.
   dist.__class__ = Distribution
 
   if dist.git_versiointi is not None:
     # Aseta versionumero ja historia Git-tietojen perusteella.
@@ -113,23 +161,17 @@
 
     # Aseta versiointi tiedostokohtaisen versioinnin määreeksi.
     _build_py.build_py.git_versiointi = dist.git_versiointi
 
   else:
     # Yritetään hakea versiotieto `sdist`-tyyppisen paketin PKG-INFOsta.
     try:
-      with open(os.path.join(
-        os.path.dirname(sys.argv[0]),
-        'PKG-INFO'
-      )) as pkg_info:
-        for rivi in pkg_info:
-          tulos = PKG_INFO_VERSIO.match(rivi)
-          if tulos:
-            dist.metadata.version = tulos.group(1)
-            break
+      dist.metadata.version = _poimi_sdist_versio(
+        sys.argv[0],
+      )
     except FileNotFoundError:
       pass
     # else (dist.git_versiointi is None)
 
   # def finalize_distribution_options
```

### Comparing `git-versiointi-1.6b9/versiointi/egg_info.py` & `git-versiointi-1.6rc2/versiointi/egg_info.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6b9/versiointi/kaytanto.py` & `git-versiointi-1.6rc2/versiointi/kaytanto.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6b9/versiointi/oletus.py` & `git-versiointi-1.6rc2/versiointi/oletus.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,31 @@
   # pylint: disable=line-too-long
 
   # Irtoversio (nk. detached HEAD).
   '*': '''{pohja}+{etaisyys}''',
 
   # (Muun kuin master-) haaran versio:
   # indeksoitu kehitysversio tai haaran mukainen tunniste.
-  'refs/heads/ refs/remotes/origin/': \
-    '''{pohja}{int(indeksi)+etaisyys if indeksi else f'+{tunnus}.{etaisyys}'}''',
+  'refs/heads/ refs/remotes/origin/': (
+    '''{pohja}{int(indeksi)+etaisyys if indeksi else f'+{tunnus}.{etaisyys}'}'''
+  ),
 
-    # Versiohaaran (v-1.2) versio:
+  # Master-haara tai versiohaara (v-X.Y):
   # indeksoitu kehitysversio tai etäisyyden mukainen pääte.
-  'refs/heads/v-[0-9].* refs/remotes/origin/v-[0-9].*': \
-    '''{pohja}{int(indeksi)+etaisyys if indeksi else f'.{etaisyys}'}''',
-
-  # Master-haaran versio:
-  # indeksoitu kehitysversio tai etäisyyden mukainen pääte.
-  'refs/heads/master refs/remotes/origin/master': \
-    '''{pohja}{int(indeksi)+etaisyys if indeksi else f'.{etaisyys}'}''',
+  ' '.join((
+    'refs/heads/master',
+    'refs/remotes/origin/master',
+    'refs/heads/v-[0-9].*',
+    'refs/remotes/origin/v-[0-9].*',
+  )): (
+    '''{pohja}{int(indeksi)+etaisyys if indeksi else f'.{etaisyys}'}'''
+  ),
 
   # Leimattu kehitysversiosarja: tulkitaan viimeinen luku indeksinä.
-  'refs/tags/v[0-9].*': '''{tunnus}{indeksoitu}''',
+  'refs/tags/v[0-9].*': '''{tunnus[1:]}{indeksoitu}''',
 
-  # Leimattu versio: käytetään sellaisenaan.
-  'refs/tags/v[0-9][0-9.]*?(?![a-z]+[0-9]*)': '''{tunnus}''',
+  # Leimattu (ei-kehitys-) versio: käytetään sellaisenaan.
+  'refs/tags/v[0-9][0-9.]*?(?![a-z]+[0-9]*)': '''{tunnus[1:]}''',
 
   # Nollaversio (edeltää ensimmäistä leimaa).
   '0': '0.0',
 }
```

### Comparing `git-versiointi-1.6b9/versiointi/parametrit.py` & `git-versiointi-1.6rc2/versiointi/parametrit.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6b9/versiointi/repo.py` & `git-versiointi-1.6rc2/versiointi/repo.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6b9/versiointi/tiedostot.py` & `git-versiointi-1.6rc2/versiointi/tiedostot.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6b9/versiointi/vaatimukset.py` & `git-versiointi-1.6rc2/versiointi/vaatimukset.py`

 * *Files identical despite different names*

### Comparing `git-versiointi-1.6b9/versiointi/versiointi.py` & `git-versiointi-1.6rc2/versiointi/versiointi.py`

 * *Files identical despite different names*

