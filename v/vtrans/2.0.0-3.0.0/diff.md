# Comparing `tmp/vtrans-2.0.0.tar.gz` & `tmp/vtrans-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtrans-2.0.0.tar", last modified: Sat May 27 11:09:48 2023, max compression
+gzip compressed data, was "vtrans-3.0.0.tar", last modified: Wed May 31 08:27:12 2023, max compression
```

## Comparing `vtrans-2.0.0.tar` & `vtrans-3.0.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 11:09:48.445428 vtrans-2.0.0/
--rw-rw-rw-   0        0        0       82 2023-05-27 11:05:51.000000 vtrans-2.0.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 08:21:58.000000 vtrans-2.0.0/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-05-27 08:18:00.000000 vtrans-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1786 2023-05-27 11:09:48.443421 vtrans-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      899 2023-05-27 09:44:39.000000 vtrans-2.0.0/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 11:09:48.447432 vtrans-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1120 2023-05-27 11:06:06.000000 vtrans-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 11:09:48.363307 vtrans-2.0.0/vtrans/
--rw-rw-rw-   0        0        0     9512 2023-05-27 11:09:14.000000 vtrans-2.0.0/vtrans/__init__.py
--rw-rw-rw-   0        0        0       58 2023-05-27 07:48:30.000000 vtrans-2.0.0/vtrans/config.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 11:09:48.435412 vtrans-2.0.0/vtrans.egg-info/
--rw-rw-rw-   0        0        0     1786 2023-05-27 11:09:47.000000 vtrans-2.0.0/vtrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-05-27 11:09:48.000000 vtrans-2.0.0/vtrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:09:47.000000 vtrans-2.0.0/vtrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-27 11:09:47.000000 vtrans-2.0.0/vtrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 11:09:47.000000 vtrans-2.0.0/vtrans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 08:27:12.075964 vtrans-3.0.0/
+-rw-rw-rw-   0        0        0       70 2023-05-31 08:23:56.000000 vtrans-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9224 2023-05-31 08:27:12.078961 vtrans-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8194 2023-05-31 08:05:03.000000 vtrans-3.0.0/README.md
+-rw-rw-rw-   0        0        0      114 2023-05-31 08:27:12.086972 vtrans-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1332 2023-05-31 08:21:47.000000 vtrans-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 08:27:11.950773 vtrans-3.0.0/vtrans/
+-rw-rw-rw-   0        0        0     9521 2023-05-31 07:01:44.000000 vtrans-3.0.0/vtrans/__init__.py
+-rw-rw-rw-   0        0        0       58 2023-05-27 07:48:30.000000 vtrans-3.0.0/vtrans/config.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 08:27:12.064943 vtrans-3.0.0/vtrans.egg-info/
+-rw-rw-rw-   0        0        0     9224 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 08:27:11.000000 vtrans-3.0.0/vtrans.egg-info/top_level.txt
```

### Comparing `vtrans-2.0.0/setup.py` & `vtrans-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from setuptools import setup, find_packages
 
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Education',
+  'Intended Audience :: End Users/Desktop',
+  'License :: Freeware',
+  'Operating System :: MacOS :: MacOS X',
+  'Topic :: Education',
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'Operating System :: Microsoft :: Windows :: Windows 8.1',
   'Operating System :: Microsoft :: Windows :: Windows 8',
   'License :: OSI Approved :: MIT License',
-  'Programming Language :: Python :: 3'
+  'Programming Language :: Python',
+  'Programming Language :: Python :: 3.8'
 ]
 
 setup(
   name='vtrans',
-  version='2.0.0',
-  description='This is a self-updating translator powered by Google Translate for free and unlimited usage.',
-  long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
+  version='3.0.0',
+  description='This is a self-updating translator for free and unlimited usage with upto 130 langauges',
+  long_description=open('README.md',"r",encoding="utf-8").read(),
+  long_description_content_type='text/markdown',
   url='https://github.com/megalosVigneswaran/vtrans/tree/main/vtrans',  
   author='S.Vigneswaran',
   author_email='t896242@gmail.com',
   license='MIT',
   classifiers=classifiers,
-  keywords=['translator', 'googletranslate', 'self-updating', 'googletrans'],
+  keywords=['translator', 'googletranslate', 'self-updating', 'googletrans','vtrans'],
   packages=find_packages(),
   package_data={
         'vtrans': ['config.txt'],
     },
   install_requires=['googletrans==3.1.0a0', 'pandas', 'requests', 'beautifulsoup4', 'astor'] 
 )
```

### Comparing `vtrans-2.0.0/vtrans/__init__.py` & `vtrans-3.0.0/vtrans/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     
     IT CHECK UPDATING IN EVERY IMPORT OF THIS LIBRARY IT MAKE IT LITTLE BIT SLOWER,
     
     BUT YOU CAN DISABLE AUTOUPDATE CHECKING BY THIS CODE '''vtrans.config(auto_updating = False)'''."""
 
 __Author__ = "S.Vigneswaran"
 
-__Version__ = 2.0
+__Version__ = 3.0
 
 import os
 
 """ This function is helps to set optional settings of this translator 
        
     it helps to disable the autoupdating"""
 def config(auto_updating='True'):
@@ -38,15 +38,15 @@
     prin = config_data['print']
     if autoup_config == auto_updating:
         pass
     else:
         #Save the new values in config file
         pattern = {'print':prin,'autoupdate':auto_updating,'original_lang':orginal_lang}
         with open(config_path,"w") as write_config:
-            write_config.write(pattern)
+            write_config.write(str(pattern))
         if auto_updating == 'True':
             print("Auto updating is turn enabled")
         elif auto_updating == 'False':
             print("Auto updating is disabled")
 
 def remove_unwanted_printing():
     data =check_con()
@@ -120,19 +120,19 @@
         update() #use update function to update
     else:
         #Else the original_lang = number of current avilable languages 
         print("this is te latest version you don't need to update") # print "this is te latest version you don't need to update"
 
 
 def update():
-    print("Please wait for a few seconds, updating is in progress...")
+    print("Please wait for a few seconds, update is in progress...")
 
     #importing modules
 
-    import ast             #ast module used to edit py files
+    import ast             #ast module used to edit .py files
     import astor           #astor module is the give support to ast
     import pandas as pd    #pandas used to scrap the table in web page
 
     tables = pd.read_html('https://cloud.google.com/translate/docs/languages')  #Collect tables in https://cloud.google.com/translate/docs/languages
 
     langlist = tables[0].to_dict(orient='records') #Get first table of this page, make dictionary like orientation using to_dict(orient='records')
 
@@ -155,15 +155,15 @@
 
     autoup_config = config_data['autoupdate'] #get autoupdate value
     prin = config_data['print']
 
     pattern = {'print':prin,'autoupdate':autoup_config,'original_lang':str(len(orginal_lang))} #insert values in dict pattern
 
     with open(config_path,"w") as write_config: # open and rewrite config data
-        write_config.write(pattern)
+        write_config.write(str(pattern))
     
     #Create main dictionary
     for dictio in langlist:
         language = str(dictio['Language'])
         langcode = str(dictio['ISO-639 code'])
         language = language.lower()
         langcode = langcode.split() #Split langcode to remove unwanted text
```

