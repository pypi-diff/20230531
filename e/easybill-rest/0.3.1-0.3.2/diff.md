# Comparing `tmp/easybill_rest-0.3.1.tar.gz` & `tmp/easybill_rest-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybill_rest-0.3.1.tar", last modified: Tue Feb 28 11:48:04 2023, max compression
+gzip compressed data, was "easybill_rest-0.3.2.tar", last modified: Wed May 31 15:34:54 2023, max compression
```

## Comparing `easybill_rest-0.3.1.tar` & `easybill_rest-0.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2023-02-28 11:48:04.944221 easybill_rest-0.3.1/
--rw-r--r--   0 jannohles   (502) staff       (20)       94 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/MANIFEST.in
--rw-r--r--   0 jannohles   (502) staff       (20)     1431 2023-02-28 11:48:04.944061 easybill_rest-0.3.1/PKG-INFO
--rw-r--r--   0 jannohles   (502) staff       (20)      377 2023-02-28 11:46:41.000000 easybill_rest-0.3.1/changelog.md
-drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2023-02-28 11:48:04.935850 easybill_rest-0.3.1/easybill_rest/
--rw-r--r--   0 jannohles   (502) staff       (20)     9547 2023-02-28 11:46:41.000000 easybill_rest-0.3.1/easybill_rest/__init__.py
--rw-r--r--   0 jannohles   (502) staff       (20)      431 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/helper.py
-drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2023-02-28 11:48:04.943811 easybill_rest-0.3.1/easybill_rest/resources/
--rw-r--r--   0 jannohles   (502) staff       (20)      470 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_abstract.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2839 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_attachments.py
--rw-r--r--   0 jannohles   (502) staff       (20)     3201 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_contacts.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2635 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_customer_groups.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2390 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_customers.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2860 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_discount_position_groups.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2697 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_discount_positions.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2131 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_document_payments.py
--rw-r--r--   0 jannohles   (502) staff       (20)     4312 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_documents.py
--rw-r--r--   0 jannohles   (502) staff       (20)     1131 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_logins.py
--rw-r--r--   0 jannohles   (502) staff       (20)      854 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_pdf_templates.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2634 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_position_groups.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2390 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_positions.py
--rw-r--r--   0 jannohles   (502) staff       (20)     1547 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_post_boxes.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2366 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_projects.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2518 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_sepa_payments.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2076 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_serial_numbers.py
--rw-r--r--   0 jannohles   (502) staff       (20)     1508 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_stocks.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2213 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_tasks.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2602 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_text_templates.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2509 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_time_trackings.py
--rw-r--r--   0 jannohles   (502) staff       (20)     2366 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/easybill_rest/resources/resource_webhooks.py
-drwxr-xr-x   0 jannohles   (502) staff       (20)        0 2023-02-28 11:48:04.936635 easybill_rest-0.3.1/easybill_rest.egg-info/
--rw-r--r--   0 jannohles   (502) staff       (20)     1431 2023-02-28 11:48:04.000000 easybill_rest-0.3.1/easybill_rest.egg-info/PKG-INFO
--rw-r--r--   0 jannohles   (502) staff       (20)     1356 2023-02-28 11:48:04.000000 easybill_rest-0.3.1/easybill_rest.egg-info/SOURCES.txt
--rw-r--r--   0 jannohles   (502) staff       (20)        1 2023-02-28 11:48:04.000000 easybill_rest-0.3.1/easybill_rest.egg-info/dependency_links.txt
--rw-r--r--   0 jannohles   (502) staff       (20)       39 2023-02-28 11:48:04.000000 easybill_rest-0.3.1/easybill_rest.egg-info/requires.txt
--rw-r--r--   0 jannohles   (502) staff       (20)       14 2023-02-28 11:48:04.000000 easybill_rest-0.3.1/easybill_rest.egg-info/top_level.txt
--rw-r--r--   0 jannohles   (502) staff       (20)     1036 2023-02-28 11:38:49.000000 easybill_rest-0.3.1/license.md
--rw-r--r--   0 jannohles   (502) staff       (20)      974 2023-02-28 11:46:41.000000 easybill_rest-0.3.1/readme.md
--rw-r--r--   0 jannohles   (502) staff       (20)       38 2023-02-28 11:48:04.944270 easybill_rest-0.3.1/setup.cfg
--rw-r--r--   0 jannohles   (502) staff       (20)      894 2023-02-28 11:46:41.000000 easybill_rest-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:34:54.674104 easybill_rest-0.3.2/
+-rw-rw-rw-   0        0        0       97 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1502 2023-05-31 15:34:54.673103 easybill_rest-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-05-31 15:33:37.000000 easybill_rest-0.3.2/changelog.md
+drwxrwxrwx   0        0        0        0 2023-05-31 15:34:54.639099 easybill_rest-0.3.2/easybill_rest/
+-rw-rw-rw-   0        0        0     9813 2023-05-31 15:33:37.000000 easybill_rest-0.3.2/easybill_rest/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/helper.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:34:54.672103 easybill_rest-0.3.2/easybill_rest/resources/
+-rw-rw-rw-   0        0        0      494 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_abstract.py
+-rw-rw-rw-   0        0        0     2918 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_attachments.py
+-rw-rw-rw-   0        0        0     3300 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_contacts.py
+-rw-rw-rw-   0        0        0     2712 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_customer_groups.py
+-rw-rw-rw-   0        0        0     2460 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_customers.py
+-rw-rw-rw-   0        0        0     2939 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_discount_position_groups.py
+-rw-rw-rw-   0        0        0     2774 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_discount_positions.py
+-rw-rw-rw-   0        0        0     2193 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_document_payments.py
+-rw-rw-rw-   0        0        0     4445 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_documents.py
+-rw-rw-rw-   0        0        0     1170 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_logins.py
+-rw-rw-rw-   0        0        0      884 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_pdf_templates.py
+-rw-rw-rw-   0        0        0     2711 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_position_groups.py
+-rw-rw-rw-   0        0        0     2460 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_positions.py
+-rw-rw-rw-   0        0        0     1595 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_post_boxes.py
+-rw-rw-rw-   0        0        0     2436 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_projects.py
+-rw-rw-rw-   0        0        0     2590 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_sepa_payments.py
+-rw-rw-rw-   0        0        0     2138 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_serial_numbers.py
+-rw-rw-rw-   0        0        0     1557 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_stocks.py
+-rw-rw-rw-   0        0        0     2278 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_tasks.py
+-rw-rw-rw-   0        0        0     2679 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_text_templates.py
+-rw-rw-rw-   0        0        0     2581 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_time_trackings.py
+-rw-rw-rw-   0        0        0     2436 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/easybill_rest/resources/resource_webhooks.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:34:54.647101 easybill_rest-0.3.2/easybill_rest.egg-info/
+-rw-rw-rw-   0        0        0     1502 2023-05-31 15:34:54.000000 easybill_rest-0.3.2/easybill_rest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1356 2023-05-31 15:34:54.000000 easybill_rest-0.3.2/easybill_rest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:34:54.000000 easybill_rest-0.3.2/easybill_rest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-31 15:34:54.000000 easybill_rest-0.3.2/easybill_rest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 15:34:54.000000 easybill_rest-0.3.2/easybill_rest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1043 2023-05-31 15:18:01.000000 easybill_rest-0.3.2/license.md
+-rw-rw-rw-   0        0        0     1005 2023-05-31 15:33:37.000000 easybill_rest-0.3.2/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 15:34:54.674104 easybill_rest-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-05-31 15:34:03.000000 easybill_rest-0.3.2/setup.py
```

### Comparing `easybill_rest-0.3.1/PKG-INFO` & `easybill_rest-0.3.2/easybill_rest.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1
-Name: easybill_rest
-Version: 0.3.1
-Summary: easybill_rest is a library to work with the easybill REST API (https://www.easybill.de/api/)
-Home-page: https://github.com/BolZer/py-ebrest
-Author: Jan Noehles (bolZer)
-Author-email: noehles@easybill.de
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-# easybill_rest (py-ebrest)
-[![Generic badge](https://img.shields.io/badge/Version-0.3.1-important.svg)]()
-[![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
-[![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
-[![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
-
-`easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
-
-All Resources are available.
-
-The library supports only the `Bearer` Authentication and calls the API only
-through `HTTPS`.
-
-```bash
-pip install easybill_rest
-```
-
-
-## Usage
-
-```Python
-from easybill_rest import Client
-
-
-client = Client("API-KEY")
-result = client.documents().get_document("2")
-
-# Returns the document model. Therefore a field "title" is included in the dict.
-print(result['title'])
-
-```
+Metadata-Version: 2.1
+Name: easybill-rest
+Version: 0.3.2
+Summary: easybill_rest is a library to work with the easybill REST API (https://www.easybill.de/api/)
+Home-page: https://github.com/BolZer/py-ebrest
+Author: Jan Noehles (bolZer)
+Author-email: noehles@easybill.de
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: license.md
+
+# easybill_rest (py-ebrest)
+[![Generic badge](https://img.shields.io/badge/Version-0.3.2-important.svg)]()
+[![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
+[![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
+[![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
+
+`easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
+
+All Resources are available.
+
+The library supports only the `Bearer` Authentication and calls the API only
+through `HTTPS`.
+
+```bash
+pip install easybill_rest
+```
+
+
+## Usage
+
+```Python
+from easybill_rest import Client
+
+
+client = Client("API-KEY")
+result = client.documents().get_document("2")
+
+# Returns the document model. Therefore a field "title" is included in the dict.
+print(result['title'])
+
+```
```

### Comparing `easybill_rest-0.3.1/easybill_rest/__init__.py` & `easybill_rest-0.3.2/easybill_rest/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,266 +1,266 @@
-import requests
-
-from easybill_rest.resources.resource_attachments import ResourceAttachments
-from easybill_rest.resources.resource_contacts import ResourceContacts
-from easybill_rest.resources.resource_customer_groups import ResourceCustomerGroups
-from easybill_rest.resources.resource_customers import ResourceCustomers
-from easybill_rest.resources.resource_discount_position_groups import ResourceDiscountPositionGroups
-from easybill_rest.resources.resource_discount_positions import ResourceDiscountPositions
-from easybill_rest.resources.resource_document_payments import ResourceDocumentPayments
-from easybill_rest.resources.resource_documents import ResourceDocuments
-from easybill_rest.resources.resource_logins import ResourceLogins
-from easybill_rest.resources.resource_pdf_templates import ResourcePdfTemplates
-from easybill_rest.resources.resource_position_groups import ResourcePositionGroups
-from easybill_rest.resources.resource_positions import ResourcePositions
-from easybill_rest.resources.resource_post_boxes import ResourcePostBoxes
-from easybill_rest.resources.resource_projects import ResourceProjects
-from easybill_rest.resources.resource_sepa_payments import ResourceSepaPayments
-from easybill_rest.resources.resource_serial_numbers import ResourceSerialNumbers
-from easybill_rest.resources.resource_stocks import ResourceStocks
-from easybill_rest.resources.resource_tasks import ResourceTasks
-from easybill_rest.resources.resource_text_templates import ResourceTextTemplates
-from easybill_rest.resources.resource_time_trackings import ResourceTimeTrackings
-from easybill_rest.resources.resource_webhooks import ResourceWebhooks
-
-
-class Client:
-    _version: str = "0.3.1"
-    _base_url: str = "https://api.easybill.de"
-    _requests = requests
-
-    api_key: str = ""
-    timeout: int
-
-    def __init__(self, api_key: str, timeout: int = 10) -> None:
-        self.timeout = timeout
-        self.api_key = api_key
-        self._requests = requests
-
-    def get_basic_headers(self) -> dict:
-        """get_basic_headers returns the basic headers used by the client. Contains auth and
-        agent. """
-
-        return {
-            "Authorization": "Bearer " + self.api_key,
-            "User-Agent": "py-ebrest " + self._version
-        }
-
-    def get_basic_headers_for_json(self) -> dict:
-        """get_basic_headers_for_json returns the basic headers extended with a
-        json content type."""
-
-        return {
-            **self.get_basic_headers(),
-            **{'Content-type': 'application/json'}
-        }
-
-    def get_basic_headers_for_pdf(self) -> dict:
-        """get_basic_headers_for_pdf returns the basic headers extended with a pdf content type."""
-
-        return {
-            **self.get_basic_headers(),
-            **{'Content-type': 'application/pdf'}
-        }
-
-    def documents(self) -> ResourceDocuments:
-        """documents returns the documents resource which exposes the api documents resource."""
-
-        return ResourceDocuments(self)
-
-    def document_payments(self) -> ResourceDocumentPayments:
-        """document_payments returns the document payments resource which exposes the ap
-        i document payments resource."""
-
-        return ResourceDocumentPayments(self)
-
-    def customers(self) -> ResourceCustomers:
-        """customers returns the customers resource which exposes the api customers resource."""
-
-        return ResourceCustomers(self)
-
-    def customer_groups(self) -> ResourceCustomerGroups:
-        """customer_groups returns the customers groups resource which exposes the
-         api customer groups resource."""
-
-        return ResourceCustomerGroups(self)
-
-    def positions(self) -> ResourcePositions:
-        """positions returns the positions resource which exposes the api positions resource."""
-
-        return ResourcePositions(self)
-
-    def position_groups(self) -> ResourcePositionGroups:
-        """position_groups returns the position groups resource which exposes
-        the api position groups resource."""
-
-        return ResourcePositionGroups(self)
-
-    def logins(self) -> ResourceLogins:
-        """logins returns the logins resource which exposes the api logins resource."""
-
-        return ResourceLogins(self)
-
-    def pdf_templates(self) -> ResourcePdfTemplates:
-        """pdf_templates returns the pdf-templates resource which exposes the api
-        pdf-templates resource."""
-
-        return ResourcePdfTemplates(self)
-
-    def post_boxes(self) -> ResourcePostBoxes:
-        """post_boxes returns the post box resource which exposes the api post-box resource."""
-
-        return ResourcePostBoxes(self)
-
-    def projects(self) -> ResourceProjects:
-        """projects returns the projects resource which exposes the api projects resource."""
-
-        return ResourceProjects(self)
-
-    def tasks(self) -> ResourceTasks:
-        """tasks returns the tasks resource which exposes the api tasks resource."""
-
-        return ResourceTasks(self)
-
-    def time_trackings(self) -> ResourceTimeTrackings:
-        """time_trackings returns the time tracking resource which exposes the
-        api time tracking resource."""
-
-        return ResourceTimeTrackings(self)
-
-    def stocks(self) -> ResourceStocks:
-        """stocks returns the stocks resource which exposes the api stocks resource."""
-
-        return ResourceStocks(self)
-
-    def serial_numbers(self) -> ResourceSerialNumbers:
-        """serial_numbers returns the serial number resource which exposes the api serial number
-        resource."""
-
-        return ResourceSerialNumbers(self)
-
-    def sepa_payments(self) -> ResourceSepaPayments:
-        """sepa_payments returns the sepa payments resource which exposes the sepa payment
-        resource."""
-
-        return ResourceSepaPayments(self)
-
-    def webhooks(self) -> ResourceWebhooks:
-        """webhooks returns the webhooks resource which exposes the webhook resource."""
-
-        return ResourceWebhooks(self)
-
-    def contacts(self) -> ResourceContacts:
-        """contacts returns the contacts resource which exposes the contact resource."""
-
-        return ResourceContacts(self)
-
-    def text_templates(self) -> ResourceTextTemplates:
-        """text_templates returns the text template resource which exposes the text template
-        resource."""
-
-        return ResourceTextTemplates(self)
-
-    def discount_positions(self) -> ResourceDiscountPositions:
-        """discount_positions returns the position discount resource which exposes the position
-        discount resource."""
-
-        return ResourceDiscountPositions(self)
-
-    def discount_position_groups(self) -> ResourceDiscountPositionGroups:
-        """discount_position_groups returns the position group discount resource which exposes
-        the position group discount resource."""
-
-        return ResourceDiscountPositionGroups(self)
-
-    def attachments(self) -> ResourceAttachments:
-        """attachments returns the attachments resource which exposes the attachment resource."""
-
-        return ResourceAttachments(self)
-
-    def call(
-            self,
-            method: str,
-            request_url: str,
-            headers: dict,
-            passed_payload: dict = None) -> dict:
-        """
-            call calls the easybill api with the prepared connection.
-            :raises: RequestException
-        """
-
-        if method == "GET":
-            response = self._requests.request(
-                method,
-                self._base_url + request_url,
-                headers=headers,
-                params=passed_payload,
-                timeout=self.timeout
-            )
-            response.raise_for_status()
-
-            return response.json()
-
-        if method in ("PUT", "POST"):
-            response = self._requests.request(
-                method,
-                self._base_url + request_url,
-                headers=headers,
-                json=passed_payload,
-                timeout=self.timeout
-            )
-            response.raise_for_status()
-
-            return response.json()
-
-        if method == "DELETE":
-            response = self._requests.request(
-                method,
-                self._base_url + request_url,
-                headers=headers,
-                timeout=self.timeout
-            )
-
-            response.raise_for_status()
-            return {}
-
-        response = self._requests.request(
-            method,
-            self._base_url + request_url,
-            headers=headers,
-            timeout=self.timeout
-        )
-        response.raise_for_status()
-
-        return response.json()
-
-    def upload(self, request_url: str, headers: dict, file: bytes) -> dict:
-        """
-            upload calls the easybill api with the prepared connection to upload the
-            passed bytes / file.
-            :raises: RequestException
-        """
-
-        response = self._requests.post(
-            self._base_url + request_url,
-            headers=headers,
-            timeout=self.timeout,
-            files={'file': file}
-        )
-        response.raise_for_status()
-
-        return response.json()
-
-    def download(self, request_url: str, headers: dict) -> bytes:
-        """
-            download calls the easybill api with the prepared connection to download the
-            referenced attachment.
-            :raises: RequestException
-        """
-
-        response = self._requests.get(
-            self._base_url + request_url,
-            headers=headers,
-            timeout=self.timeout)
-        response.raise_for_status()
-
-        return response.content
+import requests
+
+from easybill_rest.resources.resource_attachments import ResourceAttachments
+from easybill_rest.resources.resource_contacts import ResourceContacts
+from easybill_rest.resources.resource_customer_groups import ResourceCustomerGroups
+from easybill_rest.resources.resource_customers import ResourceCustomers
+from easybill_rest.resources.resource_discount_position_groups import ResourceDiscountPositionGroups
+from easybill_rest.resources.resource_discount_positions import ResourceDiscountPositions
+from easybill_rest.resources.resource_document_payments import ResourceDocumentPayments
+from easybill_rest.resources.resource_documents import ResourceDocuments
+from easybill_rest.resources.resource_logins import ResourceLogins
+from easybill_rest.resources.resource_pdf_templates import ResourcePdfTemplates
+from easybill_rest.resources.resource_position_groups import ResourcePositionGroups
+from easybill_rest.resources.resource_positions import ResourcePositions
+from easybill_rest.resources.resource_post_boxes import ResourcePostBoxes
+from easybill_rest.resources.resource_projects import ResourceProjects
+from easybill_rest.resources.resource_sepa_payments import ResourceSepaPayments
+from easybill_rest.resources.resource_serial_numbers import ResourceSerialNumbers
+from easybill_rest.resources.resource_stocks import ResourceStocks
+from easybill_rest.resources.resource_tasks import ResourceTasks
+from easybill_rest.resources.resource_text_templates import ResourceTextTemplates
+from easybill_rest.resources.resource_time_trackings import ResourceTimeTrackings
+from easybill_rest.resources.resource_webhooks import ResourceWebhooks
+
+
+class Client:
+    _version: str = "0.3.2"
+    _base_url: str = "https://api.easybill.de"
+    _requests = requests
+
+    api_key: str = ""
+    timeout: int
+
+    def __init__(self, api_key: str, timeout: int = 10) -> None:
+        self.timeout = timeout
+        self.api_key = api_key
+        self._requests = requests
+
+    def get_basic_headers(self) -> dict:
+        """get_basic_headers returns the basic headers used by the client. Contains auth and
+        agent. """
+
+        return {
+            "Authorization": "Bearer " + self.api_key,
+            "User-Agent": "py-ebrest " + self._version
+        }
+
+    def get_basic_headers_for_json(self) -> dict:
+        """get_basic_headers_for_json returns the basic headers extended with a
+        json content type."""
+
+        return {
+            **self.get_basic_headers(),
+            **{'Content-type': 'application/json'}
+        }
+
+    def get_basic_headers_for_pdf(self) -> dict:
+        """get_basic_headers_for_pdf returns the basic headers extended with a pdf content type."""
+
+        return {
+            **self.get_basic_headers(),
+            **{'Content-type': 'application/pdf'}
+        }
+
+    def documents(self) -> ResourceDocuments:
+        """documents returns the documents resource which exposes the api documents resource."""
+
+        return ResourceDocuments(self)
+
+    def document_payments(self) -> ResourceDocumentPayments:
+        """document_payments returns the document payments resource which exposes the ap
+        i document payments resource."""
+
+        return ResourceDocumentPayments(self)
+
+    def customers(self) -> ResourceCustomers:
+        """customers returns the customers resource which exposes the api customers resource."""
+
+        return ResourceCustomers(self)
+
+    def customer_groups(self) -> ResourceCustomerGroups:
+        """customer_groups returns the customers groups resource which exposes the
+         api customer groups resource."""
+
+        return ResourceCustomerGroups(self)
+
+    def positions(self) -> ResourcePositions:
+        """positions returns the positions resource which exposes the api positions resource."""
+
+        return ResourcePositions(self)
+
+    def position_groups(self) -> ResourcePositionGroups:
+        """position_groups returns the position groups resource which exposes
+        the api position groups resource."""
+
+        return ResourcePositionGroups(self)
+
+    def logins(self) -> ResourceLogins:
+        """logins returns the logins resource which exposes the api logins resource."""
+
+        return ResourceLogins(self)
+
+    def pdf_templates(self) -> ResourcePdfTemplates:
+        """pdf_templates returns the pdf-templates resource which exposes the api
+        pdf-templates resource."""
+
+        return ResourcePdfTemplates(self)
+
+    def post_boxes(self) -> ResourcePostBoxes:
+        """post_boxes returns the post box resource which exposes the api post-box resource."""
+
+        return ResourcePostBoxes(self)
+
+    def projects(self) -> ResourceProjects:
+        """projects returns the projects resource which exposes the api projects resource."""
+
+        return ResourceProjects(self)
+
+    def tasks(self) -> ResourceTasks:
+        """tasks returns the tasks resource which exposes the api tasks resource."""
+
+        return ResourceTasks(self)
+
+    def time_trackings(self) -> ResourceTimeTrackings:
+        """time_trackings returns the time tracking resource which exposes the
+        api time tracking resource."""
+
+        return ResourceTimeTrackings(self)
+
+    def stocks(self) -> ResourceStocks:
+        """stocks returns the stocks resource which exposes the api stocks resource."""
+
+        return ResourceStocks(self)
+
+    def serial_numbers(self) -> ResourceSerialNumbers:
+        """serial_numbers returns the serial number resource which exposes the api serial number
+        resource."""
+
+        return ResourceSerialNumbers(self)
+
+    def sepa_payments(self) -> ResourceSepaPayments:
+        """sepa_payments returns the sepa payments resource which exposes the sepa payment
+        resource."""
+
+        return ResourceSepaPayments(self)
+
+    def webhooks(self) -> ResourceWebhooks:
+        """webhooks returns the webhooks resource which exposes the webhook resource."""
+
+        return ResourceWebhooks(self)
+
+    def contacts(self) -> ResourceContacts:
+        """contacts returns the contacts resource which exposes the contact resource."""
+
+        return ResourceContacts(self)
+
+    def text_templates(self) -> ResourceTextTemplates:
+        """text_templates returns the text template resource which exposes the text template
+        resource."""
+
+        return ResourceTextTemplates(self)
+
+    def discount_positions(self) -> ResourceDiscountPositions:
+        """discount_positions returns the position discount resource which exposes the position
+        discount resource."""
+
+        return ResourceDiscountPositions(self)
+
+    def discount_position_groups(self) -> ResourceDiscountPositionGroups:
+        """discount_position_groups returns the position group discount resource which exposes
+        the position group discount resource."""
+
+        return ResourceDiscountPositionGroups(self)
+
+    def attachments(self) -> ResourceAttachments:
+        """attachments returns the attachments resource which exposes the attachment resource."""
+
+        return ResourceAttachments(self)
+
+    def call(
+            self,
+            method: str,
+            request_url: str,
+            headers: dict,
+            passed_payload: dict = None) -> dict:
+        """
+            call calls the easybill api with the prepared connection.
+            :raises: RequestException
+        """
+
+        if method == "GET":
+            response = self._requests.request(
+                method,
+                self._base_url + request_url,
+                headers=headers,
+                params=passed_payload,
+                timeout=self.timeout
+            )
+            response.raise_for_status()
+
+            return response.json()
+
+        if method in ("PUT", "POST"):
+            response = self._requests.request(
+                method,
+                self._base_url + request_url,
+                headers=headers,
+                json=passed_payload,
+                timeout=self.timeout
+            )
+            response.raise_for_status()
+
+            return response.json()
+
+        if method == "DELETE":
+            response = self._requests.request(
+                method,
+                self._base_url + request_url,
+                headers=headers,
+                timeout=self.timeout
+            )
+
+            response.raise_for_status()
+            return {}
+
+        response = self._requests.request(
+            method,
+            self._base_url + request_url,
+            headers=headers,
+            timeout=self.timeout
+        )
+        response.raise_for_status()
+
+        return response.json()
+
+    def upload(self, request_url: str, headers: dict, file: bytes) -> dict:
+        """
+            upload calls the easybill api with the prepared connection to upload the
+            passed bytes / file.
+            :raises: RequestException
+        """
+
+        response = self._requests.post(
+            self._base_url + request_url,
+            headers=headers,
+            timeout=self.timeout,
+            files={'file': file}
+        )
+        response.raise_for_status()
+
+        return response.json()
+
+    def download(self, request_url: str, headers: dict) -> bytes:
+        """
+            download calls the easybill api with the prepared connection to download the
+            referenced attachment.
+            :raises: RequestException
+        """
+
+        response = self._requests.get(
+            self._base_url + request_url,
+            headers=headers,
+            timeout=self.timeout)
+        response.raise_for_status()
+
+        return response.content
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_attachments.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_sepa_payments.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,72 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceAttachments(ResourceAbstract):
-    __endpoint: str = "/attachments"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_attachments(self, params: dict = None) -> dict:
-        """get_attachments returns a dict with attachment objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_attachment(self, attachment_id: str) -> dict:
-        """get_attachment returns the referenced (id) attachment"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + attachment_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_attachment(self, payload: bytes) -> dict:
-        """create_attachment returns the attachment model as dict on success with the data from the passed payload"""
-
-        return self.__client.upload(
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers(),
-            payload
-        )
-
-    def update_attachment(self, attachment_id: str, payload: dict) -> dict:
-        """update_attachment updates the reference (id) attachment with the given payload. Returns a part of the updated attachment model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                attachment_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_attachment(self, attachment_id: str) -> None:
-        """delete_attachment returns None on success and raises an exception if the attachment couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                attachment_id),
-            self.__client.get_basic_headers())
-
-    def get_content(self, attachment_id: str, headers: dict = None) -> bytes:
-        """get_content returns None on success and raises an exception if the attachment couldn't be deleted"""
-
-        return self.__client.download(
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + attachment_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceSepaPayments(ResourceAbstract):
+    __endpoint: str = "/sepa-payments"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_sepa_payments(self, params: dict = None) -> dict:
+        """get_sepa_payments returns a dict with sepa payments objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_sepa_payment(self, sepa_payment_id: str) -> dict:
+        """get_sepa_payment returns the referenced (id) sepa payment"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + sepa_payment_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_sepa_payment(self, payload: dict) -> dict:
+        """create_sepa_payment returns the sepa payment model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_sepa_payment(self, sepa_payment_id: str, payload: dict) -> dict:
+        """update_sepa_payment updates the reference (id) sepa payment with the given payload. Returns the updated sepa payment model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                sepa_payment_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_sepa_payment(self, sepa_payment_id: str) -> None:
+        """delete_sepa_payment returns None on success and raises an exception if the sepa payment couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                sepa_payment_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_contacts.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_contacts.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceContacts(ResourceAbstract):
-    __endpoint: str = "/customers"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_contacts(self, customer_id: str, params: dict = None) -> dict:
-        """get_contacts returns a dict with contact objects for the referenced customer"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_id +
-                "/" +
-                "contacts",
-                params),
-            self.__client.get_basic_headers_for_json())
-
-    def get_contact(self, customer_id: str, contact_id: str) -> dict:
-        """get_contact returns the referenced (id) contact for the referenced customer"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_id +
-                "/" +
-                "contacts" +
-                "/" +
-                contact_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_contact(self, customer_id: str, payload: dict) -> dict:
-        """create_contact returns the contact model as dict on success with the data from the passed payload for the referenced customer"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_id +
-                "/" +
-                "contacts"),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def update_contact(
-            self,
-            customer_id: str,
-            contact_id: str,
-            payload: dict) -> dict:
-        """update_contact updates the reference (id) contact with the given payload. Returns the updated contact model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_id +
-                "/" +
-                "contacts" +
-                "/" +
-                contact_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_contact(self, customer_id: str, contact_id: str) -> None:
-        """delete_contact returns None on success and raises an exception if the contact couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_id +
-                "/" +
-                "contacts" +
-                "/" +
-                contact_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceContacts(ResourceAbstract):
+    __endpoint: str = "/customers"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_contacts(self, customer_id: str, params: dict = None) -> dict:
+        """get_contacts returns a dict with contact objects for the referenced customer"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                customer_id +
+                "/" +
+                "contacts",
+                params),
+            self.__client.get_basic_headers_for_json())
+
+    def get_contact(self, customer_id: str, contact_id: str) -> dict:
+        """get_contact returns the referenced (id) contact for the referenced customer"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                customer_id +
+                "/" +
+                "contacts" +
+                "/" +
+                contact_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_contact(self, customer_id: str, payload: dict) -> dict:
+        """create_contact returns the contact model as dict on success with the data from the passed payload for the referenced customer"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                customer_id +
+                "/" +
+                "contacts"),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def update_contact(
+            self,
+            customer_id: str,
+            contact_id: str,
+            payload: dict) -> dict:
+        """update_contact updates the reference (id) contact with the given payload. Returns the updated contact model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                customer_id +
+                "/" +
+                "contacts" +
+                "/" +
+                contact_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_contact(self, customer_id: str, contact_id: str) -> None:
+        """delete_contact returns None on success and raises an exception if the contact couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                customer_id +
+                "/" +
+                "contacts" +
+                "/" +
+                contact_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_customer_groups.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_position_groups.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceCustomerGroups(ResourceAbstract):
-    __endpoint: str = "/customer-groups"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_customer_groups(self, params: dict = None) -> dict:
-        """get_customer_groups returns a dict with customer groups objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_customer_group(self, customer_group_id: str) -> dict:
-        """get_customer_group returns the referenced (id) customer group"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_group_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_customer_group(self, payload: dict) -> dict:
-        """create_customer_group returns the customer group model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_customer_group(
-            self,
-            customer_group_id: str,
-            payload: dict) -> dict:
-        """update_customer_group updates the reference (id) customer group with the given payload. Returns the updated customer group model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_group_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_customer_group(self, customer_group_id: str) -> None:
-        """delete_customer_group returns None on success and raises an exception if the customer-group couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_group_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourcePositionGroups(ResourceAbstract):
+    __endpoint: str = "/position-groups"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_position_groups(self, params: dict = None) -> dict:
+        """get_position_groups returns a dict with position group objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_position_group(self, position_group_id: str) -> dict:
+        """get_position_group returns the referenced (id) position group"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                position_group_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_position_group(self, payload: dict) -> dict:
+        """create_position_group returns the position group model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_position_group(
+            self,
+            position_group_id: str,
+            payload: dict) -> dict:
+        """update_position_group updates the reference (id) position group with the given payload. Returns the updated position group model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                position_group_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_position_group(self, position_group_id: str) -> None:
+        """delete_position_group returns None on success and raises an exception if the position group couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                position_group_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_customers.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_post_boxes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,48 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceCustomers(ResourceAbstract):
-    __endpoint: str = "/customers"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_customers(self, params: dict = None) -> dict:
-        """get_customers returns a dict with customer objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_customer(self, customer_id: str) -> dict:
-        """get_customer returns the referenced (id) customer"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + customer_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_customer(self, payload: dict) -> dict:
-        """create_customer returns the customer model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_customer(self, customer_id: str, payload: dict) -> dict:
-        """update_customer updates the reference (id) customer with the given payload. Returns the updated customer model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                customer_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_customer(self, customer_id: str) -> None:
-        """delete_document returns None on success and raises an exception if the customer couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + customer_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourcePostBoxes(ResourceAbstract):
+    __endpoint: str = "/post-boxes"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_post_boxes(self, params: dict = None) -> dict:
+        """get_post_boxes returns a dict with post box objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_post_box(self, post_box_id: str) -> dict:
+        """get_post_box returns the referenced (id) post box"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + post_box_id),
+            self.__client.get_basic_headers_for_json())
+
+    def delete_post_box(self, post_box_id: str) -> None:
+        """delete_post_box returns None on success and raises an exception if the post box couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + post_box_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_discount_position_groups.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_discount_position_groups.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceDiscountPositionGroups(ResourceAbstract):
-    __endpoint: str = "/discounts/position-group"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_position_group_discounts(self, params: dict = None) -> dict:
-        """get_position_group_discounts returns a dict with position group discount objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_position_group_discount(
-            self, position_group_discount_id: str) -> dict:
-        """get_position_group_discount returns the referenced (id) position group discount"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                position_group_discount_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_position_group_discount(self, payload: dict) -> dict:
-        """create_position_group_discount returns the position group discount model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_position_group_discount(
-            self,
-            position_group_discount_id: str,
-            payload: dict) -> dict:
-        """update_position_group_discount updates the reference (id) position group discount with the given payload. Returns the updated position group discount model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                position_group_discount_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_position_group_discount(
-            self, position_group_discount_id: str) -> None:
-        """delete_position_group_discount returns None on success and raises an exception if the discount couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                position_group_discount_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceDiscountPositionGroups(ResourceAbstract):
+    __endpoint: str = "/discounts/position-group"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_position_group_discounts(self, params: dict = None) -> dict:
+        """get_position_group_discounts returns a dict with position group discount objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_position_group_discount(
+            self, position_group_discount_id: str) -> dict:
+        """get_position_group_discount returns the referenced (id) position group discount"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                position_group_discount_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_position_group_discount(self, payload: dict) -> dict:
+        """create_position_group_discount returns the position group discount model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_position_group_discount(
+            self,
+            position_group_discount_id: str,
+            payload: dict) -> dict:
+        """update_position_group_discount updates the reference (id) position group discount with the given payload. Returns the updated position group discount model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                position_group_discount_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_position_group_discount(
+            self, position_group_discount_id: str) -> None:
+        """delete_position_group_discount returns None on success and raises an exception if the discount couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                position_group_discount_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_document_payments.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_attachments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,79 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceDocumentPayments(ResourceAbstract):
-    __endpoint: str = "/document-payments"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_document_payments(self, params: dict = None) -> dict:
-        """get_document_payments returns a dict with document payments objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_document_payment(self, document_payment_id: str) -> dict:
-        """get_document_payment returns the referenced (id) document payment"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                document_payment_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_document_payment(self, payload: dict) -> dict:
-        """create_document_payment returns the document payment model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def delete_document_payment(self, document_payment_id: str) -> None:
-        """delete_document_payment returns None on success and raises an exception if the document payment couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                document_payment_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceAttachments(ResourceAbstract):
+    __endpoint: str = "/attachments"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_attachments(self, params: dict = None) -> dict:
+        """get_attachments returns a dict with attachment objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_attachment(self, attachment_id: str) -> dict:
+        """get_attachment returns the referenced (id) attachment"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + attachment_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_attachment(self, payload: bytes) -> dict:
+        """create_attachment returns the attachment model as dict on success with the data from the passed payload"""
+
+        return self.__client.upload(
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers(),
+            payload
+        )
+
+    def update_attachment(self, attachment_id: str, payload: dict) -> dict:
+        """update_attachment updates the reference (id) attachment with the given payload. Returns a part of the updated attachment model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                attachment_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_attachment(self, attachment_id: str) -> None:
+        """delete_attachment returns None on success and raises an exception if the attachment couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                attachment_id),
+            self.__client.get_basic_headers())
+
+    def get_content(self, attachment_id: str, headers: dict = None) -> bytes:
+        """get_content returns None on success and raises an exception if the attachment couldn't be deleted"""
+
+        return self.__client.download(
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + attachment_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_documents.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_documents.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from __future__ import annotations
-
-from enum import Enum
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class SendMethod(Enum):
-    EMAIL = "email"
-    FAX = "fax"
-    POST = "post"
-
-
-class ResourceDocuments(ResourceAbstract):
-    __endpoint: str = "/documents"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_documents(self, params: dict = None) -> dict:
-        """get_documents returns a dict with document objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_document(self, document_id: str) -> dict:
-        """get_document returns the referenced (id) document"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + document_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_document(self, payload: dict) -> dict:
-        """create_document returns the document model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_document(self, document_id: str, payload: dict, params: dict = None) -> dict:
-        """update_document updates the reference (id) document with the given payload. Returns the updated document"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                document_id,
-                params
-            ),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_document(self, document_id: str) -> None:
-        """delete_document returns None on success and raises an exception if the document couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + document_id),
-            self.__client.get_basic_headers())
-
-    def finalize_document(self, document_id: str) -> dict:
-        """finalize_document returns the finalized document on success"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                document_id +
-                "/done"),
-            self.__client.get_basic_headers_for_json())
-
-    def cancel_document(self, document_id: str) -> dict:
-        """cancel_document returns the canceled document on success"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                document_id +
-                "/cancel"),
-            self.__client.get_basic_headers_for_json())
-
-    def send_document(
-            self,
-            document_id: str,
-            send_method: SendMethod,
-            payload: dict) -> None:
-        """send_document returns None on success and rises exception on failure"""
-
-        self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                document_id +
-                "/send/" +
-                str(send_method)),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def download_document(self, document_id: str) -> bytes:
-        """download_document returns the document as bytes on success"""
-
-        return self.__client.download(
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                document_id +
-                "/pdf"),
-            self.__client.get_basic_headers_for_pdf(),
-        )
+from __future__ import annotations
+
+from enum import Enum
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class SendMethod(Enum):
+    EMAIL = "email"
+    FAX = "fax"
+    POST = "post"
+
+
+class ResourceDocuments(ResourceAbstract):
+    __endpoint: str = "/documents"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_documents(self, params: dict = None) -> dict:
+        """get_documents returns a dict with document objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_document(self, document_id: str) -> dict:
+        """get_document returns the referenced (id) document"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + document_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_document(self, payload: dict) -> dict:
+        """create_document returns the document model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_document(self, document_id: str, payload: dict, params: dict = None) -> dict:
+        """update_document updates the reference (id) document with the given payload. Returns the updated document"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                document_id,
+                params
+            ),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_document(self, document_id: str) -> None:
+        """delete_document returns None on success and raises an exception if the document couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + document_id),
+            self.__client.get_basic_headers())
+
+    def finalize_document(self, document_id: str) -> dict:
+        """finalize_document returns the finalized document on success"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                document_id +
+                "/done"),
+            self.__client.get_basic_headers_for_json())
+
+    def cancel_document(self, document_id: str) -> dict:
+        """cancel_document returns the canceled document on success"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                document_id +
+                "/cancel"),
+            self.__client.get_basic_headers_for_json())
+
+    def send_document(
+            self,
+            document_id: str,
+            send_method: SendMethod,
+            payload: dict) -> None:
+        """send_document returns None on success and rises exception on failure"""
+
+        self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                document_id +
+                "/send/" +
+                str(send_method)),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def download_document(self, document_id: str) -> bytes:
+        """download_document returns the document as bytes on success"""
+
+        return self.__client.download(
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                document_id +
+                "/pdf"),
+            self.__client.get_basic_headers_for_pdf(),
+        )
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_pdf_templates.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_pdf_templates.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourcePdfTemplates(ResourceAbstract):
-    __endpoint: str = "/pdf-templates"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_pdf_templates(self, params: dict = None) -> dict:
-        """get_pdf_templates returns a dict with pdf-templates objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourcePdfTemplates(ResourceAbstract):
+    __endpoint: str = "/pdf-templates"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_pdf_templates(self, params: dict = None) -> dict:
+        """get_pdf_templates returns a dict with pdf-templates objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_positions.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_positions.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourcePositions(ResourceAbstract):
-    __endpoint: str = "/positions"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_positions(self, params: dict = None) -> dict:
-        """get_positions returns a dict with position objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_position(self, position_id: str) -> dict:
-        """get_position returns the referenced (id) position"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + position_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_position(self, payload: dict) -> dict:
-        """create_position returns the position model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_position(self, position_id: str, payload: dict) -> dict:
-        """update_position updates the reference (id) position with the given payload. Returns the updated position model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                position_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_position(self, position_id: str) -> None:
-        """delete_position returns None on success and raises an exception if the position couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + position_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourcePositions(ResourceAbstract):
+    __endpoint: str = "/positions"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_positions(self, params: dict = None) -> dict:
+        """get_positions returns a dict with position objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_position(self, position_id: str) -> dict:
+        """get_position returns the referenced (id) position"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + position_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_position(self, payload: dict) -> dict:
+        """create_position returns the position model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_position(self, position_id: str, payload: dict) -> dict:
+        """update_position updates the reference (id) position with the given payload. Returns the updated position model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                position_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_position(self, position_id: str) -> None:
+        """delete_position returns None on success and raises an exception if the position couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + position_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_sepa_payments.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_time_trackings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceSepaPayments(ResourceAbstract):
-    __endpoint: str = "/sepa-payments"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_sepa_payments(self, params: dict = None) -> dict:
-        """get_sepa_payments returns a dict with sepa payments objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_sepa_payment(self, sepa_payment_id: str) -> dict:
-        """get_sepa_payment returns the referenced (id) sepa payment"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + sepa_payment_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_sepa_payment(self, payload: dict) -> dict:
-        """create_sepa_payment returns the sepa payment model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_sepa_payment(self, sepa_payment_id: str, payload: dict) -> dict:
-        """update_sepa_payment updates the reference (id) sepa payment with the given payload. Returns the updated sepa payment model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                sepa_payment_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_sepa_payment(self, sepa_payment_id: str) -> None:
-        """delete_sepa_payment returns None on success and raises an exception if the sepa payment couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                sepa_payment_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceTimeTrackings(ResourceAbstract):
+    __endpoint: str = "/time-trackings"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_time_trackings(self, params: dict = None) -> dict:
+        """get_time_tracking returns a dict with time tracking objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_time_tracking(self, time_tracking_id: str) -> dict:
+        """get_time_tracking returns the referenced (id) time tracking"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                time_tracking_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_time_tracking(self, payload: dict) -> dict:
+        """create_time_tracking returns the time tracking model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_time_tracking(
+            self,
+            time_tracking_id: str,
+            payload: dict) -> dict:
+        """update_task updates the reference (id) time tracking with the given payload. Returns the updated time tracking model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                time_tracking_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_time_tracking(self, task_id: str) -> None:
+        """delete_time_tracking returns None on success and raises an exception if the time tracking couldn't be deleted"""
+
+        self.__client.call("DELETE", Helper.create_request_url_from_params(
+            self.__endpoint + "/" + task_id), self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_serial_numbers.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_serial_numbers.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceSerialNumbers(ResourceAbstract):
-    __endpoint: str = "/serial-numbers"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_serial_numbers(self, params: dict = None) -> dict:
-        """get_serial_numbers returns a dict with serial number objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_serial_number(self, serial_number_id: str) -> dict:
-        """get_serial_number returns the referenced (id) serial number"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                serial_number_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_serial_number(self, payload: dict) -> dict:
-        """create_serial_number returns the serial number model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def delete_serial_number(self, serial_number_id: str) -> None:
-        """delete_serial_number returns None on success and raises an exception if the serial number couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                serial_number_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceSerialNumbers(ResourceAbstract):
+    __endpoint: str = "/serial-numbers"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_serial_numbers(self, params: dict = None) -> dict:
+        """get_serial_numbers returns a dict with serial number objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_serial_number(self, serial_number_id: str) -> dict:
+        """get_serial_number returns the referenced (id) serial number"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                serial_number_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_serial_number(self, payload: dict) -> dict:
+        """create_serial_number returns the serial number model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def delete_serial_number(self, serial_number_id: str) -> None:
+        """delete_serial_number returns None on success and raises an exception if the serial number couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                serial_number_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_tasks.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_tasks.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceTasks(ResourceAbstract):
-    __endpoint: str = "/tasks"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_tasks(self, params: dict = None) -> dict:
-        """get_tasks returns a dict with task objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_task(self, task_id: str) -> dict:
-        """get_task returns the referenced (id) task"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint + "/" + task_id),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def create_task(self, payload: dict) -> dict:
-        """create_task returns the task model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_task(self, task_id: str, payload: dict) -> dict:
-        """update_task updates the reference (id) task with the given payload. Returns the updated task model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + task_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_task(self, task_id: str) -> None:
-        """delete_task returns None on success and raises an exception if the task couldn't be deleted"""
-
-        self.__client.call("DELETE", Helper.create_request_url_from_params(
-            self.__endpoint + "/" + task_id), self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceTasks(ResourceAbstract):
+    __endpoint: str = "/tasks"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_tasks(self, params: dict = None) -> dict:
+        """get_tasks returns a dict with task objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_task(self, task_id: str) -> dict:
+        """get_task returns the referenced (id) task"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint + "/" + task_id),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def create_task(self, payload: dict) -> dict:
+        """create_task returns the task model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_task(self, task_id: str, payload: dict) -> dict:
+        """update_task updates the reference (id) task with the given payload. Returns the updated task model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + task_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_task(self, task_id: str) -> None:
+        """delete_task returns None on success and raises an exception if the task couldn't be deleted"""
+
+        self.__client.call("DELETE", Helper.create_request_url_from_params(
+            self.__endpoint + "/" + task_id), self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_text_templates.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_text_templates.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceTextTemplates(ResourceAbstract):
-    __endpoint: str = "/text-templates"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_text_templates(self, params: dict = None) -> dict:
-        """get_text_templates returns a dict with text templates objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_text_template(self, text_template_id: str) -> dict:
-        """get_text_template returns the referenced (id) text template"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                text_template_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_text_template(self, payload: dict) -> dict:
-        """create_text_template returns the text template model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_text_template(
-            self,
-            text_template_id: str,
-            payload: dict) -> dict:
-        """update_text_template updates the reference (id) task with the given payload. Returns the updated text template model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                text_template_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_text_template(self, text_template_id: str) -> None:
-        """delete_text_template returns None on success and raises an exception if the text template couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                text_template_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceTextTemplates(ResourceAbstract):
+    __endpoint: str = "/text-templates"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_text_templates(self, params: dict = None) -> dict:
+        """get_text_templates returns a dict with text templates objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_text_template(self, text_template_id: str) -> dict:
+        """get_text_template returns the referenced (id) text template"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                text_template_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_text_template(self, payload: dict) -> dict:
+        """create_text_template returns the text template model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_text_template(
+            self,
+            text_template_id: str,
+            payload: dict) -> dict:
+        """update_text_template updates the reference (id) task with the given payload. Returns the updated text template model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                text_template_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_text_template(self, text_template_id: str) -> None:
+        """delete_text_template returns None on success and raises an exception if the text template couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                text_template_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest/resources/resource_webhooks.py` & `easybill_rest-0.3.2/easybill_rest/resources/resource_webhooks.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING
-
-from easybill_rest.helper import Helper
-from easybill_rest.resources.resource_abstract import ResourceAbstract
-
-if TYPE_CHECKING:
-    from easybill_rest import Client
-
-
-class ResourceWebhooks(ResourceAbstract):
-    __endpoint: str = "/webhooks"
-    __client: Client
-
-    def __init__(self, client: Client) -> None:
-        super().__init__()
-        self.__client = client
-
-    def get_resource_endpoint(self):
-        return self.__endpoint
-
-    def get_webhooks(self, params: dict = None) -> dict:
-        """get_webhooks returns a dict with webhook objects"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(self.__endpoint, params),
-            self.__client.get_basic_headers_for_json()
-        )
-
-    def get_webhook(self, webhook_id: str) -> dict:
-        """get_webhook returns the referenced (id) webhook"""
-
-        return self.__client.call(
-            "GET",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + webhook_id),
-            self.__client.get_basic_headers_for_json())
-
-    def create_webhook(self, payload: dict) -> dict:
-        """create_webhook returns the webhook model as dict on success with the data from the passed payload"""
-
-        return self.__client.call(
-            "POST",
-            Helper.create_request_url_from_params(self.__endpoint),
-            self.__client.get_basic_headers_for_json(),
-            payload
-        )
-
-    def update_webhook(self, webhook_id: str, payload: dict) -> dict:
-        """update_webhook updates the reference (id) webhook with the given payload. Returns the updated webhook model"""
-
-        return self.__client.call(
-            "PUT",
-            Helper.create_request_url_from_params(
-                self.__endpoint +
-                "/" +
-                webhook_id),
-            self.__client.get_basic_headers_for_json(),
-            payload)
-
-    def delete_webhook(self, webhook_id: str) -> None:
-        """delete_webhook returns None on success and raises an exception if the webhook couldn't be deleted"""
-
-        self.__client.call(
-            "DELETE",
-            Helper.create_request_url_from_params(
-                self.__endpoint + "/" + webhook_id),
-            self.__client.get_basic_headers())
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from easybill_rest.helper import Helper
+from easybill_rest.resources.resource_abstract import ResourceAbstract
+
+if TYPE_CHECKING:
+    from easybill_rest import Client
+
+
+class ResourceWebhooks(ResourceAbstract):
+    __endpoint: str = "/webhooks"
+    __client: Client
+
+    def __init__(self, client: Client) -> None:
+        super().__init__()
+        self.__client = client
+
+    def get_resource_endpoint(self):
+        return self.__endpoint
+
+    def get_webhooks(self, params: dict = None) -> dict:
+        """get_webhooks returns a dict with webhook objects"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(self.__endpoint, params),
+            self.__client.get_basic_headers_for_json()
+        )
+
+    def get_webhook(self, webhook_id: str) -> dict:
+        """get_webhook returns the referenced (id) webhook"""
+
+        return self.__client.call(
+            "GET",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + webhook_id),
+            self.__client.get_basic_headers_for_json())
+
+    def create_webhook(self, payload: dict) -> dict:
+        """create_webhook returns the webhook model as dict on success with the data from the passed payload"""
+
+        return self.__client.call(
+            "POST",
+            Helper.create_request_url_from_params(self.__endpoint),
+            self.__client.get_basic_headers_for_json(),
+            payload
+        )
+
+    def update_webhook(self, webhook_id: str, payload: dict) -> dict:
+        """update_webhook updates the reference (id) webhook with the given payload. Returns the updated webhook model"""
+
+        return self.__client.call(
+            "PUT",
+            Helper.create_request_url_from_params(
+                self.__endpoint +
+                "/" +
+                webhook_id),
+            self.__client.get_basic_headers_for_json(),
+            payload)
+
+    def delete_webhook(self, webhook_id: str) -> None:
+        """delete_webhook returns None on success and raises an exception if the webhook couldn't be deleted"""
+
+        self.__client.call(
+            "DELETE",
+            Helper.create_request_url_from_params(
+                self.__endpoint + "/" + webhook_id),
+            self.__client.get_basic_headers())
```

### Comparing `easybill_rest-0.3.1/easybill_rest.egg-info/PKG-INFO` & `easybill_rest-0.3.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-Metadata-Version: 2.1
-Name: easybill-rest
-Version: 0.3.1
-Summary: easybill_rest is a library to work with the easybill REST API (https://www.easybill.de/api/)
-Home-page: https://github.com/BolZer/py-ebrest
-Author: Jan Noehles (bolZer)
-Author-email: noehles@easybill.de
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
-# easybill_rest (py-ebrest)
-[![Generic badge](https://img.shields.io/badge/Version-0.3.1-important.svg)]()
-[![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
-[![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
-[![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
-
-`easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
-
-All Resources are available.
-
-The library supports only the `Bearer` Authentication and calls the API only
-through `HTTPS`.
-
-```bash
-pip install easybill_rest
-```
-
-
-## Usage
-
-```Python
-from easybill_rest import Client
-
-
-client = Client("API-KEY")
-result = client.documents().get_document("2")
-
-# Returns the document model. Therefore a field "title" is included in the dict.
-print(result['title'])
-
-```
+Metadata-Version: 2.1
+Name: easybill_rest
+Version: 0.3.2
+Summary: easybill_rest is a library to work with the easybill REST API (https://www.easybill.de/api/)
+Home-page: https://github.com/BolZer/py-ebrest
+Author: Jan Noehles (bolZer)
+Author-email: noehles@easybill.de
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: license.md
+
+# easybill_rest (py-ebrest)
+[![Generic badge](https://img.shields.io/badge/Version-0.3.2-important.svg)]()
+[![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
+[![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
+[![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
+
+`easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
+
+All Resources are available.
+
+The library supports only the `Bearer` Authentication and calls the API only
+through `HTTPS`.
+
+```bash
+pip install easybill_rest
+```
+
+
+## Usage
+
+```Python
+from easybill_rest import Client
+
+
+client = Client("API-KEY")
+result = client.documents().get_document("2")
+
+# Returns the document model. Therefore a field "title" is included in the dict.
+print(result['title'])
+
+```
```

### Comparing `easybill_rest-0.3.1/easybill_rest.egg-info/SOURCES.txt` & `easybill_rest-0.3.2/easybill_rest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easybill_rest-0.3.1/license.md` & `easybill_rest-0.3.2/license.md`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-MIT License
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `easybill_rest-0.3.1/readme.md` & `easybill_rest-0.3.2/readme.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# easybill_rest (py-ebrest)
-[![Generic badge](https://img.shields.io/badge/Version-0.3.1-important.svg)]()
-[![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
-[![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
-[![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
-
-`easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
-
-All Resources are available.
-
-The library supports only the `Bearer` Authentication and calls the API only
-through `HTTPS`.
-
-```bash
-pip install easybill_rest
-```
-
-
-## Usage
-
-```Python
-from easybill_rest import Client
-
-
-client = Client("API-KEY")
-result = client.documents().get_document("2")
-
-# Returns the document model. Therefore a field "title" is included in the dict.
-print(result['title'])
-
+# easybill_rest (py-ebrest)
+[![Generic badge](https://img.shields.io/badge/Version-0.3.2-important.svg)]()
+[![Generic badge](https://img.shields.io/badge/coverage-97%25-success.svg)]()
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/easybill_rest.svg)
+[![Generic badge](https://img.shields.io/badge/License-MIT-blue.svg)]()
+[![Build Status](https://travis-ci.com/BolZer/py-ebrest.svg?branch=master)](https://travis-ci.com/BolZer/py-ebrest)
+
+`easybill_rest` is a library to work with the easybill REST API (https://www.easybill.de/api/) written in Python.
+
+All Resources are available.
+
+The library supports only the `Bearer` Authentication and calls the API only
+through `HTTPS`.
+
+```bash
+pip install easybill_rest
+```
+
+
+## Usage
+
+```Python
+from easybill_rest import Client
+
+
+client = Client("API-KEY")
+result = client.documents().get_document("2")
+
+# Returns the document model. Therefore a field "title" is included in the dict.
+print(result['title'])
+
 ```
```

