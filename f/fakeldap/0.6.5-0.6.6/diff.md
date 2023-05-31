# Comparing `tmp/fakeldap-0.6.5.tar.gz` & `tmp/fakeldap-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakeldap-0.6.5.tar", last modified: Sat Mar  4 13:17:15 2023, max compression
+gzip compressed data, was "fakeldap-0.6.6.tar", last modified: Wed May 31 09:35:42 2023, max compression
```

## Comparing `fakeldap-0.6.5.tar` & `fakeldap-0.6.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 elev3n    (1000) elev3n    (1000)        0 2023-03-04 13:17:15.441211 fakeldap-0.6.5/
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)       39 2023-03-04 13:07:18.000000 fakeldap-0.6.5/MANIFEST.in
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)     5285 2023-03-04 13:17:15.441211 fakeldap-0.6.5/PKG-INFO
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)     4667 2023-03-04 13:07:18.000000 fakeldap-0.6.5/README.rst
-drwxrwxr-x   0 elev3n    (1000) elev3n    (1000)        0 2023-03-04 13:17:15.441211 fakeldap-0.6.5/fakeldap.egg-info/
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)     5285 2023-03-04 13:17:15.000000 fakeldap-0.6.5/fakeldap.egg-info/PKG-INFO
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)      212 2023-03-04 13:17:15.000000 fakeldap-0.6.5/fakeldap.egg-info/SOURCES.txt
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)        1 2023-03-04 13:17:15.000000 fakeldap-0.6.5/fakeldap.egg-info/dependency_links.txt
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)       61 2023-03-04 13:17:15.000000 fakeldap-0.6.5/fakeldap.egg-info/requires.txt
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)        9 2023-03-04 13:17:15.000000 fakeldap-0.6.5/fakeldap.egg-info/top_level.txt
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)    17152 2023-03-04 13:07:18.000000 fakeldap-0.6.5/fakeldap.py
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)      200 2023-03-04 13:17:15.441211 fakeldap-0.6.5/setup.cfg
--rw-rw-r--   0 elev3n    (1000) elev3n    (1000)     1259 2023-03-04 13:07:18.000000 fakeldap-0.6.5/setup.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 09:35:42.645085 fakeldap-0.6.6/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       39 2023-05-31 09:34:57.000000 fakeldap-0.6.6/MANIFEST.in
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5518 2023-05-31 09:35:42.645085 fakeldap-0.6.6/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4877 2023-05-31 09:34:57.000000 fakeldap-0.6.6/README.rst
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 09:35:42.645085 fakeldap-0.6.6/fakeldap.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5518 2023-05-31 09:35:42.000000 fakeldap-0.6.6/fakeldap.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      218 2023-05-31 09:35:42.000000 fakeldap-0.6.6/fakeldap.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-05-31 09:35:42.000000 fakeldap-0.6.6/fakeldap.egg-info/dependency_links.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       19 2023-05-31 09:35:42.000000 fakeldap-0.6.6/fakeldap.egg-info/requires.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        9 2023-05-31 09:35:42.000000 fakeldap-0.6.6/fakeldap.egg-info/top_level.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    17157 2023-05-31 09:34:57.000000 fakeldap-0.6.6/fakeldap.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      797 2023-05-31 09:34:57.000000 fakeldap-0.6.6/pyproject.toml
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       67 2023-05-31 09:35:42.645085 fakeldap-0.6.6/setup.cfg
```

### Comparing `fakeldap-0.6.5/PKG-INFO` & `fakeldap-0.6.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: fakeldap
-Version: 0.6.5
+Version: 0.6.6
 Summary: An implementation of a LDAPObject to fake a ldap server in unittests.
-Home-page: https://github.com/zulip/fakeldap
-Author: Christo Buschek
-Author-email: crito@30loops.net
+Author-email: Christo Buschek <crito@30loops.net>
+Project-URL: homepage, https://github.com/zulip/fakeldap/
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
-Provides-Extra: test
+Description-Content-Type: text/x-rst
 
 ========
 fakeldap
 ========
 
 The goal of this module is to provide a simple way to mock ldap backend servers
 for your unittests. It makes it possible to define upfront a set of directory
@@ -30,32 +29,40 @@
 taken from Peter Sagerson's excellent django-auth-ldap_ module.
 
 .. _django-auth-ldap: https://bitbucket.org/psagers/django-auth-ldap/wiki/Home
 
 Installation
 ============
 
-Get and install the code::
+Install the latest release from PyPI::
+
+    $ pip install fakeldap
+
+Running tests in development
+============================
+If you've cloned the repository locally::
 
     $ git clone git://github.com/zulip/fakeldap.git
-    $ cd fakeldap
-    $ python setup.py install
 
-If you want, you can run the tests::
+and made changes, ensure you have ``pytest`` installed::
+
+    $ pip install pytest
 
-    $ python setup.py nosetests
+and you can run the tests with::
+
+    $ pytest tests.py
 
 Usage
 =====
 
 .. note::
 
     This code is still experimental and not very tested as of yet. So is the
     documentation
-    
+
 The ``MockLDAP`` class replaces the ``LDAPObject`` of the python-ldap module.
 The easiest way to use it, is to overwrite ``ldap.initialize`` to return
 ``MockLDAP`` instead of ``LDAPObject``. The example below uses Michael Foord's
 Mock_ library to achieve that::
 
     import unittest
     from mock import patch
@@ -105,15 +112,15 @@
 
         # Run your actual code, this is just an example
         group_manager = GroupManager()
         result = group_manager.add("testgroup")
 
         # assert that the return value of your method and of the MockLDAP
         # are as expected, here using python-nose's eq() test tool:
-        eq_(return_value, result)
+        self.assertEqual(return_value, result)
 
         # Each actual ldap call your software makes gets recorded. You could
         # prepare a list of calls that you expect to be issued and compare it:
         called_records = []
 
         called_records.append(('simple_bind_s',
             {'who': 'cn=admin,dc=30loops,dc=net', 'cred': 'ldaptest'}))
@@ -123,40 +130,40 @@
             'record': [
                 ('objectClass', ['posixGroup']),
                 ('gidNumber', '2030'),
                 ('cn', 'testgroup'),
                 ]}))
 
         # And again test the expected behaviour
-        eq_(called_records, _mock_ldap.ldap_methods_called_with_arguments())
+        self.assertEqual(called_records, _mock_ldap.ldap_methods_called_with_arguments())
 
 Besides of fixing return values for specific calls, you can also imitate a full
 ldap server with a directory of entries::
 
     # Create an instance of MockLDAP with a preset directory
     tree = {
         "cn=admin,dc=30loops,dc=net": {
                 "userPassword": "ldaptest"
         }
     }
-    mock_ldap = MockLDAP(tree) 
+    mock_ldap = MockLDAP(tree)
 
     record = [
         ('uid', 'crito'),
         ('userPassword', 'secret'),
     ]
     # The return value I expect when I add another record to the directory
-    eq_(
+    self.assertEqual(
         (105,[],1,[]),
         mock_ldap.add_s("uid=crito,ou=people,dc=30loops,dc=net", record)
     )
 
     # The expected directory
     directory = {
         "cn=admin,dc=30loops,dc=net": {"userPassword": "ldaptest"},
         "uid=crito,ou=people,dc=30loops,dc=net": {
             "uid": "crito", "userPassword": "secret"}
     }
     # Compare the expected directory with the MockLDAP directory
-    eq_(directory, mock_ldap.directory)
+    self.assertEqual(directory, mock_ldap.directory)
 
 .. _Mock: http://www.voidspace.org.uk/python/mock/
```

### Comparing `fakeldap-0.6.5/README.rst` & `fakeldap-0.6.6/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -13,32 +13,40 @@
 taken from Peter Sagerson's excellent django-auth-ldap_ module.
 
 .. _django-auth-ldap: https://bitbucket.org/psagers/django-auth-ldap/wiki/Home
 
 Installation
 ============
 
-Get and install the code::
+Install the latest release from PyPI::
+
+    $ pip install fakeldap
+
+Running tests in development
+============================
+If you've cloned the repository locally::
 
     $ git clone git://github.com/zulip/fakeldap.git
-    $ cd fakeldap
-    $ python setup.py install
 
-If you want, you can run the tests::
+and made changes, ensure you have ``pytest`` installed::
+
+    $ pip install pytest
 
-    $ python setup.py nosetests
+and you can run the tests with::
+
+    $ pytest tests.py
 
 Usage
 =====
 
 .. note::
 
     This code is still experimental and not very tested as of yet. So is the
     documentation
-    
+
 The ``MockLDAP`` class replaces the ``LDAPObject`` of the python-ldap module.
 The easiest way to use it, is to overwrite ``ldap.initialize`` to return
 ``MockLDAP`` instead of ``LDAPObject``. The example below uses Michael Foord's
 Mock_ library to achieve that::
 
     import unittest
     from mock import patch
@@ -88,15 +96,15 @@
 
         # Run your actual code, this is just an example
         group_manager = GroupManager()
         result = group_manager.add("testgroup")
 
         # assert that the return value of your method and of the MockLDAP
         # are as expected, here using python-nose's eq() test tool:
-        eq_(return_value, result)
+        self.assertEqual(return_value, result)
 
         # Each actual ldap call your software makes gets recorded. You could
         # prepare a list of calls that you expect to be issued and compare it:
         called_records = []
 
         called_records.append(('simple_bind_s',
             {'who': 'cn=admin,dc=30loops,dc=net', 'cred': 'ldaptest'}))
@@ -106,40 +114,40 @@
             'record': [
                 ('objectClass', ['posixGroup']),
                 ('gidNumber', '2030'),
                 ('cn', 'testgroup'),
                 ]}))
 
         # And again test the expected behaviour
-        eq_(called_records, _mock_ldap.ldap_methods_called_with_arguments())
+        self.assertEqual(called_records, _mock_ldap.ldap_methods_called_with_arguments())
 
 Besides of fixing return values for specific calls, you can also imitate a full
 ldap server with a directory of entries::
 
     # Create an instance of MockLDAP with a preset directory
     tree = {
         "cn=admin,dc=30loops,dc=net": {
                 "userPassword": "ldaptest"
         }
     }
-    mock_ldap = MockLDAP(tree) 
+    mock_ldap = MockLDAP(tree)
 
     record = [
         ('uid', 'crito'),
         ('userPassword', 'secret'),
     ]
     # The return value I expect when I add another record to the directory
-    eq_(
+    self.assertEqual(
         (105,[],1,[]),
         mock_ldap.add_s("uid=crito,ou=people,dc=30loops,dc=net", record)
     )
 
     # The expected directory
     directory = {
         "cn=admin,dc=30loops,dc=net": {"userPassword": "ldaptest"},
         "uid=crito,ou=people,dc=30loops,dc=net": {
             "uid": "crito", "userPassword": "secret"}
     }
     # Compare the expected directory with the MockLDAP directory
-    eq_(directory, mock_ldap.directory)
+    self.assertEqual(directory, mock_ldap.directory)
 
 .. _Mock: http://www.voidspace.org.uk/python/mock/
```

### Comparing `fakeldap-0.6.5/fakeldap.egg-info/PKG-INFO` & `fakeldap-0.6.6/fakeldap.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: fakeldap
-Version: 0.6.5
+Version: 0.6.6
 Summary: An implementation of a LDAPObject to fake a ldap server in unittests.
-Home-page: https://github.com/zulip/fakeldap
-Author: Christo Buschek
-Author-email: crito@30loops.net
+Author-email: Christo Buschek <crito@30loops.net>
+Project-URL: homepage, https://github.com/zulip/fakeldap/
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
-Provides-Extra: test
+Description-Content-Type: text/x-rst
 
 ========
 fakeldap
 ========
 
 The goal of this module is to provide a simple way to mock ldap backend servers
 for your unittests. It makes it possible to define upfront a set of directory
@@ -30,32 +29,40 @@
 taken from Peter Sagerson's excellent django-auth-ldap_ module.
 
 .. _django-auth-ldap: https://bitbucket.org/psagers/django-auth-ldap/wiki/Home
 
 Installation
 ============
 
-Get and install the code::
+Install the latest release from PyPI::
+
+    $ pip install fakeldap
+
+Running tests in development
+============================
+If you've cloned the repository locally::
 
     $ git clone git://github.com/zulip/fakeldap.git
-    $ cd fakeldap
-    $ python setup.py install
 
-If you want, you can run the tests::
+and made changes, ensure you have ``pytest`` installed::
+
+    $ pip install pytest
 
-    $ python setup.py nosetests
+and you can run the tests with::
+
+    $ pytest tests.py
 
 Usage
 =====
 
 .. note::
 
     This code is still experimental and not very tested as of yet. So is the
     documentation
-    
+
 The ``MockLDAP`` class replaces the ``LDAPObject`` of the python-ldap module.
 The easiest way to use it, is to overwrite ``ldap.initialize`` to return
 ``MockLDAP`` instead of ``LDAPObject``. The example below uses Michael Foord's
 Mock_ library to achieve that::
 
     import unittest
     from mock import patch
@@ -105,15 +112,15 @@
 
         # Run your actual code, this is just an example
         group_manager = GroupManager()
         result = group_manager.add("testgroup")
 
         # assert that the return value of your method and of the MockLDAP
         # are as expected, here using python-nose's eq() test tool:
-        eq_(return_value, result)
+        self.assertEqual(return_value, result)
 
         # Each actual ldap call your software makes gets recorded. You could
         # prepare a list of calls that you expect to be issued and compare it:
         called_records = []
 
         called_records.append(('simple_bind_s',
             {'who': 'cn=admin,dc=30loops,dc=net', 'cred': 'ldaptest'}))
@@ -123,40 +130,40 @@
             'record': [
                 ('objectClass', ['posixGroup']),
                 ('gidNumber', '2030'),
                 ('cn', 'testgroup'),
                 ]}))
 
         # And again test the expected behaviour
-        eq_(called_records, _mock_ldap.ldap_methods_called_with_arguments())
+        self.assertEqual(called_records, _mock_ldap.ldap_methods_called_with_arguments())
 
 Besides of fixing return values for specific calls, you can also imitate a full
 ldap server with a directory of entries::
 
     # Create an instance of MockLDAP with a preset directory
     tree = {
         "cn=admin,dc=30loops,dc=net": {
                 "userPassword": "ldaptest"
         }
     }
-    mock_ldap = MockLDAP(tree) 
+    mock_ldap = MockLDAP(tree)
 
     record = [
         ('uid', 'crito'),
         ('userPassword', 'secret'),
     ]
     # The return value I expect when I add another record to the directory
-    eq_(
+    self.assertEqual(
         (105,[],1,[]),
         mock_ldap.add_s("uid=crito,ou=people,dc=30loops,dc=net", record)
     )
 
     # The expected directory
     directory = {
         "cn=admin,dc=30loops,dc=net": {"userPassword": "ldaptest"},
         "uid=crito,ou=people,dc=30loops,dc=net": {
             "uid": "crito", "userPassword": "secret"}
     }
     # Compare the expected directory with the MockLDAP directory
-    eq_(directory, mock_ldap.directory)
+    self.assertEqual(directory, mock_ldap.directory)
 
 .. _Mock: http://www.voidspace.org.uk/python/mock/
```

### Comparing `fakeldap-0.6.5/fakeldap.py` & `fakeldap-0.6.6/fakeldap.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,23 +415,23 @@
                 raise ldap.NO_SUCH_OBJECT
 
             return [(base, attrs)]
         elif scope == self.SCOPE_ONELEVEL:
             simple_query_regex = r"\(\w+=.+\)$"  # matches things like (some_attribute=value)
             r_simple = re.compile(simple_query_regex)
 
-            anding_query_regex = r"\(\&(\(\w+=[A-Za-z0-9_\@\.]+\))+\)$"  # matches things like (&(some_attribute=value)(other_attr=othervalue)), but with any number of "anded" conditions
+            anding_query_regex = r"\(\&(\(\w+=[A-Za-z0-9_\@\.=,]+\))+\)$"  # matches things like (&(some_attribute=value)(other_attr=othervalue)), but with any number of "anded" conditions
             r_anded = re.compile(anding_query_regex)
 
             if r_simple.match(filterstr) is not None:
                 search_attr_name, search_attr_value = filterstr[1:-1].split('=')
                 return self._multiple_attrs_onelevel_search(base, [(search_attr_name, search_attr_value)])
             elif r_anded.match(filterstr) is not None:
                 bracketList = filterstr[3:-2] # cut of the `(&(` and `))` --> attr1=val1)(attr2=val2
-                attrs_conditions = [tuple(condition.split("=")) for condition in bracketList.split(")(")]
+                attrs_conditions = [tuple(condition.split("=", 1)) for condition in bracketList.split(")(")]
                 return self._multiple_attrs_onelevel_search(base, attrs_conditions)
             else:
                 raise self.PresetReturnRequiredError('search_s("%s", %d, "%s", "%s", %d)' %
                     (base, scope, filterstr, attrlist, attrsonly))
         else:
             raise self.PresetReturnRequiredError('search_s("%s", %d, "%s", "%s", %d)' %
                 (base, scope, filterstr, attrlist, attrsonly))
```

