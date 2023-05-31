# Comparing `tmp/odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1-py3-none-any.whl.zip` & `tmp/odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 12365 bytes, number of entries: 7
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-27 18:11 odoo/addons/hr_attendance_calendar_view/__manifest__.py
--rw-r--r--  2.0 unx     9455 b- defN 23-Apr-27 18:11 odoo/addons/hr_attendance_calendar_view/static/description/icon.png
--rw-r--r--  2.0 unx      833 b- defN 23-Apr-27 18:11 odoo/addons/hr_attendance_calendar_view/views/hr_attendance_calendar_views.xml
--rw-r--r--  2.0 unx      591 b- defN 23-Apr-27 18:11 odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 18:11 odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-27 18:11 odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      817 b- defN 23-Apr-27 18:11 odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/RECORD
-7 files, 12370 bytes uncompressed, 10851 bytes compressed:  12.3%
+-rw-r--r--  2.0 unx      577 b- defN 23-May-31 15:07 odoo/addons/hr_attendance_calendar_view/__manifest__.py
+-rw-r--r--  2.0 unx     9455 b- defN 23-May-31 15:07 odoo/addons/hr_attendance_calendar_view/static/description/icon.png
+-rw-r--r--  2.0 unx      833 b- defN 23-May-31 15:07 odoo/addons/hr_attendance_calendar_view/views/hr_attendance_calendar_views.xml
+-rw-r--r--  2.0 unx      592 b- defN 23-May-31 15:07 odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 15:07 odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-31 15:07 odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      817 b- defN 23-May-31 15:07 odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/RECORD
+7 files, 12371 bytes uncompressed, 10851 bytes compressed:  12.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: odoo/addons/hr_attendance_calendar_view/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/hr_attendance_calendar_view/views/hr_attendance_calendar_views.xml
 Comment: 
 
-Filename: odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/METADATA
+Filename: odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/WHEEL
+Filename: odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/top_level.txt
+Filename: odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/RECORD
+Filename: odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/hr_attendance_calendar_view/__manifest__.py

```diff
@@ -5,13 +5,13 @@
     "name": "Add calendar view to attendance, hr_attendance_calendar_view",
     "summary": """
         This module adds the calendar view as an option to display attendance""",
     "license": "AGPL-3",
     "author": "Odoo Community Association (OCA)",
     "website": "https://github.com/OCA/hr-attendance",
     "category": "Human Resources",
-    "version": "15.0.1.0.0",
+    "version": "16.0.1.0.0",
     "depends": ["base", "hr_attendance"],
     "data": [
         "views/hr_attendance_calendar_views.xml",
     ],
 }
```

## Comparing `odoo_addon_hr_attendance_calendar_view-15.0.1.0.0.1.dist-info/METADATA` & `odoo_addon_hr_attendance_calendar_view-16.0.1.0.0.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: odoo-addon-hr-attendance-calendar-view
-Version: 15.0.1.0.0.1
+Version: 16.0.1.0.0.1
 Summary: This module adds the calendar view as an option to display attendance
 Home-page: https://github.com/OCA/hr-attendance
 Author: Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
-Classifier: Framework :: Odoo :: 15.0
+Classifier: Framework :: Odoo :: 16.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Requires-Python: >=3.8
-Requires-Dist: odoo (<15.1dev,>=15.0a)
+Requires-Python: >=3.10
+Requires-Dist: odoo (<16.1dev,>=16.0a)
 
 UNKNOWN
```

