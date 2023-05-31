# Comparing `tmp/pyone-6.6.1.tar.gz` & `tmp/pyone-6.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyone-6.6.1.tar", last modified: Tue Mar  7 10:35:46 2023, max compression
+gzip compressed data, was "pyone-6.6.2.tar", last modified: Tue May 30 17:18:23 2023, max compression
```

## Comparing `pyone-6.6.1.tar` & `pyone-6.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-03-07 10:35:46.078187 pyone-6.6.1/
--rw-rw-r--   0 one       (1001) one       (1001)      889 2023-03-07 10:35:46.078187 pyone-6.6.1/PKG-INFO
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-03-07 10:35:46.070187 pyone-6.6.1/pyone/
--rw-r--r--   0 one       (1001) one       (1001)    11256 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/__init__.py
--rw-r--r--   0 one       (1001) one       (1001)     5898 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/acl.py
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-03-07 10:35:46.070187 pyone-6.6.1/pyone/bindings/
--rw-rw-r--   0 one       (1001) one       (1001)   115076 2023-03-07 10:35:44.000000 pyone-6.6.1/pyone/bindings/__init__.py
--rw-rw-r--   0 one       (1001) one       (1001)  2624697 2023-03-07 10:35:44.000000 pyone-6.6.1/pyone/bindings/supbind.py
--rw-r--r--   0 one       (1001) one       (1001)     3278 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/helpers.py
--rw-r--r--   0 one       (1001) one       (1001)      929 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/server.py
--rw-r--r--   0 one       (1001) one       (1001)     7039 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/tester.py
--rw-r--r--   0 one       (1001) one       (1001)     5023 2023-03-07 10:22:11.000000 pyone-6.6.1/pyone/util.py
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-03-07 10:35:46.070187 pyone-6.6.1/pyone.egg-info/
--rw-rw-r--   0 one       (1001) one       (1001)      889 2023-03-07 10:35:45.000000 pyone-6.6.1/pyone.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1001) one       (1001)      299 2023-03-07 10:35:46.000000 pyone-6.6.1/pyone.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1001) one       (1001)        1 2023-03-07 10:35:45.000000 pyone-6.6.1/pyone.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1001) one       (1001)       89 2023-03-07 10:35:45.000000 pyone-6.6.1/pyone.egg-info/requires.txt
--rw-rw-r--   0 one       (1001) one       (1001)        6 2023-03-07 10:35:45.000000 pyone-6.6.1/pyone.egg-info/top_level.txt
--rw-rw-r--   0 one       (1001) one       (1001)       38 2023-03-07 10:35:46.078187 pyone-6.6.1/setup.cfg
--rw-r--r--   0 one       (1001) one       (1001)     2495 2023-03-07 10:22:11.000000 pyone-6.6.1/setup.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-05-30 17:18:23.854967 pyone-6.6.2/
+-rw-rw-r--   0 one       (1001) one       (1001)      889 2023-05-30 17:18:23.854967 pyone-6.6.2/PKG-INFO
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-05-30 17:18:23.850967 pyone-6.6.2/pyone/
+-rw-r--r--   0 one       (1001) one       (1001)    11256 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/__init__.py
+-rw-r--r--   0 one       (1001) one       (1001)     5898 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/acl.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-05-30 17:18:23.850967 pyone-6.6.2/pyone/bindings/
+-rw-rw-r--   0 one       (1001) one       (1001)   115076 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone/bindings/__init__.py
+-rw-rw-r--   0 one       (1001) one       (1001)  2625409 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone/bindings/supbind.py
+-rw-r--r--   0 one       (1001) one       (1001)     3278 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/helpers.py
+-rw-r--r--   0 one       (1001) one       (1001)      929 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/server.py
+-rw-r--r--   0 one       (1001) one       (1001)     7039 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/tester.py
+-rw-r--r--   0 one       (1001) one       (1001)     5023 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/util.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-05-30 17:18:23.850967 pyone-6.6.2/pyone.egg-info/
+-rw-rw-r--   0 one       (1001) one       (1001)      889 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1001) one       (1001)      299 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1001) one       (1001)        1 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1001) one       (1001)       89 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/requires.txt
+-rw-rw-r--   0 one       (1001) one       (1001)        6 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/top_level.txt
+-rw-rw-r--   0 one       (1001) one       (1001)       38 2023-05-30 17:18:23.854967 pyone-6.6.2/setup.cfg
+-rw-r--r--   0 one       (1001) one       (1001)     2495 2023-05-30 17:01:42.000000 pyone-6.6.2/setup.py
```

### Comparing `pyone-6.6.1/PKG-INFO` & `pyone-6.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyone
-Version: 6.6.1
+Version: 6.6.2
 Summary: Python Bindings for OpenNebula XML-RPC API
 Home-page: http://opennebula.io
 Author: Rafael del Valle
 Author-email: rvalle@privaz.io
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: PyOne is an implementation of OpenNebula XML-RPC
                 bindings in Python. It works as a proxy over the XML-RPC api and
```

### Comparing `pyone-6.6.1/pyone/__init__.py` & `pyone-6.6.2/pyone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.1/pyone/acl.py` & `pyone-6.6.2/pyone/acl.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.1/pyone/bindings/__init__.py` & `pyone-6.6.2/pyone/bindings/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 
 #
-# Generated Tue Mar  7 10:35:44 2023 by generateDS.py version 2.41.3.
-# Python 3.8.10 (default, Nov 14 2022, 12:59:47)  [GCC 9.4.0]
+# Generated Tue May 30 17:18:23 2023 by generateDS.py version 2.41.5.
+# Python 3.8.10 (default, Mar 13 2023, 10:26:41)  [GCC 9.4.0]
 #
 # Command line options:
 #   ('-q', '')
 #   ('-f', '')
 #   ('-o', 'pyone/bindings/supbind.py')
 #   ('-s', 'pyone/bindings/__init__.py')
 #   ('--super', 'supbind')
 #   ('--external-encoding', 'utf-8')
 #   ('--silence', '')
 #
 # Command line arguments:
 #   ../../../share/doc/xsd/index.xsd
 #
 # Command line:
-#   /home/one/init-build-jenkins.T9TFrJ/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
+#   /home/one/init-build-jenkins.bmbySM/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
 #
 # Current working directory (os.getcwd()):
 #   python
 #
 
 import os
 import sys
```

### Comparing `pyone-6.6.1/pyone/bindings/supbind.py` & `pyone-6.6.2/pyone/bindings/supbind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Tue Mar  7 10:35:44 2023 by generateDS.py version 2.41.3.
-# Python 3.8.10 (default, Nov 14 2022, 12:59:47)  [GCC 9.4.0]
+# Generated Tue May 30 17:18:23 2023 by generateDS.py version 2.41.5.
+# Python 3.8.10 (default, Mar 13 2023, 10:26:41)  [GCC 9.4.0]
 #
 # Command line options:
 #   ('-q', '')
 #   ('-f', '')
 #   ('-o', 'pyone/bindings/supbind.py')
 #   ('-s', 'pyone/bindings/__init__.py')
 #   ('--super', 'supbind')
 #   ('--external-encoding', 'utf-8')
 #   ('--silence', '')
 #
 # Command line arguments:
 #   ../../../share/doc/xsd/index.xsd
 #
 # Command line:
-#   /home/one/init-build-jenkins.T9TFrJ/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
+#   /home/one/init-build-jenkins.bmbySM/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
 #
 # Current working directory (os.getcwd()):
 #   python
 #
 
 import sys
 try:
@@ -259,15 +259,19 @@
             for value in values:
                 try:
                     int(value)
                 except (TypeError, ValueError):
                     raise_parse_error(node, 'Requires sequence of integer values')
             return values
         def gds_format_float(self, input_data, input_name=''):
-            return ('%.15f' % float(input_data)).rstrip('0')
+            value = ('%.15f' % float(input_data)).rstrip('0')
+            if value.endswith('.'):
+                value += '0'
+            return value
+    
         def gds_parse_float(self, input_data, node=None, input_name=''):
             try:
                 fval_ = float(input_data)
             except (TypeError, ValueError) as exp:
                 raise_parse_error(node, 'Requires float or double value: %s' % exp)
             return fval_
         def gds_validate_float(self, input_data, node=None, input_name=''):
@@ -1059,15 +1063,15 @@
         self.HISTORY = HISTORY
     def add_HISTORY(self, value):
         self.HISTORY.append(value)
     def insert_HISTORY_at(self, index, value):
         self.HISTORY.insert(index, value)
     def replace_HISTORY_at(self, index, value):
         self.HISTORY[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HISTORY
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORY_RECORDS', pretty_print=True):
@@ -1082,15 +1086,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORY_RECORDS')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORY_RECORDS', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORY_RECORDS'):
@@ -1272,15 +1276,15 @@
         return self.REQUEST_ID
     def set_REQUEST_ID(self, REQUEST_ID):
         self.REQUEST_ID = REQUEST_ID
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OID is not None or
             self.SEQ is not None or
             self.HOSTNAME is not None or
             self.HID is not None or
             self.CID is not None or
             self.STIME is not None or
@@ -1315,15 +1319,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORY')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORY', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORY'):
@@ -1594,15 +1598,15 @@
         self.ACL = ACL
     def add_ACL(self, value):
         self.ACL.append(value)
     def insert_ACL_at(self, index, value):
         self.ACL.insert(index, value)
     def replace_ACL_at(self, index, value):
         self.ACL[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ACL
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ACL_POOL', pretty_print=True):
@@ -1617,15 +1621,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ACL_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ACL_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ACL_POOL'):
@@ -1699,15 +1703,15 @@
         return self.PARAMETERS
     def set_PARAMETERS(self, PARAMETERS):
         self.PARAMETERS = PARAMETERS
     def get_EXTRA(self):
         return self.EXTRA
     def set_EXTRA(self, EXTRA):
         self.EXTRA = EXTRA
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.RESULT is not None or
             self.PARAMETERS is not None or
             self.EXTRA is not None
         ):
             return True
         else:
@@ -1724,15 +1728,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CALL_INFO')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CALL_INFO', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CALL_INFO'):
@@ -1821,15 +1825,15 @@
         self.CLUSTER = CLUSTER
     def add_CLUSTER(self, value):
         self.CLUSTER.append(value)
     def insert_CLUSTER_at(self, index, value):
         self.CLUSTER.insert(index, value)
     def replace_CLUSTER_at(self, index, value):
         self.CLUSTER[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CLUSTER
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTER_POOL', pretty_print=True):
@@ -1844,15 +1848,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTER_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTER_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTER_POOL'):
@@ -1944,15 +1948,15 @@
         return self.VNETS
     def set_VNETS(self, VNETS):
         self.VNETS = VNETS
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.NAME is not None or
             self.HOSTS is not None or
             self.DATASTORES is not None or
             self.VNETS is not None or
             self.TEMPLATE is not None
@@ -1972,15 +1976,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTER')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTER', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTER'):
@@ -2097,15 +2101,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_POOL', pretty_print=True):
@@ -2120,15 +2124,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_POOL'):
@@ -2298,15 +2302,15 @@
         return self.IMAGES
     def set_IMAGES(self, IMAGES):
         self.IMAGES = IMAGES
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -2339,15 +2343,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE'):
@@ -2592,15 +2596,15 @@
         self.DOCUMENT = DOCUMENT
     def add_DOCUMENT(self, value):
         self.DOCUMENT.append(value)
     def insert_DOCUMENT_at(self, index, value):
         self.DOCUMENT.insert(index, value)
     def replace_DOCUMENT_at(self, index, value):
         self.DOCUMENT[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DOCUMENT
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DOCUMENT_POOL', pretty_print=True):
@@ -2615,15 +2619,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DOCUMENT_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DOCUMENT_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DOCUMENT_POOL'):
@@ -2739,15 +2743,15 @@
         return self.LOCK
     def set_LOCK(self, LOCK):
         self.LOCK = LOCK
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -2771,15 +2775,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DOCUMENT')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DOCUMENT', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DOCUMENT'):
@@ -2959,15 +2963,15 @@
         self.QUOTAS.insert(index, value)
     def replace_QUOTAS_at(self, index, value):
         self.QUOTAS[index] = value
     def get_DEFAULT_GROUP_QUOTAS(self):
         return self.DEFAULT_GROUP_QUOTAS
     def set_DEFAULT_GROUP_QUOTAS(self, DEFAULT_GROUP_QUOTAS):
         self.DEFAULT_GROUP_QUOTAS = DEFAULT_GROUP_QUOTAS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.GROUP or
             self.QUOTAS or
             self.DEFAULT_GROUP_QUOTAS is not None
         ):
             return True
         else:
@@ -2984,15 +2988,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUP_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUP_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUP_POOL'):
@@ -3124,15 +3128,15 @@
         return self.IMAGE_QUOTA
     def set_IMAGE_QUOTA(self, IMAGE_QUOTA):
         self.IMAGE_QUOTA = IMAGE_QUOTA
     def get_DEFAULT_GROUP_QUOTAS(self):
         return self.DEFAULT_GROUP_QUOTAS
     def set_DEFAULT_GROUP_QUOTAS(self, DEFAULT_GROUP_QUOTAS):
         self.DEFAULT_GROUP_QUOTAS = DEFAULT_GROUP_QUOTAS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.NAME is not None or
             self.TEMPLATE is not None or
             self.USERS is not None or
             self.ADMINS is not None or
             self.DATASTORE_QUOTA is not None or
@@ -3156,15 +3160,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUP')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUP', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUP'):
@@ -3325,15 +3329,15 @@
         self.CALL_INFO = CALL_INFO
     def add_CALL_INFO(self, value):
         self.CALL_INFO.append(value)
     def insert_CALL_INFO_at(self, index, value):
         self.CALL_INFO.insert(index, value)
     def replace_CALL_INFO_at(self, index, value):
         self.CALL_INFO[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HOOK_TYPE is not None or
             self.CALL is not None or
             self.CALL_INFO
         ):
             return True
         else:
@@ -3350,15 +3354,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOOK_MESSAGE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOOK_MESSAGE', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOOK_MESSAGE'):
@@ -3449,15 +3453,15 @@
         self.HOOK = HOOK
     def add_HOOK(self, value):
         self.HOOK.append(value)
     def insert_HOOK_at(self, index, value):
         self.HOOK.insert(index, value)
     def replace_HOOK_at(self, index, value):
         self.HOOK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HOOK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOOK_POOL', pretty_print=True):
@@ -3472,15 +3476,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOOK_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOOK_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOOK_POOL'):
@@ -3566,15 +3570,15 @@
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
     def get_HOOKLOG(self):
         return self.HOOKLOG
     def set_HOOKLOG(self, HOOKLOG):
         self.HOOKLOG = HOOKLOG
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.NAME is not None or
             self.TYPE is not None or
             self.TEMPLATE is not None or
             self.HOOKLOG is not None
         ):
@@ -3593,15 +3597,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOOK')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOOK', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOOK'):
@@ -3710,15 +3714,15 @@
         self.HOST = HOST
     def add_HOST(self, value):
         self.HOST.append(value)
     def insert_HOST_at(self, index, value):
         self.HOST.insert(index, value)
     def replace_HOST_at(self, index, value):
         self.HOST[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HOST
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOST_POOL', pretty_print=True):
@@ -3733,15 +3737,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOST_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOST_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOST_POOL'):
@@ -3869,15 +3873,15 @@
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
     def get_MONITORING(self):
         return self.MONITORING
     def set_MONITORING(self, MONITORING):
         self.MONITORING = MONITORING
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.NAME is not None or
             self.STATE is not None or
             self.PREV_STATE is not None or
             self.IM_MAD is not None or
             self.VM_MAD is not None or
@@ -3903,15 +3907,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOST')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOST', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOST'):
@@ -4086,15 +4090,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_POOL', pretty_print=True):
@@ -4109,15 +4113,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_POOL'):
@@ -4359,15 +4363,15 @@
         return self.SNAPSHOTS
     def set_SNAPSHOTS(self, SNAPSHOTS):
         self.SNAPSHOTS = SNAPSHOTS
     def get_BACKUP_INCREMENTS(self):
         return self.BACKUP_INCREMENTS
     def set_BACKUP_INCREMENTS(self, BACKUP_INCREMENTS):
         self.BACKUP_INCREMENTS = BACKUP_INCREMENTS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -4412,15 +4416,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE'):
@@ -4777,15 +4781,15 @@
         self.MARKETPLACEAPP = MARKETPLACEAPP
     def add_MARKETPLACEAPP(self, value):
         self.MARKETPLACEAPP.append(value)
     def insert_MARKETPLACEAPP_at(self, index, value):
         self.MARKETPLACEAPP.insert(index, value)
     def replace_MARKETPLACEAPP_at(self, index, value):
         self.MARKETPLACEAPP[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.MARKETPLACEAPP
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MARKETPLACEAPP_POOL', pretty_print=True):
@@ -4800,15 +4804,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MARKETPLACEAPP_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MARKETPLACEAPP_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MARKETPLACEAPP_POOL'):
@@ -5002,15 +5006,15 @@
         return self.PERMISSIONS
     def set_PERMISSIONS(self, PERMISSIONS):
         self.PERMISSIONS = PERMISSIONS
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.LOCK is not None or
@@ -5047,15 +5051,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MARKETPLACEAPP')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MARKETPLACEAPP', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MARKETPLACEAPP'):
@@ -5344,15 +5348,15 @@
         self.MARKETPLACE = MARKETPLACE
     def add_MARKETPLACE(self, value):
         self.MARKETPLACE.append(value)
     def insert_MARKETPLACE_at(self, index, value):
         self.MARKETPLACE.insert(index, value)
     def replace_MARKETPLACE_at(self, index, value):
         self.MARKETPLACE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.MARKETPLACE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MARKETPLACE_POOL', pretty_print=True):
@@ -5367,15 +5371,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MARKETPLACE_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MARKETPLACE_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MARKETPLACE_POOL'):
@@ -5521,15 +5525,15 @@
         return self.PERMISSIONS
     def set_PERMISSIONS(self, PERMISSIONS):
         self.PERMISSIONS = PERMISSIONS
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -5558,15 +5562,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MARKETPLACE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MARKETPLACE', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MARKETPLACE'):
@@ -5775,15 +5779,15 @@
         self.MONITORING = MONITORING
     def add_MONITORING(self, value):
         self.MONITORING.append(value)
     def insert_MONITORING_at(self, index, value):
         self.MONITORING.insert(index, value)
     def replace_MONITORING_at(self, index, value):
         self.MONITORING[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.MONITORING
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORING_DATA', pretty_print=True):
@@ -5798,15 +5802,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORING_DATA')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORING_DATA', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORING_DATA'):
@@ -6909,15 +6913,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_VM_SUBMIT_ON_HOLDType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_VM_SUBMIT_ON_HOLDType_patterns_, ))
                 result = False
         return result
     validate_VM_SUBMIT_ON_HOLDType_patterns_ = [['^([yY][eE][sS])$', '^([nN][oO])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.API_LIST_ORDER or
             self.AUTH_MAD or
             self.AUTH_MAD_CONF or
             self.CLUSTER_ENCRYPTED_ATTR or
             self.CONTEXT_RESTRICTED_DIRS is not None or
             self.CONTEXT_SAFE_DIRS is not None or
@@ -7018,15 +7022,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OPENNEBULA_CONFIGURATION')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OPENNEBULA_CONFIGURATION', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OPENNEBULA_CONFIGURATION'):
@@ -7952,15 +7956,15 @@
         return self.LOG_TERM
     def set_LOG_TERM(self, LOG_TERM):
         self.LOG_TERM = LOG_TERM
     def get_FEDLOG_INDEX(self):
         return self.FEDLOG_INDEX
     def set_FEDLOG_INDEX(self, FEDLOG_INDEX):
         self.FEDLOG_INDEX = FEDLOG_INDEX
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.SERVER_ID is not None or
             self.STATE is not None or
             self.TERM is not None or
             self.VOTEDFOR is not None or
             self.COMMIT is not None or
             self.LOG_INDEX is not None or
@@ -7982,15 +7986,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='RAFT')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='RAFT', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='RAFT'):
@@ -8133,15 +8137,15 @@
         self.SECURITY_GROUP = SECURITY_GROUP
     def add_SECURITY_GROUP(self, value):
         self.SECURITY_GROUP.append(value)
     def insert_SECURITY_GROUP_at(self, index, value):
         self.SECURITY_GROUP.insert(index, value)
     def replace_SECURITY_GROUP_at(self, index, value):
         self.SECURITY_GROUP[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.SECURITY_GROUP
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SECURITY_GROUP_POOL', pretty_print=True):
@@ -8156,15 +8160,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SECURITY_GROUP_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SECURITY_GROUP_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SECURITY_GROUP_POOL'):
@@ -8292,15 +8296,15 @@
         return self.ERROR_VMS
     def set_ERROR_VMS(self, ERROR_VMS):
         self.ERROR_VMS = ERROR_VMS
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -8326,15 +8330,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SECURITY_GROUP')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SECURITY_GROUP', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SECURITY_GROUP'):
@@ -8505,15 +8509,15 @@
         self.SHOWBACK = SHOWBACK
     def add_SHOWBACK(self, value):
         self.SHOWBACK.append(value)
     def insert_SHOWBACK_at(self, index, value):
         self.SHOWBACK.insert(index, value)
     def replace_SHOWBACK_at(self, index, value):
         self.SHOWBACK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.SHOWBACK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SHOWBACK_RECORDS', pretty_print=True):
@@ -8528,15 +8532,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SHOWBACK_RECORDS')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SHOWBACK_RECORDS', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SHOWBACK_RECORDS'):
@@ -8628,15 +8632,15 @@
         self.QUOTAS.insert(index, value)
     def replace_QUOTAS_at(self, index, value):
         self.QUOTAS[index] = value
     def get_DEFAULT_USER_QUOTAS(self):
         return self.DEFAULT_USER_QUOTAS
     def set_DEFAULT_USER_QUOTAS(self, DEFAULT_USER_QUOTAS):
         self.DEFAULT_USER_QUOTAS = DEFAULT_USER_QUOTAS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.USER or
             self.QUOTAS or
             self.DEFAULT_USER_QUOTAS is not None
         ):
             return True
         else:
@@ -8653,15 +8657,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USER_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USER_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USER_POOL'):
@@ -8832,15 +8836,15 @@
         return self.IMAGE_QUOTA
     def set_IMAGE_QUOTA(self, IMAGE_QUOTA):
         self.IMAGE_QUOTA = IMAGE_QUOTA
     def get_DEFAULT_USER_QUOTAS(self):
         return self.DEFAULT_USER_QUOTAS
     def set_DEFAULT_USER_QUOTAS(self, DEFAULT_USER_QUOTAS):
         self.DEFAULT_USER_QUOTAS = DEFAULT_USER_QUOTAS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.GID is not None or
             self.GROUPS is not None or
             self.GNAME is not None or
             self.NAME is not None or
             self.PASSWORD is not None or
@@ -8869,15 +8873,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USER')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USER', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USER'):
@@ -9076,15 +9080,15 @@
         self.VDC = VDC
     def add_VDC(self, value):
         self.VDC.append(value)
     def insert_VDC_at(self, index, value):
         self.VDC.insert(index, value)
     def replace_VDC_at(self, index, value):
         self.VDC[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VDC
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VDC_POOL', pretty_print=True):
@@ -9099,15 +9103,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VDC_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VDC_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VDC_POOL'):
@@ -9211,15 +9215,15 @@
         return self.VNETS
     def set_VNETS(self, VNETS):
         self.VNETS = VNETS
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.NAME is not None or
             self.GROUPS is not None or
             self.CLUSTERS is not None or
             self.HOSTS is not None or
             self.DATASTORES is not None or
@@ -9241,15 +9245,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VDC')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VDC', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VDC'):
@@ -9382,15 +9386,15 @@
         self.VM_GROUP = VM_GROUP
     def add_VM_GROUP(self, value):
         self.VM_GROUP.append(value)
     def insert_VM_GROUP_at(self, index, value):
         self.VM_GROUP.insert(index, value)
     def replace_VM_GROUP_at(self, index, value):
         self.VM_GROUP[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM_GROUP
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_GROUP_POOL', pretty_print=True):
@@ -9405,15 +9409,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_GROUP_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_GROUP_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_GROUP_POOL'):
@@ -9529,15 +9533,15 @@
         return self.ROLES
     def set_ROLES(self, ROLES):
         self.ROLES = ROLES
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -9561,15 +9565,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_GROUP')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_GROUP', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_GROUP'):
@@ -9726,15 +9730,15 @@
         self.VM = VM
     def add_VM(self, value):
         self.VM.append(value)
     def insert_VM_at(self, index, value):
         self.VM.insert(index, value)
     def replace_VM_at(self, index, value):
         self.VM[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_POOL', pretty_print=True):
@@ -9749,15 +9753,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_POOL'):
@@ -9828,15 +9832,15 @@
         self.VMTEMPLATE = VMTEMPLATE
     def add_VMTEMPLATE(self, value):
         self.VMTEMPLATE.append(value)
     def insert_VMTEMPLATE_at(self, index, value):
         self.VMTEMPLATE.insert(index, value)
     def replace_VMTEMPLATE_at(self, index, value):
         self.VMTEMPLATE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VMTEMPLATE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMTEMPLATE_POOL', pretty_print=True):
@@ -9851,15 +9855,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMTEMPLATE_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMTEMPLATE_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMTEMPLATE_POOL'):
@@ -9975,15 +9979,15 @@
         return self.REGTIME
     def set_REGTIME(self, REGTIME):
         self.REGTIME = REGTIME
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -10007,15 +10011,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMTEMPLATE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMTEMPLATE', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMTEMPLATE'):
@@ -10304,15 +10308,15 @@
         self.SNAPSHOTS.insert(index, value)
     def replace_SNAPSHOTS_at(self, index, value):
         self.SNAPSHOTS[index] = value
     def get_BACKUPS(self):
         return self.BACKUPS
     def set_BACKUPS(self, BACKUPS):
         self.BACKUPS = BACKUPS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -10349,15 +10353,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM'):
@@ -10634,15 +10638,15 @@
         self.VNET = VNET
     def add_VNET(self, value):
         self.VNET.append(value)
     def insert_VNET_at(self, index, value):
         self.VNET.insert(index, value)
     def replace_VNET_at(self, index, value):
         self.VNET[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VNET
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNET_POOL', pretty_print=True):
@@ -10657,15 +10661,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNET_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNET_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNET_POOL'):
@@ -10889,15 +10893,15 @@
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
     def get_AR_POOL(self):
         return self.AR_POOL
     def set_AR_POOL(self, AR_POOL):
         self.AR_POOL = AR_POOL
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -10939,15 +10943,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNET')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNET', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNET'):
@@ -11270,15 +11274,15 @@
         self.VNTEMPLATE = VNTEMPLATE
     def add_VNTEMPLATE(self, value):
         self.VNTEMPLATE.append(value)
     def insert_VNTEMPLATE_at(self, index, value):
         self.VNTEMPLATE.insert(index, value)
     def replace_VNTEMPLATE_at(self, index, value):
         self.VNTEMPLATE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VNTEMPLATE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNTEMPLATE_POOL', pretty_print=True):
@@ -11293,15 +11297,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNTEMPLATE_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNTEMPLATE_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNTEMPLATE_POOL'):
@@ -11417,15 +11421,15 @@
         return self.REGTIME
     def set_REGTIME(self, REGTIME):
         self.REGTIME = REGTIME
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -11449,15 +11453,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNTEMPLATE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNTEMPLATE', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNTEMPLATE'):
@@ -11614,15 +11618,15 @@
         self.VROUTER = VROUTER
     def add_VROUTER(self, value):
         self.VROUTER.append(value)
     def insert_VROUTER_at(self, index, value):
         self.VROUTER.insert(index, value)
     def replace_VROUTER_at(self, index, value):
         self.VROUTER[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VROUTER
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VROUTER_POOL', pretty_print=True):
@@ -11637,15 +11641,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VROUTER_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VROUTER_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VROUTER_POOL'):
@@ -11761,15 +11765,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -11793,15 +11797,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VROUTER')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VROUTER', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VROUTER'):
@@ -11958,15 +11962,15 @@
         self.ZONE = ZONE
     def add_ZONE(self, value):
         self.ZONE.append(value)
     def insert_ZONE_at(self, index, value):
         self.ZONE.insert(index, value)
     def replace_ZONE_at(self, index, value):
         self.ZONE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ZONE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ZONE_POOL', pretty_print=True):
@@ -11981,15 +11985,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ZONE_POOL')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ZONE_POOL', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ZONE_POOL'):
@@ -12075,15 +12079,15 @@
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
     def get_SERVER_POOL(self):
         return self.SERVER_POOL
     def set_SERVER_POOL(self, SERVER_POOL):
         self.SERVER_POOL = SERVER_POOL
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.NAME is not None or
             self.STATE is not None or
             self.TEMPLATE is not None or
             self.SERVER_POOL is not None
         ):
@@ -12102,15 +12106,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ZONE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ZONE', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ZONE'):
@@ -12345,15 +12349,15 @@
         self.SNAPSHOTS.insert(index, value)
     def replace_SNAPSHOTS_at(self, index, value):
         self.SNAPSHOTS[index] = value
     def get_BACKUPS(self):
         return self.BACKUPS
     def set_BACKUPS(self, BACKUPS):
         self.BACKUPS = BACKUPS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -12389,15 +12393,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType'):
@@ -12657,15 +12661,15 @@
         else:
             return MONITORING(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='MONITORING', pretty_print=True):
@@ -12680,15 +12684,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORING')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORING', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORING'):
         pass
@@ -12787,15 +12791,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -12818,15 +12822,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType'):
@@ -13003,15 +13007,15 @@
         self.SNAPSHOT = SNAPSHOT
     def add_SNAPSHOT(self, value):
         self.SNAPSHOT.append(value)
     def insert_SNAPSHOT_at(self, index, value):
         self.SNAPSHOT.insert(index, value)
     def replace_SNAPSHOT_at(self, index, value):
         self.SNAPSHOT[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ALLOW_ORPHANS is not None or
             self.CURRENT_BASE is not None or
             self.DISK_ID is not None or
             self.NEXT_SNAPSHOT is not None or
             self.SNAPSHOT
         ):
@@ -13030,15 +13034,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTSType'):
@@ -13176,15 +13180,15 @@
         return self.PARENT
     def set_PARENT(self, PARENT):
         self.PARENT = PARENT
     def get_SIZE(self):
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ACTIVE is not None or
             self.CHILDREN is not None or
             self.DATE is not None or
             self.ID is not None or
             self.NAME is not None or
             self.PARENT is not None or
@@ -13205,15 +13209,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType'):
@@ -13343,15 +13347,15 @@
         return self.BACKUP_CONFIG
     def set_BACKUP_CONFIG(self, BACKUP_CONFIG):
         self.BACKUP_CONFIG = BACKUP_CONFIG
     def get_BACKUP_IDS(self):
         return self.BACKUP_IDS
     def set_BACKUP_IDS(self, BACKUP_IDS):
         self.BACKUP_IDS = BACKUP_IDS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.BACKUP_CONFIG is not None or
             self.BACKUP_IDS is not None
         ):
             return True
         else:
             return False
@@ -13367,15 +13371,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUPSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUPSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUPSType'):
@@ -13493,15 +13497,15 @@
         return self.LAST_INCREMENT_ID
     def set_LAST_INCREMENT_ID(self, LAST_INCREMENT_ID):
         self.LAST_INCREMENT_ID = LAST_INCREMENT_ID
     def get_MODE(self):
         return self.MODE
     def set_MODE(self, MODE):
         self.MODE = MODE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.BACKUP_VOLATILE is not None or
             self.FS_FREEZE is not None or
             self.INCREMENTAL_BACKUP_ID is not None or
             self.KEEP_LAST is not None or
             self.LAST_BACKUP_ID is not None or
             self.LAST_BACKUP_SIZE is not None or
@@ -13524,15 +13528,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_CONFIGType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_CONFIGType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_CONFIGType'):
@@ -13685,15 +13689,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_IDSType', pretty_print=True):
@@ -13708,15 +13712,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_IDSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_IDSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_IDSType'):
@@ -13810,15 +13814,15 @@
         return self.ZONE
     def set_ZONE(self, ZONE):
         self.ZONE = ZONE
     def get_STRING(self):
         return self.STRING
     def set_STRING(self, STRING):
         self.STRING = STRING
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.USER is not None or
             self.RESOURCE is not None or
             self.RIGHTS is not None or
             self.ZONE is not None or
             self.STRING is not None
@@ -13838,15 +13842,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ACLType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ACLType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ACLType'):
@@ -13969,15 +13973,15 @@
         self.PARAMETER = PARAMETER
     def add_PARAMETER(self, value):
         self.PARAMETER.append(value)
     def insert_PARAMETER_at(self, index, value):
         self.PARAMETER.insert(index, value)
     def replace_PARAMETER_at(self, index, value):
         self.PARAMETER[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.PARAMETER
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PARAMETERSType', pretty_print=True):
@@ -13992,15 +13996,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PARAMETERSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PARAMETERSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PARAMETERSType'):
@@ -14090,15 +14094,15 @@
             value = value
             enumerations = ['IN', 'OUT']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on TYPEType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.POSITION is not None or
             self.TYPE is not None or
             self.VALUE is not None
         ):
             return True
         else:
@@ -14115,15 +14119,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PARAMETERType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PARAMETERType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PARAMETERType'):
@@ -14211,15 +14215,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.anytypeobjs_
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='EXTRAType', pretty_print=True):
@@ -14234,15 +14238,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='EXTRAType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='EXTRAType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='EXTRAType'):
@@ -14312,15 +14316,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOSTSType', pretty_print=True):
@@ -14335,15 +14339,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOSTSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOSTSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOSTSType'):
@@ -14416,15 +14420,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORESType', pretty_print=True):
@@ -14439,15 +14443,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORESType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORESType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORESType'):
@@ -14520,15 +14524,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETSType', pretty_print=True):
@@ -14543,15 +14547,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNETSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNETSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNETSType'):
@@ -14663,15 +14667,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -14694,15 +14698,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType1')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType1', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType1'):
@@ -14855,15 +14859,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType', pretty_print=True):
@@ -14878,15 +14882,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType'):
@@ -14959,15 +14963,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGESType', pretty_print=True):
@@ -14982,15 +14986,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGESType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGESType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGESType'):
@@ -15092,15 +15096,15 @@
         return self.VCENTER_INSTANCE_ID
     def set_VCENTER_INSTANCE_ID(self, VCENTER_INSTANCE_ID):
         self.VCENTER_INSTANCE_ID = VCENTER_INSTANCE_ID
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VCENTER_DC_NAME is not None or
             self.VCENTER_DC_REF is not None or
             self.VCENTER_DS_NAME is not None or
             self.VCENTER_DS_REF is not None or
             self.VCENTER_HOST is not None or
             self.VCENTER_INSTANCE_ID is not None or
@@ -15121,15 +15125,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType'):
@@ -15299,15 +15303,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -15330,15 +15334,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType2')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType2', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType2'):
@@ -15500,15 +15504,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -15526,15 +15530,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType'):
@@ -15652,15 +15656,15 @@
         return self.USERS
     def set_USERS(self, USERS):
         self.USERS = USERS
     def get_ADMINS(self):
         return self.ADMINS
     def set_ADMINS(self, ADMINS):
         self.ADMINS = ADMINS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.NAME is not None or
             self.TEMPLATE is not None or
             self.USERS is not None or
             self.ADMINS is not None
         ):
@@ -15679,15 +15683,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUPType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUPType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUPType'):
@@ -15796,15 +15800,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='USERSType', pretty_print=True):
@@ -15819,15 +15823,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USERSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USERSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USERSType'):
@@ -15900,15 +15904,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ADMINSType', pretty_print=True):
@@ -15923,15 +15927,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ADMINSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ADMINSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ADMINSType'):
@@ -16019,15 +16023,15 @@
         return self.VM_QUOTA
     def set_VM_QUOTA(self, VM_QUOTA):
         self.VM_QUOTA = VM_QUOTA
     def get_IMAGE_QUOTA(self):
         return self.IMAGE_QUOTA
     def set_IMAGE_QUOTA(self, IMAGE_QUOTA):
         self.IMAGE_QUOTA = IMAGE_QUOTA
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.DATASTORE_QUOTA is not None or
             self.NETWORK_QUOTA is not None or
             self.VM_QUOTA is not None or
             self.IMAGE_QUOTA is not None
         ):
@@ -16046,15 +16050,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='QUOTASType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='QUOTASType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='QUOTASType'):
@@ -16159,15 +16163,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType', pretty_print=True):
@@ -16182,15 +16186,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType'):
@@ -16276,15 +16280,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_SIZE_USED(self):
         return self.SIZE_USED
     def set_SIZE_USED(self, SIZE_USED):
         self.SIZE_USED = SIZE_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.IMAGES is not None or
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
@@ -16303,15 +16307,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType'):
@@ -16424,15 +16428,15 @@
         self.NETWORK = NETWORK
     def add_NETWORK(self, value):
         self.NETWORK.append(value)
     def insert_NETWORK_at(self, index, value):
         self.NETWORK.insert(index, value)
     def replace_NETWORK_at(self, index, value):
         self.NETWORK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType', pretty_print=True):
@@ -16447,15 +16451,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType'):
@@ -16529,15 +16533,15 @@
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
     def get_LEASES_USED(self):
         return self.LEASES_USED
     def set_LEASES_USED(self, LEASES_USED):
         self.LEASES_USED = LEASES_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
@@ -16554,15 +16558,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType'):
@@ -16646,15 +16650,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType', pretty_print=True):
@@ -16669,15 +16673,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType'):
@@ -16817,15 +16821,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_VMS_USED(self):
         return self.VMS_USED
     def set_VMS_USED(self, VMS_USED):
         self.VMS_USED = VMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.CPU_USED is not None or
             self.MEMORY is not None or
             self.MEMORY_USED is not None or
             self.RUNNING_CPU is not None or
             self.RUNNING_CPU_USED is not None or
@@ -16853,15 +16857,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType3')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType3', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType3'):
@@ -17064,15 +17068,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType', pretty_print=True):
@@ -17087,15 +17091,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType'):
@@ -17169,15 +17173,15 @@
         return self.RVMS
     def set_RVMS(self, RVMS):
         self.RVMS = RVMS
     def get_RVMS_USED(self):
         return self.RVMS_USED
     def set_RVMS_USED(self, RVMS_USED):
         self.RVMS_USED = RVMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
@@ -17194,15 +17198,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType'):
@@ -17304,15 +17308,15 @@
         return self.VM_QUOTA
     def set_VM_QUOTA(self, VM_QUOTA):
         self.VM_QUOTA = VM_QUOTA
     def get_IMAGE_QUOTA(self):
         return self.IMAGE_QUOTA
     def set_IMAGE_QUOTA(self, IMAGE_QUOTA):
         self.IMAGE_QUOTA = IMAGE_QUOTA
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE_QUOTA is not None or
             self.NETWORK_QUOTA is not None or
             self.VM_QUOTA is not None or
             self.IMAGE_QUOTA is not None
         ):
             return True
@@ -17330,15 +17334,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DEFAULT_GROUP_QUOTASType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DEFAULT_GROUP_QUOTASType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DEFAULT_GROUP_QUOTASType'):
@@ -17433,15 +17437,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType4', pretty_print=True):
@@ -17456,15 +17460,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType4')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType4', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType4'):
@@ -17550,15 +17554,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_SIZE_USED(self):
         return self.SIZE_USED
     def set_SIZE_USED(self, SIZE_USED):
         self.SIZE_USED = SIZE_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.IMAGES is not None or
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
@@ -17577,15 +17581,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType5')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType5', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType5'):
@@ -17698,15 +17702,15 @@
         self.NETWORK = NETWORK
     def add_NETWORK(self, value):
         self.NETWORK.append(value)
     def insert_NETWORK_at(self, index, value):
         self.NETWORK.insert(index, value)
     def replace_NETWORK_at(self, index, value):
         self.NETWORK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType6', pretty_print=True):
@@ -17721,15 +17725,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType6')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType6', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType6'):
@@ -17803,15 +17807,15 @@
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
     def get_LEASES_USED(self):
         return self.LEASES_USED
     def set_LEASES_USED(self, LEASES_USED):
         self.LEASES_USED = LEASES_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
@@ -17828,15 +17832,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType7')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType7', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType7'):
@@ -17920,15 +17924,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType8', pretty_print=True):
@@ -17943,15 +17947,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType8')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType8', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType8'):
@@ -18091,15 +18095,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_VMS_USED(self):
         return self.VMS_USED
     def set_VMS_USED(self, VMS_USED):
         self.VMS_USED = VMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.CPU_USED is not None or
             self.MEMORY is not None or
             self.MEMORY_USED is not None or
             self.RUNNING_CPU is not None or
             self.RUNNING_CPU_USED is not None or
@@ -18127,15 +18131,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType9')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType9', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType9'):
@@ -18338,15 +18342,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType10', pretty_print=True):
@@ -18361,15 +18365,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType10')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType10', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType10'):
@@ -18443,15 +18447,15 @@
         return self.RVMS
     def set_RVMS(self, RVMS):
         self.RVMS = RVMS
     def get_RVMS_USED(self):
         return self.RVMS_USED
     def set_RVMS_USED(self, RVMS_USED):
         self.RVMS_USED = RVMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
@@ -18468,15 +18472,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType11')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType11', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType11'):
@@ -18569,15 +18573,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='USERSType12', pretty_print=True):
@@ -18592,15 +18596,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USERSType12')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USERSType12', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USERSType12'):
@@ -18673,15 +18677,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ADMINSType13', pretty_print=True):
@@ -18696,15 +18700,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ADMINSType13')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ADMINSType13', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ADMINSType13'):
@@ -18777,15 +18781,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType14', pretty_print=True):
@@ -18800,15 +18804,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType14')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType14', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType14'):
@@ -18894,15 +18898,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_SIZE_USED(self):
         return self.SIZE_USED
     def set_SIZE_USED(self, SIZE_USED):
         self.SIZE_USED = SIZE_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.IMAGES is not None or
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
@@ -18921,15 +18925,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType15')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType15', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType15'):
@@ -19042,15 +19046,15 @@
         self.NETWORK = NETWORK
     def add_NETWORK(self, value):
         self.NETWORK.append(value)
     def insert_NETWORK_at(self, index, value):
         self.NETWORK.insert(index, value)
     def replace_NETWORK_at(self, index, value):
         self.NETWORK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType16', pretty_print=True):
@@ -19065,15 +19069,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType16')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType16', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType16'):
@@ -19147,15 +19151,15 @@
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
     def get_LEASES_USED(self):
         return self.LEASES_USED
     def set_LEASES_USED(self, LEASES_USED):
         self.LEASES_USED = LEASES_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
@@ -19172,15 +19176,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType17')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType17', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType17'):
@@ -19264,15 +19268,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType18', pretty_print=True):
@@ -19287,15 +19291,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType18')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType18', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType18'):
@@ -19435,15 +19439,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_VMS_USED(self):
         return self.VMS_USED
     def set_VMS_USED(self, VMS_USED):
         self.VMS_USED = VMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.CPU_USED is not None or
             self.MEMORY is not None or
             self.MEMORY_USED is not None or
             self.RUNNING_CPU is not None or
             self.RUNNING_CPU_USED is not None or
@@ -19471,15 +19475,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType19')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType19', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType19'):
@@ -19682,15 +19686,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType20', pretty_print=True):
@@ -19705,15 +19709,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType20')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType20', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType20'):
@@ -19787,15 +19791,15 @@
         return self.RVMS
     def set_RVMS(self, RVMS):
         self.RVMS = RVMS
     def get_RVMS_USED(self):
         return self.RVMS_USED
     def set_RVMS_USED(self, RVMS_USED):
         self.RVMS_USED = RVMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
@@ -19812,15 +19816,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType21')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType21', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType21'):
@@ -19922,15 +19926,15 @@
         return self.VM_QUOTA
     def set_VM_QUOTA(self, VM_QUOTA):
         self.VM_QUOTA = VM_QUOTA
     def get_IMAGE_QUOTA(self):
         return self.IMAGE_QUOTA
     def set_IMAGE_QUOTA(self, IMAGE_QUOTA):
         self.IMAGE_QUOTA = IMAGE_QUOTA
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE_QUOTA is not None or
             self.NETWORK_QUOTA is not None or
             self.VM_QUOTA is not None or
             self.IMAGE_QUOTA is not None
         ):
             return True
@@ -19948,15 +19952,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DEFAULT_GROUP_QUOTASType22')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DEFAULT_GROUP_QUOTASType22', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DEFAULT_GROUP_QUOTASType22'):
@@ -20051,15 +20055,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType23', pretty_print=True):
@@ -20074,15 +20078,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType23')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType23', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType23'):
@@ -20168,15 +20172,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_SIZE_USED(self):
         return self.SIZE_USED
     def set_SIZE_USED(self, SIZE_USED):
         self.SIZE_USED = SIZE_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.IMAGES is not None or
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
@@ -20195,15 +20199,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType24')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType24', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType24'):
@@ -20316,15 +20320,15 @@
         self.NETWORK = NETWORK
     def add_NETWORK(self, value):
         self.NETWORK.append(value)
     def insert_NETWORK_at(self, index, value):
         self.NETWORK.insert(index, value)
     def replace_NETWORK_at(self, index, value):
         self.NETWORK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType25', pretty_print=True):
@@ -20339,15 +20343,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType25')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType25', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType25'):
@@ -20421,15 +20425,15 @@
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
     def get_LEASES_USED(self):
         return self.LEASES_USED
     def set_LEASES_USED(self, LEASES_USED):
         self.LEASES_USED = LEASES_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
@@ -20446,15 +20450,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType26')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType26', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType26'):
@@ -20538,15 +20542,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType27', pretty_print=True):
@@ -20561,15 +20565,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType27')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType27', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType27'):
@@ -20709,15 +20713,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_VMS_USED(self):
         return self.VMS_USED
     def set_VMS_USED(self, VMS_USED):
         self.VMS_USED = VMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.CPU_USED is not None or
             self.MEMORY is not None or
             self.MEMORY_USED is not None or
             self.RUNNING_CPU is not None or
             self.RUNNING_CPU_USED is not None or
@@ -20745,15 +20749,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType28')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType28', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType28'):
@@ -20956,15 +20960,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType29', pretty_print=True):
@@ -20979,15 +20983,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType29')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType29', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType29'):
@@ -21061,15 +21065,15 @@
         return self.RVMS
     def set_RVMS(self, RVMS):
         self.RVMS = RVMS
     def get_RVMS_USED(self):
         return self.RVMS_USED
     def set_RVMS_USED(self, RVMS_USED):
         self.RVMS_USED = RVMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
@@ -21086,15 +21090,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType30')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType30', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType30'):
@@ -21228,15 +21232,15 @@
         return self.LCM_STATE
     def set_LCM_STATE(self, LCM_STATE):
         self.LCM_STATE = LCM_STATE
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ARGUMENTS is not None or
             self.ARGUMENTS_STDIN is not None or
             self.CALL is not None or
             self.COMMAND is not None or
             self.REMOTE is not None or
             self.RESOURCE is not None or
@@ -21259,15 +21263,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType31')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType31', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType31'):
@@ -21418,15 +21422,15 @@
         self.HOOK_EXECUTION_RECORD = HOOK_EXECUTION_RECORD
     def add_HOOK_EXECUTION_RECORD(self, value):
         self.HOOK_EXECUTION_RECORD.append(value)
     def insert_HOOK_EXECUTION_RECORD_at(self, index, value):
         self.HOOK_EXECUTION_RECORD.insert(index, value)
     def replace_HOOK_EXECUTION_RECORD_at(self, index, value):
         self.HOOK_EXECUTION_RECORD[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HOOK_EXECUTION_RECORD
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOOKLOGType', pretty_print=True):
@@ -21441,15 +21445,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOOKLOGType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOOKLOGType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOOKLOGType'):
@@ -21555,15 +21559,15 @@
         return self.RETRY
     def set_RETRY(self, RETRY):
         self.RETRY = RETRY
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HOOK_ID is not None or
             self.EXECUTION_ID is not None or
             self.TIMESTAMP is not None or
             self.ARGUMENTS is not None or
             self.EXECUTION_RESULT is not None or
             self.REMOTE_HOST is not None or
@@ -21585,15 +21589,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOOK_EXECUTION_RECORDType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOOK_EXECUTION_RECORDType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOOK_EXECUTION_RECORDType'):
@@ -21741,15 +21745,15 @@
         return self.STDERR
     def set_STDERR(self, STDERR):
         self.STDERR = STDERR
     def get_CODE(self):
         return self.CODE
     def set_CODE(self, CODE):
         self.CODE = CODE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.COMMAND is not None or
             self.STDOUT is not None or
             self.STDERR is not None or
             self.CODE is not None
         ):
             return True
@@ -21767,15 +21771,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='EXECUTION_RESULTType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='EXECUTION_RESULTType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='EXECUTION_RESULTType'):
@@ -21929,15 +21933,15 @@
         return self.PCI_DEVICES
     def set_PCI_DEVICES(self, PCI_DEVICES):
         self.PCI_DEVICES = PCI_DEVICES
     def get_NUMA_NODES(self):
         return self.NUMA_NODES
     def set_NUMA_NODES(self, NUMA_NODES):
         self.NUMA_NODES = NUMA_NODES
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.MEM_USAGE is not None or
             self.CPU_USAGE is not None or
             self.TOTAL_MEM is not None or
             self.TOTAL_CPU is not None or
             self.MAX_MEM is not None or
             self.MAX_CPU is not None or
@@ -21962,15 +21966,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOST_SHAREType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOST_SHAREType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOST_SHAREType'):
@@ -22146,15 +22150,15 @@
         return self.MAX_DISK
     def set_MAX_DISK(self, MAX_DISK):
         self.MAX_DISK = MAX_DISK
     def get_USED_DISK(self):
         return self.USED_DISK
     def set_USED_DISK(self, USED_DISK):
         self.USED_DISK = USED_DISK
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DISK_USAGE is not None or
             self.FREE_DISK is not None or
             self.MAX_DISK is not None or
             self.USED_DISK is not None
         ):
             return True
@@ -22172,15 +22176,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORESType32')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORESType32', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORESType32'):
@@ -22283,15 +22287,15 @@
         self.PCI = PCI
     def add_PCI(self, value):
         self.PCI.append(value)
     def insert_PCI_at(self, index, value):
         self.PCI.insert(index, value)
     def replace_PCI_at(self, index, value):
         self.PCI[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.PCI
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='PCI_DEVICESType', pretty_print=True):
@@ -22306,15 +22310,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PCI_DEVICESType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PCI_DEVICESType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PCI_DEVICESType'):
@@ -22472,15 +22476,15 @@
         return self.VENDOR_NAME
     def set_VENDOR_NAME(self, VENDOR_NAME):
         self.VENDOR_NAME = VENDOR_NAME
     def get_VMID(self):
         return self.VMID
     def set_VMID(self, VMID):
         self.VMID = VMID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ADDRESS is not None or
             self.BUS is not None or
             self.CLASS is not None or
             self.CLASS_NAME is not None or
             self.DEVICE is not None or
             self.DEVICE_NAME is not None or
@@ -22511,15 +22515,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PCIType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PCIType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PCIType'):
@@ -22752,15 +22756,15 @@
         self.NODE = NODE
     def add_NODE(self, value):
         self.NODE.append(value)
     def insert_NODE_at(self, index, value):
         self.NODE.insert(index, value)
     def replace_NODE_at(self, index, value):
         self.NODE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NODE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NUMA_NODESType', pretty_print=True):
@@ -22775,15 +22779,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NUMA_NODESType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NUMA_NODESType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NUMA_NODESType'):
@@ -22881,15 +22885,15 @@
         return self.MEMORY
     def set_MEMORY(self, MEMORY):
         self.MEMORY = MEMORY
     def get_NODE_ID(self):
         return self.NODE_ID
     def set_NODE_ID(self, NODE_ID):
         self.NODE_ID = NODE_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CORE or
             self.HUGEPAGE or
             self.MEMORY is not None or
             self.NODE_ID is not None
         ):
             return True
@@ -22907,15 +22911,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NODEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NODEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NODEType'):
@@ -23021,15 +23025,15 @@
         return self.FREE
     def set_FREE(self, FREE):
         self.FREE = FREE
     def get_ID(self):
         return self.ID
     def set_ID(self, ID):
         self.ID = ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPUS is not None or
             self.DEDICATED is not None or
             self.FREE is not None or
             self.ID is not None
         ):
             return True
@@ -23047,15 +23051,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='COREType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='COREType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='COREType'):
@@ -23161,15 +23165,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_USAGE(self):
         return self.USAGE
     def set_USAGE(self, USAGE):
         self.USAGE = USAGE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.PAGES is not None or
             self.SIZE is not None or
             self.USAGE is not None
         ):
             return True
         else:
@@ -23186,15 +23190,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HUGEPAGEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HUGEPAGEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HUGEPAGEType'):
@@ -23290,15 +23294,15 @@
         return self.TOTAL
     def set_TOTAL(self, TOTAL):
         self.TOTAL = TOTAL
     def get_USAGE(self):
         return self.USAGE
     def set_USAGE(self, USAGE):
         self.USAGE = USAGE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DISTANCE is not None or
             self.TOTAL is not None or
             self.USAGE is not None
         ):
             return True
         else:
@@ -23315,15 +23319,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MEMORYType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MEMORYType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MEMORYType'):
@@ -23416,15 +23420,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType', pretty_print=True):
@@ -23439,15 +23443,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMSType'):
@@ -23585,15 +23589,15 @@
         return self.VCENTER_VERSION
     def set_VCENTER_VERSION(self, VCENTER_VERSION):
         self.VCENTER_VERSION = VCENTER_VERSION
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VCENTER_CCR_REF is not None or
             self.VCENTER_DS_REF or
             self.VCENTER_HOST is not None or
             self.VCENTER_INSTANCE_ID is not None or
             self.VCENTER_NAME is not None or
             self.VCENTER_PASSWORD is not None or
@@ -23617,15 +23621,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType33')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType33', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType33'):
@@ -23771,15 +23775,15 @@
         else:
             return VCENTER_RESOURCE_POOL_INFO(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='VCENTER_RESOURCE_POOL_INFO', pretty_print=True):
@@ -23794,15 +23798,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VCENTER_RESOURCE_POOL_INFO')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VCENTER_RESOURCE_POOL_INFO', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VCENTER_RESOURCE_POOL_INFO'):
         pass
@@ -23886,15 +23890,15 @@
         self.NUMA_NODE = NUMA_NODE
     def add_NUMA_NODE(self, value):
         self.NUMA_NODE.append(value)
     def insert_NUMA_NODE_at(self, index, value):
         self.NUMA_NODE.insert(index, value)
     def replace_NUMA_NODE_at(self, index, value):
         self.NUMA_NODE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.TIMESTAMP is not None or
             self.ID is not None or
             self.CAPACITY is not None or
             self.SYSTEM is not None or
             self.NUMA_NODE
         ):
@@ -23913,15 +23917,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType'):
@@ -24037,15 +24041,15 @@
         return self.USED_CPU
     def set_USED_CPU(self, USED_CPU):
         self.USED_CPU = USED_CPU
     def get_USED_MEMORY(self):
         return self.USED_MEMORY
     def set_USED_MEMORY(self, USED_MEMORY):
         self.USED_MEMORY = USED_MEMORY
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.FREE_CPU is not None or
             self.FREE_MEMORY is not None or
             self.USED_CPU is not None or
             self.USED_MEMORY is not None
         ):
             return True
@@ -24063,15 +24067,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CAPACITYType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CAPACITYType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CAPACITYType'):
@@ -24171,15 +24175,15 @@
         return self.NETRX
     def set_NETRX(self, NETRX):
         self.NETRX = NETRX
     def get_NETTX(self):
         return self.NETTX
     def set_NETTX(self, NETTX):
         self.NETTX = NETTX
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETRX is not None or
             self.NETTX is not None
         ):
             return True
         else:
             return False
@@ -24195,15 +24199,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SYSTEMType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SYSTEMType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SYSTEMType'):
@@ -24298,15 +24302,15 @@
         return self.MEMORY
     def set_MEMORY(self, MEMORY):
         self.MEMORY = MEMORY
     def get_NODE_ID(self):
         return self.NODE_ID
     def set_NODE_ID(self, NODE_ID):
         self.NODE_ID = NODE_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HUGEPAGE or
             self.MEMORY is not None or
             self.NODE_ID is not None
         ):
             return True
         else:
@@ -24323,15 +24327,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NUMA_NODEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NUMA_NODEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NUMA_NODEType'):
@@ -24417,15 +24421,15 @@
         return self.FREE
     def set_FREE(self, FREE):
         self.FREE = FREE
     def get_SIZE(self):
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.FREE is not None or
             self.SIZE is not None
         ):
             return True
         else:
             return False
@@ -24441,15 +24445,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HUGEPAGEType34')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HUGEPAGEType34', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HUGEPAGEType34'):
@@ -24529,15 +24533,15 @@
         return self.FREE
     def set_FREE(self, FREE):
         self.FREE = FREE
     def get_USED(self):
         return self.USED
     def set_USED(self, USED):
         self.USED = USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.FREE is not None or
             self.USED is not None
         ):
             return True
         else:
             return False
@@ -24553,15 +24557,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MEMORYType35')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MEMORYType35', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MEMORYType35'):
@@ -24653,15 +24657,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -24679,15 +24683,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType36')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType36', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType36'):
@@ -24829,15 +24833,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -24860,15 +24864,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType37')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType37', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType37'):
@@ -25021,15 +25025,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType38', pretty_print=True):
@@ -25044,15 +25048,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMSType38')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMSType38', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMSType38'):
@@ -25125,15 +25129,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLONESType', pretty_print=True):
@@ -25148,15 +25152,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLONESType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLONESType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLONESType'):
@@ -25229,15 +25233,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='APP_CLONESType', pretty_print=True):
@@ -25252,15 +25256,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='APP_CLONESType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='APP_CLONESType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='APP_CLONESType'):
@@ -25332,15 +25336,15 @@
         return self.VCENTER_IMPORTED
     def set_VCENTER_IMPORTED(self, VCENTER_IMPORTED):
         self.VCENTER_IMPORTED = VCENTER_IMPORTED
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VCENTER_IMPORTED is not None or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
@@ -25356,15 +25360,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType39')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType39', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType39'):
@@ -25463,15 +25467,15 @@
         self.SNAPSHOT = SNAPSHOT
     def add_SNAPSHOT(self, value):
         self.SNAPSHOT.append(value)
     def insert_SNAPSHOT_at(self, index, value):
         self.SNAPSHOT.insert(index, value)
     def replace_SNAPSHOT_at(self, index, value):
         self.SNAPSHOT[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ALLOW_ORPHANS is not None or
             self.CURRENT_BASE is not None or
             self.NEXT_SNAPSHOT is not None or
             self.SNAPSHOT
         ):
             return True
@@ -25489,15 +25493,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTSType40')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTSType40', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTSType40'):
@@ -25625,15 +25629,15 @@
         return self.PARENT
     def set_PARENT(self, PARENT):
         self.PARENT = PARENT
     def get_SIZE(self):
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CHILDREN is not None or
             self.ACTIVE is not None or
             self.DATE is not None or
             self.ID is not None or
             self.NAME is not None or
             self.PARENT is not None or
@@ -25654,15 +25658,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType41')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType41', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType41'):
@@ -25795,15 +25799,15 @@
         self.INCREMENT = INCREMENT
     def add_INCREMENT(self, value):
         self.INCREMENT.append(value)
     def insert_INCREMENT_at(self, index, value):
         self.INCREMENT.insert(index, value)
     def replace_INCREMENT_at(self, index, value):
         self.INCREMENT[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.INCREMENT
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_INCREMENTSType', pretty_print=True):
@@ -25818,15 +25822,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_INCREMENTSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_INCREMENTSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_INCREMENTSType'):
@@ -25918,15 +25922,15 @@
         return self.SOURCE
     def set_SOURCE(self, SOURCE):
         self.SOURCE = SOURCE
     def get_TYPE(self):
         return self.TYPE
     def set_TYPE(self, TYPE):
         self.TYPE = TYPE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATE is not None or
             self.ID is not None or
             self.PARENT_ID is not None or
             self.SIZE is not None or
             self.SOURCE is not None or
             self.TYPE is not None
@@ -25946,15 +25950,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='INCREMENTType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='INCREMENTType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='INCREMENTType'):
@@ -26086,15 +26090,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -26112,15 +26116,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType42')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType42', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType42'):
@@ -26262,15 +26266,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -26293,15 +26297,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType43')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType43', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType43'):
@@ -26454,15 +26458,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MARKETPLACEAPPSType', pretty_print=True):
@@ -26477,15 +26481,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MARKETPLACEAPPSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MARKETPLACEAPPSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MARKETPLACEAPPSType'):
@@ -26597,15 +26601,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -26628,15 +26632,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType44')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType44', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType44'):
@@ -26891,15 +26895,15 @@
         return self.VCENTER_VMWARETOOLS_VERSION_STATUS
     def set_VCENTER_VMWARETOOLS_VERSION_STATUS(self, VCENTER_VMWARETOOLS_VERSION_STATUS):
         self.VCENTER_VMWARETOOLS_VERSION_STATUS = VCENTER_VMWARETOOLS_VERSION_STATUS
     def get_VCENTER_VM_NAME(self):
         return self.VCENTER_VM_NAME
     def set_VCENTER_VM_NAME(self, VCENTER_VM_NAME):
         self.VCENTER_VM_NAME = VCENTER_VM_NAME
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.DISKRDBYTES is not None or
             self.DISKRDIOPS is not None or
             self.DISKWRBYTES is not None or
             self.DISKWRIOPS is not None or
             self.DISK_SIZE or
@@ -26931,15 +26935,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType45')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType45', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType45'):
@@ -27177,15 +27181,15 @@
         return self.ID
     def set_ID(self, ID):
         self.ID = ID
     def get_SIZE(self):
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.SIZE is not None
         ):
             return True
         else:
             return False
@@ -27201,15 +27205,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DISK_SIZEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DISK_SIZEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DISK_SIZEType'):
@@ -27289,15 +27293,15 @@
         return self.AUTHN
     def set_AUTHN(self, AUTHN):
         self.AUTHN = AUTHN
     def get_EXECUTABLE(self):
         return self.EXECUTABLE
     def set_EXECUTABLE(self, EXECUTABLE):
         self.EXECUTABLE = EXECUTABLE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.AUTHN is not None or
             self.EXECUTABLE is not None
         ):
             return True
         else:
             return False
@@ -27313,15 +27317,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='AUTH_MADType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='AUTH_MADType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='AUTH_MADType'):
@@ -27425,15 +27429,15 @@
         return self.PASSWORD_CHANGE
     def set_PASSWORD_CHANGE(self, PASSWORD_CHANGE):
         self.PASSWORD_CHANGE = PASSWORD_CHANGE
     def get_PASSWORD_REQUIRED(self):
         return self.PASSWORD_REQUIRED
     def set_PASSWORD_REQUIRED(self, PASSWORD_REQUIRED):
         self.PASSWORD_REQUIRED = PASSWORD_REQUIRED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DRIVER_MANAGED_GROUPS is not None or
             self.DRIVER_MANAGED_GROUP_ADMIN is not None or
             self.MAX_TOKEN_TIME is not None or
             self.NAME is not None or
             self.PASSWORD_CHANGE is not None or
             self.PASSWORD_REQUIRED is not None
@@ -27453,15 +27457,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='AUTH_MAD_CONFType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='AUTH_MAD_CONFType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='AUTH_MAD_CONFType'):
@@ -27581,15 +27585,15 @@
         return self.ARGUMENTS
     def set_ARGUMENTS(self, ARGUMENTS):
         self.ARGUMENTS = ARGUMENTS
     def get_EXECUTABLE(self):
         return self.EXECUTABLE
     def set_EXECUTABLE(self, EXECUTABLE):
         self.EXECUTABLE = EXECUTABLE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ARGUMENTS is not None or
             self.EXECUTABLE is not None
         ):
             return True
         else:
             return False
@@ -27605,15 +27609,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_MADType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_MADType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_MADType'):
@@ -27766,15 +27770,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_COMPARE_BINARYType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_COMPARE_BINARYType_patterns_, ))
                 result = False
         return result
     validate_COMPARE_BINARYType_patterns_ = [['^([yY][eE][sS])$', '^([nN][oO])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.BACKEND is not None or
             self.COMPARE_BINARY is not None or
             self.CONNECTIONS is not None or
             self.DB_NAME is not None or
             self.PASSWD is not None or
             self.PORT is not None or
@@ -27797,15 +27801,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DBType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DBType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DBType'):
@@ -27965,15 +27969,15 @@
         return self.DISK_COST
     def set_DISK_COST(self, DISK_COST):
         self.DISK_COST = DISK_COST
     def get_MEMORY_COST(self):
         return self.MEMORY_COST
     def set_MEMORY_COST(self, MEMORY_COST):
         self.MEMORY_COST = MEMORY_COST
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU_COST is not None or
             self.DISK_COST is not None or
             self.MEMORY_COST is not None
         ):
             return True
         else:
@@ -27990,15 +27994,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DEFAULT_COSTType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DEFAULT_COSTType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DEFAULT_COSTType'):
@@ -28115,15 +28119,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_PERSISTENT_ONLYType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_PERSISTENT_ONLYType_patterns_, ))
                 result = False
         return result
     validate_PERSISTENT_ONLYType_patterns_ = [['^([yY][eE][sS])$', '^([nN][oO])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.MARKETPLACE_ACTIONS is not None or
             self.NAME is not None or
             self.PERSISTENT_ONLY is not None or
             self.REQUIRED_ATTRS is not None
         ):
             return True
@@ -28141,15 +28145,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DS_MAD_CONFType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DS_MAD_CONFType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DS_MAD_CONFType'):
@@ -28279,15 +28283,15 @@
             value = value
             enumerations = ['STANDALONE', 'MASTER', 'SLAVE']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on MODEType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.MASTER_ONED is not None or
             self.MODE is not None or
             self.SERVER_ID is not None or
             self.ZONE_ID is not None
         ):
             return True
@@ -28305,15 +28309,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='FEDERATIONType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='FEDERATIONType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='FEDERATIONType'):
@@ -28415,15 +28419,15 @@
         return self.ARGUMENTS
     def set_ARGUMENTS(self, ARGUMENTS):
         self.ARGUMENTS = ARGUMENTS
     def get_EXECUTABLE(self):
         return self.EXECUTABLE
     def set_EXECUTABLE(self, EXECUTABLE):
         self.EXECUTABLE = EXECUTABLE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ARGUMENTS is not None or
             self.EXECUTABLE is not None
         ):
             return True
         else:
             return False
@@ -28439,15 +28443,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HM_MADType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HM_MADType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HM_MADType'):
@@ -28521,15 +28525,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_LOG_RETENTION(self):
         return self.LOG_RETENTION
     def set_LOG_RETENTION(self, LOG_RETENTION):
         self.LOG_RETENTION = LOG_RETENTION
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOG_RETENTION is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOOK_LOG_CONFType', pretty_print=True):
@@ -28544,15 +28548,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOOK_LOG_CONFType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOOK_LOG_CONFType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOOK_LOG_CONFType'):
@@ -28634,15 +28638,15 @@
         return self.NAME
     def set_NAME(self, NAME):
         self.NAME = NAME
     def get_THREADS(self):
         return self.THREADS
     def set_THREADS(self, THREADS):
         self.THREADS = THREADS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ARGUMENTS is not None or
             self.EXECUTABLE is not None or
             self.NAME is not None or
             self.THREADS is not None
         ):
             return True
@@ -28660,15 +28664,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IM_MADType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IM_MADType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IM_MADType'):
@@ -28768,15 +28772,15 @@
         return self.ARGUMENTS
     def set_ARGUMENTS(self, ARGUMENTS):
         self.ARGUMENTS = ARGUMENTS
     def get_EXECUTABLE(self):
         return self.EXECUTABLE
     def set_EXECUTABLE(self, EXECUTABLE):
         self.EXECUTABLE = EXECUTABLE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ARGUMENTS is not None or
             self.EXECUTABLE is not None
         ):
             return True
         else:
             return False
@@ -28792,15 +28796,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IPAM_MADType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IPAM_MADType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IPAM_MADType'):
@@ -28886,15 +28890,15 @@
         return self.SYSTEM
     def set_SYSTEM(self, SYSTEM):
         self.SYSTEM = SYSTEM
     def get_USE_VMS_LOCATION(self):
         return self.USE_VMS_LOCATION
     def set_USE_VMS_LOCATION(self, USE_VMS_LOCATION):
         self.USE_VMS_LOCATION = USE_VMS_LOCATION
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DEBUG_LEVEL is not None or
             self.SYSTEM is not None or
             self.USE_VMS_LOCATION is not None
         ):
             return True
         else:
@@ -28911,15 +28915,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOGType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOGType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOGType'):
@@ -29009,15 +29013,15 @@
         return self.ARGUMENTS
     def set_ARGUMENTS(self, ARGUMENTS):
         self.ARGUMENTS = ARGUMENTS
     def get_EXECUTABLE(self):
         return self.EXECUTABLE
     def set_EXECUTABLE(self, EXECUTABLE):
         self.EXECUTABLE = EXECUTABLE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ARGUMENTS is not None or
             self.EXECUTABLE is not None
         ):
             return True
         else:
             return False
@@ -29033,15 +29037,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MARKET_MADType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MARKET_MADType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MARKET_MADType'):
@@ -29154,15 +29158,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_PUBLICType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_PUBLICType_patterns_, ))
                 result = False
         return result
     validate_PUBLICType_patterns_ = [['^([yY][eE][sS])$', '^([nN][oO])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.APP_ACTIONS is not None or
             self.NAME is not None or
             self.PUBLIC is not None or
             self.REQUIRED_ATTRS is not None or
             self.SUNSTONE_NAME is not None
         ):
@@ -29181,15 +29185,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MARKET_MAD_CONFType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MARKET_MAD_CONFType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MARKET_MAD_CONFType'):
@@ -29325,15 +29329,15 @@
         return self.LOG_RETENTION
     def set_LOG_RETENTION(self, LOG_RETENTION):
         self.LOG_RETENTION = LOG_RETENTION
     def get_XMLRPC_TIMEOUT_MS(self):
         return self.XMLRPC_TIMEOUT_MS
     def set_XMLRPC_TIMEOUT_MS(self, XMLRPC_TIMEOUT_MS):
         self.XMLRPC_TIMEOUT_MS = XMLRPC_TIMEOUT_MS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.BROADCAST_TIMEOUT_MS is not None or
             self.ELECTION_TIMEOUT_MS is not None or
             self.LIMIT_PURGE is not None or
             self.LOG_PURGE_TIMEOUT is not None or
             self.LOG_RETENTION is not None or
             self.XMLRPC_TIMEOUT_MS is not None
@@ -29353,15 +29357,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='RAFTType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='RAFTType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='RAFTType'):
@@ -29481,15 +29485,15 @@
         return self.ARGUMENTS
     def set_ARGUMENTS(self, ARGUMENTS):
         self.ARGUMENTS = ARGUMENTS
     def get_EXECUTABLE(self):
         return self.EXECUTABLE
     def set_EXECUTABLE(self, EXECUTABLE):
         self.EXECUTABLE = EXECUTABLE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ARGUMENTS is not None or
             self.EXECUTABLE is not None
         ):
             return True
         else:
             return False
@@ -29505,15 +29509,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TM_MADType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TM_MADType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TM_MADType'):
@@ -29665,15 +29669,15 @@
         return self.SHARED
     def set_SHARED(self, SHARED):
         self.SHARED = SHARED
     def get_TM_MAD_SYSTEM(self):
         return self.TM_MAD_SYSTEM
     def set_TM_MAD_SYSTEM(self, TM_MAD_SYSTEM):
         self.TM_MAD_SYSTEM = TM_MAD_SYSTEM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ALLOW_ORPHANS is not None or
             self.CLONE_TARGET is not None or
             self.CLONE_TARGET_SHARED is not None or
             self.CLONE_TARGET_SSH is not None or
             self.DISK_TYPE_SHARED is not None or
             self.DISK_TYPE_SSH is not None or
@@ -29701,15 +29705,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TM_MAD_CONFType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TM_MAD_CONFType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TM_MAD_CONFType'):
@@ -29909,15 +29913,15 @@
         return self.RESERVED
     def set_RESERVED(self, RESERVED):
         self.RESERVED = RESERVED
     def get_START(self):
         return self.START
     def set_START(self, START):
         self.START = START
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.RESERVED is not None or
             self.START is not None
         ):
             return True
         else:
             return False
@@ -29933,15 +29937,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VLAN_IDSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VLAN_IDSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VLAN_IDSType'):
@@ -30135,15 +30139,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_LIVE_RESIZEType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_LIVE_RESIZEType_patterns_, ))
                 result = False
         return result
     validate_LIVE_RESIZEType_patterns_ = [['^([yY][eE][sS])$', '^([nN][oO])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ARGUMENTS is not None or
             self.DEFAULT is not None or
             self.EXECUTABLE is not None or
             self.IMPORTED_VMS_ACTIONS is not None or
             self.NAME is not None or
             self.SUNSTONE_NAME is not None or
@@ -30168,15 +30172,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_MADType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_MADType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_MADType'):
@@ -30354,15 +30358,15 @@
         return self.RESERVED
     def set_RESERVED(self, RESERVED):
         self.RESERVED = RESERVED
     def get_START(self):
         return self.START
     def set_START(self, START):
         self.START = START
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.RESERVED is not None or
             self.START is not None
         ):
             return True
         else:
             return False
@@ -30378,15 +30382,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNC_PORTSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNC_PORTSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNC_PORTSType'):
@@ -30466,15 +30470,15 @@
         return self.BRIDGE_TYPE
     def set_BRIDGE_TYPE(self, BRIDGE_TYPE):
         self.BRIDGE_TYPE = BRIDGE_TYPE
     def get_NAME(self):
         return self.NAME
     def set_NAME(self, NAME):
         self.NAME = NAME
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.BRIDGE_TYPE is not None or
             self.NAME is not None
         ):
             return True
         else:
             return False
@@ -30490,15 +30494,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VN_MAD_CONFType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VN_MAD_CONFType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VN_MAD_CONFType'):
@@ -30572,15 +30576,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_START(self):
         return self.START
     def set_START(self, START):
         self.START = START
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.START is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VXLAN_IDSType', pretty_print=True):
@@ -30595,15 +30599,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VXLAN_IDSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VXLAN_IDSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VXLAN_IDSType'):
@@ -30715,15 +30719,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -30746,15 +30750,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType46')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType46', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType46'):
@@ -30907,15 +30911,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType', pretty_print=True):
@@ -30930,15 +30934,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATED_VMSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATED_VMSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATED_VMSType'):
@@ -31011,15 +31015,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType', pretty_print=True):
@@ -31034,15 +31038,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OUTDATED_VMSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OUTDATED_VMSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OUTDATED_VMSType'):
@@ -31115,15 +31119,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType', pretty_print=True):
@@ -31138,15 +31142,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATING_VMSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATING_VMSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATING_VMSType'):
@@ -31219,15 +31223,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType', pretty_print=True):
@@ -31242,15 +31246,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ERROR_VMSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ERROR_VMSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ERROR_VMSType'):
@@ -31337,15 +31341,15 @@
         self.RULE.insert(index, value)
     def replace_RULE_at(self, index, value):
         self.RULE[index] = value
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DESCRIPTION is not None or
             self.RULE or
             self.anytypeobjs_
         ):
             return True
         else:
@@ -31362,15 +31366,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType47')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType47', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType47'):
@@ -31456,15 +31460,15 @@
         return self.PROTOCOL
     def set_PROTOCOL(self, PROTOCOL):
         self.PROTOCOL = PROTOCOL
     def get_RULE_TYPE(self):
         return self.RULE_TYPE
     def set_RULE_TYPE(self, RULE_TYPE):
         self.RULE_TYPE = RULE_TYPE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.PROTOCOL is not None or
             self.RULE_TYPE is not None
         ):
             return True
         else:
             return False
@@ -31480,15 +31484,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='RULEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='RULEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='RULEType'):
@@ -31640,15 +31644,15 @@
         return self.HOURS
     def set_HOURS(self, HOURS):
         self.HOURS = HOURS
     def get_RHOURS(self):
         return self.RHOURS
     def set_RHOURS(self, RHOURS):
         self.RHOURS = RHOURS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VMID is not None or
             self.VMNAME is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
@@ -31676,15 +31680,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SHOWBACKType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SHOWBACKType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SHOWBACKType'):
@@ -31941,15 +31945,15 @@
         self.LOGIN_TOKEN.insert(index, value)
     def replace_LOGIN_TOKEN_at(self, index, value):
         self.LOGIN_TOKEN[index] = value
     def get_TEMPLATE(self):
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.GID is not None or
             self.GROUPS is not None or
             self.GNAME is not None or
             self.NAME is not None or
             self.PASSWORD is not None or
@@ -31973,15 +31977,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USERType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USERType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USERType'):
@@ -32140,15 +32144,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType', pretty_print=True):
@@ -32163,15 +32167,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUPSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUPSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUPSType'):
@@ -32247,15 +32251,15 @@
         return self.EXPIRATION_TIME
     def set_EXPIRATION_TIME(self, EXPIRATION_TIME):
         self.EXPIRATION_TIME = EXPIRATION_TIME
     def get_EGID(self):
         return self.EGID
     def set_EGID(self, EGID):
         self.EGID = EGID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.TOKEN is not None or
             self.EXPIRATION_TIME is not None or
             self.EGID is not None
         ):
             return True
         else:
@@ -32272,15 +32276,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOGIN_TOKENType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOGIN_TOKENType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOGIN_TOKENType'):
@@ -32388,15 +32392,15 @@
         return self.VM_QUOTA
     def set_VM_QUOTA(self, VM_QUOTA):
         self.VM_QUOTA = VM_QUOTA
     def get_IMAGE_QUOTA(self):
         return self.IMAGE_QUOTA
     def set_IMAGE_QUOTA(self, IMAGE_QUOTA):
         self.IMAGE_QUOTA = IMAGE_QUOTA
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.DATASTORE_QUOTA is not None or
             self.NETWORK_QUOTA is not None or
             self.VM_QUOTA is not None or
             self.IMAGE_QUOTA is not None
         ):
@@ -32415,15 +32419,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='QUOTASType48')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='QUOTASType48', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='QUOTASType48'):
@@ -32528,15 +32532,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType49', pretty_print=True):
@@ -32551,15 +32555,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType49')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType49', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType49'):
@@ -32645,15 +32649,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_SIZE_USED(self):
         return self.SIZE_USED
     def set_SIZE_USED(self, SIZE_USED):
         self.SIZE_USED = SIZE_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.IMAGES is not None or
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
@@ -32672,15 +32676,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType50')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType50', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType50'):
@@ -32793,15 +32797,15 @@
         self.NETWORK = NETWORK
     def add_NETWORK(self, value):
         self.NETWORK.append(value)
     def insert_NETWORK_at(self, index, value):
         self.NETWORK.insert(index, value)
     def replace_NETWORK_at(self, index, value):
         self.NETWORK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType51', pretty_print=True):
@@ -32816,15 +32820,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType51')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType51', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType51'):
@@ -32898,15 +32902,15 @@
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
     def get_LEASES_USED(self):
         return self.LEASES_USED
     def set_LEASES_USED(self, LEASES_USED):
         self.LEASES_USED = LEASES_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
@@ -32923,15 +32927,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType52')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType52', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType52'):
@@ -33015,15 +33019,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType53', pretty_print=True):
@@ -33038,15 +33042,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType53')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType53', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType53'):
@@ -33186,15 +33190,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_VMS_USED(self):
         return self.VMS_USED
     def set_VMS_USED(self, VMS_USED):
         self.VMS_USED = VMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.CPU_USED is not None or
             self.MEMORY is not None or
             self.MEMORY_USED is not None or
             self.RUNNING_CPU is not None or
             self.RUNNING_CPU_USED is not None or
@@ -33222,15 +33226,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType54')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType54', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType54'):
@@ -33433,15 +33437,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType55', pretty_print=True):
@@ -33456,15 +33460,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType55')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType55', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType55'):
@@ -33538,15 +33542,15 @@
         return self.RVMS
     def set_RVMS(self, RVMS):
         self.RVMS = RVMS
     def get_RVMS_USED(self):
         return self.RVMS_USED
     def set_RVMS_USED(self, RVMS_USED):
         self.RVMS_USED = RVMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
@@ -33563,15 +33567,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType56')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType56', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType56'):
@@ -33673,15 +33677,15 @@
         return self.VM_QUOTA
     def set_VM_QUOTA(self, VM_QUOTA):
         self.VM_QUOTA = VM_QUOTA
     def get_IMAGE_QUOTA(self):
         return self.IMAGE_QUOTA
     def set_IMAGE_QUOTA(self, IMAGE_QUOTA):
         self.IMAGE_QUOTA = IMAGE_QUOTA
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE_QUOTA is not None or
             self.NETWORK_QUOTA is not None or
             self.VM_QUOTA is not None or
             self.IMAGE_QUOTA is not None
         ):
             return True
@@ -33699,15 +33703,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DEFAULT_USER_QUOTASType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DEFAULT_USER_QUOTASType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DEFAULT_USER_QUOTASType'):
@@ -33802,15 +33806,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType57', pretty_print=True):
@@ -33825,15 +33829,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType57')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType57', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType57'):
@@ -33919,15 +33923,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_SIZE_USED(self):
         return self.SIZE_USED
     def set_SIZE_USED(self, SIZE_USED):
         self.SIZE_USED = SIZE_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.IMAGES is not None or
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
@@ -33946,15 +33950,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType58')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType58', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType58'):
@@ -34067,15 +34071,15 @@
         self.NETWORK = NETWORK
     def add_NETWORK(self, value):
         self.NETWORK.append(value)
     def insert_NETWORK_at(self, index, value):
         self.NETWORK.insert(index, value)
     def replace_NETWORK_at(self, index, value):
         self.NETWORK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType59', pretty_print=True):
@@ -34090,15 +34094,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType59')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType59', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType59'):
@@ -34172,15 +34176,15 @@
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
     def get_LEASES_USED(self):
         return self.LEASES_USED
     def set_LEASES_USED(self, LEASES_USED):
         self.LEASES_USED = LEASES_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
@@ -34197,15 +34201,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType60')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType60', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType60'):
@@ -34289,15 +34293,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType61', pretty_print=True):
@@ -34312,15 +34316,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType61')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType61', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType61'):
@@ -34460,15 +34464,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_VMS_USED(self):
         return self.VMS_USED
     def set_VMS_USED(self, VMS_USED):
         self.VMS_USED = VMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.CPU_USED is not None or
             self.MEMORY is not None or
             self.MEMORY_USED is not None or
             self.RUNNING_CPU is not None or
             self.RUNNING_CPU_USED is not None or
@@ -34496,15 +34500,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType62')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType62', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType62'):
@@ -34707,15 +34711,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType63', pretty_print=True):
@@ -34730,15 +34734,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType63')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType63', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType63'):
@@ -34812,15 +34816,15 @@
         return self.RVMS
     def set_RVMS(self, RVMS):
         self.RVMS = RVMS
     def get_RVMS_USED(self):
         return self.RVMS_USED
     def set_RVMS_USED(self, RVMS_USED):
         self.RVMS_USED = RVMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
@@ -34837,15 +34841,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType64')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType64', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType64'):
@@ -34938,15 +34942,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType65', pretty_print=True):
@@ -34961,15 +34965,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUPSType65')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUPSType65', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUPSType65'):
@@ -35045,15 +35049,15 @@
         return self.EXPIRATION_TIME
     def set_EXPIRATION_TIME(self, EXPIRATION_TIME):
         self.EXPIRATION_TIME = EXPIRATION_TIME
     def get_EGID(self):
         return self.EGID
     def set_EGID(self, EGID):
         self.EGID = EGID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.TOKEN is not None or
             self.EXPIRATION_TIME is not None or
             self.EGID is not None
         ):
             return True
         else:
@@ -35070,15 +35074,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOGIN_TOKENType66')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOGIN_TOKENType66', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOGIN_TOKENType66'):
@@ -35171,15 +35175,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType67', pretty_print=True):
@@ -35194,15 +35198,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType67')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType67', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType67'):
@@ -35288,15 +35292,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_SIZE_USED(self):
         return self.SIZE_USED
     def set_SIZE_USED(self, SIZE_USED):
         self.SIZE_USED = SIZE_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.IMAGES is not None or
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
@@ -35315,15 +35319,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType68')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType68', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType68'):
@@ -35436,15 +35440,15 @@
         self.NETWORK = NETWORK
     def add_NETWORK(self, value):
         self.NETWORK.append(value)
     def insert_NETWORK_at(self, index, value):
         self.NETWORK.insert(index, value)
     def replace_NETWORK_at(self, index, value):
         self.NETWORK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType69', pretty_print=True):
@@ -35459,15 +35463,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType69')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType69', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType69'):
@@ -35541,15 +35545,15 @@
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
     def get_LEASES_USED(self):
         return self.LEASES_USED
     def set_LEASES_USED(self, LEASES_USED):
         self.LEASES_USED = LEASES_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
@@ -35566,15 +35570,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType70')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType70', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType70'):
@@ -35658,15 +35662,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType71', pretty_print=True):
@@ -35681,15 +35685,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType71')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType71', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType71'):
@@ -35829,15 +35833,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_VMS_USED(self):
         return self.VMS_USED
     def set_VMS_USED(self, VMS_USED):
         self.VMS_USED = VMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.CPU_USED is not None or
             self.MEMORY is not None or
             self.MEMORY_USED is not None or
             self.RUNNING_CPU is not None or
             self.RUNNING_CPU_USED is not None or
@@ -35865,15 +35869,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType72')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType72', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType72'):
@@ -36076,15 +36080,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType73', pretty_print=True):
@@ -36099,15 +36103,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType73')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType73', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType73'):
@@ -36181,15 +36185,15 @@
         return self.RVMS
     def set_RVMS(self, RVMS):
         self.RVMS = RVMS
     def get_RVMS_USED(self):
         return self.RVMS_USED
     def set_RVMS_USED(self, RVMS_USED):
         self.RVMS_USED = RVMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
@@ -36206,15 +36210,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType74')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType74', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType74'):
@@ -36316,15 +36320,15 @@
         return self.VM_QUOTA
     def set_VM_QUOTA(self, VM_QUOTA):
         self.VM_QUOTA = VM_QUOTA
     def get_IMAGE_QUOTA(self):
         return self.IMAGE_QUOTA
     def set_IMAGE_QUOTA(self, IMAGE_QUOTA):
         self.IMAGE_QUOTA = IMAGE_QUOTA
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE_QUOTA is not None or
             self.NETWORK_QUOTA is not None or
             self.VM_QUOTA is not None or
             self.IMAGE_QUOTA is not None
         ):
             return True
@@ -36342,15 +36346,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DEFAULT_USER_QUOTASType75')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DEFAULT_USER_QUOTASType75', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DEFAULT_USER_QUOTASType75'):
@@ -36445,15 +36449,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORE_QUOTAType76', pretty_print=True):
@@ -36468,15 +36472,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORE_QUOTAType76')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORE_QUOTAType76', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORE_QUOTAType76'):
@@ -36562,15 +36566,15 @@
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
     def get_SIZE_USED(self):
         return self.SIZE_USED
     def set_SIZE_USED(self, SIZE_USED):
         self.SIZE_USED = SIZE_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.IMAGES is not None or
             self.IMAGES_USED is not None or
             self.SIZE is not None or
             self.SIZE_USED is not None
         ):
@@ -36589,15 +36593,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType77')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType77', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType77'):
@@ -36710,15 +36714,15 @@
         self.NETWORK = NETWORK
     def add_NETWORK(self, value):
         self.NETWORK.append(value)
     def insert_NETWORK_at(self, index, value):
         self.NETWORK.insert(index, value)
     def replace_NETWORK_at(self, index, value):
         self.NETWORK[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.NETWORK
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='NETWORK_QUOTAType78', pretty_print=True):
@@ -36733,15 +36737,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORK_QUOTAType78')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORK_QUOTAType78', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORK_QUOTAType78'):
@@ -36815,15 +36819,15 @@
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
     def get_LEASES_USED(self):
         return self.LEASES_USED
     def set_LEASES_USED(self, LEASES_USED):
         self.LEASES_USED = LEASES_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.LEASES is not None or
             self.LEASES_USED is not None
         ):
             return True
         else:
@@ -36840,15 +36844,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NETWORKType79')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NETWORKType79', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NETWORKType79'):
@@ -36932,15 +36936,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_VM(self):
         return self.VM
     def set_VM(self, VM):
         self.VM = VM
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VM is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VM_QUOTAType80', pretty_print=True):
@@ -36955,15 +36959,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VM_QUOTAType80')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VM_QUOTAType80', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VM_QUOTAType80'):
@@ -37103,15 +37107,15 @@
         return self.VMS
     def set_VMS(self, VMS):
         self.VMS = VMS
     def get_VMS_USED(self):
         return self.VMS_USED
     def set_VMS_USED(self, VMS_USED):
         self.VMS_USED = VMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.CPU_USED is not None or
             self.MEMORY is not None or
             self.MEMORY_USED is not None or
             self.RUNNING_CPU is not None or
             self.RUNNING_CPU_USED is not None or
@@ -37139,15 +37143,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType81')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType81', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType81'):
@@ -37350,15 +37354,15 @@
         self.IMAGE = IMAGE
     def add_IMAGE(self, value):
         self.IMAGE.append(value)
     def insert_IMAGE_at(self, index, value):
         self.IMAGE.insert(index, value)
     def replace_IMAGE_at(self, index, value):
         self.IMAGE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IMAGE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='IMAGE_QUOTAType82', pretty_print=True):
@@ -37373,15 +37377,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGE_QUOTAType82')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGE_QUOTAType82', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGE_QUOTAType82'):
@@ -37455,15 +37459,15 @@
         return self.RVMS
     def set_RVMS(self, RVMS):
         self.RVMS = RVMS
     def get_RVMS_USED(self):
         return self.RVMS_USED
     def set_RVMS_USED(self, RVMS_USED):
         self.RVMS_USED = RVMS_USED
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.RVMS is not None or
             self.RVMS_USED is not None
         ):
             return True
         else:
@@ -37480,15 +37484,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='IMAGEType83')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='IMAGEType83', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='IMAGEType83'):
@@ -37581,15 +37585,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='GROUPSType84', pretty_print=True):
@@ -37604,15 +37608,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GROUPSType84')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GROUPSType84', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GROUPSType84'):
@@ -37685,15 +37689,15 @@
         self.CLUSTER = CLUSTER
     def add_CLUSTER(self, value):
         self.CLUSTER.append(value)
     def insert_CLUSTER_at(self, index, value):
         self.CLUSTER.insert(index, value)
     def replace_CLUSTER_at(self, index, value):
         self.CLUSTER[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CLUSTER
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType85', pretty_print=True):
@@ -37708,15 +37712,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType85')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType85', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType85'):
@@ -37784,15 +37788,15 @@
         return self.ZONE_ID
     def set_ZONE_ID(self, ZONE_ID):
         self.ZONE_ID = ZONE_ID
     def get_CLUSTER_ID(self):
         return self.CLUSTER_ID
     def set_CLUSTER_ID(self, CLUSTER_ID):
         self.CLUSTER_ID = CLUSTER_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ZONE_ID is not None or
             self.CLUSTER_ID is not None
         ):
             return True
         else:
             return False
@@ -37808,15 +37812,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERType'):
@@ -37899,15 +37903,15 @@
         self.HOST = HOST
     def add_HOST(self, value):
         self.HOST.append(value)
     def insert_HOST_at(self, index, value):
         self.HOST.insert(index, value)
     def replace_HOST_at(self, index, value):
         self.HOST[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HOST
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HOSTSType86', pretty_print=True):
@@ -37922,15 +37926,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOSTSType86')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOSTSType86', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOSTSType86'):
@@ -37998,15 +38002,15 @@
         return self.ZONE_ID
     def set_ZONE_ID(self, ZONE_ID):
         self.ZONE_ID = ZONE_ID
     def get_HOST_ID(self):
         return self.HOST_ID
     def set_HOST_ID(self, HOST_ID):
         self.HOST_ID = HOST_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ZONE_ID is not None or
             self.HOST_ID is not None
         ):
             return True
         else:
             return False
@@ -38022,15 +38026,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HOSTType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HOSTType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HOSTType'):
@@ -38113,15 +38117,15 @@
         self.DATASTORE = DATASTORE
     def add_DATASTORE(self, value):
         self.DATASTORE.append(value)
     def insert_DATASTORE_at(self, index, value):
         self.DATASTORE.insert(index, value)
     def replace_DATASTORE_at(self, index, value):
         self.DATASTORE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DATASTORE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='DATASTORESType87', pretty_print=True):
@@ -38136,15 +38140,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTORESType87')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTORESType87', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTORESType87'):
@@ -38212,15 +38216,15 @@
         return self.ZONE_ID
     def set_ZONE_ID(self, ZONE_ID):
         self.ZONE_ID = ZONE_ID
     def get_DATASTORE_ID(self):
         return self.DATASTORE_ID
     def set_DATASTORE_ID(self, DATASTORE_ID):
         self.DATASTORE_ID = DATASTORE_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ZONE_ID is not None or
             self.DATASTORE_ID is not None
         ):
             return True
         else:
             return False
@@ -38236,15 +38240,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DATASTOREType88')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DATASTOREType88', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DATASTOREType88'):
@@ -38327,15 +38331,15 @@
         self.VNET = VNET
     def add_VNET(self, value):
         self.VNET.append(value)
     def insert_VNET_at(self, index, value):
         self.VNET.insert(index, value)
     def replace_VNET_at(self, index, value):
         self.VNET[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VNET
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VNETSType89', pretty_print=True):
@@ -38350,15 +38354,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNETSType89')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNETSType89', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNETSType89'):
@@ -38426,15 +38430,15 @@
         return self.ZONE_ID
     def set_ZONE_ID(self, ZONE_ID):
         self.ZONE_ID = ZONE_ID
     def get_VNET_ID(self):
         return self.VNET_ID
     def set_VNET_ID(self, VNET_ID):
         self.VNET_ID = VNET_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ZONE_ID is not None or
             self.VNET_ID is not None
         ):
             return True
         else:
             return False
@@ -38450,15 +38454,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNETType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNETType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNETType'):
@@ -38580,15 +38584,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -38611,15 +38615,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType90')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType90', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType90'):
@@ -38781,15 +38785,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -38807,15 +38811,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType91')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType91', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType91'):
@@ -38918,15 +38922,15 @@
         self.ROLE = ROLE
     def add_ROLE(self, value):
         self.ROLE.append(value)
     def insert_ROLE_at(self, index, value):
         self.ROLE.insert(index, value)
     def replace_ROLE_at(self, index, value):
         self.ROLE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ROLE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ROLESType', pretty_print=True):
@@ -38941,15 +38945,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ROLESType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ROLESType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ROLESType'):
@@ -39035,15 +39039,15 @@
         return self.NAME
     def set_NAME(self, NAME):
         self.NAME = NAME
     def get_POLICY(self):
         return self.POLICY
     def set_POLICY(self, POLICY):
         self.POLICY = POLICY
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HOST_AFFINED is not None or
             self.HOST_ANTI_AFFINED is not None or
             self.ID is not None or
             self.NAME is not None or
             self.POLICY is not None
         ):
@@ -39062,15 +39066,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ROLEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ROLEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ROLEType'):
@@ -39270,15 +39274,15 @@
         return self.USER_TEMPLATE
     def set_USER_TEMPLATE(self, USER_TEMPLATE):
         self.USER_TEMPLATE = USER_TEMPLATE
     def get_HISTORY_RECORDS(self):
         return self.HISTORY_RECORDS
     def set_HISTORY_RECORDS(self, HISTORY_RECORDS):
         self.HISTORY_RECORDS = HISTORY_RECORDS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -39309,15 +39313,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMType92')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMType92', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMType92'):
@@ -39575,15 +39579,15 @@
         self.NIC.insert(index, value)
     def replace_NIC_at(self, index, value):
         self.NIC[index] = value
     def get_GRAPHICS(self):
         return self.GRAPHICS
     def set_GRAPHICS(self, GRAPHICS):
         self.GRAPHICS = GRAPHICS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.MEMORY is not None or
             self.DISK or
             self.NIC or
             self.GRAPHICS is not None
         ):
@@ -39602,15 +39606,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType93')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType93', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType93'):
@@ -39704,15 +39708,15 @@
         else:
             return GRAPHICS(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='GRAPHICS', pretty_print=True):
@@ -39727,15 +39731,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='GRAPHICS')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='GRAPHICS', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='GRAPHICS'):
         pass
@@ -39800,15 +39804,15 @@
         return self.VCENTER_INSTANCE_ID
     def set_VCENTER_INSTANCE_ID(self, VCENTER_INSTANCE_ID):
         self.VCENTER_INSTANCE_ID = VCENTER_INSTANCE_ID
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VCENTER_DS_REF is not None or
             self.VCENTER_INSTANCE_ID is not None or
             self.anytypeobjs_
         ):
             return True
         else:
@@ -39825,15 +39829,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DISKType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DISKType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DISKType'):
@@ -39935,15 +39939,15 @@
         return self.VCENTER_NET_REF
     def set_VCENTER_NET_REF(self, VCENTER_NET_REF):
         self.VCENTER_NET_REF = VCENTER_NET_REF
     def get_VCENTER_PORTGROUP_TYPE(self):
         return self.VCENTER_PORTGROUP_TYPE
     def set_VCENTER_PORTGROUP_TYPE(self, VCENTER_PORTGROUP_TYPE):
         self.VCENTER_PORTGROUP_TYPE = VCENTER_PORTGROUP_TYPE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.anytypeobjs_ or
             self.VCENTER_INSTANCE_ID is not None or
             self.VCENTER_NET_REF is not None or
             self.VCENTER_PORTGROUP_TYPE is not None
         ):
             return True
@@ -39961,15 +39965,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NICType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NICType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NICType'):
@@ -40063,15 +40067,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.anytypeobjs_
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='MONITORINGType94', pretty_print=True):
@@ -40086,15 +40090,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType94')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType94', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType94'):
@@ -40157,15 +40161,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.anytypeobjs_
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='USER_TEMPLATEType', pretty_print=True):
@@ -40180,15 +40184,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USER_TEMPLATEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USER_TEMPLATEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USER_TEMPLATEType'):
@@ -40258,15 +40262,15 @@
         self.HISTORY = HISTORY
     def add_HISTORY(self, value):
         self.HISTORY.append(value)
     def insert_HISTORY_at(self, index, value):
         self.HISTORY.insert(index, value)
     def replace_HISTORY_at(self, index, value):
         self.HISTORY[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HISTORY
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORY_RECORDSType', pretty_print=True):
@@ -40281,15 +40285,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORY_RECORDSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORY_RECORDSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORY_RECORDSType'):
@@ -40399,15 +40403,15 @@
         return self.TM_MAD
     def set_TM_MAD(self, TM_MAD):
         self.TM_MAD = TM_MAD
     def get_ACTION(self):
         return self.ACTION
     def set_ACTION(self, ACTION):
         self.ACTION = ACTION
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OID is not None or
             self.SEQ is not None or
             self.HOSTNAME is not None or
             self.HID is not None or
             self.CID is not None or
             self.DS_ID is not None or
@@ -40430,15 +40434,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORYType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORYType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORYType'):
@@ -40600,15 +40604,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -40626,15 +40630,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType95')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType95', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType95'):
@@ -40776,15 +40780,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -40807,15 +40811,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType96')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType96', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType96'):
@@ -40979,15 +40983,15 @@
         return self.VCENTER_TEMPLATE_REF
     def set_VCENTER_TEMPLATE_REF(self, VCENTER_TEMPLATE_REF):
         self.VCENTER_TEMPLATE_REF = VCENTER_TEMPLATE_REF
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VCENTER_CCR_REF is not None or
             self.VCENTER_INSTANCE_ID is not None or
             self.VCENTER_TEMPLATE_REF is not None or
             self.anytypeobjs_
         ):
             return True
@@ -41005,15 +41009,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType97')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType97', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType97'):
@@ -41153,15 +41157,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -41184,15 +41188,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType98')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType98', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType98'):
@@ -41354,15 +41358,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -41380,15 +41384,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType99')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType99', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType99'):
@@ -41593,15 +41597,15 @@
         return self.VCENTER_VMWARETOOLS_VERSION_STATUS
     def set_VCENTER_VMWARETOOLS_VERSION_STATUS(self, VCENTER_VMWARETOOLS_VERSION_STATUS):
         self.VCENTER_VMWARETOOLS_VERSION_STATUS = VCENTER_VMWARETOOLS_VERSION_STATUS
     def get_VCENTER_VM_NAME(self):
         return self.VCENTER_VM_NAME
     def set_VCENTER_VM_NAME(self, VCENTER_VM_NAME):
         self.VCENTER_VM_NAME = VCENTER_VM_NAME
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.CPU is not None or
             self.DISKRDBYTES is not None or
             self.DISKRDIOPS is not None or
             self.DISKWRBYTES is not None or
             self.DISKWRIOPS is not None or
             self.DISK_SIZE or
@@ -41633,15 +41637,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='MONITORINGType100')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='MONITORINGType100', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='MONITORINGType100'):
@@ -41879,15 +41883,15 @@
         return self.ID
     def set_ID(self, ID):
         self.ID = ID
     def get_SIZE(self):
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.SIZE is not None
         ):
             return True
         else:
             return False
@@ -41903,15 +41907,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DISK_SIZEType101')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DISK_SIZEType101', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DISK_SIZEType101'):
@@ -42294,15 +42298,15 @@
         return self.VROUTER_KEEPALIVED_ID
     def set_VROUTER_KEEPALIVED_ID(self, VROUTER_KEEPALIVED_ID):
         self.VROUTER_KEEPALIVED_ID = VROUTER_KEEPALIVED_ID
     def get_VROUTER_KEEPALIVED_PASSWORD(self):
         return self.VROUTER_KEEPALIVED_PASSWORD
     def set_VROUTER_KEEPALIVED_PASSWORD(self, VROUTER_KEEPALIVED_PASSWORD):
         self.VROUTER_KEEPALIVED_PASSWORD = VROUTER_KEEPALIVED_PASSWORD
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.AUTOMATIC_DS_REQUIREMENTS is not None or
             self.AUTOMATIC_NIC_REQUIREMENTS is not None or
             self.AUTOMATIC_REQUIREMENTS is not None or
             self.CLONING_TEMPLATE_ID is not None or
             self.CONTEXT is not None or
             self.CPU is not None or
@@ -42358,15 +42362,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType102')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType102', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType102'):
@@ -42824,15 +42828,15 @@
         else:
             return CONTEXT(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='CONTEXT', pretty_print=True):
@@ -42847,15 +42851,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CONTEXT')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CONTEXT', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CONTEXT'):
         pass
@@ -42900,15 +42904,15 @@
         else:
             return FEATURES(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='FEATURES', pretty_print=True):
@@ -42923,15 +42927,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='FEATURES')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='FEATURES', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='FEATURES'):
         pass
@@ -42976,15 +42980,15 @@
         else:
             return HYPERV_OPTIONS(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='HYPERV_OPTIONS', pretty_print=True):
@@ -42999,15 +43003,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HYPERV_OPTIONS')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HYPERV_OPTIONS', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HYPERV_OPTIONS'):
         pass
@@ -43052,15 +43056,15 @@
         else:
             return INPUT(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='INPUT', pretty_print=True):
@@ -43075,15 +43079,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='INPUT')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='INPUT', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='INPUT'):
         pass
@@ -43128,15 +43132,15 @@
         else:
             return NIC_DEFAULT(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='NIC_DEFAULT', pretty_print=True):
@@ -43151,15 +43155,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NIC_DEFAULT')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NIC_DEFAULT', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NIC_DEFAULT'):
         pass
@@ -43204,15 +43208,15 @@
         else:
             return NUMA_NODE(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='NUMA_NODE', pretty_print=True):
@@ -43227,15 +43231,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NUMA_NODE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NUMA_NODE', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NUMA_NODE'):
         pass
@@ -43280,15 +43284,15 @@
         else:
             return OS(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='OS', pretty_print=True):
@@ -43303,15 +43307,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OS')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OS', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OS'):
         pass
@@ -43356,15 +43360,15 @@
         else:
             return PCI(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='PCI', pretty_print=True):
@@ -43379,15 +43383,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PCI')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PCI', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PCI'):
         pass
@@ -43432,15 +43436,15 @@
         else:
             return RAW(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='RAW', pretty_print=True):
@@ -43455,15 +43459,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='RAW')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='RAW', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='RAW'):
         pass
@@ -43508,15 +43512,15 @@
         else:
             return SECURITY_GROUP_RULE(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='SECURITY_GROUP_RULE', pretty_print=True):
@@ -43531,15 +43535,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SECURITY_GROUP_RULE')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SECURITY_GROUP_RULE', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SECURITY_GROUP_RULE'):
         pass
@@ -43584,15 +43588,15 @@
         else:
             return SPICE_OPTIONS(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='SPICE_OPTIONS', pretty_print=True):
@@ -43607,15 +43611,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SPICE_OPTIONS')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SPICE_OPTIONS', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SPICE_OPTIONS'):
         pass
@@ -43660,15 +43664,15 @@
         else:
             return TOPOLOGY(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='TOPOLOGY', pretty_print=True):
@@ -43683,15 +43687,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TOPOLOGY')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TOPOLOGY', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TOPOLOGY'):
         pass
@@ -43736,15 +43740,15 @@
         else:
             return VMGROUP(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='VMGROUP', pretty_print=True):
@@ -43759,15 +43763,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMGROUP')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMGROUP', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMGROUP'):
         pass
@@ -43832,15 +43836,15 @@
         return self.VCENTER_INSTANCE_ID
     def set_VCENTER_INSTANCE_ID(self, VCENTER_INSTANCE_ID):
         self.VCENTER_INSTANCE_ID = VCENTER_INSTANCE_ID
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VCENTER_DS_REF is not None or
             self.VCENTER_INSTANCE_ID is not None or
             self.anytypeobjs_
         ):
             return True
         else:
@@ -43857,15 +43861,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='DISKType103')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='DISKType103', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='DISKType103'):
@@ -43967,15 +43971,15 @@
         return self.VCENTER_NET_REF
     def set_VCENTER_NET_REF(self, VCENTER_NET_REF):
         self.VCENTER_NET_REF = VCENTER_NET_REF
     def get_VCENTER_PORTGROUP_TYPE(self):
         return self.VCENTER_PORTGROUP_TYPE
     def set_VCENTER_PORTGROUP_TYPE(self, VCENTER_PORTGROUP_TYPE):
         self.VCENTER_PORTGROUP_TYPE = VCENTER_PORTGROUP_TYPE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.anytypeobjs_ or
             self.VCENTER_INSTANCE_ID is not None or
             self.VCENTER_NET_REF is not None or
             self.VCENTER_PORTGROUP_TYPE is not None
         ):
             return True
@@ -43993,15 +43997,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NICType104')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NICType104', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NICType104'):
@@ -44131,15 +44135,15 @@
         return self.VCENTER_NET_REF
     def set_VCENTER_NET_REF(self, VCENTER_NET_REF):
         self.VCENTER_NET_REF = VCENTER_NET_REF
     def get_VCENTER_PORTGROUP_TYPE(self):
         return self.VCENTER_PORTGROUP_TYPE
     def set_VCENTER_PORTGROUP_TYPE(self, VCENTER_PORTGROUP_TYPE):
         self.VCENTER_PORTGROUP_TYPE = VCENTER_PORTGROUP_TYPE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ALIAS_ID is not None or
             self.PARENT is not None or
             self.PARENT_ID is not None or
             self.anytypeobjs_ or
             self.VCENTER_INSTANCE_ID is not None or
             self.VCENTER_NET_REF is not None or
@@ -44160,15 +44164,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='NIC_ALIASType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='NIC_ALIASType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='NIC_ALIASType'):
@@ -44338,15 +44342,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_WARNING(self):
         return self.WARNING
     def set_WARNING(self, WARNING):
         self.WARNING = WARNING
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ACTION is not None or
             self.ARGS is not None or
             self.DAYS is not None or
             self.END_TYPE is not None or
             self.END_VALUE is not None or
             self.ID is not None or
@@ -44369,15 +44373,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SCHED_ACTIONType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SCHED_ACTIONType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SCHED_ACTIONType'):
@@ -44557,15 +44561,15 @@
         return self.SYSTEM_DISK_SIZE
     def set_SYSTEM_DISK_SIZE(self, SYSTEM_DISK_SIZE):
         self.SYSTEM_DISK_SIZE = SYSTEM_DISK_SIZE
     def get_TIME(self):
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ACTION is not None or
             self.ACTIVE is not None or
             self.HYPERVISOR_ID is not None or
             self.NAME is not None or
             self.SNAPSHOT_ID is not None or
             self.SYSTEM_DISK_SIZE is not None or
@@ -44586,15 +44590,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType105')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType105', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType105'):
@@ -44738,15 +44742,15 @@
         return self.VCENTER_INSTANCE_ID
     def set_VCENTER_INSTANCE_ID(self, VCENTER_INSTANCE_ID):
         self.VCENTER_INSTANCE_ID = VCENTER_INSTANCE_ID
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VCENTER_CCR_REF is not None or
             self.VCENTER_DS_REF is not None or
             self.VCENTER_INSTANCE_ID is not None or
             self.anytypeobjs_
         ):
             return True
@@ -44764,15 +44768,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='USER_TEMPLATEType106')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='USER_TEMPLATEType106', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='USER_TEMPLATEType106'):
@@ -44873,15 +44877,15 @@
         self.HISTORY = HISTORY
     def add_HISTORY(self, value):
         self.HISTORY.append(value)
     def insert_HISTORY_at(self, index, value):
         self.HISTORY.insert(index, value)
     def replace_HISTORY_at(self, index, value):
         self.HISTORY[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.HISTORY
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='HISTORY_RECORDSType107', pretty_print=True):
@@ -44896,15 +44900,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORY_RECORDSType107')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORY_RECORDSType107', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORY_RECORDSType107'):
@@ -45080,15 +45084,15 @@
         return self.GID
     def set_GID(self, GID):
         self.GID = GID
     def get_REQUEST_ID(self):
         return self.REQUEST_ID
     def set_REQUEST_ID(self, REQUEST_ID):
         self.REQUEST_ID = REQUEST_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OID is not None or
             self.SEQ is not None or
             self.HOSTNAME is not None or
             self.HID is not None or
             self.CID is not None or
             self.STIME is not None or
@@ -45122,15 +45126,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='HISTORYType108')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='HISTORYType108', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='HISTORYType108'):
@@ -45417,15 +45421,15 @@
         self.SNAPSHOT = SNAPSHOT
     def add_SNAPSHOT(self, value):
         self.SNAPSHOT.append(value)
     def insert_SNAPSHOT_at(self, index, value):
         self.SNAPSHOT.insert(index, value)
     def replace_SNAPSHOT_at(self, index, value):
         self.SNAPSHOT[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ALLOW_ORPHANS is not None or
             self.CURRENT_BASE is not None or
             self.DISK_ID is not None or
             self.NEXT_SNAPSHOT is not None or
             self.SNAPSHOT
         ):
@@ -45444,15 +45448,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTSType109')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTSType109', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTSType109'):
@@ -45590,15 +45594,15 @@
         return self.PARENT
     def set_PARENT(self, PARENT):
         self.PARENT = PARENT
     def get_SIZE(self):
         return self.SIZE
     def set_SIZE(self, SIZE):
         self.SIZE = SIZE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ACTIVE is not None or
             self.CHILDREN is not None or
             self.DATE is not None or
             self.ID is not None or
             self.NAME is not None or
             self.PARENT is not None or
@@ -45619,15 +45623,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SNAPSHOTType110')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SNAPSHOTType110', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SNAPSHOTType110'):
@@ -45757,15 +45761,15 @@
         return self.BACKUP_CONFIG
     def set_BACKUP_CONFIG(self, BACKUP_CONFIG):
         self.BACKUP_CONFIG = BACKUP_CONFIG
     def get_BACKUP_IDS(self):
         return self.BACKUP_IDS
     def set_BACKUP_IDS(self, BACKUP_IDS):
         self.BACKUP_IDS = BACKUP_IDS
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.BACKUP_CONFIG is not None or
             self.BACKUP_IDS is not None
         ):
             return True
         else:
             return False
@@ -45781,15 +45785,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUPSType111')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUPSType111', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUPSType111'):
@@ -45907,15 +45911,15 @@
         return self.LAST_INCREMENT_ID
     def set_LAST_INCREMENT_ID(self, LAST_INCREMENT_ID):
         self.LAST_INCREMENT_ID = LAST_INCREMENT_ID
     def get_MODE(self):
         return self.MODE
     def set_MODE(self, MODE):
         self.MODE = MODE
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.BACKUP_VOLATILE is not None or
             self.FS_FREEZE is not None or
             self.INCREMENTAL_BACKUP_ID is not None or
             self.KEEP_LAST is not None or
             self.LAST_BACKUP_ID is not None or
             self.LAST_BACKUP_SIZE is not None or
@@ -45938,15 +45942,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_CONFIGType112')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_CONFIGType112', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_CONFIGType112'):
@@ -46099,15 +46103,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='BACKUP_IDSType113', pretty_print=True):
@@ -46122,15 +46126,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='BACKUP_IDSType113')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='BACKUP_IDSType113', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='BACKUP_IDSType113'):
@@ -46350,15 +46354,15 @@
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
     def get_AR_POOL(self):
         return self.AR_POOL
     def set_AR_POOL(self, AR_POOL):
         self.AR_POOL = AR_POOL
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.UID is not None or
             self.GID is not None or
             self.UNAME is not None or
             self.GNAME is not None or
             self.NAME is not None or
@@ -46399,15 +46403,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VNETType114')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VNETType114', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VNETType114'):
@@ -46763,15 +46767,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -46794,15 +46798,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType115')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType115', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType115'):
@@ -46955,15 +46959,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType116', pretty_print=True):
@@ -46978,15 +46982,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType116')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType116', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType116'):
@@ -47059,15 +47063,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VROUTERSType', pretty_print=True):
@@ -47082,15 +47086,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VROUTERSType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VROUTERSType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VROUTERSType'):
@@ -47163,15 +47167,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType117', pretty_print=True):
@@ -47186,15 +47190,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATED_VMSType117')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATED_VMSType117', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATED_VMSType117'):
@@ -47267,15 +47271,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType118', pretty_print=True):
@@ -47290,15 +47294,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OUTDATED_VMSType118')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OUTDATED_VMSType118', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OUTDATED_VMSType118'):
@@ -47371,15 +47375,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType119', pretty_print=True):
@@ -47394,15 +47398,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATING_VMSType119')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATING_VMSType119', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATING_VMSType119'):
@@ -47475,15 +47479,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType120', pretty_print=True):
@@ -47498,15 +47502,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ERROR_VMSType120')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ERROR_VMSType120', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ERROR_VMSType120'):
@@ -47579,15 +47583,15 @@
         self.AR = AR
     def add_AR(self, value):
         self.AR.append(value)
     def insert_AR_at(self, index, value):
         self.AR.insert(index, value)
     def replace_AR_at(self, index, value):
         self.AR[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.AR
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='AR_POOLType', pretty_print=True):
@@ -47602,15 +47606,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='AR_POOLType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='AR_POOLType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='AR_POOLType'):
@@ -47726,15 +47730,15 @@
         return self.ULA_PREFIX
     def set_ULA_PREFIX(self, ULA_PREFIX):
         self.ULA_PREFIX = ULA_PREFIX
     def get_VN_MAD(self):
         return self.VN_MAD
     def set_VN_MAD(self, VN_MAD):
         self.VN_MAD = VN_MAD
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ALLOCATED is not None or
             self.AR_ID is not None or
             self.GLOBAL_PREFIX is not None or
             self.IP is not None or
             self.MAC is not None or
             self.PARENT_NETWORK_AR_ID is not None or
@@ -47758,15 +47762,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ARType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ARType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ARType'):
@@ -47938,15 +47942,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -47964,15 +47968,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType121')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType121', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType121'):
@@ -48114,15 +48118,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -48145,15 +48149,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType122')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType122', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType122'):
@@ -48306,15 +48310,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='CLUSTERSType123', pretty_print=True):
@@ -48329,15 +48333,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='CLUSTERSType123')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='CLUSTERSType123', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='CLUSTERSType123'):
@@ -48410,15 +48414,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VROUTERSType124', pretty_print=True):
@@ -48433,15 +48437,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VROUTERSType124')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VROUTERSType124', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VROUTERSType124'):
@@ -48514,15 +48518,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATED_VMSType125', pretty_print=True):
@@ -48537,15 +48541,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATED_VMSType125')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATED_VMSType125', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATED_VMSType125'):
@@ -48618,15 +48622,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='OUTDATED_VMSType126', pretty_print=True):
@@ -48641,15 +48645,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='OUTDATED_VMSType126')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='OUTDATED_VMSType126', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='OUTDATED_VMSType126'):
@@ -48722,15 +48726,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='UPDATING_VMSType127', pretty_print=True):
@@ -48745,15 +48749,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='UPDATING_VMSType127')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='UPDATING_VMSType127', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='UPDATING_VMSType127'):
@@ -48826,15 +48830,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='ERROR_VMSType128', pretty_print=True):
@@ -48849,15 +48853,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ERROR_VMSType128')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ERROR_VMSType128', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ERROR_VMSType128'):
@@ -49019,15 +49023,15 @@
         return self.VCENTER_TEMPLATE_REF
     def set_VCENTER_TEMPLATE_REF(self, VCENTER_TEMPLATE_REF):
         self.VCENTER_TEMPLATE_REF = VCENTER_TEMPLATE_REF
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.DNS is not None or
             self.GATEWAY is not None or
             self.GATEWAY6 is not None or
             self.GUEST_MTU is not None or
             self.IP6_METHOD is not None or
             self.IP6_METRIC is not None or
@@ -49058,15 +49062,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType129')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType129', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType129'):
@@ -49297,15 +49301,15 @@
         self.AR = AR
     def add_AR(self, value):
         self.AR.append(value)
     def insert_AR_at(self, index, value):
         self.AR.insert(index, value)
     def replace_AR_at(self, index, value):
         self.AR[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.AR
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='AR_POOLType130', pretty_print=True):
@@ -49320,15 +49324,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='AR_POOLType130')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='AR_POOLType130', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='AR_POOLType130'):
@@ -49510,15 +49514,15 @@
         return self.USED_LEASES
     def set_USED_LEASES(self, USED_LEASES):
         self.USED_LEASES = USED_LEASES
     def get_LEASES(self):
         return self.LEASES
     def set_LEASES(self, LEASES):
         self.LEASES = LEASES
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.AR_ID is not None or
             self.GLOBAL_PREFIX is not None or
             self.IP is not None or
             self.MAC is not None or
             self.PARENT_NETWORK_AR_ID is not None or
             self.SIZE is not None or
@@ -49553,15 +49557,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ARType131')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ARType131', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ARType131'):
@@ -49832,15 +49836,15 @@
         self.LEASE = LEASE
     def add_LEASE(self, value):
         self.LEASE.append(value)
     def insert_LEASE_at(self, index, value):
         self.LEASE.insert(index, value)
     def replace_LEASE_at(self, index, value):
         self.LEASE[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LEASE
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='LEASESType', pretty_print=True):
@@ -49855,15 +49859,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LEASESType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LEASESType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LEASESType'):
@@ -49973,15 +49977,15 @@
         return self.VNET
     def set_VNET(self, VNET):
         self.VNET = VNET
     def get_VROUTER(self):
         return self.VROUTER
     def set_VROUTER(self, VROUTER):
         self.VROUTER = VROUTER
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.IP is not None or
             self.IP6 is not None or
             self.IP6_GLOBAL is not None or
             self.IP6_LINK is not None or
             self.IP6_ULA is not None or
             self.MAC is not None or
@@ -50004,15 +50008,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LEASEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LEASEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LEASEType'):
@@ -50174,15 +50178,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -50200,15 +50204,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType132')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType132', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType132'):
@@ -50350,15 +50354,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -50381,15 +50385,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType133')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType133', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType133'):
@@ -50541,15 +50545,15 @@
         return self.VN_MAD
     def set_VN_MAD(self, VN_MAD):
         self.VN_MAD = VN_MAD
     def get_anytypeobjs_(self): return self.anytypeobjs_
     def set_anytypeobjs_(self, anytypeobjs_): self.anytypeobjs_ = anytypeobjs_
     def add_anytypeobjs_(self, value): self.anytypeobjs_.append(value)
     def insert_anytypeobjs_(self, index, value): self._anytypeobjs_[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.VN_MAD is not None or
             self.anytypeobjs_
         ):
             return True
         else:
             return False
@@ -50565,15 +50569,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType134')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType134', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType134'):
@@ -50693,15 +50697,15 @@
         return self.OTHER_M
     def set_OTHER_M(self, OTHER_M):
         self.OTHER_M = OTHER_M
     def get_OTHER_A(self):
         return self.OTHER_A
     def set_OTHER_A(self, OTHER_A):
         self.OTHER_A = OTHER_A
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.OWNER_U is not None or
             self.OWNER_M is not None or
             self.OWNER_A is not None or
             self.GROUP_U is not None or
             self.GROUP_M is not None or
             self.GROUP_A is not None or
@@ -50724,15 +50728,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='PERMISSIONSType135')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='PERMISSIONSType135', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='PERMISSIONSType135'):
@@ -50894,15 +50898,15 @@
         return self.TIME
     def set_TIME(self, TIME):
         self.TIME = TIME
     def get_REQ_ID(self):
         return self.REQ_ID
     def set_REQ_ID(self, REQ_ID):
         self.REQ_ID = REQ_ID
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.LOCKED is not None or
             self.OWNER is not None or
             self.TIME is not None or
             self.REQ_ID is not None
         ):
             return True
@@ -50920,15 +50924,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='LOCKType136')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='LOCKType136', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='LOCKType136'):
@@ -51031,15 +51035,15 @@
         self.ID = ID
     def add_ID(self, value):
         self.ID.append(value)
     def insert_ID_at(self, index, value):
         self.ID.insert(index, value)
     def replace_ID_at(self, index, value):
         self.ID[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='VMSType137', pretty_print=True):
@@ -51054,15 +51058,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='VMSType137')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='VMSType137', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='VMSType137'):
@@ -51150,15 +51154,15 @@
         return self.TEMPLATE
     def set_TEMPLATE(self, TEMPLATE):
         self.TEMPLATE = TEMPLATE
     def get_SERVER_POOL(self):
         return self.SERVER_POOL
     def set_SERVER_POOL(self, SERVER_POOL):
         self.SERVER_POOL = SERVER_POOL
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ID is not None or
             self.NAME is not None or
             self.STATE is not None or
             self.TEMPLATE is not None or
             self.SERVER_POOL is not None
         ):
@@ -51177,15 +51181,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ZONEType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ZONEType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ZONEType'):
@@ -51285,15 +51289,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ENDPOINT(self):
         return self.ENDPOINT
     def set_ENDPOINT(self, ENDPOINT):
         self.ENDPOINT = ENDPOINT
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ENDPOINT is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType138', pretty_print=True):
@@ -51308,15 +51312,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType138')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType138', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType138'):
@@ -51389,15 +51393,15 @@
         self.SERVER = SERVER
     def add_SERVER(self, value):
         self.SERVER.append(value)
     def insert_SERVER_at(self, index, value):
         self.SERVER.insert(index, value)
     def replace_SERVER_at(self, index, value):
         self.SERVER[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.SERVER
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVER_POOLType', pretty_print=True):
@@ -51412,15 +51416,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SERVER_POOLType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SERVER_POOLType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SERVER_POOLType'):
@@ -51494,15 +51498,15 @@
         return self.ID
     def set_ID(self, ID):
         self.ID = ID
     def get_NAME(self):
         return self.NAME
     def set_NAME(self, NAME):
         self.NAME = NAME
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ENDPOINT is not None or
             self.ID is not None or
             self.NAME is not None
         ):
             return True
         else:
@@ -51519,15 +51523,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SERVERType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SERVERType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SERVERType'):
@@ -51611,15 +51615,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_ENDPOINT(self):
         return self.ENDPOINT
     def set_ENDPOINT(self, ENDPOINT):
         self.ENDPOINT = ENDPOINT
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ENDPOINT is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='TEMPLATEType139', pretty_print=True):
@@ -51634,15 +51638,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='TEMPLATEType139')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='TEMPLATEType139', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='TEMPLATEType139'):
@@ -51715,15 +51719,15 @@
         self.SERVER = SERVER
     def add_SERVER(self, value):
         self.SERVER.append(value)
     def insert_SERVER_at(self, index, value):
         self.SERVER.insert(index, value)
     def replace_SERVER_at(self, index, value):
         self.SERVER[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.SERVER
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_=' xmlns:None="http://opennebula.org/XMLSchema" ', name_='SERVER_POOLType140', pretty_print=True):
@@ -51738,15 +51742,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SERVER_POOLType140')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SERVER_POOLType140', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SERVER_POOLType140'):
@@ -51856,15 +51860,15 @@
         return self.LOG_INDEX
     def set_LOG_INDEX(self, LOG_INDEX):
         self.LOG_INDEX = LOG_INDEX
     def get_FEDLOG_INDEX(self):
         return self.FEDLOG_INDEX
     def set_FEDLOG_INDEX(self, FEDLOG_INDEX):
         self.FEDLOG_INDEX = FEDLOG_INDEX
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ENDPOINT is not None or
             self.ID is not None or
             self.NAME is not None or
             self.STATE is not None or
             self.TERM is not None or
             self.VOTEDFOR is not None or
@@ -51887,15 +51891,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='SERVERType141')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='SERVERType141', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='SERVERType141'):
```

### Comparing `pyone-6.6.1/pyone/helpers.py` & `pyone-6.6.2/pyone/helpers.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.1/pyone/server.py` & `pyone-6.6.2/pyone/server.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.1/pyone/tester.py` & `pyone-6.6.2/pyone/tester.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.1/pyone/util.py` & `pyone-6.6.2/pyone/util.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.1/pyone.egg-info/PKG-INFO` & `pyone-6.6.2/pyone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyone
-Version: 6.6.1
+Version: 6.6.2
 Summary: Python Bindings for OpenNebula XML-RPC API
 Home-page: http://opennebula.io
 Author: Rafael del Valle
 Author-email: rvalle@privaz.io
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: PyOne is an implementation of OpenNebula XML-RPC
                 bindings in Python. It works as a proxy over the XML-RPC api and
```

### Comparing `pyone-6.6.1/setup.py` & `pyone-6.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'requests'
 ]
 
 # include future in python2
 if sys.version_info[0] < 3:
     install_requires.append('future')
 
-version = '6.6.1'
+version = '6.6.2'
 
 # mark pre-release
 v1 = int(version.split('.')[1])
 v2 = int(version.split('.')[2])
 
 if v1 >= 90 or v2 >= 90:
     pyone_version = version + 'rc1'
```

