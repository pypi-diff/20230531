# Comparing `tmp/mercoa-0.0.9.tar.gz` & `tmp/mercoa-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.0.9.tar", max compression
+gzip compressed data, was "mercoa-0.1.0.tar", max compression
```

## Comparing `mercoa-0.0.9.tar` & `mercoa-0.1.0.tar`

### file list

```diff
@@ -1,149 +1,167 @@
--rw-r--r--   0        0        0      410 2023-05-19 14:42:27.516931 mercoa-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     5163 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/__init__.py
--rw-r--r--   0        0        0     5449 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      326 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/py.typed
--rw-r--r--   0        0        0     5313 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     2582 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      359 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      148 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      216 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      407 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      855 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      199 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4513 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/client.py
--rw-r--r--   0        0        0      256 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/types/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/types/counterparty_response.py
--rw-r--r--   0        0        0     1446 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/types/find_counterparties_response.py
--rw-r--r--   0        0        0      811 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    21970 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     1195 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/__init__.py
--rw-r--r--   0        0        0      487 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/account_type.py
--rw-r--r--   0        0        0     1535 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/business_type.py
--rw-r--r--   0        0        0      741 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/ein.py
--rw-r--r--   0        0        0       80 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_id.py
--rw-r--r--   0        0        0     2432 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_request.py
--rw-r--r--   0        0        0     1814 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_status.py
--rw-r--r--   0        0        0     2084 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_update_request.py
--rw-r--r--   0        0        0     1372 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/individual_profile_response.py
--rw-r--r--   0        0        0     1059 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/invoice_metrics_response.py
--rw-r--r--   0        0        0      974 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/profile_response.py
--rw-r--r--   0        0        0      761 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/tax_id.py
--rw-r--r--   0        0        0      207 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/__init__.py
--rw-r--r--   0        0        0     9662 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/client.py
--rw-r--r--   0        0        0      281 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/types/__init__.py
--rw-r--r--   0        0        0       84 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_response.py
--rw-r--r--   0        0        0      633 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    19563 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      916 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0       81 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_id.py
--rw-r--r--   0        0        0      750 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_request.py
--rw-r--r--   0        0        0      937 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_response.py
--rw-r--r--   0        0        0     1048 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/create_vendor_request.py
--rw-r--r--   0        0        0    22179 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/currency_code.py
--rw-r--r--   0        0        0      955 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/document_response.py
--rw-r--r--   0        0        0       81 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_id.py
--rw-r--r--   0        0        0     1302 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1229 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     3437 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_request.py
--rw-r--r--   0        0        0     3144 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_response.py
--rw-r--r--   0        0        0     1485 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_status.py
--rw-r--r--   0        0        0      213 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4443 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      298 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/attachments.py
--rw-r--r--   0        0        0     1969 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/email_ocr_request.py
--rw-r--r--   0        0        0      891 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/ocr_mailbox.py
--rw-r--r--   0        0        0     1234 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      983 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0     7449 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1466 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      948 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      656 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1463 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1579 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1145 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      797 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0      943 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    12242 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/client.py
--rw-r--r--   0        0        0     1411 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/__init__.py
--rw-r--r--   0        0        0       85 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_id.py
--rw-r--r--   0        0        0     1297 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_request.py
--rw-r--r--   0        0        0     1318 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_brand.py
--rw-r--r--   0        0        0       78 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_id.py
--rw-r--r--   0        0        0     1120 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_request.py
--rw-r--r--   0        0        0     1217 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_response.py
--rw-r--r--   0        0        0      750 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_type.py
--rw-r--r--   0        0        0       79 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_id.py
--rw-r--r--   0        0        0     1152 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_request.py
--rw-r--r--   0        0        0     1327 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_response.py
--rw-r--r--   0        0        0       80 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_id.py
--rw-r--r--   0        0        0     1568 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1922 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
--rw-r--r--   0        0        0       87 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_id.py
--rw-r--r--   0        0        0     1296 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_request.py
--rw-r--r--   0        0        0     1662 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_response.py
--rw-r--r--   0        0        0     1229 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_type.py
--rw-r--r--   0        0        0      425 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0     7794 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0      589 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/__init__.py
--rw-r--r--   0        0        0     1984 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1597 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1709 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
--rw-r--r--   0        0        0      143 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/process_invoice/__init__.py
--rw-r--r--   0        0        0     2498 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/process_invoice/client.py
--rw-r--r--   0        0        0      161 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/process_invoice/types/__init__.py
--rw-r--r--   0        0        0      916 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/process_invoice/types/process_invoice_request.py
--rw-r--r--   0        0        0      269 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/__init__.py
--rw-r--r--   0        0        0     8182 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/client.py
--rw-r--r--   0        0        0      381 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/__init__.py
--rw-r--r--   0        0        0       88 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/responsibilities.py
--rw-r--r--   0        0        0      271 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     4315 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      386 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1125 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1564 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_response_expanded.py
--rw-r--r--   0        0        0     1261 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-05-31 04:09:52.712105 mercoa-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6243 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     5449 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/py.typed
+-rw-r--r--   0        0        0     6430 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     2582 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      397 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      469 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0      855 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      199 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4513 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/client.py
+-rw-r--r--   0        0        0      256 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/types/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/types/counterparty_response.py
+-rw-r--r--   0        0        0     1446 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/types/find_counterparties_response.py
+-rw-r--r--   0        0        0     1491 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    34975 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0     2109 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/account_type.py
+-rw-r--r--   0        0        0      836 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/amount_trigger.py
+-rw-r--r--   0        0        0     1075 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1003 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1059 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0      963 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/approver_rule.py
+-rw-r--r--   0        0        0     1535 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/business_profile_request.py
+-rw-r--r--   0        0        0     1492 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/business_type.py
+-rw-r--r--   0        0        0      741 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/ein.py
+-rw-r--r--   0        0        0      914 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0       80 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_id.py
+-rw-r--r--   0        0        0     2432 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_request.py
+-rw-r--r--   0        0        0     1814 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_update_request.py
+-rw-r--r--   0        0        0      727 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/identifier_list.py
+-rw-r--r--   0        0        0     1372 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/individual_profile_response.py
+-rw-r--r--   0        0        0     1059 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0       80 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/policy_id.py
+-rw-r--r--   0        0        0      974 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/profile_response.py
+-rw-r--r--   0        0        0      428 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/rule.py
+-rw-r--r--   0        0        0      761 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/tax_id.py
+-rw-r--r--   0        0        0      594 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/trigger.py
+-rw-r--r--   0        0        0      207 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/__init__.py
+-rw-r--r--   0        0        0     9662 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/client.py
+-rw-r--r--   0        0        0      281 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/types/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_response.py
+-rw-r--r--   0        0        0      847 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    23201 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0     1253 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/__init__.py
+-rw-r--r--   0        0        0      935 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/approval_request.py
+-rw-r--r--   0        0        0      990 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/approver.py
+-rw-r--r--   0        0        0      631 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/approver_action.py
+-rw-r--r--   0        0        0      862 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/approver_response.py
+-rw-r--r--   0        0        0       81 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/comment_id.py
+-rw-r--r--   0        0        0      934 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/comment_request.py
+-rw-r--r--   0        0        0     1128 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/comment_response.py
+-rw-r--r--   0        0        0     1048 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/create_vendor_request.py
+-rw-r--r--   0        0        0    22179 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/currency_code.py
+-rw-r--r--   0        0        0      955 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/document_response.py
+-rw-r--r--   0        0        0       81 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_id.py
+-rw-r--r--   0        0        0     1302 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1229 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0      870 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     4084 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_request.py
+-rw-r--r--   0        0        0     4060 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_response.py
+-rw-r--r--   0        0        0     1485 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_status.py
+-rw-r--r--   0        0        0      213 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4443 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      298 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/attachments.py
+-rw-r--r--   0        0        0     1969 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/email_ocr_request.py
+-rw-r--r--   0        0        0      891 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/ocr_mailbox.py
+-rw-r--r--   0        0        0     1234 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      983 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0     7449 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1466 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      656 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1145 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      797 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0     1087 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    14367 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/client.py
+-rw-r--r--   0        0        0     1638 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_id.py
+-rw-r--r--   0        0        0     1297 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_request.py
+-rw-r--r--   0        0        0     1318 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_type.py
+-rw-r--r--   0        0        0      819 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_brand.py
+-rw-r--r--   0        0        0       78 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_id.py
+-rw-r--r--   0        0        0     1120 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_request.py
+-rw-r--r--   0        0        0     1217 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_type.py
+-rw-r--r--   0        0        0       79 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_id.py
+-rw-r--r--   0        0        0     1152 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_request.py
+-rw-r--r--   0        0        0     1327 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_response.py
+-rw-r--r--   0        0        0       80 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_id.py
+-rw-r--r--   0        0        0     1568 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1922 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1639 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0       87 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_id.py
+-rw-r--r--   0        0        0     1296 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_request.py
+-rw-r--r--   0        0        0     1662 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_response.py
+-rw-r--r--   0        0        0     1229 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_type.py
+-rw-r--r--   0        0        0      893 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_update_request.py
+-rw-r--r--   0        0        0      425 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0     7794 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0      589 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/__init__.py
+-rw-r--r--   0        0        0     1984 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1597 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1709 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0      143 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/process_invoice/__init__.py
+-rw-r--r--   0        0        0     2498 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/process_invoice/client.py
+-rw-r--r--   0        0        0      161 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/process_invoice/types/__init__.py
+-rw-r--r--   0        0        0      916 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/process_invoice/types/process_invoice_request.py
+-rw-r--r--   0        0        0      269 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/__init__.py
+-rw-r--r--   0        0        0     8182 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/client.py
+-rw-r--r--   0        0        0      381 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/responsibilities.py
+-rw-r--r--   0        0        0      271 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     4315 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1125 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1564 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.1.0/PKG-INFO
```

### Comparing `mercoa-0.0.9/src/mercoa/__init__.py` & `mercoa-0.1.0/src/mercoa/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 from .environment import MercoaEnvironment
 from .resources import (
     ITIN,
     SSN,
     AccountType,
     Address,
+    AmountTrigger,
+    ApprovalPolicyRequest,
+    ApprovalPolicyResponse,
+    ApprovalPolicyUpdateRequest,
+    ApprovalRequest,
+    Approver,
+    ApproverAction,
+    ApproverResponse,
+    ApproverRule,
     Attachments,
     BankAccountId,
     BankAccountRequest,
     BankAccountResponse,
     BankAddress,
     BankLookupResponse,
     BankStatus,
@@ -33,76 +42,90 @@
     CommentResponse,
     CounterpartyResponse,
     CreateVendorRequest,
     CurrencyCode,
     CustomId,
     CustomPaymentMethodRequest,
     CustomPaymentMethodResponse,
+    CustomPaymentMethodUpdateRequest,
     DocumentResponse,
     Ein,
     EmailLogResponse,
     EmailOcrRequest,
     EmailProviderRequest,
     EmailProviderResponse,
     EmailSenderProvider,
     EmailSenderRequest,
     EmailSenderResponse,
+    EntityAddPayeesRequest,
     EntityId,
     EntityRequest,
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     EntityUserId,
     EntityUserRequest,
     EntityUserResponse,
     FindCounterpartiesResponse,
     FullName,
+    IdentifierList,
+    IdentifierList_RolesList,
+    IdentifierList_UserList,
     IndividualGovernmentID,
     IndividualProfileRequest,
     IndividualProfileResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
+    InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     OcrMailbox,
     OCRResponse,
+    OrderDirection,
     OrganizationId,
     OrganizationRequest,
     OrganizationResponse,
     PaymentMethodId,
     PaymentMethodRequest,
     PaymentMethodResponse,
     PaymentMethodSchemaField,
     PaymentMethodSchemaFieldType,
     PaymentMethodSchemaId,
     PaymentMethodSchemaRequest,
     PaymentMethodSchemaResponse,
     PaymentMethodsRequest,
     PaymentMethodsResponse,
     PaymentMethodType,
+    PaymentMethodUpdateRequest,
     PaymentRailMarkup,
     PaymentRailMarkupType,
     PaymentRailRequest,
     PaymentRailResponse,
     PhoneNumber,
+    PolicyId,
     ProcessInvoiceRequest,
     ProfileRequest,
     ProfileResponse,
     RepresentativeId,
     RepresentativeRequest,
     RepresentativeResponse,
     Responsibilities,
+    Rule,
+    Rule_Approver,
     TaxID,
     TransactionId,
     TransactionResponse,
     TransactionResponseExpanded,
     TransactionStatus,
+    Trigger,
+    Trigger_All,
+    Trigger_Amount,
     UnauthorizedError,
     bank_lookup,
     commons,
     counterparty,
     entity,
     entity_users,
     invoice,
@@ -114,14 +137,23 @@
     representative,
     transaction,
 )
 
 __all__ = [
     "AccountType",
     "Address",
+    "AmountTrigger",
+    "ApprovalPolicyRequest",
+    "ApprovalPolicyResponse",
+    "ApprovalPolicyUpdateRequest",
+    "ApprovalRequest",
+    "Approver",
+    "ApproverAction",
+    "ApproverResponse",
+    "ApproverRule",
     "Attachments",
     "BankAccountId",
     "BankAccountRequest",
     "BankAccountResponse",
     "BankAddress",
     "BankLookupResponse",
     "BankStatus",
@@ -145,79 +177,93 @@
     "CommentResponse",
     "CounterpartyResponse",
     "CreateVendorRequest",
     "CurrencyCode",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
+    "CustomPaymentMethodUpdateRequest",
     "DocumentResponse",
     "Ein",
     "EmailLogResponse",
     "EmailOcrRequest",
     "EmailProviderRequest",
     "EmailProviderResponse",
     "EmailSenderProvider",
     "EmailSenderRequest",
     "EmailSenderResponse",
+    "EntityAddPayeesRequest",
     "EntityId",
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "EntityUserId",
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
     "FullName",
     "ITIN",
+    "IdentifierList",
+    "IdentifierList_RolesList",
+    "IdentifierList_UserList",
     "IndividualGovernmentID",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
+    "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "MercoaEnvironment",
     "OCRResponse",
     "OcrMailbox",
+    "OrderDirection",
     "OrganizationId",
     "OrganizationRequest",
     "OrganizationResponse",
     "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodResponse",
     "PaymentMethodSchemaField",
     "PaymentMethodSchemaFieldType",
     "PaymentMethodSchemaId",
     "PaymentMethodSchemaRequest",
     "PaymentMethodSchemaResponse",
     "PaymentMethodType",
+    "PaymentMethodUpdateRequest",
     "PaymentMethodsRequest",
     "PaymentMethodsResponse",
     "PaymentRailMarkup",
     "PaymentRailMarkupType",
     "PaymentRailRequest",
     "PaymentRailResponse",
     "PhoneNumber",
+    "PolicyId",
     "ProcessInvoiceRequest",
     "ProfileRequest",
     "ProfileResponse",
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
+    "Rule",
+    "Rule_Approver",
     "SSN",
     "TaxID",
     "TransactionId",
     "TransactionResponse",
     "TransactionResponseExpanded",
     "TransactionStatus",
+    "Trigger",
+    "Trigger_All",
+    "Trigger_Amount",
     "UnauthorizedError",
     "bank_lookup",
     "commons",
     "counterparty",
     "entity",
     "entity_users",
     "invoice",
```

### Comparing `mercoa-0.0.9/src/mercoa/client.py` & `mercoa-0.1.0/src/mercoa/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/core/datetime_utils.py` & `mercoa-0.1.0/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.1.0/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,45 +12,75 @@
     payment_method,
     payment_method_schema,
     process_invoice,
     representative,
     transaction,
 )
 from .bank_lookup import BankAddress, BankLookupResponse
-from .commons import ITIN, SSN, Address, BirthDate, FullName, IndividualGovernmentID, PhoneNumber, UnauthorizedError
+from .commons import (
+    ITIN,
+    SSN,
+    Address,
+    BirthDate,
+    FullName,
+    IndividualGovernmentID,
+    OrderDirection,
+    PhoneNumber,
+    UnauthorizedError,
+)
 from .counterparty import CounterpartyResponse, FindCounterpartiesResponse
 from .entity import (
     AccountType,
+    AmountTrigger,
+    ApprovalPolicyRequest,
+    ApprovalPolicyResponse,
+    ApprovalPolicyUpdateRequest,
+    ApproverRule,
     BusinessProfileRequest,
     BusinessProfileResponse,
     BusinessType,
     Ein,
+    EntityAddPayeesRequest,
     EntityId,
     EntityRequest,
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
+    IdentifierList,
+    IdentifierList_RolesList,
+    IdentifierList_UserList,
     IndividualProfileRequest,
     IndividualProfileResponse,
     InvoiceMetricsResponse,
+    PolicyId,
     ProfileRequest,
     ProfileResponse,
+    Rule,
+    Rule_Approver,
     TaxID,
+    Trigger,
+    Trigger_All,
+    Trigger_Amount,
 )
 from .entity_users import EntityUserId, EntityUserRequest, EntityUserResponse
 from .invoice import (
+    ApprovalRequest,
+    Approver,
+    ApproverAction,
+    ApproverResponse,
     CommentId,
     CommentRequest,
     CommentResponse,
     CreateVendorRequest,
     CurrencyCode,
     DocumentResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
+    InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
 )
 from .ocr import Attachments, EmailOcrRequest, OcrMailbox, OCRResponse
 from .organization import (
     ColorSchemeRequest,
@@ -84,18 +114,20 @@
     CardType,
     CheckId,
     CheckRequest,
     CheckResponse,
     CustomId,
     CustomPaymentMethodRequest,
     CustomPaymentMethodResponse,
+    CustomPaymentMethodUpdateRequest,
     PaymentMethodId,
     PaymentMethodRequest,
     PaymentMethodResponse,
     PaymentMethodType,
+    PaymentMethodUpdateRequest,
 )
 from .payment_method_schema import (
     PaymentMethodSchemaField,
     PaymentMethodSchemaFieldType,
     PaymentMethodSchemaId,
     PaymentMethodSchemaRequest,
     PaymentMethodSchemaResponse,
@@ -103,14 +135,23 @@
 from .process_invoice import ProcessInvoiceRequest
 from .representative import RepresentativeId, RepresentativeRequest, RepresentativeResponse, Responsibilities
 from .transaction import TransactionId, TransactionResponse, TransactionResponseExpanded, TransactionStatus
 
 __all__ = [
     "AccountType",
     "Address",
+    "AmountTrigger",
+    "ApprovalPolicyRequest",
+    "ApprovalPolicyResponse",
+    "ApprovalPolicyUpdateRequest",
+    "ApprovalRequest",
+    "Approver",
+    "ApproverAction",
+    "ApproverResponse",
+    "ApproverRule",
     "Attachments",
     "BankAccountId",
     "BankAccountRequest",
     "BankAccountResponse",
     "BankAddress",
     "BankLookupResponse",
     "BankStatus",
@@ -134,78 +175,92 @@
     "CommentResponse",
     "CounterpartyResponse",
     "CreateVendorRequest",
     "CurrencyCode",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
+    "CustomPaymentMethodUpdateRequest",
     "DocumentResponse",
     "Ein",
     "EmailLogResponse",
     "EmailOcrRequest",
     "EmailProviderRequest",
     "EmailProviderResponse",
     "EmailSenderProvider",
     "EmailSenderRequest",
     "EmailSenderResponse",
+    "EntityAddPayeesRequest",
     "EntityId",
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "EntityUserId",
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
     "FullName",
     "ITIN",
+    "IdentifierList",
+    "IdentifierList_RolesList",
+    "IdentifierList_UserList",
     "IndividualGovernmentID",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
+    "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "OCRResponse",
     "OcrMailbox",
+    "OrderDirection",
     "OrganizationId",
     "OrganizationRequest",
     "OrganizationResponse",
     "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodResponse",
     "PaymentMethodSchemaField",
     "PaymentMethodSchemaFieldType",
     "PaymentMethodSchemaId",
     "PaymentMethodSchemaRequest",
     "PaymentMethodSchemaResponse",
     "PaymentMethodType",
+    "PaymentMethodUpdateRequest",
     "PaymentMethodsRequest",
     "PaymentMethodsResponse",
     "PaymentRailMarkup",
     "PaymentRailMarkupType",
     "PaymentRailRequest",
     "PaymentRailResponse",
     "PhoneNumber",
+    "PolicyId",
     "ProcessInvoiceRequest",
     "ProfileRequest",
     "ProfileResponse",
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
+    "Rule",
+    "Rule_Approver",
     "SSN",
     "TaxID",
     "TransactionId",
     "TransactionResponse",
     "TransactionResponseExpanded",
     "TransactionStatus",
+    "Trigger",
+    "Trigger_All",
+    "Trigger_Amount",
     "UnauthorizedError",
     "bank_lookup",
     "commons",
     "counterparty",
     "entity",
     "entity_users",
     "invoice",
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.1.0/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/commons/types/address.py` & `mercoa-0.1.0/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.1.0/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.1.0/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.1.0/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.1.0/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.1.0/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.1.0/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/counterparty/client.py` & `mercoa-0.1.0/src/mercoa/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/counterparty/types/counterparty_response.py` & `mercoa-0.1.0/src/mercoa/resources/counterparty/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/counterparty/types/find_counterparties_response.py` & `mercoa-0.1.0/src/mercoa/resources/counterparty/types/find_counterparties_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/entity/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,69 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     AccountType,
+    AmountTrigger,
+    ApprovalPolicyRequest,
+    ApprovalPolicyResponse,
+    ApprovalPolicyUpdateRequest,
+    ApproverRule,
     BusinessProfileRequest,
     BusinessProfileResponse,
     BusinessType,
     Ein,
+    EntityAddPayeesRequest,
     EntityId,
     EntityRequest,
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
+    IdentifierList,
+    IdentifierList_RolesList,
+    IdentifierList_UserList,
     IndividualProfileRequest,
     IndividualProfileResponse,
     InvoiceMetricsResponse,
+    PolicyId,
     ProfileRequest,
     ProfileResponse,
+    Rule,
+    Rule_Approver,
     TaxID,
+    Trigger,
+    Trigger_All,
+    Trigger_Amount,
 )
 
 __all__ = [
     "AccountType",
+    "AmountTrigger",
+    "ApprovalPolicyRequest",
+    "ApprovalPolicyResponse",
+    "ApprovalPolicyUpdateRequest",
+    "ApproverRule",
     "BusinessProfileRequest",
     "BusinessProfileResponse",
     "BusinessType",
     "Ein",
+    "EntityAddPayeesRequest",
     "EntityId",
     "EntityRequest",
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
+    "IdentifierList",
+    "IdentifierList_RolesList",
+    "IdentifierList_UserList",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
     "InvoiceMetricsResponse",
+    "PolicyId",
     "ProfileRequest",
     "ProfileResponse",
+    "Rule",
+    "Rule_Approver",
     "TaxID",
+    "Trigger",
+    "Trigger_All",
+    "Trigger_Amount",
 ]
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/client.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,457 +1,480 @@
 # This file was auto-generated by Fern from our API Definition.
 
-import datetime as dt
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
-from ...core.datetime_utils import serialize_datetime
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
-from ..invoice.types.currency_code import CurrencyCode
-from ..invoice.types.invoice_response import InvoiceResponse
-from ..invoice.types.invoice_status import InvoiceStatus
-from .types.entity_id import EntityId
-from .types.entity_request import EntityRequest
-from .types.entity_response import EntityResponse
-from .types.entity_status import EntityStatus
-from .types.entity_update_request import EntityUpdateRequest
-from .types.invoice_metrics_response import InvoiceMetricsResponse
+from .types.approval_request import ApprovalRequest
+from .types.comment_id import CommentId
+from .types.comment_request import CommentRequest
+from .types.comment_response import CommentResponse
+from .types.document_response import DocumentResponse
+from .types.invoice_id import InvoiceId
+from .types.invoice_request import InvoiceRequest
+from .types.invoice_response import InvoiceResponse
 
 
-class EntityClient:
+class InvoiceClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def get_all(self) -> typing.List[EntityResponse]:
+    def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def find(
-        self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
-    ) -> typing.List[EntityResponse]:
+    def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
-            params={"foreignId": foreign_id, "status": status},
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, *, request: EntityRequest) -> EntityResponse:
+    def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, entity_id: EntityId) -> EntityResponse:
+    def delete(self, invoice_id: InvoiceId) -> None:
+        _response = httpx.request(
+            "DELETE",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+        )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, entity_id: EntityId, *, request: EntityUpdateRequest) -> EntityResponse:
+    def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> InvoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/approve"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, entity_id: EntityId) -> None:
+    def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> InvoiceResponse:
         _response = httpx.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/reject"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_invoices(
-        self, entity_id: EntityId, *, status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]]
-    ) -> typing.List[InvoiceResponse]:
+    def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
-            params={"status": status},
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[CommentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_invoice_metrics(
-        self,
-        entity_id: EntityId,
-        *,
-        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-        due_date_start: typing.Optional[dt.datetime] = None,
-        due_date_end: typing.Optional[dt.datetime] = None,
-        created_date_start: typing.Optional[dt.datetime] = None,
-        created_date_end: typing.Optional[dt.datetime] = None,
-        currency: CurrencyCode,
-    ) -> InvoiceMetricsResponse:
+    def add_comment(self, invoice_id: InvoiceId, *, request: CommentRequest) -> CommentResponse:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoice-metrics"),
-            params={
-                "status": status,
-                "dueDateStart": serialize_datetime(due_date_start) if due_date_start is not None else None,
-                "dueDateEnd": serialize_datetime(due_date_end) if due_date_end is not None else None,
-                "createdDateStart": serialize_datetime(created_date_start) if created_date_start is not None else None,
-                "createdDateEnd": serialize_datetime(created_date_end) if created_date_end is not None else None,
-                "currency": currency,
-            },
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceMetricsResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def accept_terms_of_service(self, entity_id: EntityId) -> str:
+    def edit_comment(self, invoice_id: InvoiceId, comment_id: CommentId, *, request: CommentRequest) -> CommentResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_token(self, entity_id: EntityId) -> str:
+    def delete_comment(self, invoice_id: InvoiceId, comment_id: CommentId) -> None:
         _response = httpx.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
+            "DELETE",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def plaid_link_token(self, entity_id: EntityId) -> str:
+    def get_vendor_link(self, invoice_id: InvoiceId) -> str:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def send_vendor_email(self, invoice_id: InvoiceId) -> None:
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+        )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
-class AsyncEntityClient:
+class AsyncInvoiceClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def get_all(self) -> typing.List[EntityResponse]:
+    async def create(self, *, request: InvoiceRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", "invoice"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def find(
-        self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
-    ) -> typing.List[EntityResponse]:
+    async def get(self, invoice_id: InvoiceId) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
-                params={"foreignId": foreign_id, "status": status},
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, *, request: EntityRequest) -> EntityResponse:
+    async def update(self, invoice_id: InvoiceId, *, request: InvoiceRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, entity_id: EntityId) -> EntityResponse:
+    async def delete(self, invoice_id: InvoiceId) -> None:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "DELETE",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+            )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def get_documents(self, invoice_id: InvoiceId) -> typing.List[DocumentResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/documents"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, entity_id: EntityId, *, request: EntityUpdateRequest) -> EntityResponse:
+    async def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/approve"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(EntityResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, entity_id: EntityId) -> None:
+    async def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> InvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "DELETE",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}"),
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/reject"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
-        if 200 <= _response.status_code < 300:
-            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_invoices(
-        self, entity_id: EntityId, *, status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]]
-    ) -> typing.List[InvoiceResponse]:
+    async def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
-                params={"status": status},
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[CommentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_invoice_metrics(
-        self,
-        entity_id: EntityId,
-        *,
-        status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-        due_date_start: typing.Optional[dt.datetime] = None,
-        due_date_end: typing.Optional[dt.datetime] = None,
-        created_date_start: typing.Optional[dt.datetime] = None,
-        created_date_end: typing.Optional[dt.datetime] = None,
-        currency: CurrencyCode,
-    ) -> InvoiceMetricsResponse:
+    async def add_comment(self, invoice_id: InvoiceId, *, request: CommentRequest) -> CommentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoice-metrics"),
-                params={
-                    "status": status,
-                    "dueDateStart": serialize_datetime(due_date_start) if due_date_start is not None else None,
-                    "dueDateEnd": serialize_datetime(due_date_end) if due_date_end is not None else None,
-                    "createdDateStart": serialize_datetime(created_date_start)
-                    if created_date_start is not None
-                    else None,
-                    "createdDateEnd": serialize_datetime(created_date_end) if created_date_end is not None else None,
-                    "currency": currency,
-                },
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceMetricsResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def accept_terms_of_service(self, entity_id: EntityId) -> str:
+    async def edit_comment(
+        self, invoice_id: InvoiceId, comment_id: CommentId, *, request: CommentRequest
+    ) -> CommentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_token(self, entity_id: EntityId) -> str:
+    async def delete_comment(self, invoice_id: InvoiceId, comment_id: CommentId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
-                "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/token"),
+                "DELETE",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comment/{comment_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def plaid_link_token(self, entity_id: EntityId) -> str:
+    async def get_vendor_link(self, invoice_id: InvoiceId) -> str:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/plaidLinkToken"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/vendorlink"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(str, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def send_vendor_email(self, invoice_id: InvoiceId) -> None:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/sendVendorEmail"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+            )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .account_type import AccountType
-from .business_profile_request import BusinessProfileRequest
-from .business_profile_response import BusinessProfileResponse
-from .business_type import BusinessType
-from .ein import Ein
-from .entity_id import EntityId
-from .entity_request import EntityRequest
-from .entity_response import EntityResponse
-from .entity_status import EntityStatus
-from .entity_update_request import EntityUpdateRequest
-from .individual_profile_request import IndividualProfileRequest
-from .individual_profile_response import IndividualProfileResponse
-from .invoice_metrics_response import InvoiceMetricsResponse
-from .profile_request import ProfileRequest
-from .profile_response import ProfileResponse
-from .tax_id import TaxID
+from .approval_request import ApprovalRequest
+from .approver import Approver
+from .approver_action import ApproverAction
+from .approver_response import ApproverResponse
+from .comment_id import CommentId
+from .comment_request import CommentRequest
+from .comment_response import CommentResponse
+from .create_vendor_request import CreateVendorRequest
+from .currency_code import CurrencyCode
+from .document_response import DocumentResponse
+from .invoice_id import InvoiceId
+from .invoice_line_item_request import InvoiceLineItemRequest
+from .invoice_line_item_response import InvoiceLineItemResponse
+from .invoice_order_by_field import InvoiceOrderByField
+from .invoice_request import InvoiceRequest
+from .invoice_response import InvoiceResponse
+from .invoice_status import InvoiceStatus
 
 __all__ = [
-    "AccountType",
-    "BusinessProfileRequest",
-    "BusinessProfileResponse",
-    "BusinessType",
-    "Ein",
-    "EntityId",
-    "EntityRequest",
-    "EntityResponse",
-    "EntityStatus",
-    "EntityUpdateRequest",
-    "IndividualProfileRequest",
-    "IndividualProfileResponse",
-    "InvoiceMetricsResponse",
-    "ProfileRequest",
-    "ProfileResponse",
-    "TaxID",
+    "ApprovalRequest",
+    "Approver",
+    "ApproverAction",
+    "ApproverResponse",
+    "CommentId",
+    "CommentRequest",
+    "CommentResponse",
+    "CreateVendorRequest",
+    "CurrencyCode",
+    "DocumentResponse",
+    "InvoiceId",
+    "InvoiceLineItemRequest",
+    "InvoiceLineItemResponse",
+    "InvoiceOrderByField",
+    "InvoiceRequest",
+    "InvoiceResponse",
+    "InvoiceStatus",
 ]
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/business_profile_request.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/business_profile_response.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/business_type.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/ein.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/entity_request.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/entity_response.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/entity_status.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/entity_update_request.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/individual_profile_request.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/individual_profile_response.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/invoice_metrics_response.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/invoice_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/profile_request.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/profile_response.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity/types/tax_id.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity_users/client.py` & `mercoa-0.1.0/src/mercoa/resources/entity_users/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_request.py` & `mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_response.py` & `mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .comment_id import CommentId
-from .comment_request import CommentRequest
-from .comment_response import CommentResponse
-from .create_vendor_request import CreateVendorRequest
-from .currency_code import CurrencyCode
-from .document_response import DocumentResponse
-from .invoice_id import InvoiceId
-from .invoice_line_item_request import InvoiceLineItemRequest
-from .invoice_line_item_response import InvoiceLineItemResponse
-from .invoice_request import InvoiceRequest
-from .invoice_response import InvoiceResponse
-from .invoice_status import InvoiceStatus
+from .types import (
+    ApprovalRequest,
+    Approver,
+    ApproverAction,
+    ApproverResponse,
+    CommentId,
+    CommentRequest,
+    CommentResponse,
+    CreateVendorRequest,
+    CurrencyCode,
+    DocumentResponse,
+    InvoiceId,
+    InvoiceLineItemRequest,
+    InvoiceLineItemResponse,
+    InvoiceOrderByField,
+    InvoiceRequest,
+    InvoiceResponse,
+    InvoiceStatus,
+)
 
 __all__ = [
+    "ApprovalRequest",
+    "Approver",
+    "ApproverAction",
+    "ApproverResponse",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "CreateVendorRequest",
     "CurrencyCode",
     "DocumentResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
+    "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
 ]
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_request.py` & `mercoa-0.1.0/src/mercoa/resources/process_invoice/types/process_invoice_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...invoice.types.invoice_id import InvoiceId
 
 
-class CommentRequest(pydantic.BaseModel):
-    text: str
+class ProcessInvoiceRequest(pydantic.BaseModel):
+    invoice_ids: typing.List[InvoiceId] = pydantic.Field(alias="invoiceIds")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_response.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class CommentResponse(pydantic.BaseModel):
-    id: str
-    text: str
+class EmailLogResponse(pydantic.BaseModel):
+    from_: str = pydantic.Field(alias="from")
+    to: str
+    subject: str
+    raw_content: str = pydantic.Field(alias="rawContent")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/create_vendor_request.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/create_vendor_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/currency_code.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/document_response.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_line_item_request.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_line_item_response.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_line_item_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_request.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...entity.types.entity_id import EntityId
+from ...entity_users.types.entity_user_id import EntityUserId
 from ...payment_method.types.payment_method_id import PaymentMethodId
 from .create_vendor_request import CreateVendorRequest
 from .currency_code import CurrencyCode
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceRequest(pydantic.BaseModel):
     status: typing.Optional[InvoiceStatus]
     amount: typing.Optional[float]
     currency: typing.Optional[CurrencyCode]
+    invoice_date: typing.Optional[dt.datetime] = pydantic.Field(
+        alias="invoiceDate", description=("Date the invoice was created.\n")
+    )
     deduction_date: typing.Optional[dt.datetime] = pydantic.Field(
         alias="deductionDate", description=("Date when funds will be deducted from payer's account.\n")
     )
     funded_date: typing.Optional[dt.datetime] = pydantic.Field(
         alias="fundedDate", description=("Date of funds settlement.\n")
     )
     due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate", description=("Due date of invoice.\n"))
@@ -42,18 +46,26 @@
     update_vendor: typing.Optional[CreateVendorRequest] = pydantic.Field(
         alias="updateVendor",
         description=(
             "When paying to an existing vendor with an incomplete profile, use the updateVendor object. Mercoa will update the vendor entity tied to this invoice. This object is ignored if the vendor already has already been created with complete information and when creating a new invoice.\n"
         ),
     )
     line_items: typing.Optional[typing.List[InvoiceLineItemRequest]] = pydantic.Field(alias="lineItems")
+    metadata: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
+        description=(
+            "Metadata associated with this invoice. You can specify up to 10 keys, with key names up to 40 characters long and values up to 200 characters long.\n"
+        )
+    )
     uploaded_image: typing.Optional[str] = pydantic.Field(
         alias="uploadedImage",
         description=("Base64 encoded image or PDF of invoice. PNG, JPG, and PDF are supported. 10MB max.\n"),
     )
+    created_by_id: typing.Optional[EntityUserId] = pydantic.Field(
+        alias="createdById", description=("ID of entity user who created this invoice.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_response.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,46 +4,63 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...entity.types.entity_id import EntityId
 from ...entity.types.entity_response import EntityResponse
+from ...entity_users.types.entity_user_response import EntityUserResponse
 from ...payment_method.types.payment_method_id import PaymentMethodId
 from ...payment_method.types.payment_method_response import PaymentMethodResponse
 from ...transaction.types.transaction_response import TransactionResponse
+from .approver import Approver
+from .comment_response import CommentResponse
 from .currency_code import CurrencyCode
 from .invoice_id import InvoiceId
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceResponse(pydantic.BaseModel):
     id: InvoiceId
     status: InvoiceStatus
     amount: typing.Optional[float]
     currency: typing.Optional[CurrencyCode]
-    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
-    funded_date: typing.Optional[dt.datetime] = pydantic.Field(alias="fundedDate")
-    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
+    invoice_date: typing.Optional[dt.datetime] = pydantic.Field(
+        alias="invoiceDate", description=("Date the invoice was created.\n")
+    )
+    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(
+        alias="deductionDate", description=("Date when funds will be deducted from payer's account.\n")
+    )
+    funded_date: typing.Optional[dt.datetime] = pydantic.Field(
+        alias="fundedDate", description=("Date of funds settlement.\n")
+    )
+    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate", description=("Due date of invoice.\n"))
     invoice_number: typing.Optional[str] = pydantic.Field(alias="invoiceNumber")
     note_to_self: typing.Optional[str] = pydantic.Field(alias="noteToSelf")
     service_start_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceStartDate")
     service_end_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceEndDate")
     payer_id: typing.Optional[EntityId] = pydantic.Field(alias="payerId")
     payer: typing.Optional[EntityResponse]
     payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
     payment_source_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentSourceId")
     vendor_id: typing.Optional[EntityId] = pydantic.Field(alias="vendorId")
     vendor: typing.Optional[EntityResponse]
     payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
     payment_destination_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentDestinationId")
     payment_destination_confirmed: bool = pydantic.Field(alias="paymentDestinationConfirmed")
+    has_documents: bool = pydantic.Field(alias="hasDocuments")
+    comments: typing.Optional[typing.List[CommentResponse]]
     transactions: typing.Optional[typing.List[TransactionResponse]]
     line_items: typing.Optional[typing.List[InvoiceLineItemResponse]] = pydantic.Field(alias="lineItems")
+    approvers: typing.List[Approver]
+    metadata: typing.Dict[str, str] = pydantic.Field(description=("Metadata associated with this invoice.\n"))
+    created_by: typing.Optional[EntityUserResponse] = pydantic.Field(
+        alias="createdBy", description=("Entity user who created this invoice.\n")
+    )
     processed_at: typing.Optional[dt.datetime] = pydantic.Field(alias="processedAt")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_status.py` & `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/ocr/client.py` & `mercoa-0.1.0/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/ocr/types/attachments.py` & `mercoa-0.1.0/src/mercoa/resources/ocr/types/attachments.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/ocr/types/email_ocr_request.py` & `mercoa-0.1.0/src/mercoa/resources/ocr/types/email_ocr_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/ocr/types/ocr_mailbox.py` & `mercoa-0.1.0/src/mercoa/resources/ocr/types/ocr_mailbox.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.1.0/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/client.py` & `mercoa-0.1.0/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/color_scheme_request.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/color_scheme_response.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .email_sender_provider import EmailSenderProvider
 
 
-class EmailLogResponse(pydantic.BaseModel):
-    from_: str = pydantic.Field(alias="from")
-    to: str
-    subject: str
-    raw_content: str = pydantic.Field(alias="rawContent")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+class EmailSenderRequest(pydantic.BaseModel):
+    provider: EmailSenderProvider
+    from_email: str = pydantic.Field(alias="fromEmail")
+    from_name: str = pydantic.Field(alias="fromName")
+    api_key: typing.Optional[str] = pydantic.Field(alias="apiKey")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_update_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_sender_provider import EmailSenderProvider
+from .custom_payment_method_update_request import CustomPaymentMethodUpdateRequest
 
 
-class EmailSenderRequest(pydantic.BaseModel):
-    provider: EmailSenderProvider
-    from_email: str = pydantic.Field(alias="fromEmail")
-    from_name: str = pydantic.Field(alias="fromName")
-    api_key: typing.Optional[str] = pydantic.Field(alias="apiKey")
+class PaymentMethodUpdateRequest(pydantic.BaseModel):
+    custom: typing.Optional[CustomPaymentMethodUpdateRequest]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 from ....core.datetime_utils import serialize_datetime
 from .payment_rail_request import PaymentRailRequest
 
 
 class PaymentRailResponse(PaymentRailRequest):
-    avaliable: bool
+    available: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,18 +13,20 @@
     CardType,
     CheckId,
     CheckRequest,
     CheckResponse,
     CustomId,
     CustomPaymentMethodRequest,
     CustomPaymentMethodResponse,
+    CustomPaymentMethodUpdateRequest,
     PaymentMethodId,
     PaymentMethodRequest,
     PaymentMethodResponse,
     PaymentMethodType,
+    PaymentMethodUpdateRequest,
 )
 
 __all__ = [
     "BankAccountId",
     "BankAccountRequest",
     "BankAccountResponse",
     "BankStatus",
@@ -36,12 +38,14 @@
     "CardType",
     "CheckId",
     "CheckRequest",
     "CheckResponse",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
+    "CustomPaymentMethodUpdateRequest",
     "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodResponse",
     "PaymentMethodType",
+    "PaymentMethodUpdateRequest",
 ]
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/client.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..entity.types.entity_id import EntityId
 from .types.payment_method_id import PaymentMethodId
 from .types.payment_method_request import PaymentMethodRequest
 from .types.payment_method_response import PaymentMethodResponse
 from .types.payment_method_type import PaymentMethodType
+from .types.payment_method_update_request import PaymentMethodUpdateRequest
 
 
 class PaymentMethodClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
@@ -78,14 +79,35 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def update(
+        self, entity_id: EntityId, payment_method_id: PaymentMethodId, *, request: PaymentMethodUpdateRequest
+    ) -> PaymentMethodResponse:
+        _response = httpx.request(
+            "PUT",
+            urllib.parse.urljoin(
+                f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
+            ),
+            json=jsonable_encoder(request),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+        )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def delete(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
             ),
             headers=remove_none_from_headers(
@@ -198,14 +220,36 @@
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def update(
+        self, entity_id: EntityId, payment_method_id: PaymentMethodId, *, request: PaymentMethodUpdateRequest
+    ) -> PaymentMethodResponse:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "PUT",
+                urllib.parse.urljoin(
+                    f"{self._environment.value}/", f"entity/{entity_id}/paymentMethod/{payment_method_id}"
+                ),
+                json=jsonable_encoder(request),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PaymentMethodResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, entity_id: EntityId, payment_method_id: PaymentMethodId) -> None:
         async with httpx.AsyncClient() as _client:
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 from .card_type import CardType
 from .check_id import CheckId
 from .check_request import CheckRequest
 from .check_response import CheckResponse
 from .custom_id import CustomId
 from .custom_payment_method_request import CustomPaymentMethodRequest
 from .custom_payment_method_response import CustomPaymentMethodResponse
+from .custom_payment_method_update_request import CustomPaymentMethodUpdateRequest
 from .payment_method_id import PaymentMethodId
 from .payment_method_request import PaymentMethodRequest
 from .payment_method_response import PaymentMethodResponse
 from .payment_method_type import PaymentMethodType
+from .payment_method_update_request import PaymentMethodUpdateRequest
 
 __all__ = [
     "BankAccountId",
     "BankAccountRequest",
     "BankAccountResponse",
     "BankStatus",
     "BankType",
@@ -34,12 +36,14 @@
     "CardType",
     "CheckId",
     "CheckRequest",
     "CheckResponse",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
+    "CustomPaymentMethodUpdateRequest",
     "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodResponse",
     "PaymentMethodType",
+    "PaymentMethodUpdateRequest",
 ]
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_request.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_response.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_status.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_type.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_brand.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_request.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_response.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_type.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_request.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_response.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_payment_method_request.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_payment_method_response.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_request.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_response.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_type.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/__init__.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py` & `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/process_invoice/client.py` & `mercoa-0.1.0/src/mercoa/resources/process_invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/process_invoice/types/process_invoice_request.py` & `mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...invoice.types.invoice_id import InvoiceId
+from .policy_id import PolicyId
+from .rule import Rule
+from .trigger import Trigger
 
 
-class ProcessInvoiceRequest(pydantic.BaseModel):
-    invoice_ids: typing.List[InvoiceId] = pydantic.Field(alias="invoiceIds")
+class ApprovalPolicyRequest(pydantic.BaseModel):
+    trigger: Trigger
+    rule: Rule
+    upstream_policy_id: PolicyId = pydantic.Field(
+        alias="upstreamPolicyId", description=("Use 'root' if no upstreamPolicyId is intended to be set.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.9/src/mercoa/resources/representative/client.py` & `mercoa-0.1.0/src/mercoa/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/representative/types/representative_request.py` & `mercoa-0.1.0/src/mercoa/resources/representative/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/representative/types/representative_response.py` & `mercoa-0.1.0/src/mercoa/resources/representative/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/representative/types/responsibilities.py` & `mercoa-0.1.0/src/mercoa/resources/representative/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/transaction/client.py` & `mercoa-0.1.0/src/mercoa/resources/transaction/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_response.py` & `mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_response_expanded.py` & `mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.9/PKG-INFO` & `mercoa-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.0.9
+Version: 0.1.0
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

