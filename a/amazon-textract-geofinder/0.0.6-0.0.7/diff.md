# Comparing `tmp/amazon-textract-geofinder-0.0.6.tar.gz` & `tmp/amazon-textract-geofinder-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-geofinder-0.0.6.tar", last modified: Mon Jul 11 17:22:38 2022, max compression
+gzip compressed data, was "amazon-textract-geofinder-0.0.7.tar", last modified: Wed May 31 01:20:40 2023, max compression
```

## Comparing `amazon-textract-geofinder-0.0.6.tar` & `amazon-textract-geofinder-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 schadem    (505) staff       (20)        0 2022-07-11 17:22:38.335620 amazon-textract-geofinder-0.0.6/
--rw-r--r--   0 schadem    (505) staff       (20)    10142 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/LICENSE
--rw-r--r--   0 schadem    (505) staff       (20)      161 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/MANIFEST.in
--rw-r--r--   0 schadem    (505) staff       (20)    12075 2022-07-11 17:22:38.335790 amazon-textract-geofinder-0.0.6/PKG-INFO
--rw-r--r--   0 schadem    (505) staff       (20)    11186 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/README.md
-drwxr-xr-x   0 schadem    (505) staff       (20)        0 2022-07-11 17:22:38.328893 amazon-textract-geofinder-0.0.6/amazon_textract_geofinder.egg-info/
--rw-r--r--   0 schadem    (505) staff       (20)    12075 2022-07-11 17:22:38.000000 amazon-textract-geofinder-0.0.6/amazon_textract_geofinder.egg-info/PKG-INFO
--rw-r--r--   0 schadem    (505) staff       (20)      555 2022-07-11 17:22:38.000000 amazon-textract-geofinder-0.0.6/amazon_textract_geofinder.egg-info/SOURCES.txt
--rw-r--r--   0 schadem    (505) staff       (20)        1 2022-07-11 17:22:38.000000 amazon-textract-geofinder-0.0.6/amazon_textract_geofinder.egg-info/dependency_links.txt
--rw-r--r--   0 schadem    (505) staff       (20)       40 2022-07-11 17:22:38.000000 amazon-textract-geofinder-0.0.6/amazon_textract_geofinder.egg-info/requires.txt
--rw-r--r--   0 schadem    (505) staff       (20)       18 2022-07-11 17:22:38.000000 amazon-textract-geofinder-0.0.6/amazon_textract_geofinder.egg-info/top_level.txt
-drwxr-xr-x   0 schadem    (505) staff       (20)        0 2022-07-11 17:22:38.329269 amazon-textract-geofinder-0.0.6/bin/
--rwxr-xr-x   0 schadem    (505) staff       (20)     1830 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/bin/amazon-textract-geofinder
--rw-r--r--   0 schadem    (505) staff       (20)      402 2022-07-11 17:22:38.336439 amazon-textract-geofinder-0.0.6/setup.cfg
--rw-r--r--   0 schadem    (505) staff       (20)     2061 2022-07-11 17:22:03.000000 amazon-textract-geofinder-0.0.6/setup.py
-drwxr-xr-x   0 schadem    (505) staff       (20)        0 2022-07-11 17:22:38.334994 amazon-textract-geofinder-0.0.6/textractgeofinder/
--rw-r--r--   0 schadem    (505) staff       (20)      137 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/textractgeofinder/__init__.py
--rw-r--r--   0 schadem    (505) staff       (20)       22 2022-07-11 17:22:03.000000 amazon-textract-geofinder-0.0.6/textractgeofinder/_version.py
--rw-r--r--   0 schadem    (505) staff       (20)     7570 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/textractgeofinder/ocrdb.py
--rw-r--r--   0 schadem    (505) staff       (20)     7739 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/textractgeofinder/sample_patient_intake_form_parser.py
--rw-r--r--   0 schadem    (505) staff       (20)    49134 2022-07-11 17:21:52.000000 amazon-textract-geofinder-0.0.6/textractgeofinder/tgeofinder.py
--rw-r--r--   0 schadem    (505) staff       (20)      193 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/textractgeofinder/tinterface.py
--rw-r--r--   0 schadem    (505) staff       (20)     9683 2022-02-24 17:56:59.000000 amazon-textract-geofinder-0.0.6/textractgeofinder/tword.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-05-31 01:20:40.804037 amazon-textract-geofinder-0.0.7/
+-rw-r--r--   0 schadem    (504) staff       (20)    10142 2022-09-08 17:40:40.000000 amazon-textract-geofinder-0.0.7/LICENSE
+-rw-r--r--   0 schadem    (504) staff       (20)      161 2022-09-08 17:40:40.000000 amazon-textract-geofinder-0.0.7/MANIFEST.in
+-rw-r--r--   0 schadem    (504) staff       (20)    13728 2023-05-31 01:20:40.804154 amazon-textract-geofinder-0.0.7/PKG-INFO
+-rw-r--r--   0 schadem    (504) staff       (20)    11186 2022-09-08 17:40:40.000000 amazon-textract-geofinder-0.0.7/README.md
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-05-31 01:20:40.801407 amazon-textract-geofinder-0.0.7/amazon_textract_geofinder.egg-info/
+-rw-r--r--   0 schadem    (504) staff       (20)    13728 2023-05-31 01:20:40.000000 amazon-textract-geofinder-0.0.7/amazon_textract_geofinder.egg-info/PKG-INFO
+-rw-r--r--   0 schadem    (504) staff       (20)      555 2023-05-31 01:20:40.000000 amazon-textract-geofinder-0.0.7/amazon_textract_geofinder.egg-info/SOURCES.txt
+-rw-r--r--   0 schadem    (504) staff       (20)        1 2023-05-31 01:20:40.000000 amazon-textract-geofinder-0.0.7/amazon_textract_geofinder.egg-info/dependency_links.txt
+-rw-r--r--   0 schadem    (504) staff       (20)       40 2023-05-31 01:20:40.000000 amazon-textract-geofinder-0.0.7/amazon_textract_geofinder.egg-info/requires.txt
+-rw-r--r--   0 schadem    (504) staff       (20)       18 2023-05-31 01:20:40.000000 amazon-textract-geofinder-0.0.7/amazon_textract_geofinder.egg-info/top_level.txt
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-05-31 01:20:40.801563 amazon-textract-geofinder-0.0.7/bin/
+-rwxr-xr-x   0 schadem    (504) staff       (20)     1830 2022-09-08 17:40:40.000000 amazon-textract-geofinder-0.0.7/bin/amazon-textract-geofinder
+-rw-r--r--   0 schadem    (504) staff       (20)      402 2023-05-31 01:20:40.804582 amazon-textract-geofinder-0.0.7/setup.cfg
+-rw-r--r--   0 schadem    (504) staff       (20)     2061 2023-05-31 01:15:11.000000 amazon-textract-geofinder-0.0.7/setup.py
+drwxr-xr-x   0 schadem    (504) staff       (20)        0 2023-05-31 01:20:40.803723 amazon-textract-geofinder-0.0.7/textractgeofinder/
+-rw-r--r--   0 schadem    (504) staff       (20)      137 2022-09-08 17:40:40.000000 amazon-textract-geofinder-0.0.7/textractgeofinder/__init__.py
+-rw-r--r--   0 schadem    (504) staff       (20)       22 2023-05-31 01:15:11.000000 amazon-textract-geofinder-0.0.7/textractgeofinder/_version.py
+-rw-r--r--   0 schadem    (504) staff       (20)     7570 2022-12-09 23:02:41.000000 amazon-textract-geofinder-0.0.7/textractgeofinder/ocrdb.py
+-rw-r--r--   0 schadem    (504) staff       (20)     7739 2022-09-08 17:40:40.000000 amazon-textract-geofinder-0.0.7/textractgeofinder/sample_patient_intake_form_parser.py
+-rw-r--r--   0 schadem    (504) staff       (20)    49175 2023-05-31 01:12:10.000000 amazon-textract-geofinder-0.0.7/textractgeofinder/tgeofinder.py
+-rw-r--r--   0 schadem    (504) staff       (20)      193 2022-09-08 17:40:40.000000 amazon-textract-geofinder-0.0.7/textractgeofinder/tinterface.py
+-rw-r--r--   0 schadem    (504) staff       (20)     9683 2022-12-09 23:02:41.000000 amazon-textract-geofinder-0.0.7/textractgeofinder/tword.py
```

### Comparing `amazon-textract-geofinder-0.0.6/LICENSE` & `amazon-textract-geofinder-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-geofinder-0.0.6/PKG-INFO` & `amazon-textract-geofinder-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: amazon-textract-geofinder
-Version: 0.0.6
-Summary: Amazon Textract package to easier access data through geometric information
-Home-page: https://github.com/aws-samples/amazon-textract-textractor/tpipelinegeofinder
-Author: Amazon Rekognition Textract Demoes
-Author-email: rekognition-textract-demos@amazon.com
-License: Apache License Version 2.0
-Keywords: amazon-textract-textractor amazon textract finder geometry geo
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Textract-Pipeline-GeoFinder
 
 Provides functions to use geometric information to extract information.
 
 Use cases include:
 * Give context to key/value pairs from the Amazon Textract AnalyzeDocument API for FORMS
 * Find values in specific areas
@@ -223,9 +202,7 @@
 | COUGH->NO                                    | SELECTED       |
 | LOSS_OF_TASTE->YES                           | NOT_SELECTED   |
 | LOSS_OF_TASTE->NO                            | SELECTED       |
 | COVID_CONTACT->YES                           | SELECTED       |
 | COVID_CONTACT->NO                            | NOT_SELECTED   |
 | TRAVEL->YES                                  | NOT_SELECTED   |
 | TRAVEL->NO                                   | SELECTED       |
-
-
```

### Comparing `amazon-textract-geofinder-0.0.6/README.md` & `amazon-textract-geofinder-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,208 +1,228 @@
-# Textract-Pipeline-GeoFinder
-
-Provides functions to use geometric information to extract information.
-
-Use cases include:
-* Give context to key/value pairs from the Amazon Textract AnalyzeDocument API for FORMS
-* Find values in specific areas
-
-# Install
-
-```bash
-> python -m pip install amazon-textract-geofinder
-```
-
-Make sure your environment is setup with AWS credentials through configuration files or environment variables or an attached role. (https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html)
-
-# Concept
-
-To find information in a document based on geometry with this library the main advantage over defining x,y coordinates where the expected value should be is the concept of an area.
-
-An area is ultimately defined by a box with x_min, y_min, x_max, y_max coordinates but can be defined by finding words/phrases in the document and then use to create the area.
-
-From there functions to parse the information in the area help to extract the information. E. g. by defining the area based on the question like 'Did you feel fever or feverish lately?' we can associate the answers to it and create a new key/value pair specific to this question.
-
-
-# Samples
-
-## Get context for key value pairs
-
-Sample image:
-
-<img src="./tests/data/patient_intake_form_sample.jpg" width=300> 
-
-The Amazon Textract AnalyzeDocument API with the FORMS feature returns the following keys:
-
-| Key                                          | Value          |
-|----------------------------------------------|----------------|
-| First Name:                                  | ALEJANDRO      |
-| First Name:                                  | CARLOS         |
-| Relationship to Patient:                     | BROTHER        |
-| First Name:                                  | JANE           |
-| Marital Status:                              | MARRIED        |
-| Phone:                                       | 646-555-0111   |
-| Last Name:                                   | SALAZAR        |
-| Phone:                                       | 212-555-0150   |
-| Relationship to Patient:                     | FRIEND         |
-| Last Name:                                   | ROSALEZ        |
-| City:                                        | ANYTOWN        |
-| Phone:                                       | 650-555-0123   |
-| Address:                                     | 123 ANY STREET |
-| Yes                                          | SELECTED       |
-| Yes                                          | NOT_SELECTED   |
-| Date of Birth:                               | 10/10/1982     |
-| Last Name:                                   | DOE            |
-| Sex:                                         | M              |
-| Yes                                          | NOT_SELECTED   |
-| Yes                                          | NOT_SELECTED   |
-| Yes                                          | NOT_SELECTED   |
-| State:                                       | CA             |
-| Zip Code:                                    | 12345          |
-| Email Address:                               |                |
-| No                                           | NOT_SELECTED   |
-| No                                           | SELECTED       |
-| No                                           | NOT_SELECTED   |
-| Yes                                          | SELECTED       |
-| No                                           | SELECTED       |
-| No                                           | SELECTED       |
-| No                                           | SELECTED       |
-
-
-But the information to which section of the document the individual keys belong is not obvious. Most keys appear multiple times and we want to give them context to associate them with the 'Patient', 'Emergency Contact 1', 'Emergency Contact 2' or specific questions.
-
-
-This Jupyter notebook that walks through the sample: [sample notebook](./geofinder-sample-notebook.ipynb)
-Make sure to have AWS credentials setup when starting the notebook locally or use a SageMaker notebook with a role including permissions for Amazon Textract. 
-
-This code snippet is take from the notebook.
-
-```bash
-python -m pip install amazon-textract-helper amazon-textract-geofinder
-```
-
-```python
-from textractgeofinder.ocrdb import AreaSelection
-from textractgeofinder.tgeofinder import KeyValue, TGeoFinder, AreaSelection, SelectionElement
-from textractprettyprinter.t_pretty_print import get_forms_string
-from textractcaller import call_textract
-from textractcaller.t_call import Textract_Features
-
-import trp.trp2 as t2
-
-image_filename='./tests/data/patient_intake_form_sample.jpg'
-
-j = call_textract(input_document=image_filename, features=[Textract_Features.FORMS])
-
-
-t_document = t2.TDocumentSchema().load(j)
-doc_height = 1000
-doc_width = 1000
-geofinder_doc = TGeoFinder(j, doc_height=doc_height, doc_width=doc_width)
-
-def set_hierarchy_kv(list_kv: list[KeyValue], t_document: t2.TDocument, page_block: t2.TBlock, prefix="BORROWER"):
-    for x in list_kv:
-        t_document.add_virtual_key_for_existing_key(key_name=f"{prefix}_{x.key.text}",
-                                                    existing_key=t_document.get_block_by_id(x.key.id),
-                                                    page_block=page_block)
-# patient information
-patient_information = geofinder_doc.find_phrase_on_page("patient information")[0]
-emergency_contact_1 = geofinder_doc.find_phrase_on_page("emergency contact 1:", min_textdistance=0.99)[0]
-top_left = t2.TPoint(y=patient_information.ymax, x=0)
-lower_right = t2.TPoint(y=emergency_contact_1.ymin, x=doc_width)
-form_fields = geofinder_doc.get_form_fields_in_area(
-    area_selection=AreaSelection(top_left=top_left, lower_right=lower_right))
-set_hierarchy_kv(list_kv=form_fields, t_document=t_document, prefix='PATIENT', page_block=t_document.pages[0])
-
-set_hierarchy_kv(list_kv=form_fields, t_document=t_document, prefix='PATIENT', page_block=t_document.pages[0])
-
-print(get_forms_string(t2.TDocumentSchema().dump(t_document)))
-```
-
-| Key                     | Value          |
-|-------------------------|----------------|
-| ...                     | ...            |
-| PATIENT_first name:     | ALEJANDRO      |
-| PATIENT_address:        | 123 ANY STREET |
-| PATIENT_sex:            | M              |
-| PATIENT_state:          | CA             |
-| PATIENT_zip code:       | 12345          |
-| PATIENT_marital status: | MARRIED        |
-| PATIENT_last name:      | ROSALEZ        |
-| PATIENT_phone:          | 646-555-0111   |
-| PATIENT_email address:  |                |
-| PATIENT_city:           | ANYTOWN        |
-| PATIENT_date of birth:  | 10/10/1982     |
-
-## Using the Amazon Textact Helper command line tool with the sample
-
-This will show the full result, like the notebook.
-
-```bash
-> python -m pip install amazon-textract-helper amazon-textract-geofinder
-> cat tests/data/patient_intake_form_sample.json| bin/amazon-textract-geofinder | amazon-textract --stdin --pretty-print FORMS
-```
-
-| Key                     | Value          |
-|-------------------------|----------------|
-| First Name:                                  | ALEJANDRO      |
-| First Name:                                  | CARLOS         |
-| Relationship to Patient:                     | BROTHER        |
-| First Name:                                  | JANE           |
-| Marital Status:                              | MARRIED        |
-| Phone:                                       | 646-555-0111   |
-| Last Name:                                   | SALAZAR        |
-| Phone:                                       | 212-555-0150   |
-| Relationship to Patient:                     | FRIEND         |
-| Last Name:                                   | ROSALEZ        |
-| City:                                        | ANYTOWN        |
-| Phone:                                       | 650-555-0123   |
-| Address:                                     | 123 ANY STREET |
-| Yes                                          | SELECTED       |
-| Yes                                          | NOT_SELECTED   |
-| Date of Birth:                               | 10/10/1982     |
-| Last Name:                                   | DOE            |
-| Sex:                                         | M              |
-| Yes                                          | NOT_SELECTED   |
-| Yes                                          | NOT_SELECTED   |
-| Yes                                          | NOT_SELECTED   |
-| State:                                       | CA             |
-| Zip Code:                                    | 12345          |
-| Email Address:                               |                |
-| No                                           | NOT_SELECTED   |
-| No                                           | SELECTED       |
-| No                                           | NOT_SELECTED   |
-| Yes                                          | SELECTED       |
-| No                                           | SELECTED       |
-| No                                           | SELECTED       |
-| No                                           | SELECTED       |
-| PATIENT_first name:                          | ALEJANDRO      |
-| PATIENT_address:                             | 123 ANY STREET |
-| PATIENT_sex:                                 | M              |
-| PATIENT_state:                               | CA             |
-| PATIENT_zip code:                            | 12345          |
-| PATIENT_marital status:                      | MARRIED        |
-| PATIENT_last name:                           | ROSALEZ        |
-| PATIENT_phone:                               | 646-555-0111   |
-| PATIENT_email address:                       |                |
-| PATIENT_city:                                | ANYTOWN        |
-| PATIENT_date of birth:                       | 10/10/1982     |
-| EMERGENCY_CONTACT_1_first name:              | CARLOS         |
-| EMERGENCY_CONTACT_1_phone:                   | 212-555-0150   |
-| EMERGENCY_CONTACT_1_relationship to patient: | BROTHER        |
-| EMERGENCY_CONTACT_1_last name:               | SALAZAR        |
-| EMERGENCY_CONTACT_2_first name:              | JANE           |
-| EMERGENCY_CONTACT_2_phone:                   | 650-555-0123   |
-| EMERGENCY_CONTACT_2_last name:               | DOE            |
-| EMERGENCY_CONTACT_2_relationship to patient: | FRIEND         |
-| FEVER->YES                                   | SELECTED       |
-| FEVER->NO                                    | NOT_SELECTED   |
-| SHORTNESS->YES                               | NOT_SELECTED   |
-| SHORTNESS->NO                                | SELECTED       |
-| COUGH->YES                                   | NOT_SELECTED   |
-| COUGH->NO                                    | SELECTED       |
-| LOSS_OF_TASTE->YES                           | NOT_SELECTED   |
-| LOSS_OF_TASTE->NO                            | SELECTED       |
-| COVID_CONTACT->YES                           | SELECTED       |
-| COVID_CONTACT->NO                            | NOT_SELECTED   |
-| TRAVEL->YES                                  | NOT_SELECTED   |
-| TRAVEL->NO                                   | SELECTED       |
+Metadata-Version: 2.1
+Name: amazon-textract-geofinder
+Version: 0.0.7
+Summary: Amazon Textract package to easier access data through geometric information
+Home-page: https://github.com/aws-samples/amazon-textract-textractor/tpipelinegeofinder
+Author: Amazon Rekognition Textract Demoes
+Author-email: rekognition-textract-demos@amazon.com
+License: Apache License Version 2.0
+Description: # Textract-Pipeline-GeoFinder
+        
+        Provides functions to use geometric information to extract information.
+        
+        Use cases include:
+        * Give context to key/value pairs from the Amazon Textract AnalyzeDocument API for FORMS
+        * Find values in specific areas
+        
+        # Install
+        
+        ```bash
+        > python -m pip install amazon-textract-geofinder
+        ```
+        
+        Make sure your environment is setup with AWS credentials through configuration files or environment variables or an attached role. (https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html)
+        
+        # Concept
+        
+        To find information in a document based on geometry with this library the main advantage over defining x,y coordinates where the expected value should be is the concept of an area.
+        
+        An area is ultimately defined by a box with x_min, y_min, x_max, y_max coordinates but can be defined by finding words/phrases in the document and then use to create the area.
+        
+        From there functions to parse the information in the area help to extract the information. E. g. by defining the area based on the question like 'Did you feel fever or feverish lately?' we can associate the answers to it and create a new key/value pair specific to this question.
+        
+        
+        # Samples
+        
+        ## Get context for key value pairs
+        
+        Sample image:
+        
+        <img src="./tests/data/patient_intake_form_sample.jpg" width=300> 
+        
+        The Amazon Textract AnalyzeDocument API with the FORMS feature returns the following keys:
+        
+        | Key                                          | Value          |
+        |----------------------------------------------|----------------|
+        | First Name:                                  | ALEJANDRO      |
+        | First Name:                                  | CARLOS         |
+        | Relationship to Patient:                     | BROTHER        |
+        | First Name:                                  | JANE           |
+        | Marital Status:                              | MARRIED        |
+        | Phone:                                       | 646-555-0111   |
+        | Last Name:                                   | SALAZAR        |
+        | Phone:                                       | 212-555-0150   |
+        | Relationship to Patient:                     | FRIEND         |
+        | Last Name:                                   | ROSALEZ        |
+        | City:                                        | ANYTOWN        |
+        | Phone:                                       | 650-555-0123   |
+        | Address:                                     | 123 ANY STREET |
+        | Yes                                          | SELECTED       |
+        | Yes                                          | NOT_SELECTED   |
+        | Date of Birth:                               | 10/10/1982     |
+        | Last Name:                                   | DOE            |
+        | Sex:                                         | M              |
+        | Yes                                          | NOT_SELECTED   |
+        | Yes                                          | NOT_SELECTED   |
+        | Yes                                          | NOT_SELECTED   |
+        | State:                                       | CA             |
+        | Zip Code:                                    | 12345          |
+        | Email Address:                               |                |
+        | No                                           | NOT_SELECTED   |
+        | No                                           | SELECTED       |
+        | No                                           | NOT_SELECTED   |
+        | Yes                                          | SELECTED       |
+        | No                                           | SELECTED       |
+        | No                                           | SELECTED       |
+        | No                                           | SELECTED       |
+        
+        
+        But the information to which section of the document the individual keys belong is not obvious. Most keys appear multiple times and we want to give them context to associate them with the 'Patient', 'Emergency Contact 1', 'Emergency Contact 2' or specific questions.
+        
+        
+        This Jupyter notebook that walks through the sample: [sample notebook](./geofinder-sample-notebook.ipynb)
+        Make sure to have AWS credentials setup when starting the notebook locally or use a SageMaker notebook with a role including permissions for Amazon Textract. 
+        
+        This code snippet is take from the notebook.
+        
+        ```bash
+        python -m pip install amazon-textract-helper amazon-textract-geofinder
+        ```
+        
+        ```python
+        from textractgeofinder.ocrdb import AreaSelection
+        from textractgeofinder.tgeofinder import KeyValue, TGeoFinder, AreaSelection, SelectionElement
+        from textractprettyprinter.t_pretty_print import get_forms_string
+        from textractcaller import call_textract
+        from textractcaller.t_call import Textract_Features
+        
+        import trp.trp2 as t2
+        
+        image_filename='./tests/data/patient_intake_form_sample.jpg'
+        
+        j = call_textract(input_document=image_filename, features=[Textract_Features.FORMS])
+        
+        
+        t_document = t2.TDocumentSchema().load(j)
+        doc_height = 1000
+        doc_width = 1000
+        geofinder_doc = TGeoFinder(j, doc_height=doc_height, doc_width=doc_width)
+        
+        def set_hierarchy_kv(list_kv: list[KeyValue], t_document: t2.TDocument, page_block: t2.TBlock, prefix="BORROWER"):
+            for x in list_kv:
+                t_document.add_virtual_key_for_existing_key(key_name=f"{prefix}_{x.key.text}",
+                                                            existing_key=t_document.get_block_by_id(x.key.id),
+                                                            page_block=page_block)
+        # patient information
+        patient_information = geofinder_doc.find_phrase_on_page("patient information")[0]
+        emergency_contact_1 = geofinder_doc.find_phrase_on_page("emergency contact 1:", min_textdistance=0.99)[0]
+        top_left = t2.TPoint(y=patient_information.ymax, x=0)
+        lower_right = t2.TPoint(y=emergency_contact_1.ymin, x=doc_width)
+        form_fields = geofinder_doc.get_form_fields_in_area(
+            area_selection=AreaSelection(top_left=top_left, lower_right=lower_right))
+        set_hierarchy_kv(list_kv=form_fields, t_document=t_document, prefix='PATIENT', page_block=t_document.pages[0])
+        
+        set_hierarchy_kv(list_kv=form_fields, t_document=t_document, prefix='PATIENT', page_block=t_document.pages[0])
+        
+        print(get_forms_string(t2.TDocumentSchema().dump(t_document)))
+        ```
+        
+        | Key                     | Value          |
+        |-------------------------|----------------|
+        | ...                     | ...            |
+        | PATIENT_first name:     | ALEJANDRO      |
+        | PATIENT_address:        | 123 ANY STREET |
+        | PATIENT_sex:            | M              |
+        | PATIENT_state:          | CA             |
+        | PATIENT_zip code:       | 12345          |
+        | PATIENT_marital status: | MARRIED        |
+        | PATIENT_last name:      | ROSALEZ        |
+        | PATIENT_phone:          | 646-555-0111   |
+        | PATIENT_email address:  |                |
+        | PATIENT_city:           | ANYTOWN        |
+        | PATIENT_date of birth:  | 10/10/1982     |
+        
+        ## Using the Amazon Textact Helper command line tool with the sample
+        
+        This will show the full result, like the notebook.
+        
+        ```bash
+        > python -m pip install amazon-textract-helper amazon-textract-geofinder
+        > cat tests/data/patient_intake_form_sample.json| bin/amazon-textract-geofinder | amazon-textract --stdin --pretty-print FORMS
+        ```
+        
+        | Key                     | Value          |
+        |-------------------------|----------------|
+        | First Name:                                  | ALEJANDRO      |
+        | First Name:                                  | CARLOS         |
+        | Relationship to Patient:                     | BROTHER        |
+        | First Name:                                  | JANE           |
+        | Marital Status:                              | MARRIED        |
+        | Phone:                                       | 646-555-0111   |
+        | Last Name:                                   | SALAZAR        |
+        | Phone:                                       | 212-555-0150   |
+        | Relationship to Patient:                     | FRIEND         |
+        | Last Name:                                   | ROSALEZ        |
+        | City:                                        | ANYTOWN        |
+        | Phone:                                       | 650-555-0123   |
+        | Address:                                     | 123 ANY STREET |
+        | Yes                                          | SELECTED       |
+        | Yes                                          | NOT_SELECTED   |
+        | Date of Birth:                               | 10/10/1982     |
+        | Last Name:                                   | DOE            |
+        | Sex:                                         | M              |
+        | Yes                                          | NOT_SELECTED   |
+        | Yes                                          | NOT_SELECTED   |
+        | Yes                                          | NOT_SELECTED   |
+        | State:                                       | CA             |
+        | Zip Code:                                    | 12345          |
+        | Email Address:                               |                |
+        | No                                           | NOT_SELECTED   |
+        | No                                           | SELECTED       |
+        | No                                           | NOT_SELECTED   |
+        | Yes                                          | SELECTED       |
+        | No                                           | SELECTED       |
+        | No                                           | SELECTED       |
+        | No                                           | SELECTED       |
+        | PATIENT_first name:                          | ALEJANDRO      |
+        | PATIENT_address:                             | 123 ANY STREET |
+        | PATIENT_sex:                                 | M              |
+        | PATIENT_state:                               | CA             |
+        | PATIENT_zip code:                            | 12345          |
+        | PATIENT_marital status:                      | MARRIED        |
+        | PATIENT_last name:                           | ROSALEZ        |
+        | PATIENT_phone:                               | 646-555-0111   |
+        | PATIENT_email address:                       |                |
+        | PATIENT_city:                                | ANYTOWN        |
+        | PATIENT_date of birth:                       | 10/10/1982     |
+        | EMERGENCY_CONTACT_1_first name:              | CARLOS         |
+        | EMERGENCY_CONTACT_1_phone:                   | 212-555-0150   |
+        | EMERGENCY_CONTACT_1_relationship to patient: | BROTHER        |
+        | EMERGENCY_CONTACT_1_last name:               | SALAZAR        |
+        | EMERGENCY_CONTACT_2_first name:              | JANE           |
+        | EMERGENCY_CONTACT_2_phone:                   | 650-555-0123   |
+        | EMERGENCY_CONTACT_2_last name:               | DOE            |
+        | EMERGENCY_CONTACT_2_relationship to patient: | FRIEND         |
+        | FEVER->YES                                   | SELECTED       |
+        | FEVER->NO                                    | NOT_SELECTED   |
+        | SHORTNESS->YES                               | NOT_SELECTED   |
+        | SHORTNESS->NO                                | SELECTED       |
+        | COUGH->YES                                   | NOT_SELECTED   |
+        | COUGH->NO                                    | SELECTED       |
+        | LOSS_OF_TASTE->YES                           | NOT_SELECTED   |
+        | LOSS_OF_TASTE->NO                            | SELECTED       |
+        | COVID_CONTACT->YES                           | SELECTED       |
+        | COVID_CONTACT->NO                            | NOT_SELECTED   |
+        | TRAVEL->YES                                  | NOT_SELECTED   |
+        | TRAVEL->NO                                   | SELECTED       |
+        
+Keywords: amazon-textract-textractor amazon textract finder geometry geo
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `amazon-textract-geofinder-0.0.6/amazon_textract_geofinder.egg-info/PKG-INFO` & `amazon-textract-geofinder-0.0.7/amazon_textract_geofinder.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,231 +1,228 @@
 Metadata-Version: 2.1
 Name: amazon-textract-geofinder
-Version: 0.0.6
+Version: 0.0.7
 Summary: Amazon Textract package to easier access data through geometric information
 Home-page: https://github.com/aws-samples/amazon-textract-textractor/tpipelinegeofinder
 Author: Amazon Rekognition Textract Demoes
 Author-email: rekognition-textract-demos@amazon.com
 License: Apache License Version 2.0
+Description: # Textract-Pipeline-GeoFinder
+        
+        Provides functions to use geometric information to extract information.
+        
+        Use cases include:
+        * Give context to key/value pairs from the Amazon Textract AnalyzeDocument API for FORMS
+        * Find values in specific areas
+        
+        # Install
+        
+        ```bash
+        > python -m pip install amazon-textract-geofinder
+        ```
+        
+        Make sure your environment is setup with AWS credentials through configuration files or environment variables or an attached role. (https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html)
+        
+        # Concept
+        
+        To find information in a document based on geometry with this library the main advantage over defining x,y coordinates where the expected value should be is the concept of an area.
+        
+        An area is ultimately defined by a box with x_min, y_min, x_max, y_max coordinates but can be defined by finding words/phrases in the document and then use to create the area.
+        
+        From there functions to parse the information in the area help to extract the information. E. g. by defining the area based on the question like 'Did you feel fever or feverish lately?' we can associate the answers to it and create a new key/value pair specific to this question.
+        
+        
+        # Samples
+        
+        ## Get context for key value pairs
+        
+        Sample image:
+        
+        <img src="./tests/data/patient_intake_form_sample.jpg" width=300> 
+        
+        The Amazon Textract AnalyzeDocument API with the FORMS feature returns the following keys:
+        
+        | Key                                          | Value          |
+        |----------------------------------------------|----------------|
+        | First Name:                                  | ALEJANDRO      |
+        | First Name:                                  | CARLOS         |
+        | Relationship to Patient:                     | BROTHER        |
+        | First Name:                                  | JANE           |
+        | Marital Status:                              | MARRIED        |
+        | Phone:                                       | 646-555-0111   |
+        | Last Name:                                   | SALAZAR        |
+        | Phone:                                       | 212-555-0150   |
+        | Relationship to Patient:                     | FRIEND         |
+        | Last Name:                                   | ROSALEZ        |
+        | City:                                        | ANYTOWN        |
+        | Phone:                                       | 650-555-0123   |
+        | Address:                                     | 123 ANY STREET |
+        | Yes                                          | SELECTED       |
+        | Yes                                          | NOT_SELECTED   |
+        | Date of Birth:                               | 10/10/1982     |
+        | Last Name:                                   | DOE            |
+        | Sex:                                         | M              |
+        | Yes                                          | NOT_SELECTED   |
+        | Yes                                          | NOT_SELECTED   |
+        | Yes                                          | NOT_SELECTED   |
+        | State:                                       | CA             |
+        | Zip Code:                                    | 12345          |
+        | Email Address:                               |                |
+        | No                                           | NOT_SELECTED   |
+        | No                                           | SELECTED       |
+        | No                                           | NOT_SELECTED   |
+        | Yes                                          | SELECTED       |
+        | No                                           | SELECTED       |
+        | No                                           | SELECTED       |
+        | No                                           | SELECTED       |
+        
+        
+        But the information to which section of the document the individual keys belong is not obvious. Most keys appear multiple times and we want to give them context to associate them with the 'Patient', 'Emergency Contact 1', 'Emergency Contact 2' or specific questions.
+        
+        
+        This Jupyter notebook that walks through the sample: [sample notebook](./geofinder-sample-notebook.ipynb)
+        Make sure to have AWS credentials setup when starting the notebook locally or use a SageMaker notebook with a role including permissions for Amazon Textract. 
+        
+        This code snippet is take from the notebook.
+        
+        ```bash
+        python -m pip install amazon-textract-helper amazon-textract-geofinder
+        ```
+        
+        ```python
+        from textractgeofinder.ocrdb import AreaSelection
+        from textractgeofinder.tgeofinder import KeyValue, TGeoFinder, AreaSelection, SelectionElement
+        from textractprettyprinter.t_pretty_print import get_forms_string
+        from textractcaller import call_textract
+        from textractcaller.t_call import Textract_Features
+        
+        import trp.trp2 as t2
+        
+        image_filename='./tests/data/patient_intake_form_sample.jpg'
+        
+        j = call_textract(input_document=image_filename, features=[Textract_Features.FORMS])
+        
+        
+        t_document = t2.TDocumentSchema().load(j)
+        doc_height = 1000
+        doc_width = 1000
+        geofinder_doc = TGeoFinder(j, doc_height=doc_height, doc_width=doc_width)
+        
+        def set_hierarchy_kv(list_kv: list[KeyValue], t_document: t2.TDocument, page_block: t2.TBlock, prefix="BORROWER"):
+            for x in list_kv:
+                t_document.add_virtual_key_for_existing_key(key_name=f"{prefix}_{x.key.text}",
+                                                            existing_key=t_document.get_block_by_id(x.key.id),
+                                                            page_block=page_block)
+        # patient information
+        patient_information = geofinder_doc.find_phrase_on_page("patient information")[0]
+        emergency_contact_1 = geofinder_doc.find_phrase_on_page("emergency contact 1:", min_textdistance=0.99)[0]
+        top_left = t2.TPoint(y=patient_information.ymax, x=0)
+        lower_right = t2.TPoint(y=emergency_contact_1.ymin, x=doc_width)
+        form_fields = geofinder_doc.get_form_fields_in_area(
+            area_selection=AreaSelection(top_left=top_left, lower_right=lower_right))
+        set_hierarchy_kv(list_kv=form_fields, t_document=t_document, prefix='PATIENT', page_block=t_document.pages[0])
+        
+        set_hierarchy_kv(list_kv=form_fields, t_document=t_document, prefix='PATIENT', page_block=t_document.pages[0])
+        
+        print(get_forms_string(t2.TDocumentSchema().dump(t_document)))
+        ```
+        
+        | Key                     | Value          |
+        |-------------------------|----------------|
+        | ...                     | ...            |
+        | PATIENT_first name:     | ALEJANDRO      |
+        | PATIENT_address:        | 123 ANY STREET |
+        | PATIENT_sex:            | M              |
+        | PATIENT_state:          | CA             |
+        | PATIENT_zip code:       | 12345          |
+        | PATIENT_marital status: | MARRIED        |
+        | PATIENT_last name:      | ROSALEZ        |
+        | PATIENT_phone:          | 646-555-0111   |
+        | PATIENT_email address:  |                |
+        | PATIENT_city:           | ANYTOWN        |
+        | PATIENT_date of birth:  | 10/10/1982     |
+        
+        ## Using the Amazon Textact Helper command line tool with the sample
+        
+        This will show the full result, like the notebook.
+        
+        ```bash
+        > python -m pip install amazon-textract-helper amazon-textract-geofinder
+        > cat tests/data/patient_intake_form_sample.json| bin/amazon-textract-geofinder | amazon-textract --stdin --pretty-print FORMS
+        ```
+        
+        | Key                     | Value          |
+        |-------------------------|----------------|
+        | First Name:                                  | ALEJANDRO      |
+        | First Name:                                  | CARLOS         |
+        | Relationship to Patient:                     | BROTHER        |
+        | First Name:                                  | JANE           |
+        | Marital Status:                              | MARRIED        |
+        | Phone:                                       | 646-555-0111   |
+        | Last Name:                                   | SALAZAR        |
+        | Phone:                                       | 212-555-0150   |
+        | Relationship to Patient:                     | FRIEND         |
+        | Last Name:                                   | ROSALEZ        |
+        | City:                                        | ANYTOWN        |
+        | Phone:                                       | 650-555-0123   |
+        | Address:                                     | 123 ANY STREET |
+        | Yes                                          | SELECTED       |
+        | Yes                                          | NOT_SELECTED   |
+        | Date of Birth:                               | 10/10/1982     |
+        | Last Name:                                   | DOE            |
+        | Sex:                                         | M              |
+        | Yes                                          | NOT_SELECTED   |
+        | Yes                                          | NOT_SELECTED   |
+        | Yes                                          | NOT_SELECTED   |
+        | State:                                       | CA             |
+        | Zip Code:                                    | 12345          |
+        | Email Address:                               |                |
+        | No                                           | NOT_SELECTED   |
+        | No                                           | SELECTED       |
+        | No                                           | NOT_SELECTED   |
+        | Yes                                          | SELECTED       |
+        | No                                           | SELECTED       |
+        | No                                           | SELECTED       |
+        | No                                           | SELECTED       |
+        | PATIENT_first name:                          | ALEJANDRO      |
+        | PATIENT_address:                             | 123 ANY STREET |
+        | PATIENT_sex:                                 | M              |
+        | PATIENT_state:                               | CA             |
+        | PATIENT_zip code:                            | 12345          |
+        | PATIENT_marital status:                      | MARRIED        |
+        | PATIENT_last name:                           | ROSALEZ        |
+        | PATIENT_phone:                               | 646-555-0111   |
+        | PATIENT_email address:                       |                |
+        | PATIENT_city:                                | ANYTOWN        |
+        | PATIENT_date of birth:                       | 10/10/1982     |
+        | EMERGENCY_CONTACT_1_first name:              | CARLOS         |
+        | EMERGENCY_CONTACT_1_phone:                   | 212-555-0150   |
+        | EMERGENCY_CONTACT_1_relationship to patient: | BROTHER        |
+        | EMERGENCY_CONTACT_1_last name:               | SALAZAR        |
+        | EMERGENCY_CONTACT_2_first name:              | JANE           |
+        | EMERGENCY_CONTACT_2_phone:                   | 650-555-0123   |
+        | EMERGENCY_CONTACT_2_last name:               | DOE            |
+        | EMERGENCY_CONTACT_2_relationship to patient: | FRIEND         |
+        | FEVER->YES                                   | SELECTED       |
+        | FEVER->NO                                    | NOT_SELECTED   |
+        | SHORTNESS->YES                               | NOT_SELECTED   |
+        | SHORTNESS->NO                                | SELECTED       |
+        | COUGH->YES                                   | NOT_SELECTED   |
+        | COUGH->NO                                    | SELECTED       |
+        | LOSS_OF_TASTE->YES                           | NOT_SELECTED   |
+        | LOSS_OF_TASTE->NO                            | SELECTED       |
+        | COVID_CONTACT->YES                           | SELECTED       |
+        | COVID_CONTACT->NO                            | NOT_SELECTED   |
+        | TRAVEL->YES                                  | NOT_SELECTED   |
+        | TRAVEL->NO                                   | SELECTED       |
+        
 Keywords: amazon-textract-textractor amazon textract finder geometry geo
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Textract-Pipeline-GeoFinder
-
-Provides functions to use geometric information to extract information.
-
-Use cases include:
-* Give context to key/value pairs from the Amazon Textract AnalyzeDocument API for FORMS
-* Find values in specific areas
-
-# Install
-
-```bash
-> python -m pip install amazon-textract-geofinder
-```
-
-Make sure your environment is setup with AWS credentials through configuration files or environment variables or an attached role. (https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html)
-
-# Concept
-
-To find information in a document based on geometry with this library the main advantage over defining x,y coordinates where the expected value should be is the concept of an area.
-
-An area is ultimately defined by a box with x_min, y_min, x_max, y_max coordinates but can be defined by finding words/phrases in the document and then use to create the area.
-
-From there functions to parse the information in the area help to extract the information. E. g. by defining the area based on the question like 'Did you feel fever or feverish lately?' we can associate the answers to it and create a new key/value pair specific to this question.
-
-
-# Samples
-
-## Get context for key value pairs
-
-Sample image:
-
-<img src="./tests/data/patient_intake_form_sample.jpg" width=300> 
-
-The Amazon Textract AnalyzeDocument API with the FORMS feature returns the following keys:
-
-| Key                                          | Value          |
-|----------------------------------------------|----------------|
-| First Name:                                  | ALEJANDRO      |
-| First Name:                                  | CARLOS         |
-| Relationship to Patient:                     | BROTHER        |
-| First Name:                                  | JANE           |
-| Marital Status:                              | MARRIED        |
-| Phone:                                       | 646-555-0111   |
-| Last Name:                                   | SALAZAR        |
-| Phone:                                       | 212-555-0150   |
-| Relationship to Patient:                     | FRIEND         |
-| Last Name:                                   | ROSALEZ        |
-| City:                                        | ANYTOWN        |
-| Phone:                                       | 650-555-0123   |
-| Address:                                     | 123 ANY STREET |
-| Yes                                          | SELECTED       |
-| Yes                                          | NOT_SELECTED   |
-| Date of Birth:                               | 10/10/1982     |
-| Last Name:                                   | DOE            |
-| Sex:                                         | M              |
-| Yes                                          | NOT_SELECTED   |
-| Yes                                          | NOT_SELECTED   |
-| Yes                                          | NOT_SELECTED   |
-| State:                                       | CA             |
-| Zip Code:                                    | 12345          |
-| Email Address:                               |                |
-| No                                           | NOT_SELECTED   |
-| No                                           | SELECTED       |
-| No                                           | NOT_SELECTED   |
-| Yes                                          | SELECTED       |
-| No                                           | SELECTED       |
-| No                                           | SELECTED       |
-| No                                           | SELECTED       |
-
-
-But the information to which section of the document the individual keys belong is not obvious. Most keys appear multiple times and we want to give them context to associate them with the 'Patient', 'Emergency Contact 1', 'Emergency Contact 2' or specific questions.
-
-
-This Jupyter notebook that walks through the sample: [sample notebook](./geofinder-sample-notebook.ipynb)
-Make sure to have AWS credentials setup when starting the notebook locally or use a SageMaker notebook with a role including permissions for Amazon Textract. 
-
-This code snippet is take from the notebook.
-
-```bash
-python -m pip install amazon-textract-helper amazon-textract-geofinder
-```
-
-```python
-from textractgeofinder.ocrdb import AreaSelection
-from textractgeofinder.tgeofinder import KeyValue, TGeoFinder, AreaSelection, SelectionElement
-from textractprettyprinter.t_pretty_print import get_forms_string
-from textractcaller import call_textract
-from textractcaller.t_call import Textract_Features
-
-import trp.trp2 as t2
-
-image_filename='./tests/data/patient_intake_form_sample.jpg'
-
-j = call_textract(input_document=image_filename, features=[Textract_Features.FORMS])
-
-
-t_document = t2.TDocumentSchema().load(j)
-doc_height = 1000
-doc_width = 1000
-geofinder_doc = TGeoFinder(j, doc_height=doc_height, doc_width=doc_width)
-
-def set_hierarchy_kv(list_kv: list[KeyValue], t_document: t2.TDocument, page_block: t2.TBlock, prefix="BORROWER"):
-    for x in list_kv:
-        t_document.add_virtual_key_for_existing_key(key_name=f"{prefix}_{x.key.text}",
-                                                    existing_key=t_document.get_block_by_id(x.key.id),
-                                                    page_block=page_block)
-# patient information
-patient_information = geofinder_doc.find_phrase_on_page("patient information")[0]
-emergency_contact_1 = geofinder_doc.find_phrase_on_page("emergency contact 1:", min_textdistance=0.99)[0]
-top_left = t2.TPoint(y=patient_information.ymax, x=0)
-lower_right = t2.TPoint(y=emergency_contact_1.ymin, x=doc_width)
-form_fields = geofinder_doc.get_form_fields_in_area(
-    area_selection=AreaSelection(top_left=top_left, lower_right=lower_right))
-set_hierarchy_kv(list_kv=form_fields, t_document=t_document, prefix='PATIENT', page_block=t_document.pages[0])
-
-set_hierarchy_kv(list_kv=form_fields, t_document=t_document, prefix='PATIENT', page_block=t_document.pages[0])
-
-print(get_forms_string(t2.TDocumentSchema().dump(t_document)))
-```
-
-| Key                     | Value          |
-|-------------------------|----------------|
-| ...                     | ...            |
-| PATIENT_first name:     | ALEJANDRO      |
-| PATIENT_address:        | 123 ANY STREET |
-| PATIENT_sex:            | M              |
-| PATIENT_state:          | CA             |
-| PATIENT_zip code:       | 12345          |
-| PATIENT_marital status: | MARRIED        |
-| PATIENT_last name:      | ROSALEZ        |
-| PATIENT_phone:          | 646-555-0111   |
-| PATIENT_email address:  |                |
-| PATIENT_city:           | ANYTOWN        |
-| PATIENT_date of birth:  | 10/10/1982     |
-
-## Using the Amazon Textact Helper command line tool with the sample
-
-This will show the full result, like the notebook.
-
-```bash
-> python -m pip install amazon-textract-helper amazon-textract-geofinder
-> cat tests/data/patient_intake_form_sample.json| bin/amazon-textract-geofinder | amazon-textract --stdin --pretty-print FORMS
-```
-
-| Key                     | Value          |
-|-------------------------|----------------|
-| First Name:                                  | ALEJANDRO      |
-| First Name:                                  | CARLOS         |
-| Relationship to Patient:                     | BROTHER        |
-| First Name:                                  | JANE           |
-| Marital Status:                              | MARRIED        |
-| Phone:                                       | 646-555-0111   |
-| Last Name:                                   | SALAZAR        |
-| Phone:                                       | 212-555-0150   |
-| Relationship to Patient:                     | FRIEND         |
-| Last Name:                                   | ROSALEZ        |
-| City:                                        | ANYTOWN        |
-| Phone:                                       | 650-555-0123   |
-| Address:                                     | 123 ANY STREET |
-| Yes                                          | SELECTED       |
-| Yes                                          | NOT_SELECTED   |
-| Date of Birth:                               | 10/10/1982     |
-| Last Name:                                   | DOE            |
-| Sex:                                         | M              |
-| Yes                                          | NOT_SELECTED   |
-| Yes                                          | NOT_SELECTED   |
-| Yes                                          | NOT_SELECTED   |
-| State:                                       | CA             |
-| Zip Code:                                    | 12345          |
-| Email Address:                               |                |
-| No                                           | NOT_SELECTED   |
-| No                                           | SELECTED       |
-| No                                           | NOT_SELECTED   |
-| Yes                                          | SELECTED       |
-| No                                           | SELECTED       |
-| No                                           | SELECTED       |
-| No                                           | SELECTED       |
-| PATIENT_first name:                          | ALEJANDRO      |
-| PATIENT_address:                             | 123 ANY STREET |
-| PATIENT_sex:                                 | M              |
-| PATIENT_state:                               | CA             |
-| PATIENT_zip code:                            | 12345          |
-| PATIENT_marital status:                      | MARRIED        |
-| PATIENT_last name:                           | ROSALEZ        |
-| PATIENT_phone:                               | 646-555-0111   |
-| PATIENT_email address:                       |                |
-| PATIENT_city:                                | ANYTOWN        |
-| PATIENT_date of birth:                       | 10/10/1982     |
-| EMERGENCY_CONTACT_1_first name:              | CARLOS         |
-| EMERGENCY_CONTACT_1_phone:                   | 212-555-0150   |
-| EMERGENCY_CONTACT_1_relationship to patient: | BROTHER        |
-| EMERGENCY_CONTACT_1_last name:               | SALAZAR        |
-| EMERGENCY_CONTACT_2_first name:              | JANE           |
-| EMERGENCY_CONTACT_2_phone:                   | 650-555-0123   |
-| EMERGENCY_CONTACT_2_last name:               | DOE            |
-| EMERGENCY_CONTACT_2_relationship to patient: | FRIEND         |
-| FEVER->YES                                   | SELECTED       |
-| FEVER->NO                                    | NOT_SELECTED   |
-| SHORTNESS->YES                               | NOT_SELECTED   |
-| SHORTNESS->NO                                | SELECTED       |
-| COUGH->YES                                   | NOT_SELECTED   |
-| COUGH->NO                                    | SELECTED       |
-| LOSS_OF_TASTE->YES                           | NOT_SELECTED   |
-| LOSS_OF_TASTE->NO                            | SELECTED       |
-| COVID_CONTACT->YES                           | SELECTED       |
-| COVID_CONTACT->NO                            | NOT_SELECTED   |
-| TRAVEL->YES                                  | NOT_SELECTED   |
-| TRAVEL->NO                                   | SELECTED       |
-
-
```

### Comparing `amazon-textract-geofinder-0.0.6/amazon_textract_geofinder.egg-info/SOURCES.txt` & `amazon-textract-geofinder-0.0.7/amazon_textract_geofinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-textract-geofinder-0.0.6/bin/amazon-textract-geofinder` & `amazon-textract-geofinder-0.0.7/bin/amazon-textract-geofinder`

 * *Files identical despite different names*

### Comparing `amazon-textract-geofinder-0.0.6/setup.py` & `amazon-textract-geofinder-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     os.system('twine upload --repository pypi dist/*')
     sys.exit()
 
 setup(name='amazon-textract-geofinder',
       packages=find_packages(exclude=['tests']),
       include_package_data=True,
       exclude_package_data={"": ["test_*.py", "__pycache__"]},
-      version='0.0.6',
+      version='0.0.7',
       description='Amazon Textract package to easier access data through geometric information',
       install_requires=requirements,
       scripts=['bin/amazon-textract-geofinder'],
       long_description_content_type='text/markdown',
       long_description=read('README.md'),
       author='Amazon Rekognition Textract Demoes',
       author_email='rekognition-textract-demos@amazon.com',
```

### Comparing `amazon-textract-geofinder-0.0.6/textractgeofinder/ocrdb.py` & `amazon-textract-geofinder-0.0.7/textractgeofinder/ocrdb.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-geofinder-0.0.6/textractgeofinder/sample_patient_intake_form_parser.py` & `amazon-textract-geofinder-0.0.7/textractgeofinder/sample_patient_intake_form_parser.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-geofinder-0.0.6/textractgeofinder/tgeofinder.py` & `amazon-textract-geofinder-0.0.7/textractgeofinder/tgeofinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,21 +251,22 @@
                         number_of_words_to_return: int = None,
                         text_type: str = 'word',
                         area_selection: AreaSelection = None,
                         page_number: int = 1,
                         exclude_ids: List[str] = None) -> List[TWord]:
         xmin = anker.top_left.x
         xmax = anker.lower_right.x
+        ymax = anker.lower_right.y
 
         query = ''' and ? < (xmin + xmax) / 2
                     and ? > ( xmin + xmax ) / 2
                     and ? < ymin
                     and text_type = ?
                     order by ymin  asc '''
-        params = [xmin, xmax, text_type]
+        params = [xmin, xmax, ymax, text_type]
         if number_of_words_to_return:
             query += " limit ? "
             params.append(number_of_words_to_return)
 
         return self.ocrdb.execute(query=query,
                                   textract_doc_uuid=self.textract_doc_uuid,
                                   params=params,
```

### Comparing `amazon-textract-geofinder-0.0.6/textractgeofinder/tword.py` & `amazon-textract-geofinder-0.0.7/textractgeofinder/tword.py`

 * *Files identical despite different names*

