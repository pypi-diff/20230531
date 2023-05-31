# Comparing `tmp/odoo14_addons_oca_account_invoicing-14.0.20230324.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_account_invoicing-14.0.20230530.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2026 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4292 b- defN 23-Mar-25 03:04 odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-25 03:04 odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-25 03:04 odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      449 b- defN 23-Mar-25 03:04 odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/RECORD
-4 files, 4834 bytes uncompressed, 1140 bytes compressed:  76.4%
+Zip file size: 2039 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     4358 b- defN 23-May-31 02:45 odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 02:45 odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-31 02:45 odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      449 b- defN 23-May-31 02:45 odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/RECORD
+4 files, 4900 bytes uncompressed, 1153 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/METADATA
+Filename: odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/RECORD
+Filename: odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_account_invoicing-14.0.20230324.0.dist-info/METADATA` & `odoo14_addons_oca_account_invoicing-14.0.20230530.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-account-invoicing
-Version: 14.0.20230324.0
+Version: 14.0.20230530.0
 Summary: Meta package for oca-account-invoicing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -57,14 +57,15 @@
 Requires-Dist: odoo14-addon-account-move-line-accounting-description
 Requires-Dist: odoo14-addon-account-move-line-accounting-description-purchase
 Requires-Dist: odoo14-addon-account-move-line-accounting-description-sale
 Requires-Dist: odoo14-addon-account-move-original-partner
 Requires-Dist: odoo14-addon-account-move-post-block
 Requires-Dist: odoo14-addon-account-move-propagate-ref
 Requires-Dist: odoo14-addon-account-move-tier-validation
+Requires-Dist: odoo14-addon-account-move-tier-validation-approver
 Requires-Dist: odoo14-addon-account-move-tier-validation-forward
 Requires-Dist: odoo14-addon-account-receipt-journal
 Requires-Dist: odoo14-addon-account-receipt-print
 Requires-Dist: odoo14-addon-account-refund-payment-term
 Requires-Dist: odoo14-addon-product-supplierinfo-for-customer-invoice
 Requires-Dist: odoo14-addon-purchase-stock-picking-return-invoicing
 Requires-Dist: odoo14-addon-sale-line-refund-to-invoice-qty
```

