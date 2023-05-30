# Comparing `tmp/polyswarm-3.2.0.tar.gz` & `tmp/polyswarm-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyswarm-3.2.0.tar", last modified: Tue Mar 21 20:15:25 2023, max compression
+gzip compressed data, was "polyswarm-3.2.1.tar", last modified: Tue May 30 22:09:01 2023, max compression
```

## Comparing `polyswarm-3.2.0.tar` & `polyswarm-3.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:15:25.878822 polyswarm-3.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-03-21 20:15:03.000000 polyswarm-3.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2804 2023-03-21 20:15:25.878822 polyswarm-3.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-03-21 20:15:03.000000 polyswarm-3.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-21 20:15:25.878822 polyswarm-3.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-03-21 20:15:03.000000 polyswarm-3.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:15:25.874822 polyswarm-3.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:15:25.874822 polyswarm-3.2.0/src/polyswarm/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:15:25.878822 polyswarm-3.2.0/src/polyswarm/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/download.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/engine.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/families.py
--rw-rw-rw-   0 root         (0) root         (0)     4528 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/historical.py
--rw-rw-rw-   0 root         (0) root         (0)     2430 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/links.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/live.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6130 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/polyswarm.py
--rw-rw-rw-   0 root         (0) root         (0)     2163 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/rules.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/sandbox.py
--rw-rw-rw-   0 root         (0) root         (0)     6349 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/scan.py
--rw-rw-rw-   0 root         (0) root         (0)     5883 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/search.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/tags.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/client/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:15:25.878822 polyswarm-3.2.0/src/polyswarm/formatters/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/formatters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/formatters/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2153 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/formatters/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     5528 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/formatters/json.py
--rw-rw-rw-   0 root         (0) root         (0)    22328 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/formatters/text.py
--rw-rw-rw-   0 root         (0) root         (0)     9994 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/polyswarm.py
--rw-rw-rw-   0 root         (0) root         (0)     3760 2023-03-21 20:15:03.000000 polyswarm-3.2.0/src/polyswarm/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:15:25.874822 polyswarm-3.2.0/src/polyswarm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2804 2023-03-21 20:15:25.000000 polyswarm-3.2.0/src/polyswarm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1023 2023-03-21 20:15:25.000000 polyswarm-3.2.0/src/polyswarm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 20:15:25.000000 polyswarm-3.2.0/src/polyswarm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-21 20:15:25.000000 polyswarm-3.2.0/src/polyswarm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-03-21 20:15:25.000000 polyswarm-3.2.0/src/polyswarm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-21 20:15:25.000000 polyswarm-3.2.0/src/polyswarm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.136853 polyswarm-3.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-30 22:08:39.000000 polyswarm-3.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-30 22:09:01.136853 polyswarm-3.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-05-30 22:08:39.000000 polyswarm-3.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 22:09:01.136853 polyswarm-3.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-05-30 22:08:39.000000 polyswarm-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.132853 polyswarm-3.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.132853 polyswarm-3.2.1/src/polyswarm/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.136853 polyswarm-3.2.1/src/polyswarm/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/families.py
+-rw-rw-rw-   0 root         (0) root         (0)     4528 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/historical.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/live.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/polyswarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2163 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/sandbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     6349 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     5916 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.136853 polyswarm-3.2.1/src/polyswarm/formatters/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1276 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2153 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     5618 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    22994 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     9994 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/polyswarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3760 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.132853 polyswarm-3.2.1/src/polyswarm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/top_level.txt
```

### Comparing `polyswarm-3.2.0/LICENSE` & `polyswarm-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/PKG-INFO` & `polyswarm-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm
-Version: 3.2.0
+Version: 3.2.1
 Summary: CLI for using the PolySwarm Customer APIs
 Home-page: https://github.com/polyswarm/polyswarm-cli
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `polyswarm-3.2.0/README.md` & `polyswarm-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/setup.py` & `polyswarm-3.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The README.md will be used as the content for the PyPi package details page on the Python Package Index.
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 
 setup(
     name='polyswarm',
-    version='3.2.0',
+    version='3.2.1',
     description='CLI for using the PolySwarm Customer APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='PolySwarm Developers',
     author_email='info@polyswarm.io',
     url='https://github.com/polyswarm/polyswarm-cli',
     license='MIT',
```

### Comparing `polyswarm-3.2.0/src/polyswarm/__main__.py` & `polyswarm-3.2.1/src/polyswarm/__main__.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/download.py` & `polyswarm-3.2.1/src/polyswarm/client/download.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/engine.py` & `polyswarm-3.2.1/src/polyswarm/client/engine.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/families.py` & `polyswarm-3.2.1/src/polyswarm/client/families.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/historical.py` & `polyswarm-3.2.1/src/polyswarm/client/historical.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/links.py` & `polyswarm-3.2.1/src/polyswarm/client/links.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/live.py` & `polyswarm-3.2.1/src/polyswarm/client/live.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/metadata.py` & `polyswarm-3.2.1/src/polyswarm/client/metadata.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/polyswarm.py` & `polyswarm-3.2.1/src/polyswarm/client/polyswarm.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/rules.py` & `polyswarm-3.2.1/src/polyswarm/client/rules.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/sandbox.py` & `polyswarm-3.2.1/src/polyswarm/client/sandbox.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/scan.py` & `polyswarm-3.2.1/src/polyswarm/client/scan.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/search.py` & `polyswarm-3.2.1/src/polyswarm/client/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,16 @@
         params['domain'] = value
     elif type == 'ttp':
         params['ttp'] = value
     elif type == 'imphash':
         params['imphash'] = value
 
     if params:
-        output.iocs(api.search_by_ioc(**params))
+        for result in api.search_by_ioc(**params):
+            output.ioc(result)
     else:
         output.iocs(api.iocs_by_hash(type, value, hide_known_good=hide_known_good))
 
 
 @search.command('known', short_help='Check if host is known.')
 @click.option('-p', '--ip', type=click.STRING, multiple=True)
 @click.option('-d', '--domain', type=click.STRING, multiple=True)
```

### Comparing `polyswarm-3.2.0/src/polyswarm/client/tags.py` & `polyswarm-3.2.1/src/polyswarm/client/tags.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/client/utils.py` & `polyswarm-3.2.1/src/polyswarm/client/utils.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/formatters/base.py` & `polyswarm-3.2.1/src/polyswarm/formatters/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         raise NotImplementedError
 
     def ruleset(self, result, contents=False):
         raise NotImplementedError
 
     def iocs(self, iocs, write=True):
         raise NotImplementedError
+    
+    def ioc(self, iocs, write=True):
+        raise NotImplementedError
 
     def known_host(self, iocs, write=True):
         raise NotImplementedError
 
     def metadata(self, result):
         raise NotImplementedError
```

### Comparing `polyswarm-3.2.0/src/polyswarm/formatters/hashes.py` & `polyswarm-3.2.1/src/polyswarm/formatters/hashes.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/formatters/json.py` & `polyswarm-3.2.1/src/polyswarm/formatters/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,17 @@
 
     def votes(self, result):
         click.echo(self._to_json(result.json), file=self.out)
 
     def iocs(self, results):
         click.echo(self._to_json([result.json for result in results]), file=self.out)
 
+    def ioc(self, result):
+        click.echo(self._to_json(result.json), file=self.out)
+
     def known_host(self, result):
         click.echo(self._to_json(result.json), file=self.out)
 
     def artifact_metadata(self, result, only=None):
         click.echo(self._to_json(result.json), file=self.out)
 
     def sandbox_list(self, result):
```

### Comparing `polyswarm-3.2.0/src/polyswarm/formatters/text.py` & `polyswarm-3.2.1/src/polyswarm/formatters/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,14 +290,27 @@
                 output.append(self._white('IPs: {}'.format(", ".join(data['ips']))))
                 output.append(self._white('URLs: {}'.format(", ".join(data['urls']))))
                 output.append(self._white('TTPs: {}'.format(", ".join(data['ttps']))))
             else:
                 output.append(self._white('SHA256: {}'.format(data)))
         return self._output(output, write)
     
+    def ioc(self, ioc, write=True):
+        output = []
+        output.append(self._white('============================= IOC ============================='))
+        data = ioc.json
+        if type(data) is dict:
+            output.append(self._white('ImpHash: {}'.format(data['imphash'])))
+            output.append(self._white('IPs: {}'.format(", ".join(data['ips']))))
+            output.append(self._white('URLs: {}'.format(", ".join(data['urls']))))
+            output.append(self._white('TTPs: {}'.format(", ".join(data['ttps']))))
+        else:
+            output.append(self._white('SHA256: {}'.format(data)))
+        return self._output(output, write)
+    
     def known_host(self, ioc_known, write=True):
         output = []
         output.append(self._white('============================= Known IOC ============================='))
         output.append(self._white('ID: {}'.format(ioc_known.json['id'])))
         output.append(self._white('type: {}'.format(ioc_known.json['type'])))
         output.append(self._white('host: {}'.format(ioc_known.json['host'])))
         output.append(self._white('source: {}'.format(ioc_known.json['source'])))
```

### Comparing `polyswarm-3.2.0/src/polyswarm/polyswarm.py` & `polyswarm-3.2.1/src/polyswarm/polyswarm.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm/utils.py` & `polyswarm-3.2.1/src/polyswarm/utils.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.0/src/polyswarm.egg-info/PKG-INFO` & `polyswarm-3.2.1/src/polyswarm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm
-Version: 3.2.0
+Version: 3.2.1
 Summary: CLI for using the PolySwarm Customer APIs
 Home-page: https://github.com/polyswarm/polyswarm-cli
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `polyswarm-3.2.0/src/polyswarm.egg-info/SOURCES.txt` & `polyswarm-3.2.1/src/polyswarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

