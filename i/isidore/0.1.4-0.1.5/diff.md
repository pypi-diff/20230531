# Comparing `tmp/isidore-0.1.4.tar.gz` & `tmp/isidore-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/data/Documents/Programs/isidore/lib/dist/.tmp-gvw_81_m/isidore-0.1.4.tar", last modified: Wed May 24 17:38:01 2023, max compression
+gzip compressed data, was "/media/data/Documents/Programs/isidore/lib/dist/.tmp-4i41bj9k/isidore-0.1.5.tar", last modified: Wed May 31 19:29:38 2023, max compression
```

## Comparing `isidore-0.1.4.tar` & `isidore-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-24 17:38:01.000000 isidore-0.1.4/
--rw-r--r--   0 scott     (1000) scott     (1000)     1063 2023-05-06 12:39:48.000000 isidore-0.1.4/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-24 17:38:01.000000 isidore-0.1.4/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      245 2023-05-12 17:10:25.000000 isidore-0.1.4/README.md
--rw-r--r--   0 scott     (1000) scott     (1000)      880 2023-05-24 17:37:13.000000 isidore-0.1.4/pyproject.toml
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-05-24 17:38:01.000000 isidore-0.1.4/setup.cfg
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-24 17:38:01.000000 isidore-0.1.4/src/
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore/
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-12 12:18:21.000000 isidore-0.1.4/src/isidore/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)    33953 2023-05-24 17:37:13.000000 isidore-0.1.4/src/isidore/libIsidore.py
--rw-r--r--   0 scott     (1000) scott     (1000)    37675 2023-05-24 17:37:13.000000 isidore-0.1.4/src/isidore/libIsidoreCmdline.py
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      289 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       30 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/requires.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        8 2023-05-24 17:38:01.000000 isidore-0.1.4/src/isidore.egg-info/top_level.txt
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-31 19:29:38.000000 isidore-0.1.5/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1063 2023-05-06 12:39:48.000000 isidore-0.1.5/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-31 19:29:38.000000 isidore-0.1.5/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      245 2023-05-12 17:10:25.000000 isidore-0.1.5/README.md
+-rw-r--r--   0 scott     (1000) scott     (1000)      880 2023-05-31 19:27:08.000000 isidore-0.1.5/pyproject.toml
+-rw-r--r--   0 scott     (1000) scott     (1000)       38 2023-05-31 19:29:38.000000 isidore-0.1.5/setup.cfg
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-31 19:29:38.000000 isidore-0.1.5/src/
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-31 19:29:38.000000 isidore-0.1.5/src/isidore/
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-12 12:18:21.000000 isidore-0.1.5/src/isidore/__init__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    34097 2023-05-31 19:27:08.000000 isidore-0.1.5/src/isidore/libIsidore.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    41876 2023-05-31 19:27:08.000000 isidore-0.1.5/src/isidore/libIsidoreCmdline.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2023-05-31 19:29:38.000000 isidore-0.1.5/src/isidore.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1002 2023-05-31 19:29:38.000000 isidore-0.1.5/src/isidore.egg-info/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      289 2023-05-31 19:29:38.000000 isidore-0.1.5/src/isidore.egg-info/SOURCES.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2023-05-31 19:29:38.000000 isidore-0.1.5/src/isidore.egg-info/dependency_links.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       30 2023-05-31 19:29:38.000000 isidore-0.1.5/src/isidore.egg-info/requires.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        8 2023-05-31 19:29:38.000000 isidore-0.1.5/src/isidore.egg-info/top_level.txt
```

### Comparing `isidore-0.1.4/LICENSE` & `isidore-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `isidore-0.1.4/PKG-INFO` & `isidore-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isidore
-Version: 0.1.4
+Version: 0.1.5
 Summary: database, API, and CLI suite for managing Ansible inventories
 Author-email: Scott Court <Z5T1@Z5T1.com>
 Project-URL: Homepage, https://github.com/Z5T1/isidore
 Project-URL: Bug Tracker, https://github.com/Z5T1/isidore/issues
 Project-URL: Documentation, https://github.com/Z5T1/isidore/blob/master/doc/README.md
 Project-URL: Discord, https://discord.gg/c357N3JQFJ
 Project-URL: Source Code, https://github.com/Z5T1/isidore
```

### Comparing `isidore-0.1.4/pyproject.toml` & `isidore-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "isidore"
-version = "0.1.4"
+version = "0.1.5"
 keywords = [ "ansible", "inventory", "database", "isidore" ]
 authors = [
   { name="Scott Court", email="Z5T1@Z5T1.com" },
 ]
 description = "database, API, and CLI suite for managing Ansible inventories"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `isidore-0.1.4/src/isidore/libIsidore.py` & `isidore-0.1.5/src/isidore/libIsidore.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import yaml
 import json
 
 # Represents an Isidore database instance
 class Isidore:
 
     _conn = None
-    _version = '0.1.4'
+    _version = '0.1.5'
 
     # Connects to a MySQL database and creates a new Isidore object to interact
     # with it.
     # @param user       The MySQL username
     # @param password   The password for the MySQL user
     # @param host       The MySQL server to connect to
     # @param database   The name of the database to use
@@ -496,15 +496,17 @@
             path = '$.' + path
 
         # Set the variable
         stmt = '''
             UPDATE Host
             SET Variables =
                 JSON_ARRAY_APPEND(
-                    (SELECT Variables FROM Host WHERE HostId = %s),
+                    (SELECT Variables
+                        FROM (SELECT * FROM Host) AS temp
+                        WHERE HostId = %s),
                     %s,
                     JSON_EXTRACT(%s, '$')
                 )
             WHERE HostID = %s'''
         cursor = self._isidore._conn.cursor()
         cursor.execute(stmt, [
             self._hostId,
@@ -785,15 +787,17 @@
             path = '$.' + path
 
         # Set the variable
         stmt = '''
             UPDATE Tag
             SET Variables =
                 JSON_ARRAY_APPEND(
-                    (SELECT Variables FROM Tag WHERE TagID = %s),
+                    (SELECT Variables
+                        FROM (SELECT * FROM Tag) AS temp
+                        WHERE TagId = %s),
                     %s,
                     JSON_EXTRACT(%s, '$')
                 )
             WHERE TagID = %s'''
         cursor = self._isidore._conn.cursor()
         cursor.execute(stmt, [
             self._tagId,
```

### Comparing `isidore-0.1.4/src/isidore/libIsidoreCmdline.py` & `isidore-0.1.5/src/isidore/libIsidoreCmdline.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from isidore.libIsidore import *
 
 # The Isidore command prompt
 class IsidoreCmdline:
 
     _isidore = None
-    _version = '0.1.4'
+    _version = '0.1.5'
 
     # Creates a new Isidore command prompt
     # @param isidore    The underlying Isidore instance for the command prompt
     #                   to connect to.
     def __init__(self, isidore):
         self._isidore = isidore
 
@@ -98,14 +98,16 @@
         # Parse inut
         if args[0] == '?':
             self.help(args)
         elif args[0] == 'create':
             self.create(args)
         elif args[0] == 'delete':
             self.delete(args)
+        elif args[0] == 'describe':
+            self.describe(args)
         elif args[0] == 'echo':
             self.echo(args)
         elif args[0] == 'help':
             print('''\
 Pst! You should really use ? to display the help message. ? will
 work at every subprompt level. help only works at the root
 prompt.
@@ -126,14 +128,15 @@
 
     # > ?
     def help(self, args):
         print('''\
 ?           print this help message
 create      create various objects (such as hosts and tags)
 delete      delete various objects (such as hosts and tags)
+describe    print details about various data
 echo        print text back to the console
 help        alias for ?
 host        manipulate a host
 rename      rename various objects (such as hosts and tags)
 show        print various data
 tag         manipulate a tag
 version     display Isidore version information''')
@@ -275,14 +278,82 @@
         print(yaml.dump(tags, default_flow_style=False))
 
     # > show tags
     def show_tags(self, args):
         for tag in self._isidore.getTags():
             print(tag.getName())
 
+    # > describe
+    def describe(self, args):
+        if len(args) == 1:
+            self.subprompt(args, self.describe)
+
+        elif args[1] == '?':
+            print('''\
+?           print this help message
+hosts       describe all commissioned hosts in the database
+graveyard   describe all decommissioned hosts in the database
+tag-groups  describe all the tag groups in the database
+tags        describe all tags in the database''')
+
+        elif args[1] == 'hosts':
+            self.describe_hosts(args[1])
+
+        elif args[1] == 'graveyard':
+            self.describe_graveyard(args[1])
+
+        elif args[1] == 'tag-groups':
+            self.describe_taggroups(args[1])
+
+        elif args[1] == 'tags':
+            self.describe_tags(args[1])
+
+        else:
+            print('Invalid argument '+args[1]+'. Enter ? for help.', file=sys.stderr)
+
+    # > describe hosts
+    def describe_hosts(self, args):
+        hosts = {}
+        for host in self._isidore.getCommissionedHosts():
+            hosts[host.getHostname()] = host.getDescription()
+        print(yaml.dump(hosts, default_flow_style=False))
+
+    # > describe graveyard
+    def describe_graveyard(self, args):
+        hosts = {}
+        for host in self._isidore.getDecommissionedHosts():
+            hosts[host.getHostname()] = host.getDescription()
+        print(yaml.dump(hosts, default_flow_style=False))
+
+
+    # > describe tag-groups
+    def describe_taggroups(self, args):
+        tags = {}
+
+        # Populate the top level
+        for (group, tagsstr) in self._isidore.getTagGroups():
+            if group == None:
+                group = 'ungrouped'
+            tags[group] = list()
+
+        for tag in self._isidore.getTags():
+            group = tag.getGroup()
+            if group == None:
+                group = 'ungrouped'
+            tags[group].append( { tag.getName(): tag.getDescription() } )
+
+        print(yaml.dump(tags, default_flow_style=False))
+
+    # > describe tags
+    def describe_tags(self, args):
+        tags = {}
+        for tag in self._isidore.getTags():
+            tags[tag.getName()] = tag.getDescription()
+        print(yaml.dump(tags, default_flow_style=False))
+
     # > create
     def create(self, args):
         if len(args) == 1:
             self.subprompt(args, self.create)
         elif args[1] == '?':
             print('''\
 ?           print this help message
@@ -446,49 +517,73 @@
 
         # Handle arg #2 (host foo <ARG2>)
         elif len(args) == 2:
             self.subprompt(args, self.host)
         elif args[2] == '?':
             print('''\
 ?           print this help message
+describe    print details about host attributes
 set         modify host attributes
 show        display host attributes
 tag         display and modify this host's tags
 var         display and modify this host's variables''')
+        elif args[2] == 'describe':
+            self.host_describe(args)
         elif args[2] == 'set':
             self.host_set(args)
         elif args[2] == 'show':
             self.host_show(args)
         elif args[2] == 'tag':
             self.host_tag(args)
         elif args[2] == 'var':
             self.host_var(args)
         else:
             print('Invalid command '+args[2]+'. Enter ? for help.', file=sys.stderr)
 
+    # > host <hostname> describe
+    def host_describe(self, args):
+        host = self._isidore.getHost(args[1])
+        if len(args) == 3:
+            self.subprompt(args, self.host_describe)
+        elif args[3] == '?':
+            print('''\
+?           print this help message
+tags        describe the tags currently assigned to this host''')
+        elif args[3] == 'tags':
+            tags = {}
+            for tag in host.getTags():
+                tags[tag.getName()] = tag.getDescription()
+            print(yaml.dump(tags, default_flow_style=False))
+        else:
+            print('Invalid argument '+args[3]+'. Enter ? for help.', file=sys.stderr)
+
     # > host <hostname> show
     def host_show(self, args):
         host = self._isidore.getHost(args[1])
         if len(args) == 3:
             self.subprompt(args, self.host)
         elif args[3] == '?':
             print('''\
 ?           print this help message
 all         print all the information about the host
 commissioned    print the date the host was commissioned
 description     print the host's description
-decommissioned  print the date the host was decommissioned''')
+decommissioned  print the date the host was decommissioned
+tags        print the tags currently assigned to this host''')
         elif args[3] == 'all':
             print(yaml.dump(host.getDetails(), default_flow_style=False))
         elif args[3] == 'commissioned':
             print(host.getCommissionDate())
         elif args[3] == 'description':
             print(host.getDescription())
         elif args[3] == 'decommissioned':
             print(host.getDecommissionDate())
+        elif args[3] == 'tags':
+            for tag in host.getTags():
+                print(tag.getName())
         else:
             print('Invalid argument '+args[3]+'. Enter ? for help.', file=sys.stderr)
 
     # > host <hostname> set
     def host_set(self, args):
         host = self._isidore.getHost(args[1])
         if len(args) == 3:
@@ -574,15 +669,15 @@
             tags = list()
             for tag in host.getTags(True):
                 tags.append( {
                     'name': tag.getName(),
                     'group': tag.getGroup(),
                     'description': tag.getDescription()
                     } )
-            print(yaml.dump(tags, default_flow_style=False))
+            print(yaml.dump(tags, default_flow_style=False, sort_keys=False))
 
         elif args[3] == 'remove':
             self.host_tag_remove(args)
         else:
             print('Invalid command '+args[3]+'. Enter ? for help.', file=sys.stderr)
 
     # > host <hostname> var
@@ -878,29 +973,49 @@
 
         # Handle arg #2 (tag foo <ARG2>)
         elif len(args) == 2:
             self.subprompt(args, self.tag)
         elif args[2] == '?':
             print('''\
 ?           print this help message
+describe    print details about tag attributes
 host        display and modify hosts that have this tag
 set         modify tag attributes
 show        display tag attributes
 var         display and modify this tag's variables''')
+        elif args[2] == 'describe':
+            self.tag_describe(args)
         elif args[2] == 'host':
             self.tag_host(args)
         elif args[2] == 'set':
             self.tag_set(args)
         elif args[2] == 'show':
             self.tag_show(args)
         elif args[2] == 'var':
             self.tag_var(args)
         else:
             print('Invalid command '+args[2]+'. Enter ? for help.', file=sys.stderr)
 
+    # > tag <tagname> describe
+    def tag_describe(self, args):
+        tag = self._isidore.getTag(args[1])
+        if len(args) == 3:
+            self.subprompt(args, self.tag_describe)
+        elif args[3] == '?':
+            print('''\
+?           print this help message
+hosts       describe the hosts currently assigned to this tag''')
+        elif args[3] == 'hosts':
+            hosts = {}
+            for host in tag.getHosts():
+                hosts[host.getHostname()] = host.getDescription()
+            print(yaml.dump(hosts, default_flow_style=False))
+        else:
+            print('Invalid argument '+args[3]+'. Enter ? for help.', file=sys.stderr)
+
     # > tag <tagname> host
     def tag_host(self, args):
         tag = self._isidore.getTag(args[1])
         if len(args) == 3:
             self.subprompt(args, self.tag)
         elif args[3] == '?':
             print('''\
@@ -966,21 +1081,25 @@
         if len(args) == 3:
             self.subprompt(args, self.tag)
         elif args[3] == '?':
             print('''\
 ?           print this help message
 all         print all the information about the tag
 description print the tag's description
-group       print the date the tag was commissioned''')
+group       print the date the tag was commissioned
+hosts       print all hosts that have this tag''')
         elif args[3] == 'all':
             print(yaml.dump(tag.getDetails(), default_flow_style=False))
         elif args[3] == 'description':
             print(tag.getDescription())
         elif args[3] == 'group':
             print(tag.getGroup())
+        elif args[3] == 'hosts':
+            for host in tag.getHosts():
+                print(host.getHostname())
         else:
             print('Invalid argument '+args[3]+'. Enter ? for help.', file=sys.stderr)
 
     # > tag <tagname> set
     def tag_set(self, args):
         tag = self._isidore.getTag(args[1])
         if len(args) == 3:
```

### Comparing `isidore-0.1.4/src/isidore.egg-info/PKG-INFO` & `isidore-0.1.5/src/isidore.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isidore
-Version: 0.1.4
+Version: 0.1.5
 Summary: database, API, and CLI suite for managing Ansible inventories
 Author-email: Scott Court <Z5T1@Z5T1.com>
 Project-URL: Homepage, https://github.com/Z5T1/isidore
 Project-URL: Bug Tracker, https://github.com/Z5T1/isidore/issues
 Project-URL: Documentation, https://github.com/Z5T1/isidore/blob/master/doc/README.md
 Project-URL: Discord, https://discord.gg/c357N3JQFJ
 Project-URL: Source Code, https://github.com/Z5T1/isidore
```

