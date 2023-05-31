# Comparing `tmp/vector_vault-1.6.2.tar.gz` & `tmp/vector_vault-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.2.tar", last modified: Tue May 30 23:38:47 2023, max compression
+gzip compressed data, was "vector_vault-1.6.3.tar", last modified: Wed May 31 06:49:05 2023, max compression
```

## Comparing `vector_vault-1.6.2.tar` & `vector_vault-1.6.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:38:47.903531 vector_vault-1.6.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    21423 2023-05-30 23:38:47.903355 vector_vault-1.6.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    20698 2023-05-30 23:19:30.000000 vector_vault-1.6.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-30 23:38:47.903602 vector_vault-1.6.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-30 23:38:37.000000 vector_vault-1.6.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:38:47.899169 vector_vault-1.6.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    21423 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:38:47.902662 vector_vault-1.6.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.6.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3261 2023-05-30 23:18:26.000000 vector_vault-1.6.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1590 2023-05-30 23:36:22.000000 vector_vault-1.6.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.2/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18189 2023-05-30 23:18:17.000000 vector_vault-1.6.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4344 2023-05-30 21:10:57.000000 vector_vault-1.6.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-31 06:49:05.289125 vector_vault-1.6.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    21275 2023-05-31 06:49:05.289001 vector_vault-1.6.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    20550 2023-05-31 05:38:28.000000 vector_vault-1.6.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-31 06:49:05.289162 vector_vault-1.6.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-31 06:47:53.000000 vector_vault-1.6.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-31 06:49:05.285782 vector_vault-1.6.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    21275 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-31 06:49:05.000000 vector_vault-1.6.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-31 06:49:05.288600 vector_vault-1.6.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.6.3/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3249 2023-05-31 06:45:39.000000 vector_vault-1.6.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1582 2023-05-31 06:45:44.000000 vector_vault-1.6.3/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.3/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18190 2023-05-31 06:45:53.000000 vector_vault-1.6.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.6.3/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.3/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.2/LICENSE` & `vector_vault-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.2/PKG-INFO` & `vector_vault-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.2
+Version: 1.6.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -257,18 +257,14 @@
 
 <br>
 <br>
 <br>
 
 # Metadata
 
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/56e35d92-f673-4e53-b8cc-7f31e86f2c3b/metadata_meme.png?" width="50%" height="50%" />
-</p>
-
 Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
@@ -496,39 +492,43 @@
 
 ---
 <br>
 <br>
 
 
 
-### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
-
+## Getting Started:
 Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
+
+## Contact:
+### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
+Happy coding!
+<br>
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
+</p>
+
 <br>
 
 
 ## FAQ
+<br>
 
 ### What is the latency on large datasets?
 To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
 
+<br>
 
 ### How should I segment my data?
 Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
 
+<br>
 
 ### What if I'm a large company with very large data
 If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need, that is always active. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
 
-<br>
-
-Happy coding!
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
-</p>
-
-<br>
```

### Comparing `vector_vault-1.6.2/README.md` & `vector_vault-1.6.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -238,18 +238,14 @@
 
 <br>
 <br>
 <br>
 
 # Metadata
 
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/56e35d92-f673-4e53-b8cc-7f31e86f2c3b/metadata_meme.png?" width="50%" height="50%" />
-</p>
-
 Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
@@ -477,37 +473,41 @@
 
 ---
 <br>
 <br>
 
 
 
-### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
-
+## Getting Started:
 Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
+
+## Contact:
+### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
+Happy coding!
+<br>
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
+</p>
+
 <br>
 
 
 ## FAQ
+<br>
 
 ### What is the latency on large datasets?
 To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
 
+<br>
 
 ### How should I segment my data?
 Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
 
+<br>
 
 ### What if I'm a large company with very large data
 If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need, that is always active. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
 
-<br>
-
-Happy coding!
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
-</p>
-
-<br>
```

### Comparing `vector_vault-1.6.2/setup.py` & `vector_vault-1.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.2",
+    version="1.6.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.6.3/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.2
+Version: 1.6.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -257,18 +257,14 @@
 
 <br>
 <br>
 <br>
 
 # Metadata
 
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/56e35d92-f673-4e53-b8cc-7f31e86f2c3b/metadata_meme.png?" width="50%" height="50%" />
-</p>
-
 Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
 ```
 meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
@@ -496,39 +492,43 @@
 
 ---
 <br>
 <br>
 
 
 
-### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
-
+## Getting Started:
 Open the "examples" folder and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
+
+## Contact:
+### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
+Happy coding!
+<br>
+<p align="center">
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
+</p>
+
 <br>
 
 
 ## FAQ
+<br>
 
 ### What is the latency on large datasets?
 To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
 
+<br>
 
 ### How should I segment my data?
 Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
 
+<br>
 
 ### What if I'm a large company with very large data
 If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need, that is always active. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
 
-<br>
-
-Happy coding!
-<p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
-</p>
-
-<br>
```

### Comparing `vector_vault-1.6.2/vectorvault/__init__.py` & `vector_vault-1.6.3/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.2/vectorvault/ai.py` & `vector_vault-1.6.3/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.2/vectorvault/cloudmanager.py` & `vector_vault-1.6.3/vectorvault/cloudmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             blob = self.cloud.blob(vault_name)
             blob.download_to_filename(temp_file.name) 
             return temp_file.name
 
     def upload(self, item, text, meta):
         with ThreadPoolExecutor() as executor:
-            executor.submit(self.upload_to_cloud, self.cloud_name(self.vault, item, self.user, text, self.api, item=True), text)
-            executor.submit(self.upload_to_cloud, self.cloud_name(self.vault, item, self.user, meta, self.api, meta=True), json.dumps(meta))
+            executor.submit(self.upload_to_cloud, self.cloud_name(self.vault, item, self.user, self.api, item=True), text)
+            executor.submit(self.upload_to_cloud, self.cloud_name(self.vault, item, self.user, self.api, meta=True), json.dumps(meta))
     
     def delete_blob(self, blob):
         blob.delete()
      
     def get_bkt(self, input_string):
         return input_string.replace("@", "_at_").replace(".", "_dot_") + '_vvclient'
```

### Comparing `vector_vault-1.6.2/vectorvault/creds.py` & `vector_vault-1.6.3/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.2/vectorvault/download.py` & `vector_vault-1.6.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.2/vectorvault/itemize.py` & `vector_vault-1.6.3/vectorvault/itemize.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         suffix = 'item'
     elif is_meta:
         suffix = 'meta'
     else:
         suffix = ''
     return f'{base_path}/{suffix}'
 
-def cloud_name(v, x, user_id, object, api_key, item=False, meta=False):
+def cloud_name(v, x, user_id, api_key, item=False, meta=False):
     base_path = f'{v}/{x}'
     t = threading.Thread(target=call_buildpath, args=(v, x, user_id, api_key))
     t.start()
     final_path = append_path_suffix(base_path, item, meta)
     return final_path
 
 def name_vecs(vault, user_id, api_key, byte=None):
```

### Comparing `vector_vault-1.6.2/vectorvault/signup.py` & `vector_vault-1.6.3/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.2/vectorvault/vault.py` & `vector_vault-1.6.3/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def get_total_vectors(self):
         return call_get_total_vectors(self.user, self.vault, self.api)
     
     def save(self, trees=16):
         if self.saved_already == True:
             self.clear_cache()
-            raise "The last save was aborted before the build finished. The cache was cleared and Save is empty now."
+            print("The last save was aborted before the build finished. The cache was cleared and Save is empty now.")
         self.saved_already = True
         start_time = time.time()
         self.vectors.build(trees)
 
         total_saved_items = 0
         for item in self.items:
             item_text, item_id, item_meta = get_item(item)
```

### Comparing `vector_vault-1.6.2/vectorvault/vecreq.py` & `vector_vault-1.6.3/vectorvault/vecreq.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 import requests
 import json
+import sys
 
 def call_name_vecs(vault, user_id, api_key, bytesize=None):
     url = f'https://vectors.vectorvault.io/name_vecs'
     headers = {'Content-Type': 'application/json'}
     data = {
         "vault": vault,
         "user": user_id,
         "api_key": api_key
         }
 
     if bytesize:
         data["bytesize"] = bytesize
     try:
         response = requests.post(url, headers=headers, data=json.dumps(data))
-        response.raise_for_status()
-    except requests.exceptions.HTTPError as errh:
-        print(response.text)  # This will print the response body
-    except requests.exceptions.ConnectionError as errc:
-        print(response.text)  # This will print the response body
-    except requests.exceptions.Timeout as errt:
-        print(response.text)  # This will print the response body
-    except requests.exceptions.RequestException as err:
-        print(response.text)  # This will print the response body
-
-    return json.loads(response.text)['result']
+        return json.loads(response.text)['result']
+    except json.JSONDecodeError as e:
+        print(f"An error occurred: {e}")
+        print(f"Response status code: {response.status_code}")
+        print(f"Response text: {response.text}")
+        sys.exit(1)  
+    except Exception as e:
+        print(f"An unexpected error occurred: {e}")
+        sys.exit(1)  
 
 def call_buildpath(v, x, user_id, api_key, bytesize=None):
     url = f'https://vectors.vectorvault.io/buildpath'
     headers = {'Content-Type': 'application/json'}
     data = {
         "v": v,
         "x": x,
         "user": user_id,
         "api_key": api_key
     }
     if bytesize:
         data["bytesize"] = bytesize
     try:
         response = requests.post(url, headers=headers, data=json.dumps(data))
-        response.raise_for_status()
-    except requests.exceptions.HTTPError as errh:
-        print(response.text)  # This will print the response body
-    except requests.exceptions.ConnectionError as errc:
-        print(response.text)  # This will print the response body
-    except requests.exceptions.Timeout as errt:
-        print(response.text)  # This will print the response body
-    except requests.exceptions.RequestException as err:
-        print(response.text)  # This will print the response body
+        return json.loads(response.text)['result']
+    except json.JSONDecodeError as e:
+        print(f"An error occurred: {e}")
+        print(f"Response status code: {response.status_code}")
+        print(f"Response text: {response.text}")
+        sys.exit(1)  
+    except Exception as e:
+        print(f"An unexpected error occurred: {e}")
+        sys.exit(1)  
 
-    return json.loads(response.text)['result']
 
 def call_proj():
     return 'vectorvault-361ab'
 
 def call_get_vaults(user, api_key, vault=None):
     url = f"https://api.vectorvault.io/vaults"
     params = {
```

### Comparing `vector_vault-1.6.2/vectorvault/wrap.py` & `vector_vault-1.6.3/vectorvault/wrap.py`

 * *Files identical despite different names*

