# Comparing `tmp/ga4_data_import-0.1.0-py3-none-any.whl.zip` & `tmp/ga4_data_import-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 30856 bytes, number of entries: 9
+Zip file size: 30850 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-May-23 23:00 ga4_data_import/__init__.py
 -rw-r--r--  2.0 unx     1122 b- defN 23-May-24 20:59 ga4_data_import/common.py
--rw-r--r--  2.0 unx     8482 b- defN 23-May-24 21:37 ga4_data_import/compute.py
+-rw-r--r--  2.0 unx     8468 b- defN 23-May-31 11:20 ga4_data_import/compute.py
 -rw-r--r--  2.0 unx      891 b- defN 23-May-24 18:36 ga4_data_import/storage.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-30 20:17 ga4_data_import-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    42812 b- defN 23-May-30 20:17 ga4_data_import-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 20:17 ga4_data_import-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-30 20:17 ga4_data_import-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      756 b- defN 23-May-30 20:17 ga4_data_import-0.1.0.dist-info/RECORD
-9 files, 89320 bytes uncompressed, 29544 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    42831 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      756 b- defN 23-May-31 11:28 ga4_data_import-0.1.1.dist-info/RECORD
+9 files, 89325 bytes uncompressed, 29538 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: ga4_data_import/compute.py
 Comment: 
 
 Filename: ga4_data_import/storage.py
 Comment: 
 
-Filename: ga4_data_import-0.1.0.dist-info/LICENSE
+Filename: ga4_data_import-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: ga4_data_import-0.1.0.dist-info/METADATA
+Filename: ga4_data_import-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: ga4_data_import-0.1.0.dist-info/WHEEL
+Filename: ga4_data_import-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ga4_data_import-0.1.0.dist-info/top_level.txt
+Filename: ga4_data_import-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ga4_data_import-0.1.0.dist-info/RECORD
+Filename: ga4_data_import-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ga4_data_import/compute.py

```diff
@@ -43,25 +43,25 @@
         project=project_id, region=region, address=address_name
     )
     address_client = AddressesClient()
 
     try:
         # Check if the address already exists
         existing_address_response = address_client.get(address_request)
-        return existing_address_response.get("address")
+        return existing_address_response.address
     except:
         # Address does not exist, create a new one
         insert_address_request = InsertAddressRequest(
             project=project_id,
             region=region,
             address_resource=Address(name=address_name, network_tier="STANDARD"),
         )
         address_client.insert(insert_address_request).result()
         new_address_response = address_client.get(address_request)
-        return new_address_response.get("address")
+        return new_address_response.address
 
 
 def create_instance(
     instance_name, project_id, zone, static_address, sftp_username, bucket_name
 ):
     """
     Create a Compute Engine instance with the provided name, project id, zone, and bucket name.
```

## Comparing `ga4_data_import-0.1.0.dist-info/LICENSE` & `ga4_data_import-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ga4_data_import-0.1.0.dist-info/METADATA` & `ga4_data_import-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ga4-data-import
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Analytics 4 Data Import code samples
 Author-email: Max Ostapenko <ga4_data_import@maxostapenko.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,18 +674,18 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/max-ostapenko/ga4_data_import
+Project-URL: Homepage, https://www.maxostapenko.com/projects/ga4_data_import
 Project-URL: Bug Reports, https://github.com/max-ostapenko/ga4_data_import/issues
-Project-URL: Funding, https://donate.pypi.org
-Project-URL: Say Thanks!, http://saythanks.io/to/example
+Project-URL: Funding, https://maxostapenko.com/donate
+Project-URL: Say Thanks!, https://www.maxostapenko.com/sponsor
 Project-URL: Source, https://github.com/max-ostapenko/ga4_data_import/
 Keywords: Google Analytics 4,Data Import,SFTP
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

